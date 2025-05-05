---
title: ' [!DNL Microsoft Advertising] 쇼핑 캠페인 구현'
description: ' [!DNL Microsoft Advertising] 쇼핑 캠페인을 설정하는 워크플로에 대해 알아봅니다.'
exl-id: fd10237b-864d-4808-8644-3fcb18edebde
feature: Search Campaign Management
source-git-commit: 283fced2b3faa64b6383b6ab2a41696cba0da06f
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# [!DNL Microsoft Advertising] 쇼핑 캠페인 구현

쇼핑 캠페인의 광고는 키워드 대신 기존 [!DNL Microsoft Merchant Center] 제품 피드의 제품에 대한 데이터를 사용하여 광고를 표시할 방법과 위치를 결정합니다.

[!DNL Microsoft]개의 쇼핑 캠페인이 [!DNL Microsoft Advertising Shopping Network]을(를) 대상으로 합니다. 쇼핑 캠페인에 대한 설정에는 제품을 판매하는 지정된 국가와 우선 순위([!DNL High], [!DNL Medium] 또는 [!DNL Low])가 포함됩니다. 선택적으로 인벤토리를 필터링하여 특정 속성이 있는 제품을 광고하고 특정 위치 및 장치 유형을 타기팅하거나 제외할 수 있습니다.

광고 그룹 수준에서 다중 수준 *[제품 그룹](/help/search-social-commerce/campaign-management/campaigns/product-group-about.md)*&#x200B;을 설정하여 쇼핑 광고와 함께 표시되는 제품을 제어할 수 있습니다. 제품 그룹은 모든 제품 특성(범주, 제품 유형, 브랜드, 조건, 제품 ID 및 사용자 지정 레이블)을 기반으로 하며 &quot;[!DNL Add Products]&quot;을(를) 포함하지 않고 입찰에서 포함하거나 제외할 제품 그룹의 수준을 최대 7개까지 만들 수 있습니다. 일치하는 모든 제품에 대해 동일한 입찰을 사용하여 제품 그룹의 최하위 수준에서 입찰을 설정할 수 있습니다. 동일한 제품이 두 개 이상의 캠페인에 포함된 경우 [!DNL Microsoft Advertising]은(는) 캠페인 수준 우선 순위를 먼저 사용하여 광고 경매에 적합한 캠페인(및 관련 입찰)을 결정합니다. 모든 캠페인이 동일한 우선 순위를 갖는 경우 입찰이 가장 높은 캠페인이 적격입니다.

## [!DNL Microsoft Advertising] 쇼핑 캠페인을 설정하는 단계

[!DNL Microsoft Advertising]에 대해 [인벤토리 피드 템플릿](/help/search-social-commerce/campaign-management/inventory-feeds/inventory-feeds-about.md), [일괄 시트](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-about.md)를 사용하거나 개별적으로 쇼핑 캠페인을 설정할 수 있습니다. 다음 지침에는 개별 엔티티 만들기에 대한 링크가 포함되어 있습니다.

1. [!DNL Microsoft Merchant Center] 계정을 설정하고 제품 데이터로 채웁니다.

1. [검색, 소셜 및 Commerce에서  [!DNL Microsoft Merchant Center] 계정](/help/search-social-commerce/campaign-management/accounts/merchant-account-manage.md)에서 데이터를 다운로드하도록 허용합니다.

1. 쇼핑 네트워크에서 [캠페인을 만듭니다](/help/search-social-commerce/campaign-management/campaigns/campaign-manage.md).

1. [캠페인 내에 광고 그룹을 만들고](/help/search-social-commerce/campaign-management/campaigns/ad-group-manage.md) 모든 광고에 대한 기본 입찰을 설정합니다.

   개별 제품 그룹에 대한 기본 입찰을 재정의할 수 있습니다.

1. 광고 그룹에 대한 제품 그룹 만들기:

   1. [모든 제품 그룹 만들기](/help/search-social-commerce/campaign-management/campaigns/product-group-manage.md).

   1. (선택 사항) [하위 제품 그룹을 만듭니다](/help/search-social-commerce/campaign-management/campaigns/product-group-manage.md).

   1. 광고 그룹 내의 각 쇼핑 광고에 포함될 수 있는 [&#128279;](/help/search-social-commerce/campaign-management/campaigns/product-group-settings-microsoft.md)프로모션 줄이 있는 [제품 광고](/help/search-social-commerce/campaign-management/campaigns/ad-manage.md)를 만듭니다.

      Microsoft Advertising은 각 광고에 대한 광고 사본과 랜딩 페이지 URL을 동적으로 생성합니다.

      >[!NOTE]
      >
      >광고 그룹에 광고 엔터티가 포함되어 있지 않더라도 [!DNL Microsoft Advertising]에서 제품에 대한 광고를 표시합니다.

1. (선택 사항) 광고 클릭을 추적하려면 [추적 URL 도구를 사용하여 추적 URL을 생성합니다](/help/search-social-commerce/tools/click-tracking-url-generate.md). 가장 좋은 방법은 계정, 캠페인 또는 제품 그룹 설정의 [!UICONTROL Tracking Template] 필드에 추적 URL을 추가하는 것입니다. 간편하게 유지 관리할 수 있도록 최대한 높은 수준으로 추가하십시오.

   또는 [!DNL Microsoft Merchant Center] 계정 내에서 제품 데이터에 추적 URL을 추가할 수 있습니다. 이렇게 하려면 제품 피드 내의 사용자 지정 열 &quot;[bingads_redirect](https://help.ads.microsoft.com/#apex/3/en/51084)&quot;에 추적 URL과 &quot;link&quot; 또는 &quot;mobile_link&quot; 필드의 값을 적절하게 포함하십시오. &quot;bingads_redirect&quot; 필드의 값은 &quot;link&quot; 및 &quot;mobile_link&quot; 필드의 값을 대체합니다. 이 방법을 사용하여 생성된 URL에는 검색, 소셜 및 Commerce 계정 또는 캠페인 설정에 지정된 추적 매개 변수가 포함되지 않습니다.

1. [[!UICONTROL Product Group Report]](/help/search-social-commerce/reports/management/basic-advanced/basic-advanced-report-generate.md)을(를) 생성하여 성능을 모니터링합니다.

1. 필요한 경우:

   1. 캠페인 예산을 조정하려면 [캠페인 설정을 편집](/help/search-social-commerce/campaign-management/campaigns/campaign-manage.md)하세요.

      캠페인이 포트폴리오의 일부인 경우 포트폴리오 설정 &quot;[!UICONTROL Auto adjust campaign budget limits]&quot;을(를) 사용하면 검색, 소셜 및 Commerce에서 포트폴리오의 모든 캠페인에 대한 예산을 최적화할 수 있습니다.

   1. 기존 제품 그룹의 최대 입찰가를 조정하고, 더 이상 광고를 만들지 않으려는 제품 그룹을 삭제하거나, 새 &quot;모든 제품&quot; 제품 그룹 또는 새 하위 제품 그룹을 추가하여 추가 제품에 대한 광고를 만듭니다.

>[!NOTE]
>
>* [일괄 시트](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-microsoft.md) 및 [인벤토리 피드 템플릿](/help/search-social-commerce/campaign-management/inventory-feeds/ad-templates/template-microsoft-shopping.md)을 사용하여 [!DNL Microsoft Shopping] 캠페인 및 제품 그룹을 관리하는 데 필요한 필드를 참조하세요.
>* [!DNL Microsoft Shopping] 캠페인에 대한 자세한 내용은 [[!DNL Microsoft Advertising] 설명서](https://help.ads.microsoft.com/#apex/3/en/50903)를 참조하세요.
