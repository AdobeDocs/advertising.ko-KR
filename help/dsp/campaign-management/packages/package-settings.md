---
title: 패키지 설정
description: 사용 가능한 패키지 설정에 대한 설명을 참조하십시오.
feature: DSP Packages
exl-id: 20ec5e8e-4980-4fa0-80c9-531f5b02c0f9
source-git-commit: a8227e42c49e30d6b73daf51e4f62da05f6508f3
workflow-type: tm+mt
source-wordcount: '996'
ht-degree: 0%

---

# 패키지 설정

## [!UICONTROL Basic Details]

**[!UICONTROL Name]:** 패키지 이름. 최대 길이는 60자입니다.

**[!UICONTROL Description]:** (선택 사항) 패키지에 대한 설명입니다.

**[!UICONTROL 3rd Party Billed Fees]:** (선택 사항) 청구 불가능한 비용으로 추적할 정적 서드파티 비용:

>[!NOTE]
>
>청구 가능 요금은 다음에 반영됩니다. [!UICONTROL Net CPM] 지표.
>
* **[!UICONTROL CPM]:** 1000회 노출당 비용(CPM).

* **[!UICONTROL CPM Description]:** CPM 요금에 대한 설명.

에서 패키지 수준 설정을 재정의할 수 있습니다. [배치 수준](/help/dsp/campaign-management/placements/placement-settings.md).

## [!UICONTROL Goals & Budget]

**[!UICONTROL Pacing & Capping]:** (기존 패키지의 읽기 전용) 패키지에서 배치 속도 및 상한 수준:

* **[!UICONTROL Package level pacing]:** 이 게재 간격 전략은 포함된 모든 배치를 로 게재 간격 및 캡핑하여 작동합니다. *그룹*. 이 전략을 사용하면 지정된 패키지 내의 모든 배치가 전체적으로 최적화되어 성능과 규모를 기반으로 한 지출을 선택한 주요 성과 지표(KPI)에 분산할 수 있습니다.

* **[!UICONTROL Placement level pacing]:**  이 게재 간격 전략은 포함된 모든 배치의 게재 간격 및 캡핑을 통해 작동합니다 *개별적으로*. 가장 좋은 방법은 이 전략을 사용하여 보장된 프라이빗 마켓 플레이스 거래를 실행하는 것입니다.

**[!UICONTROL Flight Dates]:** 패키지의 전체 시작 날짜 및 종료 날짜입니다. 비행 날짜는 캠페인 비행 날짜 내에 포함되어야 합니다.

>[!NOTE]
>
>* 이 패키지에 할당된 모든 배치에 대한 비행 날짜는 이 날짜 내에 포함되어야 합니다.
> * 사용자 지정 플라이팅이 활성화된 경우 패키지 시작 날짜를 편집할 수 없습니다.

**[!UICONTROL *Activate Custom Flighting]:** 에서 패키지의 비균일 게재 항공편을 만들 수 있습니다. [!UICONTROL Flighting] 아래 섹션. 사용자 정의 조명을 활성화하고 패키지를 저장하면 사용자 정의 조명을 비활성화하거나 패키지 시작 날짜를 편집할 수 없습니다.

**[!UICONTROL Budget]:** (패키지 수준 게재 간격 전용 패키지) 총 예산 상한 및 예산 간격.

사용자 지정 조명이 있는 패키지의 경우 예산 간격은 항상 입니다. *[!UICONTROL All time]*. 사용자 지정 플라이팅이 없는 패키지의 경우 예산 간격을 지정합니다. *[!UICONTROL All time],* *[!UICONTROL Daily],* *[!UICONTROL Monthly],* 또는 *[!UICONTROL Weekly]*.

**[!UICONTROL Gross Budget]:** (패키지 수준 게재 간격 및 동적 마진 관리 전용 패키지) 패키지 기간에 대한 총 예산 상한.

**[!UICONTROL Optimization Goal]:** (패키지 수준 게재 간격 전용 패키지) 패키지에 대한 최적화 목표입니다. 에서 각 최적화 목표에 대한 설명을 참조하십시오. [최적화 목표 및 사용 방법](/help/dsp/optimization/optimization-goals.md).

**[!UICONTROL Custom Goal for Model Learning]:** (가 포함된 패키지)[!UICONTROL Highest Return on Ad Spend]&quot; 및 &quot;[!UICONTROL Lowest Cost per Acquisition]&quot; 최적화 목표만 해당) A [사용자 정의 목표](/help/dsp/optimization/custom-goal.md) 여기에는 CPA 또는 ROAS 지표를 계산하는 데 사용되는 매출 또는 전환 이벤트가 포함됩니다. 사용자 지정 목표에는 패키지 최적화를 위한 CPA 또는 ROAS 지표 외에 사용할 추가 가중치가 적용된 상위 단계 이벤트(예: 페이지 방문 및 장바구니 추가)가 선택적으로 포함될 수 있습니다. 사용자 지정 목표 및 이를 사용하는 캠페인에 대한 모범 사례에 대한 자세한 내용은 다음을 참조하십시오. [사용자 지정 목표 빌드를 위한 우수 사례](/help/dsp/optimization/custom-goal.md#custom-goal-best-practices) 및 [성과 캠페인 설정에 대한 우수 사례](/help/dsp/optimization/campaign-best-practices-performance.md).<!-- At some point, all of the objectives will be prefixed with "ADSP " -->

**[!UICONTROL Consider Only Click Conversions for Model Learning]:** (선택 사항, &quot;가 포함된 패키지[!UICONTROL Highest Return on Ad Spend]&quot; 및 &quot;[!UICONTROL Lowest Cost per Acquisition]&quot; 최적화 목표만 해당) 최적화 모델에 클릭 기반 전환에서만 학습하도록 지시합니다. 그렇지 않으면 최적화 모델이 클릭 및 노출 기반 전환 모두에서 학습합니다.

**[!UICONTROL Conversion Metric]:** (선택 사항, &quot;가 포함된 패키지[!UICONTROL Highest Return on Ad Spend]&quot; 및 &quot;[!UICONTROL Lowest Cost per Acquisition]&quot; 최적화 목표만 해당) 광고 투자 수익률 또는 획득당 비용을 계산하는 데 사용할 최종 전환 이벤트(예: 서명) 또는 매출 이벤트/판매 금액(예: 구매 및 구매 값)입니다. 선택한 사용자 정의 목표에 매핑된 모든 기본 이벤트(&quot;목표 지표&quot;) 목록에서 선택합니다. 목록이 비어 있는 경우 기본 이벤트 중 하나 이상을 목표 지표로 포함하도록 사용자 지정 목표를 편집합니다.

**[!UICONTROL Package Goal Type]:** (사용자 지정 최적화 목표가 있는 패키지만 해당) 패키지의 목적입니다. 이 설정은 패키지를 최적화하는 방법을 결정하는 데 도움이 됩니다.

* *[!UICONTROL Prospecting]:* 잠재 고객 패키지는 신규 고객 확보에 중점을 둡니다.

* *[!UICONTROL Retargeting]:* 패키지 재타겟팅은 이전 방문자 또는 고객을 다시 노출하는 데 중점을 둡니다.

* *[!UICONTROL Other]:* 다른 모든 용도.

**[!UICONTROL Linked Package for Optimization Learnings Carryover]:** (사용자 지정 최적화 목표가 있는 패키지만 해당) 패키지 최적화를 위한 입력으로 내역 데이터가 사용되는 다른 패키지.

**[!UICONTROL Target]:** (패키지 수준 게재 간격 전용 패키지) 성능을 추적하는 데 사용되는 타겟 목표입니다.

>[!NOTE]
>
>이 필드는 벤치마크일 뿐이며 의사 결정에는 사용되지 않습니다.

**[!UICONTROL Frequency Cap]:** (패키지 수준 게재 간격 전용 패키지) 고유 장치, 범용 ID 또는 개인용 횟수(지정된 항목에 따라 다름) [!UICONTROL Cross Device Level] 캠페인 및 배치 [!UICONTROL Targeting] 설정)은 패키지에서 광고를 제공할 수 있습니다. 옵션은 다음과 같습니다 *[!UICONTROL Unlimited]* 또는 일별, 주별, 월별 특정 금액입니다.

>[!NOTE]
>
>* 캠페인, 패키지 및 배치 수준에서 빈도 상한을 설정할 수 있습니다. DSP은 campaign 계층 구조에서 가장 엄격한 빈도 상한을 따릅니다.
>* 가장 좋은 방법은 패키지 수준에서 전망 및 재타겟팅 모두에 대한 빈도 상한을 설정하는 것입니다.
> * 빈도 상한이 높을수록 지출과 노출은 증가하지만 도달 거리는 감소합니다. 빈도 상한이 낮으면 지출과 노출이 줄어들지만 도달 범위가 높아집니다.

**[!UICONTROL Pace on]:** (패키지 수준 게재 간격 전용 패키지) 게재 간격 기준은 다음과 같습니다.

* *[!UICONTROL Budget]:* (기본값) 이 옵션은 할당된 패키지 예산 내에서 가능한 한 많은 노출 횟수를 제공합니다.

* *[!UICONTROL Impressions]:* 이 옵션은 지정된 수량이 지정된 간격 내에 도달할 때까지 노출을 전달합니다. 이 옵션을 선택할 때 노출 횟수와 간격을 지정합니다. *항상,* *[!UICONTROL Daily],* *[!UICONTROL Monthly],* 또는 *[!UICONTROL Weekly]*.

**[!UICONTROL Flight pacing]:** (패키지 수준 게재 간격 전용 패키지) 전체 항공편에서 광고 게재의 속도를 조절하는 방법:

* *[!UICONTROL Even]:* 각 비행 내내 균일하게 배송이 진행되며, 비행 전반부 중 배송의 50%가 목표입니다.

* *[!UICONTROL Slightly Ahead]:* (기본값) 게재를 가속화하여 플라이트 기간 중간에 55~65% 완료됩니다.

* *[!UICONTROL Frontload]:* 배송을 가속화하여 비행 중간에 65~75% 완료.

* *[!UICONTROL Aggressive Frontload]:* 배송을 가속화하여 비행 중간에 75~85% 완료.

**[!UICONTROL Intraday pacing]:** (패키지 수준 게재 속도만 있는 패키지) 비행 내에서 매일 광고 게재의 속도를 조절하는 방법:

* *[!UICONTROL Even]:* (기본값) 재고 가용성에 따라 게재의 배율을 조정합니다. 일반적으로 경매량이 많은 낮에는 시간당 더 많은 광고가 게재되고 아침과 저녁에는 더 적은 수의 광고가 게재된다.

* *[!UICONTROL ASAP]:* 보다 2배 빠른 속도로 게재 *균일*.

  >[!CAUTION]
  >
  >이 옵션은 성능에 부정적인 영향을 줄 수 있습니다. 성능 최적화에 비해 게재 우선 순위 및 비용을 완전히 우선시하는 경우에만 사용하십시오.

## [!UICONTROL Flighting]

(패키지 수준 게재 간격이 있고 &quot;[!UICONTROL Activate Custom Flighting]&quot;활성화됨) 전체 내에서 사용자 정의 플라이트 기간 [!UICONTROL Flight Dates] 다음에 지정됨: [!UICONTROL Goals & Budget] 섹션.

각 항공편에 대해 시작 일자, 종료 일자 및 목표 지출 목표를 입력합니다. 다른 항공편을 추가하려면 **[!UICONTROL Add Flight]**.

기존 패키지의 경우 선택적으로 다음에 값을 입력할 수 있습니다. [!UICONTROL Rollover] 다음 비행에 잠재적 미지출 예산을 추가하기 위한 모든 비행에 대한 열입니다. 의 예상 값 [!UICONTROL Adjusted Goal (Goal + Rollover)] 그에 따라 열이 변경됩니다.<!-- clarify usage -->

>[!MORELIKETHIS]
>
>* [패키지 관리 정보](package-about.md)
>* [패키지 만들기](package-create.md)
>* [패키지 편집](package-edit.md)
>* [패키지에 배치 첨부](package-attach-placement.md)
>* [패키지에 대한 변경 로그 보기](package-change-log.md)
>* [Campaign Management에 대한 FAQ](/help/dsp/campaign-management/faq-campaign-management.md)
