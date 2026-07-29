---
title: '[!DNL Google Ads] 광고 그룹 설정'
description: ' [!DNL Google Ads] 광고 그룹에 대한 설정을 참조합니다.'
exl-id: def75630-19b9-4676-ad34-5d9041cc3680
feature: Search Campaign Management
TQID: https://experienceleague.adobe.com/pDFheVIM62XNCh2-7jbCscIqOrcTep7qnNg5S1tHYF8
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
source-git-commit: 41a9add10a9d12e8452d18825fd732720b27243f
workflow-type: tm+mt
source-wordcount: 549
ht-degree: 0%

---

# [!DNL Google Ads] 광고 그룹 설정

## \[페이지 상단]

**[!UICONTROL Ad Group Name]:** 캠페인 내에서 고유한 광고 그룹 이름입니다.

**[!UICONTROL Status]:** 캠페인의 표시 상태: *활성* 또는 *일시 중지됨*. 새 광고 캠페인의 기본값은 *활성*&#x200B;입니다.

## [!UICONTROL Basic Settings] 탭

*새 캠페인만*

**[!UICONTROL Network]:** 광고 네트워크입니다.

**[!UICONTROL Account]:** 광고 네트워크 계정입니다.

**[!UICONTROL Campaign]:** 캠페인입니다.

## [!UICONTROL Ad Group Details] 탭

**[!UICONTROL Ad Group Type]:**(확장된 동적 검색 광고 캠페인만 해당) 광고 그룹 유형:

* *[!UICONTROL Search Standard]*(기본값): 표준 광고의 경우.

* 동적 검색 광고의 경우 *[!UICONTROL Search Dynamic]:*.

**[!UICONTROL Ad Rotation Mode]:** [!DNL Google Ads]이(가) 광고 그룹 내에서 서로 관련하여 활성 광고를 전달하는 빈도:

* *[!UICONTROL Optimize]:* [!DNL Google Ads]은(는) 광고 그룹의 다른 광고보다 더 나은 성과를 기대하는 광고를 선호합니다. 이러한 광고는 광고 경매에 더 자주 참여하며 시간이 지남에 따라 단일 광고가 선호됩니다. 이는 비즈니스 및 최적화 목표와 일치하지 않을 수 있습니다.

* *[!UICONTROL Rotate forever]:* 각 광고는 더 많은 횟수로 광고 경매에 들어가므로 Search, Social 및 Commerce에서 클릭스루율뿐만 아니라 전환율에서도 광고를 채점할 수 있습니다.

* *[!UICONTROL Use campaign setting]*(새 광고 그룹의 기본값): 기존 캠페인 수준의 광고 순환 설정을 사용합니다. **참고:** 캠페인 수준 설정은 검색, 소셜 및 Commerce에 표시되지 않습니다.

캠페인이 스마트 입찰 입찰 전략(예: [!UICONTROL Target CPA], [!UICONTROL Target ROAS])을 사용하는 경우 [!DNL Google Ads]에서 옵션을 자동으로 &quot;[!UICONTROL Optimize]&quot;(으)로 설정합니다.

**[!UICONTROL Custom Bid Level]:**(디스플레이 네트워크만 대상으로 하는 캠페인) 입찰 방법: *[!UICONTROL Ad Group]*(기본값), *[!UICONTROL Age]*, *[!UICONTROL Gender]*, *[!UICONTROL Interest and List]*(Google 광고의 관심 분야 및 리마케팅), *[!UICONTROL Keyword]*, *[!UICONTROL Placement]*(웹 사이트), *[!UICONTROL Unknown]* 또는 *[!UICONTROL Vertical]*.

>[!NOTE]
>
>* 키워드로 입찰하면 키워드 수준에서 추적 템플릿을 만듭니다. 마찬가지로, 배치로 입찰하는 경우 배치 수준에서 추적 템플릿을 만듭니다. 다른 모든 차원에 대해 광고 수준에서 추적 템플릿을 만듭니다.
>* 포트폴리오의 캠페인에 대해 연령, 성별, 관심사 및 목록 또는 세로로 입찰할 때 최적화 기능이 차원에 대한 입찰을 최적화하지 않습니다. 또한 모든 속성이 광고 그룹에 적용됩니다.
>* 검색 네트워크의 광고는 항상 키워드 입찰을 사용합니다.

**[!UICONTROL AI Max Search Term Matching]:**(검색 네트워크를 대상으로 하며 [AI 최대 기능](https://support.google.com/google-ads/answer/15910366) 및 캠페인 수준 검색어 일치 기능이 활성화된 캠페인입니다. 읽기 전용) 광고 그룹 수준 검색어 일치가 활성화되어 있는지 여부: *[!UICONTROL Disabled]* 또는 *[!UICONTROL Enabled]*.

## [!UICONTROL Budget Options] 탭

<!-- **[!UICONTROL Bid]:** -->

{{$include /help/_includes/bid-ad-group.md}}

**[!UICONTROL Target CPA]:**(입찰 [!UICONTROL Target CPA]개가 있는 캠페인, 선택 사항) 광고 그룹에 대한 CPA(획득당 목표 비용)입니다. 이 값은 캠페인 수준 타겟을 무시합니다.

**[!UICONTROL Target ROAS]:**(입찰 [!UICONTROL Target ROAS]개가 있는 캠페인, 선택 사항) 광고 그룹에 대한 ROAS(타겟 광고 투자 수익률)입니다. 이 값은 캠페인 수준 타겟을 무시합니다.

## [!UICONTROL Ad Group Targeting] 탭

**[!UICONTROL Audience Target Method]:**(검색 네트워크에만 있는 캠페인 및 표시 네트워크에는 기존 읽기 전용 [!DNL Gmail] 캠페인):

* *[!UICONTROL Target and Bid]:* 광고 그룹의 다른 타겟도 충족하는 타겟 대상자와 연결된 사용자에게만 광고를 표시합니다.

* *[!UICONTROL Bid Only]:* 다른 광고 그룹 수준 타겟을 만족시키는 한 타겟 대상자와 연결되지 않은 사람에게도 광고를 표시합니다. 그러나 해당 대상에 대해 더 높은 입찰가를 설정하여 특정 대상에게 광고가 표시될 가능성을 높일 수 있습니다.

<!-- **[!UICONTROL Devices]:** -->

{{$include /help/_includes/devices.md}}

## [!UICONTROL AI Max] 탭

*검색 네트워크만 대상으로 하는 캠페인*

## [!UICONTROL AI Max] 탭

**[!UICONTROL AI Search Term Matching]:**([!DNL AI Max]이(가) 활성화된 캠페인만 해당) 도달 범위와 최적화를 향상시키기 위해 AI 기반 키워드 없는 검색어 일치를 사용할지 여부입니다.<!--SUPPOSEDLY, BUT THIS IS OFF FOR ME:  It's enabled by default for campaigns with [!DNL AI Max], but you can disable it at the ad group level. -->

**[!UICONTROL Locations of Interest]:**([!DNL AI Max]이(가) 활성화된 캠페인만 해당) 타깃팅할 지리적 의도의 특정 위치(제외는 아님). 사용자는 캠페인의 지리적 타깃팅도 충족해야 합니다. 기본적으로 모든 지리적 위치에 있거나, 정기적으로 또는 관심 있는 사용자가 타깃팅됩니다. 대상 범위를 좁히려면 타겟팅할 각 위치를 선택합니다.

## [!UICONTROL URL Options] 탭

<!-- **[!UICONTROL Tracking Template]:** -->

{{$include /help/_includes/tracking-template-google.md}}

## [!UICONTROL Additional Ad Group Information] 탭

### [!UICONTROL Negative Keywords]

<!-- **[!UICONTROL Negative Keywords]:** -->

{{$include /help/_includes/negative-keyword.md}}

<!-- Note for **[!UICONTROL Negative Keywords]:** -->

{{$include /help/_includes/negative-keyword-note-google.md}}

### [!UICONTROL Negative Websites]

<!-- **[!UICONTROL Negative Websites]:** -->

{{$include /help/_includes/negative-websites-google.md}}

>[!MORELIKETHIS]
>
>* [광고 그룹 관리](/help/search-social-commerce/campaign-management/campaigns/ad-group-manage.md)
