---
title: (새 UI) Advertising 인사이트
description: 모델 정확도, 성능, 시뮬레이션, 예산 한도 및 전환에 대해 광고 insight 대시보드를 구성하고 보는 방법을 알아봅니다.
feature: Search Advertising Insights
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: bc8b5578-58f6-5342-a640-fce94e5ff4a7
    internal-label: Search Advertising Insights
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: 54920f5e0e08c1bf6f960b4d96aa4161dfa11143
workflow-type: tm+mt
source-wordcount: '1217'
ht-degree: 0%
---
# (새 UI) Advertising 인사이트

Advertising 인사이트는 포트폴리오 성능을 평가하고, 최적화 문제를 식별하고, 전환 데이터를 비교하는 데 도움이 되는 시각적이고 실행 가능한 데이터를 제공합니다. 각 insight은 온디맨드로 생성되고 온스크린 대시보드로 표시됩니다.

**[!UICONTROL Reports]>[!UICONTROL Insights]** 보기에는 **[!UICONTROL Dashboards]** 아래에 사용 가능한 인사이트가 표시됩니다. 페이지 머리글은 **[!UICONTROL Advertising Insights]**&#x200B;입니다.

>[!NOTE]
>
>이 페이지에서는 Beta 새 사용자 인터페이스의 insight 대시보드에 대해 설명합니다. 사용 가능 여부는 선택한 광고주가 사용할 수 있는 인사이트 및 액세스 권한에 따라 다릅니다. [기존 Advertising Insights](/help/search-social-commerce/advertising-insights/insight-about.md)에는 생성된 파일에 대한 다른 분석 및 절차 집합이 포함되어 있습니다.

## 인사이트 유형 {#insight-types}

| Insight | 설명 |
| --- | --- |
| [!UICONTROL Model Accuracy] | Search, Social 및 Commerce이 포트폴리오의 비용과 수익을 얼마나 잘 예측하는지를 식별합니다. 포트폴리오, 광고 네트워크 및 캠페인 수준에서 모델 정확도를 검토할 수 있습니다. |
| [!UICONTROL Performance Insights] | 최적화 상태 변경, 목표 변경 또는 지정된 날짜 전후의 포트폴리오 성과를 비교합니다. 대시보드에는 성능 요약, 최적화에 영향을 주는 변경 사항 감사, 캠페인 비교, 트렌드 및 목표 값 분석이 포함됩니다. |
| [!UICONTROL Portfolio Simulation Analysis] | 기존 사용자 지정 시뮬레이션을 실제 성능과 비교합니다. 포트폴리오 및 캠페인 데이터를 검토하고, 시뮬레이션 정확도를 분석하고, 다양한 목표 지출 수준에서 예상 성과를 탐색할 수 있습니다. |
| [!UICONTROL Campaign Budget Cap Analysis] | 포트폴리오 지출이 캠페인 예산 상한으로 제한되었는지 여부를 나타냅니다. 대시보드에는 제한 지출, 영향을 받는 캠페인, 예상 손실 노출 횟수, 일별 및 주별 트렌드 및 포트폴리오 설정에 대한 권장 사항이 포함됩니다. |
| [!UICONTROL Modeled Conversions] | Adobe 전환 값을 모델 데이터를 포함하여 광고 네트워크에서 보고한 값과 비교합니다. 계정, 포트폴리오 또는 캠페인을 분석하고 Adobe 측정 및 Adobe 측정 및 모델 값을 게시자가 보고한 값과 비교할 수 있습니다. |
| [!UICONTROL Delayed Revenue Analysis] | 전환 지연(광고 클릭 또는 뷰스루와 후속 전환 사이에 경과된 시간)을 측정하고, 목표값, 투자 수익률(ROI) 및 모델 정확도에 대한 영향을 보여줍니다. 분석은 클릭 기반 또는 뷰스루 매출 기여도 분석이 있는 포트폴리오에만 사용할 수 있습니다. |

## insight 생성 {#insight-generate}

1. 메인 메뉴에서 **[!UICONTROL Reports]>[!UICONTROL Insights]**&#x200B;을(를) 클릭합니다.

1. 생성하려는 insight을 클릭합니다.

1. **[!UICONTROL Configure]** 패널에서 [insight 설정](#insight-settings)을 지정합니다.

1. **[!UICONTROL Generate Insight]**&#x200B;을(를) 클릭합니다.

   구성 패널이 닫히고 대시보드에 분석이 표시됩니다.

1. [insight 결과](#insight-results)를 검토하십시오.

설정을 변경하려면 **[!UICONTROL Configure]**&#x200B;을(를) 클릭하고 값을 변경한 다음 **[!UICONTROL Generate Insight]**&#x200B;을(를) 다시 클릭합니다. insight 목록으로 돌아가려면 탐색 표시에서 **[!UICONTROL Analysis List]**&#x200B;을(를) 클릭합니다.

## Insight 설정 {#insight-settings}

### 모델 정확도 {#model-accuracy-settings}

* **[!UICONTROL Portfolios]:** 포트폴리오를 하나 선택하십시오.

* **[!UICONTROL Choose Revenue Type]:** **[!UICONTROL Actual Revenue]**(기본값) 또는 **[!UICONTROL Delayed Revenue]** 선택

* **[!UICONTROL Date Range]:** 분석할 날짜를 선택하십시오. [날짜 범위 설정](#date-range-settings)을 참조하세요.

### 성능 인사이트 {#performance-insights-settings}

* **[!UICONTROL Portfolios]:** 포트폴리오를 하나 선택하십시오.

* **[!UICONTROL Revenue Type]:** **[!UICONTROL Actual Revenue]**(기본값) 또는 **[!UICONTROL Delayed Revenue]** 선택

* **이벤트 날짜:** 성능을 비교할 날짜 유형을 선택하십시오.

  * **[!UICONTROL Optimization Status Change (last 90 days)]**(기본값): 포트폴리오에 사용할 수 있는 최적화 상태 변경 날짜를 선택하십시오.

  * **[!UICONTROL Objective Change Date (last 90 days)]:** 포트폴리오에 사용할 수 있는 목표 변경 날짜를 선택하십시오.

  * **[!UICONTROL Specific Date]:** 날짜 선택기를 사용하여 날짜를 지정합니다.

  비교 기간을 구성하기 전에 이벤트 날짜를 선택합니다. 선택한 포트폴리오에 사용할 수 있는 이벤트 날짜가 없으면 **[!UICONTROL Specific Date]**&#x200B;을(를) 사용할 수 있습니다.

* **[!UICONTROL Pre Days]:** 이벤트 날짜 이전 기간을 지정하십시오.

  * **[!UICONTROL 7]**(기본값), **[!UICONTROL 14]** 또는 **[!UICONTROL 30]**&#x200B;을(를) 선택하십시오.

  * **[!UICONTROL Pre Start Date]**&#x200B;을(를) 선택하고 **[!UICONTROL Custom Pre Date]**&#x200B;을(를) 지정하십시오.

  * **[!UICONTROL Custom Pre Days]**&#x200B;을(를) 선택하고 양수를 입력하십시오.

* **[!UICONTROL Post Days]:** 이벤트 날짜 이후의 기간을 지정합니다.

  * **[!UICONTROL 7]**(기본값), **[!UICONTROL 14]** 또는 **[!UICONTROL 30]**&#x200B;을(를) 선택하십시오.

  * **[!UICONTROL Post End Date]**&#x200B;을(를) 선택하고 **[!UICONTROL Custom Post Date]**&#x200B;을(를) 지정하십시오.

  * **[!UICONTROL Custom Post Days]**&#x200B;을(를) 선택하고 양수를 입력하십시오.

  이벤트 날짜 자체는 두 비교 기간에 포함되지 않습니다.

* **[!UICONTROL Date Exclusion]:**(선택 사항) 분석에서 날짜 제외:

  1. **[!UICONTROL Select Dates]**&#x200B;을(를) 클릭합니다.

  1. 제외할 날짜 선택:

     * 개별 날짜를 클릭하여 선택하거나 선택 취소합니다.

     * 범위를 선택하려면 클릭하여 **[!UICONTROL Shift]**&#x200B;을(를) 길게 누르십시오.

     * 모든 제외를 제거하려면 **[!UICONTROL Clear All]**&#x200B;을(를) 클릭합니다.

  1. 완료되면 **[!UICONTROL Done]**&#x200B;을(를) 클릭합니다.

### Portfolio 시뮬레이션 분석 {#simulation-settings}

* **[!UICONTROL Portfolios]:** 기존 사용자 지정 시뮬레이션을 사용하는 포트폴리오를 하나 선택하십시오.

* **[!UICONTROL Simulation Date]:** 분석할 시뮬레이션 날짜를 선택하십시오. 해당 날짜에 여러 시뮬레이션을 사용할 수 있는 경우 이름별 시뮬레이션을 선택하십시오.

  사용 가능한 사용자 지정 시뮬레이션이 없는 경우 이 insight을 사용하기 전에 [사용자 지정 시뮬레이션을 생성](/help/search-social-commerce/new-ui/manage/portfolios/portfolio-create-simulation.md)하십시오.

* **[!UICONTROL Actual Days]:** **[!UICONTROL 7]**(기본값), **[!UICONTROL 14]** 또는 **[!UICONTROL 30]**&#x200B;일의 실제 성능 데이터를 선택합니다. 다른 숫자를 지정하려면 **[!UICONTROL Enter Actual Days]**&#x200B;을(를) 선택하고 1-90 사이의 값을 입력하십시오.

* **[!UICONTROL Type]:** 전환 속성에 대해 **[!UICONTROL Transaction Date]**(기본값) 또는 **[!UICONTROL Click Date]**&#x200B;을(를) 선택합니다.

### 캠페인 예산 상한 분석 {#budget-cap-settings}

* **[!UICONTROL Portfolio]:** 포트폴리오를 하나 선택하십시오.

* **[!UICONTROL Date Range]:** 분석할 날짜를 선택하십시오. [날짜 범위 설정](#date-range-settings)을 참조하세요.

### 모델 전환 {#modeled-conversions-settings}

* **[!UICONTROL Analysis Level]:** **[!UICONTROL Account]**, **[!UICONTROL Portfolio]**(기본값) 또는 **[!UICONTROL Campaign]**&#x200B;을(를) 선택합니다.

* **[!UICONTROL Accounts]**, **[!UICONTROL Portfolios]** 또는 **[!UICONTROL Campaigns]:** 분석 수준에 적용할 수 있는 엔터티를 선택합니다. 여러 엔티티를 선택할 수 있습니다.

* **[!UICONTROL Date Range]:** 분석할 날짜를 선택하십시오. [날짜 범위 설정](#date-range-settings)을 참조하세요.

* **[!UICONTROL Adobe Conversion]:** 비교할 Adobe 전환 속성을 선택합니다.

* **[!UICONTROL Publisher Conversion]:** 비교할 게시자 전환 속성을 선택합니다.

  사용 가능한 전환 속성은 분석 수준, 선택한 엔티티 및 날짜 범위에 따라 다릅니다. 비교에는 두 전환 속성이 모두 필요합니다.

### 지연된 수익 분석 {#delayed-revenue-settings}

* **[!UICONTROL Portfolios]:** 클릭 기반 또는 뷰스루 매출 기여도 분석이 있는 포트폴리오를 하나 선택하십시오.

* **[!UICONTROL Date Range]:** 분석할 날짜를 선택하십시오. [날짜 범위 설정](#date-range-settings)을 참조하세요.

### 날짜 범위 설정 {#date-range-settings}

**[!UICONTROL Date Range]** 설정이 있는 인사이트의 경우 **[!UICONTROL Last 7 days]**(기본값), **[!UICONTROL Last 14 days]** 또는 **[!UICONTROL Last 30 days]**&#x200B;을(를) 선택하십시오.

다른 기간을 지정하려면 **[!UICONTROL Custom Date]**&#x200B;을(를) 선택하고 **[!UICONTROL Start Date]** 및 **[!UICONTROL End Date]**&#x200B;을(를) 입력하십시오. 현재 날짜부터 지난 90일 이내의 날짜를 선택할 수 있습니다.

## insight 결과 보기 {#insight-results}

### 모델 정확도 {#model-accuracy-results}

포트폴리오 세부 사항을 검토하고 다음 탭을 사용하십시오.

* **[!UICONTROL Portfolio]:** 포트폴리오 수준 모델 정확도 및 예산 비교를 검토합니다.

* **[!UICONTROL Ad Network]:** 광고 네트워크별 모델 정확도 및 예산 비교를 검토합니다.

* **[!UICONTROL Campaigns]:** 캠페인 수준 모델 정확도 및 대상 대 실제 성능을 검토하십시오.

* **[!UICONTROL Playground Beta]:** 여러 캠페인에 대한 모델 정확도를 비교합니다.

캠페인 정확도 차트의 경우 **[!UICONTROL Comparison Options]** 및 **[!UICONTROL Campaign]**&#x200B;을(를) 선택하십시오. **[!UICONTROL Playground Beta]**&#x200B;에서 여러 캠페인을 선택할 수 있습니다. 차트와 기본 데이터 간을 전환하려면 **[!UICONTROL Table View]**&#x200B;을(를) 클릭하십시오.

### 성능 인사이트 {#performance-insights-results}

대시보드에는 **[!UICONTROL Pre Period]** 및 **[!UICONTROL Post Period]**, 두 기간에 대한 집계된 성과 지표 및 포트폴리오 세부 정보가 표시됩니다.

**[!UICONTROL Audit Trail]**&#x200B;은(는) 포트폴리오 예산, 지출 전략, 최소 캠페인 지출 및 지출 제한 다수를 포함하여 최적화에 영향을 주는 요인에 대한 변경 사항을 요약합니다. 변경 내용에 사용 가능한 세부 정보가 있으면 **[!UICONTROL View Details]**&#x200B;을(를) 클릭하여 검사하십시오.

**[!UICONTROL Comparative Overview]**, **[!UICONTROL Campaigns Comparison]**, **[!UICONTROL Trends & Patterns]**, **[!UICONTROL Deep Analysis]** 및 **[!UICONTROL Objective Value And Analysis]** 탭을 사용하여 비교를 살펴보십시오.

### Portfolio 시뮬레이션 분석 {#simulation-results}

시뮬레이션 세부 사항을 검토하고 다음 탭을 사용합니다.

* **[!UICONTROL Portfolio]:** 포트폴리오 수준의 시뮬레이션 데이터를 검토합니다. 이 탭 내:

  * **[!UICONTROL Simulation Data]**&#x200B;은(는) 시뮬레이션 지표와 타겟 지출 성과를 보여 줍니다.

  * **[!UICONTROL Simulation Vs Actual]**&#x200B;이(가) 시뮬레이션된 성능과 실제 성능을 비교합니다.

  * **[!UICONTROL Try New Target]**&#x200B;을(를) 통해 **[!UICONTROL Explore Target Spend]**&#x200B;에 타겟 지출을 입력하여 예상 클릭수, 비용 및 매출을 볼 수 있습니다. 이는 포트폴리오의 지출 목표를 변경하지 않고 예상 성과를 분석하는 것입니다.

* **[!UICONTROL Campaigns]:** 캠페인 수준 시뮬레이션 비교를 검토합니다.

* **[!UICONTROL Accuracy Analysis]:** 시뮬레이션 정확도를 검토합니다.

### 캠페인 예산 상한 분석 {#budget-cap-results}

포트폴리오 세부 정보 및 요약 지표를 검토합니다.

* **[!UICONTROL Total Capped Spend]:** 캠페인 예산이 적중된 날의 지출 비율입니다.

* **[!UICONTROL Capped Campaigns]:** 예산을 한 번 이상 사용한 캠페인 수입니다.

* 예산 한도로 인해 **[!UICONTROL Est. Lost Impressions]:**&#x200B;개의 예상 노출 수가 누락되었습니다.

* **[!UICONTROL Peak Capping Day]:** 사용 한도가 가장 제한된 요일입니다.

**[!UICONTROL Spend on Capped Campaigns by Day]** 및 **[!UICONTROL Capped Spend by Weekday]** 차트는 최대 가용량 트렌드를 보여 줍니다. 캠페인 세부 정보는 **[!UICONTROL Capped Campaign Performance]**&#x200B;을(를), 제안된 설정 변경 사항은 **[!UICONTROL Portfolio Settings Recommendations]**&#x200B;을(를) 검토하십시오.

### 모델 전환 {#modeled-conversions-results}

선택한 엔티티 및 날짜 범위에 대해 다음 표를 검토하십시오.

* **[!UICONTROL Adobe Measured vs Publisher Conversions]:** Adobe에서 직접 측정한 전환 값을 측정 및 모델링된 데이터를 포함하는 게시자가 보고한 값과 비교합니다.

* **[!UICONTROL Adobe Modeled vs Publisher Conversions]:** Adobe 측정 및 모델 전환 값을 게시자가 보고한 값과 비교합니다.

두 테이블 모두 엔티티 이름과 ID, Adobe 값, 게시자가 보고한 값, 절대 차이 및 백분율 차이를 포함합니다.

사용할 수 있는 데이터가 없는 경우 전환 속성을 모두 선택했는지, 선택한 엔티티 및 날짜 범위에 대한 데이터가 있는지 확인합니다.

### 지연된 수익 분석 {#delayed-revenue-results}

**[!UICONTROL Key Insights Summary]**&#x200B;은(는) 예상 가중 매출(이제 &quot;[목표값](/help/search-social-commerce/glossary.md#o-p)&quot;이라고 함), ROI 및 모델 정확도 정보를 보여 줍니다.

**[!UICONTROL Conversion Lag Breakdown by Revenue Property]** 섹션은 각 매출 속성에 대해 0일에 실현된 전환 비율을 3, 7, 14 및 28일별로 보여 줍니다.

**[!UICONTROL Performance Over Time]**&#x200B;에서 **[!UICONTROL Objective Value]**, **[!UICONTROL ROI]** 또는 **[!UICONTROL Model Accuracy]**&#x200B;을(를) 선택하여 클릭 날짜, 트랜잭션 날짜 및 예상 성능을 비교합니다. 차트와 기본 데이터 간을 전환하려면 **[!UICONTROL Table View]**&#x200B;을(를) 클릭하십시오.

**[!UICONTROL Metrics Definitions]**&#x200B;에서 분석에 사용된 날짜 및 지표에 대한 설명을 보려면 **[!UICONTROL Show]**&#x200B;을(를) 클릭하고 축소하려면 **[!UICONTROL Hide]**&#x200B;을(를) 클릭합니다.

분석을 적용할 수 없는 경우 클릭 기반 또는 뷰스루 매출 기여도 분석이 포함된 포트폴리오를 선택하십시오. 사용할 수 있는 데이터가 없는 경우 선택한 포트폴리오 및 날짜 범위에 대한 데이터가 있는지 확인하십시오.
