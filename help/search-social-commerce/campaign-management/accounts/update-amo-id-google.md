---
title: 에 대한 AMO ID(s\_kwcid) 추적 코드 업데이트 [!DNL Google Ads] account
description: 에 대한 최신 AMO ID 추적 코드로 전환하는 방법에 대해 알아봅니다. [!DNL Google Ads] 계정입니다.
exl-id: 82168ee6-43bb-4b8d-882d-5254a1abcb09
feature: Search Campaign Management
source-git-commit: f80d05aa40fd4114e9585220fe747ca7d36a19bb
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# 에 대한 s_kwcid 추적 코드 업데이트 [!DNL Google Ads] account

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

*[!DNL Google Ads]계정만*

기존 s\_kwcid 추적 코드에 대한 레거시 형식 [!DNL Google Ads] 은 Analytics에서 캠페인 및 광고 그룹 수준에서의 보고와 같은 일부 기능을 지원하지 않습니다. [!DNL Google Ads] 여러 캠페인에 동일한 광고+키워드+일치 유형 조합이 있는 성과 최대 캠페인, 초안 및 실험 캠페인 및 기타 사용 사례입니다.

최신 형식에는 캠페인 ID 및 광고 그룹 ID에 대한 매개 변수가 포함되어 있습니다.

```
s_kwcid=AL!{userid}!3!{creative}!{matchtype}!{placement}!{network}!{product_partition_id}!{keyword}!{campaignid}!{adgroupid}
```

기존 계정 중 일부 또는 전체에 대해 새 형식으로 개별적으로 변경할 수 있습니다. 성과 최대 캠페인 또는 초안 및 실험 캠페인이 없는 경우 새로운 포맷으로의 마이그레이션은 선택 사항입니다.

모든 신규 [!DNL Google Ads] 계정은 자동으로 새 s\_kwcid 형식을 사용합니다.

>[!NOTE]
>
>계정을 마이그레이션한 후 모든 클릭, 비용 및 노출 데이터가 변경 후 올바르게 보고되지만 마이그레이션 전에 발생한 클릭스루는 여전히 이전 s\_kwcid 형식을 기반으로 한 전환 데이터에 기여합니다.

1. 메인 메뉴에서 **[!UICONTROL Search]** \> **[!UICONTROL Campaigns]** \> **[!UICONTROL Campaigns]**. 하위 메뉴에서 **[!UICONTROL Live]** \> **[!UICONTROL Accounts]**.
1. 계정 이름 위에 커서를 놓고 ![화살표 드롭다운 아이콘](/help/search-social-commerce/assets/arrow-dropdown-menu.png)을 선택한 다음 을 선택합니다 **[!UICONTROL Edit]**.
1. 클릭 **[!UICONTROL Set Account Tracking]**.
1. 마이그레이션을 시작합니다.

   1. 다음 **[!UICONTROL S_KWCID FORMAT]** , 클릭 **[!UICONTROL LEGACY S_KWCID FORMAT]**.
   1. 클릭 **[!UICONTROL Migrate to new s_kwcid format]**.
   1. 확인 메시지에서 확인란을 선택한 다음 을 클릭합니다. **[!UICONTROL Continue]**.
   1. 계정 설정에서 **[!UICONTROL Post]**.

   캠페인에 대한 메타데이터는 며칠 내에 Analytics에서 업데이트됩니다. 추적은 중단되지 않고 계속되므로 데이터가 손실되지 않지만, Analytics가 모든 메타데이터를 수신할 때까지 보고에 새 추적 코드가 반영되지 않을 수 있습니다.

   >[!NOTE]
   >
   >마이그레이션 전에 발생한 모든 클릭스루는 여전히 이전 형식을 기반으로 전환 데이터를 보고합니다.

1. 마이그레이션을 시작한 후 필요에 따라 랜딩 페이지 접미사 설정(일부 광고 네트워크에서는 &quot;최종 URL 접미사&quot;라고 함)을 업데이트합니다.

   * 다음의 경우 [!UICONTROL Auto Upload]&quot;추적 설정에서 기능을 활성화하면 검색, 소셜 및 상거래는 이 계정 및 해당 캠페인에 대한 랜딩 페이지 접미사의 추적 코드를 자동으로 업데이트합니다. 아무것도 안 해도 돼
   * 다음의 경우 [!UICONTROL Auto Upload]&quot;기능이 활성화되지 않았으며 서버측 s-kwcid를 사용하지 않는 경우 랜딩 페이지 접미어 설정에서 s\_kwcid 매개 변수를 수동으로 업데이트해야 합니다. 계정 및 캠페인 설정에서 수동으로 또는 일괄 시트에서 변경 사항을 업로드하여 계정 및 캠페인 수준 접미사를 변경할 수 있습니다. 광고 그룹 수준 또는 하위 수준에서 접미사를 구성하려면 [!DNL Google Ads] 편집자.
   * 캠페인 구성 요소에 대한 기본 URL 설정에 s\_kwcid를 포함하는 경우 해당 랜딩 페이지 접미사 설정으로 이동합니다.

1. (권장) 추가 계정을 마이그레이션하기 전에 Analytics에서 이 계정에 대한 데이터를 확인하십시오.

>[!MORELIKETHIS]
>
>* [광고 네트워크 계정 관리](ad-network-account-manage.md)
>* [AMO ID 추적 매개 변수](/help/search-social-commerce/tracking/skwcid-tracking-parameter.md)
>* [개요 [!DNL Analytics for Advertising]](https://experienceleague.adobe.com/docs/advertising/integrations/home.html){target="_blank"}
