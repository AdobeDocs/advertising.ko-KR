---
title: '[!DNL Microsoft Ads] 인벤토리 피드에 대한 쇼핑 광고 템플릿 설정'
description: 인벤토리 피드에 대한  [!DNL Microsoft Ads] 쇼핑 광고 템플릿 설정을 참조하십시오.
exl-id: a0dd6542-0516-406a-b8c5-2e102ec7ab3d
feature: Search Inventory Feeds
source-git-commit: 67fe8581832dc0762d62908d01672e53cc95b847
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 0%

---

# 인벤토리 피드에 대한 [!DNL Microsoft Ads] 쇼핑 광고 템플릿 설정

쇼핑 광고 템플릿을 사용하여 쇼핑 광고를 구성합니다.

>[!NOTE]
>
>* 다음 문자는 템플릿에서 열 이름 및 수정자 이름을 지정하기 위해 예약되어 있으므로 모든 특성 필드에 텍스트로 사용할 수 없습니다. `[ ] < > `


## \[모든 탭 위로\]

<!-- **Template Name:** -->

{{$include /help/_includes/inventory-feed-template-name.md}}

<!-- **Status:** -->

{{$include /help/_includes/inventory-feed-template-status.md}}

<!-- **Account:** -->

{{$include /help/_includes/inventory-feed-template-account.md}}

## \[왼쪽 패널\]

<!-- **[!UICONTROL Feed &amp; Columns]:** -->

{{$include /help/_includes/inventory-feed-template-feed-and-columns.md}}

<!-- **[!UICONTROL Modifiers]:** -->

{{$include /help/_includes/inventory-feed-template-modifiers.md}}

## [!UICONTROL Campaigns]

<!-- **[!UICONTROL Campaign]:** -->

{{$include /help/_includes/inventory-feed-template-campaign.md}}

<!-- **[!UICONTROL Campaign Map Only]:** -->

{{$include /help/_includes/inventory-feed-template-shopping-campaign-map-only.md}}

<!-- **[!UICONTROL Campaign Map Method]:** -->

{{$include /help/_includes/inventory-feed-template-shopping-campaign-map-method.md}}

**[!UICONTROL Campaign Tracking Template]:**(클라이언트 피드 파일 템플릿에 대한 선택 사항) 모든 랜딩 도메인 리디렉션 및 추적 매개 변수를 지정하고 매개 변수에 최종 URL을 임베드하는 캠페인 수준 추적 템플릿입니다. 이 값은 계정 수준 설정을 무시하지만, 더 세분화된 수준에서(키워드를 가장 세분화된 수준으로) 추적 템플릿이 이 값을 무시합니다.

* 캠페인 설정에 &quot;[!UICONTROL EF Redirect]&quot; 및 &quot;[!UICONTROL Auto Upload]&quot;이(가) 포함된 경우 적용되는 Adobe Advertising 전환 추적의 경우 다음 중 하나를 수행합니다.&quot;

   * (권장) [Microsoft 쇼핑 캠페인에 대한 추적 템플릿 형식](/help/search-social-commerce/tracking/formats-click-tracking-microsoft.md)을 사용하십시오. 전체 계정이 쇼핑 광고 전용인 경우 대신 계정 수준에서 추적 템플릿을 정의할 수 있습니다.

   * 대신 &quot;[!DNL bingads_redirect]&quot; 열([올바른 형식](/help/search-social-commerce/tracking/formats-click-tracking-microsoft.md) 사용)을 사용하여 피드에 각 제품의 값을 포함하는 경우 매개 변수 `{lpurl}`을(를) 입력하십시오. 필요에 따라 `{lpurl}` 매개 변수에 타사 리디렉션 및 추적을 추가할 수 있습니다.

* 서드파티 리디렉션 및 추적의 경우 값을 입력합니다.

<!-- **[!UICONTROL Campaign Final URL Suffix]:** -->

{{$include /help/_includes/final-url-suffix.md}}

**[!UICONTROL Merchant ID]:** 캠페인에 사용되는 제품을 가진 판매자 계정의 고객 ID입니다.

**[!UICONTROL Sales Country]:** 캠페인 제품을 판매하는 국가입니다. 제품이 연결되어 있기 때문입니다.
target 국가의 경우 이 설정은 캠페인에 광고되는 제품을 결정합니다.

<!-- **[!UICONTROL Stock Level]:** -->

{{$include /help/_includes/inventory-feed-template-campaign-stock-level.md}}

<!-- **[!UICONTROL This column has non-numeric values]:** -->

{{$include /help/_includes/inventory-feed-template-nonnumeric-values.md}}

### [!UICONTROL Campaign Level Negative Keywords]

{{$include /help/_includes/inventory-feed-template-campaign-negative-keywords.md}}

### [!UICONTROL Manage Settings for NEW Campaigns]

<!-- Flag/check box **[!UICONTROL Manage Settings for NEW Campaigns]:** -->

{{$include /help/_includes/inventory-feed-template-campaign-manage-settings-new-campaigns.md}}

<!-- **[!UICONTROL Initial Budget]:** -->

{{$include /help/_includes/inventory-feed-template-campaign-initial-budget.md}}

**[!UICONTROL Campaign Priority]:** 여러 캠페인이 광고를 할 때 캠페인이 사용되는 우선 순위입니다.
동일한 제품: *[!UICONTROL Low]*(새 캠페인의 기본값), *[!UICONTROL Medium]* 또는 *[!UICONTROL High]*. 동일한 제품이 두 개 이상의 캠페인에 포함된 경우 광고 네트워크는 을 사용합니다
광고 경매에 적합한 캠페인(및 관련 입찰)을 결정하는 캠페인 우선 순위. 모든 캠페인이 동일한 우선 순위를 갖는 경우 입찰이 가장 높은 캠페인이 적격입니다.

<!-- **[!UICONTROL Locations]:** -->

{{$include /help/_includes/inventory-feed-template-campaign-locations.md}}

## [!UICONTROL Ad Groups]

<!-- **[!UICONTROL Ad Group]:** -->

{{$include /help/_includes/inventory-feed-template-ad-group.md}}

<!-- **[!UICONTROL Map Only]:** -->

{{$include /help/_includes/inventory-feed-template-ad-group-map-only.md}}

<!-- **[!UICONTROL Map Method]:** -->

{{$include /help/_includes/inventory-feed-template-ad-group-map-method.md }}

**[!UICONTROL Ad Group Tracking Template]:**(선택 사항) 모든 랜딩 외부 도메인 리디렉션 및 추적 매개 변수를 지정하고 매개 변수에 최종 URL을 임베드하는 광고 그룹 수준의 추적 템플릿입니다. 이 값은 계정 및 캠페인 수준 설정을 무시하지만 더 세분화된 수준에서 추적 템플릿이 이 값을 무시합니다.

Adobe Advertising 전환 추적의 경우 값을 입력할 필요가 없습니다. 캠페인 수준 값이면 충분합니다.

서드파티 리디렉션 및 추적의 경우 값을 입력합니다.

### [!UICONTROL Ad Group Level Negative Keywords]

{{$include /help/_includes/inventory-feed-template-ad-group-negative-keywords.md}}

### [!UICONTROL Manage Settings for NEW Ad Groups]

<!-- Flag/check box **[!UICONTROL Manage Settings for NEW Ad Groups]:** -->

{{$include /help/_includes/inventory-feed-template-ad-group-manage-settings-new-ad-groups.md}}

<!-- **[!UICONTROL Languages]:** -->

{{$include /help/_includes/inventory-feed-template-ad-group-language-microsoft.md}}

## [!UICONTROL Product Groups]

**[!UICONTROL Tier 1]:** 기본, 모든 포함 제품 그룹 &quot;[!UICONTROL All products]&quot;입니다. 이 상위 제품 그룹은 삭제할 수 없지만, 피드에 하위 계층이 모두 누락된 경우 자동으로 삭제됩니다.

<!-- **[!UICONTROL Tier 2 - Tier 8]:** -->

{{$include /help/_includes/inventory-feed-template-tier2-8.md}}

<!-- **[!UICONTROL Row Level Value]:** -->

{{$include /help/_includes/inventory-feed-template-row-level-value.md}}

**[!UICONTROL Tracking Template]:**(하위 제품 그룹이 없는 단위, 선택 사항) 제품에 대한 추적 템플릿
모든 오프랜딩 도메인 리디렉션 및 추적 매개 변수를 지정하고 [!DNL ValueTrack] 매개 변수에 최종 URL을 임베드하는 그룹입니다. 이 템플릿은 상위 수준의 템플릿을 무시합니다.

Adobe Advertising 전환 추적의 경우 값을 입력할 필요가 없습니다. 캠페인 수준 값이면 충분합니다.

서드파티 리디렉션 및 추적의 경우 값을 입력합니다.

**[!UICONTROL Initial Bid]:** 각 광고의 초기 입찰가입니다.

## [!UICONTROL Feed Filters]

<!-- **\[Feed Filter\]:** -->

{{$include /help/_includes/inventory-feed-template-feed-filter.md}}

## [!UICONTROL Label Classifications]

<!-- **\[Component\] [!UICONTROL Label Classifications] &gt; `[Label Classification and Value`]:** -->

{{$include /help/_includes/inventory-feed-template-label-classifications.md}}

>[!MORELIKETHIS]
>
>* [인벤토리 피드를 사용하여 광고 관리 자동화 정보](../inventory-feeds-about.md)
>* [수정자 관리](../modifiers-manage.md)
>* [인벤토리 데이터 피드 파일 관리](/help/search-social-commerce/campaign-management/inventory-feeds/feed-files-manage.md)
>* [템플릿을 통해 피드 데이터 전파](../feed-data-propagate.md)
>* [인벤토리 피드에서 광고 네트워크로 캠페인 데이터 게시](../propagated-data-post.md)
