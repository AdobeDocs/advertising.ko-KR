---
title: '[!DNL Microsoft® Advertising] 캠페인 설정'
description: 다음에 대한 설정 참조 [!DNL Microsoft® Advertising] 캠페인.
exl-id: f11cb61e-d627-4074-870d-e186f3e65572
feature: Search Campaign Management
source-git-commit: 8d1ff29322799ff7905ee808703e00f5190ae8af
workflow-type: tm+mt
source-wordcount: '1912'
ht-degree: 0%

---

# [!DNL Microsoft® Advertising] 캠페인 설정

## \[캠페인 만들기 화면\]

**[!UICONTROL Campaign Type]:** (캠페인 생성 중에만 사용 가능) 광고를 배치할 위치와 캠페인에 포함될 수 있는 광고 유형:

* *[!UICONTROL Search]:* 검색 네트워크에 텍스트 광고를 표시합니다.

* *[!UICONTROL Shopping Network]:* 의 제품에 대한 제품 광고를 표시합니다. [!DNL Microsoft® Merchant Center] 제품 카탈로그 — 쇼핑 네트워크.

* *[!UICONTROL Audience]:* 에 기본/디스플레이 광고를 표시합니다. [!DNL Microsoft® Audience Network]. a) 캠페인을 의 판매자 센터 상점에 연결하여 피드 기반 광고를 자동으로 생성할 수 있습니다. [!UICONTROL Shopping Settings] 섹션 또는 b) 텍스트 에셋 및 업로드된 이미지가 있는 반응형 광고를 만듭니다. 두 옵션 모두 사용자 타깃팅으로 광고 그룹을 만들어야 합니다.

* *[!UICONTROL Shopping Campaigns for Brands]:* (Beta 기능) 검색 및 대상 네트워크에서 연결된 소매점을 통해 제품을 홍보합니다. 하위 광고 그룹과 제품 그룹(홍보용 앱), 캠페인에 대한 선택적 제품 광고를 만들 수 있습니다. [!DNL Microsoft® Advertising] 는 제품 그룹에 대한 광고를 자동으로 만듭니다. 브랜드를 위한 쇼핑 캠페인의 경우 입찰 전략을 사용하십시오 [!UICONTROL Manual CPC]; 브랜드에 대한 쇼핑 프로모션의 경우 입찰 전략을 사용하십시오 [!UICONTROL Cost per Sale].

* *[!UICONTROL Microsoft® Store Ads Campaign]:* (Beta 기능)에서 사용할 수 있는 앱 및 게임을 홍보합니다. [!DNL Microsoft® Store]. 캠페인에 대한 하위 광고 그룹, 제품 그룹 및 선택적 제품 광고를 만들 수 있습니다. [!DNL Microsoft® Advertising] 는 제품 그룹에 대한 광고를 자동으로 만듭니다.

* *[!UICONTROL Audience CTV Video]:* (Beta 기능) Audience Network에서 연결된 TV(CTV) 비디오 광고를 표시합니다.

* *[!UICONTROL Audience Video]:* (Beta 기능) 대상 네트워크의 표준 비디오 광고를 표시합니다.

* *[!UICONTROL Performance Max]:* (Beta 기능) 를 사용하여 모든 네트워크에서 여러 광고 유형을 표시합니다. [!DNL Microsoft® Advertising] 현명한 입찰. 캠페인 설정 내에서 이미지, 로고, 헤드라인, 설명, 선택적 콜 투 액션 및 대상 신호를 포함하는 자산 그룹을 하나 이상 지정해야 합니다. 광고 네트워크는 채널을 기반으로 광고를 제공할 자산을 자동으로 결합합니다.

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

* *[!UICONTROL Cost per Sale]:* (쇼핑 캠페인 전용) 검색, 소셜 및 Commerce이 아닌 광고 네트워크는 다음을 기반으로 입찰을 최적화합니다. [!UICONTROL Target CPS] (판매당 비용). 제품을 클릭할 때만 지불하고 24시간 이내에 판매합니다. **참고:** 이 입찰 전략이 포함된 캠페인을 포트폴리오에 포함하지 마십시오. 이 입찰 전략을 사용하는 캠페인에는 검색, 소셜 및 Commerce 최적화를 사용할 수 없습니다.

  이 입찰 전략으로 브랜드에 대한 쇼핑 캠페인을 저장하면 입찰 전략을 변경할 수 없습니다. 다른 쇼핑 캠페인 유형의 경우 이 전략은 새 캠페인에만 사용할 수 있습니다.

* *[!UICONTROL CPV]* (Audience CTV 비디오 캠페인만 해당) CPV(Cost-per-View) 모델을 사용합니다. <!-- Campaigns with this bid strategy aren't optimized when they're included in portfolios. -->

* *[!UICONTROL Enhanced CPC]:* (대상, 검색 및 쇼핑 네트워크의 캠페인) 평균 CPC를 최대 CPC 미만으로 유지하려고 시도하는 동안 광고 네트워크(검색, 소셜 및 Commerce이 아님) 내에서 지정된 전환을 사용하여 전환을 극대화하기 위해 광고 네트워크가 각 경매의 클릭당 비용(CPC) 입찰을 자동으로 변경할 수 있는 광고 네트워크의 eCPC(향상된 클릭당 비용) 모델을 사용합니다.

  최적화된 검색, 소셜 및 Commerce 포트폴리오에 eCPC가 있는 캠페인을 추가하면 검색, 소셜 및 Commerce은 기본 입찰가를 최적화하고, 다음과 같은 경우에[!UICONTROL Auto adjust campaign budget limits]&quot;옵션이 활성화됨 — 캠페인 예산. 광고 네트워크는 모든 입찰 조정을 최적화하고 독점 데이터 및 통찰력을 기반으로 사용자 쿼리 시 검색, 소셜 및 Commerce 생성 입찰을 변경할 수 있습니다. **주의:** 광고 네트워크에서 추적된 총 전환이 포트폴리오 목표에 맞는 경우에만 포트폴리오에서 eCPC 캠페인을 사용하십시오.

* *[!UICONTROL Manual CPC]*: (브랜드를 위한 쇼핑 캠페인) [!DNL Microsoft® Store Ads] 캠페인; 사용 중단됨 [!DNL Microsoft® Advertising] (다른 캠페인 유형의 경우 2021년) 클릭당 비용(CPC) 모델을 사용합니다. 일부 광고 유형의 경우 선택적으로 광고 네트워크가 캠페인에 대한 입찰을 변경하도록 허용할 수 있습니다.

   * **[!UICONTROL Enable Enhanced CPC]** (기본적으로 비활성화됨): 이 옵션은 &quot;[!UICONTROL Enhanced CPC]&quot; 옵션입니다.

* *[!UICONTROL Manual CPA]:* ([!DNL Microsoft® Store Ads] 캠페인) CPA(취득당 비용) 모델을 사용합니다.

* *[!UICONTROL Manual CPM]* (대상 캠페인 및 대상 비디오 캠페인만 해당) 1,000회의 보기 노출 횟수당 소비할 항목을 지정하는 CPM(비용-천 단위 노출 횟수) 모델을 사용합니다. 이 입찰 전략을 사용하는 캠페인은 포트폴리오에 포함될 때 최적화되지 않습니다.

* *[!UICONTROL Maximize Clicks]:* (검색 및 쇼핑 캠페인) 검색, 소셜 및 Commerce이 아닌 광고 네트워크는 클릭수를 최대화하기 위해 입찰을 최적화합니다. 다음을 입력합니다(선택적). **[!UICONTROL Max CPC]** (클릭당 비용) 광고 네트워크가 클릭당 특정 금액 이상을 지불하지 않도록 하기 위한 것입니다. **주의:** 이 전략을 사용하는 캠페인을 포트폴리오에 추가하면 클릭 가중치(포트폴리오 목표가 아님)가 입찰을 유도합니다.

* *[!UICONTROL Maximize Conversion Value]:* (검색 및 쇼핑/스마트 쇼핑 네트워크, 성과 최대 캠페인) 검색, 소셜 및 Commerce이 아닌 광고 네트워크는 입찰을 최적화하여 전환 가치를 극대화합니다. 필요한 경우 다음을 입력합니다. **[!UICONTROL Target Return on Ad Spend]** (ROAS) 를 백분율로 표시합니다. **참고:** 표준 포트폴리오가 아닌 하이브리드 포트폴리오의 캠페인에 이 옵션을 사용합니다.

* *[!UICONTROL Maximize Conversions]:* (검색 네트워크 또는 대상 네트워크에서 성과 최대 캠페인 및 캠페인(대상 비디오 또는 연결된 TV는 아님) 검색, 소셜 및 Commerce이 아닌 광고 네트워크는 전환을 최대화하기 위해 입찰을 최적화합니다. 필요한 경우 다음을 입력합니다. **[!UICONTROL Target CPC]** (클릭당 비용) 대상자 캠페인의 경우 선택 사항을 입력할 수도 있습니다 **[!UICONTROL Target CPA]** (취득당 비용) **참고:** 표준 포트폴리오가 아닌 하이브리드 포트폴리오의 캠페인에 이 옵션을 사용합니다.

* *[!UICONTROL Target CPA]:* (검색 네트워크의 캠페인) 검색, 소셜 및 Commerce이 아닌 광고 네트워크는 선택 사항을 기반으로 입찰을 최적화합니다 **[!UICONTROL Target CPA]** (취득당 비용) - 취득(전환)에 대해 지불할 30일 평균 금액입니다. **참고:** 지출 전략을 사용하는 하이브리드 포트폴리오(표준 포트폴리오는 아님)의 캠페인에 이 옵션을 사용합니다. [!UICONTROL Weekly] 또는 [!UICONTROL Google Target CPA].

  이 입찰 전략이 있는 캠페인에는 평균 위치 및 CPC 입찰 데이터를 사용할 수 없습니다.

* *[!UICONTROL Target Impression Share]:* (검색 네트워크의 캠페인) 검색, 소셜 및 Commerce이 아닌 광고 네트워크는 입찰을 최적화하여 타겟 노출 점유율 및 광고 위치를 달성합니다. 다음을 입력합니다(선택적). **[!UICONTROL Target Impression Share]** 백분율로, **[!UICONTROL Target Ad Position]**, 및 **[!UICONTROL Max CPC]** (클릭당 비용) **참고:** 이 옵션은 하이브리드 포트폴리오에서 지원되지 않습니다.

* *[!UICONTROL Target Return on Ad Spend]:* (검색 및 쇼핑 네트워크의 캠페인) 검색, 소셜 및 Commerce이 아닌 광고 네트워크는 다음을 기반으로 입찰을 최적화합니다. **[!UICONTROL Target ROAS]** (광고 투자 수익률), 백분율로 지정됩니다. 다음을 입력합니다(선택적). **[!UICONTROL Max CPC]** (클릭당 비용) 광고 네트워크가 클릭당 특정 금액 이상을 지불하지 않도록 하기 위한 것입니다. **참고:** 지출 전략을 사용하는 하이브리드 포트폴리오(표준 포트폴리오는 아님)의 캠페인에 이 옵션을 사용합니다. [!UICONTROL Weekly] 또는 [!UICONTROL Google Target ROAS].

  이 입찰 전략이 있는 캠페인에는 평균 위치 및 CPC 입찰 데이터를 사용할 수 없습니다.

## [!UICONTROL Shopping Settings]

**[!UICONTROL Sales Country]:** (쇼핑 캠페인 전용, 기존 캠페인의 경우 읽기 전용) 캠페인의 제품이 판매되는 국가입니다. 제품은 대상 국가와 연결되어 있으므로 이 설정은 캠페인에 광고되는 제품을 결정합니다.

<!-- **[!UICONTROL Campaign Priority]:** -->

**[!UICONTROL Link with Microsoft® Merchant Center]:** (대상 캠페인만 해당, 선택 사항) 반응형 광고가 아닌 자동화된 피드 기반 광고를 위해 특정 머천트 센터 상점과 캠페인을 연결합니다. 이 옵션을 선택할 때 [!UICONTROL Merchant ID] 및 [!UICONTROL Products]. 캠페인에 대한 광고 그룹을 만들어야 하지만 광고를 만들 필요는 없습니다.

캠페인을 저장소에 연결하고 설정을 저장하면 이 옵션을 변경할 수 없습니다.

{{$include /help/_includes/campaign-priority.md}}

<!-- **[!UICONTROL Merchant ID]:** -->

{{$include /help/_includes/merchant-id.md}}

**[!UICONTROL Products]:** (상인 센터 상점에만 연결된 대상자 캠페인) 광고할 제품. 기본적으로, *[!UICONTROL All products]* 이(가) 선택되어 있습니다. 특정 속성이 있는 제품만 광고하려면 다음을 선택합니다. *[!UICONTROL Filter products]* 제품을 필터링할 제품 차원 및 속성 조합을 최대 7개까지 지정할 수 있습니다. 제품에 대한 광고가 표시되도록 지정된 모든 값을 적용할 수 있어야 합니다. 예를 들어 Acme 애완 동물 용품 광고를 표시하려면 필터를 만들 수 있습니다 `Custom Label 1=animals`, `Category=pet supplies`, 및 `Brand=Acme Pet Supplies`.

<!-- **[!UICONTROL Inventory Filter]:** -->

{{$include /help/_includes/inventory-filter.md}}

## [!UICONTROL Campaign Targeting]

**[!UICONTROL Languages]:** (성과 최대 캠페인만 해당) 광고가 게재될 수 있는 사이트의 언어와 일치해야 하는 광고 언어입니다. [!DNL Microsoft® Advertising] 는 사용자의 쿼리, 게시자의 국가 및 사용자의 언어 설정을 포함한 다양한 신호로부터 사용자의 언어를 결정합니다.

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

가용성에 대한 자세한 내용은 &quot;에 대한 Microsoft® Advertising 도움말을 참조하십시오.[특정 웹 사이트에 광고가 표시되지 않도록 하기](https://help.ads.microsoft.com/#apex/bae/en/14061/0).&quot;

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

## [!UICONTROL Asset Groups] (에셋 그룹당)

**[!UICONTROL Asset Group Name]:** 에셋 폴더(에셋 그룹)의 이름입니다.

**[!UICONTROL Asset Group Status]:** 자산 그룹의 상태: *[!UICONTROL Active]* 또는 *[!UICONTROL Paused]*.

**[!UICONTROL Final URL]:** 자산 그룹에서 만든 모든 광고의 최종 URL입니다.

**[!UICONTROL Images]:** 하나 이상의 정사각형 이미지와 가로 이미지를 포함하여 광고용 이미지 최대 20개. 다음을 참조하십시오. [[!DNL Microsoft® Advertising] 이미지 지침](https://help.ads.microsoft.com/#apex/ads/en/60204/0). 이미지를 업로드하거나 [!UICONTROL Asset Library] — 그러나 둘 다 동일한 작업에 포함되지는 않습니다.

* 이미지를 업로드하려면:

   1. 다음에서 [!UICONTROL Upload from Device] 탭을 클릭하고 **[!UICONTROL +]** 장치 또는 네트워크에서 이미지를 선택합니다.

   1. 각 이미지에 대해:

      1. 종횡비를 선택합니다.

      1. 필요에 따라 자르기 상자를 끌어서 놓고 이미지의 볼 수 있는 부분을 선택한 다음 필요할 경우 이미지의 볼 수 있는 부분의 크기를 조정합니다.

      1. (선택 사항) 추가 종횡비를 선택하고 선택한 각 종횡비에 필요한 경우 이미지의 위치를 변경하고 크기를 선택적으로 조정합니다.

         선택한 각 종횡비에 대해 하나의 에셋이 만들어집니다.

      1. 클릭 **[!UICONTROL Proceed]**.

   1. 이미지 지정이 끝나면 **[!UICONTROL Upload]**.

* 에서 이미지를 선택하려면 [!UICONTROL Asset Library], 클릭 **[!UICONTROL Asset Library]** 이미지를 선택합니다.

**[!UICONTROL Logos]:** 하나 이상의 로고. 최대 5개까지 추가할 수 있습니다. 다음을 참조하십시오. [[!DNL Microsoft® Advertising] 자산 지침](https://help.ads.microsoft.com/#apex/ads/en/60204/0). 이미지를 업로드하거나 [!UICONTROL Asset Library] — 그러나 둘 다 동일한 작업에 포함되지는 않습니다.

* 이미지를 업로드하려면:

   1. 다음에서 [!UICONTROL Upload from Device] 탭을 클릭하고 **[!UICONTROL +]** 장치 또는 네트워크에서 이미지를 선택합니다.

   1. 각 이미지에 대해:

      1. 종횡비를 선택합니다.

      1. 필요에 따라 자르기 상자를 끌어서 놓고 이미지의 볼 수 있는 부분을 선택한 다음 필요할 경우 이미지의 볼 수 있는 부분의 크기를 조정합니다.

      1. (선택 사항) 추가 종횡비를 선택하고 선택한 각 종횡비에 필요한 경우 이미지의 위치를 변경하고 크기를 선택적으로 조정합니다.

         선택한 각 종횡비에 대해 하나의 에셋이 만들어집니다.

      1. 클릭 **[!UICONTROL Proceed]**.

   1. 이미지 지정이 끝나면 **[!UICONTROL Upload]**.

* 에서 이미지를 선택하려면 [!UICONTROL Asset Library], 클릭 **[!UICONTROL Asset Library]** 이미지를 선택합니다.

**[!UICONTROL Headlines]:** 최소 3자, 최대 15자의 짧은 머리글로 각각 최대 30자까지 사용할 수 있습니다. 텍스트를 입력하거나 [!UICONTROL Asset Library] — 그러나 둘 다 동일한 작업에 포함되지는 않습니다.

* 텍스트를 입력하려면 다음을 수행합니다.

   1. 다음에서 [!UICONTROL Enter Text] 탭에서 텍스트를 입력합니다.

   1. (선택 사항) 다른 텍스트 문자열을 추가하려면 **[!UICONTROL + Add]** 문자열을 입력합니다.

* 에서 에셋을 선택하려면 [!UICONTROL Asset Library], 클릭 **[!UICONTROL Asset Library]** 에셋을 선택합니다.

**[!UICONTROL Long Headlines]:** 각각 최대 90자의 긴 머리글이 최소 1개에서 최대 5개까지 표시됩니다. 텍스트를 입력하거나 [!UICONTROL Asset Library] — 그러나 둘 다 동일한 작업에 포함되지는 않습니다.

* 텍스트를 입력하려면 다음을 수행합니다.

   1. 다음에서 [!UICONTROL Enter Text] 탭에서 텍스트를 입력합니다.

   1. (선택 사항) 다른 텍스트 문자열을 추가하려면 **[!UICONTROL + Add]** 문자열을 입력합니다.

* 에서 에셋을 선택하려면 [!UICONTROL Asset Library], 클릭 **[!UICONTROL Asset Library]** 에셋을 선택합니다.

**[!UICONTROL Descriptions]:** 최소 2자부터 최대 5자까지 최대 90자까지 입력할 수 있습니다. 텍스트를 입력하거나 [!UICONTROL Asset Library] — 그러나 둘 다 동일한 작업에 포함되지는 않습니다.

* 텍스트를 입력하려면 다음을 수행합니다.

   1. 다음에서 [!UICONTROL Enter Text] 탭에서 텍스트를 입력합니다.

   1. (선택 사항) 다른 텍스트 문자열을 추가하려면 **[!UICONTROL + Add]** 문자열을 입력합니다.

* 에서 에셋을 선택하려면 [!UICONTROL Asset Library], 클릭 **[!UICONTROL Asset Library]** 에셋을 선택합니다.

**[!UICONTROL Call to Action]:** 광고에 포함할 클릭 유도 문안. 기본적으로, *[!UICONTROL Act Now]* 이(가) 선택되어 있습니다.

**[!UICONTROL Business Name]:** 비즈니스 이름(최대 25자). 스크립트, HTML 또는 기타 마크업 언어를 포함할 수 없습니다.

**[!UICONTROL Audience Signal]:** (선택 사항) [!DNL Microsoft® Advertising] 캠페인을 위한 대상자 신호로 사용할 대상자. [!DNL Microsoft® Advertising] 기계 학습 모델은 대상을 사용하여 타깃팅할 유사한 웹 서퍼를 찾고, 성능 목표를 충족하는 데 도움이 되도록 신호로 지정되지 않은 대상에 광고를 표시할 수도 있습니다. 변환할 가능성이 가장 큰 대상을 선택하십시오.

>[!NOTE]
>대상 신호가 다음과 다름 [광고 그룹 수준 대상](/help/search-social-commerce/campaign-management/campaigns/audience-targets-manage.md).

<!-- **[!UICONTROL Display Path 1]**, **[!UICONTROL Display Path 2]:** -->

{{$include /help/_includes/display-path1-2.md}}

**[!UICONTROL Add new asset group]:** 다른 에셋 그룹을 지정할 수 있습니다.

## [!UICONTROL Conversion Goals]

**[!UICONTROL Conversion Goal]:** 종료 여부 *[!UICONTROL Use account conversion goals for this campaign]* (기본값) 또는 *[!UICONTROL Use campaign specific conversion goals]*. 캠페인에 대한 전환 목표를 지정하도록 선택한 경우 사용 가능한 모든 목표 목록에서 목표를 선택합니다. **참고:** 목표는 매일 동기화되므로 이전 24시간 동안 생성된 목표는 나열되지 않을 수 있습니다. 목록을 업데이트하려면 [수동으로 광고 네트워크 데이터 동기화](/help/search-social-commerce/campaign-management/campaigns/sync-network.md).

캠페인이 포트폴리오의 일부인 경우 포트폴리오의 목표와 동일한 전환 목표를 사용합니다. 다양한 전환 목표를 사용하면 포트폴리오 성능에 영향을 줄 수 있습니다.

>[!MORELIKETHIS]
>
>* [캠페인 관리](/help/search-social-commerce/campaign-management/campaigns/campaign-manage.md)
