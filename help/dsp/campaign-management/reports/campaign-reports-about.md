---
title: Campaign Management 보기의 성능 보고서 유형
description: 캠페인 관리 보기에 포함된 보고서 데이터에 대해 알아봅니다.
feature: DSP Campaign Data Views
exl-id: 7af97704-2053-4862-a851-12db009e6776
source-git-commit: 1ac58da2d538cc682161ebc944a0412ad4a8af17
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---

# Campaign Management 보기의 성능 보고서 유형

캠페인 관리 보기에는 포괄적인 보고서 데이터가 포함됩니다. 사용 가능한 보고서를 통해 성과가 좋은 패키지 및 배치와 주의가 필요한 배치를 식별할 수 있습니다. 또한 빠른 작업 버튼을 사용하면 생산성이 향상됩니다.

## 모든 캠페인 보기

다음 [!UICONTROL Campaigns] 성능 데이터 차트 세트와 계정 내 모든 캠페인 목록에 대한 보기 가 열립니다.

### 차트 보기 {#chart-view}

다음을 수행할 수 있습니다. [시계열 트렌드 차트 사용자 지정](campaign-data-views-manage.md#data-visualizations-manage) 세 개의 지표를 사용하는 모든 캠페인에서. 기본적으로 다음에 대한 데이터 [!UICONTROL Net Spend], [!UICONTROL Impressions], 및 [!UICONTROL Net CPM] 별도의 차트(트렐리스 차트)에 포함됩니다. 선택적으로 지표를 변경할 수 있습니다. 시계열 트렌드 차트에서 시간별 데이터를 활성화하려면 날짜 선택 사항을 하루 ( )로 변경하십시오.[!UICONTROL Today], [!UICONTROL Yesterday]또는 특정 날짜)에 전송됩니다.

![세 가지 지표에 대한 별도의 트렌드 차트](/help/dsp/assets/trend-chart-separate.png)

또한 선택적으로 세 개의 지표를 오버레이하여 예외 항목을 쉽게 탐지하고 규모나 성능을 향상시킬 수 있는 영역을 탐지할 수 있습니다.

![오버레이가 있는 트렌드 차트](/help/dsp/assets/trend-chart.png)

### 표 보기

![캠페인 목록](/help/dsp/assets/campaigns-list.png)

기본적으로 각 캠페인 행에는 게재 간격 및 게재 지표가 포함됩니다. 게재 간격 지표는 다음과 같습니다 [!UICONTROL Gross Spend (Lifetime)]캠페인의 모든 패키지에서 실제 타겟 내 지출과 예상 타겟 내 지출의 측정이 포함되어 있어 성과가 낮은 캠페인을 한 눈에 파악할 수 있습니다. 다음을 선택적으로 수행할 수 있습니다 [열 보기 변경](campaign-data-views-manage.md#column-view-change) 또는 짝수 [사용자 정의 열 보기 만들기](campaign-data-views-manage.md#column-view-create).

추가 작업 가능 [데이터 테이블 사용자 지정](campaign-data-views-manage.md#data-tables-manage) 추가적인 방법으로 [표시되는 데이터 필터링](campaign-data-views-manage.md#filter-data-tables).

<!--
An "Alerts" column indicates when a campaign (or any child entity under it) has an issue. Alert indicators include "Critical" (![Critical](/help/dsp/assets/indicator-critical.png "Critical")) and "Warning" (![Warning](/help/dsp/assets/indicator-warning.png "Warning")). See "[View Alerts and Notifications](campaign-alerts.md) for more information.
-->

캠페인을 자세히 보려면 캠페인 이름을 클릭합니다.

## 단일 캠페인 보고 {#single-campaign-reporting}

캠페인 내에서 캠페인 엔티티를 기반으로 데이터를 필터링할 수 있습니다. [!UICONTROL Packages], [!UICONTROL Placements], 및 [!UICONTROL Ads]. 추가 작업 가능 [표시되는 데이터 필터링](campaign-data-views-manage.md#filter-data-tables) 보려는 패키지, 배치 또는 광고만 포함합니다.

![캠페인 엔티티 탭](/help/dsp/assets/campaign-subtabs.png)

### 차트 보기

각 캠페인에 대해 다음을 수행할 수 있습니다. [시계열 트렌드 차트 사용자 지정](campaign-data-views-manage.md#data-visualizations-manage) 세 개의 지표를 사용하며, 각 엔티티 보기에서 사용할 수 있습니다. 캠페인의 모든 트렌드 차트에 동일한 지표가 유지됩니다.

다음을 참조하십시오. [캠페인 간 지표에 대한 &quot;차트 보기&quot; 섹션](#chart-view) 추가 정보.

### 표 보기

각 엔티티 탭에서 각 행에는 기본적으로 게재 간격 및 게재 지표가 포함되어 있지만 다음을 수행할 수 있습니다. [열 보기 변경](campaign-data-views-manage.md#column-view-change) 또는 짝수 [사용자 정의 열 보기 만들기](campaign-data-views-manage.md#column-view-create) 을 추가하여 캠페인의 모든 하위 탭에 적용합니다. 추가 작업 가능 [데이터 테이블 사용자 지정](campaign-data-views-manage.md#data-tables-manage) 추가 방법으로. 각 데이터 테이블에는 [!UICONTROL Subtotals] 행 - 표시되는 모든 행에서 각 지표의 합계 또는 평균 값을 표시합니다.

<!--
An "Alerts" column indicates when a package, placement, or ad &mdash; or any child entity under a package or placement &mdash; has an issue. Alert indicators include "Critical" (![Critical](/help/dsp/assets/indicator-critical.png "Critical")) and "Warning" (![Warning](/help/dsp/assets/indicator-warning.png "Warning")). See "[View Alerts and Notifications](campaign-alerts.md) for more information.
-->

### 기타 유형의 캠페인 수준 보고

기타 데이터 분류의 경우 다음을 확인하십시오. [캠페인 수준 보고 페이지](/help/dsp/campaign-management/campaigns/campaign-view-report.md). 이 보고서에는 다음 섹션이 포함됩니다. [!UICONTROL Geography], [!UICONTROL Device], [!UICONTROL Viewability], 및 [!UICONTROL Audience Performance] 데이터.

### 배치 수준 보고의 다른 유형

기타 데이터 분류의 경우 다음을 확인하십시오. [배치 수준 보고 페이지](/help/dsp/campaign-management/placements/placement-view-report.md). 이 보고서에는 다음 섹션이 포함됩니다. [!UICONTROL Geography], [!UICONTROL Device], [!UICONTROL Viewability], [!UICONTROL Audience Performance], [!UICONTROL Notifications], 및 [!UICONTROL Ads] 데이터.

또한 배치 설정 내에서 다음 데이터를 볼 수 있습니다.

* [A (세부 사항 보기) [!UICONTROL Inspector])](placement-details-view.md): 모든 타겟팅된 사이트, 광고, 빈도 데이터 및 배치 거래를 보여 줍니다.

* A [배치 예측 보고서](/help/dsp/campaign-management/reports/placement-forecast.md)

* [배치 진단 보고서](/help/dsp/campaign-management/reports/placement-diagnostics.md).


### 기타 유형의 광고 수준 보고

기타 데이터 분류의 경우 다음을 확인하십시오. [광고 수준 보고 페이지](/help/dsp/campaign-management/ads/ad-view-report.md). 보고서에는 다음이 포함됩니다 [!UICONTROL Overview], [!UICONTROL Geography], 및 [!UICONTROL Viewability] 데이터.

>[!MORELIKETHIS]
>
>* [배치에 대한 사이트, 광고 및 빈도 세부 정보 보기](placement-details-view.md)
>* [Campaign 데이터 보기 관리](campaign-data-views-manage.md)
>* [Campaign Management 보기에서 데이터 내보내기](campaign-export-data.md)
>* [캠페인에 대한 세부 보고서 보기](/help/dsp/campaign-management/campaigns/campaign-view-report.md)
