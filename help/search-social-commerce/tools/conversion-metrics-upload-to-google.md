---
title: 전환 지표 업로드 [!DNL Google Ads]
description: 검색, 소셜 및 상거래 추적 전환 지표를 로 업로드하는 방법을 알아봅니다 [!DNL Google Ads].
exl-id: 976792ae-135c-4790-82cf-9503edb93fb1
feature: Search Tools
source-git-commit: a004f5025ee94c6a40c24124a9cb134a4e1668ce
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---

# 전환 지표 업로드 [!DNL Google Ads]

*를 사용하는 광고주 [!DNL Google Ads] 계정만*

검색, 소셜 및 상거래를 선택적으로 업로드할 수 있습니다. [!DNL Google Ads] 추적되는 모든 전환 지표 [!DNL Google Ads] Adobe Advertising 전환 추적 서비스를 사용하는 캠페인. 이 옵션을 사용하면 하이브리드 최적화에 변환을 사용할 수 없습니다. 하이브리드 최적화에 Adobe 전환을 사용하려면 &quot;[광고 네트워크에 목표 업로드 활성화](objective-upload-to-networks.md).&quot;

일별 업로드에는 추적된 내용이 포함됩니다 `gclid` 값, 광고주 수준 속성 모델을 사용하여 정의된 전환 값 및 타임스탬프입니다. 속성 모델이 업데이트되면 다음 업로드에서 새 모델을 사용하지만, 이전 데이터는 새 모델을 사용하도록 업데이트되지 않습니다.

>[!NOTE]
>
>피드 파일에서 Adobe Advertising에 업로드되는 변환 지표는 업로드에 포함되지 않습니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Tools] >[!UICONTROL Conversion Upload Setup]**.

1. 옆에 있는 확인란을 선택합니다. **[!UICONTROL Upload Conversions to Google Ads]**.

1. (EEA(European Economic Area) 또는 영국(UK)에서 비즈니스를 수행하는 광고주; 선택 사항) EEA 및 영국 사용자로부터 광고 목적으로 데이터를 업로드하는 것에 대한 동의를 확보한 경우, 다음 옆의 확인란을 선택합니다 **[!UICONTROL If you are doing business in EEA and/or UK, check this box to send consent status as GRANTED for the user data sent to [!DNL Google Ads] for advertising purposes. If left unchecked, we will send consent status as UNSPECIFIED for the user data sent to [!DNL Google Ads] for advertising purposes.]**

1. 클릭 **[!UICONTROL Save]**.

1. (관리자 계정 수준에서 전환을 추적하는 경우) [관리자 계정에 대한 자격 증명 추가](/help/search-social-commerce/admin/manager-accounts.md) 위치: **[!UICONTROL Search]> [!UICONTROL Admin] >[!UICONTROL Manager Accounts]**.

>[!MORELIKETHIS]
>
>* [광고 네트워크에 목표 업로드 활성화](objective-upload-to-networks.md)
