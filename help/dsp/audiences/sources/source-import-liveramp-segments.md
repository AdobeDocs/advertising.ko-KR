---
title: 에서 인증된 세그먼트 수동으로 가져오기 [!DNL LiveRamp]
description: 다음을 통해 인증된 대상 활성화에 대해 알아보기 [!DNL LiveRamp].
feature: DSP Audiences
exl-id: c56a54c7-5300-4cda-96d0-82d86e76ee39
source-git-commit: f10a0bd487d641bd150d9ecbefe907b2bf25e5a7
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 0%

---

# 에서 인증된 세그먼트 수동으로 가져오기 [!DNL LiveRamp]

*Beta 기능*

인증된 파일을 수동으로 보낼 수 있습니다. [!DNL LiveRamp] 세그먼트를 사용하여 DSP에 [!DNL LiveRamp] [!DNL Connect] 대시보드입니다. 가져온 세그먼트를 배치 타깃팅에 사용할 수 있습니다. 자사 세그먼트의 경우, 요금은 게재된 디스플레이 광고 노출당 USD 0.15이고 게재된 비디오 광고 노출당 USD 0.25입니다.

각 가져오기 작업에 대한 세그먼트 매핑 및 업로드는 최대 7일이 소요될 수 있습니다.

<!--Is this first step relevant for this process?

1. For measurement using [[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md):

   1. Complete all [prerequisites for implementing [!DNL Analytics for Advertising]](/help/integrations/analytics/prerequisites.md) and make sure that the [AMO ID and EF ID](/help/integrations/analytics/ids.md) are being populated in your tracking URLs.
   
   1. [Maybe just add a param to existing tag] Deploy a second JavaScript tag for [!DNL RampIDs] on your webpages to match onsite events to ad impressions. Contact your Adobe Account Team to get the tag and instructions for where to implement it.

 -->

1. 에서 다음 단계를 완료합니다 [!DNL Connect] 대시보드:

   1. 대상 타일 활성화 **[!DNL AAC API 1P Onboarding]**.

   1. 설정 [!DNL Identifier Settings] 끝 **[!DNL Ramp ID]** 만 해당.

      ![식별자 설정](/help/dsp/assets/liveramp-tile-settings.png)

   1. (선택 사항) 쿠키 기반 식별자를 계속 수신하려면 두 번째 식별자를 만듭니다 [!DNL AAC API 1P Onboarding] 대상 타일(&quot;&quot;)[!DNL Cookies],&quot; &quot;[!DNL IDFA],&quot; 및 &quot;[!DNL AAID]&quot;선택됨.

   1. 대상 라이브러리에서 확인합니다(에서 대상을 만들거나 편집할 때 사용 가능). [!UICONTROL Audiences] > [!UICONTROL All Audiences] 또는 배치 설정 내에서) 전체 세그먼트 수를 가져왔습니다.

>[!MORELIKETHIS]
>
>* [자사 대상 소스 정보](source-about.md)
>* [범용 ID 대상을 활성화하는 대상 소스 만들기](source-create.md)
>* [대상 소스 설정](source-settings.md)
>* [Adobe Advertising DSP 연결](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/advertising/adobe-advertising-cloud-connection.html)
>* [대상자 관리 기본 정보](/help/dsp/audiences/audience-about.md)
