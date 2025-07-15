---
title: (새 UI) 포트폴리오 성능 세부 정보 보기
description: 포트폴리오 수준 및 할당된 각 캠페인에 대한 실제 및 예상 지표를 포함하여 포트폴리오 성과 세부 정보를 보는 방법에 대해 알아봅니다.
feature: Search Portfolios, Search Optimization
hide: true
source-git-commit: 62de95d7e3d21ae6c7f0a6f40e97352af71411e1
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 0%

---

# (새 UI) 포트폴리오 성능 세부 정보 보기

*Beta 기능*

<!-- Verify all, including why (if) the first report is for active and optimized portfolios(?), and why the other reports are for active portfolios, not optimized ones -->

포트폴리오 세부 사항 보기에는 포트폴리오에 대한 다음 정보가 포함됩니다.

* 최대 3개의 성능 지표에 대한 실제 및 예측 값입니다. 보고서에는 포트폴리오의 총 지표 값 및 날짜별 지표 분류가 포함됩니다.<!-- Not for active portfolios only?  -->

* 모델이 예측에서 얼마나 이탈했는지 보여 주는 활성 포트폴리오의 모델 정확도 데이터입니다. 이 보고서는 전반적인 일일 또는 순환 7일 비용 정확도, 클릭 정확도 및 목표 값 정확도를 보여줍니다.

  클릭 날짜(기본값) 또는 트랜잭션 날짜별로 데이터를 볼 수 있습니다.   데이터를 추세 차트(기본값) 또는 표로 볼 수도 있습니다.

* 타겟 지출과 활성 포트폴리오의 실제 지출. 포트폴리오에 대한 총 캠페인 예산을 선택적으로 포함할 수도 있습니다.

* 광고 네트워크별 활성 포트폴리오에 대한 비용, 클릭 또는 [목표 값](/help/search-social-commerce/glossary.md#o-p) 예측의 정확성.<!-- Verify -->

* 포트폴리오 설정입니다.

  선택적으로 포트폴리오 설정을 열어 편집할 수 있습니다.

## 포트폴리오에 대한 성과 세부 정보 열기

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Portfolios]**&#x200B;을(를) 클릭합니다.

1. 포트폴리오 이름을 클릭합니다.

1. (선택 사항) **[!UICONTROL Granularity]** 메뉴에서 *[!UICONTROL Daily],* *[!UICONTROL Weekly],* 또는 *[!UICONTROL Monthly]사이의 데이터 세부 기간을 변경합니다.*

1. (선택 사항) 포트폴리오 세부 정보에 대한 날짜 범위를 변경하려면 오른쪽 상단의 날짜 범위를 클릭하고 날짜 범위를 지정한 다음 **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

## [!UICONTROL Portfolio Overview] 탭 사용자 지정

* (선택 사항) [!UICONTROL Portfolio Performance] 보고서를 사용자 지정하려면 다음 중 하나를 수행합니다.

   * 총 지표와 세부 지표 모두에 사용되는 성능 지표를 변경하려면 **[!UICONTROL Metrics]**&#x200B;을(를) 클릭하고 최대 3개의 지표를 선택하십시오.

     기본 지표는 *[!UICONTROL Cost]*, *[!UICONTROL Clicks]* 및 *[!UICONTROL Objective Value]*.<!-- What else is available: the advertiser's revenue metrics? Anything else from the ad networks? -->입니다.

   * 세부 지표의 경우:

      * 예측된 지표 값을 표시하거나 숨기려면 **[!UICONTROL Display predictions]** 옆으로 스위치를 이동하십시오.

      * 차트 보기(![차트 보기](/help/search-social-commerce/assets/chart-view.png "차트 보기"))와 테이블 보기(![표 보기](/help/search-social-commerce/assets/table-view.png "표 보기")) 간을 전환합니다.

      * (차트 보기에서) 차트의 임의 지점에 대한 데이터를 보려면 해당 지점 위에 커서를 놓습니다.

* (선택 사항) [!UICONTROL Model accuracy] 트렌드 차트를 사용자 지정하려면 다음 중 하나를 수행하십시오.

   * 차트 보기(![차트 보기](/help/search-social-commerce/assets/chart-view.png "차트 보기"))와 테이블 보기(![표 보기](/help/search-social-commerce/assets/table-view.png "표 보기")) 간을 전환합니다.

   * *[!UICONTROL Click Date]*&#x200B;과(와) *[!UICONTROL Transaction Date]*&#x200B;의 데이터 보기 간에 전환합니다.

   * *[!UICONTROL Daily Accuracy]*&#x200B;과(와) *[!UICONTROL 7 Day Rolling Accuracy]*&#x200B;에 대한 데이터 보기 간에 전환합니다.

     [!UICONTROL 7 Day Rolling Accuracy]은(는) 이전 7일 동안의 평균 예측 정확도로 백분율로 표시됩니다. 예를 들어, 2025년 5월 8일 값은 2025년 5월 1일 - 7일 기간에 대한 평균 정확도입니다.

   * (차트 보기에서) 차트의 임의 지점에 대한 데이터를 보려면 해당 지점 위에 커서를 놓습니다.

* (선택 사항) [!UICONTROL Target vs actual spend] 트렌드 차트를 사용자 지정하려면 다음 중 하나를 수행하십시오.

   * **[!UICONTROL Display budget]** 옆으로 스위치를 이동하여 각 날짜에 대한 총 캠페인 예산을 표시하거나 숨깁니다.

   * 차트에서 임의의 점에 대한 데이터를 보려면 해당 점 위에 커서를 놓습니다.

* (선택 사항) [!UICONTROL Network Accuracy] 트렌드 차트를 사용자 지정하려면 다음 중 하나를 수행하십시오.

   * 보고된 지표를 *[!UICONTROL Cost]*, *[!UICONTROL Clicks]* 또는 *[!UICONTROL Objective Value]*(으)로 변경하십시오.

   * 차트에서 임의의 점에 대한 데이터를 보려면 해당 점 위에 커서를 놓습니다.

## 포트폴리오에 캠페인 나열

* **[!UICONTROL Campaigns]** 탭을 클릭합니다.

## 포트폴리오의 광고 그룹 나열

* 포트폴리오 내의 캠페인에 있는 모든 광고 그룹을 보려면 **[!UICONTROL Campaigns]** 탭을 클릭한 다음 캠페인 이름을 클릭합니다.

## 포트폴리오의 키워드 나열

* 포트폴리오의 모든 키워드를 보려면 **[!UICONTROL Keywords]** 탭을 클릭하십시오.

* 포트폴리오 내의 광고 그룹에 있는 모든 키워드를 보려면 **[!UICONTROL Ad Groups]** 탭을 클릭한 다음 광고 그룹 이름을 클릭합니다.

## 포트폴리오 설정 보기 및 편집

* 포트폴리오 설정을 보거나 숨기려면 **[!UICONTROL Portfolio Settings]**&#x200B;을(를) 클릭합니다.

   * 표시되는 포트폴리오 설정을 편집하려면 설정 섹션 옆에 있는 ![편집](/help/search-social-commerce/assets/edit.png "편집")을 클릭하고 [포트폴리오 설정 편집](portfolio-edit.md)을 클릭합니다.

포트폴리오 설정에 대한 자세한 내용은 Search, Social 및 Commerce 내에서 사용할 수 있는 최적화 안내서를 참조하십시오.

>[!MORELIKETHIS]
>
>* 포트폴리오에 대한 [(새 UI)](portfolio-about.md)
>* [(새 UI) 포트폴리오 편집](portfolio-edit.md)
>* [(새 UI) [!UICONTROL Portfolios] 보기에서 데이터를 다운로드합니다](portfolio-view-report.md)
