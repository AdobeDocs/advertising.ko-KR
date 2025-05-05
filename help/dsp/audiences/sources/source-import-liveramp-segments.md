---
title: ' [!DNL LiveRamp]에서 인증된 세그먼트 수동으로 가져오기'
description: ' [!DNL LiveRamp]을(를) 통해 인증된 대상을 활성화하는 방법에 대해 알아봅니다.'
feature: DSP Audiences
exl-id: c56a54c7-5300-4cda-96d0-82d86e76ee39
source-git-commit: 0a1555875fd18b326297475bc19fcfd6f28ea0c5
workflow-type: tm+mt
source-wordcount: '152'
ht-degree: 0%

---

# [!DNL LiveRamp]에서 인증된 세그먼트 수동으로 가져오기

*Beta 기능*

[!DNL LiveRamp] [!DNL Connect] 대시보드를 사용하여 인증된 [!DNL LiveRamp] 세그먼트를 수동으로 DSP에 보낼 수 있습니다. 가져온 세그먼트를 배치 타깃팅에 사용할 수 있습니다. 자사 세그먼트의 경우, 요금은 게재된 디스플레이 광고 노출당 USD 0.15이고 게재된 비디오 광고 노출당 USD 0.25입니다.

각 가져오기 작업에 대한 세그먼트 매핑 및 업로드는 최대 7일이 소요될 수 있습니다.

<!--Is this first step relevant for this process?

1. For measurement using [[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md):

   1. Complete all [prerequisites for implementing [!DNL Analytics for Advertising]](/help/integrations/analytics/prerequisites.md) and make sure that the [AMO ID and EF ID](/help/integrations/analytics/ids.md) are being populated in your tracking URLs.
   
   1. [Maybe just add a param to existing tag] Deploy a second JavaScript tag for [!DNL RampIDs] on your webpages to match onsite events to ad impressions. Contact your Adobe Account Team to get the tag and instructions for where to implement it.

 -->

1. [!DNL Connect] 대시보드에서 다음 단계를 완료하십시오.

   1. 대상 타일 **[!DNL AAC API 1P Onboarding]**&#x200B;을(를) 활성화합니다.

   1. [!DNL Identifier Settings]을(를) **[!DNL Ramp ID]**(으)로만 설정합니다.

      ![식별자 설정](/help/dsp/assets/liveramp-tile-settings.png)

   1. (선택 사항) 쿠키 기반 식별자를 계속 수신하려면 &quot;[!DNL Cookies]&quot;, &quot;[!DNL IDFA]&quot; 및 &quot;[!DNL AAID]&quot;이(가) 선택된 두 번째 [!DNL AAC API 1P Onboarding] 대상 타일을 만듭니다.

   1. 대상 라이브러리([!UICONTROL Audiences] > [!UICONTROL All Audiences]에서 대상을 만들거나 편집할 때 또는 배치 설정 내에서 사용 가능)에서 전체 세그먼트 수를 가져왔는지 확인합니다.

>[!MORELIKETHIS]
>
>* [자사 대상 소스 정보](source-about.md)
>* [범용 ID 대상을 활성화하기 위한 대상 소스 관리](source-manage.md)
>* [Adobe Advertising DSP 연결](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/advertising/adobe-advertising-cloud-connection.html?lang=ko)
>* [대상자 관리 정보](/help/dsp/audiences/audience-about.md)
