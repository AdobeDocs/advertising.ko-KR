---
title: '[!DNL Google Ads] 광고 그룹 설정'
description: ' [!DNL Google Ads] 광고 그룹에 대한 설정을 참조합니다.'
exl-id: def75630-19b9-4676-ad34-5d9041cc3680
feature: Search Campaign Management
source-git-commit: 345c2af5363ca10412f3809700e281af5b06897f
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 0%

---

# [!DNL Google Ads] 광고 그룹 설정

## [!UICONTROL Adgroup Details]

**[!UICONTROL Ad Group Name]:** 캠페인 내에서 고유한 광고 그룹 이름입니다. 최대 길이는 255개의 더블바이트 문자입니다.

**[!UICONTROL Status]:** 광고 그룹의 표시 상태: *활성* 또는 *일시 중지됨*. 새 광고 그룹의 기본값은 *활성*&#x200B;입니다.

**[!UICONTROL Ad Group Type]:**(확장된 동적 검색 광고 캠페인만 해당) 광고 그룹 유형:

* *[!UICONTROL Search Standard]*(기본값): 표준 광고의 경우.

* 동적 검색 광고의 경우 *[!UICONTROL Search Dynamic]:*.

**[!UICONTROL Ad Rotation Mode]:** [!DNL Google Ads]이(가) 광고 그룹 내에서 서로 관련하여 활성 광고를 전달하는 빈도:

* *[!UICONTROL Optimize]:* Google 광고는 광고 그룹의 다른 광고보다 더 나은 성과를 기대하는 광고를 선호합니다. 이러한 광고는 광고 경매에 더 자주 참여하며 시간이 지남에 따라 단일 광고가 선호됩니다. 이는 비즈니스 및 최적화 목표와 일치하지 않을 수 있습니다.

* *[!UICONTROL Rotate forever]:*   각 광고는 더 많은 횟수로 광고 경매에 들어가므로 검색, 소셜 및 Commerce에서 클릭스루 비율뿐만 아니라 전환 횟수에서도 광고에 점수를 매길 수 있습니다.

* *[!UICONTROL Use campaign setting]*(새 광고 그룹의 기본값): 기존 캠페인 수준의 광고 순환 설정을 사용합니다. **참고:** 캠페인 수준 설정은 검색, 소셜 및 Commerce에 표시되지 않습니다.

캠페인이 스마트 입찰 입찰 전략(예: [!UICONTROL Target CPA], [!UICONTROL Target ROAS])을 사용하는 경우 [!DNL Google Ads]에서 옵션을 자동으로 &quot;[!UICONTROL Optimize]&quot;(으)로 설정합니다.

**[!UICONTROL Custom Bid Level]:**(디스플레이 네트워크만 대상으로 하는 캠페인) 입찰 방법: *[!UICONTROL Ad Group]*(기본값), *[!UICONTROL Age]*, *[!UICONTROL Gender]*, *[!UICONTROL Interest and List]*(Google 광고의 관심 분야 및 리마케팅), *[!UICONTROL Keyword]*, *[!UICONTROL Placement]*(웹 사이트), *[!UICONTROL Unknown]* 또는 *[!UICONTROL Vertical]*.

>[!NOTE]
>
>* 키워드로 입찰하면 키워드 수준에서 추적 템플릿을 만듭니다. 마찬가지로, 배치로 입찰하는 경우 배치 수준에서 추적 템플릿을 만듭니다. 다른 모든 차원에 대해 광고 수준에서 추적 템플릿을 만듭니다.
>* 포트폴리오의 캠페인에 대해 연령, 성별, 관심사 및 목록 또는 세로로 입찰할 때 최적화 기능이 차원에 대한 입찰을 최적화하지 않습니다. 또한 모든 속성이 광고 그룹에 적용됩니다.
>* 검색 네트워크의 광고는 항상 키워드 입찰을 사용합니다.

**[!UICONTROL AI Max Search Term Matching]:**(검색 네트워크를 대상으로 하며 [AI 최대 기능](https://support.google.com/google-ads/answer/15910366) 및 캠페인 수준 검색어 일치 기능이 활성화된 캠페인입니다. 읽기 전용) 광고 그룹 수준 검색어 일치가 활성화되어 있는지 여부: *[!UICONTROL Disabled]* 또는 *[!UICONTROL Enabled]*.

## [!UICONTROL Budget Options]

<!-- **[!UICONTROL Bid]:** -->

{{$include /help/_includes/bid-ad-group.md}}

**[!UICONTROL Target CPA]:**(입찰 [!UICONTROL Target CPA]개가 있는 캠페인, 선택 사항) 광고 그룹에 대한 CPA(획득당 목표 비용)입니다. 이 값은 캠페인 수준 타겟을 무시합니다.

**[!UICONTROL Target ROAS]:**(입찰 [!UICONTROL Target ROAS]개가 있는 캠페인, 선택 사항) 광고 그룹에 대한 ROAS(타겟 광고 투자 수익률)입니다. 이 값은 캠페인 수준 타겟을 무시합니다.

## [!UICONTROL Ad Group Targeting]

**[!UICONTROL Audience Target Method]:**(검색 네트워크에만 있는 캠페인 및 표시 네트워크에는 기존 읽기 전용 [!DNL Gmail] 캠페인):

* *[!UICONTROL Target and Bid]:* 광고 그룹의 다른 타겟도 충족하는 타겟 대상자와 연결된 사용자에게만 광고를 표시합니다.

* *[!UICONTROL Bid Only]:* 다른 광고 그룹 수준 타겟을 만족시키는 한 타겟 대상자와 연결되지 않은 사람에게도 광고를 표시합니다. 그러나 해당 대상에 대해 더 높은 입찰가를 설정하여 특정 대상에게 광고가 표시될 가능성을 높일 수 있습니다.

<!-- **[!UICONTROL Devices]:** -->

{{$include /help/_includes/devices.md}}

## [!UICONTROL URL Options]

<!-- **[!UICONTROL Tracking Template]:** -->

{{$include /help/_includes/tracking-template-google.md}}

## [!UICONTROL Negative Keywords]

<!-- **[!UICONTROL Negative Keywords]:** -->

{{$include /help/_includes/negative-keyword.md}}

<!-- Note for **[!UICONTROL Negative Keywords]:** -->

{{$include /help/_includes/negative-keyword-note-google.md}}

## [!UICONTROL Negative Websites]

<!-- **[!UICONTROL Negative Websites]:** -->

{{$include /help/_includes/negative-websites-google.md}}

>[!MORELIKETHIS]
>
>* [광고 그룹 관리](/help/search-social-commerce/campaign-management/campaigns/ad-group-manage.md)
