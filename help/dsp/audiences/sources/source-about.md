---
title: 자사 대상 소스 정보
description: 쿠키 없는 타깃팅을 위해 자사 세그먼트의 다른 사용자 식별자를 범용 ID로 변환하는 방법에 대해 알아봅니다.
feature: DSP Audiences
exl-id: ba056440-fa2b-4472-bbfd-16dd0af887f1
source-git-commit: 3a641db6b145e67e6e1f1daca271dd524973e075
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# 자사 대상 소스 정보

*Beta 기능*

DSP은 고객 데이터 플랫폼(CDP) 내에 구축된 해시된 이메일 ID로 구성된 자사 세그먼트를 수집하여 범용 ID로 구성된 세그먼트로 변환할 수 있습니다. 각 결과 ID는 사용자를 기반으로 하며 광고 빈도 상한은 ID 수준 <!-- Move that info. to somewhere else? -->에서 적용됩니다.

세그먼트 세부 사항에는 각 범용 ID 유형의 크기와 쿠키 또는 장치 ID로 추적되는 각 장치 유형의 크기가 포함됩니다.

## 범용 ID 유형 {#universal-id-types}

<!--  Replace below with this once ID5 sources are possible 

Using your first-party data, you can create segments with IDs from the following universal ID partners.

* Authenticated (deterministic) IDs using hashed email addresses:

-->

다음 범용 ID 파트너의 인증된(결정론적) ID를 사용하여 자사 세그먼트를 세그먼트로 번역할 수 있습니다.

* [[!DNL LiveRamp] [!DNL RampIDs]](https://liveramp.com/identity-resolution):

   * 로그인한 사용자를 재타겟팅하기 위해

     [!DNL RampIDs]은(는) 북미, 오스트레일리아 및 뉴질랜드의 사용자가 사용할 수 있습니다.

     요금은 게재된 디스플레이 광고 노출당 USD 0.15 및 게재된 비디오 광고 노출당 USD 0.25입니다.

   * [[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md)을(를) 사용한 측정용입니다.

* [[!DNL Unified ID 2.0 (UID2.0)] ](https://unifiedid.com):

   * 로그인한 사용자를 재타겟팅하기 위해

     [!DNL UID2 IDs]은(는) 유럽 경제 지역 및 일부 추가 국가에서 사용할 수 없습니다. [금지 국가 목록](/help/policies/universal-id-policy.md#prohibited-countries-uid2)을 참조하세요.

     요금은 게재된 디스플레이 광고 노출당 USD 0.15 및 게재된 비디오 광고 노출당 USD 0.25입니다.

<!-- Not yet

* Probabilistic (unauthenticated) IDs using hashed email addresses:

  * [[!DNL ID5] IDs](https://id5.io): For retargeting unauthenticated site traffic, prospecting using third-party data, and measurement for both using [[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md). ID5 IDs are available for no fee.

    ID5 creates an ID by stitching together user signals (hashed email address) with various browser signals (such as IP address and timestamp).

    [!DNL Analytics] measurement requires all [prerequisites for implementing [!DNL Analytics for Advertising]](/help/integrations/analytics/prerequisites.md) and the [AMO ID and EF ID in your tracking URLs](/help/integrations/analytics/ids.md). You also must sign an agreement with [!DNL ID5] and set a parameter within your existing JavaScript tracking tags. <!-- Contact your Adobe Account Team for instructions. -->

<!--
    >[!NOTE]
    >
    >Third-party segments from [!DNL Eyeota] may automatically include ID5 IDs, in addition to users tracked by cookies or device IDs. The segment details include the size for each type. The usual usage fee for each segment, which is stated next to the segment name, applies; no additional fees are charged for the ID5 IDs.
-->

## 자사 세그먼트에 대해 지원되는 고객 데이터 플랫폼

DSP은 자사 세그먼트를 빠르게 수집할 수 있도록 다음 CDP에 대한 커넥터를 설정했습니다.

DSP은 배치, 스트리밍 또는 API 기반 데이터 공유를 사용하여 추가 CDP에 연결할 수도 있습니다. 새 CDP와 통합하려면 Adobe 계정 팀에 문의하십시오.

### [!DNL Adobe Real-Time CDP]

DSP은(는) Adobe Experience Platform의 일부인 [the [!DNL Adobe Real-Time CDP]](https://experienceleague.adobe.com/docs/experience-platform/rtcdp/overview.html)에 대한 통합된 *대상*&#x200B;입니다.

[!DNL Real-Time CDP]에서 대상은 원활한 데이터 활성화를 허용하는 외부 데이터 플랫폼에 대한 연결입니다. 대상을 사용하여 DSP의 타깃팅된 광고를 위해 해시된 이메일 주소를 활성화할 수 있습니다. 대상에 대한 자세한 내용은 Experience Platform [대상 안내서](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html)를 참조하세요. 제품 개요, [대상 작업 공간 만들기](https://experienceleague.adobe.com/docs/experience-platform/destinations/ui/destinations-workspace.html) 및 [대상 연결 만들기](https://experienceleague.adobe.com/docs/experience-platform/destinations/ui/connect-destination.html)에 대한 지침, [대상에 대한 데이터 활성화](https://experienceleague.adobe.com/docs/experience-platform/destinations/ui/activate/activate-segment-streaming-destinations.html).

DSP에서 [!DNL Adobe] [!DNL Real-time CDP] 자사 세그먼트를 수집하고 해시된 이메일 주소를 범용 ID로 변환할 수 있도록 하려면 &quot;[사용자 ID를  [!DNL Adobe Real-Time CDP] 에서 범용 ID로 변환](/help/dsp/audiences/sources/source-adobe-rtcdp.md)&quot;을(를) 참조하십시오.

### [!DNL ActionIQ]

[!DNL ActionIQ] 고객 데이터 플랫폼에서 조직의 자사 데이터를 DSP과 공유하여 해시된 이메일 주소를 DSP의 타깃팅된 광고를 위한 범용 ID로 변환할 수 있습니다. 이 통합에는 사용자 정의가 필요합니다. 자세한 내용은 Adobe 계정 팀에 문의하십시오.

### [!DNL Amperity]

[!DNL Amperity] 고객 데이터 플랫폼에서 조직의 자사 데이터를 DSP과 공유하여 해시된 이메일 주소를 DSP의 타깃팅된 광고를 위한 범용 ID로 변환할 수 있습니다. 자세한 내용은 &quot;[사용자 ID를  [!DNL Amperity] 에서 범용 ID로 변환](/help/dsp/audiences/sources/source-amperity.md)&quot;을 참조하십시오.

### [!DNL Optimizely]

[!DNL Optimizely] 고객 데이터 플랫폼에서 조직의 자사 데이터를 DSP과 공유하여 해시된 이메일 주소를 DSP의 타깃팅된 광고를 위한 범용 ID로 변환할 수 있습니다. 자세한 내용은 &quot;[사용자 ID를  [!DNL Optimizely] 에서 범용 ID로 변환](/help/dsp/audiences/sources/source-optimizely.md)&quot;을 참조하십시오.

### [!DNL Tealium]

[!DNL Amazon Web Services]을(를) 사용하여 [!DNL Tealium] 고객 데이터 플랫폼에서 조직의 자사 데이터를 공유할 수 있습니다. DSP에서 타깃팅된 광고를 위해 해시된 이메일 주소를 범용 ID로 변환하는 방법에 대한 자세한 내용은 &quot;[사용자 ID를  [!DNL Tealium] 에서 범용 ID로 변환](/help/dsp/audiences/sources/source-tealium.md)&quot;을 참조하십시오.

>[!MORELIKETHIS]
>
>* [범용 ID 대상을 활성화하기 위한 대상 소스 관리](source-manage.md)
>* [범용 ID 활성화 지원](/help/dsp/audiences/universal-ids.md)
>* [사용자 ID를  [!DNL Adobe Real-Time CDP] 에서 범용 ID로 변환](/help/dsp/audiences/sources/source-adobe-rtcdp.md)
>* [사용자 ID를  [!DNL Amperity] 에서 범용 ID로 변환](/help/dsp/audiences/sources/source-amperity.md)
>* [사용자 ID를  [!DNL Optimizely] 에서 범용 ID로 변환](/help/dsp/audiences/sources/source-optimizely.md)
>* [사용자 ID를  [!DNL Tealium] 에서 범용 ID로 변환](/help/dsp/audiences/sources/source-tealium.md)
>* [대상자 관리 정보](/help/dsp/audiences/audience-about.md)
>* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)
