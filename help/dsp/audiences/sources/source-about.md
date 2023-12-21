---
title: 대상 소스에서 인증된 세그먼트 활성화 정보
description: 고객 데이터 플랫폼에서 자사 세그먼트를 수집하는 방법에 대해 알아봅니다.
feature: DSP Audiences
exl-id: ba056440-fa2b-4472-bbfd-16dd0af887f1
source-git-commit: e3e8753db31bc835c49eb2037fdcd7696a895a8c
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---

# 대상 소스에서 인증된 세그먼트 활성화 정보

DSP은 해시된 이메일 ID 또는 CDP(고객 데이터 플랫폼) 내에 구축된 범용 ID로 구성된 자사 세그먼트를 수집할 수 있습니다. 수집된 세그먼트를 배치의 타겟으로 사용할 수 있습니다.

다음 CDP는 커넥터를 설정했지만, DSP은 배치, 스트리밍 또는 API 기반 데이터 공유를 사용하여 모든 CDP에 연결할 수도 있습니다. 새 CDP와 통합하려면 Adobe 계정 팀에 문의하십시오.

## [!DNL Adobe Real-Time Customer Data Platform]

DSP은 와 통합됩니다. [다음 [!DNL Adobe Real-Time Customer Data Platform (CDP)]](https://experienceleague.adobe.com/docs/experience-platform/rtcdp/overview.html): Adobe Experience Platform의 일부입니다.

위치 [!DNL Real-Time CDP], *대상* 원활한 데이터 활성화를 허용하는 외부 데이터 플랫폼에 대한 연결입니다. 예를 들어 대상을 사용하여 DSP에서 지원하는 디지털 형식 전반에 걸친 타겟팅 광고에 대해 알려진 고객 관계(해시된 이메일 주소 등)를 활성화할 수 있습니다. 대상에 대한 자세한 내용은 Experience Platform 를 참조하십시오. [대상 안내서](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html), 제품 개요, 지침 포함 [대상 작업 공간 만들기](https://experienceleague.adobe.com/docs/experience-platform/destinations/ui/destinations-workspace.html) 및 [대상 연결 만들기](https://experienceleague.adobe.com/docs/experience-platform/destinations/ui/connect-destination.html), 및 [대상으로 데이터 활성화](https://experienceleague.adobe.com/docs/experience-platform/destinations/ui/activate/activate-segment-streaming-destinations.html).

를 참조하십시오.[과 DSP 통합을 사용하기 위한 워크플로우 [!DNL Adobe Real-Time CDP]](/help/dsp/audiences/sources/source-adobe-rtcdp.md).&quot;

## [!DNL ActionIQ]

에서 조직의 자사 데이터를 공유할 수 있습니다. [!DNL Action IQ] DSP을 사용하는 고객 데이터 플랫폼. 그런 다음 를 사용하여 DSP 배치를 세그먼트에 타깃팅할 수 있습니다. [!DNL RampIDs] 또는 [!DNL Unified IDs 2.0].

이 통합에는 사용자 정의가 필요합니다. 자세한 내용은 Adobe 계정 팀에 문의하십시오.

## [!DNL Tealium]

에서 조직의 자사 데이터를 공유할 수 있습니다. [!DNL Tealium] 다음을 사용하는 고객 데이터 플랫폼 [!DNL Amazon Web Services]. 그런 다음 를 사용하여 DSP 배치를 세그먼트에 타깃팅할 수 있습니다. [!DNL RampIDs]. 를 참조하십시오.[과 DSP 통합을 사용하기 위한 워크플로우 [!DNL Tealium]](/help/dsp/audiences/sources/source-tealium.md).&quot;

>[!MORELIKETHIS]
>
>* [과 DSP 통합을 사용하기 위한 워크플로우 [!DNL Adobe Real-Time CDP]](/help/dsp/audiences/sources/source-adobe-rtcdp.md)
>* [과 DSP 통합을 사용하기 위한 워크플로우 [!DNL Tealium]](/help/dsp/audiences/sources/source-tealium.md)
>* [자사 대상을 활성화할 대상 소스 만들기](source-create.md)
>* [대상 소스 설정](source-settings.md)
>* [대상자 관리 기본 정보](/help/dsp/audiences/audience-about.md)

<!--
>* [Workflow for Using the DSP Integration with [!DNL ActionIQ]](/help/dsp/audiences/sources/source-actioniq.md)
-->
