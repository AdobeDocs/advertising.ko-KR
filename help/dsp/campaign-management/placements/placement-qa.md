---
title: 스프레드시트를 사용하여 배치 설정 검토 및 수정
description: 스프레드시트를 사용하여 주요 배치 설정을 검토하고 편집하는 방법에 대해 알아봅니다.
feature: DSP Placements
exl-id: 2de4407d-eb3b-44ff-893c-9fdf6921d4b3
source-git-commit: f352af0ffd5bfeab08f6592b4f3af56a9668feaa
workflow-type: tm+mt
source-wordcount: '1435'
ht-degree: 0%

---

# 스프레드시트를 사용하여 배치 설정 검토 및 수정

하나 이상의 배치 또는 캠페인의 모든 배치에 대한 설정을 XLSX(Excel 스프레드시트) 형식으로 다운로드하여 검토할 수 있습니다. 이 기능을 사용하여 다음과 같은 세부 사항을 신속하게 검토할 수 있습니다.

* 캠페인이 타겟팅하는 대상자입니다.
* 배치가 게재를 시작하는 시점과 중단되는 시점.
* 배치에 어떤 광고가 첨부됩니까?

그런 다음 변경 작업을 수행하여 필드를 선택하고 한 번에 모두 DSP에 다시 업로드할 수 있습니다. 편집 가능한 필드에는 배치 이름, 상태, 입찰, 예산, 게재 간격 전략 및 빈도 상한이 포함됩니다.

>[!TIP]
>
>배치 설정을 보다 광범위하게 변경하려면 [벌크 편집 기능](/help/dsp/campaign-management/placements/placement-edit.md).

## 캠페인의 모든 배치에 대한 다운로드 설정

1. 메인 메뉴에서 **[!UICONTROL Campaigns]**.

1. 다음 중 하나를 수행합니다.

   * 캠페인 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Download Excel QA sheet]**.

   * 캠페인 세부 사항을 보려면 캠페인 이름을 클릭합니다. 오른쪽 상단에서 **[!UICONTROL ...]** > **[!UICONTROL Download Excel QA sheet]**.

   알림 메시지는 파일을 다운로드할 수 있는 시기를 나타냅니다.

1. 다음 중 하나를 수행합니다.

   * 알림 메시지에서 다음을 클릭합니다. **[!UICONTROL Download].**

   * 상단 메뉴 모음의 오른쪽에서 ![작업](/help/dsp/assets/downloads.png). 클릭 **[!UICONTROL Download]** 작업 옆에 있습니다.

   파일은 브라우저의 다운로드 폴더에 저장됩니다. 를 참조하십시오.[다운로드/업로드된 스프레드시트의 열](#qa-sheet-columns)포함된 열의 목록은 &quot;을 참조하십시오.

## 하나 이상의 배치에 대한 다운로드 설정

1. 메인 메뉴에서 **[!UICONTROL Campaigns]**.

1. 캠페인의 이름을 클릭합니다.

1. 하위 메뉴에서 **[!UICONTROL Placements]**.

1. 설정을 다운로드할 각 배치 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 를 클릭합니다 **[!UICONTROL ...]** > **[!UICONTROL Download Edit in Excel Sheet]**.

파일은 브라우저의 다운로드 폴더에 자동으로 저장됩니다. 를 참조하십시오.[다운로드/업로드된 스프레드시트의 열](#qa-sheet-columns)포함된 열의 목록은 &quot;을 참조하십시오.

## 캠페인의 모든 배치에 대한 설정 업로드

1. 메인 메뉴에서 **[!UICONTROL Campaigns]**.

1. 다음 중 하나를 수행합니다.

   * 캠페인 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Upload Excel QA sheet]**.

   * 캠페인 세부 사항을 보려면 캠페인 이름을 클릭합니다. 오른쪽 상단에서 **[!UICONTROL ...]** > **[!UICONTROL Upload Excel QA sheet]**.

1. 다음에서 [!UICONTROL Edit in Excel] 대화 상자:

   1. 파일을 상자로 끌어다 놓거나 상자 안을 클릭하여 장치나 네트워크에서 파일을 선택합니다.

   1. 클릭 **[!UICONTROL Upload]**.

1. (선택 사항) 업데이트가 처리되었는지 확인하려면 ![작업](/help/dsp/assets/downloads.png) 을 클릭합니다.

## 하나 이상의 배치에 대한 설정 업로드

1. 메인 메뉴에서 **[!UICONTROL Campaigns]**.

1. 캠페인의 이름을 클릭합니다.

1. 하위 메뉴에서 **[!UICONTROL Placements]**.

1. 설정을 업로드할 각 배치 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 를 클릭합니다 **[!UICONTROL ...]** > **[!UICONTROL Upload Edit in Excel Sheet]**.

1. 다음에서 [!UICONTROL Edit in Excel] 대화 상자:

   1. 파일을 상자로 끌어다 놓거나 상자 안을 클릭하여 장치나 네트워크에서 파일을 선택합니다.

   1. 클릭 **[!UICONTROL Upload]**.

1. (선택 사항) 업데이트가 처리되었는지 확인하려면 ![작업](/help/dsp/assets/downloads.png) 을 클릭합니다.

## 다운로드/업로드한 스프레드시트의 배치 설정 열{#qa-sheet-columns}

>[!TIP]
>
> 다운로드한 스프레드시트에서 편집 가능한 모든 열이 파란색으로 강조 표시됩니다.

### 캠페인 수준 스프레드시트

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
| [!UICONTROL Goals] | [!UICONTROL Day parting] | Dayparting이 *[!UICONTROL ON]* 또는 *[!UICONTROL OFF]*.<br><b>참고:</b> 실제 날짜 분할 일정을 확인하려면 DSP에서 배치 설정을 엽니다. | — |
| [!UICONTROL Goals] | [!UICONTROL Budget] | 배치 예산(있는 경우). | 예 |
| [!UICONTROL Goals] | [!UICONTROL Budget Interval] | 예산 간격: &lt;i span=&quot;&quot; id=&quot;0&quot; translate=&quot;no&quot; />*, *[!UICONTROL Weekly]*, *[!UICONTROL Monthly]*, 또는 *[!UICONTROL All Time]*.[!UICONTROL >Daily] | 예 |
| [!UICONTROL Goals] | [!UICONTROL Optimization Goal] | 패키지의 목적입니다. | — |
| [!UICONTROL Goals] | [!UICONTROL Optimization Target] | 목표의 타겟 값입니다. | — |
| [!UICONTROL Goals] | [!UICONTROL Pace on] | 배치가 다음 방향으로 진행되는지 여부 *[!UICONTROL Budget]* 또는 *[!UICONTROL Impressions]*. | — |
| [!UICONTROL Goals] | [!UICONTROL Max Bid] | 배치에 대한 최대 입찰가. | 예 |
| [!UICONTROL Goals] | [!UICONTROL Flight Pacing] | 배치를 위한 플라이트 게재 간격 전략: *[!UICONTROL Even]*, *[!UICONTROL slightly ahead]*, *[!UICONTROL frontload]*, 또는 *[!UICONTROL aggressive frontload]*. | 예 |
| [!UICONTROL Goals] | [!UICONTROL Intraday Pacing] | 배치에 대한 일일 게재 전략: *[!UICONTROL Even]* 또는 *[!UICONTROL ASAP]*. | 예 |
| [!UICONTROL Goals] | [!UICONTROL Pre-Bid Filters] | 적용할 모든 사전 입찰 필터 기준. | — |
| [!UICONTROL Goals] | [!UICONTROL Bidding Rules] | 입찰 규칙(더 이상 사용되지 않음)이 *[!UICONTROL ON]* 또는 *[!UICONTROL OFF]*. | — |
| [!UICONTROL Goals] | [!UICONTROL Frequency Cap] | 지정된 기간 동안 배치에 대한 주 빈도 상한 [!UICONTROL Frequency Cap Interval]. | 예 |
| [!UICONTROL Goals] | [!UICONTROL Frequency Cap Interval] | 기본 빈도 제한 간격: *[!UICONTROL Day]*, *[!UICONTROL Week]*, 또는 *[!UICONTROL Month]*. | 예 |
| [!UICONTROL Goals] | [!UICONTROL Secondary Frequency Cap] | 지정한 기간 동안 배치에 대한 보조 주파수 캡 [!UICONTROL Secondary Frequency Cap Interval] | 예 |
| [!UICONTROL Goals] | [!UICONTROL Secondary Frequency Cap Interval] | 보조 주파수 상한 간격 유형: *[!UICONTROL Week]*, *[!UICONTROL Day]*, *[!UICONTROL Hour]*, 또는 *[!UICONTROL Minute]*. 적용 가능한 주, 일, 시간 또는 분 수는 [!UICONTROL Secondary Frequency Cap Interval Value]. | 예 |
| [!UICONTROL Goals] | [!UICONTROL Secondary Frequency Cap Interval Value] | 다음 항목에 대한 주, 일, 시간 또는 분 수 [!UICONTROL Secondary Frequency Cap] 적용됩니다. 예를 들어, 보조 캡이 6시간당 세 개의 노출 횟수인 경우 여기서 값은 다음과 같습니다. `6`. | 예 |
| [!UICONTROL Audience Location] | [!UICONTROL Audience Location - Included #] | 타깃팅된 지리적 위치 수, *[!UICONTROL All]*, 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Audience Location] | [!UICONTROL Audience Location - Included] | 세미콜론으로 구분된 타겟팅된 지리적 위치 또는 *[!UICONTROL All Locations]*. | — |
| [!UICONTROL Audience Location] | [!UICONTROL Audience Location - Excluded #] | 제외된 지리적 위치 수 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Audience Location] | [!UICONTROL Audience Location - Excluded] | 세미콜론으로 구분된 제외된 지리적 위치 *[!UICONTROL None]*. | — |
| [!UICONTROL Inventory] | [!UICONTROL Public Inventory - Included #] | 지정된 경우 대상 공개 인벤토리 거래의 수 *[!UICONTROL All]*, 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Inventory] | [!UICONTROL Public Inventory - Excluded #] | 제외된 공개 재고 거래 수(지정된 경우) 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Inventory] | [!UICONTROL Private Inventory - Included #] | 지정된 경우 대상 개인 재고 거래 수 *[!UICONTROL All]*, 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Inventory] | [!UICONTROL Private Inventory - Excluded #] | 제외된 개인 재고 거래 수(지정된 경우) 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Inventory] | [!UICONTROL On Demand Inventory - Included #] | 타겟팅된 수 [!UICONTROL On-Demand Inventory] 거래(지정된 경우) *[!UICONTROL All]*, 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Inventory] | [!UICONTROL On Demand Inventory - Excluded #] | 제외된 온디맨드 재고 거래 수(지정된 경우) 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Sites] | [!UICONTROL Traffic Type] | 타겟팅된 트래픽 유형: *[!UICONTROL Website]* 및/또는 *[!UICONTROL Apps]* | — |
| [!UICONTROL Sites] | [!UICONTROL Exclude out-stream] | 아웃스트림 트래픽을 제외하는 인벤토리 타기팅 옵션이 &lt;i span=&quot;&quot; id=&quot;0&quot; translate=&quot;no&quot; />* 또는 *[!UICONTROL OFF]*.[!UICONTROL >ON]<br>아웃스트림 광고는 대개 비디오 플레이어에서 일반 비디오 광고가 아니라 콘텐츠 위에 팝업 또는 콘텐츠로 채워집니다(기본 경험에서). | — |
| [!UICONTROL Sites] | [!UICONTROL Site Tier] | 타겟팅할 사이트의 품질: *[!UICONTROL Tier 1]*, *[!UICONTROL Tier 2]*, *[!UICONTROL Tier 3]*, 또는 *[!UICONTROL All Sites]*. | — |
| [!UICONTROL Sites] | [!UICONTROL Categories - Included #] | 지정된 경우 타겟팅된 사이트 카테고리의 수 또는 *[!UICONTROL All]*. | — |
| [!UICONTROL Sites] | [!UICONTROL Categories - Excluded #] | 제외된 사이트 범주의 수(지정된 경우) 또는 *[!UICONTROL All]*. | — |
| [!UICONTROL Sites] | [!UICONTROL Excluded Sites] | 제외된 사이트(지정된 경우) 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Sites] | [!UICONTROL Language] | 타겟팅된 사이트 언어입니다. | — |
| [!UICONTROL Sites] | [!UICONTROL Allow unscreened sites] | (표준 디스플레이 배치만 해당) 감사되지 않은 사이트에서의 광고 게재 허용 여부: *[!UICONTROL ON]* 또는 *[!UICONTROL OFF]*. 배치가 개인 인벤토리를 타겟팅하면 이 옵션은 차단된 사이트에 광고를 게재할 수 있습니다. | — |
| [!UICONTROL Sites] | [!UICONTROL Targeted Sites] | 타겟팅된 사이트의 수(있는 경우) 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Audience Targeting] | [!UICONTROL Audience - Included] | 타겟팅된 대상(있는 경우) 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Audience Targeting] | [!UICONTROL Audience - Excluded] | 제외된 대상자(있는 경우) 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Audience Targeting] | [!UICONTROL Demographic booster] | 여부를 불문한다 [!DNL Comscore] 인구 통계학적 세그먼트는 배치(및 캠페인의 다른 배치)에 대해 활성화됩니다. *[!UICONTROL ON]* 또는 *[!UICONTROL OFF]*. 이 기능은 를 사용하는 캠페인에 대해서만 활성화할 수 있습니다. [!DNL Audience Verification] 이(가) 다음에 대해 활성화되었습니다. [!DNL Nielsen] 및/또는 [!DNL Comscore].  추가 비용이 발생합니다. | — |
| [!UICONTROL Audience Targeting] | [!UICONTROL Extend across screens] | 장치 간에 광고 타겟팅을 확장할지 여부: *[!UICONTROL ON]* 또는 *[!UICONTROL OFF]*. 크로스 디바이스 타깃팅은 캠페인 설정에 지정된 디바이스 그래프에 따라 개인의 알려진 모든 디바이스에서 타깃팅을 확장합니다. | — |
| [!UICONTROL Audience Targeting] | [!UICONTROL Topic Targeting] - 포함 # | 지정된 경우 타겟팅된 주제 코드의 수 또는 *[!UICONTROL All]*. | — |
| [!UICONTROL Audience Targeting] | [!UICONTROL Topic Targeting - Excluded #] | 제외된 주제 코드 수(지정된 경우) 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Audience Targeting] | [!UICONTROL Device Targeting - Included #] | 지정된 경우 타겟팅된 디바이스 타겟의 수 또는 *[!UICONTROL All]*. | — |
| [!UICONTROL Audience Targeting] | [!UICONTROL Device Targeting - Excluded #] | 지정된 경우 제외된 장치 대상 수 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Audience Targeting] | [!UICONTROL ISP Targeting - Included #] | 타겟팅된 ISP 공급자 수(지정된 경우) 또는 *[!UICONTROL All]/i>. | — |
| [!UICONTROL Audience Targeting] | [!UICONTROL ISP Targeting - Excluded #] | 제외된 ISP 공급자 수(지정된 경우) 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Brand Safety] | [!UICONTROL Brand Safety - Contextual Filtering #] | 적용된 브랜드 안전 필터 수(지정된 경우) 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Brand Safety] | [!UICONTROL Brand Safety - Pre-Bid Fraud blocking #] | 적용된 사전 입찰 사기 차단 필터 수(지정된 경우) 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Brand Safety] | [!UICONTROL Brand Safety - Pre-Bid Viewability #] | 지정된 경우 적용된 사전 입찰 가시성 필터 수 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Brand Safety] | [!UICONTROL Site Safety Block] | 사이트 안전 차단 활성화 여부: *[!UICONTROL ON]* 또는 *[!UICONTROL OFF]*.<!-- Whether or not the advertiser-level setting Enable Site Safety Block is enabled: *ON* or *OFF*.I don’t see this option at the placement level. Should there be one? --> | — |
| [!UICONTROL Tracking] | [!UICONTROL Tracking Pixels #] | 배치에 연결된 타사 이벤트 추적 픽셀 수 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Tracking] | [!UICONTROL Conversion Pixels #] | 배치에 첨부된 전환 추적 픽셀 수 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Tracking] | [!UICONTROL 3rd-party fees] | 1000회 노출당 청구 불가능한 비용으로 추적할 정적 타사 수수료 비율(해당하는 경우). | — |
| [!UICONTROL Ads] | [!UICONTROL # of Ads Attached] | 배치에 첨부된 광고 수(있는 경우) 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Ads] | [!UICONTROL Ad Names] | 배치에 첨부된 광고의 이름 또는 *[!UICONTROL None]*. | — |
| [!UICONTROL Ads] | [!UICONTROL Attached Ad ID] | 배치에 첨부된 고유 DSP 생성 광고 ID로, 세미콜론으로 구분됩니다. 에서 광고 이름 및 관련 광고 ID 목록을 다운로드하려면 [!UICONTROL Ads] 보기, 다음을 포함하는 사용자 지정 보기 만들기 [!UICONTROL Ad ID] 지표 및 [데이터 내보내기](/help/dsp/campaign-management/reports/campaign-export-data.md). | 예 |

### 배치 수준 스프레드시트

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
| [!UICONTROL Budget Interval] | 예산 간격: &lt;i span=&quot;&quot; id=&quot;0&quot; translate=&quot;no&quot; />*, *[!UICONTROL Weekly]*, *[!UICONTROL Monthly]*, 또는 *[!UICONTROL All Time]*.[!UICONTROL >Daily] | 예 |
| [!UICONTROL Primary Frequency Cap] | 지정된 기간 동안 배치에 대한 주 빈도 상한 [!UICONTROL Primary Frequency Cap Interval]. | 예 |
| [!UICONTROL Primary Frequency Cap Interval] | 기본 빈도 제한 간격: *[!UICONTROL Day]*, *[!UICONTROL Week]*, 또는 *[!UICONTROL Month]*. | 예 |
| [!UICONTROL Secondary Frequency Cap] | 지정한 기간 동안 배치에 대한 보조 주파수 캡 [!UICONTROL Secondary Frequency Cap Interval] | 예 |
| [!UICONTROL Secondary Frequency Cap Interval] | 보조 주파수 상한 간격 유형: *[!UICONTROL Week]*, *[!UICONTROL Day]*, *[!UICONTROL Hour]*, 또는 *[!UICONTROL Minute]*. 적용 가능한 주, 일, 시간 또는 분 수는 [!UICONTROL Secondary Frequency Cap Interval Value]. | 예 |
| [!UICONTROL Secondary Frequency Cap Interval Value] | 다음 항목에 대한 주, 일, 시간 또는 분 수 [!UICONTROL Secondary Frequency Cap] 적용됩니다. 예를 들어, 보조 캡이 6시간당 세 개의 노출 횟수인 경우 여기서 값은 다음과 같습니다. `6`. | 예 |
| [!UICONTROL Attached Ad ID] | 배치에 첨부된 고유 DSP 생성 광고 ID로, 세미콜론으로 구분됩니다. 에서 광고 이름 및 관련 광고 ID 목록을 다운로드하려면 [!UICONTROL Ads] 보기, 다음을 포함하는 사용자 지정 보기 만들기 [!UICONTROL Ad ID] 지표 및 [데이터 내보내기](/help/dsp/campaign-management/reports/campaign-export-data.md). | 예 |

>[!MORELIKETHIS]
>
>* [배치 편집](/help/dsp/campaign-management/placements/placement-edit.md)
>* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)
