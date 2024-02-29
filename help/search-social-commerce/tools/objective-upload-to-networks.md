---
title: 광고 네트워크에 목표 업로드 활성화
description: 하이브리드 포트폴리오에 대한 목표를 업로드하는 방법을 알아봅니다. [!DNL Google Ads] 및 [!DNL Microsoft® Advertising].
exl-id: 09ab0b7a-b6ea-45ad-a82c-2c40d518d2e7
feature: Search Tools
source-git-commit: 0fb03410e67be28d24496c948b52399c8465e041
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# 광고 네트워크에 목표 업로드 활성화

*를 사용하는 광고주 [!DNL Google Ads] 및 [!DNL Microsoft® Advertising] 계정만*

*하이브리드 최적화에만 활성화된 광고주*

광고주 계정이 하이브리드 최적화를 사용하도록 구성되어 있는 경우 Adobe Advertising은 필요에 따라 계정의 포트폴리오에 대한 목표를 업로드할 수 있습니다. [!DNL Google Ads] 및 [!DNL Microsoft® Advertising] 하이브리드 최적화에 사용할 수 있는 전환으로.

이 옵션을 활성화하면 스마트 입찰 전략이 포함된 캠페인이 포함된 포트폴리오에 대한 업로드가 자동으로 트리거됩니다. Search, Social 및 Commerce는 해당되는 각 포트폴리오와 객관적인 조합에 대해 광고 네트워크에서 전환을 만듭니다. 각 전환에는 이름이 있습니다. `ACS_OBJ_SID_<portfolio_id>_<se_acctid/conversion_manager_se_acctid>`, 여기서 `<portfolio_id>` 는 숫자 포트폴리오 ID이고 `<se_acctid/conversion_manager_se_acctid>` 광고 네트워크 계정 또는 관리자 계정의 숫자 ID입니다. 전환은 목표의 모든 가중 전환 지표를 나타냅니다.

에 업로드 [!DNL Google Ads] 광고주의 시간대에서 매일 06:00에 발생합니다. 에 업로드 [!DNL Microsoft® Advertising] 광고주의 시간대에서 매일 09:00에 발생합니다.

<!-- Note to self: Conversions tracked by Google Ads and by the Microsoft Advertising universal event tracking (UET) tag aren't re-uploaded to the ad networks. -->

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Tools] >[!UICONTROL Conversion Upload Setup]**.

1. 옆에 있는 확인란을 선택합니다. **[!UICONTROL Enable Objective Upload]**.

   이 옵션은 광고주 계정이 하이브리드 최적화를 사용하도록 구성된 경우에만 사용할 수 있습니다. 하이브리드 최적화를 활성화하려면 Adobe 계정 팀에 문의하십시오.

1. (광고주: [!DNL Google Ads] 유럽 경제 지역(EEA) 또는 영국(UK)에서 비즈니스를 수행하는 계정(선택 사항) EEA 및 영국 사용자로부터 광고 목적으로 데이터를 업로드하는 것에 대한 동의를 확보한 경우 다음 옆에 있는 확인란을 선택합니다. **[!UICONTROL If you are doing business in EEA and/or UK, check this box to send consent status as GRANTED for the user data sent to [!DNL Google Ads] for advertising purposes. If left unchecked, we will send consent status as UNSPECIFIED for the user data sent to [!DNL Google Ads] for advertising purposes.]**

1. 클릭 **[!UICONTROL Save]**.

1. (관리자 계정 수준에서 전환을 추적하는 경우) [관리자 계정에 대한 자격 증명 추가](/help/search-social-commerce/admin/manager-accounts.md) 위치: **[!UICONTROL Search]> [!UICONTROL Admin] >[!UICONTROL Manager Accounts]**.

>[!MORELIKETHIS]
>
>* [광고주의 전환 지표 관리 정보](/help/search-social-commerce/admin/conversion-metrics/conversion-metric-about.md)
>* [전환 지표 업로드 [!DNL Google Ads]](conversion-metrics-upload-to-google.md)
