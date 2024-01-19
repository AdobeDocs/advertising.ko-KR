---
title: 과 DSP 통합을 사용하기 위한 워크플로우 [!DNL Tealium]
description: DSP을 활성화하여 다음을 수집하는 방법 알아보기 [!DNL Tealium] 자사 세그먼트.
feature: DSP Audiences
exl-id: 100abbe7-e228-4eb6-a5b9-bf74e83b3aa2
source-git-commit: b94541bf8675d535b2f19b26c05235eb56bc6c0b
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 0%

---

# 과 DSP 통합을 사용하기 위한 워크플로우 [!DNL Tealium]

에서 조직의 자사 데이터를 공유할 수 있습니다. [!DNL Tealium] 를 사용하는 고객 데이터 플랫폼 [!DNL Amazon Web Services] (AWS) firehose 커넥터. Tealium의 데이터를 DSP과 공유하는 네 가지 단계가 있습니다.

1. [DSP에서 대상 소스 만들기](#source-create).

1. [세그먼트 매핑 데이터 준비 및 공유](#map-data).

1. [에서 커넥터 만들기 [!DNL Tealium] 세그먼트 데이터를 공유하려면](#tealium-connector).

1. [에서 기존 커넥터 복제 [!DNL Tealium] 세그먼트를 계속 공유하려면](#duplicate-connector).

## 1단계: DSP에서 대상 소스 만들기 {#source-create}

* [대상자 소스 만들기](source-create.md) 대상을 DSP 계정 또는 광고주 계정으로 가져오고 소스 코드 키를 [!DNL Tealium] 사용자.

## 2단계: 세그먼트 매핑 데이터 준비 및 공유 {#map-data}

1. 광고주는 세그먼트 매핑 데이터를 준비하고 공유해야 합니다.

   1. 광고주는 다음 범위 내에서 데이터를 준비해야 합니다. [!DNL Tealium]:

      1. 광고주의 대상자에 대한 이메일 ID는 SHA-256 알고리즘을 사용하여 해시해야 합니다.

      1. 해시된 이메일 ID가 포함된 열은 방문자 ID 유형의 속성에 매핑되어야 합니다.

      1. 대상자는 `Tealium_visitor_id` 특성. 대상자를 트리거하려면 올바른 데이터 보강 기능을 적용해야 합니다. 다음을 참조하십시오. [[!DNL Tealium] 방문자 ID 속성에 대한 설명서](https://docs.tealium.com/server-side/visitor-stitching/visitor-id-attribute/).

   1. 광고주는 DSP에서 세그먼트를 만들려면 Adobe 계정 팀에 세그먼트 매핑 데이터를 제공해야 합니다. 쉼표로 구분된 값 파일에서 다음 열 이름과 값을 사용합니다.

      * **외부 세그먼트 키:** 나중에 커넥터 작업 설정에서 지정할 외부 세그먼트 키 [!DNL Tealium]. 권장되는 명명 규칙은 &quot;`<DSP source key>_<Tealium segment name>`&quot;57bf424dc10_coffee-drinkers&quot;와 같은 &quot;입니다.

      * **세그먼트 이름:** 세그먼트 이름입니다.

      * **세그먼트 설명:** 세그먼트의 목적 또는 규칙 또는 둘 다입니다.

      * **상위 ID:** 비워 둠

      * **비디오 CPM:** 0

      * **CPM 표시:** 0

      * **세그먼트 창:** 세그먼트 TTL(time-to-live).

## 3단계: 에서 커넥터 만들기 [!DNL Tealium] 세그먼트 데이터를 공유하려면 {#tealium-connector}

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

            1. 사용자 정의 필드를 만드는 옵션에서 [!DNL Source Key] 필드에 [!UICONTROL External Segment Key] 의 세그먼트 매핑 데이터에 포함되었습니다. [2단계](#map-data).

               DSP은 이 키를 사용하여 세그먼트를 채웁니다.

            1. (권장) 업데이트 작업을 만들어 세그먼트를 최신 상태로 유지합니다.

## 4단계: 의 기존 커넥터 복제 [!DNL Tealium] 세그먼트를 계속 공유하려면 {#duplicate-connector}

세그먼트당 하나의 커넥터와 커넥터당 하나의 세그먼트만 가질 수 있습니다.

1. 위치 [!DNL Tealium]를 클릭하고, 다른 세그먼트를 만들려는 세그먼트를 복제한 다음 새 세그먼트의 이름을 변경합니다.

1. 위치 [!DNL Tealium]에서 만든 커넥터를 복제합니다. [3단계](#tealium-connector), 새 커넥터의 이름을에서 바꿉니다.`<original name>-copy`&quot;새 세그먼트 이름.

>[!MORELIKETHIS]
>
>* [대상 소스에서 인증된 세그먼트 활성화 정보](/help/dsp/audiences/sources/source-about.md)
>* [자사 대상을 활성화할 대상 소스 만들기](source-create.md)
>* [대상 소스 설정](source-settings.md)
>* [과 DSP 통합을 사용하기 위한 워크플로우 [!DNL Adobe Real-Time CDP]](/help/dsp/audiences/sources/source-adobe-rtcdp.md)
>* [대상자 관리 기본 정보](/help/dsp/audiences/audience-about.md)
