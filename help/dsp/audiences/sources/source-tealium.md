---
title: 다음에서 사용자 ID 변환 [!DNL Tealium] 범용 ID로
description: DSP을 활성화하여 다음을 수집하는 방법 알아보기 [!DNL Tealium] 자사 세그먼트.
feature: DSP Audiences
exl-id: 100abbe7-e228-4eb6-a5b9-bf74e83b3aa2
source-git-commit: 729098f01fb9d076efb2b945be4011df9ab1c905
workflow-type: tm+mt
source-wordcount: '1109'
ht-degree: 0%

---

# 다음에서 사용자 ID 변환 [!DNL Tealium] 범용 ID로

*Beta 기능*

와 DSP 통합 사용 [!DNL Tealium] 고객 데이터 플랫폼 : 조직의 자사 해시된 이메일 주소를 타겟팅된 광고를 위한 범용 ID로 변환합니다. 프로세스에서는 [!DNL Amazon Web Services] (AWS) firehose 커넥터. Tealium의 데이터를 DSP과 공유하려면 다음 단계를 따르십시오.

1. (이메일 주소를 (으)로 변환 [!DNL RampIDs]<!-- or [!DNL ID5] IDs -->; 광고주 [[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md)) [활성화하려면 추적 설정 [!DNL Analytics] 측정](#analytics-tracking).

1. [DSP에서 대상 소스 만들기](#source-create).

1. [세그먼트 매핑 데이터 준비 및 공유](#map-data).

1. [에서 커넥터 만들기 [!DNL Tealium] 세그먼트 데이터를 공유하려면](#tealium-connector).

1. [에서 기존 커넥터 복제 [!DNL Tealium] 세그먼트를 계속 공유하려면](#duplicate-connector).

1. [범용 ID 수를 해시된 이메일 주소 수와 비교](#compare-id-count).

세그먼트는 24시간 이내에 DSP에서 사용할 수 있어야 하며 24시간마다 새로 고쳐집니다.

## 1단계: 추적 설정 [!DNL Analytics] 측정 {#analytics-tracking}

*를 사용하는 광고주 [[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md))*

이메일 주소를 다음으로 변환하려면 [!DNL RampIDs] 또는 [!DNL ID5] ID, 다음을 수행해야 합니다.

1. (아직 완료하지 않은 경우) 모두 완료 [구현을 위한 사전 요구 사항 [!DNL Analytics for Advertising]](/help/integrations/analytics/prerequisites.md) 및 다음을 확인합니다. [AMO ID 및 EF ID](/help/integrations/analytics/ids.md) 가 추적 URL에서 채워집니다.

1. 범용 ID 파트너에 등록하고 웹 페이지에 범용 ID 관련 코드를 배포하여 데스크탑 및 모바일 웹 브라우저(모바일 앱은 아님)의 ID에서 뷰스루로의 전환을 일치시킵니다.

   * **대상 [!DNL RampIDs]:** 뷰스루를 위해 데스크탑 및 모바일 웹 브라우저(모바일 앱은 아님)의 ID에서 변환된 내용을 일치시키려면 웹 페이지에 추가 JavaScript 태그를 배포해야 합니다. Adobe 계정 팀에 문의하여 다음에 대한 등록 지침을 제공합니다. [!DNL LiveRamp] [!DNL LaunchPad] 태그 위치: [!DNL LiveRamp] 인증 트래픽 솔루션. 등록은 무료이지만 계약서에 서명하셔야 합니다 등록하면 Adobe 계정 팀이 웹 페이지에서 구현할 조직의 고유 태그를 생성하고 제공합니다.

## 2단계: DSP에서 대상 소스 만들기 {#source-create}

1. [대상자 소스 만들기](source-manage.md) DSP 계정 또는 광고주 계정으로 대상자를 가져오려면 다음을 수행하십시오. 사용자 식별자를 다음 중 하나로 변환하도록 선택할 수 있습니다 [사용 가능한 범용 ID 형식](source-about.md).

   소스 설정에는 세그먼트 매핑 데이터를 준비하는 데 사용할 자동 생성 소스 키가 포함됩니다.

1. 대상 소스를 만든 후 소스 코드 키를 [!DNL Tealium] 사용자.

## 3단계: 세그먼트 매핑 데이터 준비 및 공유 {#map-data}

1. 광고주는 세그먼트 매핑 데이터를 준비하고 공유해야 합니다.

   1. 광고주는 다음 범위 내에서 데이터를 준비해야 합니다. [!DNL Tealium]:

      1. SHA-256 알고리즘을 사용하여 광고주의 대상에 대한 이메일 ID를 해시합니다.

      1. 해시된 이메일 ID가 포함된 열을 방문자 ID 유형의 속성에 매핑합니다.

      1. 를 사용하여 대상자 만들기 `Tealium_visitor_id` 특성. 대상자를 트리거하는 올바른 데이터 보강 기능을 적용합니다. 다음을 참조하십시오. [[!DNL Tealium] 방문자 ID 속성에 대한 설명서](https://docs.tealium.com/server-side/visitor-stitching/visitor-id-attribute/).

   1. 광고주는 DSP에서 세그먼트를 만들려면 Adobe 계정 팀에 세그먼트 매핑 데이터를 제공해야 합니다. 쉼표로 구분된 값 파일에서 다음 열 이름과 값을 사용합니다.

      * **외부 세그먼트 키:** 나중에 커넥터 작업 설정에서 지정할 외부 세그먼트 키 [!DNL Tealium]. 권장되는 명명 규칙은 &quot;`<DSP source key>_<Tealium segment name>`&quot;57bf424dc10_coffee-drinkers&quot;와 같은 &quot;입니다. DSP 소스 키의 경우 [!UICONTROL Source Key] DSP 대상자 소스 설정에서.

      * **세그먼트 이름:** 세그먼트 이름입니다.

      * **세그먼트 설명:** 세그먼트의 목적 또는 규칙 또는 둘 다입니다.

      * **상위 ID:** 비워 둠

      * **비디오 CPM:** 0

      * **CPM 표시:** 0

      * **세그먼트 창:** 세그먼트 TTL(time-to-live).

## 4단계: 커넥터 만들기 [!DNL Tealium] 세그먼트 데이터를 공유하려면 {#tealium-connector}

공유할 각 세그먼트에 대해 데이터 변경을 트리거하는 각 작업에 대해 별도의 커넥터를 만듭니다. 예를 들어 각각 트리거가 2개인 2개의 세그먼트를 공유하려면 4개의 커넥터를 만듭니다.

1. Adobe 계정 팀은 광고주에게 AWS firehose 커넥터 자격 증명을 제공합니다.

1. 위치 [!DNL Tealium], [커넥터 추가](https://docs.tealium.com/server-side/connectors/add/), 다음 옵션 사용:

   1. 다음 항목 선택 [!DNL AWS Firehose] 커넥터.

   1. 소스 설정에서:

      1. 공유할 대상 세그먼트를 선택합니다.

      1. 트리거 설정:

         * 세그먼트의 첫 번째 커넥터에 대해 트리거를 선택합니다 `Joined Audience`. 이렇게 하면 사용자가 세그먼트에 참여할 때마다 DSP과 데이터가 공유됩니다.

         * 세그먼트의 두 번째 커넥터에 대해 트리거를 선택합니다 `Left Audience`. 이 커넥터는 DSP에서 세그먼트를 나가는 모든 옵트아웃 및 사용자를 처리하는 데 사용됩니다.

   1. 구성 설정에서 AWS firehose 커넥터를 지정합니다. DSP용 Firehose 커넥터를 아직 추가하지 않은 경우 다음 정보를 사용하여 Firehose 커넥터를 추가합니다.

      * **이름:** 커넥터의 이름입니다.

      * **액세스 키:** Adobe 계정 팀에서 제공한 액세스 키입니다.

      * **비밀 키:** Adobe 계정 팀에서 제공한 비밀 키.

      * **지역:** US East North Virginia (us-east-1)

   1. 작업 설정에서 다음을 수행합니다.

      1. 다음 정보를 사용하여 세그먼트에 데이터를 추가하는 &quot;게재 스트림으로 고객 데이터 보내기(고급)&quot; 작업을 만듭니다.

         * **작업 이름:** 작업의 이름입니다.

         * **작업 유형:** 게재 스트림으로 고객 데이터 보내기(고급)

         * **게재 스트림:** Tealium_CDP_Connector

         * **메시지 데이터:**  다음을 수행합니다.

            1. 세그먼트에 대해 속성 하나를 선택합니다.

               * Hashed_Email 속성의 경우 사용자 지정 메시지의 이름을 지정합니다 `hashed_email`.

               * Cookies 속성의 경우 사용자 지정 메시지의 이름을 로 지정합니다 `cookies`.

            1. 사용자 정의 필드를 만드는 옵션에서 [!DNL Source Key] 필드에 [!UICONTROL External Segment Key] 이(가)에 포함되었습니다. [세그먼트 매핑 데이터](#map-data) 이전 절차에서.

               DSP은 이 키를 사용하여 세그먼트를 채웁니다.

            1. (권장) 업데이트 작업을 만들어 세그먼트를 최신 상태로 유지합니다.

## 5단계: 의 기존 커넥터 복제 [!DNL Tealium] 세그먼트를 계속 공유하려면 {#duplicate-connector}

세그먼트당 하나의 커넥터와 커넥터당 하나의 세그먼트만 가질 수 있습니다.

1. 위치 [!DNL Tealium]를 클릭하고, 다른 세그먼트를 만들려는 세그먼트를 복제한 다음 새 세그먼트의 이름을 변경합니다.

1. 위치 [!DNL Tealium], 복제 [만든 커넥터](#tealium-connector) 이전 절차에서 새 커넥터의 이름을 로 바꿉니다.`<original name>-copy`&quot;새 세그먼트 이름.

## 6단계: 범용 ID 수를 해시된 이메일 주소 수와 비교 {#compare-id-count}

모든 단계를 완료하고에서 대상을 만들거나 편집할 때 사용할 수 있는 대상 라이브러리에서 확인합니다 [!UICONTROL Audiences] > [!UICONTROL All Audiences] 또는 배치 설정 내에서) 세그먼트가 24시간 내에 채워집니다. 범용 ID 수를 해시된 원본 이메일 주소 수와 비교합니다.

범용 ID에 대한 해시된 이메일 주소의 번역률은 90%보다 커야 합니다. 예를 들어 고객 데이터 플랫폼에서 100개의 해시된 이메일 주소를 전송하는 경우 90개 이상의 범용 ID로 변환되어야 합니다. 90% 이하의 번역률이 문제입니다. 세그먼트 카운트가 달라질 수 있는 방법에 대한 자세한 내용은 &quot;[이메일 ID와 범용 ID 간의 데이터 분산 원인](#universal-ids-data-variances).&quot;

세그먼트는 24시간마다 새로 고쳐집니다. 단, 세그먼트에 포함하면 30일 후에 만료되어 개인 정보 규정을 준수할 수 있으므로 대상자를에서 다시 푸시하여 새로 고침하십시오. [!DNL Tealium] 30일 이내입니다.

문제 해결 지원은 Adobe 계정 팀에 문의하거나 `adcloud-support@adobe.com`.

>[!MORELIKETHIS]
>
>* [자사 대상 소스 정보](/help/dsp/audiences/sources/source-about.md)
>* [범용 ID 대상을 활성화하기 위한 대상 소스 관리](source-manage.md)
>* [대상 소스 설정](source-settings.md)
>* [다음에서 사용자 ID 변환 [!DNL Adobe Real-Time CDP] 범용 ID로](/help/dsp/audiences/sources/source-adobe-rtcdp.md)
>* [대상자 관리 기본 정보](/help/dsp/audiences/audience-about.md)

<!--
>* [Convert User IDs from [!DNL Optimizely] to Universal IDs](/help/dsp/audiences/sources/source-optimizely.md)
-->
