---
title: 일괄 시트를 사용하여 배치 설정 검토 및 편집
description: 스프레드시트를 사용하여 주요 배치 설정을 대량으로 검토하고 편집하는 방법에 대해 알아봅니다.
feature: DSP Placements
exl-id: 2de4407d-eb3b-44ff-893c-9fdf6921d4b3
source-git-commit: 9d9330847c9356180928337a4a452f35e7024545
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# 일괄 시트를 사용하여 배치 설정 검토 및 편집

하나 이상의 배치 또는 캠페인의 모든 배치에 대한 설정을 XLSX([!DNL Microsoft Excel] 스프레드시트) 형식으로 다운로드하여 검토할 수 있습니다. 이 기능을 사용하여 다음과 같은 세부 사항을 신속하게 검토할 수 있습니다.

* 캠페인이 타겟팅하는 대상자입니다.
* 배치가 게재를 시작할 때와 중단될 때.
* 배치에 어떤 광고가 첨부됩니까?

여러 설정을 한 번에 업데이트하려면 필드를 선택하고, 파일을 저장하고, 편집된 일괄 시트 파일을 다시 DSP에 업로드하도록 변경할 수 있습니다. 편집 가능한 필드에는 가장 편집 가능한 설정이 포함됩니다.

>[!TIP]
>
>하나 이상의 배치에 대해 더 많은 필드를 빠르게 편집하려면 &quot;[배치 편집](/help/dsp/campaign-management/placements/placement-edit.md)&quot;을(를) 참조하십시오.

## 캠페인의 모든 배치에 대한 다운로드 설정

1. 주 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * 캠페인 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Download Bulksheet]**&#x200B;을(를) 클릭합니다.

   * 캠페인 이름을 클릭합니다. 오른쪽 상단에서 **[!UICONTROL ...]** > **[!UICONTROL Download Bulksheet]**&#x200B;을(를) 클릭합니다.

1. [!UICONTROL Bulksheet Download] 대화 상자에서 다운로드한 파일에서 설정을 제외할 캠페인 구성 요소의 선택을 취소한 다음 **[!UICONTROL Download]**&#x200B;을(를) 클릭합니다.

기본적으로 패키지와 연결된 모든 배치 및 광고에 대한 설정이 선택됩니다.

알림 메시지는 파일을 다운로드할 수 있는 시기를 나타냅니다.

1. 파일을 다운로드하려면 다음 중 하나를 수행합니다.

   * 알림 메시지에서 **[!UICONTROL Download].**&#x200B;을(를) 클릭합니다

   * 상단 메뉴 모음 오른쪽에서 ![작업](/help/dsp/assets/downloads.png)을 클릭합니다. 작업 옆에 있는 **[!UICONTROL Download]**&#x200B;을(를) 클릭합니다.

   파일이 브라우저의 다운로드 폴더에 저장됩니다.<!-- See "[Placement Columns in Downloaded/Uploaded Spreadsheets](#qa-sheet-columns)" for a list of the included columns. -->

## 특정 배치에 대한 다운로드 설정

1. 주 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 캠페인의 이름을 클릭합니다.

1. 하위 메뉴에서 **[!UICONTROL Placements]**&#x200B;을(를) 클릭합니다.

1. 설정을 다운로드할 각 배치 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL ...]** > **[!UICONTROL Download Bulksheet]**&#x200B;을(를) 클릭합니다.

   일괄 시트 파일을 다운로드할 수 있는 시기를 나타내는 알림 메시지가 표시됩니다.

1. 일괄 시트를 다운로드하려면 다음 중 하나를 수행하십시오.

   * 알림 메시지에서 **[!UICONTROL Download].**&#x200B;을(를) 클릭합니다

   * 상단 메뉴 모음 오른쪽에서 ![작업](/help/dsp/assets/downloads.png)을 클릭합니다. 작업 옆에 있는 **[!UICONTROL Download]**&#x200B;을(를) 클릭합니다.

   파일이 브라우저의 다운로드 폴더에 저장됩니다.<!-- See "[Placement Columns in Downloaded/Uploaded Spreadsheets](#qa-sheet-columns)" for a list of the included columns. -->

   설정을 편집하려면 파일을 직접 편집한 다음 변경 사항을 업로드하십시오.  편집 가능한 모든 열이 파란색으로 강조 표시됩니다. 필드에 올바른 형식을 사용하려면 해당 패키지 설정 또는 배치 설정에서 값을 선택하고 복사합니다. 데이터 분할, 사용자 정의 목표 및 전환 지표와 같은 일부 타겟 설정의 경우 설정 내에서 복사 옵션을 사용할 수 있습니다.

## 배치 설정이 있는 일괄 시트 업로드 {#upload-bulksheet-placement}

배치와 배치와 연관된 광고 및 패키지에 대한 설정을 Bulksheet 파일에 업로드할 수 있습니다.

1. 주 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * 상위 캠페인 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Upload Bulksheet]**&#x200B;을(를) 클릭합니다.

   * 캠페인 이름을 클릭합니다. 오른쪽 상단에서 **[!UICONTROL ...]** > **[!UICONTROL Upload Bulksheet]**&#x200B;을(를) 클릭합니다.

     이 옵션은 [!UICONTROL Packages], [!UICONTROL Placements] 또는 [!UICONTROL Ads] 탭에서 사용할 수 있습니다.

   * 하위 메뉴에서 **[!UICONTROL Placements]**&#x200B;을(를) 클릭하고 배치에 대한 확인란을 선택합니다. 일괄 작업 도구 모음에서 **[!UICONTROL ...]** > **[!UICONTROL Upload Bulksheet]**&#x200B;을(를) 클릭합니다.

1. [!UICONTROL Upload Bulksheet] 대화 상자에서:

   1. 파일을 상자로 끌어다 놓거나 상자 안을 클릭하여 장치나 네트워크에서 파일을 선택합니다.

   1. **[!UICONTROL Upload]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 업데이트가 처리되었는지 확인하려면 맨 위 메뉴 모음의 오른쪽에 있는 ![작업](/help/dsp/assets/downloads.png)을 클릭합니다.

설정 업데이트에 실패하면 색상 코딩이 있는 일괄 시트 오류 파일을 다운로드하여 저장된 설정(행)과 각 실패에 대한 이유를 표시할 수 있습니다. 그런 다음 동일한 파일 내에서 문제를 해결하고 다시 업로드하여 수정된 정보를 처리할 수 있습니다.

<!--
## Placement Setting Columns in Downloaded/Uploaded Bulksheets{#qa-sheet-columns}

>[!TIP]
>
> In a downloaded bulksheet, all editable columns are highlighted in blue.

### [!UICONTROL Placements] Sheet

| Section | Column | Description | Editable? |
|---------|--------|-------------|-----------|
| [!UICONTROL Basic] | [!UICONTROL Placement ID] | The numeric ID of the placement. | &mdash; |
| [!UICONTROL Basic] | [!UICONTROL Placement Name] | The name of the placement. | Yes |
| [!UICONTROL Basic] | [!UICONTROL Labels] | Any applied labels, for reporting. | &mdash; |
| [!UICONTROL Basic] | [!UICONTROL Edit Link] | A link to open the placement in Edit mode. | &mdash; |
| [!UICONTROL Basic] | [!UICONTROL Status] | The placement status: *[!UICONTROL active]* or *[!UICONTROL inactive]*. | Yes |
| [!UICONTROL Basic] | [!UICONTROL Placement Type] | The placement type. | &mdash; |
| [!UICONTROL Basic] | [!UICONTROL Package Name] | The name of the parent package, when applicable. | &mdash; |
| [!UICONTROL Goals] | [!UICONTROL Start Date] | The start date of the placement. | &mdash; |
| [!UICONTROL Goals] | [!UICONTROL End Date] | The end date of the placement. | &mdash; |
| [!UICONTROL Goals] | [!UICONTROL Day parting] | Whether dayparting is *[!UICONTROL ON]* or *[!UICONTROL OFF]*.<br><b>Note:</b> To check the actual dayparting schedule, open the placement settings in DSP. | &mdash; |
| [!UICONTROL Goals] | [!UICONTROL Budget] | The placement budget, if there is one. | Yes |
| [!UICONTROL Goals] | [!UICONTROL Budget Interval] | The budget interval: <i[!UICONTROL >Daily]*, *[!UICONTROL Weekly]*, *[!UICONTROL Monthly]*, or *[!UICONTROL All Time]*. | Yes |
| [!UICONTROL Goals] | [!UICONTROL Optimization Goal] | The objective of the package. | &mdash; |
| [!UICONTROL Goals] | [!UICONTROL Optimization Target] | The target value of the goal. | &mdash; |
| [!UICONTROL Goals] | [!UICONTROL Pace on] | Whether the placement is pacing towards the *[!UICONTROL Budget]* or *[!UICONTROL Impressions]*. | &mdash; |
| [!UICONTROL Goals] | [!UICONTROL Max Bid] | The maximum bid for the placement. | Yes |
| [!UICONTROL Goals] | [!UICONTROL Flight Pacing] | The flight pacing strategy for the placement: *[!UICONTROL Even]*, *[!UICONTROL slightly ahead]*, *[!UICONTROL frontload]*, or *[!UICONTROL aggressive frontload]*. | Yes |
| [!UICONTROL Goals] | [!UICONTROL Intraday Pacing] | The intraday pacing strategy for the placement: *[!UICONTROL Even]* or *[!UICONTROL ASAP]*. | Yes |
| [!UICONTROL Goals] | [!UICONTROL Pre-Bid Filters] | Any pre-bid filter criteria to be applied. | &mdash; |
| [!UICONTROL Goals] | [!UICONTROL Bidding Rules] | Whether bidding rules (deprecated) are *[!UICONTROL ON]* or *[!UICONTROL OFF]*. | &mdash; |
| [!UICONTROL Goals] | [!UICONTROL Frequency Cap] | The primary frequency cap for the placement during the specified [!UICONTROL Frequency Cap Interval]. | Yes |
| [!UICONTROL Goals] | [!UICONTROL Frequency Cap Interval] | The interval for the primary frequency cap: *[!UICONTROL Day]*, *[!UICONTROL Week]*, or *[!UICONTROL Month]*. | Yes |
| [!UICONTROL Goals] | [!UICONTROL Secondary Frequency Cap] | The secondary frequency cap for the placement during the specified [!UICONTROL Secondary Frequency Cap Interval] | Yes |
| [!UICONTROL Goals] | [!UICONTROL Secondary Frequency Cap Interval] | The type of interval for the secondary frequency cap: *[!UICONTROL Week]*, *[!UICONTROL Day]*, *[!UICONTROL Hour]*, or *[!UICONTROL Minute]*. The applicable number of weeks, days, hours, or minutes is indicated by the [!UICONTROL Secondary Frequency Cap Interval Value]. | Yes |
| [!UICONTROL Goals] | [!UICONTROL Secondary Frequency Cap Interval Value] | The number of weeks, days, hours, or minutes for which the [!UICONTROL Secondary Frequency Cap] applies. For example, if the secondary cap is three impressions per six hours, then the value here would be `6`. | Yes |
| [!UICONTROL Audience Location] | [!UICONTROL Audience Location - Included #] | The number of targeted geographical locations, *[!UICONTROL All]*, or *[!UICONTROL None]*. | &mdash; |
| [!UICONTROL Audience Location] | [!UICONTROL Audience Location - Included] | The targeted geographical locations, separated by semi-colons,or *[!UICONTROL All Locations]*. | &mdash; |
| [!UICONTROL Audience Location] | [!UICONTROL Audience Location - Excluded #] | The number of excluded geographical locations or *[!UICONTROL None]*. | &mdash; |
| [!UICONTROL Audience Location] | [!UICONTROL Audience Location - Excluded] | The excluded geographical locations, separated by semi-colons,  or *[!UICONTROL None]*. | &mdash; |
| [!UICONTROL Inventory] | [!UICONTROL Public Inventory - Included #] | The number of targeted public inventory deals, if any are specified, *[!UICONTROL All]*, or *[!UICONTROL None]*. | &mdash; |
| [!UICONTROL Inventory] | [!UICONTROL Public Inventory - Excluded #] | The number of excluded public inventory deals, if any are specified, or *[!UICONTROL None]*. | &mdash; |
| [!UICONTROL Inventory] | [!UICONTROL Private Inventory - Included #] | The number of targeted private inventory deals, if any are specified, *[!UICONTROL All]*, or *[!UICONTROL None]*. | &mdash; |
| [!UICONTROL Inventory] | [!UICONTROL Private Inventory - Excluded #] | The number of excluded private inventory deals, if any are specified, or *[!UICONTROL None]*. | &mdash; |
| [!UICONTROL Inventory] | [!UICONTROL On Demand Inventory - Included #] | The number of targeted [!UICONTROL On-Demand Inventory] deals, if any are specified, *[!UICONTROL All]*, or *[!UICONTROL None]*. | &mdash; |
| [!UICONTROL Inventory] | [!UICONTROL On Demand Inventory - Excluded #] | The number of excluded On-Demand Inventory deals, if any are specified, or *[!UICONTROL None]*. | &mdash; |
| [!UICONTROL Sites] | [!UICONTROL Traffic Type] | The targeted type of traffic: *[!UICONTROL Website]* and/or *[!UICONTROL Apps]* | &mdash; |
| [!UICONTROL Sites] | [!UICONTROL Site Tier] | The quality of the sites to target: *[!UICONTROL Tier 1]*, *[!UICONTROL Tier 2]*, *[!UICONTROL Tier 3]*, or *[!UICONTROL All Sites]*. | &mdash; |
| [!UICONTROL Sites] | [!UICONTROL Categories - Included #] | The number of targeted site categories, if any are specified, or *[!UICONTROL All]*. | &mdash; |
| [!UICONTROL Sites] | [!UICONTROL Categories - Excluded #] | The number of excluded site categories, if any are specified, or *[!UICONTROL All]*. | &mdash; |
| [!UICONTROL Sites] | [!UICONTROL Excluded Sites] | The excluded sites, if any are specified, or *[!UICONTROL None]*. | &mdash; |
| [!UICONTROL Sites] | [!UICONTROL Language] | The targeted site languages. | &mdash; |
| [!UICONTROL Sites] | [!UICONTROL Allow unscreened sites] | (Standard display placements only) Whether or not to allow ad delivery on non-audited sites: *[!UICONTROL ON]* or *[!UICONTROL OFF]*. When the placement targets private inventory, this option may deliver ads on blocked sites. | &mdash; |
| [!UICONTROL Sites] | [!UICONTROL Targeted Sites] | The number of targeted sites, if any are specified, or *[!UICONTROL None]*. | &mdash; |
| [!UICONTROL Audience Targeting] | [!UICONTROL Audience - Included] | The targeted audiences, if any are specified, or *[!UICONTROL None]*. | &mdash; |
| [!UICONTROL Audience Targeting] | [!UICONTROL Audience - Excluded] | The excluded audiences, if any are specified, or *[!UICONTROL None]*. | &mdash; |
| [!UICONTROL Audience Targeting] | [!UICONTROL Demographic booster] | Whether or not [!DNL Comscore] demographic segments are enabled for the placement (and other placements in the campaign): *[!UICONTROL ON]* or *[!UICONTROL OFF]*. This feature may be enabled only for campaigns for which the [!DNL Audience Verification] feature is enabled for [!DNL Nielsen] and/or [!DNL Comscore].  It incurs additional fees.  | &mdash; |
| [!UICONTROL Audience Targeting] | [!UICONTROL Extend across screens] | Whether or not to extend the ad targeting across devices: *[!UICONTROL ON]* or *[!UICONTROL OFF]*. Cross-device targeting extends your targeting across all of a person's known device, per the device graph specified in the campaign settings. | &mdash; |
| [!UICONTROL Audience Targeting] | [!UICONTROL Topic Targeting] - Included # | The number of targeted topic codes, if any are specified, or *[!UICONTROL All]*.   | &mdash; |
| [!UICONTROL Audience Targeting] | [!UICONTROL Topic Targeting - Excluded #] | The number of excluded topic codes, if any are specified, or *[!UICONTROL None]*. | &mdash; |
| [!UICONTROL Audience Targeting] | [!UICONTROL Device Targeting - Included #] | The number of targeted device targets, if any are specified, or *[!UICONTROL All]*. | &mdash; |
| [!UICONTROL Audience Targeting] | [!UICONTROL Device Targeting - Excluded #] | The number of excluded device targets, if any are specified, or *[!UICONTROL None]*. | &mdash; |
| [!UICONTROL Audience Targeting] | [!UICONTROL ISP Targeting - Included #] | The number of targeted ISP providers, if any are specified, or *[!UICONTROL All]/i>. | &mdash; |
| [!UICONTROL Audience Targeting] | [!UICONTROL ISP Targeting - Excluded #] | The number of excluded ISP providers, if any are specified, or *[!UICONTROL None]*. | &mdash; |
| [!UICONTROL Brand Safety] | [!UICONTROL Brand Safety - Contextual Filtering #] | The number of brand safety filters applied, if any are specified, or *[!UICONTROL None]*. | &mdash; |
| [!UICONTROL Brand Safety] | [!UICONTROL Brand Safety - Pre-Bid Fraud blocking #] | The number of pre-bid fraud blocking filters applied, if any are specified, or *[!UICONTROL None]*. | &mdash; |
| [!UICONTROL Brand Safety] | [!UICONTROL Brand Safety - Pre-Bid Viewability #] | The number of pre-bid viewability filters applied, if any are specified, or *[!UICONTROL None]*. | &mdash; |
| [!UICONTROL Brand Safety] | [!UICONTROL Site Safety Block] | Whether or not Site Safety Block is enabled: *[!UICONTROL ON]* or *[!UICONTROL OFF]*.[Whether or not the advertiser-level setting Enable Site Safety Block is enabled: *ON* or *OFF*.I don't see this option at the placement level. Should there be one?] | &mdash; |
| [!UICONTROL Tracking] | [!UICONTROL Tracking Pixels #] | The number of third-party  event-tracking pixels attached to the placement, or *[!UICONTROL None]*.| &mdash; |
| [!UICONTROL Tracking] | [!UICONTROL Conversion Pixels #] | The number of conversion tracking pixels attached to the placement, or *[!UICONTROL None]*. | &mdash; |
| [!UICONTROL Tracking] | [!UICONTROL 3rd-party fees] | A static, third-party fee rate to be tracked as a non-billable cost per 1000 impressions, if applicable. | &mdash; |
| [!UICONTROL Ads] | [!UICONTROL # of Ads Attached] | The number of ads attached to the placement, if any are attached, or *[!UICONTROL None]*. | &mdash; |
| [!UICONTROL Ads] | [!UICONTROL Ad Names] | The names of any ads attached to the placement, or *[!UICONTROL None]*. | &mdash; |
| [!UICONTROL Ads] | [!UICONTROL Attached Ad ID] | The unique DSP-generated Ad IDs of any ads attached to the placement, separated by semi-colons. To download a list of ad names and associated Ad IDs from the [!UICONTROL Ads] view, create a custom view that includes the [!UICONTROL Ad ID] metric, and then [export the data](/help/dsp/campaign-management/reports/campaign-export-data.md). | Yes |

### [!UICONTROL Placement_AdSchedules] Sheet

| [!UICONTROL Placement ID] | The numeric ID of the placement. | &mdash; |
| [!UICONTROL Placement Name] | The name of the placement. | &mdash; |
| [!UICONTROL Ad ID] | The numeric ID of the ad. | &mdash; |
| [!UICONTROL Ad Name] | The name of the ad. | Yes |
| [!UICONTROL Start Date] | The start date of the ad. | &mdash; |
| [!UICONTROL End Date] | The end date of the ad. | &mdash; |
| [!UICONTROL Adobe Ad Approval Status] | The status of the Advertising DSP approval process, such as *Approved* or *Incomplete*. | &mdash; |
| [!UICONTROL Flight 1 Start Date] - [!UICONTROL Flight 12 Start Date] | The start date for a specific flight. | Yes |
| [!UICONTROL Flight 1 End Date] - [!UICONTROL Flight 12 End Date] | The end date for a specific flight. | Yes |
| [!UICONTROL Flight 1 Weight] - [!UICONTROL Flight 12 Weight] | How to rotate a specific ad for a specific flight:  *Even* to rotate the ad evenly, or a relative weight by which to rotate the ad, as a percentage (such as `40` for 40%); the total weights for all ads in the flight must equal 100. | Yes |

### [!UICONTROL Placement_BidMultipliers] Sheet

*Available in campaign-level bulksheets only*

| Section | Column | Description | Editable? |
|---------|--------|-------------|-----------|
| [!UICONTROL Basic] | [!UICONTROL Placement ID] | The numeric ID of the placement. | &mdash; |
| [!UICONTROL Basic] | [!UICONTROL Placement Name] | The name of the placement. | &mdash; |
| [!UICONTROL Geo] | [!UICONTROL Country] | The bid multiplier and the name of the country, separated with a comma. Each target is followed by a semi-colon (;). | &mdash; |
| [!UICONTROL Geo] | [!UICONTROL State] | The bid multiplier and the name of the state. Each target is followed by a semi-colon (;). | &mdash; |
| [!UICONTROL Geo] | [!UICONTROL City] | The bid multiplier and the name of the city, separated with a comma. Each target is followed by a semi-colon (;). | &mdash; |
| [!UICONTROL Geo] | [!UICONTROL DMA] | (U.S. locations only) The bid multiplier and the designated market area, separated with a comma. Each target is followed by a semi-colon (;). | &mdash; |
| [!UICONTROL Geo] | [!UICONTROL Postal code] | The bid multiplier and the postal code, separated with a comma. Each target is followed by a semi-colon (;). | &mdash; |
| [!UICONTROL Inventory] | [!UICONTROL Public Inventory Source] | The bid multiplier and the public inventory source, separated with a comma. Each target is followed by a semi-colon (;). | &mdash; |
| [!UICONTROL Inventory] | [!UICONTROL Public Inventory Feed] | The bid multiplier and the public inventory feed, separated with a comma. Each target is followed by a semi-colon (;). | &mdash; |
| [!UICONTROL Inventory] | [!UICONTROL OnDemand Inventory Source] | The bid multiplier and the OnDemand inventory source, separated with a comma. Each target is followed by a semi-colon (;). | &mdash; |
| [!UICONTROL Inventory] | [!UICONTROL OnDemand Inventory Feed] | The bid multiplier and the OnDemand inventory feed, separated with a comma. Each target is followed by a semi-colon (;). | &mdash; |
| [!UICONTROL Sites/Apps] | [!UICONTROL Domains] | The bid multiplier and the domains, separated with a comma. Each target is followed by a semi-colon (;). | &mdash; |
| [!UICONTROL Sites/Apps] | [!UICONTROL Category] | The bid multiplier and the site/app category, separated with a comma. Each target is followed by a semi-colon (;). | &mdash; |
| [!UICONTROL Audience] | [!UICONTROL Daypart] | The bid multiplier and the daypart interval, separated with a comma. Each target is followed by a semi-colon (;). | &mdash; |
| [!UICONTROL Audience] | [!UICONTROL Topics - Comscore] | The bid multiplier and the [!DNL Comscore] topics, separated with a comma. Each target is followed by a semi-colon (;). | &mdash; |
| [!UICONTROL Brand Safety] | [!UICONTROL Ads.txt] | The bid multiplier and the level of [Ads.txt](https://iabtechlab.com/ads-txt-about/) pre-bid filtering to use, separated with a comma. Each target is followed by a semi-colon (;). | &mdash; |

-->

<!-- LOTS MORE THAN I HAD ORIGINALLY DOCUMENTED -- BELOW ARE THE LAST, BUT NOT ALL:

| Brand Safety | Brand Safety - Contextual Filtering # |  |  |
| Brand Safety | Brand Safety - Pre-Bid Fraud blocking # |  |  |
| Brand Safety | Brand Safety - Pre-Bid Viewability # |  |  |
| Brand Safety | Site Safety Block |  |  |
| Tracking | Tracking Pixels # |  |  |
| Tracking | Conversion Pixels # |  |  |
| Tracking | 3rd-party fees |  |  |
| # of Ads Attached |  |  |
| Ads |  Ad Names |  |  |
| Ads | Attached Ad ID |  |  |
| Environment | Environment |  |  |
-->

<!-- 
Check on Brand Safety - Contextual Filtering # with new DV feature/fct change.
-->

>[!MORELIKETHIS]
>
>* [일괄 시트를 사용하여 캠페인 구성 요소 설정 검토 및 편집](/help/dsp/campaign-management/campaign-components-review-edit.md)
>* [배치 편집](/help/dsp/campaign-management/placements/placement-edit.md)
>* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)
