---
title: 대상 소스에서 인증된 세그먼트 활성화 정보
description: 고객 데이터 플랫폼에서 자사 세그먼트를 수집하는 방법에 대해 알아봅니다.
feature: DSP Audiences
exl-id: ba056440-fa2b-4472-bbfd-16dd0af887f1
source-git-commit: 14f78b89dea8cc680756232c6116975c652feee5
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# 대상 소스에서 인증된 세그먼트 활성화 정보

<!-- Doesn't specifically explain what you can do in our UI -->
*Beta 기능*

DSP은 고객 데이터 플랫폼(CDP) 내에 구축된 인증된 신호로 구성된 자사 세그먼트를 수집할 수 있습니다. 수집된 세그먼트를 배치의 타겟으로 사용할 수 있습니다.

## [!DNL Adobe Real-Time Customer Data Profile]

DSP은 [다음 [!DNL Adobe Real-Time Customer Data Profile (CDP)]](https://experienceleague.adobe.com/docs/experience-platform/rtcdp/overview.html): Adobe Experience Platform의 일부입니다.

위치 [!DNL Real-time CDP], *대상* 원활한 데이터 활성화를 허용하는 외부 데이터 플랫폼에 대한 연결입니다. 예를 들어 대상을 사용하여 DSP에서 지원하는 디지털 형식 전반에 걸친 타겟팅 광고에 대해 알려진 고객 관계(해시된 이메일 주소 등)를 활성화할 수 있습니다.

대상에 대한 자세한 내용은 Experience Platform 를 참조하십시오. [대상 안내서](https://experienceleague.adobe.com/docs/experience-platform/destinations/home.html), 제품 개요, 지침 포함 [대상 작업 공간 만들기](https://experienceleague.adobe.com/docs/experience-platform/destinations/ui/destinations-workspace.html) 및 [대상 연결 만들기](https://experienceleague.adobe.com/docs/experience-platform/destinations/ui/connect-destination.html), 및 [대상으로 데이터 활성화](https://experienceleague.adobe.com/docs/experience-platform/destinations/ui/activate/activate-segment-streaming-destinations.html).

### 과 DSP 통합을 사용하기 위한 워크플로우 [!DNL Real-time CDP] {#workflow-sources}

<!-- Make sure that titles make the distinctions clear -- everything can't be "Activate XXX." -->

1. [DSP에서 고객 데이터 세그먼트를 (으)로 번역하도록 허용 [!DNL LiveRamp RampIDs]](source-durable-id.md) 바인딩 가능한 환경에서 인식할 수 있습니다.<!-- I don't think I need this here: This requires DSP account-level and campaign-level settings to enable segment sharing with [!DNL LiveRamp], which will translate customer data to [!DNL RampIDs] to create targetable segments. Your DSP account team will perform this configuration. -->

1. [대상자 소스 만들기](source-create.md) DSP 계정 또는 광고주 계정으로 대상자를 가져오려면 다음을 수행하십시오.

1. [구성 [!DNL Real-Time CDP] Experience Platform의 대상 연결](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/advertising/adobe-advertising-cloud-connection.html).

추가 지원은 Adobe 계정 팀에 문의하거나 `adcloud-support@adobe.com`.

>[!MORELIKETHIS]
>
>* [지속 ID 파트너에서 인증된 세그먼트 활성화](source-durable-id.md)
>* [자사 대상을 활성화할 대상 소스 만들기](source-create.md)
>* [대상 소스 설정](source-settings.md)
>* [Adobe Advertising DSP 연결](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/advertising/adobe-advertising-cloud-connection.html)
>* Adobe Experience Platform [대상 카탈로그 개요](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/overview.html)
>* [대상자 관리 기본 정보](/help/dsp/audiences/audience-about.md)

