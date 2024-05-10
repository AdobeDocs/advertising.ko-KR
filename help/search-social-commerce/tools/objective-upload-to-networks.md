---
title: 광고 네트워크에 목표 업로드 활성화
description: 하이브리드 포트폴리오에 대한 목표를 업로드하는 방법을 알아봅니다. [!DNL Google Ads] 및 [!DNL Microsoft Advertising].
exl-id: 09ab0b7a-b6ea-45ad-a82c-2c40d518d2e7
feature: Search Tools
source-git-commit: 67fe8581832dc0762d62908d01672e53cc95b847
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# 광고 네트워크에 목표 업로드 활성화

*를 사용하는 광고주 [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 계정만*

*하이브리드 최적화에만 활성화된 광고주*

Search, Social 및 Commerce은 광고주 계정의 포트폴리오에 대한 목표를 업로드할 수 있습니다. [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 따라서 하이브리드 최적화에 사용할 수 있습니다. 업로드한 목표는 계정 수준 및 캠페인 수준의 사용자 정의 전환 목표에 대한 전환 작업으로 사용할 수 있습니다.

이 옵션을 활성화하면 스마트 입찰 전략이 포함된 캠페인이 포함된 포트폴리오에서 목표에 대한 업로드가 자동으로 트리거됩니다. Search, Social 및 Commerce은 적용 가능한 각 목표에 대해 광고 네트워크에서 전환을 만듭니다. 전환은 목표의 모든 가중 전환 지표를 나타냅니다. 각 전환에는 다음 이름 중 하나가 있습니다.

* `O_ACS_OBJ_<network_ID>_<objective_ID>_<network_account_ID>`

  위치 `<network_ID>` 는 Search, Social 및 Commerce이 광고 네트워크에 사용하는 숫자 ID입니다. `<objective_id>` 는 숫자 목표 ID이고, `<network_account_ID>` 광고 네트워크 계정 또는 관리자 계정의 숫자 ID입니다.

* (나중에 더 이상 사용되지 않는 이전 형식) `ACS_OBJ_SID_<portfolio_id>_<se_acctid/conversion_manager_se_acctid>`

  위치 `<portfolio_id>` 는 숫자 포트폴리오 ID이고 `<se_acctid/conversion_manager_se_acctid>` 광고 네트워크 계정 또는 관리자 계정의 숫자 ID입니다.

  Adobe 계정 팀은 이전 형식이 더 이상 사용되지 않기 전에 광고 네트워크 내에서 기존 전환 작업 이름을 마이그레이션하도록 사용자와 협력합니다. 마이그레이션 기간 동안 이전 형식과 새 형식 업로드가 모두 동시에 실행됩니다. 새 전환 작업이 처음에 &quot;보조&quot;(최적화되지 않음) 상태와 90일의 데이터 채우기로 표시되므로 모델링 및 최적화는 영향을 받지 않습니다.

에 업로드 [!DNL Google Ads] 광고주의 시간대에서 매일 06:00에 발생합니다. 에 업로드 [!DNL Microsoft Advertising] 광고주의 시간대에서 매일 09:00에 발생합니다.

>[!IMPORTANT]
>
>Google 광고 및 Microsoft Advertising UET(범용 이벤트 추적) 태그로 추적된 전환은 광고 네트워크에 다시 업로드되지 않습니다. 목표에 이러한 목표를 포함하는 경우 광고 네트워크의 편집기 내에서 캠페인 목표에 해당 목표를 추가합니다.

<!--
>[!IMPORTANT]
>
>Objectives for hybrid portfolios may include conversion goals from multiple ad networks and other types of conversion metrics. However, the individual campaigns in the portfolio can't include conversion goals that aren't included in the portfolio's objective; using additional conversion goals may impact portfolio performance.
-->

<!-- Can conversions from events triggered on other ad networks be included in the portfolio (and just be ignored)? -->

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Tools] >[!UICONTROL Conversion Upload Setup]**.

1. 옆에 있는 확인란을 선택합니다. **[!UICONTROL Enable Objective Upload]**.

1. (광고주: [!DNL Google Ads] 유럽 경제 지역(EEA) 또는 영국(영국)에서 비즈니스를 수행하는 계정(선택 사항) EEA 및 영국 사용자로부터 광고 목적으로 데이터를 업로드하는 것에 대한 동의를 수집한 경우 다음 옆에 있는 확인란을 선택합니다 **[!UICONTROL If you are doing business in EEA and/or UK, check this box to send consent status as GRANTED for the user data sent to [!DNL Google Ads] for advertising purposes. If left unchecked, we will send consent status as UNSPECIFIED for the user data sent to [!DNL Google Ads] for advertising purposes.]**

1. 클릭 **[!UICONTROL Save]**.

1. (관리자 계정 수준에서 전환을 추적하는 경우) [관리자 계정에 대한 자격 증명 추가](/help/search-social-commerce/admin/manager-accounts.md) 위치: **[!UICONTROL Search]> [!UICONTROL Admin] >[!UICONTROL Manager Accounts]**.

일별 업로드가 완료되면 전환 작업이 광고 네트워크에 표시되는지 확인할 수 있습니다.

>[!MORELIKETHIS]
>
>* [광고주의 전환 지표 관리 정보](/help/search-social-commerce/admin/conversion-metrics/conversion-metric-about.md)
>* [전환 지표 업로드 [!DNL Google Ads]](conversion-metrics-upload-to-google.md)
