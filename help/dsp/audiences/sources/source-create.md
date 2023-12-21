---
title: 자사 대상을 활성화할 대상 소스 만들기
description: 소스를 만들어 대상자를 계정 또는 광고주 계정으로 가져오는 방법에 대해 알아봅니다.
feature: DSP Audiences
exl-id: 728130d7-d19c-4d5d-9bca-695f8c17f89b
source-git-commit: 6c918b387067237de5d1eae42ae8ad253884d761
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# 자사 대상을 활성화할 대상 소스 만들기

<!-- Will this remain for admin users/Adobe Account Team users only? -->

DSP에서 소스를 만들어 자사 대상을 DSP 계정 또는 광고주 계정으로 가져옵니다.

특정 고객 데이터 플랫폼에서 세그먼트를 수집하는 데 필요한 추가 단계는 [대상별 활성화 워크플로](source-about.md)

1. 메인 메뉴에서 **[!UICONTROL Audiences]** > **[!UICONTROL Sources]**.

1. 클릭 **[!UICONTROL Add Source]**.

1. 다음에서 [!UICONTROL Select a Type] 메뉴에서 소스 유형을 선택합니다.

   * *[!UICONTROL RT-CDP]*: [다음 [!DNL Adobe Real-Time Customer Data Platform]](source-about.md).

   <!-- * *[!UICONTROL ActionIQ]*: The [[!DNL ActionIQ] customer data platform](source-about.md). -->

   * *[!UICONTROL Tealium CDP]*: [[!DNL Tealium] 고객 데이터 플랫폼](source-about.md).

1. 다음을 지정합니다. [!UICONTROL Data Visibility Level]: *[!UICONTROL Advertiser]* 또는 *[!UICONTROL Account]*.

1. 나머지 항목 입력 [소스 설정](source-settings.md).

   복사본 보관 [!UICONTROL Source Key] 생성됩니다. 나중에 값이 필요합니다.

1. 클릭 **[!UICONTROL Save]**.

>[!NOTE]
>
>고객 데이터 플랫폼에 대한 소스를 만든 후에는 추가 단계를 완료해야 합니다. 다음을 참조하십시오. [활성화 워크플로 [!DNL Adobe] [!DNL Real-time CDP]](source-adobe-rtcdp.md)<!-- the [activation workflow for [!DNL ActionIQ]](source-actioniq.md), --> 및 [활성화 워크플로 [!DNL Tealium]](source-tealium.md).

>[!MORELIKETHIS]
>
>* [대상 소스 설정](source-settings.md)
>* [대상 소스에서 인증된 세그먼트 활성화 정보](source-about.md)
>* [범용 ID 파트너에서 인증된 세그먼트 활성화](source-universal-id.md)<!-- title?-->
>* [Adobe Advertising Cloud DSP 연결](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/advertising/adobe-advertising-cloud-connection.html)
>* [대상자 관리 기본 정보](/help/dsp/audiences/audience-about.md)
