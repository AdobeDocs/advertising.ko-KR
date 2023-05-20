---
title: 플랫폼 내 보고서 정보
description: 캠페인 관리 보기에 포함된 보고서 데이터에 대해 알아봅니다.
feature: DSP Campaign Data Views
exl-id: 7af97704-2053-4862-a851-12db009e6776
source-git-commit: 7e614ecb517515217d812926f61ca10437820efd
workflow-type: tm+mt
source-wordcount: '940'
ht-degree: 0%

---

# 플랫폼 내 보고서 정보

<!-- rename "About Performance Reports in Campaign Management Views?" -->
캠페인 관리 보기에는 포괄적인 보고서 데이터가 포함됩니다. 사용 가능한 보고서를 통해 성과가 좋은 패키지 및 배치와 주의가 필요한 배치를 식별할 수 있습니다. 또한 빠른 작업 버튼을 사용하면 생산성이 향상됩니다.

## 모든 캠페인 보기

다음 [!UICONTROL Campaigns] 성능 데이터 차트 세트와 계정 내 모든 캠페인 목록에 대한 보기 가 열립니다.

### 차트 보기 {#chart-view}

다음을 수행할 수 있습니다. [시계열 트렌드 차트 사용자 지정](campaign-data-visualization-manage.md) 세 개의 지표를 사용하는 모든 캠페인에서. 기본적으로 다음에 대한 데이터 [!UICONTROL Net Spend], [!UICONTROL Impressions], 및 [!UICONTROL Net CPM] 별도의 차트(트렐리스 차트)에 포함됩니다. 선택적으로 지표를 변경할 수 있습니다. 시계열 트렌드 차트에서 시간별 데이터를 활성화하려면 날짜 선택 사항을 하루 ( )로 변경하십시오.[!UICONTROL Today], [!UICONTROL Yesterday]또는 특정 날짜)에 전송됩니다.

![세 가지 지표에 대한 별도의 트렌드 차트](/help/dsp/assets/trend-chart-separate.png)

또한 선택적으로 세 개의 지표를 오버레이하여 예외 항목을 쉽게 탐지하고 규모나 성능을 향상시킬 수 있는 영역을 탐지할 수 있습니다.

![오버레이가 있는 트렌드 차트](/help/dsp/assets/trend-chart.png)

### 표 보기

![캠페인 목록](/help/dsp/assets/campaigns-list.png)

기본적으로 각 캠페인 행에는 게재 간격 및 게재 지표가 포함됩니다. 게재 간격 지표는 다음과 같습니다 [!UICONTROL Gross Spend (Lifetime)]캠페인의 모든 패키지에서 실제 타겟 내 지출과 예상 타겟 내 지출의 측정이 포함되어 있어 성과가 낮은 캠페인을 한 눈에 파악할 수 있습니다. 다음을 선택적으로 수행할 수 있습니다 [열 보기 변경](column-view-change.md) 또는 짝수 [사용자 정의 열 보기 만들기](column-view-create.md).

추가 작업 가능 [데이터 테이블 사용자 지정](campaign-data-views-about.md) 추가적인 방법으로 [표시되는 데이터 필터링](campaign-data-filter.md).

캠페인을 자세히 보려면 캠페인 이름을 클릭합니다.

## 단일 캠페인 보고 {#single-campaign-reporting}

캠페인 내에서 캠페인 엔티티를 기반으로 데이터를 필터링할 수 있습니다. [!UICONTROL Packages], [!UICONTROL Placements], 및 [!UICONTROL Ads]. 추가 작업 가능 [표시되는 데이터 필터링](campaign-data-filter.md) 보려는 패키지, 배치 또는 광고만 포함합니다.

![캠페인 엔티티 탭](/help/dsp/assets/campaign-subtabs.png)

### 차트 보기

각 캠페인에 대해 다음을 수행할 수 있습니다. [시계열 트렌드 차트 사용자 지정](campaign-data-visualization-manage.md) 세 개의 지표를 사용하며, 각 엔티티 보기에서 사용할 수 있습니다. 캠페인의 모든 트렌드 차트에 동일한 지표가 유지됩니다.

다음을 참조하십시오. [캠페인 간 지표에 대한 &quot;차트 보기&quot; 섹션](#chart-view) 추가 정보.

### 표 보기

각 엔티티 탭에서 각 행에는 기본적으로 게재 간격 및 게재 지표가 포함되어 있지만 다음을 수행할 수 있습니다. [열 보기 변경](column-view-change.md) 또는 짝수 [사용자 정의 열 보기 만들기](column-view-create.md) 을 추가하여 캠페인의 모든 하위 탭에 적용합니다. 추가 작업 가능 [데이터 테이블 사용자 지정](campaign-data-views-about.md) 추가 방법으로. 각 데이터 테이블에는 [!UICONTROL Subtotals] 행 - 표시되는 모든 행에서 각 지표의 합계 또는 평균 값을 표시합니다.

### 배치 [!UICONTROL Inspector] {#placement-inspector}

각 배치에 대해 다음 작업을 수행할 수 있습니다 [(세부 사항 보기) 열기 [!UICONTROL Inspector])](placement-details-view.md): 다음과 같은 심층 데이터가 포함됩니다.

* **[!UICONTROL Sites]:** 배치가 인상을 받은 모든 사이트입니다.

   다음 [!UICONTROL Sites] 탭에는 검색 및 필터 기능, 기본 페이지에서 사용할 수 있는 동일한 표준 및 사용자 정의 열 보기 옵션, [!UICONTROL Exclude] 배치에서 사이트를 빠르게 제외할 수 있도록 각 행의 단추

* **[!UICONTROL Ads]:** 배치의 모든 광고.

   다음 [!UICONTROL Ads] 탭에는 검색 및 필터 기능, 기본 페이지에서 사용할 수 있는 동일한 표준 및 사용자 정의 열 보기 옵션, 각 행의 빠른 작업 버튼이 포함되어 있습니다. [!UICONTROL Pause] (따라서 광고를 빠르게 일시 중지할 수 있습니다.)

* **[!UICONTROL Frequency]:** 다음을 포함한 배치의 각 광고 빈도 수준에 대한 데이터:
   * 광고 빈도 수준(예: 사용자가 광고를 한 번 본 모든 인스턴스의 경우 &quot;1&quot;)
   * 예상 고유 장치/브라우저 또는 사람 수(지정된 항목에 따라 다름) [!UICONTROL Cross Device Level] (캠페인의 경우) 지정된 빈도 수준에서 노출시킨 사용자
   * 지정된 빈도 수준의 예상 노출 횟수
   * 지정된 빈도 수준의 예상 평균 빈도입니다. 이 값은 (예상 노출 횟수)/(예상 고유 수)와 같습니다.

* **[!UICONTROL Inventory]:** 배치의 타겟이 되는 모든 거래에 대한 정보.

   다음 [!UICONTROL Inventory] 탭에서는 다음과 같은 성능 통계를 표시하여 신속한 문제 해결을 지원합니다. [!UICONTROL Auctions], [!UICONTROL Bids], 및 [!UICONTROL Win Rate]. 탭에는 검색 및 필터 기능, 기본 페이지에서 사용할 수 있는 동일한 표준 및 사용자 정의 열 보기 옵션, 각 행의 빠른 작업 버튼이 포함되어 있습니다. [!UICONTROL Edit], [!UICONTROL View Report], 및 [[!UICONTROL Auction Insights] 추가적인 문제 해결을 위해](/help/dsp/inventory/private-deal-auction-insights.md).

#### 인벤토리 문제 해결

| 문제 | 가능한 원인 | 수행할 작업 |
| -----------| ---------- | ---------- |
| [!UICONTROL Zero Auctions] | 게시자가 입찰 요청을 보내지 않았습니다. | 게시자에게 연락하여 거래를 활성화하십시오. |
|  | 잘못된 외부 거래 ID를 입력하는 등 거래가 잘못 설정되었습니다. | 거래 세부 사항을 확인하고 거래를 편집합니다. |
| [!UICONTROL Auctions but no Bids] | 배치 타깃팅이 거래에 대한 수신 입찰 요청과 일치하지 않습니다. <br><br> 예를 들어, 배치는 거래에 적합하지 않은 지역을 타깃팅할 수 있습니다. | 타겟팅 불일치를 방지하기 위해 필요에 따라 배치 타겟을 편집합니다. |
|  | 게재에 거래에 필요한 미디어 유형의 활성 광고가 없습니다. | 올바른 미디어 유형의 광고를 만들어 배치에 첨부합니다. |
|  | 그 자리에는 충분한 예산이 없다. | 수신 요청에 대한 입찰을 허용하도록 배치 예산을 늘립니다. |
|  | 배치 플라이트 날짜가 거래의 노출 전달 날짜와 겹치지 않습니다. | 필요에 따라 배치의 플라이트 날짜를 편집합니다. |
| [!UICONTROL Low Win Rate] | 배치의 최대 입찰(층 또는 고정)이 거래에서 요구하는 최소 입찰가보다 낮습니다. | 배치 늘리기 [!UICONTROL Max Bid] 필요한 경우. |
|  | 배치에서는 입찰을 제한하는 사전 입찰 필터를 사용합니다. | 더 많은 입찰을 허용하도록 사전 입찰 필터의 임계값을 낮춥니다. |
|  | 배치에 대한 대상 타깃팅이 너무 제한적입니다. | 지정된 대상 타겟에 활성 사용자가 충분한지 확인하고, 가능한 경우 대상을 확장합니다. |

![배치 검사기](/help/dsp/assets/placement-inspector.png)

다음에서 데이터를 내보낼 수 있습니다. [!UICONTROL Sites], [!UICONTROL Ads], 또는 [!UICONTROL Frequency] 탭으로 이동하여 브라우저의 기본 다운로드 폴더를 XLSM 형식의 보고서로 표시합니다.

### 기타 유형의 캠페인 수준 보고

기타 데이터 분류의 경우 다음을 확인하십시오. [캠페인 수준 보고 페이지](/help/dsp/campaign-management/campaigns/campaign-view-report.md). 다음 <!--legacy --> 보고서에 다음 섹션이 포함됨: [!UICONTROL Geography], [!UICONTROL Device], [!UICONTROL Viewability], 및 [!UICONTROL Audience Performance] 데이터.

>[!MORELIKETHIS]
>
>* [배치에 대한 사이트, 광고 및 빈도 세부 정보 보기](placement-details-view.md)
>* [Campaign 데이터 보기 정보](campaign-data-views-about.md)
>* [사용자 정의 열 보기 만들기](column-view-create.md)
>* [열 보기 변경](column-view-change.md)
>* [데이터 시각화 관리](campaign-data-visualization-manage.md)
>* [Campaign Management 보기에서 데이터 내보내기](campaign-export-data.md)
>* [캠페인에 대한 세부 보고서 보기](/help/dsp/campaign-management/campaigns/campaign-view-report.md)

