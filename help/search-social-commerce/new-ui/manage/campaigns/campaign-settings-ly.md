---
title: '[!DNL LY Ads] 캠페인 설정'
description: ' [!DNL LY Ads] 캠페인에 대한 설정을 참조합니다.'
feature: Search Campaign Management
product_v2: id: a829a185-511f-4bf8-8dcf-9e684f8011cf
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: d45eb490f9dbb7da89bd1270582e5548b70cbd31
workflow-type: tm+mt
source-wordcount: 190
ht-degree: 0%

---

# [!DNL LY Ads] 캠페인 설정

## \[페이지 상단]

**[!UICONTROL Campaign Name]:** 계정에서 고유한 캠페인 이름.

**[!UICONTROL Status]:** 캠페인의 표시 상태: *활성* 또는 *일시 중지됨*. 새 광고 캠페인의 기본값은 *활성*&#x200B;입니다.

## [!UICONTROL Basic Settings] 탭

*새 캠페인만*

**[!UICONTROL Network]:** 광고 네트워크입니다.

**[!UICONTROL Account]:** 광고 네트워크 계정입니다.

**[!UICONTROL Campaign Type]:** 광고를 배치할 위치: 검색 네트워크에 텍스트 광고를 표시하는 유일한 옵션은 *[!UICONTROL Search Network Only]*&#x200B;입니다.

## [!UICONTROL Campaign Details] 탭

<!-- **[!UICONTROL Start date]:** -->

{{$include /help/_includes/start-date.md}}

<!-- **[!UICONTROL End date]:** -->

{{$include /help/_includes/end-date.md}}

## [!UICONTROL Budget Options]

**[!UICONTROL Budget]:** 일일 지출 금액인 평균 예산입니다. 최소 일일 예산은 100 JPY입니다.

캠페인 예산 제한이 자동으로 조정되는 포트폴리오에 이 캠페인을 지정하는 경우(검색 조건에 따라) 실제로 특정 기간에 지정된 예산보다 더 많이 또는 더 적게 지출할 수 있습니다.

<!-- **[!UICONTROL Delivery Method]:** -->

{{$include /help/_includes/delivery-method.md}}

## [!UICONTROL Campaign Targeting]

<!-- **[!UICONTROL Location Targets]:** -->

{{$include /help/_includes/location-targets.md}}

## [!UICONTROL URL Options]

<!-- **[!UICONTROL Tracking Template]:** -->

{{$include /help/_includes/tracking-template-yahoo-japan.md}}

## [!UICONTROL Additional Campaign Information] 탭

### [!UICONTROL Negative Keywords]

<!-- **[!UICONTROL Campaign Negative Keywords]:** -->

{{$include /help/_includes/negative-keyword.md}}

<!-- Note for **[!UICONTROL Campaign Negative Keywords]:** -->

{{$include /help/_includes/negative-keyword-note-yahoo-japan.md}}

### [!UICONTROL Campaign Tracking]

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
