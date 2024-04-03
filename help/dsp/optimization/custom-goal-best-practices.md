---
title: 사용자 지정 목표 빌드를 위한 우수 사례
description: 성공 이벤트를 정의하기 위한 사용자 정의 목표 구축의 모범 사례에 대해 알아봅니다.
feature: DSP Optimization, DSP Best Practices
exl-id: 8b1247cd-083d-4c8c-8588-9e8c03c4cc67
source-git-commit: 6aa81fe4fd5ea6cb188b7f18b1574c26ddfcbb92
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# 사용자 지정 목표 빌드를 위한 우수 사례

## 단일 속성을 갖는 사용자 정의 목표

다음 예에서는 단일 전환 지표를 대상으로 하는 목표를 구성하는 방법을 보여 줍니다.

### 가 있는 캠페인의 예[!UICONTROL Highest Return on Ad Spend (ROAS)]&quot; 최적화 목표

캠페인 목표가 매출인 경우([!UICONTROL Highest Return on Ad Spend (ROAS)])을 지정하면 사용자 지정 목표(목표)에 &quot;[!UICONTROL Revenue]가중치가 1인 &quot; 지표.

![단일 전환 지표를 사용하는 ROAS 사용자 지정 목표의 예](/help/dsp/assets/custom-goal-roas.png)

>[!NOTE]
>
> A [!UICONTROL Property Weight] 하나는 추적된 매출 1달러당 1달러의 값과 동일합니다.
>
> 예를 들어 가중치가 1인 $250 전환은 $250로 보고됩니다. 전환 지표에 가중치 0.5가 지정되면 $250 전환은 Adobe Advertising($250 전환 * 0.5)에서 $125로 보고됩니다 [!UICONTROL Property Weight] = $125).

### 가 있는 캠페인의 예[!UICONTROL Lowest Cost per Acquisition (CPA)]&quot; 최적화 목표

캠페인 목표가 CPA(취득당 최저 비용)이고 하나의 성공 이벤트만 필요한 경우 해당 지표를 한 개 포함합니다(다음 예에서 &quot;애플리케이션 제출&quot;). 가중치를 1로 설정하는 것이 가장 좋습니다.

![단일 전환 지표를 사용하는 CPA 사용자 지정 목표의 예](/help/dsp/assets/custom-goal-roas.png)

>[!NOTE]
>
> A [!UICONTROL Property Weight] 중 하나는 추적되는 각 전환에 대한 하나의 값과 동일합니다.
>
> 예를 들어 10개의 애플리케이션 제출 전환이 추적되면 10개의 애플리케이션 제출 전환이 보고됩니다.  전환 지표에 가중치 0.5가 할당되면 Adobe Advertising (10 전환 * 0.5에서 10 전환이 5(5)로 보고됩니다 [!UICONTROL Property Weight] = 5).

## 여러 속성을 갖는 사용자 정의 목표

사용자 지정 목표에서 여러 속성을 사용하는 두 가지 시나리오가 있습니다.

* 캠페인 목표에는 여러 개의 성공 이벤트가 있습니다. 예를 들어 두 개 이상의 현장 작업에 대한 광고를 하는 경우 모두 CPA 목표에 귀속될 수 있습니다. 다음 예제 목표에는 각각 가중치가 1(1)인 세 개의 개별 속성(PDF 다운로드, 연락처 및 이메일 등록)이 포함되어 있습니다. [!DNL Adobe Sensei] 각 속성의 중요도가 동일한 알고리즘. 다양한 비용이나 중요도가 있는 속성을 포함하는 경우 그에 따라 상대적인 가중치를 조정할 수 있습니다.

  ![여러 속성이 있는 사용자 지정 목표의 예](/help/dsp/assets/custom-goal-multiple-properties.png)

* 사용자 지정 목표의 단일 전환 지표는 최적화된 성능에 필요한 하루 최소 10개의 전환을 달성하지 못합니다. 이는 최소 일일 패키지 지출 또는 제한된 수의 자연 전환으로 인해 발생할 수 있습니다. 사용자 지정 목표에 추가 지원 속성을 추가하면 일별 전환 임계값 10개를 달성할 수 있습니다. 10개의 지원 이벤트는 각 가중치가 1보다 작은 경우에도 패키지가 10일 임계값을 충족하는 데 도움이 될 수 있습니다. 그러나 이러한 많은 이벤트를 추가할 필요는 없습니다.

  사용자 지정 목표에 지원 속성을 추가할 때 기본 성공 이벤트에 대한 상대적 중요도에 따라 가중치를 부여하고 데이터 포인트의 수량을 염두에 두십시오. 이를 통해 Adobe Sensei 알고리즘은 여러 속성의 균형을 맞추고 목표에 맞게 최적화할 수 있습니다.

  다음 예제 목표에는 각각 다른 가중치를 갖는 세 가지 속성(애플리케이션 제출 = 1, 애플리케이션 시작 = 0.1, 광고주 랜딩 페이지 = 0.01)이 포함됩니다. 즉, 각 애플리케이션 제출 전환은 평균 10개의 애플리케이션 시작 전환과 100개의 광고주 랜딩 페이지 전환과 동일한 값을 비즈니스에 제공합니다.

  ![여러 속성이 있는 사용자 지정 목표의 예](/help/dsp/assets/custom-goal-multiple-properties2.png)

  대신 랜딩 페이지 방문 횟수를 애플리케이션 제출과 동일하게 가중하면 랜딩 페이지 방문 횟수가 자연히 증가하여 목표를 압도하고 랜딩 페이지 방문 횟수로 기울일 수 있습니다.<!--reword-->

>[!MORELIKETHIS]
>
>* [사용자 정의 목표 정보](custom-goal-about.md)
>* [사용자 지정 목표 만들기](custom-goal-create.md)
>* [최적화 목표 및 사용 방법](optimization-goals.md)
>* [패키지 설정](/help/dsp/campaign-management/packages/package-settings.md)
> * [DSP이 캠페인을 최적화하는 방법](optimization-how-dsp-optimizes-campaigns.md)
