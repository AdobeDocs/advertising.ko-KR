---
title: 구현 [!DNL Microsoft Advertising] 쇼핑 캠페인
description: 설정 워크플로에 대해 알아보기 [!DNL Microsoft Advertising] 쇼핑 캠페인.
exl-id: fd10237b-864d-4808-8644-3fcb18edebde
feature: Search Campaign Management
source-git-commit: d5d4dee4356d941ea9cae74b9385add00e0480c3
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# 구현 [!DNL Microsoft Advertising] 쇼핑 캠페인

쇼핑 캠페인의 광고는 기존 제품의 데이터를 사용합니다 [!DNL Microsoft Merchant Center] 키워드 대신 제품 피드를 사용하여 광고를 표시할 방법과 위치를 결정할 수 있습니다.

[!DNL Microsoft] 쇼핑 캠페인은 다음을 타겟팅합니다 [!DNL Microsoft Advertising Shopping Network]. 쇼핑 캠페인에 대한 설정에는 제품이 판매되는 지정된 국가와 우선 순위([!DNL High], [!DNL Medium], 또는 [!DNL Low]). 선택적으로 인벤토리를 필터링하여 특정 속성이 있는 제품을 광고하고 특정 위치 및 장치 유형을 타기팅하거나 제외할 수 있습니다.

다중 수준을 설정하여 쇼핑 광고와 함께 표시되는 제품을 제어할 수 있습니다 *[제품 그룹](/help/search-social-commerce/campaign-management/campaigns/product-group-about.md)* 광고 그룹 수준에서. 제품 그룹은 모든 제품 속성(카테고리, 제품 유형, 브랜드, 조건, 제품 ID 및 사용자 정의 레이블)을 기반으로 하며, &quot;을 제외하고 입찰에서 포함 또는 제외할 최대 7개의 제품 그룹 수준을 만들 수 있습니다.[!DNL Add Products].&quot; 일치하는 모든 제품에 대해 동일한 입찰을 사용하여 제품 그룹의 최하위 수준에서 입찰을 설정할 수 있습니다. 동일한 제품이 두 개 이상의 캠페인에 포함된 경우 [!DNL Microsoft Advertising] 캠페인 수준 우선 순위를 먼저 사용하여 광고 경매에 적합한 캠페인(및 관련 입찰)을 결정합니다. 모든 캠페인이 동일한 우선 순위를 갖는 경우 입찰이 가장 높은 캠페인이 적격입니다.

## 설정 단계 [!DNL Microsoft Advertising] 쇼핑 캠페인

다음을 사용하여 쇼핑 캠페인을 설정할 수 있습니다 [인벤토리 피드 템플릿](/help/search-social-commerce/campaign-management/inventory-feeds/inventory-feeds-about.md) 대상 [!DNL Microsoft Advertising], 사용 [일괄 시트](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-about.md)또는 개별적으로 사용할 수 있습니다. 다음 지침에는 개별 엔티티 만들기에 대한 링크가 포함되어 있습니다.

1. 설정 [!DNL Microsoft Merchant Center] 계정을 만들고 제품 데이터로 채웁니다.

1. [검색, 소셜 및 Commerce에서 [!DNL Microsoft Merchant Center] account](/help/search-social-commerce/campaign-management/accounts/merchant-account-manage.md).

1. [캠페인 만들기](/help/search-social-commerce/campaign-management/campaigns/campaign-manage.md) 쇼핑 네트워크에서.

1. [광고 그룹 만들기](/help/search-social-commerce/campaign-management/campaigns/ad-group-manage.md) 캠페인 내에서 모든 광고에 대한 기본 입찰을 설정합니다.

   개별 제품 그룹에 대한 기본 입찰을 재정의할 수 있습니다.

1. 광고 그룹에 대한 제품 그룹 만들기:

   1. [&quot;모든 제품&quot; 제품 그룹 만들기](/help/search-social-commerce/campaign-management/campaigns/product-group-manage.md).

   1. (선택 사항) [하위 제품 그룹 만들기](/help/search-social-commerce/campaign-management/campaigns/product-group-manage.md).

   1. 만들기 [제품 광고](/help/search-social-commerce/campaign-management/campaigns/ad-manage.md) 포함 [각 쇼핑 광고에 잠재적으로 포함할 프로모션 라인](/help/search-social-commerce/campaign-management/campaigns/product-group-settings-microsoft.md) 광고 그룹 내.

      Microsoft Advertising은 각 광고에 대한 광고 사본과 랜딩 페이지 URL을 동적으로 생성합니다.

      >[!NOTE]
      >
      >광고 그룹에 광고 엔티티가 포함되지 않은 경우에도 [!DNL Microsoft Advertising] 는 여전히 제품에 대한 광고를 표시합니다.

1. (선택 사항) 광고 클릭을 추적하려면, [추적 URL 도구를 사용하여 추적 URL 생성](/help/search-social-commerce/tools/click-tracking-url-generate.md). 가장 좋은 방법은 추적 URL을 [!UICONTROL Tracking Template] 계정, 캠페인 또는 제품 그룹 설정의 필드입니다. 간편하게 유지 관리할 수 있도록 최대한 높은 수준으로 추가하십시오.

   또는 내에서 제품 데이터에 추적 URL을 추가할 수 있습니다. [!DNL Microsoft Merchant Center] 계정입니다. 이렇게 하려면 추적 URL을 &quot;link&quot; 또는 &quot;mobile_link&quot; 필드의 값과 함께 필요에 따라 사용자 정의 열 &quot;에 포함합니다.[bingads_redirect](https://help.ads.microsoft.com/#apex/3/en/51084)&quot;를 입력합니다. &quot;bingads_redirect&quot; 필드의 값은 &quot;link&quot; 및 &quot;mobile_link&quot; 필드의 값을 대체합니다. 이 방법을 사용하여 생성된 URL에는 검색, 소셜 및 Commerce 계정 또는 캠페인 설정에 지정된 추적 매개 변수가 포함되지 않습니다.

1. 성능 모니터링 기준 [생성 [!UICONTROL Product Group Report]](/help/search-social-commerce/reports/management/basic-advanced/basic-advanced-report-generate.md).

1. 필요한 경우:

   1. [캠페인 설정 편집](/help/search-social-commerce/campaign-management/campaigns/campaign-manage.md) 캠페인 예산을 조정합니다.

      캠페인이 포트폴리오의 일부인 경우 포트폴리오 설정 &quot;[!UICONTROL Auto adjust campaign budget limits]&quot;검색, 소셜 및 Commerce을 통해 포트폴리오의 모든 캠페인에 대한 예산을 최적화할 수 있습니다.

   1. 기존 제품 그룹의 최대 입찰가를 조정하고, 더 이상 광고를 만들지 않으려는 제품 그룹을 삭제하거나, 새 &quot;모든 제품&quot; 제품 그룹 또는 새 하위 제품 그룹을 추가하여 추가 제품에 대한 광고를 만듭니다.

>[!NOTE]
>
>* 관리에 필요한 필드 보기 [!DNL Microsoft Shopping] 을 사용하는 캠페인 및 제품 그룹 [일괄 시트](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-microsoft.md) 및 [인벤토리 피드 템플릿](/help/search-social-commerce/campaign-management/inventory-feeds/ad-templates/template-microsoft-shopping.md).
>* 에 대한 자세한 내용 [!DNL Microsoft Shopping] 캠페인, 참조: [[!DNL Microsoft Advertising] 설명서](https://help.ads.microsoft.com/#apex/3/en/50903).
