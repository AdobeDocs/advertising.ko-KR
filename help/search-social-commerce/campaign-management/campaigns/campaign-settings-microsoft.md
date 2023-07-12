---
title: '[!DNL Microsoft Advertising] 캠페인 설정'
description: 다음에 대한 설정 참조 [!DNL Microsoft Advertising] 캠페인.
exl-id: c6d86fb8-48b0-40fd-bcfc-c4afdccd5283
source-git-commit: f2889bbafc1b3cd3c467d94abae2ad1a52d0eaed
workflow-type: tm+mt
source-wordcount: '992'
ht-degree: 0%

---

# [!DNL Microsoft Advertising] 캠페인 설정

## \[캠페인 만들기 화면\]

**[!UICONTROL Campaign Type]:** (캠페인 생성 중에만 사용 가능) 광고를 배치할 위치와 캠페인에 포함될 수 있는 광고 유형:

* *[!UICONTROL Search and Display Network]:* 검색 네트워크에서만 텍스트 광고를 표시합니다.

* *[!UICONTROL Shopping Network]:* 의 제품에 대한 제품 광고를 표시합니다. [!DNL Microsoft Merchant Center] 제품 카탈로그 — 쇼핑 네트워크

* *[!UICONTROL Audience]:* 에 기본/디스플레이 광고를 표시합니다. [!DNL Microsoft Audience Network]. a) 캠페인을 의 판매자 센터 상점에 연결하여 피드 기반 광고를 자동으로 생성할 수 있습니다. [!UICONTROL Shopping Settings] 섹션 또는 b) 텍스트 에셋 및 업로드된 이미지가 있는 반응형 광고를 만듭니다. 두 옵션 모두 사용자 타깃팅으로 광고 그룹을 만들어야 합니다.

## [!UICONTROL Campaign Details]

**[!UICONTROL Campaign Name]:** 계정 내에서 고유한 캠페인 이름. 최대 길이는 128자입니다.

**[!UICONTROL Status]:** 캠페인의 표시 상태: *활성* 또는 *일시 중지됨*. 새 광고 캠페인의 기본값은 입니다 *활성*.

<!-- **[!UICONTROL Start Date]:** -->

{{$include /help/_includes/start-date.md}}

<!-- **[!UICONTROL End Date]:** -->

{{$include /help/_includes/end-date.md}}

## [!UICONTROL Budget Options]

<!-- **[!UICONTROL Budget]:** -->

{{$include /help/_includes/budget.md}}

<!-- **[!UICONTROL Delivery Method]:** -->

{{$include /help/_includes/delivery-method.md}}

**[!UICONTROL Bid strategy]:** 캠페인에 대한 입찰 전략:

* *[!UICONTROL Enhanced CPC]:* (대상, 검색 및 쇼핑 네트워크의 캠페인) 평균 CPC를 최대 CPC 미만으로 유지하려고 시도하는 동안 광고 네트워크에서 전환을 극대화하기 위해 광고 네트워크(검색, 소셜 및 상거래가 아님) 내에 지정된 전환을 사용하여 각 경매에 대한 CPC(클릭당 비용) 입찰을 자동으로 변경할 수 있는 광고 네트워크의 eCPC(향상된 클릭당 비용) 모델을 사용합니다.

최적화된 검색, 소셜 및 상거래 포트폴리오에 eCPC가 있는 캠페인을 추가하면 검색, 소셜 및 상거래는 기본 입찰가를 최적화하고,[!UICONTROL Auto adjust campaign budget limits]&quot;옵션이 활성화됨 — 캠페인 예산. 광고 네트워크는 모든 입찰 조정을 최적화하고 독점 데이터 및 통찰력을 기반으로 사용자 쿼리 시 검색, 소셜 및 상거래에서 생성한 입찰을 변경할 수 있습니다. **주의:** 광고 네트워크에서 추적된 총 전환이 포트폴리오 목표에 맞는 경우에만 포트폴리오에서 eCPC 캠페인을 사용하십시오.

* *[!UICONTROL Manual CPC]* (기본값): (더 이상 사용되지 않음 [!DNL Microsoft Advertising] 2021년) CPC(Cost-per-Click) 모델을 사용합니다. 광고 네트워크에서 캠페인에 대한 입찰을 변경하도록 허용할 수 있습니다(선택적).

   * **[!UICONTROL Enable Enhanced CPC]** (기본적으로 비활성화됨): &quot;[!UICONTROL Enhanced CPC]&quot; 옵션입니다.

* *[!UICONTROL Manual CPM]* (대상 네트워크의 캠페인만 해당) 1,000개의 조회 횟수당 소비할 항목을 지정하는 CPM(비용-천 단위 노출 횟수) 모델을 사용합니다. 이 입찰 전략을 사용하는 캠페인은 포트폴리오에 포함될 때 최적화되지 않습니다.

* *[!UICONTROL Maximize Clicks]:* (검색 및 쇼핑 캠페인) 검색, 소셜 및 상거래가 아닌 광고 네트워크는 클릭수를 최대화하기 위해 입찰을 최적화합니다. 다음을 입력합니다(선택적). **[!UICONTROL Max CPC]** (클릭당 비용) 광고 네트워크가 클릭당 특정 금액 이상을 지불하지 않도록 하기 위한 것입니다. **주의:** 이 전략을 사용하는 캠페인을 포트폴리오에 추가하면 입찰은 포트폴리오 목표가 아니라 클릭 가중치에 의해 결정됩니다.

* *[!UICONTROL Maximize Conversion Value]:* (검색 및 쇼핑/스마트 쇼핑 네트워크) 검색, 소셜 및 상거래가 아닌 광고 네트워크는 전환 가치를 극대화하기 위해 입찰을 최적화합니다. 필요한 경우 다음을 입력합니다. **[!UICONTROL Target Return on Ad Spend]** (ROAS) 를 백분율로 표시합니다. **참고:** 표준 포트폴리오가 아닌 하이브리드 포트폴리오의 캠페인에 이 옵션을 사용합니다.

* *[!UICONTROL Maximize Conversions]:* (검색 네트워크의 캠페인 <!-- future: and audience network -->) 광고 네트워크(검색, 소셜 및 상거래가 아님)는 전환을 최대화하기 위해 입찰을 최적화합니다. 필요한 경우 다음을 입력합니다. **[!UICONTROL Target CPC]** (클릭당 비용)<!-- future: ; for audience campaigns, you can also enter an optional [!UICONTROL Target CPA] (cost per acquisition) -->. **참고:** 표준 포트폴리오가 아닌 하이브리드 포트폴리오의 캠페인에 이 옵션을 사용합니다.

* *[!UICONTROL Target CPA]:* (검색 네트워크의 캠페인) 검색, 소셜 및 상거래가 아닌 광고 네트워크는 선택 사항을 기반으로 입찰을 최적화합니다 **[!UICONTROL Target CPA]** (취득당 비용) - 취득(전환)에 대해 지불할 30일 평균 금액입니다. **참고:** 지출 전략을 사용하는 하이브리드 포트폴리오(표준 포트폴리오는 아님)의 캠페인에 이 옵션을 사용합니다. [!UICONTROL Weekly] 또는 [!UICONTROL Google Target CPA].

  이 입찰 전략이 있는 캠페인에는 평균 위치 및 CPC 입찰 데이터를 사용할 수 없습니다.

* *[!UICONTROL Target Impression Share]:* (검색 네트워크의 캠페인) 검색, 소셜 및 상거래가 아닌 광고 네트워크는 타겟 노출 점유율 및 광고 위치를 달성하기 위해 입찰을 최적화합니다. 다음을 입력합니다(선택적). **[!UICONTROL Target Impression Share]** 백분율로, **[!UICONTROL Target Ad Position]**, 및 **[!UICONTROL Max CPC]** (클릭당 비용) **참고:** 이 옵션은 하이브리드 포트폴리오에서 지원되지 않습니다.

* *[!UICONTROL Target Return on Ad Spend]:*  (검색 및 쇼핑 네트워크의 캠페인) 검색, 소셜 및 상거래가 아닌 광고 네트워크는 다음을 기반으로 입찰을 최적화합니다. **[!UICONTROL Target ROAS]** (광고 투자 수익률), 백분율로 지정됩니다. 다음을 입력합니다(선택적). **[!UICONTROL Max CPC]** (클릭당 비용) 광고 네트워크가 클릭당 특정 금액 이상을 지불하지 않도록 하기 위한 것입니다. **참고:** 지출 전략을 사용하는 하이브리드 포트폴리오(표준 포트폴리오는 아님)의 캠페인에 이 옵션을 사용합니다. [!UICONTROL Weekly] 또는 [!UICONTROL Google Target ROAS].

  이 입찰 전략이 있는 캠페인에는 평균 위치 및 CPC 입찰 데이터를 사용할 수 없습니다.

## [!UICONTROL Shopping Settings]

**[!UICONTROL Sales Country]:** (쇼핑 캠페인 전용, 기존 캠페인의 경우 읽기 전용) 캠페인의 제품이 판매되는 국가입니다. 제품은 대상 국가와 연결되어 있으므로 이 설정은 캠페인에 광고되는 제품을 결정합니다.

<!-- **[!UICONTROL Campaign Priority]:** -->

**[!UICONTROL Link with Microsoft Merchant Center]:** (대상 캠페인만 해당, 선택 사항) 반응형 광고가 아닌 자동화된 피드 기반 광고를 위해 특정 머천트 센터 상점과 캠페인을 연결합니다. 이 옵션을 선택할 때 [!UICONTROL Merchant ID] 및 [!UICONTROL Products]. 캠페인에 대한 광고 그룹을 만들어야 하지만 광고를 만들 필요는 없습니다.

캠페인을 저장소에 연결하고 설정을 저장하면 이 옵션을 변경할 수 없습니다.

{{$include /help/_includes/campaign-priority.md}}

<!-- **[!UICONTROL Merchant ID]:** -->

{{$include /help/_includes/merchant-id.md}}


**[!UICONTROL Products]:** (상인 센터 상점에만 연결된 대상자 캠페인) 광고할 제품. 기본적으로, *[!UICONTROL All products]* 이(가) 선택되어 있습니다. 특정 속성이 있는 제품만 광고하려면 다음을 선택합니다. *[!UICONTROL Filter products]* 제품을 필터링할 제품 차원 및 속성 조합을 최대 7개까지 지정할 수 있습니다. 제품에 대한 광고가 표시되도록 지정된 모든 값을 적용할 수 있어야 합니다. 예를 들어 Acme 애완 동물 용품 광고를 표시하려면 필터를 만들 수 있습니다 `Custom Label 1=animals`, `Category=pet supplies`, 및 `Brand=Acme Pet Supplies`.

<!-- **[!UICONTROL Inventory Filter]:** -->

{{$include /help/_includes/inventory-filter.md}}

## [!UICONTROL Campaign Targeting]

<!-- **[!UICONTROL Location Targets]:** -->

{{$include /help/_includes/location-targets.md}}

<!-- **[!UICONTROL Devices]:** -->

{{$include /help/_includes/devices.md}}

## [!UICONTROL URL Options]

<!-- **[!UICONTROL Tracking Template]:** -->

{{$include /help/_includes/tracking-template-microsoft.md}}

<!-- **[!UICONTROL Custom Parameters]:** -->

{{$include /help/_includes/custom-parameters.md}}

<!-- **[!UICONTROL Landing Page Suffix]:** -->

{{$include /help/_includes/landing-page-suffix.md}}

## [!UICONTROL DSA Options]

<!-- **[!UICONTROL Website Domain]:** -->

{{$include /help/_includes/website-domain.md}}

<!-- **[!UICONTROL DSA Language]:** -->

{{$include /help/_includes/dsa-language.md}}

## [!UICONTROL Negative Keywords]

<!-- **[!UICONTROL Negative Keywords]:** -->

{{$include /help/_includes/negative-keyword.md}}

<!-- Note for **[!UICONTROL Negative Keywords]:** -->

{{$include /help/_includes/negative-keyword-note-microsoft.md}}

## [!UICONTROL Negative Websites]

**[!UICONTROL Negative Websites]:** (디스플레이/기본 네트워크의 캠페인만 해당, 선택 사항) 광고를 표시하지 않으려는 디스플레이 네트워크의 사이트. 올바른 URL(예: www.example.com)을 입력하십시오. 여러 문자열을 지정하려면 쉼표로 구분하거나 별도의 줄에 입력합니다.

가용성에 대한 자세한 내용은 &quot; Microsoft Advertising 도움말을 참조하십시오.[특정 웹 사이트에 광고가 표시되지 않도록 하기](https://help.ads.microsoft.com/#apex/bae/en/14061/0).&quot;

## [!UICONTROL Campaign Tracking]

<!-- **[!UICONTROL Override Account Tracking]:** -->

{{$include /help/_includes/override-account-tracking.md}}

<!-- **[!UICONTROL Tracking Type]:** -->

{{$include /help/_includes/tracking-type.md}}

<!-- **[!UICONTROL Redirect Type]:** -->

{{$include /help/_includes/redirect-type.md}}

<!-- **[!UICONTROL Auto Upload]:** -->

{{$include /help/_includes/auto-upload.md}}

<!-- **[!UICONTROL Encode Base URL]:** -->

{{$include /help/_includes/encode-base-url.md}}

<!-- **[!UICONTROL Tracking Level]:** -->

{{$include /help/_includes/tracking-level.md}}

**[!UICONTROL Track Product Group]:** (대상 [!UICONTROL EF Redirect] 만) 구현되지 않음

<!-- **[!UICONTROL Append Parameters]:** -->

{{$include /help/_includes/append-parameters.md}}

## [!UICONTROL Conversion Goals]

**[!UICONTROL Conversion Goal]:** 종료 여부 *[!UICONTROL Use account conversion goals for this campaign]* (기본값) 또는 *[!UICONTROL Use campaign specific conversion goals]*. 캠페인에 대한 전환 목표를 지정하도록 선택한 경우 사용 가능한 모든 목표 목록에서 목표를 선택합니다. **참고:** 목표는 매일 동기화되므로 이전 24시간 동안 생성된 목표는 나열되지 않을 수 있습니다. 목록을 업데이트하려면 [수동으로 광고 네트워크 데이터 동기화](/help/search-social-commerce/campaign-management/campaigns/sync-network.md).

캠페인이 포트폴리오의 일부인 경우 포트폴리오의 목표와 동일한 전환 목표를 사용합니다. 다양한 전환 목표를 사용하면 포트폴리오 성능에 영향을 줄 수 있습니다.

>[!MORELIKETHIS]
>
>* [캠페인 관리](/help/search-social-commerce/campaign-management/campaigns/campaign-manage.md)
