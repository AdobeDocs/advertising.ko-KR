---
title: (새 UI) 포트폴리오 정보
description: 포트폴리오에 대해 알아봅니다.
feature: Search Portfolios, Search Optimization
hide: true
exl-id: 8d023c22-a1dd-4608-8c72-0a61f055e7e5
source-git-commit: f7c63646b3eae20fd3413446789fe06ce583e23e
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 0%

---

# (새 UI) 포트폴리오 정보

*Beta 기능*

포트폴리오(투자 포트폴리오와 유사)를 사용하여 광고 캠페인을 일괄적으로 관리할 수 있습니다. 포트폴리오는 연결된 키워드 및 광고를 포함하여 단일 비즈니스 목표에 최적화된 광고 캠페인 또는 광고 세트 세트입니다. 목표에는 여러 가중 전환과 단일 예산 또는 성과 목표(예: 월별 예산 또는 목표 ROI)가 포함될 수 있습니다. 개별 캠페인/광고 세트, 키워드 및 광고는 서로 다르게 수행할 수 있으므로(예를 들어, 서로 다른 금액을 지출하거나 다른 ROI를 달성할 수 있음), 최적화 기능은 AI 기반 모델을 사용하여 전체 포트폴리오를 제어하여 목표를 전체적으로 달성할 수 있습니다. 포트폴리오의 모든 캠페인은 동일한 통화를 사용합니다.

일부 사용자 역할은 포트폴리오를 만들고 구성할 수 있습니다. 포트폴리오 유형에 따라 포트폴리오 설정에는 포트폴리오 목표, 할당된 캠페인, 지출 전략, 포트폴리오 수준의 입찰 제한 및 모델링 및 최적화 매개변수가 포함될 수 있습니다. 검색, 소셜 및 Commerce에서 포트폴리오 최적화를 시작할 준비가 되면 상태를 &quot;최적화됨&quot;으로 변경합니다.

포트폴리오를 [포트폴리오 그룹](portfolio-group-manage.md)(으)로 그룹화하여 전체 그룹에 대한 복합 데이터를 볼 수 있습니다(선택 사항).

역할에 따라 예측 모델링을 사용하여 최적의 지출 포인트와 상세 예측 정확도 보고서를 식별하는 성능 시뮬레이션을 생성할 수 있습니다.<!-- Mention this now? In addition, all users can use the Spend Recommendation Tool to identify the optimal budget distribution across portfolios. -->

## 입찰 전략별 최적화 지원 {#optimization-by-bid-strategy}

캠페인은 캠페인 또는 광고 그룹 입찰 전략에 따라 최적화할 수 있습니다.

>[!NOTE]
>
>&#39;스마트 입찰&#39;과 &#39;자동화 입찰&#39;이 혼용되는 경우가 많지만 같은 일은 아니다. 스마트 입찰은 경매 시간 입찰을 사용하는 [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 자동화된 입찰 전략만 참조합니다. 즉, 광고 네트워크는 각 경매 시 전환 또는 전환 값을 최적화합니다.

<!-- Add "Frequency of Bidding (or other actions, like adjusting campaign budget or bid adjustment values?) -->

| 입찰 전략 | 스마트 입찰? | 키워드/제품 그룹 수준의 입찰 | 지원 수준 | 목표 유형 | 입찰 단위 | Adobe은 무엇을 설정합니까? | 광고 네트워크는 무엇을 설정합니까? |
|---|---|---|---|---|---|---|---|
| 수동 CPC([!DNL Google Ads] 전용 옵션) | — | 예 | 만들기, 편집, 최적화 | 가중치 값이 있는 단일 또는 다중 속성 목표 | 키워드 + 일치 유형 + 캠페인 | 키워드 입찰, 캠페인 예산, 입찰 조정 값 | 해당 사항 없음 |
| ECPC(향상된 CPC) | 예 | 예 | 만들기, 편집, 최적화 | 가중치 값이 있는 단일 또는 다중 속성 목표 | 키워드 + 일치 유형 + 캠페인 | 키워드 입찰, 캠페인 예산 | 실시간으로 입찰 조정 |
| 클릭 수 최대화[^1] | — | — | 만들기, 편집, 최적화 | 없음, 클릭으로만 최적화 | 캠페인 | 캠페인 예산 | 실시간으로 입찰가를 조정하여 예산 내에서 클릭 수를 최대화합니다. |
| 전환 최대화<br>(TCPA 포함 또는 제외) | 예 | — | 만들기, 편집, 최적화 | 가중치 1을 사용하는 단일 속성 목표 | 캠페인 또는 광고 그룹([!DNL Google Ads])<br>캠페인만([!DNL Microsoft Advertising]) | 캠페인 예산, 설정된 경우 Target CPA<br>TCPA는 [!DNL Microsoft Advertising]에서 독립 실행형 입찰 전략일 수 있음) | 실시간으로 입찰을 조정하여 예산 내에서 주문/리드를 최대화하고, 대상이 설정될 때 CPA 목표를 충족합니다. |
| 전환 값 <br> 최대화(TROAS 포함 또는 제외) | 예 | — | 만들기, 편집, 최적화 | 가중치 값이 있는 다중 속성 목표 또는 가중치 값이 1보다 큰 단일 속성 목표(통화 값을 나타냄) | 캠페인 또는 광고 그룹([!DNL Google Ads])<br>캠페인만([!DNL Microsoft Advertising]) | 캠페인 예산, 설정된 경우 타겟 ROAS<br>TROAS는 [!DNL Microsoft Advertising]에서 독립형 입찰 전략일 수 있음) | 실시간으로 입찰을 조정하여 예산 내에서 수익/이익을 극대화하고, 대상이 설정될 때 ROAS 목표를 충족합니다. |
| 타겟 노출 점유율 | — | — | 만들기, 편집 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 - 포트폴리오에 할당할 수 없음 | 노출 점유율 목표를 충족하도록 입찰을 실시간으로 조정 |

[^1]: 광고 네트워크의 [!UICONTROL Maximize Clicks] 입찰 전략 설정이 Search, Social 및 Commerce 목표 [!UICONTROL Maximize Clicks]과(와) 다릅니다. 입찰 전략이 [!UICONTROL Maximize Clicks]인 경우 키워드 수준의 최적화가 있는 포트폴리오가 아니라 캠페인 수준 또는 광고 그룹 수준의 최적화가 있는 포트폴리오에만 지정해야 합니다.

## Portfolio 상태 {#portfolio-status}

포트폴리오의 상태는 다음과 같습니다.

<!-- **Link to include file for "Portfolio status"** -->

{{$include /help/_includes/search-portfolio-status.md}}

## [!UICONTROL Portfolios] 보기

[!UICONTROL Portfolios] 보기는 사용자 지정 가능한 성능 데이터와 함께 기존 포트폴리오를 나열합니다. [보기 내의 열을 사용자 지정하고](/help/search-social-commerce/common-tasks/data-views/custom-default-views-manage.md) 도구 모음[ 또는 ](/help/search-social-commerce/common-tasks/data-views/ad-hoc-settings/column-filter-apply-from-toolbar.md)열 제목[에서 특정 포트폴리오 ](/help/search-social-commerce/common-tasks/data-views/ad-hoc-settings/column-filter-apply-from-column-heading.md)을(를) 포함하도록 데이터를 필터링할 수 있습니다.

<!-- No options yet to edit anything within the grid, view bid changes, add a portfolio to a portfolio group, edit the Target column, or import/export DOW targets. -->

### 사용 가능한 작업

<!-- Update with any new options -->

<!-- within row:
* [Rename a portfolio](portfolio-rename.md)

* [View the constraints for a portfolio](portfolio-view-constraint.md)

* [View the change history for a portfolio](portfolio-view-change-history.md)
-->

* [포트폴리오 만들기](portfolio-create.md)

* [포트폴리오 복제](portfolio-duplicate.md)

* [포트폴리오 설정 편집](portfolio-edit.md)

* [일괄 시트 파일을 사용하여 포트폴리오 설정 일괄 편집](portfolio-bulksheets.md)

* [포트폴리오 성능 세부 정보 보기](portfolio-details.md)

* [[!UICONTROL Portfolios] 보기에서 데이터 다운로드](portfolio-view-report.md)

>[!MORELIKETHIS]
>
>* [포트폴리오 만들기](portfolio-create.md)
>* [포트폴리오 복제](portfolio-duplicate.md)
>* [포트폴리오 편집](portfolio-edit.md)
>* [[!UICONTROL Portfolios] 보기에서 데이터 보기 보고서 관리](portfolio-view-report.md)
