---
title: 검색, 소셜 및 Commerce 추적 전환 지표를  [!DNL Google Ads]에 업로드합니다.
description: 검색, 소셜 및 Commerce 추적 전환 지표를  [!DNL Google Ads]에 업로드하는 방법을 알아봅니다.
exl-id: 976792ae-135c-4790-82cf-9503edb93fb1
feature: Search Tools
TQID: https://experienceleague.adobe.com/ayxUfDgkrnPz0s-pFAdkmvYy94Il5szQHl6lYg8DpF8
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
source-git-commit: 527ca2bb74de388c13ba1ce5bde3f8be1cead8d0
workflow-type: tm+mt
source-wordcount: 212
ht-degree: 0%

---

# 검색, 소셜 및 Commerce에서 추적한 전환 지표를 [!DNL Google Ads]에 업로드합니다.

*계정 [!DNL Google Ads]개와 Adobe Advertising 전환 추적만 있는 광고주*

검색, 소셜 및 Commerce은 Adobe Advertising 전환 추적 서비스를 사용하는 [!DNL Google Ads] 캠페인에 대해 추적하는 모든 전환 지표를 [!DNL Google Ads]에 선택적으로 업로드할 수 있습니다. 이 옵션을 사용하면 하이브리드 최적화에 변환을 사용할 수 없습니다. 하이브리드 최적화에 Adobe 전환을 사용하려면 &quot;[광고 네트워크에 목표 업로드 사용](objective-upload-to-networks.md)&quot;을 참조하십시오.

일별 업로드에는 추적된 `gclid` 값, 광고주 수준 속성 모델을 사용하여 정의된 전환 값 및 타임스탬프가 포함됩니다. 속성 모델이 업데이트되면 다음 업로드에서 새 모델을 사용하지만, 이전 데이터는 새 모델을 사용하도록 업데이트되지 않습니다.

>[!NOTE]
>
>피드 파일에서 Adobe Advertising에 업로드되는 전환 지표는 업로드에 포함되지 않습니다.

1. 메인 메뉴에서 **[!UICONTROL Search, Social, & Commerce]> [!UICONTROL Tools] >[!UICONTROL Conversion Upload Setup]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Upload Conversions to Google Ads]** 옆의 확인란을 선택합니다.

1. (EEA(European Economic Area) 또는 영국(UK)에서 사업을 하는 광고주(선택 사항) EEA 및 영국 사용자로부터 광고 목적으로 데이터를 업로드하는 것에 대한 동의를 수집한 경우 **[!UICONTROL If you are doing business in EEA and/or UK, check this box to send consent status as GRANTED for the user data sent to [!DNL Google Ads] for advertising purposes. If left unchecked, we will send consent status as UNSPECIFIED for the user data sent to [!DNL Google Ads] for advertising purposes.]** 옆의 확인란을 선택합니다

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

1. (전환이 관리자 계정 수준에서 추적되는 경우) [&#x200B; > &#x200B;](/help/search-social-commerce/admin/manager-accounts.md) > **[!UICONTROL Search, Social, & Commerce]에서 [!UICONTROL Admin]관리자 계정에 대한 자격 증명을 추가[!UICONTROL Manager Accounts]**&#x200B;합니다.

>[!MORELIKETHIS]
>
>* [광고 네트워크에 목표를 업로드할 수 있도록 설정](objective-upload-to-networks.md)
