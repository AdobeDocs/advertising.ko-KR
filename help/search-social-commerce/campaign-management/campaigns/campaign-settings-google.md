---
title: '[!DNL Google Ads] 캠페인 설정'
description: ' [!DNL Google Ads] 캠페인에 대한 설정을 참조합니다.'
exl-id: 19973286-b7c8-496e-8b87-767cda6e3542
feature: Search Campaign Management
source-git-commit: cbe18b75d49ca53460883931ecea21aa6c2d8326
workflow-type: tm+mt
source-wordcount: '2472'
ht-degree: 0%

---

# [!DNL Google Ads] 캠페인 설정

## \[캠페인 만들기 화면\]

**[!UICONTROL Campaign Type]:**(캠페인 생성 중에만 사용 가능) 광고를 배치할 위치와 캠페인에 포함될 수 있는 광고 유형:

* *[!UICONTROL Search Network Only]:* 검색 네트워크에 [!DNL Google]개의 검색 결과와 선택적으로 검색 파트너 사이트를 포함하는 광고를 표시합니다. 각 광고 그룹에 대해 키워드를 지정해야 합니다.

* *[!UICONTROL Search with Display Select]:* 검색 네트워크(검색 결과 [!DNL Google]개 및 선택적으로 검색 파트너 사이트 포함)에 광고를 표시하고 디스플레이 네트워크 사이트에 광고를 표시할 수 있습니다. 디스플레이 네트워크에서 [!DNL Google Ads]은(는) 캠페인의 입찰 전략과 관계없이 자동화된 입찰을 사용하여 선택적으로 광고를 표시합니다. 검색 광고의 경우 각 광고 그룹에 대한 키워드를 지정하고, 디스플레이 광고의 경우 배치를 지정하고 선택적으로 각 광고 그룹에 대한 키워드를 지정합니다.

* *[!UICONTROL Shopping Network]:* 제품 광고를 표시합니다. 이 광고는 [!DNL Google]에서 [!DNL Google Shopping]의 [!DNL Google Merchant Center], [!DNL Google]개의 검색 결과 옆 영역(텍스트 광고와 별도) 및 검색 파트너 웹 사이트(선택 사항)에 있는 제품을 기반으로 자동으로 생성합니다. 캠페인의 각 광고 그룹에 대해 광고할 제품 그룹을 지정할 수 있습니다.

* *[!UICONTROL Display Network Only]:* 디스플레이 네트워크에 광고를 표시합니다. 각 광고 그룹에 대해 배치를 지정해야 하며 선택적으로 키워드를 지정할 수 있습니다.

* *[!UICONTROL Performance Max]:* [!DNL Google Ads] 스마트 입찰을 사용하여 채널 간 광고에 대한 전환을 표시하고 최적화합니다. 캠페인 설정 내에서 이미지, 로고, 헤드라인, 설명, 선택적 비디오 및 대상 신호를 포함하는 에셋 그룹을 하나 이상 지정해야 합니다. [!DNL Google Ads]은(는) 채널을 기반으로 광고를 제공할 자산을 자동으로 결합합니다([!DNL YouTube], [!DNL Gmail] 또는 [!DNL Search]).

  **메모:**

   * 필요한 설정만 사용할 수 있습니다. 옵션 설정을 보려면 [!DNL Google Ads] 편집기에 로그인합니다.

   * [!DNL Google Merchant Center] 제품 피드에 대한 링크는 지원되지 않습니다.

   * 목록 그룹 지원을 사용할 수 없습니다. 목록 그룹에 대한 데이터를 관리하고 보려면 [!DNL Google Ads] 편집기에 로그인하십시오.

   * 하이브리드 최적화가 지원됩니다. 입찰 전략 목표와 캠페인 예산은 캠페인 수준에서 설정됩니다.

## [!UICONTROL Campaign Details]

**[!UICONTROL Campaign Name]:** 계정 내에서 고유한 캠페인 이름.

<!-- **[!UICONTROL Start Date]:** -->

{{$include /help/_includes/start-date.md}}

**[!UICONTROL Audience Target Method]:**(기존, 읽기 전용 Gmail 캠페인만 해당) 다음을 수행할지 여부:

* *[!UICONTROL Target and Bid]* 광고 그룹의 다른 타겟을 충족시키는 타겟 대상자와 연결된 사용자에게만 광고를 표시합니다.

* *[!UICONTROL Bid Only]:* 다른 광고 그룹 수준 타겟을 만족시키는 한 타겟 대상자와 연결되지 않은 사람에게도 광고를 표시합니다. 그러나 해당 대상자에 대해 더 높은 입찰가를 설정하여 특정 대상자에게 광고가 표시될 가능성을 높일 수 있습니다.

**[!UICONTROL Status]:** 캠페인의 표시 상태: *활성* 또는 *일시 중지됨*. 새 광고 캠페인의 기본값은 *활성*&#x200B;입니다.

<!-- **[!UICONTROL End Date]:** -->

{{$include /help/_includes/end-date.md}}

**[!UICONTROL Search Partners]:**(쇼핑 캠페인을 포함하여 검색 네트워크만 대상으로 하는 캠페인) 표시
광고 네트워크의 검색 파트너 네트워크에 광고를 게시합니다. 기본적으로 이 옵션은 *[!UICONTROL Off]*&#x200B;입니다.

## [!UICONTROL Budget Options]

<!-- **[!UICONTROL Budget]:** -->

{{$include /help/_includes/budget.md}}

<!-- **[!UICONTROL Delivery Method]:** -->

{{$include /help/_includes/delivery-method.md}}

**[!UICONTROL Bid strategy]:** 캠페인에 대한 입찰 전략:

* *[!UICONTROL Enhanced CPC]:*&#x200B;은(는) 사용되지 않습니다. [!DNL Google Ads]이(가) 2025년 3월 15일부터 기존 [향상된 CPC 입찰 전략](https://support.google.com/google-ads/answer/2464964)을 수동 CPC로 자동으로 변경하기 시작했습니다.

* *[!UICONTROL Manual CPC]*(기본값): (성과 최대 캠페인에는 사용할 수 없음) 클릭당 비용(CPC) 모델을 사용합니다. 광고 네트워크에서 캠페인에 대한 입찰을 변경하도록 허용할 수 있습니다(선택적).

   * **[!UICONTROL Enable Enhanced CPC]**(기본적으로 비활성화됨): 사용되지 않는 &quot;[!UICONTROL Enhanced CPC]&quot; 옵션을 사용하는 것과 같습니다. [!DNL Google Ads]이(가) 2025년 3월 15일부터 기존 [향상된 CPC 입찰 전략](https://support.google.com/google-ads/answer/2464964)을 수동 CPC로 자동으로 변경하기 시작했습니다.

* *[!UICONTROL Maximize Clicks]:*(검색, 표시 및 쇼핑 캠페인) 검색, 소셜 및 Commerce이 아닌 광고 네트워크는 클릭수를 최대화하기 위해 입찰을 최적화합니다. 선택적으로 **[!UICONTROL Max CPC]**(클릭당 비용)을 입력하여 광고 네트워크가 클릭당 특정 금액 이상을 지불하지 않도록 합니다. **주의:** 이 전략을 사용하는 캠페인을 포트폴리오에 추가하면 입찰이 포트폴리오 목표가 아니라 클릭 가중치에 의해 결정됩니다.

* *[!UICONTROL Maximize Conversion Value]:*(검색, 성과 최대 및 스마트 쇼핑 캠페인) 검색, 소셜 및 Commerce이 아닌 광고 네트워크는 전환 값을 최대화하기 위해 입찰을 최적화합니다. 필요한 경우 **[!UICONTROL Target Return on Ad Spend]**(ROAS)을(를) 백분율로 입력하십시오. **참고:** 표준 포트폴리오가 아닌 하이브리드 포트폴리오의 캠페인에 이 옵션을 사용합니다. 하이브리드 포트폴리오에서 검색, 소셜 및 Commerce은 캠페인 수준 또는 (사용 가능한 경우) 광고 그룹 수준의 Target ROAS를 최적화합니다.

* *[!UICONTROL Maximize Conversions]:*(검색, 표시 및 성과 최대 캠페인) 검색, 소셜 및 Commerce이 아닌 광고 네트워크는 전환을 최대화하기 위해 입찰을 최적화합니다. 필요한 경우 **[!UICONTROL Target CPA]**(획득당 비용)을 입력합니다. **참고:** 표준 포트폴리오가 아닌 하이브리드 포트폴리오의 캠페인에 이 옵션을 사용합니다. 하이브리드 포트폴리오에서 검색, 소셜 및 Commerce은 캠페인 수준 또는 (사용 가능한 경우) 광고 그룹 수준의 Target CPA를 최적화합니다.

* *[!UICONTROL Target CPA]:*(캠페인 표시) 검색, 소셜 및 Commerce이 아닌 광고 네트워크는 선택적 **[!UICONTROL Target CPA]**(획득당 비용)을 기준으로 입찰을 최적화합니다. 이는 획득(전환)에 대해 지불할 30일 평균 금액입니다. **참고:** [!UICONTROL Weekly] 또는 [!UICONTROL Google Target CPA]을(를) 제외한 지출 전략이 있는 하이브리드 포트폴리오(표준 포트폴리오는 아님)의 캠페인에 이 옵션을 사용합니다. 하이브리드 포트폴리오에서 검색, 소셜 및 Commerce은 캠페인 수준 또는 (사용 가능한 경우) 광고 그룹 수준의 Target CPA를 최적화합니다.

  이 입찰 전략이 있는 캠페인에는 평균 위치 및 CPC 입찰 데이터를 사용할 수 없습니다.

* *[!UICONTROL Target Impression Share]:*(검색 캠페인) 검색, 소셜 및 Commerce이 아닌 광고 네트워크는 입찰을 최적화하여 타겟 노출 점유율 및 광고 위치를 달성합니다. **[!UICONTROL Target Impression Share]**, **[!UICONTROL Target Ad Position]** 및 **[!UICONTROL Max CPC]**(클릭당 비용)을(를) 입력합니다(선택 사항). **참고:** 이 옵션은 포트폴리오에서 지원되지 않습니다.

* *[!UICONTROL Target Return on Ad Spend]:*(디스플레이 및 쇼핑 캠페인) 검색, 소셜 및 Commerce이 아닌 광고 네트워크는 백분율로 지정된 **[!UICONTROL Target ROAS]**(광고 투자 수익률)을 기반으로 입찰을 최적화합니다. **참고:** [!UICONTROL Weekly] 또는 [!UICONTROL Google Target ROAS]을(를) 제외한 지출 전략이 있는 하이브리드 포트폴리오(표준 포트폴리오는 아님)의 캠페인에 이 옵션을 사용합니다. 하이브리드 포트폴리오에서 검색, 소셜 및 Commerce은 캠페인 수준 또는 (사용 가능한 경우) 광고 그룹 수준의 Target ROAS를 최적화합니다.

  이 입찰 전략이 있는 캠페인에는 평균 위치 및 CPC 입찰 데이터를 사용할 수 없습니다.

* *[!UICONTROL Viewable CPM]:*(기존, 읽기 전용 [!DNL Gmail] 캠페인만 해당) 검색, 소셜 및 Commerce이 아닌 광고 네트워크는 조회 가능한 것으로 측정된 광고에만 입찰합니다. **참고:** 이 전략에 대한 최적화는 포트폴리오 유형에서 지원되지 않습니다.

## [!UICONTROL Shopping Settings]

**[!UICONTROL Sales Country]:**(쇼핑 캠페인 전용, 기존 캠페인의 경우 읽기 전용)
캠페인의 제품이 판매됩니다. 제품은 대상 국가와 연결되어 있으므로 이 설정은 캠페인에 광고되는 제품을 결정합니다.

<!-- **[!UICONTROL Campaign Priority]:** -->

{{$include /help/_includes/campaign-priority.md}}

<!-- **[!UICONTROL Merchant ID]:** -->

{{$include /help/_includes/merchant-id.md}}

**[!UICONTROL Local Inventory Ads]:**(쇼핑 캠페인만 해당, 미국, 영국, DE, FR, JP 및 AU에 있는 [!DNL Google Merchant Center]개 매장을 사용하는 로컬 쇼핑 프로그램에 이미 참여하고 있는 광고주(선택 사항), [!DNL Google Ads]에서 Google.com의 쇼핑 광고에 로컬 인벤토리 정보를 자동으로 추가할 수 있습니다.

**팁:** 이 설정을 사용하는 경우 [!UICONTROL Inventory Filter] 설정에서 로컬 광고를 제외하지 마십시오.

**참고:** 로컬 인벤토리 광고에는 [!DNL Google Merchant Center]에 대한 두 개의 추가 피드가 필요합니다. 하나는 로컬 제품 데이터를 사용하고 다른 하나는 로컬 제품 인벤토리를 사용합니다. [로컬 쇼핑 광고](https://www.google.com/retail/local-inventory-ads/)에 대한 자세한 내용은 [!DNL Google Ads] 설명서를 참조하세요.

<!-- **[!UICONTROL Inventory Filter]:** -->

{{$include /help/_includes/inventory-filter.md}}

## [!UICONTROL Campaign Targeting]

**[!UICONTROL Languages]:**(검색 및 디스플레이 네트워크만 해당) 캠페인의 광고에 대한 하나 이상의 대상 언어입니다.

[!DNL Google Ads]은(는) 사용자의 [!DNL Google] 언어 설정 또는 [!DNL Google Display Network]에 있는 검색 쿼리, 현재 페이지 또는 최근에 본 페이지의 언어에서 사용자의 언어를 결정합니다.

**[!UICONTROL Location Targets]:** 대상으로 포함하거나 제외할 특정 사용자 지리적 위치입니다. 기본적으로 모든 위치가 타깃팅됩니다. 모든 위치의 조합에서 사용자를 포함 및 제외할 수 있습니다. 제외는 항상 포함을 무시합니다.

* 모든 위치를 타깃팅하려면 위치를 선택하지 마십시오.

* 특정 위치를 타겟팅하거나 제외하려면 다음을 수행합니다.

   * (국가, 주, 대도시 또는 도시) **[!UICONTROL Location Target]**(![위치 대상](/help/search-social-commerce/assets/location-target.png "위치 대상"))을 클릭하고 포함 및 제외할 위치를 찾으십시오.

      * 위치와 자식 위치를 포함하려면 파란색 확인 표시(![포함](/help/search-social-commerce/assets/include.png "포함"))가 나타나도록 인접한 원을 한 번 클릭합니다.

      * 위치를 제외하려면 인접한 원을 두 번 클릭하여 빨간색 확인 표시(![제외](/help/search-social-commerce/assets/exclude.png "제외"))를 표시합니다.

      * 위치를 하위 구성 요소(예: 미국 주, 대도시 또는 도시)로 확장하려면 위치 이름을 클릭합니다.

      * 위치를 검색하려면 입력 필드에 해당 위치의 처음 세 문자 이상을 입력하거나 붙여넣습니다. 검색 결과에서 포함할 위치 옆의 **[!UICONTROL Include]** 또는 제외할 위치 옆의 **[!UICONTROL Exclude]**&#x200B;을(를) 클릭합니다.

   * (주소 근처 위치, 포함된 대상만 해당) **[!UICONTROL Radius Target]**(![반경 대상](/help/search-social-commerce/assets/radius-target.png "반경 대상"))을 클릭한 다음 **[!UICONTROL Address]**&#x200B;을(를) 클릭합니다. 대상으로 지정할 주소 및 반경(마일 또는 킬로미터)을 입력한 다음 **[!UICONTROL Add]**&#x200B;을(를) 클릭합니다.

   * (지리적 좌표 근처의 위치, 포함된 대상만 해당) **[!UICONTROL Radius Target]**(![반경 대상](/help/search-social-commerce/assets/radius-target.png "반경 대상"))을 클릭한 다음 **[!UICONTROL Coordinate]**&#x200B;을(를) 클릭합니다. 타깃팅할 위치를 중심으로 마일 또는 킬로미터 단위로 위도와 경도 및 반경을 입력한 다음 **[!UICONTROL Add]**&#x200B;을(를) 클릭합니다.

* (포함된 대상 위치에 대한 입찰 조정을 추가하려면) 입찰 조정 값을 입력합니다.

* 0%: 이 위치에서 광고에 대한 입찰을 조정하지 않습니다.

* \[기타 값: -90% ~ 300%\]: 이 위치에서 광고 입찰을 늘리거나 줄이려면.

**참고:**

* [!DNL Google Ads]이(가) 서퍼 위치를 위치 대상에 매핑하기 위해 제공하는 데이터의 제한으로 인해 Search, Social 및 Commerce에서 다음 위치 대상에 대해 자동 조정된 입찰 조정을 제공하지 않습니다.

   * 반경 타겟.

   * [!DNL Google Ads]이(가) 서퍼의 URL에서 상위 위치를 보내지 않는 주/도/지역/군/현 수준 아래의 일부 위치(공항 및 미국 의회 지구 포함).

<!-- **[!UICONTROL Devices]:** -->

{{$include /help/_includes/devices.md}}

## [!UICONTROL Advanced Device Options]

**[!UICONTROL Mobile Carriers]:**(네트워크 표시 전용) 특정 이동통신사를 대상으로 합니다. 통신사는 정렬됩니다.
국가별로. 아무 것도 선택하지 않으면 모두 타겟팅됩니다.

**[!UICONTROL Mobile Carriers]:**(네트워크 표시 전용) 특정 운영 체제를 대상으로 합니다. 아무 것도 선택하지 않으면 모두 타겟팅됩니다.

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

## [!UICONTROL Customer Acquisition Goals]

**[!UICONTROL Customer Acquisition]:**(성과 최대 및 검색 캠페인만 해당) 새 고객 및 기존 고객에 대한 입찰을 할당하는 방법:

* *[!UICONTROL Bid equally for new and existing customers]*

* *[!UICONTROL Bid higher for new customers than for existing customers]*

  **참고:** 이 설정을 사용하려면 먼저 [!DNL Google Ads] 계정에 대해 새 고객 확보 목표를 활성화해야 하며, 해당하는 경우 관리자 계정에 대해 새 고객 확보 목표를 활성화해야 합니다. 목표는 적격한 기존 고객 목록과 전환 설정에서 새 고객에 대한 추가 전환 값을 정의합니다. [!DNL Google Ads] 도움말의 1-2단계 &quot;[새 고객 확보 목표 활성화](https://support.google.com/google-ads/answer/14007601)&quot;를 참조하십시오.

* *[!UICONTROL Only bid for new customers]*

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

**[!UICONTROL Track Product Group]:**([!UICONTROL EF Redirect]에만 해당) 구현되지 않음

<!-- **[!UICONTROL Append Parameters]:** -->

{{$include /help/_includes/append-parameters.md}}

## [!UICONTROL Asset Groups]&#x200B;(자산 그룹당)

**[!UICONTROL Asset Group Name]:** 자산 그룹의 이름입니다. [!DNL Google Merchant Center] 제품 피드에 대한 링크는 지원되지 않습니다.

**[!UICONTROL Asset Group Status]:** 자산 그룹의 상태: *[!UICONTROL Active]* 또는 *[!UICONTROL Paused]*.

**[!UICONTROL Final URL]:** 자산 그룹에서 만든 모든 광고의 최종 URL입니다. <!-- For campaigns created within Search, Social, & Commerce, final URL expansion is automatically enabled for the campaign, and Google Ads replaces this value with a more relevant landing page based on the user's search query and intent, and also customizes the headline based on the landing page content. You can disable final URL expansion, or exclude specific URLs from expansion, from within the [!DNL Google Ads] editor. -->

**[!UICONTROL Images]:** 다음 크기를 포함하여 광고용 이미지를 최대 15개까지 포함합니다. 1) 정사각형 이미지 3개 이상, 가로 이미지 3개 이상, 세로 이미지 1개 이상. [[!DNL Google Ads] 이미지 사양](https://support.google.com/google-ads/answer/10724492?hl=en&amp;ref_topic=10631992#zippy=,audience-signal-inputs,video-specifications,image-specifications)을 참조하세요. 이미지를 업로드하거나 [!UICONTROL Asset Library]에서 선택할 수 있지만 둘 다 동일한 작업에서 선택할 수는 없습니다.

* 이미지를 업로드하려면:

   1. [!UICONTROL Upload from Device] 탭에서 **[!UICONTROL +]**&#x200B;을(를) 클릭하고 장치 또는 네트워크에서 이미지를 선택합니다.

   1. 각 이미지에 대해:

      1. 종횡비를 선택합니다.

      1. 필요에 따라 자르기 상자를 끌어서 놓고 이미지의 볼 수 있는 부분을 선택한 다음 필요할 경우 이미지의 볼 수 있는 부분의 크기를 조정합니다.

      1. (선택 사항) 추가 종횡비를 선택하고 선택한 각 종횡비에 필요한 경우 이미지의 위치를 변경하고 크기를 선택적으로 조정합니다.

         선택한 각 종횡비에 대해 하나의 에셋이 만들어집니다.

      1. **[!UICONTROL Proceed]**&#x200B;을(를) 클릭합니다.

   1. 이미지 지정을 마치면 **[!UICONTROL Upload]**&#x200B;을(를) 클릭합니다.

* [!UICONTROL Asset Library]에서 이미지를 선택하려면 **[!UICONTROL Asset Library]**&#x200B;을(를) 클릭하고 이미지를 선택하십시오.

**[!UICONTROL Logos]:** 하나 이상의 사각형(1:1) 로고와 가로(4:1) 로고. 각 크기의 최대 5개를 포함할 수 있습니다. [[!DNL Google Ads] 로고 사양](https://support.google.com/google-ads/answer/10724492?hl=en&amp;ref_topic=10631992#zippy=,audience-signal-inputs,video-specifications,image-specifications)을 참조하세요. 이미지를 업로드하거나 [!UICONTROL Asset Library]에서 선택할 수 있지만 둘 다 동일한 작업에서 선택할 수는 없습니다.

* 이미지를 업로드하려면:

   1. [!UICONTROL Upload from Device] 탭에서 **[!UICONTROL +]**&#x200B;을(를) 클릭하고 장치 또는 네트워크에서 이미지를 선택합니다.

   1. 각 이미지에 대해:

      1. 종횡비를 선택합니다.

      1. 필요에 따라 자르기 상자를 끌어서 놓고 이미지의 볼 수 있는 부분을 선택한 다음 필요할 경우 이미지의 볼 수 있는 부분의 크기를 조정합니다.

      1. (선택 사항) 추가 종횡비를 선택하고 선택한 각 종횡비에 필요한 경우 이미지의 위치를 변경하고 크기를 선택적으로 조정합니다.

         선택한 각 종횡비에 대해 하나의 에셋이 만들어집니다.

      1. **[!UICONTROL Proceed]**&#x200B;을(를) 클릭합니다.

   1. 이미지 지정을 마치면 **[!UICONTROL Upload]**&#x200B;을(를) 클릭합니다.

* [!UICONTROL Asset Library]에서 이미지를 선택하려면 **[!UICONTROL Asset Library]**&#x200B;을(를) 클릭하고 이미지를 선택하십시오.

**[!UICONTROL Videos]:**(선택 사항) 최소 1개, 최대 5개의 [!DNL YouTube] 비디오가 최소 10초 동안 재생됩니다. URL을 입력하거나 [!UICONTROL Asset Library]에서 선택할 수 있지만 두 URL이 동일한 작업에서 모두 선택되지는 않습니다.

* URL을 입력하려면 다음을 수행하십시오.

   1. [!UICONTROL Enter Video Url] 탭에서 URL을 입력합니다.

   1. (선택 사항) 다른 URL을 추가하려면 **[!UICONTROL + Add]**&#x200B;을(를) 클릭하고 URL을 입력하십시오.

* [!UICONTROL Asset Library]에서 비디오를 선택하려면 **[!UICONTROL Asset Library]**&#x200B;을(를) 클릭하고 비디오를 선택하십시오.

**[!UICONTROL Headlines]:** 최소 3자, 최대 5자의 짧은 헤드라인(각각 최대 30자)입니다. 하나 이상의 헤드라인은 15자 이하여야 합니다. 최종 URL 확장을 활성화하는 캠페인 수준 옵션이 [!DNL Google Ads] 내에 설정된 경우 [!DNL Google Ads]은(는) 랜딩 페이지 콘텐츠를 기반으로 이 값을 사용자 지정 헤드라인으로 대체합니다.

텍스트를 입력하거나 [!UICONTROL Asset Library]에서 자산을 선택할 수 있지만, 두 작업 모두 같은 작업에서 선택할 수는 없습니다.

* 텍스트를 입력하려면 다음을 수행합니다.

   1. [!UICONTROL Enter Text] 탭에서 텍스트를 입력합니다.

   1. (선택 사항) 다른 텍스트 문자열을 추가하려면 **[!UICONTROL + Add]**&#x200B;을(를) 클릭하고 문자열을 입력합니다.

* [!UICONTROL Asset Library]에서 자산을 선택하려면 **[!UICONTROL Asset Library]**&#x200B;을(를) 클릭하고 자산을 선택하십시오.

**[!UICONTROL Long Headlines]:** 최소 1개, 최대 5개의 긴 헤드라인(각각 최대 90자). 텍스트를 입력하거나 [!UICONTROL Asset Library]에서 자산을 선택할 수 있지만, 두 작업 모두 같은 작업에서 선택할 수는 없습니다.

* 텍스트를 입력하려면 다음을 수행합니다.

   1. [!UICONTROL Enter Text] 탭에서 텍스트를 입력합니다.

   1. (선택 사항) 다른 텍스트 문자열을 추가하려면 **[!UICONTROL + Add]**&#x200B;을(를) 클릭하고 문자열을 입력합니다.

* [!UICONTROL Asset Library]에서 자산을 선택하려면 **[!UICONTROL Asset Library]**&#x200B;을(를) 클릭하고 자산을 선택하십시오.

**[!UICONTROL Descriptions]:** 최소 2개, 최대 4개의 설명(각각 최대 90자)입니다. 설명은 최소 30자 이하여야 합니다. 텍스트를 입력하거나 [!UICONTROL Asset Library]에서 자산을 선택할 수 있지만, 두 작업 모두 같은 작업에서 선택할 수는 없습니다.

* 텍스트를 입력하려면 다음을 수행합니다.

   1. [!UICONTROL Enter Text] 탭에서 텍스트를 입력합니다.

   1. (선택 사항) 다른 텍스트 문자열을 추가하려면 **[!UICONTROL + Add]**&#x200B;을(를) 클릭하고 문자열을 입력합니다.

* [!UICONTROL Asset Library]에서 자산을 선택하려면 **[!UICONTROL Asset Library]**&#x200B;을(를) 클릭하고 자산을 선택하십시오.

**[!UICONTROL Call to Action]:** 광고에 포함할 call to action. 기본적으로 *[!UICONTROL Automated]*&#x200B;이(가) 선택되어 있고 [!DNL Google Ads]이(가) call to action을 선택합니다. 선택적으로 다른 작업을 선택할 수 있습니다.

**[!UICONTROL Business Name]:** 비즈니스 이름으로, 최대 25자입니다.

**[!UICONTROL Audience Signal]:**(선택 사항) 캠페인을 위한 대상 신호로 사용할 대상 [!DNL Google Ads]개. [!DNL Google Ads] 기계 학습 모델은 대상을 사용하여 타깃팅할 유사한 웹 서퍼를 찾고, 성능 목표를 충족하는 데 도움이 되도록 신호로 지정되지 않은 대상에 광고를 표시할 수도 있습니다. 변환할 가능성이 가장 큰 대상을 선택하십시오.

>[!NOTE]
>대상자 신호가 [캠페인 수준 및 광고 그룹 수준의 대상자 대상](/help/search-social-commerce/campaign-management/campaigns/audience-targets-manage.md)과(와) 다릅니다.

**[!UICONTROL Primary Status]:**(성과 최대 캠페인의 기존 에셋 그룹에 대한 읽기 전용 필드) 에셋 그룹이 전체 용량으로 제공되거나 제공되지 않는 이유. 자산 그룹 상태뿐만 아니라 정책 및 품질 승인과 같은 기타 신호를 고려합니다. 값에는 *적격,* *제한,* *NOT_적격,* *일시 중지됨,* *보류 중,* *제거됨,* *알 수 없음,* 또는 *지정되지 않음.*<!-- GGL also has a Primary Status field for campaigns; if we ever sync that, then we'll need to distinguish between them. -->&#x200B;이 포함될 수 있습니다.

**[!UICONTROL Primary Status Reason]:**(성과 최대 캠페인의 기존 자산 그룹에 대한 읽기 전용 필드) 자산 그룹의 기본 상태에 대한 추가 세부 정보. 값에는 *ASSET_GROUP_DISAPPROVED,* *ASSET_GROUP_LIMITED,* *ASSET_GROUP_PAUSED,* *ASSET_GROUP_REMOVED,* *ASSET_GROUP_UNDER_REVIEW,* *CAMPAIGN_ENDED,* *CAMPAIGN_PAIGN_PAIGN,* *CAMPAIGN_PENDING,* *CAMPAIGN_REMOVED,* *UNKNOWN,* 또는 *미지정 안 됨}이 포함될 수 있습니다.*

## [!UICONTROL Conversion Goals]

**[!UICONTROL Conversion Goal]:** *[!UICONTROL Use account conversion goals for this campaign]*(기본값) 또는 *[!UICONTROL Use campaign specific conversion goals]* 중 어느 것을 사용할지 여부입니다. 캠페인에 대한 전환 목표를 지정하도록 선택한 경우 표준 목표를 선택하거나 캠페인에 대한 사용자 지정 목표를 만듭니다.

목표는 매일 동기화되므로 이전 24시간 동안 생성된 기존 목표는 나열되지 않을 수 있습니다. 목록을 업데이트하려면 [광고 네트워크 데이터를 수동으로 동기화](/help/search-social-commerce/campaign-management/campaigns/sync-network.md)하십시오.

사용자 지정 전환 목표를 만들려면 **[!UICONTROL + Add custom goal]**&#x200B;을(를) 클릭하고 사용자 지정 목표 이름을 입력한 다음 사용자 지정 목표에 포함할 [전환 작업](https://support.google.com/google-ads/answer/6032150)을(를) 선택한 다음 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다. **참고:** 각 캠페인에는 하나의 사용자 지정 목표만 있을 수 있습니다.

>[!TIP]
>
>캠페인이 하이브리드 포트폴리오의 일부인 경우 포트폴리오의 목표에서 전환 목표와 일치하는 캠페인 수준 목표를 사용하는 것이 좋습니다. 추가 전환 목표를 포함하면 포트폴리오 성능에 영향을 줄 수 있습니다.
>
>그러나 [목표를 광고 네트워크에 업로드](/help/search-social-commerce/tools/objective-upload-to-networks.md)하는 하이브리드 포트폴리오의 캠페인의 경우, 광고 네트워크의 편집기 내에서 다음 작업을 대신 수행하십시오. a) 업로드한 검색, 소셜 및 Commerce 포트폴리오 목표 지표(&quot;O_ACS_OBJ&quot;로 시작하는)를 캠페인에 대한 전환 작업으로 추가하고, b) 광고 네트워크에서 추적한 지표가 목표를 사용하여 광고 네트워크에 업로드되지 않으므로 [!DNL Google] 추적된 전환을 포함하는 캠페인 목표를 추가합니다.

>[!MORELIKETHIS]
>
>* [캠페인 관리](/help/search-social-commerce/campaign-management/campaigns/campaign-manage.md)
