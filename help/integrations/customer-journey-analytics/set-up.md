---
title: 데이터 수집, 데이터 전송 및 보고 설정
description: 데이터 수집, 데이터 전송 및 보고를 설정하는 방법에 대해 알아봅니다.
feature: Integration with Adobe Customer Journey Analytics
exl-id: a955e2b0-ea1b-4b5c-937b-f8c66603cd36
TQID: https://experienceleague.adobe.com/u6xL6FuW-TwqAkse3VTS3zcyt-10Cv-ADTZLJTiWWT8
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2:
  - id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
  - id: d3cdead0-685a-4489-9250-4bb709942f66
source-git-commit: ede5b5b1eb8ab449b982fdadba93e944cd2e062f
workflow-type: tm+mt
source-wordcount: 2103
ht-degree: 1%

---

# 데이터 수집, 데이터 전송 및 보고 설정

*Advertising DSP 및[!DNL Advertising Search, Social, & Commerce]*&#x200B;을(를) 사용하는 광고주

*[!DNL Analytics for Advertising]이(가) 없는 광고주*

<!-- may need to remove references to Experience Platform if it's not really required, just Data Collection? In that case, I may need to change all of the links accordingly.... -->

[Adobe Experience Platform [!DNL Web SDK]](https://experienceleague.adobe.com/docs/experience-platform/edge/home.html)을(를) 사용하여 Adobe Advertising과 Customer Journey Analytics 간에 기본적으로 데이터를 교환하려면 다음 작업이 필요합니다. 데이터 전송 및 속성은 론치 후에 시작되며 내역 데이터는 포함되지 않습니다.

[!DNL Analytics for Advertising]을(를) 사용하는 광고주에게는 이러한 작업이 필요하지 않습니다.

1. (조직의 Adobe Experience Platform 사이트 관리자) [Experience Platform에서 데이터 수집을 설정하고 전환 추적 태그를 구현합니다](#data-collection).

1. (조직의 Customer Journey Analytics 사이트 관리자) [Customer Journey Analytics에서 Experience Platform 데이터 세트에 대한 연결을 만듭니다](#dataset-connection).

1. (조직의 웹 분석가) [Customer Journey Analytics에서 데이터 보기 설정](#cja-data-views).

1. (조직의 웹 분석가) [Customer Journey Analytics Workspace에서 보고서 및 시각화를 설정](#cja-reports)합니다.

다음 섹션에는 통합에 필요한 작업 및 설정을 포함하지만 워크플로우에서 사용할 수 있는 모든 기능을 설명하지는 않는 세부 절차가 포함되어 있습니다. 자세한 내용은 연결된 리소스를 참조하십시오.

## Adobe Experience Platform 및 웹 사이트에서 데이터 수집 설정 {#data-collection}

Experience Platform에서 데이터 수집을 설정하고 전환 추적 태그를 구현하는 데 다음 작업이 필요합니다. 조직의 Experience Platform 사이트 관리자가 이러한 작업을 수행할 수 있지만, 조직의 IT 부서에서 추적 태그를 배포해야 할 수 있습니다.

### Adobe Advertising에서 데이터를 수집하여 Experience Platform Edge Network에 데이터 세트로 전송합니다 {#dataset-datastream}

이 절차에는 스키마 생성이 포함됩니다. 대신 선택적으로 기존 스키마를 편집할 수 있습니다. 이 경우 데이터 세트 또는 데이터 스트림을 만들 필요가 없습니다.

1. 데이터 수집 인터페이스에서 XDM(Experience Data Model)을 사용하여 수집할 웹 사이트 데이터에 대한 [스키마를 정의](https://experienceleague.adobe.com/en/docs/platform-learn/implement-web-sdk/initial-configuration/configure-schemas)합니다.

   웹 사이트 데이터에 대한 스키마가 이미 있는 경우 다음 설정으로 대신 사용할 수 있습니다.

   * [!UICONTROL Schema Details]에서 사이트 이벤트를 캡처할 스키마의 기본 클래스로 **[!UICONTROL Experience Event]**&#x200B;을(를) 선택합니다. 스키마 이름을 지정하고 **[!UICONTROL Finish]**&#x200B;을(를) 클릭합니다.

   * 왼쪽 패널에서 필드 그룹 [Adobe Advertising Cloud ExperienceEvent 전체 확장](https://experienceleague.adobe.com/en/docs/experience-platform/xdm/field-groups/event/advertising-full-extension)을(를) 추가하여 Adobe Advertising 관련 필드를 추가합니다. 최소한 [AMO ID 및 EF ID](ids.md)를 포함하는 `trackingCode` 및 `trackingIdentities` 속성이 있는 conversionDetails 개체를 포함하십시오. 다른 필드는 선택 사항입니다. 다른 구성은 필요하지 않습니다.

   * (선택 사항) 필요에 따라 추가 데이터 필드를 Adobe Advertising 데이터에 연결하는 데 추가 필드 그룹을 추가합니다.

   **참고:** 여러 개의 스키마를 만들 수 있지만 데이터 세트 및 데이터 스트림당 하나의 스키마만 사용할 수 있습니다. 다음 단계에서 만들 수 있습니다.

1. 이벤트 데이터 컬렉션을 저장 및 관리하려면 스키마를 기반으로 [데이터 집합을 만듭니다](https://experienceleague.adobe.com/en/docs/experience-platform/catalog/datasets/create). *이벤트 데이터 세트*&#x200B;가 됩니다. 데이터 세트로 기존 스키마를 편집하는 경우 이 단계를 건너뛸 수 있습니다.

   * **[!UICONTROL Create dataset from schema]** 옵션을 선택하고 스키마를 선택하세요.

     Adobe Advertising은 이벤트 데이터 세트를 기반으로 두 개의 추가 데이터 세트를 만듭니다. 1\) 관련 요약 데이터(예: 집계된 클릭 수 및 집계된 노출 수)가 포함된 *요약 데이터 세트* 및 2\) *조회 데이터 세트*(Adobe Advertising 캠페인 이름과 같은 차원/분류 메타데이터 포함). 데이터 세트에 대한 데이터는 Experience Platform에서 매일 채워집니다.

   >[!TIP]
   >
   >프로덕션 데이터 세트를 사용하기 전에 데이터 흐름을 확인하기 위해 먼저 더미 이벤트 데이터 세트를 만듭니다.

1. [데이터 스트림을 만들어](https://experienceleague.adobe.com/en/docs/experience-platform/datastreams/configure) 웹 사이트 또는 앱에서 데이터를 보낼 위치와 들어오는 데이터를 처리하는 방법을 지정합니다.

   * [!UICONTROL Mapping schema] 설정의 경우 1단계에서 만든 스키마를 선택합니다.

   * `Adobe Advertising` 및 `Adobe Experience Platform` 서비스를 데이터 스트림에 추가하고 사용하도록 설정합니다.

     [!UICONTROL Adobe Advertising] 서비스를 사용하면 광고 노출을 페이로드와 연결할 수 있고, [!UICONTROL Adobe Experience Platform]을(를) 사용하면 Edge Network이 데이터 세트를 저장하고 Adobe Advertising으로 라우팅할 수 있습니다.

   * [!UICONTROL Event dataset] 설정의 경우 이벤트 데이터 세트를 선택하십시오.

     각 데이터 스트림은 하나의 데이터 세트에만 데이터를 삽입할 수 있습니다.

### 조직의 웹 사이트 데이터를 <!-- ?? -->Experience Platform 데이터스트림 {#tags-websdk}(으)로 보내기

Adobe Tags의 Adobe Experience Platform Web SDK 확장 기능을 사용하여 조직의 웹 사이트 데이터를 Experience Platform 데이터스트림으로 전송합니다.

>[!NOTE]
>
>Adobe 태그만 지원됩니다. 독립 실행형 Experience Platform Web SDK(`alloy.js`) 또는 타사 태그 관리자에 대해서는 지원을 사용할 수 없습니다.

1. Experience Platform [tags](https://experienceleague.adobe.com/en/docs/experience-platform/tags/home)&#x200B;(이전 이름: [!DNL Launch])을(를) 사용하여 조직의 웹 사이트 데이터를 데이터 스트림으로 보낼 JavaScript 태그를 생성합니다.

   * 태그 구성의 컨테이너인 태그 속성을 만듭니다.

   * 속성의 경우 확장 카탈로그에서 [확장 &quot;Adobe Experience Platform Web SDK&quot;를 설치](https://experienceleague.adobe.com/en/docs/experience-platform/tags/extensions/client/web-sdk/web-sdk-extension-configuration)합니다.

     이 확장은 Experience Platform Edge Network을 통해 웹 속성에서 Adobe CX Enterprise로 데이터를 전송합니다.

     Adobe Advertising 확장 기능을 사용하지 마십시오.

   * [사용자 지정 웹 SDK 빌드](https://experienceleague.adobe.com/en/docs/experience-platform/tags/extensions/client/web-sdk/web-sdk-extension-configuration#custom-build) 만들기:

      * [!UICONTROL Custom build components] 섹션에서 **Advertising** 구성 요소를 사용하도록 설정합니다.

        이 구성 요소에는 태그의 Adobe Advertising에 필요한 모든 JavaScript 코드가 포함되어 있으며 Advertising DSP 및 Advertising 검색, 소셜, Commerce 고객 모두에게 필요합니다. 또한 구성 요소는 태그 규칙(선택 사항)에 &quot;Advertising&quot; 설정을 추가하여 속성 측정에 광고 데이터를 사용하는 방법을 정의합니다.

        필요에 따라 추가 구성 요소를 활성화할 수 있습니다.

      * [!UICONTROL SDK Instances] 섹션에서:

         * [!UICONTROL Datastreams] 설정에서 각 웹 환경(프로덕션, 스테이징, 개발)에 사용할 데이터 스트림을 선택합니다.

         * (Adobe Advertising DSP을 사용하는 조직만 해당) [[!UICONTROL Adobe Advertising] 설정](https://experienceleague.adobe.com/en/docs/experience-platform/tags/extensions/client/web-sdk/configure/advertising)에서 **[!UICONTROL Adobe Advertising DSP]**&#x200B;을(를) 사용하여 뷰스루 추적을 허용하고 뷰스루 추적을 활성화할 광고주를 지정하십시오. 필요에 따라 조직의 ID5 파트너 ID 및/또는 [!DNL RampIDs]에 대한 조직의 [!DNL LiveRamp] [!DNL LaunchPad] JavaScript 코드(ats.js)에 대한 경로를 추가하여 유니버설 ID([자사 대상 소스](/help/dsp/audiences/sources/source-about.md)에서 번역됨)에서 ID를 수집할 수 있습니다.

           광고주가 나열되지 않은 경우 각 광고주에 대한 광고주 ID를 입력합니다. 필요한 경우 Adobe 계정 팀에 ID를 문의하십시오.

           잘못된 ID를 입력하면 Adobe 계정 팀에 알림이 표시됩니다.

           [!DNL RampID] JavaScript 경로의 예: `https://launchpad-wrapper.privacymanager.io/<customer-specific-id>/launchpad-liveramp.js`

         * 빌드를 저장합니다.

   * (선택 사항) Web SDK에서 Edge Network으로 데이터를 보내야 하는 시기를 결정하는 데 필요한 경우 [규칙을 만듭니다](https://experienceleague.adobe.com/en/docs/experience-platform/tags/ui/rules).

      * `[sendEvent](https://experienceleague.adobe.com/en/docs/experience-platform/tags/extensions/client/web-sdk/actions/send-event)` 작업의 경우 [[!UICONTROL Advertising] 설정](https://experienceleague.adobe.com/en/docs/experience-platform/tags/extensions/client/web-sdk/action-types#advertising)을(를) 사용하여 속성 측정에 광고 데이터를 사용하는 방법을 정의합니다. 이 설정은 규칙에 여러 작업의 시퀀스가 포함되어 있을 때 유용하며 사용자 지정 빌드 구성 요소에 대해 &quot;[!UICONTROL Advertising]&quot; 구성 요소를 선택한 경우에만 사용할 수 있습니다.

   * 필요에 따라 웹 사이트의 변수를 이전에 만든 XDM 스키마의 구조에 매핑하는 [데이터 요소](https://experienceleague.adobe.com/en/docs/experience-platform/tags/ui/data-elements)를 만듭니다.

1. Adobe Experience Platform 관리자에게 태그를 [테스트 환경에 게시](https://experienceleague.adobe.com/en/docs/experience-platform/tags/publish/publishing-flow)하도록 요청하십시오. 이렇게 하면 태그 개발을 반복적으로 수행할 수 있습니다.

### 데이터 게재 유효성 검사

1. Adobe 계정 팀에 요청하여 웹 사이트에서 추적을 확인합니다.

   ![클릭스루 추적 페이로드 유효성 검사의 예](/help/integrations/assets/cja-example-click-through-validation.png "클릭스루 추적 페이로드 유효성 검사의 예")

   ![뷰스루 추적 페이로드 유효성 검사의 예](/help/integrations/assets/cja-example-view-through-validation.png "뷰스루 추적 페이로드 유효성 검사의 예")

1. [세 개의 각 데이터 세트(웹 사이트 이벤트 데이터 세트, Adobe Advertising 분류 데이터 세트 및 Adobe Advertising 요약 지표 데이터 세트)에 대한 활동을 확인하여 데이터 배달의 유효성을 검사합니다](https://experienceleague.adobe.com/en/docs/experience-platform/catalog/datasets/user-guide#view-datasets).

   일별 일괄 처리 수집에 대한 데이터 세트 활동이 표시됩니다. 24시간 후에 이벤트 데이터 집합에 레코드가 0으로 표시되면 [데이터 스트림](#dataset-datastream) 및 [Adobe 태그의 웹 SDK 확장 구성](#tags-websdk)을 다시 확인하세요.

1. Adobe Experience Platform 관리자에게 [태그를 라이브 프로덕션 환경에 게시](https://experienceleague.adobe.com/en/docs/experience-platform/tags/publish/publishing-flow)하도록 요청하십시오.

   조직의 IT 부서나 다른 그룹은 태그 배포를 예약하거나 그에 대한 정보를 받아야 할 수 있습니다.

## Customer Journey Analytics에서 Experience Platform 데이터 세트에 대한 연결 만들기 {#dataset-connection}

다음 단계에 따라 Experience Platform 데이터 세트에서 Adobe Advertising으로 Customer Journey Analytics 데이터를 가져옵니다. Customer Journey Analytics에 대한 조직의 사이트 관리자가 이러한 작업을 수행할 수 있습니다.

동일한 정보로 기존 연결을 선택적으로 편집할 수도 있습니다.

1. Customer Journey Analytics에서 Experience Platform 데이터 세트와 스키마를 포함하는 연결을 [만들거나 편집](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-connections/create-connection)합니다.

   <!-- **Note:** You must send data for all DSP and Search, Social, & Commerce accounts to a single Experience Platform instance and sandbox.  -->

   * 올바른 샌드박스(조직에서 설정)가 선택되었는지 확인합니다.

   * 일일 평균 이벤트 수를 계산합니다(대부분의 조직의 경우 100만 개 미만).

   * Experience Platform 이벤트 지표 데이터 세트(유형: `Event`), <!-- Adobe Advertising --> 이벤트 요약 지표 데이터 세트(유형: `Event`) 및 <!-- Adobe Advertising --> 차원(분류/메타데이터) 데이터 세트(유형: `Lookup`)를 추가합니다.

     팀이 이벤트 데이터 세트를 만들고 Adobe Advertising이 이벤트 데이터 세트를 기반으로 요약 및 차원 데이터 세트를 만들었습니다.

     필요에 따라 추가 데이터 세트를 선택적으로 포함할 수 있습니다.

   * 데이터 세트 설정을 구성합니다.

      * [!UICONTROL Event Dataset] 설정의 경우:

         * **[!UICONTROL Person ID]:** `Identity Map`

         * **[!UICONTROL Use primary identity namespace]:** Customer Journey Analytics과 Adobe Real-Time CDP 모두에 대해 하나의 데이터 세트와 스키마를 사용하려면 이 설정을 사용하도록 설정하고 `IdentityMap` 필드 그룹에서 기본 ID를 정의합니다. `Required Field`도 지원됩니다.

         * **[!UICONTROL Data Source Type]:** `Web Data > Others` <!-- I don't see "Others" in the screen shot example -->

         * **[!UICONTROL Import all new data]:** 설정 사용

      * 분류([!UICONTROL Lookup Dataset]) 설정의 경우 차원 데이터 세트를 이벤트 데이터 세트에 매핑합니다.

         * **[!UICONTROL Key]**(차원 데이터 세트의 키로 사용할 필드): `Tracking Code`(스키마의 `trackingCode` 필드와 동일).

         * **[!UICONTROL Matching key]**(이벤트 데이터 세트에 대해 일치하는 키로 사용할 필드): `Tracking Code (Event datasets)`.

         * **[!UICONTROL Import all new data]:** 설정 사용

         * **[!UICONTROL Backfill all existing data]:** 설정 사용

      * [!UICONTROL Metrics Dataset] 설정의 경우:

         * **[!UICONTROL Person ID]:** `Identity Map`

         * **[!UICONTROL Timestamp]:** 값 확인

         * **[!UICONTROL Import all new data]:** 설정 사용

2. 3시간 이내에 Customer Journey Analytics에서 데이터를 사용할 수 있는지 확인합니다.

   1. Customer Journey Analytics에서 **[!UICONTROL Connections]**(으)로 이동하여 연결을 선택하십시오.

   2. 표시된 데이터 집합 목록에서 &quot;[!UICONTROL Number of Records]&quot; 보고서에 데이터가 추가되었는지 확인하십시오.

## Customer Journey Analytics에서 데이터 보기 설정 {#cja-data-views}

Customer Journey Analytics에서 하나 이상의 데이터 보기를 만들어 보고를 위한 지표 및 차원을 정의합니다. 웹 분석가는 이러한 작업을 수행할 수 있습니다.

1. Customer Journey Analytics에서 [데이터 보기를 만듭니다](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-dataviews/create-dataview).

1. 다음 정보를 포함하도록 보기를 구성합니다.

   * Adobe Analytics 계정이 있는 경우 [!UICONTROL Configure] 탭의 [!UICONTROL Calendar] 섹션에서 [!DNL Analytics] 계정에 대해 [!UICONTROL Time Zone]을(를) 사용하십시오.

   * [!UICONTROL Components] 탭에서:

      * 조회 데이터 세트(차원/분류 데이터 포함), 이벤트 데이터 세트(이벤트 수준 데이터 포함) 및 요약 데이터 세트(클릭과 같은 다른 지표 포함)를 추가합니다.

      * 데이터 보기에 포함할 이벤트 데이터 세트 및 조회 데이터 세트에서 지표를 선택합니다.

      * 스키마 경로가 `_experience.adcloud.conversionDetails.trackingCode`인 이벤트 데이터 집합에 속하는 &quot;[!UICONTROL Tracking Code]&quot;을(를) 검색합니다. **[!UICONTROL Persistence]**&#x200B;을(를) *[!UICONTROL Most Recent]*(으)로 설정합니다.

<!--

Seems to not be necessary now:


       You already joined these two datasets in the connection that you created in the [last procedure](#dataset-connection).
     
     *  Join the events dataset to the summary dataset, which isn't yet joined to anything:
     
       * For each dimension with summary data that you want to be available in Customer Journey Analytics, [create a derived field](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-dataviews/derived-fields).

         For example, to view summary data for campaigns, create a derived field for the dimension `Adobe Advertising Campaign`.
         
         You'll link the two datasets using the matching key `trackingCode` (which is the schema field for the Adobe Advertising ID).
       
         * In the [!UICONTROL Lookup] section of the derived rule builder:
         
           * For the **[!UICONTROL Value]** field, select "[!UICONTROL Tracking Code]" from the metrics summary dataset.

           * For the **[!UICONTROL Lookup dataset]** field, select the dimensions dataset (such as "Adobe Advertising Classification").

           * For the **[!UICONTROL Matching Key]** field, select "[!UICONTROL Tracking Code]" from the classification dataset.

           * For the **[!UICONTROL Values to return]** field, select the dimension (such as "[!UICONTROL Adobe Advertising Campaign]")" from the classification dataset.
         
         The derived field name is appended with "(DF)", such as `Adobe Advertising Campaign(DF)`. 
         
       * For each derived field:
       
         * In the [!UICONTROL Included components] section, add the derived field.
         
           Two names are now listed for the same dimension (for example, "Adobe Advertising Campaign(DF)" (the derived field) and "Adobe Advertising Campaign" (the field in the summary dataset)).

         * Select the dimension in the summary dataset (such as "Adobe Advertising Campaign") and edit the settings for the dataset.

           The settings open on the right.

           * In the the Summary Data Group section, select the option to **[!UICONTROL Create grouping]**.

           * For the **[!UICONTROL Dimension]** field, select the derived field (which is appended with "(DF)," such as "Adobe Advertising Campaign(DF)").
         
           * Select the option to **[!UICONTROL Hide in reporting]**, which hides the derived field name in Workspace.

-->

## Customer Journey Analytics Workspace에서 보고서 및 시각화 설정 {#cja-reports}

Customer Journey Analytics Workspace에서 다음 단계에 따라 보고서 및 시각화를 구성합니다. 웹 분석가는 이러한 작업을 수행할 수 있습니다.

1. 데이터 보기 내에 구성된 차원 및 지표를 기반으로 보고서와 시각화를 빌드하려면 Workspace에서 [프로젝트를 만듭니다](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-workspace/build-workspace-project/create-projects).

   예를 들어 [!UICONTROL Tracking Code (2)]&#x200B;(이벤트를 캠페인 메타데이터에 연결), [!UICONTROL Adobe Advertising Campaign]&#x200B;(캠페인 수준 데이터의 경우), [!UICONTROL Adobe Advertising Placement] 또는 [!UICONTROL Adobe Advertising Ad Group]&#x200B;(배치 수준 또는 광고 그룹 수준 데이터의 경우), [!UICONTROL Events], [!UICONTROL Impressions] 및 [!UICONTROL Clicks] 차원을 포함합니다.

하나의 자유 형식 테이블에서 동일한 차원을 사용하여 요약 지표와 이벤트 데이터를 모두 분류할 수 있습니다.

1. ([!DNL Google Ads] 또는 [!DNL Microsoft Advertising]의 데이터가 있는 경우) 광고 네트워크별 지표에 대해 `googleConversions` 및 `microsoftConversions`(으)로 그룹화된 필드를 사용하여 게시자가 추적한 전환 보고서를 만듭니다.

1. 데이터가 표시되는지 확인합니다.

>[!TIP]
>
>요약 이벤트는 일반적으로 몇 개의 추가 이벤트, 하루에 한 개의 추가 세션 또는 보고서당 한 명의 추가 사용자와 같이 적은 양의 추가 데이터를 보고서에 추가합니다. 이러한 추가 사항은 표준 웹 이벤트에 비해 무시할 수 있습니다. 그러나 더미 개인 ID `00000000-0000-0000-0000-000000000000`에 대한 데이터를 제외하여 이 추가 요약 이벤트 데이터를 필터링할 수 있습니다.개인 ID를 사용하여 데이터를 제외하는 예&rbrack;(/help/integrations/assets/cja-report-with-person-id.png "개인 ID를 사용하여 데이터를 제외하는 예")

![데이터 세트가 Customer Journey Analytics에 표시되는 방법](/help/integrations/assets/cja-report-example.png "데이터 세트가 Customer Journey Analytics에 표시되는 방법")

>[!MORELIKETHIS]
>
>* [개요](overview.md)
>* [필수 구성 요소](prerequisites.md)
>*  [!DNL Customer Journey Analytics][&#128279;](ids.md)에서 사용하는 Adobe Advertising ID
>* [Customer Journey Analytics의 Adobe Advertising 지표 및 차원](advertising-data-in-cja.md)
>* [Adobe Customer Journey Analytics에서 사용할 AMO ID 및 EF ID에 대한 내역 데이터를 수집합니다](/help/integrations/analytics/rvars-to-evars.md).
>* [문제 해결](troubleshooting.md)
>* [Customer Journey Analytics 안내서](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-landing)
>* Customer Journey Analytics [Adobe Analytics 사용자를 위한 사용 안내서](https://experienceleague.adobe.com/en/docs/analytics-platform/using/compare-aa-cja/aa-to-cja-user)
