---
title: 광고 네트워크에 목표 업로드 활성화
description: 하이브리드 포트폴리오에 대한 목표를 업로드하는 방법을 알아봅니다. [!DNL Google Ads] 및 [!DNL Microsoft® Advertising].
exl-id: 75a1a804-ad6a-4dbc-9cde-30fe54476162
feature: Search Tools
source-git-commit: 052574217d7ddafb8895c74094da5997b5ff83db
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# 광고 네트워크에 목표 업로드 활성화

*를 사용하는 광고주 [!DNL Google Ads] 및 [!DNL Microsoft® Advertising] 계정만*

*하이브리드 최적화에만 활성화된 광고주*

광고주 계정이 하이브리드 최적화를 사용하도록 구성되어 있는 경우 Adobe Advertising은 필요에 따라 계정의 포트폴리오에 대한 목표를 업로드할 수 있습니다. [!DNL Google Ads] 및 [!DNL Microsoft® Advertising] 하이브리드 최적화에 사용할 수 있는 전환으로.

이 옵션을 활성화하면 스마트 입찰 전략이 포함된 캠페인이 포함된 포트폴리오에 대한 업로드가 자동으로 트리거됩니다. Search, Social 및 Commerce는 해당되는 각 포트폴리오와 객관적인 조합에 대해 광고 네트워크에서 전환을 만듭니다. 각 전환에는 이름이 있습니다. `ACS_OBJ_SID_<portfolio_id>_<se_acctid/conversion_manager_se_acctid>`, 여기서 `<portfolio_id>` 는 숫자 포트폴리오 ID이고 `<se_acctid/conversion_manager_se_acctid>` 광고 네트워크 계정 또는 관리자 계정의 숫자 ID입니다. 변환은 목표의 모든 가중치가 적용된 거래 속성을 나타냅니다.

에 업로드 [!DNL Google Ads] 광고주의 시간대에서 매일 06:00에 발생합니다. 에 업로드 [!DNL Microsoft® Advertising] 광고주의 시간대에서 매일 09:00에 발생합니다.

<!-- Note to self: Conversions tracked by Google Ads and by the Microsoft Advertising universal event tracking (UET) tag aren't re-uploaded to the ad networks. -->

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Tools] >[!UICONTROL Conversion Upload Setup]**.

1. 옆에 있는 확인란을 선택합니다. **[!UICONTROL Enable Objective Upload]**.

   이 옵션은 광고주 계정이 하이브리드 최적화를 사용하도록 구성된 경우에만 사용할 수 있습니다. 하이브리드 최적화를 활성화하려면 Adobe 계정 팀에 문의하십시오.

1. 클릭 **[!UICONTROL Save]**.

1. (관리자 계정 수준에서 전환을 추적하는 경우) [관리자 계정에 대한 자격 증명 추가](/help/search-social-commerce/admin/manager-accounts.md) 위치: **[!UICONTROL Search]> [!UICONTROL Admin] >[!UICONTROL Manager Accounts]**.

>[!MORELIKETHIS]
>
>* [광고주의 거래 속성 관리 정보](/help/search-social-commerce/admin/transaction-properties/transaction-property-about.md)
>* [전환 지표 업로드 [!DNL Google Ads]](conversion-metrics-upload-to-google.md)
