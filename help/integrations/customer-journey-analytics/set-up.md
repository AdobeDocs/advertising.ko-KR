---
title: 데이터 수집, 데이터 전송 및 보고 설정
description: 데이터 수집, 데이터 전송 및 보고를 설정하는 방법에 대해 알아봅니다.
feature: Integration with Adobe Customer Journey Analytics
source-git-commit: 2d6cba8d5a3d966b272c5048404ac8fdf0185b74
workflow-type: tm+mt
source-wordcount: '1236'
ht-degree: 0%

---

# 데이터 수집, 데이터 전송 및 보고 설정

*Beta 기능*

Customer Journey Analytics에서 Advertising Cloud 데이터를 보려면 다음 작업이 필요합니다.

1. (조직의 웹 분석가, 선택 사항) [AMO ID 및 EF ID에 대한 내역 데이터를 수집합니다](/help/integrations/analytics/rvars-to-evars.md){target="_blank"}.

   이 단계는 [!DNL Analytics for Advertising]을(를) 사용하는 광고주에만 적용됩니다.

1. (조직의 Adobe Experience Platform 사이트 관리자) [Experience Platform에서 데이터 수집을 설정하고 전환 추적 태그를 구현합니다](#data-collection).

1. (조직의 Customer Journey Analytics 사이트 관리자) [Customer Journey Analytics에서 Experience Platform 데이터 세트에 대한 연결을 만듭니다](#dataset-connection).

1. (조직의 웹 분석가) [Customer Journey Analytics에서 데이터 보기 설정](#cja-data-views).

1. (조직의 웹 분석가) [Customer Journey Analytics Workspace에서 보고서 및 시각화를 설정](#cja-reports)합니다.

다음 섹션에는 통합에 필요한 작업 및 설정을 포함하지만 워크플로우에서 사용할 수 있는 모든 기능을 설명하지는 않는 세부 절차가 포함되어 있습니다. 자세한 내용은 연결된 리소스를 참조하십시오.

## Adobe Experience Platform 및 웹 사이트에서 데이터 수집 설정 {#data-collection}

Experience Platform에서 데이터 수집을 설정하고 전환 추적 태그를 구현하는 데 다음 작업이 필요합니다. 조직의 Experience Platform 사이트 관리자가 이러한 작업을 수행할 수 있지만, 조직의 IT 부서에서 추적 태그를 배포해야 할 수 있습니다.

1. Adobe Advertising에서 Experience Platform Edge Network으로 데이터를 수집하여 데이터 세트로 보냅니다.

   1. Experience Platform에서 XDM(Experience Data Model)을 사용하여 수집할 데이터에 대해 [수동 스키마를 정의](https://experienceleague.adobe.com/ko/docs/experience-platform/xdm/ui/resources/schemas)합니다.

      * [!UICONTROL Schema Details]에서 사이트 이벤트를 캡처할 스키마의 기본 클래스로 **[!UICONTROL Experience Event]**&#x200B;을(를) 선택합니다. 스키마 이름을 지정하고 **[!UICONTROL Finish]**&#x200B;을(를) 클릭합니다.

      * 왼쪽 패널에서 필드 그룹 `Adobe Advertising Cloud ExperienceEvent Full Extension`을(를) 추가하여 Adobe Advertising 관련 필드를 추가합니다.<!-- Add link once published --> 최소한 `trackingCode`AMO ID 및 EF ID`trackingIdentities`를 포함하는 [ 및 ](ids.html) 속성으로 conversionDetails 개체를 포함하십시오. 다른 필드는 선택 사항입니다.

      * (선택 사항) 필요에 따라 추가 데이터 필드를 Adobe Advertising 데이터에 연결하는 데 추가 필드 그룹을 추가합니다.

      **참고:** 여러 개의 스키마를 만들 수 있지만 데이터 세트 및 데이터 스트림당 하나의 스키마만 사용할 수 있습니다. 다음 단계에서 만들 수 있습니다.

   1. 이벤트 데이터 컬렉션을 저장 및 관리하려면 스키마를 기반으로 [데이터 집합을 만듭니다](https://experienceleague.adobe.com/ko/docs/experience-platform/catalog/datasets/create).

      * **[!UICONTROL Create dataset from schema]** 옵션을 선택하고 스키마를 선택하세요.

        Adobe Advertising은 이벤트 데이터 세트를 기반으로 관련 요약 지표 데이터(예: 전환 값) 및 조회 데이터(차원/분류 메타데이터(예: Adobe Advertising 캠페인 이름)에 대한 추가 데이터 세트를 만듭니다. 데이터 세트에 대한 데이터는 Experience Platform에서 매일 채워집니다.

   1. 스키마에 대한 [데이터 스트림을 만듭니다](https://experienceleague.adobe.com/ko/docs/experience-platform/datastreams/configure).

      * [!UICONTROL Mapping schema] 설정에 대해 스키마를 선택합니다.

      * `Adobe Advertising` 및 `Adobe Experience Platform` 서비스를 데이터 스트림에 추가하고 사용하도록 설정합니다.

        이러한 서비스를 통해 Edge Network은 데이터 세트를 저장하고 Adobe Advertising으로 라우팅할 수 있습니다.

      * [!UICONTROL Event dataset] 설정에 대해 데이터 세트를 선택하십시오.

        각 데이터 스트림은 하나의 데이터 세트에만 데이터를 삽입할 수 있습니다.

1. 조직의 웹 사이트 데이터를 Experience Platform 데이터 스트림으로 보냅니다.

   1. Experience Platform [tags](https://experienceleague.adobe.com/ko/docs/experience-platform/tags/home)&#x200B;(이전 이름: [!DNL Launch])을(를) 사용하여 조직의 웹 사이트 데이터를 데이터 스트림으로 보낼 JavaScript 태그를 생성합니다.

      * 태그 구성의 컨테이너인 태그 속성을 만듭니다.

      * 속성의 경우 확장 카탈로그에서 [확장 &quot;Adobe Experience Platform Web SDK&quot;를 설치](https://experienceleague.adobe.com/ko/docs/experience-platform/tags/extensions/client/web-sdk/web-sdk-extension-configuration)합니다.

        이 확장은 웹 속성의 데이터를 Experience Platform Edge Network을 통해 Experience Cloud으로 보냅니다.

        Adobe Advertising 확장 기능을 사용하지 마십시오.

      * 사용자 지정 웹 SDK 빌드 만들기:

         * [!UICONTROL Custom build components] 섹션에서 **Advertising** 구성 요소를 사용하도록 설정합니다.

           이 구성 요소에는 태그에 Adobe Advertising에 필요한 모든 JavaScript 코드가 포함되어 있습니다. 또한 태그 규칙(선택 사항)에 &quot;Advertising&quot; 설정을 추가하여 속성 측정에 광고 데이터를 사용하는 방법을 정의합니다.

           필요에 따라 추가 구성 요소를 활성화할 수 있습니다.

         * [!UICONTROL SDK Instances] 섹션에서:

            * [!UICONTROL Datastreams] 설정에서 각 웹 환경(프로덕션, 스테이징, 개발)에 사용할 데이터 스트림을 선택합니다.

            * (Adobe Advertising DSP을 사용하는 조직만 해당) [!UICONTROL Adobe Advertising] 설정에서:

               * 뷰스루 추적을 사용하려면 **[!UICONTROL Adobe Advertising DSP]** 설정을 활성화하십시오.

               * 뷰스루 추적을 활성화할 광고주를 지정합니다.

               * (선택 사항) ID를 수집하려면 조직의 ID5 파트너 ID를 입력합니다.

               * (선택 사항) ID를 수집하려면 조직의 [!DNL LiveRamp RampID] JavaScript 코드(ats.js)에 대한 경로를 입력합니다.

            * 빌드를 저장합니다.

      * (선택 사항) Web SDK에서 Edge Network으로 데이터를 보내야 하는 시기를 결정하는 데 필요한 경우 [규칙을 만듭니다](https://experienceleague.adobe.com/ko/docs/experience-platform/tags/ui/rules).

         * [!UICONTROL Advertising] 설정의 경우 속성 측정에 광고 데이터를 사용하는 방법을 정의합니다. 이 설정은 규칙에 여러 작업의 시퀀스가 포함되어 있을 때 유용하며 사용자 지정 빌드 구성 요소에 대해 &quot;[!UICONTROL Advertising]&quot; 구성 요소를 선택한 경우에만 사용할 수 있습니다. 옵션은 다음과 같습니다.

           *자동:* 캐시의 데이터를 기반으로 현재 `sendEvent` 작업에서 광고 속성을 측정하는 데 광고 데이터를 사용할 수 있습니다. 이 경우 광고 노출 이벤트는 기회가 있을 때 실행되며, 현재 이벤트에는 사용할 수 없습니다. 예를 들어 구매 체크아웃 이벤트를 실행하고 캐시에서 사용 가능한 광고 노출 데이터가 없는 경우, 체크아웃 이벤트는 광고 노출로 인한 것이 아닙니다.

           *대기:* 광고 데이터가 서버에서 성공적으로 검색되고 해결될 때까지 호출 실행을 지연시켜 정확한 속성 측정을 보장합니다. 예를 들어 구매 체크아웃 이벤트를 실행하기 전에 광고 노출 이벤트가 해결될 때까지 기다리려고 할 수 있습니다. **참고:** 확인 ID는 브라우저 및 ID 유형에 따라 몇 초 정도 걸릴 수 있습니다. 현재 `sendEvent` 작업에서 몇 초의 지연을 수용할 수 있는 경우 이 옵션을 사용합니다.

           *사용 안 함:*(기본값) 실행 중인 요청에서 광고 데이터를 제외하여 속성 또는 관련 추적에 사용할 수 없게 합니다.

           *데이터 요소를 제공합니다.* 페이지를 로드하는 동안 광고 데이터를 포함하거나 제외하려면 데이터 요소를 사용하십시오. 데이터 요소에 대해 확인된 값에는 `automatic`, `wait` 및 `disabled`이(가) 포함될 수 있습니다. 다음 단계를 참조하십시오.

        규칙을 사용하여 `sendEvent` 작업을 구성하지 않으면 광고 데이터가 별도의 광고 데이터 보강 이벤트로 전송됩니다.

      * 필요에 따라 웹 사이트의 변수를 이전에 만든 XDM 스키마의 구조에 매핑하는 [데이터 요소](https://experienceleague.adobe.com/ko/docs/experience-platform/tags/ui/data-elements)를 만듭니다.

   1. 태그 개발을 반복할 수 있는 테스트 환경에 [태그를 게시](https://experienceleague.adobe.com/ko/docs/experience-platform/tags/publish/publishing-flow)합니다.

   1. 데이터 세트 배달의 유효성을 검사한 다음 [태그를 라이브 프로덕션 환경에 게시](https://experienceleague.adobe.com/ko/docs/experience-platform/tags/publish/publishing-flow)합니다.

      조직의 IT 부서나 다른 그룹은 태그 배포를 예약하거나 그에 대한 정보를 받아야 할 수 있습니다.

## Customer Journey Analytics에서 Experience Platform 데이터 세트에 대한 연결 만들기 {#dataset-connection}

다음 단계에 따라 Experience Platform 데이터 세트에서 Adobe Advertising으로 Customer Journey Analytics 데이터를 가져옵니다. Customer Journey Analytics에 대한 조직의 사이트 관리자가 이러한 작업을 수행할 수 있습니다.

*준비 중*

## Customer Journey Analytics에서 데이터 보기 설정 {#cja-data-views}

Customer Journey Analytics에서 하나 이상의 데이터 보기를 만들어 보고를 위한 지표 및 차원을 정의합니다. 웹 분석가는 이러한 작업을 수행할 수 있습니다.

*준비 중*

## Customer Journey Analytics Workspace에서 보고서 및 시각화 설정 {#cja-reports}

Customer Journey Analytics Workspace에서 다음 단계에 따라 보고서 및 시각화를 구성합니다. 웹 분석가는 이러한 작업을 수행할 수 있습니다.

1. 데이터 보기 내에 구성된 차원 및 지표를 기반으로 보고서와 시각화를 빌드하려면 Workspace에서 [프로젝트를 만듭니다](https://experienceleague.adobe.com/ko/docs/analytics-platform/using/cja-workspace/build-workspace-project/create-projects).

1. ([!DNL Google Ads] 또는 [!DNL Microsoft Advertising]의 데이터가 있는 경우) 광고 네트워크별 지표에 대해 `googleConversions` 및 `microsoftConversions`(으)로 그룹화된 필드를 사용하여 게시자가 추적한 전환 보고서를 만듭니다.

>[!MORELIKETHIS]
>
>* [개요](overview.md)
>* [필수 구성 요소](prerequisites.md)
>* [사용한 Adobe Advertising ID [!DNL Customer Journey Analytics]](ids.md)
>* [Customer Journey Analytics의 Adobe Advertising 지표 및 차원](advertising-data-in-cja.md)
>* [Adobe Customer Journey Analytics에서 사용할 AMO ID 및 EF ID에 대한 내역 데이터 수집](/help/integrations/analytics/rvars-to-evars.md).
>* [Customer Journey Analytics 안내서](https://experienceleague.adobe.com/ko/docs/analytics-platform/using/cja-landing)
>* Customer Journey Analytics [Adobe Analytics 사용자를 위한 사용 안내서](https://experienceleague.adobe.com/ko/docs/analytics-platform/using/compare-aa-cja/aa-to-cja-user)
