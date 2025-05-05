---
title: '[!DNL Google Ads] 제품 그룹 설정'
description: ' [!DNL Google Ads] 쇼핑 제품 그룹의 설정을 참조합니다.'
exl-id: 2cfef9de-b265-4fa5-b1bd-84e6cba79914
feature: Search Campaign Management
source-git-commit: 7e4d2aa502f26b480a5fd76d68411586c24f68b2
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# [!DNL Google Ads] 제품 그룹 설정

## &quot;모든 제품&quot; 제품 그룹

**[!UICONTROL Condition]:**(읽기 전용) 모든 제품

**[!UICONTROL Bid]:**(포함된 제품 그룹만 해당) 광고 클릭에 대해 지불할 가장 높은 금액인 클릭당 최대 비용(CPC)입니다. 이 값은 하위 제품 그룹이 없는 단위에 대해서만 사용되며 광고 그룹 수준 값 대신 사용됩니다.

<!-- **[!UICONTROL Tracking Template]:** -->

{{$include /help/_includes/tracking-template-google.md}}

이 템플릿은 상위 수준의 템플릿을 재정의하며 하위 제품 그룹이 없는 단위에 대해서만 사용됩니다.

## 기타 모든 제품 그룹

**[!UICONTROL Condition/Value]:**(기존 제품 그룹의 경우 읽기 전용) 대상 제품 차원입니다. 새 제품 그룹의 경우 제품을 타겟팅할 차원 및 선택한 정보 카테고리의 자격 속성(예: 브랜드별로 타겟팅하는 경우 &quot;Acme&quot; 또는 조건별로 타겟팅하는 경우 &quot;New&quot;)을 입력합니다.

특정 제품 차원(&quot;모든 제품&quot;이 아닌)에 대한 제품 그룹을 만들면 검색, 소셜 및 Commerce에서 자동으로 &quot;기타 모두&quot;에 대한 제품 그룹을 만듭니다.

사용 가능한 제품 차원 목록을 보려면 &quot;[쇼핑 캠페인 제품 필터](/help/search-social-commerce/campaign-management/campaigns/shopping-campaign-product-filters.md)&quot;을 참조하세요. 캠페인의 [!UICONTROL Inventory Filter] 설정에 따라 차원 목록이 제한될 수 있습니다.

**[!UICONTROL Excluded]:**(새 제품 그룹의 경우 선택 사항, 기존 제품 그룹의 경우 읽기 전용) 일치하는 제품의 광고에 대한 입찰을 제외합니다.

**[!UICONTROL Bid]:**(포함된 제품 그룹만 해당) 광고 클릭에 대해 지불할 가장 높은 금액인 클릭당 최대 비용(CPC)입니다. 이 값은 하위 제품 그룹이 없는 단위에 대해서만 사용되며 광고 그룹 수준 값 대신 사용됩니다.

<!-- **[!UICONTROL Tracking Template]:** -->

<!-- ExL can't handle the same include twice in the same file, so using a snippet for the second occurrence.

{{$include /help/_includes/tracking-template-google.md}}
-->

{{tracking-template-google}}

이 템플릿은 상위 수준의 템플릿을 재정의하며 하위 제품 그룹이 없는 단위에 대해서만 사용됩니다.

>[!MORELIKETHIS]
>
>* [쇼핑 제품 그룹 정보](product-group-about.md)
>* [쇼핑 제품 그룹 관리](product-group-manage.md)
>* [쇼핑 캠페인 제품 필터](/help/search-social-commerce/campaign-management/campaigns/shopping-campaign-product-filters.md)
>* [쇼핑 캠페인 구현 [!DNL Google Ads] 2&rbrace;](/help/search-social-commerce/campaign-management/special-workflows/google-shopping-campaigns.md)
