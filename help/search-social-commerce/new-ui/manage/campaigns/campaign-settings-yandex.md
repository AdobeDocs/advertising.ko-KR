---
title: '[!DNL Yandex] 캠페인 설정'
description: ' [!DNL Yandex] 캠페인에 대한 설정을 참조합니다.'
feature: Search Campaign Management
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: d45eb490f9dbb7da89bd1270582e5548b70cbd31
workflow-type: tm+mt
source-wordcount: 252
ht-degree: 0%

---

# [!DNL Yandex] 캠페인 설정

## \[페이지 상단]

**[!UICONTROL Campaign Name]:** 계정에서 고유한 캠페인 이름.

**[!UICONTROL Status]:** 캠페인의 표시 상태: *활성* 또는 *일시 중지됨*. 새 광고 캠페인의 기본값은 *활성*&#x200B;입니다.

## [!UICONTROL Basic Settings] 탭

*새 캠페인만*

**[!UICONTROL Network]:** 광고 네트워크입니다.

**[!UICONTROL Account]:** 광고 네트워크 계정입니다.

**[!UICONTROL Campaign Type]:** 광고를 배치할 위치:

* *[!UICONTROL Search Network Only]:* 검색 네트워크에 텍스트 광고를 표시합니다. 각 광고 그룹에 대해 키워드를 지정해야 합니다.

* *[!UICONTROL Search and Display Network]:* 검색 네트워크 및 [!DNL Yandex Advertising Network]에 텍스트 광고를 표시합니다. 검색 광고의 경우 각 광고 그룹에 대한 검색 키워드를 지정해야 합니다. 디스플레이 광고의 경우 각 광고 그룹에 대해 광고할 웹 사이트에 대한 키워드를 지정해야 합니다.

* *[!UICONTROL Display Network Only]:*&#x200B;이(가) [!DNL Yandex Advertising Network]에 텍스트 광고를 표시합니다. 각 광고 그룹에 대해 광고할 웹 사이트에 대한 키워드를 지정해야 합니다.

## [!UICONTROL Campaign Details] 탭

<!-- **[!UICONTROL Start date]:** -->

{{$include /help/_includes/start-date.md}}

## [!UICONTROL Budget Options] 탭

**[!UICONTROL Budget]:** 계정의 예산 유형에 따라 일일(평균) 또는 캠페인 기간 동안 소비할 금액인 예산입니다. 최소 예산은 py6 300, EUR 10 또는 USD 10입니다.

**메모:**

* 새 캠페인에는 입찰 관리 전략 &quot;가장 높은 가용 위치&quot;가 있습니다.

* 검색 조건에 따라 캠페인 예산 한도를 자동으로 조정할 수 있도록 구성된 포트폴리오에 이 캠페인을 할당하면 주어진 일, 월 또는 라이프타임에 지정된 예산보다 실제로 더 많이 또는 더 적게 지출할 수 있습니다.

<!-- **[!UICONTROL Delivery Method]:** -->

{{$include /help/_includes/delivery-method.md}}

## [!UICONTROL Additional Campaign Information] 탭

### [!UICONTROL Campaign Tracking]

<!-- **[!UICONTROL Override Account Tracking]:** -->

<!-- **[!UICONTROL Override Account Tracking]:** -->

{{$include /help/_includes/override-account-tracking.md}}

<!-- **[!UICONTROL Tracking Type]:** -->

{{$include /help/_includes/tracking-type.md}}

<!-- **[!UICONTROL Redirect Type]:** -->

{{$include /help/_includes/redirect-type.md}}

**[!UICONTROL Tracking Level]:**([!UICONTROL EF Redirect]에만 해당하며 읽기 전용) 클릭 수와 매출을 추적해야 하는 수준입니다. *[!UICONTROL Creative]*&#x200B;만 [!DNL Yandex]에 사용할 수 있습니다. 데이터는 광고(광고) 수준에서만 추적됩니다.

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
