---
title: 광고 네트워크에 목표 업로드 사용 설정
description: 하이브리드 포트폴리오 [!DNL Google Ads] 에 대한 목표를 and에 [!DNL Microsoft Advertising] 업로드 하는 방법을 알아보십시오.
exl-id: 09ab0b7a-b6ea-45ad-a82c-2c40d518d2e7
feature: Search Tools
source-git-commit: 803f1ad2ad5be005b7dab467efbeb1c4ceaa7559
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# 광고 네트워크에 목표 업로드 사용 설정

*및 [!DNL Microsoft Advertising] 계정이 있는 [!DNL Google Ads] 광고주 전용*

*하이브리드 최적화만 사용할 수 있는 광고주*

Search, Social 및 상거래는 광고주 계정 포트폴리오 [!DNL Google Ads] [!DNL Microsoft Advertising] 에 대한 목표를 업로드할 수 있으므로 하이브리드 최적화에 사용할 수 있습니다. 업로드된 목표는 계정 수준 및 캠페인 수준의 맞춤 전환 목표에 대한 전환 작업으로 사용할 수 있습니다.

이 옵션을 사용 설정하면 스마트 자동 입찰 전략이 있는 캠페인이 포함된 포트폴리오의 목표에 대한 업로드 작업이 자동으로 트리거됩니다. Search, Social 및 Commerce는 적용 가능한 각 목표에 대해 광고 네트워크 상에서 전환을 생성합니다. 전환은 목표의 모든 가중치가 적용된 전환 지표를 나타냅니다. 각 전환 이름에는 다음 이름 중 하나가 있습니다.

* `O_ACS_OBJ_<network_ID>_<objective_ID>_<network_account_ID>`

  여기서 `<network_ID>` 은 Search, Social 및 상거래에서 광고 네트워크에 사용하는 숫자 ID이고, `<objective_id>` 는 숫자 목표 ID이고, `<network_account_ID>` 는 광고 네트워크 계정 또는 관리자 계정의 숫자 ID입니다.

* (향후 더 이상 사용되지 않는 이전 포맷) `ACS_OBJ_SID_<portfolio_id>_<se_acctid/conversion_manager_se_acctid>`

  여기서 `<portfolio_id>` 은 숫자 포트폴리오 ID이고 `<se_acctid/conversion_manager_se_acctid>` 은 광고 네트워크 계정 또는 관리자 계정의 숫자 ID입니다.

  Adobe Systems 계정 팀은 사용자와 협력하여 이전 포맷이 더 이상 사용되지 않기 전에 광고 네트워크 내에서 기존 전환 작업 이름을 마이그레이션합니다. 마이그레이션 기간 동안 이전 포맷 업로드와 새  업로드가 모두 동시에 실행됩니다. 모델링 및 최적화는 새로운 전환 작업이 처음에 &#39;보조&#39;(최적화되지 않음) 상태와 90일간의 채우기 데이터로 표시되기 때문에 영향을 받지 않습니다.

업로드는 [!DNL Google Ads] 광고주 표준 시간대로 매일 06:00에 발생합니다. 업로드는 [!DNL Microsoft Advertising] 광고주 표준 시간대로 매일 09:00에 발생합니다.

>[!IMPORTANT]
>
>Google Ads 및 Microsoft Advertising 유니버설 이벤트 추적(UET) 태그에 의해 추적된 전환은 광고 네트워크에 다시 업로드되지 않습니다. 목표 내에 포함하는 경우 광고 네트워크 편집기 내에서 캠페인 목표에 추가하세요.

<!--
>[!IMPORTANT]
>
>Objectives for hybrid portfolios may include conversion goals from multiple ad networks and other types of conversion metrics. However, the individual campaigns in the portfolio can't include conversion goals that aren't included in the portfolio's objective; using additional conversion goals may impact portfolio performance.
-->

<!-- Can conversions from events triggered on other ad networks be included in the portfolio (and just be ignored)? -->

1. 주 메뉴에서 > [!UICONTROL Tools] > [!UICONTROL Conversion Upload Setup]**을 클릭합니다**[!UICONTROL Search] .

1. 옆에 **[!UICONTROL Enable Objective Upload]**&#x200B;있는 확인란을 선택합니다.

1. (유럽 경제 지역(EEA) 또는 영국(UK)에서 비즈니스를 운영하는 계정이 있는 [!DNL Google Ads] 광고주, 선택사항) EEA 및 영국 사용자로부터 광고 목적으로 데이터를 업로드하는 것에 대한 동의를 얻은 경우 **[!UICONTROL If you are doing business in EEA and/or UK, check this box to send consent status as GRANTED for the user data sent to [!DNL Google Ads] for advertising purposes. If left unchecked, we will send consent status as UNSPECIFIED for the user data sent to [!DNL Google Ads] for advertising purposes.]**

1. 을 누르십시오 **[!UICONTROL Save]**.

1. (전환이 관리자 계정 수준에서 추적되는 경우) [> >**[!UICONTROL Search][!UICONTROL Manager Accounts]**&#x200B;에서 관리자 계정](/help/search-social-commerce/admin/manager-accounts.md) [!UICONTROL Admin] 에 대한 자격 증명을 추가합니다.

1. 이름이 지정된 `O_ACS_OBJ_<network_ID>_<objective_ID>_<network_account_ID>` 각 목표가 광고 네트워크 상에서 2일 이내에 표시되는지 확인합니다.

   [!DNL Google Ads] 편집기에서 전환 작업을](https://support.google.com/google-ads/answer/11461796) 조회합니다[. [!DNL Microsoft Advertising] 편집기에서 전환 목표를](https://help.ads.microsoft.com/#apex/ads/en/56709) 조회합니다[.

   필요한 경우 업로드 날짜를 포함하도록 날짜 범위를 업데이트합니다.

## 누락된 목표 문제 해결

포트폴리오 중 하나에 대한 목표(이름이 지정 `O_ACS_OBJ_<network_ID>_<objective_ID>_<network_account_ID>` 됨)가 광고 네트워크 페이지에 표시되지 않으면 다음을 확인하세요.

* ([!DNL Google Ads]) 전환을 계정 또는 관리자 수준으로 업로드해야 하는지 확인합니다. 관리자 수준에서 업로드해야 하는 경우:

   * 관리자 계정에 대한 자격 증명이 [!DNL Google Ads] > [!UICONTROL Admin] >[!UICONTROL Manager Accounts]**에서 제공**[!UICONTROL Search] 되는지 확인합니다. 필요한 [경우 관리자 계정](/help/search-social-commerce/admin/manager-accounts.md) 인증 정보를 추가합니다.

   * 광고 네트워크 계정에 이미 동일한 지표 이름이 포함되어 있는지 확인합니다. 이 경우 올바른 관리자 수준 속성을 만들 수 있도록 지표의 이름을 바꿉니다.

* 포트폴리오의 &quot;하이브리드&quot; 옵션이 선택되어 있고 목표에 유효한 매출이 있는지 확인합니다.

>[!MORELIKETHIS]
>
>* [광고주의 전환 지표 관리 정보](/help/search-social-commerce/admin/conversion-metrics/conversion-metric-about.md)
>* [전환 지표를 업로드 대상 [!DNL Google Ads]](conversion-metrics-upload-to-google.md)
