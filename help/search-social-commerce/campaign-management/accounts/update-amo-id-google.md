---
title: ' [!DNL Google Ads] 계정에 대한 AMO ID(s_kwcid) 추적 코드 업데이트'
description: ' [!DNL Google Ads]  계정에 대한 최신 AMO ID 추적 코드로 전환하는 방법에 대해 알아봅니다.'
exl-id: 4dfd9ea6-f639-4b9a-aaa5-13f574e3961b
feature: Search Campaign Management
source-git-commit: edb46265c6977a1e2c1b352f41fedcfc3a9e3bbf
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# [!DNL Google Ads] 계정에 대한 AMO ID(s_kwcid) 추적 코드 업데이트

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

*[!DNL Google Ads]개의 계정만*

기존 [!DNL Google Ads] 계정의 [AMO ID 추적 코드](/help/integrations/analytics/ids.md#amo-id-formats)에 대한 레거시(2019년 10월 이전) 형식은 [!DNL Google Ads] 성과 최대 캠페인, 초안 및 실험 캠페인에 대한 캠페인 및 광고 그룹 수준에서의 보고와 같은 Analytics의 일부 기능을 지원하지 않으며, 여러 캠페인에 동일한 ad+키워드+일치 유형 조합이 있는 기타 사용 사례도 지원합니다.

현재 형식에는 캠페인 ID 및 광고 그룹 ID에 대한 매개 변수가 포함되어 있습니다.

```
s_kwcid=AL!{userid}!3!{creative}!{matchtype}!{placement}!{network}!{product_partition_id}!{keyword}!{campaignid}!{adgroupid}
```

기존 형식을 사용하는 기존 계정의 경우 현재 형식으로 변경할 수 있습니다. 성과 최대 캠페인 또는 초안 및 실험 캠페인이 없는 경우 새로운 포맷으로의 마이그레이션은 선택 사항입니다.

모든 새 [!DNL Google Ads] 계정은 현재 AMO ID 형식을 자동으로 사용합니다.

>[!NOTE]
>
>이 옵션은 현재 형식을 사용하지 않는 계정에만 사용할 수 있습니다.
>
>계정을 마이그레이션한 후 모든 클릭, 비용 및 노출 데이터가 변경 후 올바르게 보고되지만 마이그레이션 전에 발생한 모든 클릭스루는 여전히 이전 AMO ID 형식을 기반으로 한 전환 데이터에 기여합니다.

1. 주 메뉴에서 **[!UICONTROL Search]** \> **[!UICONTROL Campaigns]** \> **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다. 하위 메뉴에서 **[!UICONTROL Live]** \> **[!UICONTROL Accounts]**&#x200B;을(를) 클릭합니다.

1. 계정 이름 위에 커서를 놓고 ![화살표 드롭다운 아이콘](/help/search-social-commerce/assets/arrow-dropdown-menu.png)을 클릭한 다음 **[!UICONTROL Edit]**&#x200B;을(를) 선택합니다.

1. **[!UICONTROL Set Account Tracking]**&#x200B;을(를) 클릭합니다.

1. 마이그레이션을 시작합니다.

   1. [!UICONTROL Account Tracking] 설정에서 **[!UICONTROL S_KWCID FORMAT]** 옆에 있는 **[!UICONTROL LEGACY S_KWCID FORMAT]**&#x200B;을(를) 클릭합니다.

   1. **[!UICONTROL Migrate to new s_kwcid format]**&#x200B;을(를) 클릭합니다.

   1. 확인 메시지에서 확인란을 선택한 다음 **[!UICONTROL Continue]**&#x200B;을(를) 클릭합니다.

   1. 계정 설정에서 **[!UICONTROL Post]**&#x200B;을(를) 클릭합니다.

   캠페인에 대한 메타데이터가 며칠 내에 [!DNL Analytics]에서 업데이트됩니다. 추적은 중단되지 않고 계속되므로 데이터가 손실되지 않지만 [!DNL Analytics]에서 모든 메타데이터를 받을 때까지 보고에 새 추적 코드가 반영되지 않을 수 있습니다.

   >[!NOTE]
   >
   >마이그레이션 전에 발생한 모든 클릭스루는 여전히 이전 형식을 기반으로 전환 데이터를 보고합니다.

1. 마이그레이션을 시작한 후 필요에 따라 랜딩 페이지 접미사 설정(일부 광고 네트워크에서는 &quot;최종 URL 접미사&quot;라고 함)을 업데이트합니다.

   * 추적 설정에서 [!UICONTROL Auto Upload] 기능을 사용하도록 설정하면 검색, 소셜 및 Commerce은 이 계정과 해당 캠페인에 대한 랜딩 페이지 접미사의 추적 코드를 자동으로 업데이트합니다. 아무것도 안 해도 돼

   * [!UICONTROL Auto Upload] 기능을 사용할 수 없고 [서버측 AMO ID 기능](/help/integrations/analytics/ids.md#amo-id-formats)을 사용하지 않는 경우 랜딩 페이지 접미사 설정에서 AMO ID 매개 변수를 수동으로 업데이트해야 합니다. [계정 설정](/help/search-social-commerce/campaign-management/accounts/ad-network-account-manage.md) 및 [캠페인 설정](/help/search-social-commerce/campaign-management/campaigns/campaign-settings-google.md)에서 또는 [일괄 시트에서 변경 내용을 업로드](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-upload.md)하여 계정 및 캠페인 수준 접미사를 수동으로 변경할 수 있습니다. 광고 그룹 수준 이하에서 접미사를 구성하려면 [!DNL Google Ads] 편집기를 사용하십시오.

   * 캠페인 구성 요소에 대한 기본 URL 설정에 AMO ID를 포함하는 경우 해당 랜딩 페이지 접미사 설정으로 이동합니다.

1. (권장) 추가 계정을 마이그레이션하기 전에 [!DNL Analytics]에서 이 계정에 대한 데이터를 확인하십시오.

>[!MORELIKETHIS]
>
>* [광고 네트워크 계정 관리](ad-network-account-manage.md)
>*  [!DNL Analytics]](/help/integrations/analytics/ids.md)에서 사용하는 [Adobe Advertising ID
>* [개요 [!DNL Analytics for Advertising]](https://experienceleague.adobe.com/docs/advertising/integrations/home.html){target="_blank"}
