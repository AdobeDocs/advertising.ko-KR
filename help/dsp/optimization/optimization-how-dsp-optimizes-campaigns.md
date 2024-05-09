---
title: DSP이 캠페인을 최적화하는 방법
description: DSP이 캠페인에서 패키지를 최적화하는 방법을 알아봅니다.
feature: DSP Optimization
exl-id: 92d411cf-4307-4449-97b4-da3817f2a0b4
source-git-commit: 4b9cc5956d573b346eacdf71a8ea490c162b4660
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---

# Advertising DSP이 캠페인을 최적화하는 방법

이 페이지에서는 는에서 제공하는 DSP 최적화 엔진에 대해 간략하게 설명합니다. [!DNL Adobe Sensei]는 캠페인의 패키지를 최적화합니다. 캠페인을 수동으로 최적화하는 방법에 대한 팁과 요령은 Adobe 계정 팀에 문의하십시오. <!-- add link to trading playbook if we add it to help -->

패키지 최적화 목표는 다음 두 가지 수준에서 작동합니다.

* 각 패키지에 대해: DSP은 선택한 KPI에 대한 배치의 성과를 기반으로 패키지 내의 각 배치에 예산을 할당합니다.

* 패키지의 각 배치/경매에 대해: DSP은 배치당 각 경매에 대한 실시간 경제적 KPI 값을 계산한 다음 이 값을 사용하여 입찰을 결정합니다.

  >[!NOTE]
  >
  >경제적 가치는 배치가 얼마나 잘 지출되는지에 따라 크게 가중될 수 있다. 만약 배치가 지출 목표의 뒤에 있다면, 그것은 더 낮은 품질의 경매를 살 수 있습니다. 배치가 지출 목표를 쉽게 달성하는 경우 초점이 더 높은 품질의 경매로 이동합니다.

## 패키지 최적화

DSP은 특정 성능 목표에 맞게 사용할 수 있는 20개의 변형을 통해 두 가지 기본 방법으로 게재를 최적화할 수 있습니다. 다음을 선택할 수 있습니다.

* 성능 우선 순위 지정

* 비용 효율성과 성능 사이의 우선 순위 조정

다음을 참조하십시오 [최적화 목표 및 사용 방법](optimization-goals.md) 를 사용하여 KPI를 달성하는 데 도움이 되는 최적화 목표를 결정하십시오.

### 성능 우선 순위를 지정하는 패키지

성능 비율을 우선시하는 최적화 목표의 경우 DSP은 각 경매의 성능을 예측하고 항상 최대 입찰에서 입찰합니다. 적용 가능한 최적화 목표의 예는 다음과 같습니다. [!UICONTROL Highest Viewability Rate], [!UICONTROL Highest Clickthrough Rate]등.

이 최적화 모드는 다음과 같은 경우에 잘 작동합니다.

* 이미 유효/허용 CPM 수준(예: 과거 벤치마크)을 알고 있습니다.

* 다음을 수동으로 조정할 수 있습니다. [!UICONTROL Max Bid] 배율 조정과 관련하여 문제가 발생하는 경우 각 배치에 대해 설명합니다.

* 효율성보다 규모를 우선시하고 있습니다.

#### 게재 간격 논리 {#pacing-logic-performance}

* 지출이 진행 중이라면 입찰이 더 선택적이 되기 때문에 높은 이행률을 보일 것으로 예상되는 경매에만 입찰을 하게 된다.

* 지출이 늦어지면 입찰이 덜 선택적이 되기 때문에 게재 속도를 따라잡기 위해 더 낮은 이행률을 가질 것으로 예상되는 경매에 입찰하게 됩니다.

#### 가격/입찰 음영 지우기 {#clearing-price-performance}

게재 간격 논리를 실행한 후 DSP은 클리어링 가격 예측 모델을 통해 제안된 입찰을 실행합니다. 예측이 낙찰률에 대한 최소 감소와 함께 입찰이 낮아질 수 있음을 나타낸다면, 입찰은 예측에 따라 감소된다.

### 비용 효율성과 성능 사이의 균형을 최우선으로 고려하는 패키지

일부 최적화 목표의 경우 DSP은 각 경매의 성과를 예측하고 입찰 가격을 자동으로 조정하며 배치를 초과하지 않습니다. [!UICONTROL Max Bid]. 적용 가능한 최적화 목표의 예는 다음과 같습니다. [!UICONTROL Lowest CPM], [!UICONTROL Lowest CPA], [!UICONTROL Lowest Cost per View], [!UICONTROL Lowest Cost per Click]등.

#### 게재 간격 논리 {#pacing-logic-balanced}

* 만약 지출이 속도를 유지한다면, DSP은 더 가격에 민감해지고, 더 낮은 금액을 입찰하여 경쟁률과 경쟁률을 맞춘다.

* 성능 지표도 균형을 이루고 있는 경우 (다음을 제외한 모든 목표) [!UICONTROL Lowest CPM])를 입력하면 예측된 KPI가 입찰 금액으로 결합됩니다. 따라서 &quot;비용 기준&quot;으로 더 성능이 높을 것으로 예상되는 경매에 대해 더 높은 입찰을 합니다.

* 지출이 늦어지면 DSP은 덜 가격 민감해지고 입찰가는 더 높아져 [!UICONTROL Max Bid], 게재 비율을 게재 간격 계획과 맞교환.

#### 가격/입찰 음영 지우기 {#clearing-price-balanced}

게재 간격 논리를 실행한 후 DSP은 클리어링 가격 예측 모델을 통해 제안된 입찰을 실행합니다. 예측이 낙찰률에 대한 최소 감소와 함께 입찰이 낮아질 수 있음을 나타낸다면, 입찰은 예측에 따라 감소된다.

## 배치 최적화

배치 사전 입찰 필터는 강력한 성능을 보장하기 위한 가장 엄격한 방법입니다. DSP은 다양한 광고 유형에서 사전 입찰 필터를 전략적으로 사용하여 각 패키지 내의 배치 전반에서 성능 목표를 달성합니다. 패키지 수준 최적화와 동시에 또는 독립적으로 사전 입찰 필터를 사용할 수 있습니다.

>[!NOTE]
>
>사용 가능한 사전 입찰 필터는 광고 유형에 따라 다릅니다. 예를 들어 표준 디스플레이 배치의 경우 클릭스루 비율 및 가시성별로 필터링할 수 있지만 완료 비율로는 필터링할 수 없습니다.

다음을 참조하십시오 [배치 수준 사전 입찰 필터 및 사용 방법](optimization-pre-bid-filters.md) 은 어떤 사전 입찰 필터가 KPI를 달성하는 데 도움이 되는지 결정합니다.

>[!MORELIKETHIS]
>
>* [패키지 설정](/help/dsp/campaign-management/packages/package-settings.md)
>* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)
>* [최적화 목표 및 사용 방법](optimization-goals.md)
>* [배치 수준 사전 입찰 필터 및 사용 방법](optimization-pre-bid-filters.md)
>* [문제 해결 성능](/help/dsp/optimization/troubleshooting-performance.md)
