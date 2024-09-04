---
title: 패키지 설정
description: 사용 가능한 패키지 설정에 대한 설명을 참조하십시오.
feature: DSP Packages
exl-id: 20ec5e8e-4980-4fa0-80c9-531f5b02c0f9
source-git-commit: c1967636a762379f1daafb52cfe57dd0122b0748
workflow-type: tm+mt
source-wordcount: '1088'
ht-degree: 0%

---

# 패키지 설정

## [!UICONTROL Basic Details]

**[!UICONTROL Name]:** 패키지 이름입니다. 최대 길이는 60자입니다.

**[!UICONTROL Description]:**(선택 사항) 패키지에 대한 설명입니다.

**[!UICONTROL 3rd Party Billed Fees]:** (선택 사항) 청구 불가능한 비용으로 추적할 정적 타사 수수료:

* **[!UICONTROL CPM]:** CPM(1000회 노출당 비용.

* **[!UICONTROL Description]:** CPM 요금에 대한 설명입니다.

>[!NOTE]
>
>청구 가능 요금은 [!UICONTROL Net CPM] 지표에 반영됩니다.

[배치 수준](/help/dsp/campaign-management/placements/placement-settings.md)에서 패키지 수준 설정을 재정의할 수 있습니다.

## [!UICONTROL Goals & Budget]

**[!UICONTROL Pacing & Capping]:**(기존 패키지의 경우 읽기 전용) 패키지 배치 수준:

* **[!UICONTROL Package level pacing]:** 이 게재 간격 전략은 포함된 모든 배치를 *그룹*(으)로 게재 간격 및 캡핑하는 방식으로 작동합니다. 이 전략을 사용하면 지정된 패키지 내의 모든 배치가 전체적으로 최적화되어 성능과 규모를 기반으로 한 지출을 선택한 주요 성과 지표(KPI)에 분산할 수 있습니다.

* **[!UICONTROL Placement level pacing]:** 이 게재 간격 전략은 포함된 모든 배치 *개별적으로*&#x200B;의 게재 간격 및 제한을 설정하여 작동합니다. 가장 좋은 방법은 이 전략을 사용하여 보장된 프라이빗 마켓 플레이스 거래를 실행하는 것입니다.

**[!UICONTROL Flight Dates]:** 패키지의 전체 시작 날짜와 종료 날짜입니다. 비행 날짜는 캠페인 비행 날짜 내에 포함되어야 합니다.

>[!NOTE]
>
>* 이 패키지에 할당된 모든 배치에 대한 비행 날짜는 이 날짜 내에 포함되어야 합니다.
> * 사용자 지정 플라이팅이 활성화된 경우 패키지 시작 날짜를 편집할 수 없습니다.

**[!UICONTROL Activate Custom Flighting]:** 아래 [!UICONTROL Flighting] 섹션에서 패키지의 비균일 게재 간격을 만들 수 있습니다. 사용자 정의 조명을 활성화하고 패키지를 저장하면 사용자 정의 조명을 비활성화하거나 패키지 시작 날짜를 편집할 수 없습니다.

**[!UICONTROL Budget]:**(패키지 수준 게재 간격 전용 패키지) 총 예산 상한 및 예산 간격.

사용자 지정 조명이 있는 패키지의 경우 예산 간격은 항상 *[!UICONTROL All time]*&#x200B;입니다. 사용자 지정 확인이 없는 패키지의 경우 예산 간격: *[!UICONTROL All time],* *[!UICONTROL Daily],* *[!UICONTROL Monthly],* 또는 *[!UICONTROL Weekly]*&#x200B;을(를) 지정하십시오.

**[!UICONTROL Gross Budget]:**(패키지 수준 게재 간격 및 동적 마진 관리 전용 패키지) 패키지 기간에 대한 총 예산 상한.

**[!UICONTROL Optimization Goal]:**(패키지 수준 간격 지정 전용 패키지) 패키지의 최적화 목표입니다. [최적화 목표 및 사용 방법](/help/dsp/optimization/optimization-goals.md)에서 각 최적화 목표에 대한 설명을 참조하십시오.


**[!UICONTROL Link PG Placements for Incremental Reach Optimization]:**(패키지 수준 게재 간격, &quot;[!UICONTROL Always Max Bid & Maximize Reach]&quot; 및 &quot;[!UICONTROL Lowest Cost per Reach]&quot; 최적화 목표만 있는 패키지) 캠페인에서 프로그래밍 방식으로 보장된 모든 배치의 가구 도달 데이터를 사용하여 증분 도달 속도를 최적화합니다.

**[!UICONTROL Custom Goal for Model Learning]:**(&quot;[!UICONTROL Highest Return on Ad Spend]&quot; 및 &quot;[!UICONTROL Lowest Cost per Acquisition]&quot; 최적화 목표만 있는 패키지) CPA 또는 ROAS 지표를 계산하는 데 사용되는 매출 또는 전환 이벤트가 포함된 [사용자 지정 목표](/help/dsp/optimization/custom-goal.md). 사용자 지정 목표에는 패키지 최적화를 위한 CPA 또는 ROAS 지표 외에 사용할 추가 가중치가 적용된 상위 단계 이벤트(예: 페이지 방문 및 장바구니 추가)가 선택적으로 포함될 수 있습니다. 사용자 지정 목표 및 이를 사용하는 캠페인에 대한 생성 모범 사례를 포함하여 사용자 지정 목표에 대한 자세한 내용은 &quot;[사용자 지정 목표](/help/dsp/optimization/custom-goal.md)&quot; 및 &quot;[성능 캠페인 설정에 대한 모범 사례](/help/dsp/optimization/campaign-best-practices-performance.md)&quot;를 참조하십시오.<!-- At some point, all of the objectives will be prefixed with "ADSP_," but probably that won't show up in the Custom Goal list in the DSP UI. -->

**[!UICONTROL Consider Only Click Conversions for Model Learning]:**(선택 사항, 최적화 목표가 &quot;[!UICONTROL Highest Return on Ad Spend]&quot; 및 &quot;[!UICONTROL Lowest Cost per Acquisition]&quot;인 패키지 전용) 최적화 모델에 클릭 기반 전환에서만 학습하도록 지시합니다. 그렇지 않으면 최적화 모델이 클릭 및 노출 기반 전환 모두에서 학습합니다.

**[!UICONTROL Conversion Metric]:**(선택 사항; &quot;[!UICONTROL Highest Return on Ad Spend]&quot; 및 &quot;[!UICONTROL Lowest Cost per Acquisition]&quot; 최적화 목표만 포함된 패키지) 광고 지출 수익률 또는 획득당 비용을 계산하는 데 사용할 최종 전환 이벤트(예: 등록) 또는 매출 이벤트/판매 금액(예: 구매 및 구매 값)입니다. 선택한 사용자 정의 목표에 매핑된 모든 기본 이벤트(&quot;목표 지표&quot;) 목록에서 선택합니다. 목록이 비어 있는 경우 기본 이벤트 중 하나 이상을 목표 지표로 포함하도록 사용자 지정 목표를 편집합니다.

**[!UICONTROL Package Goal Type]:**(사용자 지정 최적화 목표가 있는 패키지 전용) 패키지의 목적입니다. 이 설정은 패키지를 최적화하는 방법을 결정하는 데 도움이 됩니다.

* *[!UICONTROL Prospecting]:* 전망 패키지는 신규 고객 확보에 중점을 둡니다.

* *[!UICONTROL Retargeting]:* 리타겟팅 패키지는 이전 방문자 또는 고객을 다시 노출하는 데 중점을 둡니다.

* *[!UICONTROL Other]:* 다른 모든 용도.

**[!UICONTROL Linked Package for Optimization Learnings Carryover]:**(사용자 지정 최적화 목표만 있는 패키지) 패키지 최적화를 위한 입력으로 내역 데이터가 사용되는 다른 패키지.

**[!UICONTROL Target]:**(패키지 수준 게재 간격 전용 패키지) 성능을 추적하는 데 사용되는 대상 목표입니다.

>[!NOTE]
>
>이 필드는 벤치마크일 뿐이며 의사 결정에는 사용되지 않습니다.

**[!UICONTROL Frequency Cap]:**(패키지 수준 게재 전용 패키지) 패키지에서 고유한 장치, 유니버설 ID 또는 사용자(캠페인에 대해 지정된 [!UICONTROL Cross Device Level] 및 배치의 [!UICONTROL Targeting] 설정에 따라 다름)가 광고를 제공할 수 있는 횟수입니다. 옵션에는 *[!UICONTROL Unlimited]* 또는 일, 주 또는 월당 특정 금액이 포함됩니다.

>[!NOTE]
>
>* 캠페인, 패키지 및 배치 수준에서 빈도 상한을 설정할 수 있습니다. DSP은 campaign 계층 구조에서 가장 엄격한 빈도 상한을 따릅니다.
>* 가장 좋은 방법은 패키지 수준에서 전망 및 재타겟팅 모두에 대한 빈도 상한을 설정하는 것입니다.
> * 빈도 상한이 높을수록 지출과 노출은 증가하지만 도달 거리는 감소합니다. 빈도 상한이 낮으면 지출과 노출이 줄어들지만 도달 범위가 높아집니다.

**[!UICONTROL Pace on]:**(패키지 수준 게재 간격 전용 패키지) 게재 간격 기준:

* *[!UICONTROL Budget]:*(기본값) 이 옵션은 할당된 패키지 예산 내에서 가능한 한 많은 노출 횟수를 제공합니다.

* *[!UICONTROL Impressions]:* 이 옵션은 지정된 간격 내에 지정된 수량에 도달할 때까지 노출을 전달합니다. 이 옵션을 선택하는 경우 노출 횟수와 간격: *항상,* *[!UICONTROL Daily],* *[!UICONTROL Monthly],* 또는 *[!UICONTROL Weekly]*&#x200B;을(를) 지정합니다.

**[!UICONTROL Flight pacing]:**(패키지 수준 게재 속도만 있는 패키지) 전체 플라이트 간 광고 게재 속도를 조정하는 방법:

* *[!UICONTROL Even]:* 각 항공편 전체에 걸쳐 균등하게 배송되며, 상반기 배송의 50%가 목표입니다.

* *[!UICONTROL Slightly Ahead]:*(기본값) 게재를 가속화하여 플라이트 기간 중간에 55~65% 완료됩니다.

* *[!UICONTROL Frontload]:* 배달 속도를 높여 비행 중간에 65~75% 완료됩니다.

* *[!UICONTROL Aggressive Frontload]:* 배달 속도를 높여 비행 중간에 75~85% 완료됩니다.

**[!UICONTROL Intraday pacing]:**(패키지 수준 게재 속도만 있는 패키지) 비행 내에서 매일 광고 게재 속도를 조정하는 방법:

* *[!UICONTROL Even]:*(기본값) 인벤토리 가용성에 따라 게재 크기를 조정합니다. 일반적으로 경매량이 많은 낮에는 시간당 더 많은 광고가 게재되고 아침과 저녁에는 더 적은 수의 광고가 게재된다.

* *[!UICONTROL ASAP]:*&#x200B;은(는) 게재를 *짝수*&#x200B;의 두 배 속도로 가속화합니다.

  >[!CAUTION]
  >
  >이 옵션은 성능에 부정적인 영향을 줄 수 있습니다. 성능 최적화에 비해 게재 우선 순위 및 비용을 완전히 우선시하는 경우에만 사용하십시오.

## [!UICONTROL Flighting]

(패키지 수준 게재 간격이 있는 패키지) 패키지의 전체 [!UICONTROL Flight Dates] 내의 사용자 지정 게재 기간을 포함하여 패키지의 플라이트 기간입니다. [!UICONTROL Goals & Budget] 섹션에서 [!UICONTROL Activate Custom Flighting] 옵션이 활성화된 경우에만 사용자 지정 항공편을 구성할 수 있습니다.

**[!UICONTROL Automatically rollover remaining flight budget to next flight]:**([!UICONTROL Activate Custom Flighting] 옵션이 활성화된 경우에만 사용 가능) 다음 항공편의 기존 예산에 이전 항공편의 남은 예산을 자동으로 추가합니다.

[!UICONTROL Packages] 보기 및 [!DNL Package Name] > [!UICONTROL Flights] 보기에서 현재 비행 목표를 표시하는 [!UICONTROL Interval Goal] 필드에 롤오버 예산이 포함되어 있습니다.

**[!DNL Flight N]:**([!UICONTROL Activate Custom Flighting] 옵션이 활성화된 경우에만 사용 가능) 각 항공편에 대해 시작 날짜, 종료 날짜 및 목표 지출 목표를 지정하십시오. 다른 비행기를 추가하려면 **[!UICONTROL Add Flight]**&#x200B;을(를) 클릭하십시오.

&quot;[!UICONTROL Automatically rollover remaining flight budget to next flight]&quot; 옵션이 활성화된 기존 패키지의 경우 설정을 다시 열어 모든 비행에 대해 **[!UICONTROL Rollover]** 열에 값을 입력하여 다음 비행에 지출되지 않은 잠재적 예산을 추가할 수 있습니다.

>[!MORELIKETHIS]
>
>* [패키지 관리 정보](package-about.md)
>* [패키지 만들기](package-create.md)
>* [패키지 편집](package-edit.md)
>* [패키지에 배치 첨부](package-attach-placement.md)
>* [패키지에 대한 변경 로그 보기](package-change-log.md)
>* Campaign Management에 대한 [FAQ](/help/dsp/campaign-management/faq-campaign-management.md)
