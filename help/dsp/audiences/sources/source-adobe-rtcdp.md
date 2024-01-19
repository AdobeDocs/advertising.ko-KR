---
title: 과 DSP 통합을 사용하기 위한 워크플로우 [!DNL Adobe] [!DNL Real-time CDP]
description: DSP을 활성화하여 다음을 수집하는 방법 알아보기 [!DNL Adobe] [!DNL Real-time CDP] 자사 세그먼트.
feature: DSP Audiences
exl-id: cb1da95b-0d19-4450-8770-6c383248ddae
source-git-commit: b94541bf8675d535b2f19b26c05235eb56bc6c0b
workflow-type: tm+mt
source-wordcount: '143'
ht-degree: 0%

---

# 과 DSP 통합을 사용하기 위한 워크플로우 [!DNL Adobe Real-Time CDP]

1. [DSP에서 고객 데이터 세그먼트를 (으)로 번역하도록 허용 [!DNL LiveRamp RampIDs]](source-universal-id.md) 바인딩 가능한 환경에서 인식할 수 있습니다.<!-- I don't think I need this here: This requires DSP account-level and campaign-level settings to enable segment sharing with [!DNL LiveRamp], which will translate customer data to [!DNL RampIDs] to create targetable segments. Your Adobe Account Team will perform this configuration. -->

1. [대상자 소스 만들기](source-create.md) DSP 계정 또는 광고주 계정으로 대상자를 가져오려면 다음을 수행하십시오.

1. Experience Platform에서 다음을 사용하여 Advertising DSP 대상 연결을 구성합니다. [!UICONTROL Source Key] DSP 소스 설정에서 생성되었습니다.

   DSP 대상 연결을 활성화하고, 세그먼트를 선택하고, 제어 권한에 액세스하는 방법에 대한 지침은 &quot;[Adobe Advertising Cloud DSP 연결](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/advertising/adobe-advertising-cloud-connection.html).&quot;

추가 지원은 Adobe 계정 팀에 문의하거나 `adcloud-support@adobe.com`.


>[!MORELIKETHIS]
>
>* [범용 ID 파트너에서 인증된 세그먼트 활성화](source-universal-id.md)
>* [자사 대상을 활성화할 대상 소스 만들기](source-create.md)
>* [대상 소스 설정](source-settings.md)
>* [Adobe Advertising DSP 연결](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/advertising/adobe-advertising-cloud-connection.html)
>* Adobe Experience Platform [대상 카탈로그 개요](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/overview.html)
>* [과 DSP 통합을 사용하기 위한 워크플로우 [!DNL Tealium]](/help/dsp/audiences/sources/source-tealium.md)
>* [대상자 관리 기본 정보](/help/dsp/audiences/audience-about.md)
