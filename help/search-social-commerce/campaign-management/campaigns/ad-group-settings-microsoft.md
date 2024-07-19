---
title: '[!DNL Microsoft Advertising] 광고 그룹 설정'
description: ' [!DNL Microsoft Advertising] 광고 그룹에 대한 설정을 참조합니다.'
exl-id: 5d788e5b-ddf3-4f4e-8e8d-98e3235cb187
feature: Search Campaign Management
source-git-commit: 67fe8581832dc0762d62908d01672e53cc95b847
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---

# [!DNL Microsoft Advertising] 광고 그룹 설정

## [!UICONTROL Adgroup Details]

**[!UICONTROL Ad Group Name]:** 캠페인 내에서 고유한 광고 그룹 이름입니다. 최대 길이는 128자입니다.

**[!UICONTROL Status]:** 광고 그룹의 표시 상태: *활성* 또는 *일시 중지됨*. 새 광고 그룹의 기본값은 *활성*&#x200B;입니다.

**[!UICONTROL Ad Language]:**(검색 캠페인) 광고 대상 언어입니다.

<!-- **[!UICONTROL Start Date]:** -->

{{$include /help/_includes/start-date.md}}

<!-- **[!UICONTROL End Date]:** -->

{{$include /help/_includes/end-date.md}}

## [!UICONTROL Networks]

**[!UICONTROL Networks]:**(광고 검색) 광고 그룹 내에 광고를 배치하는 방법 및 위치:

* *[!UICONTROL Only Microsoft Advertising and Yahoo! websites]*(기본값): 검색 네트워크에 광고 입찰을 합니다.

* *[!UICONTROL Only Microsoft Advertising and Yahoo! syndicated search partners]:* 신디케이트된 파트너 사이트에 광고를 입찰합니다.

* *[!UICONTROL Content network]:* 사용되지 않음

## [!UICONTROL Budget Options]

<!-- **[!UICONTROL Bid]:** -->

{{$include /help/_includes/bid-ad-group.md}}

**[!UICONTROL Content Bid]:** 사용되지 않음

## [!UICONTROL Ad Group Targeting]

**[!UICONTROL Audience Target Method]:**(대상 광고 그룹):

* *[!UICONTROL Target and Bid]:* 광고 그룹의 다른 타겟도 충족하는 타겟 대상자와 연결된 사용자에게만 광고를 표시합니다.

* *[!UICONTROL Bid Only]:* 다른 광고 그룹 수준 타겟을 만족시키는 한 타겟 대상자와 연결되지 않은 사람에게도 광고를 표시합니다. 그러나 해당 대상에 대해 더 높은 입찰가를 설정하여 특정 대상에게 광고가 표시될 가능성을 높일 수 있습니다.

<!-- **[!UICONTROL Location Target]:** -->

{{$include /help/_includes/location-targets.md}}

대상 네트워크의 [!DNL Microsoft Advertising] 광고 그룹에 대해 위치 대상에 대한 입찰 수정자는 &quot;[!UICONTROL Auto-optimize Bid Adjustment Values]&quot; 설정이 있는 표준 포트폴리오에서 최적화되지 않습니다.

**[!UICONTROL Genre]:**([!UICONTROL Audience CTV Video] 캠페인의 광고 그룹, 미국, CA, BR, MX, 영국, DE, ES, FR, IT, AU, MY, TH에서 사용 가능<!-- Should that go in the campaign sub-type description instead, or is this applicable for this feature only? -->) 광고가 표시되는 프로그램 및 채널을 결정하는 타겟 장르:

* *[!UICONTROL All genres]:*(기본값) 모든 장르를 타깃팅합니다.

* *[!UICONTROL Select From Below List]:* 선택한 장르를 대상으로 합니다. 사용 가능한 모든 장르 목록에서 선택합니다.

연결된 TV(CTV) 광고 위치는 비디오 품질과 입찰 금액에 따라 다릅니다. [CTV 광고에 대한 기술 요구 사항](https://help.ads.microsoft.com/#apex/ads/en/60102/0/#TechnicalRequirements)을 참조하세요.

<!-- **[!UICONTROL Devices]:** -->

{{$include /help/_includes/devices.md}}

**[!UICONTROL Gender]:**(대상 광고 그룹, 선택 사항) 대상으로 포함하거나 제외할 특정 성별: *[!UICONTROL Male]*, *[!UICONTROL Female]* 및 *[!UICONTROL Unknown]*. 기본적으로 모든 성별이 타깃팅됩니다. 제외는 항상 포함을 무시합니다.

* 모든 값을 대상으로 지정하려면 값을 선택하지 마십시오.

* 값을 포함하려면 파란색 확인 표시(![포함](/help/search-social-commerce/assets/include.png "포함"))가 나타나도록 인접한 원을 한 번 클릭합니다. 선택적으로 타겟팅된 각 성별에 대해 지정된 백분율만큼 입찰을 늘리거나 줄일 수 있습니다.

* 값을 제외하려면 인접한 원을 두 번 클릭하여 빨간색 확인 표시(![Exclude](/help/search-social-commerce/assets/exclude.png "Exclude"))를 표시합니다.

**[!UICONTROL Age]:**(대상 광고 그룹, 선택 사항) 대상으로 포함하거나 제외할 특정 연령 범주: *[!UICONTROL 18-24]*, *[!UICONTROL 25-34]*, *[!UICONTROL 35-49]*, *[!UICONTROL 50-64]*, *[!UICONTROL 65+]* 및 *[!UICONTROL Unknown]*. 기본적으로 모든 연령이 타겟팅됩니다. 제외는 항상 포함을 무시합니다.

* 모든 값을 대상으로 지정하려면 값을 선택하지 마십시오.

* 값을 포함하려면 파란색 확인 표시(![포함](/help/search-social-commerce/assets/include.png "포함"))가 나타나도록 인접한 원을 한 번 클릭합니다. 타겟팅된 각 기간에 대해 지정된 퍼센트만큼 입찰가를 선택적으로 늘리거나 줄일 수 있습니다.

* 값을 제외하려면 인접한 원을 두 번 클릭하여 빨간색 확인 표시(![Exclude](/help/search-social-commerce/assets/exclude.png "Exclude"))를 표시합니다.

**[!UICONTROL Industry]:**(대상 광고 그룹, 선택 사항) 대상으로 포함하거나 제외할 특정 산업입니다. 기본적으로 모든 업종이 타깃팅됩니다. 제외는 항상 포함을 무시합니다.

* 모든 값을 대상으로 지정하려면 값을 선택하지 마십시오.

* 값을 포함하려면 파란색 확인 표시(![포함](/help/search-social-commerce/assets/include.png "포함"))가 나타나도록 인접한 원을 한 번 클릭합니다. 타겟팅된 각 산업에 대해 지정된 퍼센트만큼 입찰을 선택적으로 증가 또는 감소시킬 수 있습니다.

* 값을 제외하려면 인접한 원을 두 번 클릭하여 빨간색 확인 표시(![Exclude](/help/search-social-commerce/assets/exclude.png "Exclude"))를 표시합니다.

**[!UICONTROL Job Function Targets]:**(대상 광고 그룹, 선택 사항) 대상으로 포함하거나 제외할 특정 작업 함수입니다. 기본적으로 모든 작업 기능은 타깃팅됩니다. 제외는 항상 포함을 무시합니다.

* 모든 값을 대상으로 지정하려면 값을 선택하지 마십시오.

* 값을 포함하려면 파란색 확인 표시(![포함](/help/search-social-commerce/assets/include.png "포함"))가 나타나도록 인접한 원을 한 번 클릭합니다. 선택적으로 타겟팅된 각 작업 기능에 대해 지정된 퍼센트만큼 입찰을 늘리거나 줄일 수 있습니다.

* 값을 제외하려면 인접한 원을 두 번 클릭하여 빨간색 확인 표시(![Exclude](/help/search-social-commerce/assets/exclude.png "Exclude"))를 표시합니다.

## [!UICONTROL URL Options]

<!-- **[!UICONTROL Tracking Template]:** -->

{{$include /help/_includes/tracking-template-microsoft.md}}

<!-- **[!UICONTROL Custom Parameters]:** -->

{{$include /help/_includes/custom-parameters.md}}

**[!UICONTROL Adgroup Frequency Cap Settings]:**(선택 사항) 고객이 광고 그룹에서 광고를 받을 수 있는 횟수입니다. 값을 입력하고 시간 단위(*[!UICONTROL Hour]*, *[!UICONTROL Day]* 또는 *[!UICONTROL Week]*)를 선택하십시오.

## [!UICONTROL Negative Keywords]

<!-- **[!UICONTROL Negative Keywords]:** -->

{{$include /help/_includes/negative-keyword.md}}

<!-- Note for **[!UICONTROL Negative Keywords]:** -->

{{$include /help/_includes/negative-keyword-note-microsoft.md}}

## [!UICONTROL Negative Websites]

**[!UICONTROL Negative Websites]:**(디스플레이/기본 네트워크의 캠페인만 해당, 선택 사항) 광고를 표시하지 않으려는 디스플레이 네트워크의 사이트. 올바른 URL(예: www.example.com)을 입력하십시오. 여러 문자열을 지정하려면 쉼표로 구분하거나 별도의 줄에 입력합니다.

가용성에 대한 자세한 내용은 &quot;[특정 웹 사이트에 광고가 표시되지 않도록 하기](https://help.ads.microsoft.com/#apex/bae/en/14061/0)&quot;에 대한 [!DNL Microsoft Advertising] 도움말을 참조하십시오.

>[!MORELIKETHIS]
>
>* [광고 그룹 관리](/help/search-social-commerce/campaign-management/campaigns/ad-group-manage.md)
