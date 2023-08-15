---
title: '[!DNL Google Ads] 캠페인 설정'
description: 다음에 대한 설정 참조 [!DNL Google Ads] 캠페인.
exl-id: d16ef1a9-f943-494c-8655-975383707f3c
feature: Search Campaign Management
source-git-commit: 1dbe8da7122b38dd11a242c453d71a832b31eee8
workflow-type: tm+mt
source-wordcount: '2025'
ht-degree: 0%

---

# [!DNL Google Ads] 캠페인 설정

## \[캠페인 만들기 화면\]

**[!UICONTROL Campaign Type]:** (캠페인 생성 중에만 사용 가능) 광고를 배치할 위치와 캠페인에 포함될 수 있는 광고 유형:

* *[!UICONTROL Search Network Only]:* 다음을 포함하는 검색 네트워크에 광고를 표시합니다. [!DNL Google] 검색 결과 및 선택적으로 파트너 사이트를 검색합니다. 각 광고 그룹에 대해 키워드를 지정해야 합니다.

* *[!UICONTROL Search with Display Select]:* 검색 네트워크에 광고를 표시합니다(다음 포함). [!DNL Google] 검색 결과 및 검색 파트너 사이트(선택 사항)를 검색하고 디스플레이 네트워크 사이트에 광고를 표시할 수 있습니다. 디스플레이 네트워크에서 [!DNL Google Ads] 캠페인의 입찰 전략에 관계없이 자동화된 입찰을 사용하여 광고를 선택적으로 표시합니다. 검색 광고의 경우 각 광고 그룹에 대한 키워드를 지정하고, 디스플레이 광고의 경우 배치를 지정하고 선택적으로 각 광고 그룹에 대한 키워드를 지정합니다.

* *[!UICONTROL Shopping Network]:* 제품 광고를 표시합니다. [!DNL Google] 는에서 제품을 기반으로 자동으로 생성됩니다. [!DNL Google Merchant Center] 날짜 [!DNL Google Shopping], 옆에 있는 영역 [!DNL Google] 검색 결과(텍스트 광고와 별도) 및 (선택 사항) 검색 파트너 웹 사이트. 캠페인의 각 광고 그룹에 대해 광고할 제품 그룹을 지정할 수 있습니다.

* *[!UICONTROL Display Network Only]:* 디스플레이 네트워크에 광고를 표시합니다. 각 광고 그룹에 대해 배치를 지정해야 하며 선택적으로 키워드를 지정할 수 있습니다.

* *[!UICONTROL Performance Max]:* (Beta 기능) 을 사용하여 채널 간 광고에 대한 전환을 표시하고 최적화합니다. [!DNL Google Ads] 현명한 입찰. 캠페인 설정 내에서 이미지, 로고, 헤드라인, 설명, 선택적 비디오 및 대상 신호를 포함하는 에셋 그룹을 하나 이상 지정해야 합니다. [!DNL Google Ads] 은 채널을 기반으로 광고를 게재할 자산을 자동으로 결합합니다(예: [!DNL YouTube], [!DNL Gmail], 또는 [!DNL Search]).

  **참고:**

   * 필요한 설정만 사용할 수 있습니다. 선택적 설정을 하려면에 로그인합니다. [!DNL Google Ads] 편집자.

   * 링크 대상 [!DNL Google Merchant Center] 제품 피드는 지원되지 않습니다.

   * 목록 그룹 지원을 사용할 수 없습니다. 목록 그룹에 대한 데이터를 관리하고 보려면 [!DNL Google Ads] 편집자.

   * 하이브리드 최적화가 지원됩니다. 입찰 전략 목표와 캠페인 예산은 캠페인 수준에서 설정됩니다.

## [!UICONTROL Campaign Details]

**[!UICONTROL Campaign Name]:** 계정 내에서 고유한 캠페인 이름.

<!-- **[!UICONTROL Start Date]:** -->

{{$include /help/_includes/start-date.md}}

**[!UICONTROL Audience Target Method]:**(기존, 읽기 전용 Gmail 캠페인만 해당)

* *[!UICONTROL Target and Bid]* 광고 그룹에 대한 다른 타겟을 충족시키는 타겟 대상과 연관된 사용자에게만 광고를 표시할 수 있습니다.

* *[!UICONTROL Bid Only]:*  다른 광고 그룹 수준의 타겟을 충족하는 한 타겟 대상자와 연결되지 않은 사람에게도 광고를 표시할 수 있습니다. 그러나 해당 대상자에 대해 더 높은 입찰가를 설정하여 특정 대상자에게 광고가 표시될 가능성을 높일 수 있습니다.

**[!UICONTROL Status]:** 캠페인의 표시 상태: *활성* 또는 *일시 중지됨*. 새 광고 캠페인의 기본값은 입니다 *활성*.

<!-- **[!UICONTROL End Date]:** -->

{{$include /help/_includes/end-date.md}}

**[!UICONTROL Search Partners]:** (쇼핑 캠페인을 포함하여 검색 네트워크만 타깃팅하는 캠페인) 광고 네트워크의 검색 파트너 네트워크에 광고를 표시합니다. 기본적으로 이 옵션은 *[!UICONTROL Off]*.

## [!UICONTROL Budget Options]

<!-- **[!UICONTROL Budget]:** -->

{{$include /help/_includes/budget.md}}

<!-- **[!UICONTROL Delivery Method]:** -->

{{$include /help/_includes/delivery-method.md}}

**[!UICONTROL Bid strategy]:** 캠페인에 대한 입찰 전략:

* *[!UICONTROL Enhanced CPC]:* (최대 성능 또는 기존 읽기 전용에는 사용할 수 없음) [!DNL Gmail] 캠페인 은 광고 네트워크의 향상된 클릭당 비용(eCPC) 모델을 사용합니다. 이 모델은 광고 네트워크에서 평균 CPC를 최대 CPC 미만으로 유지하려고 하는 동안 전환을 최대화하기 위해 광고 네트워크(검색, 소셜 및 상거래에 있지 않음)에서 지정된 전환을 사용하여 각 경매에 대한 클릭당 비용(CPC) 입찰을 자동으로 변경할 수 있도록 합니다.

최적화된 검색, 소셜 및 상거래 포트폴리오에 eCPC가 있는 캠페인을 추가하면 검색, 소셜 및 상거래는 기본 입찰가를 최적화하고,[!UICONTROL Auto adjust campaign budget limits]&quot;옵션이 활성화됨 — 캠페인 예산. 광고 네트워크는 모든 입찰 조정을 최적화하고 독점 데이터 및 통찰력을 기반으로 사용자 쿼리 시 검색, 소셜 및 상거래에서 생성한 입찰을 변경할 수 있습니다. **주의:** 광고 네트워크에서 추적된 총 전환이 포트폴리오 목표에 맞는 경우에만 포트폴리오에서 eCPC 캠페인을 사용하십시오. <!-- Note to self: Within the ad network UI, you specify conversion goals either a) all conversion actions you've set to be included in "Conversions" at the account level or b) one or more individual conversions to use for optimization -->

* *[!UICONTROL Manual CPC]* (기본값): (성과 최대 캠페인에는 사용할 수 없음) 클릭당 비용(CPC) 모델을 사용합니다. 광고 네트워크에서 캠페인에 대한 입찰을 변경하도록 허용할 수 있습니다(선택적).

   * **[!UICONTROL Enable Enhanced CPC]** (기본적으로 비활성화됨): &quot;[!UICONTROL Enhanced CPC]&quot; 옵션입니다.

* *[!UICONTROL Maximize Clicks]:* (검색, 표시 및 쇼핑 캠페인) 검색, 소셜 및 상거래가 아닌 광고 네트워크는 클릭수를 최대화하기 위해 입찰을 최적화합니다. 다음을 입력합니다(선택적). **[!UICONTROL Max CPC]** (클릭당 비용) 광고 네트워크가 클릭당 특정 금액 이상을 지불하지 않도록 하기 위한 것입니다. **주의:** 이 전략을 사용하는 캠페인을 포트폴리오에 추가하면 입찰은 포트폴리오 목표가 아니라 클릭 가중치에 의해 결정됩니다.

* *[!UICONTROL Maximize Conversion Value]:* (검색, 성과 최대 및 스마트 쇼핑 캠페인) 검색, 소셜 및 상거래가 아닌 광고 네트워크는 전환 가치를 극대화하기 위해 입찰을 최적화합니다. 필요한 경우 다음을 입력합니다. **[!UICONTROL Target Return on Ad Spend]** (ROAS)(백분율)입니다. **참고:** 표준 포트폴리오가 아닌 하이브리드 포트폴리오의 캠페인에 이 옵션을 사용합니다.

* *[!UICONTROL Maximize Conversions]:* (검색, 표시 및 성과 최대 캠페인) 검색, 소셜 및 상거래가 아닌 광고 네트워크는 전환을 최대화하기 위해 입찰을 최적화합니다. 필요한 경우 다음을 입력합니다. **[!UICONTROL Target CPA]** (취득당 비용) **참고:** 표준 포트폴리오가 아닌 하이브리드 포트폴리오의 캠페인에 이 옵션을 사용합니다.

* *[!UICONTROL Target CPA]:* (캠페인 표시, 기존 검색 캠페인) 검색, 소셜 및 상거래가 아닌 광고 네트워크는 선택 사항을 기반으로 입찰을 최적화합니다 **[!UICONTROL Target CPA]** (취득당 비용) - 취득(전환)에 대해 지불할 30일 평균 금액입니다. **참고:** 지출 전략을 사용하는 하이브리드 포트폴리오(표준 포트폴리오는 아님)의 캠페인에 이 옵션을 사용합니다. [!UICONTROL Weekly] 또는 [!UICONTROL Google Target CPA].

  이 입찰 전략이 있는 캠페인에는 평균 위치 및 CPC 입찰 데이터를 사용할 수 없습니다.

  새 검색 캠페인의 경우 [!DNL Google Ads] 이(가) 이 입찰 전략을 (으)로 대체했습니다. [!UICONTROL Maximize Conversions] 를 사용한 전략 [!UICONTROL Target CPA] 값. 이 전략을 사용하는 기존 검색 캠페인의 경우 타겟 값만 편집할 수 있으며 이렇게 하면 전략이 [!UICONTROL Maximize Conversions] 지정된 을 사용한 전략 [!UICONTROL Target CPA] 값.

* *[!UICONTROL Target Impression Share]:* (검색 캠페인) 검색, 소셜 및 상거래가 아닌 광고 네트워크는 타겟 노출 점유율 및 광고 위치를 달성하기 위해 입찰을 최적화합니다. 다음을 입력합니다(선택적). **[!UICONTROL Target Impression Share]** 백분율로, **[!UICONTROL Target Ad Position]**, 및 **[!UICONTROL Max CPC]** (클릭당 비용) **참고:** 이 옵션은 포트폴리오에서 지원되지 않습니다.

* *[!UICONTROL Target Return on Ad Spend]:*  (디스플레이 및 쇼핑 캠페인, 기존 검색 캠페인) 검색, 소셜 및 상거래가 아닌 광고 네트워크는 지정된 항목을 기반으로 입찰을 최적화합니다 **[!UICONTROL Target ROAS]** (광고 투자 수익률), 백분율로 지정됩니다. **참고:** 지출 전략을 사용하는 하이브리드 포트폴리오(표준 포트폴리오는 아님)의 캠페인에 이 옵션을 사용합니다. [!UICONTROL Weekly] 또는 [!UICONTROL Google Target ROAS].

  이 입찰 전략이 있는 캠페인에는 평균 위치 및 CPC 입찰 데이터를 사용할 수 없습니다.

  새 검색 캠페인의 경우 [!DNL Google Ads] 이(가) 이 입찰 전략을 (으)로 대체했습니다. [!UICONTROL Maximize Conversion Value] 를 사용한 전략 [!UICONTROL Target Return on Ad Spend value]. 이 전략을 사용하는 기존 검색 캠페인의 경우 타겟 값만 편집할 수 있으며 이렇게 하면 전략이 [!UICONTROL Maximize Conversion Value] 지정된 을 사용한 전략 [!UICONTROL Target Return on Ad Spend] 값.

* *[!UICONTROL Viewable CPM]:* (기존, 읽기 전용 [!DNL Gmail] 캠페인 전용) 검색, 소셜 및 상거래가 아닌 광고 네트워크는 조회 가능한 것으로 측정된 광고에만 입찰합니다. **참고:** 이 전략에 대한 최적화는 어떤 유형의 포트폴리오에서도 지원되지 않습니다.

## [!UICONTROL Shopping Settings]

**[!UICONTROL Sales Country]:** (쇼핑 캠페인 전용, 기존 캠페인의 경우 읽기 전용) 캠페인의 제품이 판매되는 국가입니다. 제품은 대상 국가와 연결되어 있으므로 이 설정은 캠페인에 광고되는 제품을 결정합니다.

<!-- **[!UICONTROL Campaign Priority]:** -->

{{$include /help/_includes/campaign-priority.md}}

<!-- **[!UICONTROL Merchant ID]:** -->

{{$include /help/_includes/merchant-id.md}}

**[!UICONTROL Local Inventory Ads]:** (쇼핑 캠페인만 해당). 광고주는 이미 다음과 같이 로컬 쇼핑 프로그램에 참여하고 있습니다. [!DNL Google Merchant Center] 미국, 영국, DE, FR, JP 및 AU의 상점(선택 사항) 허용 [!DNL Google Ads] 로컬 인벤토리 정보를 Google.com의 쇼핑 광고에 자동으로 추가합니다.

**팁:** 이 설정을 사용하는 경우 [!UICONTROL Inventory Filter] 설정.

**참고:** 로컬 인벤토리 광고에는 다음 작업을 수행하는 데 두 개의 추가 피드가 필요합니다. [!DNL Google Merchant Center] — 하나는 로컬 제품 데이터를 사용하고 다른 하나는 로컬 제품 인벤토리를 사용합니다. 다음을 참조하십시오. [!DNL Google Ads] 에 대한 자세한 내용은 설명서 를 참조하십시오. [로컬 쇼핑 광고](https://www.google.com/retail/local-inventory-ads/).

<!-- **[!UICONTROL Inventory Filter]:** -->

{{$include /help/_includes/inventory-filter.md}}

## [!UICONTROL Campaign Targeting]

**[!UICONTROL Languages]:** (검색 및 디스플레이 네트워크만 해당) 캠페인의 광고에 대한 하나 이상의 타겟 언어입니다.

[!DNL Google Ads] 사용자의 언어에서 사용자의 언어를 결정합니다. [!DNL Google] 언어 설정 또는 검색 쿼리, 현재 페이지 또는 최근에 본 페이지의 언어 [!DNL Google Display Network].

**[!UICONTROL Location Targets]:** 타겟으로 포함하거나 제외할 특정 사용자 지리적 위치. 기본적으로 모든 위치가 타깃팅됩니다. 모든 위치의 조합에서 사용자를 포함 및 제외할 수 있습니다. 제외는 항상 포함을 무시합니다.

* 모든 위치를 타깃팅하려면 위치를 선택하지 마십시오.

* 특정 위치를 타겟팅하거나 제외하려면 다음을 수행합니다.

   * (국가, 주, 대도시 또는 도시) 클릭 **[!UICONTROL Location Target]** (![위치 대상](/help/search-social-commerce/assets/location-target.png "위치 대상")) 포함 및 제외할 위치를 찾습니다.

      * 위치와 자식 위치를 포함하려면 파란색 확인 표시가 되도록 옆에 있는 원을 한 번 클릭합니다(![포함](/help/search-social-commerce/assets/include.png "포함"))가 표시됩니다.

      * 위치를 제외하려면 빨간색 확인 표시()가 되도록 옆에 있는 원을 두 번 클릭합니다.![제외](/help/search-social-commerce/assets/exclude.png "제외"))가 표시됩니다.

      * 위치를 하위 구성 요소(예: 미국 주, 대도시 또는 도시)로 확장하려면 위치 이름을 클릭합니다.

      * 위치를 검색하려면 입력 필드에 해당 위치의 처음 세 문자 이상을 입력하거나 붙여넣습니다. 검색 결과에서 **[!UICONTROL Include]** 또는 을 포함할 위치 옆 **[!UICONTROL Exclude]** 를 클릭합니다.

   * (주소 근처 위치, 포함된 대상만 해당) 클릭 **[!UICONTROL Radius Target]** (![반경 대상](/help/search-social-commerce/assets/radius-target.png "반경 대상"))을 클릭한 다음 **[!UICONTROL Address]**. 주소 및 타깃팅할 주소 주변 반경(마일 또는 킬로미터)을 입력한 다음 을 클릭합니다. **[!UICONTROL Add]**.

   * (지리적 좌표 근처의 위치, 포함된 대상만 해당) 클릭 **[!UICONTROL Radius Target]** (![반경 대상](/help/search-social-commerce/assets/radius-target.png "반경 대상"))을 클릭한 다음 **[!UICONTROL Coordinate]**. 타깃팅할 위치를 중심으로 마일 또는 킬로미터 단위로 위도와 경도 및 반경을 입력한 다음 을 클릭합니다. **[!UICONTROL Add]**.

   * (위치 근처) [!DNL My Business] 위치 확장으로 사용할 수 있는 위치. 포함된 대상만 해당) **[!UICONTROL Location Group Target]** (![위치 그룹](/help/search-social-commerce/assets/location-group.png "위치 그룹")); 국가, 주, 대도시 또는 도시를 입력하여 사용 가능한 위치 목록 아래에 화살표를 놓은 후, 목록에서 위치를 하나 이상 선택합니다(선택 사항). [!DNL Google My Business] 위치. 타깃팅할 위치 주변의 반경(마일 또는 킬로미터)을 지정한 다음 를 클릭합니다. **[!UICONTROL Add]**.

* (포함된 대상 위치에 대한 입찰 조정을 추가하려면) 입찰 조정 값을 입력합니다.

* 0%: 이 위치에서 광고에 대한 입찰을 조정하지 않습니다.

* \[기타 값: -90% ~ 300%\]: 이 위치에서 광고 입찰을 늘리거나 줄이려면.

**참고:**

* Search, Social 및 Commerce는 데이터의 제한으로 인해 다음 위치 대상에 대해 자동 조정된 입찰 조정을 제공하지 않습니다. [!DNL Google Ads] 는 서퍼 위치를 위치 대상에 매핑합니다.

   * 반경 타겟.

   * 다음에 대한 주/도/지역/군/현 수준 아래의 일부 위치 [!DNL Google Ads] 은 공항과 미국 의회 지역을 포함하여 서퍼의 URL에서 상위 위치를 전송하지 않습니다.

<!-- **[!UICONTROL Devices]:** -->

{{$include /help/_includes/devices.md}}

## [!UICONTROL Advanced Device Options]

**[!UICONTROL Mobile Carriers]:** (네트워크 표시만 해당) 타깃팅할 특정 이동통신사, 통신사는 국가별로 정렬됩니다. 아무 것도 선택하지 않으면 모두 타겟팅됩니다.

**[!UICONTROL Mobile Carriers]:** (네트워크만 표시) 타깃팅할 특정 운영 체제입니다. 아무 것도 선택하지 않으면 모두 타겟팅됩니다.

## [!UICONTROL URL Options]

<!-- **[!UICONTROL Tracking Template]:** -->

{{$include /help/_includes/tracking-template-google.md}}

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

{{$include /help/_includes/negative-keyword-note-google.md}}

## [!UICONTROL Negative Websites]

<!-- **[!UICONTROL Negative Websites]:** -->

{{$include /help/_includes/negative-websites-google.md}}

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

**[!UICONTROL Asset Group Name]:** 자산 그룹의 이름입니다. 링크 대상 [!DNL Google Merchant Center] 제품 피드는 지원되지 않습니다.

**[!UICONTROL Asset Group Status]:** 자산 그룹의 상태: *[!UICONTROL Active]* 또는 *[!UICONTROL Paused]*.

**[!UICONTROL Final URL]:** 자산 그룹에서 만든 모든 광고의 최종 URL입니다. <!-- For campaigns created within Search, Social, & Commerce, final URL expansion is automatically enabled for the campaign, and Google Ads replaces this value with a more relevant landing page based on the user's search query and intent, and also customizes the headline based on the landing page content. You can disable final URL expansion, or exclude specific URLs from expansion, from within the [!DNL Google Ads] editor. -->

**[!UICONTROL Images]:** 다음 크기를 포함하여 광고용 이미지 최대 15개. 1) 정사각형 이미지 3개 이상, 2) 가로 이미지 3개 이상, 3) 세로 이미지 1개 이상 다음을 참조하십시오. [[!DNL Google Ads] 이미지 사양](https://support.google.com/google-ads/answer/10724492?hl=en&amp;ref_topic=10631992#zippy=,audience-signal-inputs,video-specifications,image-specifications). 이미지를 업로드하려면:

1. 클릭 **[!UICONTROL +]** 장치 또는 네트워크에서 이미지를 선택합니다.

1. 각 이미지에 대해:

   1. 종횡비를 선택합니다.

   1. 필요에 따라 자르기 상자를 끌어서 놓고 이미지의 볼 수 있는 부분을 선택한 다음 필요할 경우 이미지의 볼 수 있는 부분의 크기를 조정합니다.

   1. (선택 사항) 추가 종횡비를 선택하고 선택한 각 종횡비에 필요한 경우 이미지의 위치를 변경하고 크기를 선택적으로 조정합니다.

      선택한 각 종횡비에 대해 하나의 에셋이 만들어집니다.

   1. 클릭 **[!UICONTROL Proceed]**.

1. 이미지 지정이 끝나면 **[!UICONTROL Upload]**.

**[!UICONTROL Logos]:** 하나 이상의 사각형(1:1) 로고 및 가로(4:1) 로고. 각 크기의 최대 5개를 포함할 수 있습니다. 다음을 참조하십시오. [[!DNL Google Ads] 로고 사양](https://support.google.com/google-ads/answer/10724492?hl=en&amp;ref_topic=10631992#zippy=,audience-signal-inputs,video-specifications,image-specifications). 이미지를 업로드하려면:

1. 클릭 **[!UICONTROL +]** 장치 또는 네트워크에서 이미지를 선택합니다.

1. 각 이미지에 대해:

   1. 종횡비를 선택합니다.

   1. 필요에 따라 자르기 상자를 끌어서 놓고 이미지의 볼 수 있는 부분을 선택한 다음 필요할 경우 이미지의 볼 수 있는 부분의 크기를 조정합니다.

   1. (선택 사항) 추가 종횡비를 선택하고 선택한 각 종횡비에 필요한 경우 이미지의 위치를 변경하고 크기를 선택적으로 조정합니다.

      선택한 각 종횡비에 대해 하나의 에셋이 만들어집니다.

   1. 클릭 **[!UICONTROL Proceed]**.

1. 이미지 지정이 끝나면 **[!UICONTROL Upload]**.

**[!UICONTROL Videos]:** (선택 사항) 최소 1개, 최대 5개의 URL [!DNL YouTube] 최소 10초 길이의 비디오입니다.

**[!UICONTROL Headlines]:** 최소 3자, 최대 5자의 짧은 머리글로 각각 최대 30자까지 사용할 수 있습니다. 하나 이상의 헤드라인은 15자 이하여야 합니다. 최종 URL 확장을 활성화하는 캠페인 수준 옵션이 [!DNL Google Ads], 그런 다음 [!DNL Google Ads] 는 이 값을 랜딩 페이지 콘텐츠를 기반으로 하는 사용자 지정 헤드라인으로 대체합니다.

**[!UICONTROL Long Headlines]:** 각각 최대 90자의 긴 머리글이 최소 1개에서 최대 5개까지 표시됩니다.

**[!UICONTROL Descriptions]:** 최소 2자부터 최대 4자까지 최대 90자까지 입력할 수 있습니다. 설명은 최소 30자 이하여야 합니다.

**[!UICONTROL Call to Action]:** 광고에 포함할 클릭 유도 문안. 기본적으로, *[!UICONTROL Automated]* 이(가) 선택되어 있고 [!DNL Google Ads] 콜 투 액션을 선택합니다. 선택적으로 다른 작업을 선택할 수 있습니다.

**[!UICONTROL Business Name]:** 비즈니스 이름(최대 25자).

**[!UICONTROL Add new asset group]:** 다른 에셋 그룹을 지정할 수 있습니다.

>[!MORELIKETHIS]
>
>* [캠페인 관리](/help/search-social-commerce/campaign-management/campaigns/campaign-manage.md)
