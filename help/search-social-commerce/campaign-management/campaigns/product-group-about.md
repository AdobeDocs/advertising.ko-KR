---
title: 쇼핑 제품 그룹 기본 정보
description: 쇼핑 캠페인의 쇼핑 제품 그룹에 대해 알아봅니다.
exl-id: ae270935-1464-4393-8b8c-745fee077522
feature: Search Campaign Management
source-git-commit: d0f1c413134a0868ddec79ded7672af316267edd
workflow-type: tm+mt
source-wordcount: '721'
ht-degree: 0%

---

# 쇼핑 제품 그룹 기본 정보

*[!DNL Google Ads]및 [!DNL Microsoft Advertising] 쇼핑 캠페인만*

쇼핑 캠페인에서 키워드가 아닌 제품 그룹은 쇼핑 광고가 표시되는 머천트 센터 계정의 제품을 결정합니다. 각 제품 그룹은 단일 제품 속성(예: 카테고리, 제품 유형, 브랜드, 조건, 제품 ID 또는 사용자 정의 레이블)을 기반으로 하며 일치하는 모든 제품에 대해 동일한 입찰을 사용합니다. 각 그룹의 제품에 대한 입찰을 포함하거나 제외할 수 있습니다.

광고 그룹 수준에서 제품 그룹을 구성하여 머천트 센터 계정의 제품 중 광고 그룹의 쇼핑 광고에 나타나는 제품을 결정합니다. 광고 그룹에 광고 엔티티가 포함되지 않은 경우에도 광고 네트워크에는 여전히 제품에 대한 광고가 표시됩니다.

동일한 제품이 둘 이상의 캠페인에 포함된 경우 광고 네트워크는 먼저 캠페인 우선 순위를 사용하여 광고 경매에 적합한 캠페인(및 관련 입찰)을 결정합니다. 모든 캠페인이 동일한 우선 순위를 갖는 경우 입찰이 가장 높은 캠페인이 적격입니다.

[!DNL Google] 쇼핑 캠페인 및 광고에 대한 자세한 내용은 &quot;[&#128279;](/help/search-social-commerce/campaign-management/special-workflows/google-shopping-campaigns.md)쇼핑 캠페인 구현 [!DNL Google Ads] 3&rbrace;&quot; 및 [Google 광고 설명서](https://support.google.com/google-ads/answer/3455481?visit_id=638205553638977410-2592024034&rd=1)를 참조하십시오.  [!DNL Microsoft] 쇼핑 캠페인에 대한 자세한 내용은 &quot;[&#128279;](/help/search-social-commerce/campaign-management/special-workflows/microsoft-shopping-campaigns.md)쇼핑 캠페인 구현 [!DNL Microsoft Advertising] 3&rbrace;&quot; 및 [[!DNL Microsoft Advertising] 설명서](https://help.bingads.microsoft.com/#apex/3/en/50903/1-500)를 참조하세요.

>[!NOTE]
>
>스마트 쇼핑 캠페인을 대체하는 성과 최대 캠페인에 그룹을 나열하는 [!DNL Google Ads]에 대해서는 지원을 사용할 수 없습니다. 목록 그룹에 대한 데이터를 관리하고 보려면 [!DNL Google Ads] 편집기를 사용하십시오.

## 제품 그룹 계층

광고 그룹에 대한 특정 특성을 사용하여 제품 그룹을 만들려면 먼저 &quot;[!UICONTROL All Products]&quot;이라는 포괄적 제품 그룹을 만들어야 합니다. 이 상위 제품 그룹에서 제품 하위 집합에 대한 하위 제품 그룹을 생성할 수 있으며 하위 제품 그룹에서 손자를 생성할 수 있습니다. 광고 그룹에 대해 첫 번째 하위 제품 그룹을 만들면 기본 광고 그룹 입찰을 사용하여 &quot;[!UICONTROL Everything Else]&quot;이라는 다른 제품 그룹이 자동으로 만들어집니다. 제품 그룹을 더 추가하면 &quot;[!UICONTROL Everything Else]&quot; 그룹이 다른 제품 그룹에 없는 모든 제품을 구성하도록 적절하게 조정됩니다.

광고 그룹 내에서 입찰에서 포함하거나 제외할 제품 그룹을 최대 7개까지 만들 수 있습니다(&quot;[!UICONTROL All Products]&quot; 제외). 하나 이상의 제품 그룹은 각 수준에서 동일한 특성을 타깃팅합니다(예: 한 제품 그룹의 경우 [!UICONTROL Brand]=Acme, 같은 수준의 다른 제품 그룹의 경우 [!UICONTROL Brand]=AcmePlus). 상위 제품군을 세부분류라고 하며, 세부분류의 가장 낮은 수준을 단위라고 한다. 단위 수준에서 입찰 및 추적 템플릿을 설정하거나 입찰을 완전히 제외할 수 있습니다. 광고 그룹에 대한 전체 활성 제품 그룹 세트가 계층적으로 적용되어 적격 제품을 결정합니다. 예를 들어 [!UICONTROL All Products]을(를) [!UICONTROL Brand]=AcmeBasic 및 [!UICONTROL Brand]=AcmePlus로 세분한 다음 각 제품 그룹을 [!UICONTROL Condition]=New로 세분하고 입찰을 설정하면 AcmeBasic 및 AcmePlus 브랜드가 있는 새 제품만 광고하거나 광고에서 제외할 수 있습니다.

![제품 그룹 집합의 예](/help/search-social-commerce/assets/product-group-list.png "제품 그룹 집합의 예")

![제품 그룹 계층 구조 예](/help/search-social-commerce/assets/product-group-tree.png "제품 그룹 계층 구조 예")

## [!UICONTROL Product Groups] 보기

[!UICONTROL Search, Social, & Commerce] > [!UICONTROL Campaigns] > [!UICONTROL Campaigns] > [!UICONTROL Product Groups] 보기에서 제품 그룹을 만들고 편집하고, 제품 그룹과 해당 하위 제품 그룹을 삭제할 수 있습니다.

## 쇼핑 제품 그룹에 대한 추적 및 성능 데이터

(추적 옵션이 &quot;[!UICONTROL EF Redirect]&quot;인 계정/캠페인) Search, Social 및 Commerce에서 제품 그룹의 전환을 추적할 수 있도록 하려면 [추적 URL 도구를 사용하여 제품 그룹의 추적 URL을 생성](/help/search-social-commerce/tools/click-tracking-url-generate.md)한 다음, 다음 중 하나를 수행하십시오.

* ([!DNL Google Ads]에 필요; [!DNL Microsoft Advertising]에 대한 모범 사례) 계정, 캠페인 또는 제품 그룹 설정의 [!DNL Tracking Template] 필드에 추적 URL을 추가합니다. 간편하게 유지 관리할 수 있도록 가능한 한 높은 수준에서 추가하십시오. 계정이나 캠페인에 대해 지정된 추가 매개 변수는 포함되지 않습니다.

  >[!CAUTION]
  >
  >([!DNL Microsoft Advertising]) 제품 피드 내의 사용자 지정 열에 Search, Social 및 Commerce 추적 URL을 포함하지 않는 경우에만 이 옵션을 사용합니다. 두 작업을 모두 수행하는 경우 URL에 두 개의 리디렉션이 포함되어 링크가 끊어집니다.

* ([!DNL Microsoft Advertising]만 해당) [!DNL Microsoft Merchant Center] 계정 내의 제품 데이터에 추적 URL을 추가합니다. 이렇게 하려면 제품 피드 내의 [`bingads_redirect`](https://help.ads.microsoft.com/#apex/3/en/51084/0)이라는 사용자 지정 열에 `link` 또는 `mobile_link` 필드의 값과 함께 추적 URL을 적절하게 포함하십시오. 이 방법을 사용하여 생성된 URL에는 검색, 소셜 및 Commerce 내의 계정 또는 캠페인 설정에 지정된 추적 매개 변수가 포함되지 않습니다.

[의 [!UICONTROL Product Group Report]](/help/search-social-commerce/reports/management/basic-advanced/product-group-report.md)에서 제품 그룹에 대한 데이터를 볼 수 있습니다.

>[!MORELIKETHIS]
>
>* [쇼핑 제품 그룹 관리](product-group-manage.md)
>* [[!DNL Google Ads] 제품 그룹 설정](product-group-settings-google.md)
>* [쇼핑 캠페인 구현 [!DNL Google Ads] 2&rbrace;](/help/search-social-commerce/campaign-management/special-workflows/google-shopping-campaigns.md)
>* [[!DNL Microsoft Advertising] 제품 그룹 설정](product-group-settings-microsoft.md)
>* [쇼핑 캠페인 구현 [!DNL Microsoft Advertising] 2&rbrace;](/help/search-social-commerce/campaign-management/special-workflows/microsoft-shopping-campaigns.md)
