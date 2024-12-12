---
title: 일괄 시트를 사용하여 배치 설정 검토 및 편집
description: 스프레드시트를 사용하여 주요 배치 설정을 대량으로 검토하고 편집하는 방법에 대해 알아봅니다.
feature: DSP Placements
exl-id: 2de4407d-eb3b-44ff-893c-9fdf6921d4b3
source-git-commit: 8f4e694885919a8dcf7895c2f8d8aeb11249e03c
workflow-type: tm+mt
source-wordcount: '1457'
ht-degree: 0%

---

# 일괄 시트를 사용하여 배치 설정 검토 및 편집

하나 이상의 배치 또는 캠페인의 모든 배치에 대한 설정을 XLSX([!DNL Microsoft Excel] 스프레드시트) 형식으로 다운로드하여 검토할 수 있습니다. 이 기능을 사용하여 다음과 같은 세부 사항을 신속하게 검토할 수 있습니다.

* 캠페인이 타겟팅하는 대상자입니다.
* 배치가 게재를 시작할 때와 중단될 때.
* 배치에 어떤 광고가 첨부됩니까?

여러 설정을 한 번에 업데이트하려면 다음 중 하나를 수행할 수 있습니다.

* 필드를 선택하고, 파일을 저장하고, 편집된 일괄 시트 파일을 다시 DSP에 업로드하도록 변경합니다.

* 추가 배치 및 모든 패키지의 설정을 변경하려면 각 캠페인 구성 요소 유형에 대한 탭이 포함된 빈 일괄 시트 템플릿을 다운로드하고 템플릿 파일에 새 설정이나 업데이트된 설정을 입력하거나 붙여 넣은 다음 파일을 업로드하여 변경합니다. 지침은 &quot;[일괄 시트를 사용하여 캠페인 구성 요소 설정 검토 및 편집](/help/dsp/campaign-management/campaign-components-review-edit.md)&quot;을 참조하십시오.

편집 가능한 필드에는 배치 이름, 상태, 입찰, 예산, 게재 간격 전략 및 빈도 상한이 포함됩니다.

>[!TIP]
>
>하나 이상의 배치에 대해 더 많은 필드를 빠르게 편집하려면 &quot;[배치 편집](/help/dsp/campaign-management/placements/placement-edit.md)&quot;을(를) 참조하십시오.

## 캠페인의 모든 배치에 대한 다운로드 설정

1. 주 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 오른쪽 상단에서 **[!UICONTROL ...]** > **[!UICONTROL Download Setup Excel]**&#x200B;을(를) 클릭합니다.

   알림 메시지는 파일을 다운로드할 수 있는 시기를 나타냅니다.

1. 파일을 다운로드하려면 다음 중 하나를 수행합니다.

   * 알림 메시지에서 **[!UICONTROL Download].**&#x200B;을(를) 클릭합니다

   * 상단 메뉴 모음 오른쪽에서 ![작업](/help/dsp/assets/downloads.png)을 클릭합니다. 작업 옆에 있는 **[!UICONTROL Download]**&#x200B;을(를) 클릭합니다.

   파일은 브라우저의 다운로드 폴더에 저장됩니다. 포함된 열의 목록은 &quot;[다운로드한/업로드한 스프레드시트의 배치 열](#qa-sheet-columns)&quot;을 참조하십시오.

## 하나 이상의 배치에 대한 다운로드 설정

1. 주 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 캠페인의 이름을 클릭합니다.

1. 하위 메뉴에서 **[!UICONTROL Placements]**&#x200B;을(를) 클릭합니다.

1. 설정을 다운로드할 각 배치 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL ...]** > **[!UICONTROL Download Bulksheet]**&#x200B;을(를) 클릭합니다.

   일괄 시트 파일을 다운로드할 수 있는 시기를 나타내는 알림 메시지가 표시됩니다.

1. 일괄 시트를 다운로드하려면 다음 중 하나를 수행하십시오.

   * 알림 메시지에서 **[!UICONTROL Download].**&#x200B;을(를) 클릭합니다

   * 상단 메뉴 모음 오른쪽에서 ![작업](/help/dsp/assets/downloads.png)을 클릭합니다. 작업 옆에 있는 **[!UICONTROL Download]**&#x200B;을(를) 클릭합니다.

   파일은 브라우저의 다운로드 폴더에 저장됩니다. 포함된 열의 목록은 &quot;[다운로드한/업로드한 스프레드시트의 배치 열](#qa-sheet-columns)&quot;을 참조하십시오.


<!-- I don't think I need this here

## Download a Bulksheet Template {#download-template}

Download a blank bulksheet template that includes tabs for each type of campaign component. You can later add rows to any tab on the template and [upload the edited file](##upload-bulksheet-package) to make changes. 

1. Click the name of the campaign.

1.  In the upper right, click **[!UICONTROL ...]** > **[!UICONTROL Download Bulksheet]**.

   The file is saved to the browser's Downloads folder. See "[Placement Columns in Downloaded/Uploaded Spreadsheets](#qa-sheet-columns)" for a list of the included columns.

-->

## 배치 설정이 있는 일괄 시트 업로드 {#upload-bulksheet-placement}

배치와 배치와 연관된 광고 및 패키지에 대한 설정을 Bulksheet 파일에 업로드할 수 있습니다.

1. 주 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 캠페인의 이름을 클릭합니다.

1. 오른쪽 상단에서 **[!UICONTROL ...]** > **[!UICONTROL Upload Bulksheet]**&#x200B;을(를) 클릭합니다.

1. [!UICONTROL Upload Bulksheet] 대화 상자에서:

   1. 파일을 상자로 끌어다 놓거나 상자 안을 클릭하여 장치나 네트워크에서 파일을 선택합니다.

   1. **[!UICONTROL Upload]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 업데이트가 처리되었는지 확인하려면 맨 위 메뉴 모음의 오른쪽에 있는 ![작업](/help/dsp/assets/downloads.png)을 클릭합니다.

## 다운로드/업로드한 스프레드시트의 배치 설정 열{#qa-sheet-columns}

>[!TIP]
>
> 다운로드한 스프레드시트에서 편집 가능한 모든 열이 파란색으로 강조 표시됩니다.

### 캠페인 수준 스프레드시트

<!-- 
Check on Brand Safety - Contextual Filtering # with new DV feature/fct change.
-->

| 섹션 | 열 | 설명 | 편집 가능합니까? |
|---------|--------|-------------|-----------|
| [!UICONTROL Basic] | [!UICONTROL Placement ID] | 배치의 숫자 ID입니다. | — |
| [!UICONTROL Basic] | [!UICONTROL Placement Name] | 배치의 이름입니다. | 예 |
| [!UICONTROL Basic] | [!UICONTROL Labels] | 보고를 위해 적용된 모든 레이블. | — |
| [!UICONTROL Basic] | [!UICONTROL Edit Link] | 편집 모드에서 배치를 여는 링크입니다. | — |
| [!UICONTROL Basic] | [!UICONTROL Status] | 배치 상태: *[!UICONTROL active]* 또는 *[!UICONTROL inactive]*. | 예 |
| [!UICONTROL Basic] | [!UICONTROL Placement Type] | 배치 유형. | — |
| [!UICONTROL Basic] | [!UICONTROL Package Name] | 해당되는 경우 상위 패키지의 이름입니다. | — |
| [!UICONTROL Goals] | [!UICONTROL Start Date] | 배치의 시작 날짜입니다. | — |
| [!UICONTROL Goals] | [!UICONTROL End Date] | 배치의 종료 날짜입니다. | — |
| [!UICONTROL Goals] | [!UICONTROL Day parting] | dayparting이 *[!UICONTROL ON]*&#x200B;인지 *[!UICONTROL OFF]*&#x200B;인지 여부.<br><b>참고:</b> 실제 날짜 분할 일정을 확인하려면 DSP에서 배치 설정을 여십시오. | — |
| [!UICONTROL Goals] | [!UICONTROL Budget] | 배치 예산(있는 경우). | 예 |
| [!UICONTROL Goals] | [!UICONTROL Budget Interval] | 예산 간격: &lt;i[!UICONTROL >Daily]*, *[!UICONTROL Weekly]*, *[!UICONTROL Monthly]* 또는 *[!UICONTROL All Time]*. | 예 |
| [!UICONTROL Goals] | [!UICONTROL Optimization Goal] | 패키지의 목적입니다. | — |
| [!UICONTROL Goals] | [!UICONTROL Optimization Target] | 목표의 타겟 값입니다. | — |
| [!UICONTROL Goals] | [!UICONTROL Pace on] | 배치가 *[!UICONTROL Budget]* 또는 *[!UICONTROL Impressions]* 방향으로 진행되는지 여부입니다. | — |
| [!UICONTROL Goals] | [!UICONTROL Max Bid] | 배치에 대한 최대 입찰가. | 예 |
| [!UICONTROL Goals] | [!UICONTROL Flight Pacing] | 배치에 대한 플라이트 게재 간격 전략: *[!UICONTROL Even]*, *[!UICONTROL slightly ahead]*, *[!UICONTROL frontload]* 또는 *[!UICONTROL aggressive frontload]*. | 예 |
| [!UICONTROL Goals] | [!UICONTROL Intraday Pacing] | 배치에 대한 일일 간격 전략: *[!UICONTROL Even]* 또는 *[!UICONTROL ASAP]*. | 예 |
| [!UICONTROL Goals] | [!UICONTROL Pre-Bid Filters] | 적용할 모든 사전 입찰 필터 기준. | — |
| [!UICONTROL Goals] | [!UICONTROL Bidding Rules] | 입찰 규칙(더 이상 사용되지 않음)이 *[!UICONTROL ON]*&#x200B;인지 *[!UICONTROL OFF]*&#x200B;인지 여부. | — |
| [!UICONTROL Goals] | [!UICONTROL Frequency Cap] | 지정한 [!UICONTROL Frequency Cap Interval] 동안 배치에 대한 기본 빈도 제한입니다. | 예 |
| [!UICONTROL Goals] | [!UICONTROL Frequency Cap Interval] | 기본 빈도 제한 간격: *[!UICONTROL Day]*, *[!UICONTROL Week]* 또는 *[!UICONTROL Month]*. | 예 |
| [!UICONTROL Goals] | [!UICONTROL Secondary Frequency Cap] | 지정한 [!UICONTROL Secondary Frequency Cap Interval] 동안 배치에 대한 보조 빈도 제한 | 예 |
| [!UICONTROL Goals] | [!UICONTROL Secondary Frequency Cap Interval] | 보조 빈도 제한 간격 유형: *[!UICONTROL Week]*, *[!UICONTROL Day]*, *[!UICONTROL Hour]* 또는 *[!UICONTROL Minute]*. 적용 가능한 주, 일, 시간 또는 분 수는 [!UICONTROL Secondary Frequency Cap Interval Value]에 표시됩니다. | 예 |
| [!UICONTROL Goals] | [!UICONTROL Secondary Frequency Cap Interval Value] | [!UICONTROL Secondary Frequency Cap]이(가) 적용되는 주, 일, 시간 또는 분 수입니다. 예를 들어 보조 캡이 6시간당 세 개의 노출 횟수이면 여기에 있는 값은 `6`입니다. | 예 |
| [!UICONTROL Audience Location] | [!UICONTROL Audience Location - Included #] | 타깃팅된 지리적 위치 수 *[!UICONTROL All]* 또는 *[!UICONTROL None]*&#x200B;입니다. | — |
| [!UICONTROL Audience Location] | [!UICONTROL Audience Location - Included] | 세미콜론으로 구분된 대상 지리적 위치 또는 *[!UICONTROL All Locations]*&#x200B;입니다. | — |
| [!UICONTROL Audience Location] | [!UICONTROL Audience Location - Excluded #] | 제외된 지리적 위치 또는 *[!UICONTROL None]*&#x200B;의 수입니다. | — |
| [!UICONTROL Audience Location] | [!UICONTROL Audience Location - Excluded] | 세미콜론 또는 *[!UICONTROL None]*(으)로 구분된 제외된 지리적 위치입니다. | — |
| [!UICONTROL Inventory] | [!UICONTROL Public Inventory - Included #] | 대상 공개 인벤토리 거래 수(지정된 경우), *[!UICONTROL All]* 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Inventory] | [!UICONTROL Public Inventory - Excluded #] | 제외된 공개 인벤토리 거래 수(지정된 경우) 또는 *[!UICONTROL None]*&#x200B;입니다. | — |
| [!UICONTROL Inventory] | [!UICONTROL Private Inventory - Included #] | 지정된 경우 타깃팅된 개인 인벤토리 거래 수, *[!UICONTROL All]* 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Inventory] | [!UICONTROL Private Inventory - Excluded #] | 제외된 개인 인벤토리 거래 수(지정된 경우) 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Inventory] | [!UICONTROL On Demand Inventory - Included #] | 타겟팅된 [!UICONTROL On-Demand Inventory]개 거래 수(지정된 경우), *[!UICONTROL All]* 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Inventory] | [!UICONTROL On Demand Inventory - Excluded #] | 제외된 온디맨드 인벤토리 거래 수(지정된 경우) 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Sites] | [!UICONTROL Traffic Type] | 대상 트래픽 유형: *[!UICONTROL Website]* 및/또는 *[!UICONTROL Apps]* | — |
| [!UICONTROL Sites] | [!UICONTROL Exclude out-stream] | 아웃스트림 트래픽을 제외하는 인벤토리 타기팅 옵션이 &lt;i[!UICONTROL >ON]*인지 *[!UICONTROL OFF]*&#x200B;인지 여부.<br>외부 스트리밍 광고는 대개 비디오 플레이어에서 일반 비디오 광고가 아니라 콘텐츠 위에 팝업이나 콘텐츠로 채워집니다(기본 환경에서). | — |
| [!UICONTROL Sites] | [!UICONTROL Site Tier] | 타깃팅할 사이트 품질: *[!UICONTROL Tier 1]*, *[!UICONTROL Tier 2]*, *[!UICONTROL Tier 3]* 또는 *[!UICONTROL All Sites]*. | — |
| [!UICONTROL Sites] | [!UICONTROL Categories - Included #] | 타겟팅된 사이트 범주의 수(지정된 경우) 또는 *[!UICONTROL All]*&#x200B;입니다. | — |
| [!UICONTROL Sites] | [!UICONTROL Categories - Excluded #] | 제외된 사이트 범주의 수(지정된 경우) 또는 *[!UICONTROL All]*&#x200B;입니다. | — |
| [!UICONTROL Sites] | [!UICONTROL Excluded Sites] | 제외된 사이트(지정된 경우) 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Sites] | [!UICONTROL Language] | 타겟팅된 사이트 언어입니다. | — |
| [!UICONTROL Sites] | [!UICONTROL Allow unscreened sites] | (표준 디스플레이 배치만 해당) 감사되지 않은 사이트(*[!UICONTROL ON]* 또는 *[!UICONTROL OFF]*)에서 광고 게재를 허용할지 여부입니다. 배치가 개인 인벤토리를 타겟팅하면 이 옵션은 차단된 사이트에 광고를 게재할 수 있습니다. | — |
| [!UICONTROL Sites] | [!UICONTROL Targeted Sites] | 타겟팅된 사이트의 수(지정된 경우) 또는 *[!UICONTROL None]*&#x200B;입니다. | — |
| [!UICONTROL Audience Targeting] | [!UICONTROL Audience - Included] | 타깃팅된 대상(지정된 경우) 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Audience Targeting] | [!UICONTROL Audience - Excluded] | 제외된 대상자(지정된 경우) 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Audience Targeting] | [!UICONTROL Demographic booster] | 배치(및 캠페인의 다른 배치)에 대해 [!DNL Comscore] 인구 통계학적 세그먼트를 사용할지 여부: *[!UICONTROL ON]* 또는 *[!UICONTROL OFF]*. 이 기능은 [!DNL Nielsen] 및/또는 [!DNL Comscore]에 대해 [!DNL Audience Verification] 기능이 활성화된 캠페인에만 사용할 수 있습니다.  추가 비용이 발생합니다. | — |
| [!UICONTROL Audience Targeting] | [!UICONTROL Extend across screens] | 장치 간에 광고 타깃팅을 확장할지 여부: *[!UICONTROL ON]* 또는 *[!UICONTROL OFF]*. 크로스 디바이스 타깃팅은 캠페인 설정에 지정된 디바이스 그래프에 따라 개인의 알려진 모든 디바이스에서 타깃팅을 확장합니다. | — |
| [!UICONTROL Audience Targeting] | [!UICONTROL Topic Targeting] - 포함 # | 대상 항목 코드(지정된 경우) 또는 *[!UICONTROL All]*&#x200B;의 수입니다. | — |
| [!UICONTROL Audience Targeting] | [!UICONTROL Topic Targeting - Excluded #] | 제외된 항목 코드(지정된 경우) 또는 *[!UICONTROL None]*&#x200B;의 수입니다. | — |
| [!UICONTROL Audience Targeting] | [!UICONTROL Device Targeting - Included #] | 대상 장치 대상 수(지정된 경우) 또는 *[!UICONTROL All]*&#x200B;입니다. | — |
| [!UICONTROL Audience Targeting] | [!UICONTROL Device Targeting - Excluded #] | 제외된 장치 대상 수(지정된 경우) 또는 *[!UICONTROL None]*&#x200B;입니다. | — |
| [!UICONTROL Audience Targeting] | [!UICONTROL ISP Targeting - Included #] | 타겟팅된 ISP 공급자 수(지정된 경우) 또는 *[!UICONTROL All]/i>. | — |
| [!UICONTROL Audience Targeting] | [!UICONTROL ISP Targeting - Excluded #] | 제외된 ISP 공급자 수(지정된 경우) 또는 *[!UICONTROL None]*&#x200B;입니다. | — |
| [!UICONTROL Brand Safety] | [!UICONTROL Brand Safety - Contextual Filtering #] | 적용된 브랜드 안전 필터의 수(지정된 경우) 또는 *[!UICONTROL None]*&#x200B;입니다. | — |
| [!UICONTROL Brand Safety] | [!UICONTROL Brand Safety - Pre-Bid Fraud blocking #] | 적용된 사전 입찰 사기 차단 필터의 수(지정된 경우) 또는 *[!UICONTROL None]*&#x200B;입니다. | — |
| [!UICONTROL Brand Safety] | [!UICONTROL Brand Safety - Pre-Bid Viewability #] | 적용된 사전 입찰 가시성 필터 수(지정된 경우) 또는 *[!UICONTROL None]*&#x200B;입니다. | — |
| [!UICONTROL Brand Safety] | [!UICONTROL Site Safety Block] | 사이트 안전 차단 사용 여부: *[!UICONTROL ON]* 또는 *[!UICONTROL OFF]*.<!-- Whether or not the advertiser-level setting Enable Site Safety Block is enabled: *ON* or *OFF*.I don’t see this option at the placement level. Should there be one? --> | — |
| [!UICONTROL Tracking] | [!UICONTROL Tracking Pixels #] | 배치에 연결된 타사 이벤트 추적 픽셀 수 또는 *[!UICONTROL None]*&#x200B;입니다. | — |
| [!UICONTROL Tracking] | [!UICONTROL Conversion Pixels #] | 배치에 연결된 전환 추적 픽셀 수 또는 *[!UICONTROL None]*&#x200B;입니다. | — |
| [!UICONTROL Tracking] | [!UICONTROL 3rd-party fees] | 1000회 노출당 청구 불가능한 비용으로 추적할 정적 타사 수수료 비율(해당하는 경우). | — |
| [!UICONTROL Ads] | [!UICONTROL # of Ads Attached] | 배치에 첨부된 광고 수(있는 경우) 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Ads] | [!UICONTROL Ad Names] | 배치에 첨부된 광고의 이름 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Ads] | [!UICONTROL Attached Ad ID] | 배치에 첨부된 고유 DSP 생성 광고 ID로, 세미콜론으로 구분됩니다. [!UICONTROL Ads] 보기에서 광고 이름 및 관련 광고 ID 목록을 다운로드하려면 [!UICONTROL Ad ID] 지표를 포함하는 사용자 지정 보기를 만든 다음 [데이터를 내보냅니다](/help/dsp/campaign-management/reports/campaign-export-data.md). | 예 |

### 배치 레벨 일괄 시트

| 열 | 설명 | 편집 가능합니까? |
|--------|-------------|-----------|
| [!UICONTROL Placement ID] | 배치의 숫자 ID입니다. | — |
| [!UICONTROL Placement Name] | 배치의 이름입니다. | 예 |
| [!UICONTROL Package Name] | 해당되는 경우 상위 패키지의 이름입니다. | — |
| [!UICONTROL Start Date] | 배치의 시작 날짜입니다. | — |
| [!UICONTROL End Date] | 배치의 종료 날짜입니다. | — |
| [!UICONTROL Status] | 배치 상태: *[!UICONTROL active]* 또는 *[!UICONTROL inactive]*. | — |
| [!UICONTROL Max Bid] | 배치에 대한 최대 입찰가. | 예 |
| [!UICONTROL Budget] | 배치 예산(있는 경우). | 예 |
| [!UICONTROL Budget Interval] | 예산 간격: &lt;i[!UICONTROL >Daily]*, *[!UICONTROL Weekly]*, *[!UICONTROL Monthly]* 또는 *[!UICONTROL All Time]*. | 예 |
| [!UICONTROL Primary Frequency Cap] | 지정한 [!UICONTROL Primary Frequency Cap Interval] 동안 배치에 대한 기본 빈도 제한입니다. | 예 |
| [!UICONTROL Primary Frequency Cap Interval] | 기본 빈도 제한 간격: *[!UICONTROL Day]*, *[!UICONTROL Week]* 또는 *[!UICONTROL Month]*. | 예 |
| [!UICONTROL Secondary Frequency Cap] | 지정한 [!UICONTROL Secondary Frequency Cap Interval] 동안 배치에 대한 보조 빈도 제한 | 예 |
| [!UICONTROL Secondary Frequency Cap Interval] | 보조 빈도 제한 간격 유형: *[!UICONTROL Week]*, *[!UICONTROL Day]*, *[!UICONTROL Hour]* 또는 *[!UICONTROL Minute]*. 적용 가능한 주, 일, 시간 또는 분 수는 [!UICONTROL Secondary Frequency Cap Interval Value]에 표시됩니다. | 예 |
| [!UICONTROL Secondary Frequency Cap Interval Value] | [!UICONTROL Secondary Frequency Cap]이(가) 적용되는 주, 일, 시간 또는 분 수입니다. 예를 들어 보조 캡이 6시간당 세 개의 노출 횟수이면 여기에 있는 값은 `6`입니다. | 예 |
| [!UICONTROL Attached Ad ID] | 배치에 첨부된 고유 DSP 생성 광고 ID로, 세미콜론으로 구분됩니다. [!UICONTROL Ads] 보기에서 광고 이름 및 관련 광고 ID 목록을 다운로드하려면 [!UICONTROL Ad ID] 지표를 포함하는 사용자 지정 보기를 만든 다음 [데이터를 내보냅니다](/help/dsp/campaign-management/reports/campaign-export-data.md). | 예 |


<!-- LOTS MORE THAN I HAD ORIGINALLY DOCUMENTED -- BELOW ARE THE LAST, BUT NOT ALL:

Brand Safety - Contextual Filtering #								"		

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


>[!MORELIKETHIS]
>
>* [일괄 시트를 사용하여 캠페인 구성 요소 설정 검토 및 편집](/help/dsp/campaign-management/campaign-components-review-edit.md)
>* [배치 편집](/help/dsp/campaign-management/placements/placement-edit.md)
>* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)
