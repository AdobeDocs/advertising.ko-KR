---
title: '[!DNL Baidu] 캠페인 설정'
description: ' [!DNL Baidu] 캠페인에 대한 설정을 참조합니다.'
feature: Search Campaign Management
product_v2: id: a829a185-511f-4bf8-8dcf-9e684f8011cf
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
source-git-commit: 3a5c2507f3acb08419e143ba906cf55df2496d0f
workflow-type: tm+mt
source-wordcount: 309
ht-degree: 0%

---

# [!DNL Baidu] 캠페인 설정

## \[페이지 상단]

**[!UICONTROL Campaign Name]:** 계정에서 고유한 캠페인 이름.

**[!UICONTROL Status]:** 캠페인의 표시 상태: *활성* 또는 *일시 중지됨*. 새 광고 캠페인의 기본값은 *활성*&#x200B;입니다.

## [!UICONTROL Basic Settings] 탭

*새 캠페인만*

**[!UICONTROL Network]:** 광고 네트워크입니다.

**[!UICONTROL Account]:** 광고 네트워크 계정입니다.

**[!UICONTROL Campaign Type]:** 광고를 배치할 위치와 캠페인에 포함될 수 있는 광고 유형입니다. 유일한 옵션은 *검색 네트워크만*&#x200B;입니다.

## [!UICONTROL Campaign Details] 탭

<!-- **[!UICONTROL Start Date]:** -->

{{$include /help/_includes/start-date.md}}

<!-- **[!UICONTROL End Date]:** -->

{{$include /help/_includes/end-date.md}}

**[!UICONTROL Contains EU Political Ads]:**(유럽 연합(EU)에서 대상을 타겟팅하는 캠페인에 적용) EU 규정 2024/90: *[!UICONTROL Yes]* 또는 *[!UICONTROL No]*&#x200B;에 따라 유럽 연합에서 제공되는 광고에 대한 요구 사항에 따라 캠페인에 정치적 광고가 포함되어 있는지 여부.

## [!UICONTROL Budget Options] 탭

<!-- **[!UICONTROL Budget]:** -->

{{$include /help/_includes/budget.md}}

<!-- **[!UICONTROL Delivery Method]:** -->

{{$include /help/_includes/delivery-method.md}}

<!--VERIFY OPTIMIZATION BEHAVIOR -->**[!UICONTROL Bid strategy]:** 캠페인에 대한 입찰 전략:

* *[!UICONTROL Maximize Conversions]:* 검색, 소셜 및 Commerce이 아닌 광고 네트워크는 전환을 최대화하기 위해 입찰을 최적화합니다. 필요한 경우 **[!UICONTROL Target CPA]**(획득당 비용)을 입력합니다. **참고:** 캠페인 수준 최적화가 적용된 포트폴리오의 캠페인에 이 옵션을 사용하십시오. 캠페인 수준 최적화를 사용하는 포트폴리오에서 검색, 소셜 및 Commerce은 Target CPA를 최적화합니다.

* *[!UICONTROL Maximize Conversion Value]:* 검색, 소셜 및 Commerce이 아닌 광고 네트워크는 전환 값을 최대화하기 위해 입찰을 최적화합니다. 필요한 경우 **[!UICONTROL Target Return on Ad Spend]**(ROAS)을(를) 백분율로 입력하십시오. **참고:** 캠페인 수준 최적화가 적용된 포트폴리오의 캠페인에 이 옵션을 사용하십시오. 캠페인 수준 최적화를 사용하는 포트폴리오에서 검색, 소셜 및 Commerce은 Target ROAS를 최적화합니다.

## [!UICONTROL Campaign Targeting] 탭

**[!UICONTROL Languages]:** 광고의 언어로서 광고가 표시될 수 있는 사이트의 언어와 일치해야 합니다. 광고 네트워크는 사용자의 쿼리, 게시자의 국가 및 사용자의 언어 설정을 포함한 다양한 신호로부터 사용자의 언어를 결정합니다.

<!-- **[!UICONTROL Location Targets]:** -->

{{$include /help/_includes/location-targets.md}}

## [!UICONTROL Additional Campaign Information] 탭

### [!UICONTROL Negative Keywords]

<!-- **[!UICONTROL Campaign Negative Keywords]:** -->

{{$include /help/_includes/negative-keyword.md}}

<!-- Note for **[!UICONTROL Campaign Negative Keywords]:** -->

{{$include /help/_includes/negative-keyword-note-baidu.md}}

### [!UICONTROL Campaign Tracking] 탭

<!-- **[!UICONTROL Override Account Tracking]:** -->

{{$include /help/_includes/override-account-tracking.md}}

<!-- **[!UICONTROL Tracking Type]:** -->

{{$include /help/_includes/tracking-type.md}}

<!-- **[!UICONTROL Redirect Type]:** -->

{{$include /help/_includes/redirect-type.md}}

**[!UICONTROL Tracking Level]:**([!UICONTROL EF Redirect]에만 해당) 리디렉션(해당되는 경우)을 추가하고 관련 URL에 매개 변수를 추가하여 클릭 수 및 매출을 추적해야 하는 수준:

* *[!UICONTROL Keyword]:* 키워드 수준에서만 데이터를 추적합니다.

* *[!UICONTROL Creative]:* 광고(광고) 수준에서만 데이터를 추적합니다.

* *[!UICONTROL Creative and Keyword]:* 광고(광고) 및 키워드 수준 모두에서 데이터를 추적하려면.

**[!UICONTROL Enable conversion reporting in Adobe Analytics]:** 전환 추적을 위해 계정이나 캠페인의 광고에 URL 매개 변수를 추가합니다.

<!-- **[!UICONTROL Encode Base URL]:** -->

{{$include /help/_includes/encode-base-url.md}}

<!-- **[!UICONTROL Append Parameters]:** -->

{{$include /help/_includes/append-parameters.md}}

<!--

Not there as of 7/22 -- what's going on here? If we're removing it, then I need to update many references throughout the whole doc:

[               **[!UICONTROL Auto Upload]:**      ]

{{$include /help/_includes/auto-upload.md}}

-->

>[!MORELIKETHIS]
>
>* [캠페인 관리](/help/search-social-commerce/new-ui/manage/campaigns/campaign-manage.md)
