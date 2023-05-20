---
title: 자사 대상을 활성화할 대상 소스 만들기
description: 소스를 만들어 대상자를 계정 또는 광고주 계정으로 가져오는 방법에 대해 알아봅니다.
feature: DSP Audiences
exl-id: 728130d7-d19c-4d5d-9bca-695f8c17f89b
source-git-commit: 3347bfbaec92bb13428a39207954f895eb4f5d6d
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 3%

---

# 자사 대상을 활성화할 대상 소스 만들기

<!-- Will this remain for admin users/Adobe Account Team users only? -->

소스를 만들어 DSP 계정 또는 광고주 계정으로 대상자를 가져옵니다. 현재,에서 대상자를 가져올 수 있습니다. [다음 [!DNL Adobe Real-Time Customer Data Profile (CDP)]](https://experienceleague.adobe.com/docs/experience-platform/rtcdp/overview.html?lang=ko).

>[!NOTE]
>
>다음에 대한 소스를 만든 후 [!DNL Real-Time CDP], 을(를) 활성화해야 합니다. [!DNL Real-Time CDP] 내의 Adobe Advertising DSP 대상을 통한 대상 [!DNL Real-Time CDP] 가져오기를 시작합니다. 다음을 참조하십시오 [활성화 워크플로의 단계](source-about.md#workflow-sources).

1. 메인 메뉴에서 **[!UICONTROL Audiences]** > **[!UICONTROL Sources]**.

1. 클릭 [!UICONTROL Add Source].

1. 다음에서 [!UICONTROL Select a Type] 메뉴에서 소스 유형을 선택합니다.

   *[!UICONTROL RT-CDP]*: 이 소스 유형, 대상 [다음 [!DNL Adobe Real-Time Customer Data Profile]](source-about.md)는 유일한 옵션입니다.

1. 다음을 지정합니다. [!UICONTROL Data Visibility Level]: *[!UICONTROL Advertiser]* 또는 *[!UICONTROL Account]*.

1. 나머지 항목 입력 [소스 설정](source-settings.md).

   복사본 보관 [!UICONTROL Source Key] 생성됩니다. 나중에 값이 필요합니다.

1. 클릭 **[!UICONTROL Save]**.

1. Experience Platform에서 를 사용하여 Advertising DSP 대상 연결을 만듭니다. [!UICONTROL Source Key] DSP 소스 설정에서 생성되었습니다.

   DSP 대상 연결을 활성화하고, 세그먼트를 선택하고, 제어 권한에 액세스하는 방법에 대한 지침은 &quot;[Adobe Advertising Cloud DSP 연결](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/advertising/adobe-advertising-cloud-connection.html).&quot;

>[!MORELIKETHIS]
>
>* [대상 소스 설정](source-settings.md)
>* [대상 소스에서 인증된 세그먼트 활성화 정보](source-about.md)
>* [지속 ID 파트너에서 인증된 세그먼트 활성화](source-durable-id.md)<!-- title?-->
>* [Adobe Advertising Cloud DSP 연결](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/advertising/adobe-advertising-cloud-connection.html)
>* [대상자 관리 기본 정보](/help/dsp/audiences/audience-about.md)

