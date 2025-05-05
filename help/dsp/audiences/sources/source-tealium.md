---
title: 사용자 ID를  [!DNL Tealium] 에서 범용 ID로 변환
description: DSP에서  [!DNL Tealium] 자사 세그먼트를 수집할 수 있도록 하는 방법을 알아봅니다.
feature: DSP Audiences
exl-id: 100abbe7-e228-4eb6-a5b9-bf74e83b3aa2
source-git-commit: 91b08bf54f067666c9c27949ff740639738887d0
workflow-type: tm+mt
source-wordcount: '1092'
ht-degree: 0%

---

# 사용자 ID를 [!DNL Tealium]에서 유니버설 ID로 변환

*Beta 기능*

[!DNL Tealium] 고객 데이터 플랫폼과 DSP 통합을 사용하여 조직의 자사 해시된 이메일 주소를 타깃팅된 광고를 위한 범용 ID로 변환합니다. 프로세스에서 [!DNL Amazon Web Services] (AWS) firehose 커넥터를 사용합니다. Tealium의 데이터를 DSP과 공유하려면 다음 단계를 따르십시오.

1. (전자 메일 주소를 [!DNL RampIDs]<!-- or [!DNL ID5] IDs -->; [[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md)을(를) 사용하는 광고주로 변환하려면) [추적을 사용하도록 설정 [!DNL Analytics] 측정](#analytics-tracking)합니다.

1. [DSP에서 대상 소스를 만듭니다](#source-create).

1. [세그먼트 매핑 데이터를 준비하고 공유합니다](#map-data).

1. [세그먼트 데이터를 공유하려면 [!DNL Tealium] 에 커넥터를 만듭니다](#tealium-connector).

1. [기존 커넥터를  [!DNL Tealium] 복제하여 세그먼트를 계속 공유](#duplicate-connector)합니다.

1. [범용 ID 수를 해시된 이메일 주소 수와 비교](#compare-id-count).

## 1단계: [!DNL Analytics] 측정에 대한 추적 설정 {#analytics-tracking}

*[[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md)을(를) 사용하는 광고주*

전자 메일 주소를 [!DNL RampIDs] 또는 [!DNL ID5] ID로 변환하려면 다음을 수행해야 합니다.

1. 아직 완료하지 않았다면 [구현을 위한 필수 구성 요소 [!DNL Analytics for Advertising]](/help/integrations/analytics/prerequisites.md)를 모두 완료하고 [AMO ID 및 EF ID](/help/integrations/analytics/ids.md)이(가) 추적 URL에 채워져 있는지 확인하십시오.

1. 범용 ID 파트너에 등록하고 웹 페이지에 범용 ID 관련 코드를 배포하여 데스크탑 및 모바일 웹 브라우저(모바일 앱은 아님)의 ID에서 뷰스루로의 전환을 일치시킵니다.

   * **[!DNL RampIDs]의 경우:** 뷰스루에 대한 데스크톱 및 모바일 웹 브라우저(모바일 앱은 아님)의 ID 전환과 일치하려면 웹 페이지에 추가 JavaScript 태그를 배포해야 합니다. Adobe 계정 팀에 문의하여 [!DNL LiveRamp] 인증 트래픽 솔루션에서 [!DNL LiveRamp] [!DNL LaunchPad] 태그를 등록하는 방법에 대한 지침을 제공받으십시오. 등록은 무료이지만 계약서에 서명하셔야 합니다 등록하면 Adobe 계정 팀이 웹 페이지에서 구현할 조직의 고유 태그를 생성하고 제공합니다.

## 2단계: DSP에서 대상 소스 만들기 {#source-create}

1. 대상을 DSP 계정 또는 광고주 계정으로 가져오려면 [대상 소스를 만듭니다](source-manage.md). 사용자 식별자를 [사용 가능한 범용 ID 형식](source-about.md) 중 하나로 변환하도록 선택할 수 있습니다.

   소스 설정에는 세그먼트 매핑 데이터를 준비하는 데 사용할 자동 생성 소스 키가 포함됩니다.

1. 대상 소스를 만든 후 [!DNL Tealium] 사용자와 소스 코드 키를 공유합니다.

## 3단계: 세그먼트 매핑 데이터 준비 및 공유 {#map-data}

광고주는 세그먼트 매핑 데이터를 준비하고 공유해야 합니다.

1. 광고주는 [!DNL Tealium] 내에 데이터를 준비해야 합니다.

   1. SHA-256 알고리즘을 사용하여 광고주의 대상에 대한 이메일 ID를 해시합니다.

   1. 해시된 이메일 ID가 포함된 열을 방문자 ID 유형의 속성에 매핑합니다.

   1. `Tealium_visitor_id` 특성을 사용하여 대상자를 만듭니다. 대상자를 트리거하는 올바른 데이터 보강 기능을 적용합니다. 방문자 ID 특성에 대한 [[!DNL Tealium] 설명서를 참조하십시오](https://docs.tealium.com/server-side/visitor-stitching/visitor-id-attribute/).

1. 광고주는 DSP에서 세그먼트를 만들려면 Adobe 계정 팀에 세그먼트 매핑 데이터를 제공해야 합니다. 쉼표로 구분된 값 파일에서 다음 열 이름과 값을 사용합니다.

   * **외부 세그먼트 키:** 나중에 [!DNL Tealium]의 커넥터에 대한 동작 설정에서 지정할 외부 세그먼트 키입니다. 권장되는 명명 규칙은 &quot;`<DSP source key>_<Tealium segment name>`&quot;(예: &quot;57bf424dc10_coffee-drinkers&quot;)입니다. DSP 소스 키의 경우 DSP 대상 소스 설정의 [!UICONTROL Source Key]을(를) 사용합니다.

   * **세그먼트 이름:** 세그먼트 이름입니다.

   * **세그먼트 설명:** 세그먼트의 목적이나 규칙 또는 둘 다입니다.

   * **상위 ID:** 비워 둠

   * **비디오 CPM:** 0

   * **CPM 표시:** 0

   * **세그먼트 창:** 세그먼트 TTL(Time-to-Live)입니다.

## 4단계: [!DNL Tealium]에 커넥터를 만들어 세그먼트 데이터를 공유합니다. {#tealium-connector}

공유할 각 세그먼트에 대해 데이터 변경을 트리거하는 각 작업에 대해 별도의 커넥터를 만듭니다. 예를 들어 각각 트리거가 2개인 2개의 세그먼트를 공유하려면 4개의 커넥터를 만듭니다.

1. Adobe 계정 팀은 광고주에게 AWS firehose 커넥터 자격 증명을 제공합니다.

1. [!DNL Tealium]에서 다음 옵션을 사용하여 [커넥터를 추가](https://docs.tealium.com/server-side/connectors/add/)합니다.

   1. [!DNL AWS Firehose] 커넥터를 선택하십시오.

   1. 소스 설정에서:

      1. 공유할 대상 세그먼트를 선택합니다.

      1. 트리거 설정:

         * 세그먼트에 대한 첫 번째 커넥터에 대해 `Joined Audience` 트리거를 선택합니다. 이렇게 하면 사용자가 세그먼트에 참여할 때마다 DSP과 데이터가 공유됩니다.

         * 세그먼트에 대한 두 번째 커넥터에 대해 `Left Audience` 트리거를 선택합니다. 이 커넥터는 DSP에서 세그먼트를 나가는 모든 옵트아웃 및 사용자를 처리하는 데 사용됩니다.

   1. 구성 설정에서 AWS firehose 커넥터를 지정합니다. DSP용 Firehose 커넥터를 아직 추가하지 않은 경우 다음 정보를 사용하여 Firehose 커넥터를 추가합니다.

      * **이름:** 커넥터의 이름입니다.

      * **액세스 키:** Adobe 계정 팀에서 제공한 액세스 키입니다.

      * **암호 키:** Adobe 계정 팀에서 제공한 암호 키입니다.

      * **지역:** 미국 동부 버지니아(미국 동부-1)

   1. 작업 설정에서 다음을 수행합니다.

      1. 다음 정보를 사용하여 세그먼트에 데이터를 추가하는 &quot;게재 스트림으로 고객 데이터 보내기(고급)&quot; 작업을 만듭니다.

         * **작업 이름:** 작업의 이름입니다.

         * **작업 유형:** 게재 스트림으로 고객 데이터 보내기(고급)

         * **게재 스트림:** Tealium_CDP_Connector

         * **메시지 데이터:** 다음을 수행합니다.

            1. 세그먼트에 대해 속성 하나를 선택합니다.

               * Hashed_Email 특성의 경우 사용자 지정 메시지의 이름을 `hashed_email`로 지정합니다.

               * Cookies 특성의 경우 사용자 지정 메시지의 이름을 `cookies`로 지정합니다.

            1. 사용자 지정 필드를 만드는 옵션의 [!DNL Source Key] 필드에 이전 절차의 [세그먼트 매핑 데이터](#map-data)에 포함된 [!UICONTROL External Segment Key]을(를) 입력하십시오.

               DSP은 이 키를 사용하여 세그먼트를 채웁니다.

            1. (권장) 업데이트 작업을 만들어 세그먼트를 최신 상태로 유지합니다.

## 5단계: 세그먼트를 계속 공유하려면 [!DNL Tealium]에서 기존 커넥터를 복제하십시오. {#duplicate-connector}

세그먼트당 하나의 커넥터와 커넥터당 하나의 세그먼트만 가질 수 있습니다.

1. [!DNL Tealium]에서 다른 세그먼트를 만들 세그먼트를 복제하고 새 세그먼트 이름을 바꾸십시오.

1. [!DNL Tealium]에서 이전 절차에서 [만든 커넥터](#tealium-connector)를 복제하고 새 커넥터의 이름을 &quot;`<original name>-copy`&quot;에서 새 세그먼트 이름으로 바꾸십시오.

## 6단계: 범용 ID 수를 해시된 이메일 주소 수와 비교 {#compare-id-count}

세그먼트는 24시간 이내에 DSP에서 사용할 수 있어야 합니다. DSP이 세그먼트 데이터를 받은 후 대상자 카운트는 9시간 이내에 표시됩니다.

대상 라이브러리([!UICONTROL Audiences] > [!UICONTROL All Audiences]에서 대상을 만들거나 편집할 때 또는 배치 설정 내에서 사용 가능)에서 세그먼트가 채워지고 있는지 확인하고 범용 ID 수를 원래 해시된 이메일 주소 수와 비교합니다. 허용되는 ID 변환 속도와 세그먼트 수가 달라질 수 있는 이유에 대한 자세한 내용은 &quot;[이메일 ID와 범용 ID 간의 데이터 분산](#universal-ids-data-variances)&quot;을 참조하십시오.

세그먼트는 24시간마다 새로 고쳐집니다. 하지만 세그먼트에 포함되면 기본적으로 30일 이후 또는 고객이 지정한 만료 기간 이후에 만료됩니다. 만료 전에 [!DNL Tealium]에서 세그먼트를 다시 푸시하여 세그먼트를 새로 고치십시오. 사용자 지정 세그먼트 만료를 요청하려면 Adobe 계정 팀에 문의하십시오.

## 문제 해결

번역 속도 및 사용자 수 문제를 해결하려면 &quot;[범용 ID 활성화 지원](/help/dsp/audiences/universal-ids.md)&quot;을 참조하십시오.

전환 프로시저의 문제를 해결하려면 Adobe 계정 팀이나 `adcloud-support@adobe.com`에 문의하십시오.

>[!MORELIKETHIS]
>
>* [자사 대상 소스 정보](/help/dsp/audiences/sources/source-about.md)
>* [범용 ID 대상을 활성화하기 위한 대상 소스 관리](source-manage.md)
>* [범용 ID 활성화 지원](/help/dsp/audiences/universal-ids.md)
>* [대상자 관리 정보](/help/dsp/audiences/audience-about.md)
