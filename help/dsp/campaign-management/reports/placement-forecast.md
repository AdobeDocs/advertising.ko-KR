---
title: 배치 예측 보고서 보기
description: 배치에 대한 특정 타겟팅 전략에 대해 예측된 노출 횟수, 지출 횟수 및 최적 최대 입찰가 를 참조하십시오.
feature: DSP Placements
exl-id: 6ff228b2-b656-493e-a299-98c7a68a0f51
source-git-commit: 1ac58da2d538cc682161ebc944a0412ad4a8af17
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# 배치 예측 보고서 보기

<!-- Does this really belong in the Campaign Management > Reports section or in the Placements section? -->

배치 예측 도구는 특정 타겟팅 전략에 대해 예측된 노출 횟수, 지출 횟수 및 최적의 최대 입찰가를 보여 줍니다. 예측은 배치와 함께 사용할 수 있는 전체 인벤토리와 사용 가능한 고유 사용자를 기반으로 계산됩니다.

>[!NOTE]
>
>* 가용성과 지출이 결정적이기 때문에 프로그램 보증(PG) 타깃팅만 있는 배치에 대한 예측이 생성되지 않습니다.

## Forecast 의 정보

예측에는 다음 정보가 포함됩니다.

* **[!UICONTROL Summary]:**

   * **[!UICONTROL Estimated CPM]:** 타겟팅 설정에 도달할 것으로 예상되는 노출 횟수당 예상 비용(eCPM).

   * **[!UICONTROL Budget]:** 타겟팅 설정에 대한 예상 예산.

   * **[!UICONTROL Impression]:** 타겟팅 설정에 대한 예상 노출 횟수입니다.

* **[!UICONTROL Budget Yield Curve]:** 다른 모든 타겟팅 설정이 동일한 경우 배치가 다른 예산 수준에서 제공할 수 있는 예상 노출 횟수입니다.

* **[!UICONTROL Max Bid Yield Curve]:** 다른 모든 타깃팅 설정이 동일할 때 서로 다른 최대 입찰 수준에서 배치에 대한 예상 지출입니다.

* **[!UICONTROL Message]:** 예측을 생성할 수 없는 시나리오를 포함하여 예측된 출력에 대한 정보를 제공합니다. 또한 검토되었지만 데이터 부족으로 인해 해당 시나리오에서 고려되지 않은 모든 타겟팅 설정을 강조 표시합니다.

### 예산 계산

* 패키지에 할당되지 않은 배치의 경우, 배치 예산이 계산에 사용됩니다. 비행 내에서 동일한 전체 예산이 계산됩니다.

* 패키지 내의 배치의 경우 배치에 지정된 예산이 계산에 사용됩니다. 비행 중 배치에 할당된 예산이 계산되고 메시지에 포함됩니다.

* 진행 중인 패키지에 추가된 배치의 경우 배치 수에 따라 예산이 균등하게 분할됩니다. 배치가 실행되면 패키지에서 할당한 예산이 계산됩니다.

## 요구 사항

* 최소 지출: 일일 $25 또는 배치당 현지 통화로 이에 해당합니다.

* 최대 지출: 일일 $15,000 또는 배치당 현지 통화로 이에 해당합니다.

* 최소 최대 입찰, 최대 입찰: 배치 유형별로 최소 최대 입찰(예산 수익률 곡선의 경우) 및 최대 입찰(최대 입찰 수익률 곡선의 경우)이 있습니다. 이러한 값은 전역적으로 true이며 지역 변형을 고려하지 않습니다. 때때로, 이러한 값들은 타겟팅된 영역에 대해 너무 높거나 낮을 수 있다.

* 내역 데이터: 충분한 내역 데이터를 사용할 수 있을 때 배치 예측을 사용할 수 있습니다. 다음은 충분하지 않은 내역 데이터를 사용할 수 있는 경우의 예입니다.

   * 배치는 캠페인의 새 영역을 타겟팅합니다.

   * 배치는 캠페인에 대한 새로운 인벤토리 거래를 타깃팅합니다.

   * 배치는 캠페인에 새 광고 유형을 사용합니다.

     배치는 일반적으로 공급측 플랫폼에 정의된 여러 광고 템플릿의 컬렉션입니다. 따라서 배치가 오래 존재하더라도 기본 광고 템플릿이 새로 생성될 수 있으며 예측 도구는 예측할 수 없습니다.

## 배치 예측 보고서 열기

1. 메인 메뉴에서 **[!UICONTROL Campaigns]**.

1. 캠페인 이름을 클릭한 다음 **[!UICONTROL Placements]**.

1. 배치 이름 옆에 있는 를 클릭합니다  **[!UICONTROL ...]** > **[!UICONTROL Edit]**.

1. 를 찾습니다. **[!UICONTROL Forecast]** 오른쪽 상단에 있는 섹션입니다. 필요한 경우 ![예측](/help/dsp/assets/placement-forecast.png).

   >[!NOTE]
   >
   >* 브라우저 캐시로 인해 예측을 사용할 수 없는 경우가 있습니다. 이 경우 캐시를 지우고 다시 시도하십시오.

>[!MORELIKETHIS]
>
>* [Campaign Management 보기의 성능 보고서 유형](campaign-reports-about.md)
>* [배치 진단 보고서 보기](/help/dsp/campaign-management/reports/placement-diagnostics.md)
>* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)
