---
title: Campaign 데이터 보기 관리
description: 캠페인, 패키지, 배치 및 광고에 대한 데이터 보기를 사용자 지정하는 방법을 알아봅니다.
feature: DSP Campaign Data Views
source-git-commit: 1ac58da2d538cc682161ebc944a0412ad4a8af17
workflow-type: tm+mt
source-wordcount: '915'
ht-degree: 0%

---

# Campaign 데이터 보기 관리

캠페인 관리 보기( )에 표시되는 데이터를 사용자 지정할 수 있습니다.[!UICONTROL Campaigns], [!UICONTROL Packages], [!UICONTROL Placements], 및 [!UICONTROL Ads]).

## 데이터 시각화 관리 {#data-visualizations-manage}

캠페인 간 또는 단일 캠페인에 대한 모든 데이터 시각화에 대한 지표 및 차트 모드를 변경할 수 있습니다. 단일 캠페인에 대한 변경 사항은 의 데이터 시각화를 포함하여 캠페인에 대한 모든 데이터 시각화에 적용됩니다. [!UICONTROL Packages], [!UICONTROL Placements], 및 [!UICONTROL Ads] 보기.

### 데이터 시각화를 위한 지표 변경

1. 데이터 시각화의 오른쪽 상단에서 ![설정](/help/dsp/assets/settings-chart.png).

1. 지표를 선택합니다.

   동일한 지표를 두 번 선택할 수 없습니다.

1. 클릭 **[!UICONTROL Apply]**.

### 데이터 시각화의 표시 모드 변경

* 데이터 시각화의 오른쪽 상단에서 [!UICONTROL Overlay] 전환(![오버레이 스위치](/help/dsp/assets/overlay.png)) 오버레이 모드(모든 차트가 함께 오버레이됨)와 트렐리스 차트 모드(세 개의 개별 차트) 간에 변경할 수 있습니다.

## 데이터 테이블 관리 {#data-tables-manage}

모든 캠페인 관리 보기([!UICONTROL Campaigns], [!UICONTROL Packages], [!UICONTROL Placements], 및 [!UICONTROL Ads]) 데이터 테이블 내에 표시되는 데이터를 사용자 지정할 수 있습니다.

### 열 보기 관리 {#column-views-manage}

각 캠페인 관리 수준([!UICONTROL Campaigns], [!UICONTROL Packages], [!UICONTROL Placements], 및 [!UICONTROL Ads]) 기본 제공 포함 [!UICONTROL Pacing] 및 [!UICONTROL Performance] 해당 엔티티에 대한 관련 지표를 포함하는 보기. 기본적으로 [!UICONTROL Pacing] 성과가 낮은 캠페인 및 캠페인 구성 요소를 한 눈에 식별할 수 있도록 보기가 표시됩니다. 선택적으로 사용자 정의 열 세트를 만들고 편집할 수 있습니다.

![열 보기 선택기](/help/dsp/assets/column-view-selector.png)

DSP에서는 가장 최근 보기를 기본 보기로 저장하므로 페이지로 돌아올 때마다 사용자와 관련된 지표를 항상 볼 수 있습니다.

#### 열 보기 변경 {#column-view-change}

* 보기 선택기에서 ![아래쪽 화살표](/help/dsp/assets/chevron-down.png)을 클릭하고 원하는 열 보기의 이름을 클릭합니다.

#### 사용자 정의 열 보기 만들기 {#column-view-create}

1. 보기 선택기에서 ![아래쪽 화살표](/help/dsp/assets/chevron-down.png)을 클릭한 다음 을 클릭합니다 **[!UICONTROL Create View]**.

1. 보기에 포함할 지표를 지정합니다.

   1. 사용 가능한 지표 목록에서 포함할 각 지표 옆에 있는 확인란을 선택합니다.

      모든 지표는 범주별로 알파벳순입니다. [!UICONTROL Settings], [!UICONTROL Spend], [!UICONTROL Pacing], [!UICONTROL Reporting] (DSP이 추적하는 표준 지표), [!UICONTROL Viewability], 및 [!UICONTROL Conversions]. &quot;(&quot;가 추가된 지표[!UICONTROL Lifetime])&quot; 페이지에서 선택한 날짜 범위에 관계없이 캠페인 시작부터 값을 반환합니다.

   1. 오른쪽 패널의 열 이름을 클릭하고 필요한 위치로 끌어 열 순서를 필요에 따라 편집합니다.

   일부 열에는 고정된 위치가 있으므로 이동하거나 제거할 수 없습니다.

1. 설정을 적용하거나 저장합니다.

   * 설정을 보기에 저장하지 않고 임시로 적용하려면 **[!UICONTROL Apply].**

   * 설정을 새로운 사용자 정의 열 보기에 저장하려면 **[!UICONTROL Save As]**. 다음에서 [!UICONTROL Save View] 창에서 새 뷰의 이름을 입력한 다음 **[!UICONTROL Save]**.

#### 열 보기 편집 {#column-view-edit}

>[!NOTE]
>
>변경 내용을 표준(사전 정의된) 열 보기에 저장할 수는 없지만 변경 내용을 일시적으로 적용하거나 새 사용자 지정 보기에 저장할 수는 있습니다.

1. 보기 선택기에서 ![아래쪽 화살표](/help/dsp/assets/chevron-down.png)을 클릭하고 기존 열 보기 이름을 클릭합니다.

1. 보기 선택기에서 ![아래쪽 화살표](/help/dsp/assets/chevron-down.png)을 클릭한 다음 을 클릭합니다 **[!UICONTROL Edit View]**.

1. 보기에 포함할 지표를 편집합니다.

   1. 사용 가능한 지표 목록에서 포함할 각 지표 옆의 확인란을 선택하고 제외할 각 지표 옆의 확인란을 선택 취소합니다.

      모든 지표는 범주별로 알파벳순입니다. [!UICONTROL Settings], [!UICONTROL Spend], [!UICONTROL Pacing], [!UICONTROL Reporting] (DSP이 추적하는 표준 지표), [!UICONTROL Viewability], 및 [!UICONTROL Conversions]. &quot;(&quot;가 추가된 지표[!UICONTROL Lifetime])&quot; 페이지에서 선택한 날짜 범위에 관계없이 캠페인 시작부터 값을 반환합니다.

   1. 오른쪽 패널의 열 이름을 클릭하고 필요한 위치로 끌어 열 순서를 필요에 따라 편집합니다.

   일부 열에는 고정된 위치가 있으므로 이동하거나 제거할 수 없습니다.

1. 설정을 적용하거나 저장합니다.

   * (사용자 정의 보기 전용) 설정을 저장하려면 **[!UICONTROL Save]**.

   * 설정을 보기에 저장하지 않고 임시로 적용하려면 **[!UICONTROL Apply].**

   * 설정을 새로운 사용자 정의 열 보기에 저장하려면 **[!UICONTROL Save As]**. 다음에서 [!UICONTROL Save View] 창에서 새 뷰의 이름을 입력한 다음 **[!UICONTROL Save]**.

### 캠페인 데이터 필터링 {#filter-data-tables}

필터는 현재 탭에 표시되는 데이터를 변경합니다. 사용 가능한 필터는 엔티티 유형에 따라 다르지만 엔티티 이름, 상태 및 추가 속성 열을 포함할 수 있습니다.

1. 기본 도구 모음에서 를 클릭합니다 ![필터 단추](/help/dsp/assets/filter.png).
1. 적용할 각 필터에 대해 왼쪽 열에서 필터 이름을 클릭한 다음 필터 값을 지정합니다.
1. 클릭 **[!UICONTROL Apply]**.

#### 사용 가능한 필터

에서 다음 필터를 사용할 수 있습니다. [!UICONTROL Campaigns], [!UICONTROL Packages], 및 [!UICONTROL Placements] 보기 수:

* [!UICONTROL Campaigns] 필터 보기:
   * [!UICONTROL Campaign status]
   * [!UICONTROL Advertiser]
* [!UICONTROL Packages] 필터 보기:
   * [!UICONTROL Custom flights] (존재 여부)
   * [!UICONTROL Custom goal] (해당되는 경우)
   * [!UICONTROL End end date]
   * [!UICONTROL Optimization goal]
   * [!UICONTROL Flight pacing]
   * [!UICONTROL Intraday pacing]
   * [!UICONTROL Package status]
   * [!UICONTROL Start date]
* [!UICONTROL Placements] 필터 보기:
   * [!UICONTROL Custom ad scheduling]
   * [!UICONTROL Custom goal] (해당되는 경우)
   * [!UICONTROL End date]
   * [!UICONTROL Max bid] ([!UICONTROL less than], [!UICONTROL greater than], 또는 [!UICONTROL equal to] 지정된 값)
   * [!UICONTROL Optimization goal]
   * [!UICONTROL Pacing on] ([!UICONTROL impressions] 또는 [!UICONTROL spend])
   * [!UICONTROL Flight pacing]
   * [!UICONTROL Intraday pacing]
   * [!UICONTROL Package]
   * [!UICONTROL Placement status]
   * [!UICONTROL Placement type]
   * [!UICONTROL Placement sub-type]
   * [!UICONTROL Start date]
   * [!UICONTROL Creation date]
* [!UICONTROL Ads] 필터 보기:
   * [!UICONTROL Adobe ad approval status]
   * [!UICONTROL Ad ID]
   * [!UICONTROL Ad name]
   * [!UICONTROL Ad type]
   * [!UICONTROL Creation date]


### 날짜 범위 변경

데이터 테이블 위에 날짜 범위 선택기를 사용하여 모든 표준 및 사용자 지정 보기에 사용되는 날짜 범위를 변경합니다.

![날짜 범위 선택기](/help/dsp/assets/date-range-selector.png "날짜 범위 선택기")

* 사전 설정된 범위의 경우: 공통 시간 증가 목록에서 선택합니다. 기본값은 입니다 [!UICONTROL Last 30 days]*.

* 특정 범위에 대해 다음 중 하나를 수행합니다.

   * 클릭 ![캘린더](/help/dsp/assets/calendar.png "캘린더")을 클릭한 다음 달력 내에서 시작 날짜와 종료 날짜를 클릭합니다.

   * 날짜 범위 내에서 를 클릭한 다음 시작 날짜와 종료 날짜를 입력하거나 달력 내에서 선택합니다.

     숫자 값(M-D-YY부터 MM-DD-YYYY까지) 및/또는 월 이름이나 약어(예: Jan 또는 January)를 입력할 수 있습니다.

### 데이터 열 정렬

데이터 열을 오름차순(A에서 Z까지 또는 1에서 10까지) 또는 내림차순(Z에서 A까지 또는 10에서 1)으로 정렬할 수 있습니다.

* 오름차순과 내림차순 간을 전환하려면 열 헤더를 클릭하십시오.


### 데이터 행 수 지정

페이지의 오른쪽 하단에 있는 **[!UICONTROL Items per page]** , 선택 *[!UICONTROL 25]*, *[!UICONTROL 50]*, 또는 *[!UICONTROL 100]*.

>[!MORELIKETHIS]
>
>* [Campaign Management 보기의 성능 보고서 유형](campaign-reports-about.md)
>* [배치에 대한 사이트, 광고 및 빈도 세부 정보 보기](placement-details-view.md)
>* [배치 예측 보고서 보기](/help/dsp/campaign-management/reports/placement-forecast.md)
>* [배치 진단 보고서 보기](placement-diagnostics.md)
>* [Campaign Management 보기에서 데이터 내보내기](campaign-export-data.md)
>* [비디오: DSP 계정 구조 및 사용자 인터페이스](https://experienceleague.adobe.com/docs/advertising-learn/tutorials/dsp/ui.html)
