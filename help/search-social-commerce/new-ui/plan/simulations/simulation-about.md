---
title: 시뮬레이션 정보
description: 포트폴리오 시뮬레이션에 대해 알아봅니다.
feature: Search Optimization, Search Portfolios, Search Simulations
hide: true
source-git-commit: 62de95d7e3d21ae6c7f0a6f40e97352af71411e1
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 0%

---

# 시뮬레이션 정보

*Beta 기능*

시뮬레이션 보고서는 다양한 지출 수준(비용)과 해당 일별 예산 또는 기타 타겟에서 포트폴리오에 대해 예상할 수 있는 예상 한계 비용-목표 값, 비용, 클릭 수 및 목표 값을 보여 줍니다. 선택적으로 <!-- add link --> 보기를 사용자 지정하여 추가 트래픽 지표, 시뮬레이션 설정 및 특정 시뮬레이션 유형([!UICONTROL Weekly] 또는 [!UICONTROL Custom])만 볼 수 있습니다.

<!-- Not available as of 6/21/25:
When the portfolio has a daily budget, you can optionally change the portfolio's spend target to any of the spend targets listed in the simulation.
-->

## 시뮬레이션 유형

* **자동화된 주간 시뮬레이션:** 현재 포트폴리오 설정을 사용하여 매주 시뮬레이션 보고서가 자동으로 실행됩니다. 자동 주간 시뮬레이션은 포트폴리오가 [최적화 또는 활성](/help/search-social-commerce/new-ui/manage/portfolios/portfolio-about.md)인 기간에만 사용할 수 있습니다.

  다운로드한 각 주간 시뮬레이션은 하나의 통합 문서로 구성됩니다. 각 워크북에는 20개 단계 레벨 각각에 대한 목표와 해당 목표를 기준으로 목표에 포함된 예상 비용, 클릭 수, 가중 수익(객관적 값) 및 전환 지표가 포함되어 있습니다. 처음 20개 데이터 행의 경우 제한이 적용되지 않고 나머지 데이터 행의 경우 제한이 적용되었습니다.

* **사용자 지정, 사용자가 생성한 시뮬레이션:** 현재 포트폴리오 설정 또는 사용자 지정 포트폴리오 설정을 사용하여 단일 [최적화 또는 활성](/help/search-social-commerce/new-ui/manage/portfolios/portfolio-about.md) 포트폴리오에 대한 사용자 지정 시뮬레이션 보고서를 만들어 해당 설정이 실제로 변경하지 않고 결과를 확인할 수 있습니다. 예를 들어 사용자 지정 시뮬레이션을 만들어 다른 지출 전략이나 학습 예산<!-- Not available yet:  , or without considering active constraints on bid units in the portfolio-->을 사용하는 효과를 볼 수 있습니다. 포트폴리오, 캠페인, 입찰 단위 및 장치 수준에서 예상 성과를 볼 수 있습니다. 사용자 지정 시뮬레이션은 포트폴리오의 제한 지출 설정을 상속합니다.

  >[!NOTE]
  >
  > 새 사용자 정의 시뮬레이션 양식은 레거시 양식과 동일한 설정을 사용하지만, 포트폴리오 설정에서 입찰 단위 제한 정보를 상속합니다. 이전 사용자 정의 시뮬레이션 설정 페이지에서 수행한 것처럼 입찰 단위 제한을 무시할 수 있는 옵션이 없습니다.

  다운로드한 각 사용자 정의 시뮬레이션은 하나의 통합 문서로 구성됩니다. 각 통합 문서에는 지정된 각 엔티티 시뮬레이션 수준(포트폴리오, 캠페인, 광고 그룹, 입찰 단위)에 대한 워크시트가 하나씩 포함되어 있습니다. 장치 수준 데이터를 지정하면 각 워크시트에 [!UICONTROL Device] 열이 포함됩니다. 각 워크시트에는 적용 가능한 각 엔티티에 대한 데이터와 20개의 각 단계에 대한 장치 유형(예: 캠페인당 행 1개)이 포함된 행이 있습니다. 각 행의 데이터에는 예상 매출 대비 한계 비용, 비용, 클릭 수, 가중 매출(객관적 값), 장치 유형 및 해당 목표를 기반으로 목표에 포함된 전환 지표가 포함됩니다. 포트폴리오 수준 워크시트에는 단계 수준에 대한 대상도 포함되며 엔티티 수준 워크시트에는 광고 네트워크, 계정, 캠페인 및 (해당되는 경우) 광고 그룹이 포함됩니다.   <!-- I don't see a Bid Units tab when specified; clarify when it is and isn't included -->

## [!UICONTROL Simulations] 보기

[!UICONTROL Simulations] 보기에는 주별 시뮬레이션 및 사용자 지정 시뮬레이션이 나열됩니다. 관리자 및 일부 다른 사용자 형식<!-- Verify which -->은(는) 다른 사용자가 만든 사용자 지정 시뮬레이션을 볼 수 있습니다. 다른 모든 사용자는 자신이 만든 사용자 지정 시뮬레이션만 볼 수 있습니다.

데이터 테이블에는 각 시뮬레이션의 진행 상황, 각 행에 대해 채워진 [!UICONTROL Target Midpoint] 열, 비용/노출/클릭/목표 값 예측, 실제 값 및 정확도에 대한 열이 포함되어 있습니다. 선택적으로 추가 사용자 정의 열(실제 목표 값을 원가로 나눈 값과 같은 상승도 지표 포함)을 추가할 수 있습니다.

### 사용 가능한 작업 {#simulations-actions}

* [보기를 사용자 지정](/help/search-social-commerce/common-tasks/data-views/custom-default-views-manage.md)하여 예상 노출수, 실제 비용, 클릭 수, 노출수 및 목표 값, 비용 대비 목표 값, 비용 정확도, 클릭 정확도 및 목표 값 정확도, 예측 및 실제 목표 값과 비용 대비 목표 값의 차이(델타)를 포함한 추가 지표를 포함합니다. 대부분의 시뮬레이션 설정 및 시뮬레이션 유형([!UICONTROL Custom] 또는 [!UICONTROL Weekly])에 대한 열을 포함할 수도 있습니다.

* 단일 포트폴리오에 대해 [사용자 지정 시뮬레이션을 생성하거나 다시 실행합니다](simulation-create.md). 새 시뮬레이션을 생성하거나 목록에서 기존 시뮬레이션을 재생성할 수 있습니다.

* ZIP 파일에서 [주별 및 사용자 지정 시뮬레이션 다운로드](simulation-download.md)를 [!DNL Microsoft Excel] 통합 문서로 사용합니다.

* [!UICONTROL Spend Planner] 단추를 사용하여 포트폴리오에서 최적의 지출 분포를 식별하는 데 도움이 되는 레거시 지출 권장 사항 도구를 엽니다.

## 우수 사례

다음 상황에서 시뮬레이션 보고서를 모니터링합니다.

* 포트폴리오를 시작하여 해당 포트폴리오 설정으로 예상할 수 있는 성과를 추정하기 전에 최소 2주의 데이터를 사용하십시오. 포함된 캠페인에 대한 내역 데이터를 기반으로 시뮬레이션 결과가 예상보다 낮은 성과를 나타내는 경우 포트폴리오를 시작하기 전에 문제를 조사 및 해결하십시오.

* 캠페인 추가 또는 목표 변경과 같이 포트폴리오가 주요 변경 후. 포트폴리오의 모델링 시작 날짜, 전환 지표의 가중치 또는 목표의 클릭 값을 변경하는 경우 업데이트된 비용 및 수익 모델을 사용할 수 있는 경우 다음 날 17:00 PST 이후까지 기다린 후 시뮬레이션을 실행하십시오.

* 정기적으로 전환 지표 수준에서 성능 트렌드를 모니터링합니다.

>[!MORELIKETHIS]
>
>* [시뮬레이션 실행 또는 다시 실행](simulation-create.md)
>* [시뮬레이션 다운로드](simulation-download.md)
