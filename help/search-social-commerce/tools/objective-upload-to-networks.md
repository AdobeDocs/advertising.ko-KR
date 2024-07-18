---
title: 광고 네트워크에 목표 업로드 활성화
description: 하이브리드 포트폴리오의 목표를  [!DNL Google Ads] 및 [!DNL Microsoft Advertising]에 업로드하는 방법을 알아봅니다.
exl-id: 09ab0b7a-b6ea-45ad-a82c-2c40d518d2e7
feature: Search Tools
source-git-commit: f491537c2dd56716abe0ab4fa8c26b8558dca664
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 0%

---

# 광고 네트워크에 목표 업로드 활성화

*[!DNL Google Ads] 및 [!DNL Microsoft Advertising] 계정만 있는 광고주*

*하이브리드 최적화에만 사용할 수 있는 광고주*

Search, Social 및 Commerce에서 광고주 계정의 포트폴리오의 목표를 [!DNL Google Ads] 및 [!DNL Microsoft Advertising]에 업로드하여 하이브리드 최적화에 사용할 수 있습니다. 업로드한 목표는 계정 수준 및 캠페인 수준의 사용자 정의 전환 목표에 대한 전환 작업으로 사용할 수 있습니다.

이 옵션을 활성화하면 스마트 입찰 전략이 포함된 캠페인이 포함된 포트폴리오에서 목표에 대한 업로드가 자동으로 트리거됩니다. Search, Social 및 Commerce은 적용 가능한 각 목표에 대해 광고 네트워크에서 전환을 만듭니다. 전환은 EF ID(클릭 ID) 수준에서 목표의 모든 가중 전환 지표를 나타냅니다. [!DNL Google Ads] 클릭의 경우 EF ID는 [!DNL Google Ads] `gclid`이고, [!DNL Microsoft Advertising] 클릭의 경우 EF ID는 [!DNL Microsoft Advertising] `msclkid`입니다. 이 클릭 ID로 인해 전환 데이터가 특정 키워드 및 클릭 시간에 매핑될 수 있습니다.

업로드된 각 전환의 이름은 다음과 같습니다.

`O_ACS_OBJ_<network_ID>_<objective_ID>_<network_account_ID>`

여기서 `<network_ID>`은(는) Search, Social 및 Commerce에서 광고 네트워크에 사용하는 숫자 ID이고, `<objective_id>`은(는) 숫자 목표 ID이며, `<network_account_ID>`은(는) 광고 네트워크 계정 또는 관리자 계정에 대한 숫자 ID입니다.

[!DNL Google Ads]에 대한 업로드는 광고주 시간대의 06:00에 매일 발생합니다. [!DNL Microsoft Advertising]에 대한 업로드는 광고주 시간대의 09:00에 매일 발생합니다.

>[!IMPORTANT]
>
>Google 광고 및 Microsoft Advertising UET(범용 이벤트 추적) 태그로 추적된 전환은 광고 네트워크에 다시 업로드되지 않습니다. 목표에 이러한 목표를 포함하는 경우 광고 네트워크의 편집기 내에서 캠페인 목표에 해당 목표를 추가해야 합니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Tools] >[!UICONTROL Conversion Upload Setup]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Enable Objective Upload]** 옆의 확인란을 선택합니다.

1. (EEA(European Economic Area) 또는 영국(United Kingdom)에서 비즈니스를 수행하는 [!DNL Google Ads] 계정이 있는 광고주(선택 사항) EEA 및 영국 사용자로부터 광고 목적으로 데이터를 업로드하는 것에 대한 동의를 수집한 경우 **[!UICONTROL If you are doing business in EEA and/or UK, check this box to send consent status as GRANTED for the user data sent to [!DNL Google Ads] for advertising purposes. If left unchecked, we will send consent status as UNSPECIFIED for the user data sent to [!DNL Google Ads] for advertising purposes.]** 옆의 확인란을 선택합니다

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

1. (전환이 관리자 계정 수준에서 추적되는 경우) **[!UICONTROL Search]> [!UICONTROL Admin] >[!UICONTROL Manager Accounts]**&#x200B;에서 [관리자 계정에 대한 자격 증명을 추가](/help/search-social-commerce/admin/manager-accounts.md)합니다.

1. 광고 네트워크에 이틀 안에 `O_ACS_OBJ_<network_ID>_<objective_ID>_<network_account_ID>`(이)라는 각 목표가 표시되는지 확인하십시오.

   [!DNL Google Ads] 편집기에서 [전환 작업](https://support.google.com/google-ads/answer/11461796)을 조회합니다. [!DNL Microsoft Advertising] 편집기에서 [전환 목표](https://help.ads.microsoft.com/#apex/ads/en/56709)를 조회합니다.

   필요한 경우 업로드 날짜를 포함하도록 날짜 범위를 업데이트합니다.

## 가중 목표 계산 방법

광고 네트워크에 전달된 가중 목표는 [!DNL Google Ads] 또는 [!DNL Microsoft Advertising] UET(범용 이벤트 추적) 태그에 의해 추적된 전환을 제외하고 수집된 모든 지표 값의 합계입니다. 값은 광고주의 Search, Social 및 Commerce 계정에 대해 설정된 속성 방법을 사용하여 계산됩니다.

예를 들어 목표의 목표 지표가 가중치가 25인 장바구니 추가이고, 지원 지표에는 가중치가 1인 GGL_Lead 및 매출 과 가중치가 0.5인 다운로드 가 있다고 가정해 보겠습니다.

![가중 목표의 예](/help/search-social-commerce/assets/objective-example.png "가중 목표의 예")

키워드가 포트폴리오에 대해 다음 작업을 수행했다고 가정해 보십시오.

* 장바구니 추가 10개
* 매출 500달러
* 50개 다운로드
* 5GGL_Lead

GGL_Lead 는 Google 광고 추적 지표이므로 계산/업로드에 포함되지 않습니다. 따라서 가중 목적값은 ((10 x 25) + (500 x 1) + (50 x 0.5)) = 775로 계산된다.

>[!TIP]
>
>광고 네트워크의 보고서 내에서 Adobe Advertising 가중 매출에 대한 데이터를 볼 수 있습니다. 가장 좋은 방법은 가중 수익을 [!DNL Google Ads] &quot;모든 conv&quot;와(과) 비교하는 것입니다. (conv에 의해. time)&quot; 지표 또는 [!DNL Microsoft Advertising] 지표 &quot;All conv. O_ACS_OBJ* 지표로 세그먼트화된 매출액.<!--clarify -->

## 누락된 목표 문제 해결

포트폴리오 중 하나에 대한 목표(`O_ACS_OBJ_<network_ID>_<objective_ID>_<network_account_ID>`)가 광고 네트워크에 표시되지 않으면 다음을 확인하십시오.

* ([!DNL Google Ads]) 전환을 계정 또는 관리자 수준으로 업로드해야 하는지 확인하십시오. 관리자 수준에서 업로드해야 하는 경우:

   * [!DNL Google Ads] 관리자 계정의 자격 증명이 **[!UICONTROL Search]> [!UICONTROL Admin] >[!UICONTROL Manager Accounts]**&#x200B;에 제공되었는지 확인하십시오. 필요한 경우 [관리자 계정에 대한 자격 증명을 추가](/help/search-social-commerce/admin/manager-accounts.md)하십시오.

   * 광고 네트워크 계정에 이미 동일한 지표 이름이 포함되어 있는지 확인합니다. 그럴 경우 올바른 관리자 수준 속성을 만들 수 있도록 지표의 이름을 변경합니다.

* 포트폴리오의 &quot;하이브리드&quot; 옵션이 선택되어 있고 목표에 유효한 수익이 있는지 확인하십시오.

>[!MORELIKETHIS]
>
>* [광고주의 전환 지표 관리 정보](/help/search-social-commerce/admin/conversion-metrics/conversion-metric-about.md)
>* [전환 지표를  [!DNL Google Ads]](conversion-metrics-upload-to-google.md)에 업로드
