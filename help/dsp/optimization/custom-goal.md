---
title: 사용자 정의 목표
description: 가장 낮은 CPA 또는 가장 높은 ROAS에 최적화된 패키지에서 성공 이벤트를 정의하는 사용자 정의 목표에 대해 알아봅니다.
feature: DSP Optimization
source-git-commit: 7b9926d0bbba12728ed6a42e56115e8df708587b
workflow-type: tm+mt
source-wordcount: '1104'
ht-degree: 0%

---

# 사용자 정의 목표

사용자 지정 목표는 광고주가 비즈니스 목표를 달성하는 데 필요한 성공 이벤트를 정의합니다. 최적화 목표 를 사용하는 각 패키지[!UICONTROL Highest Return on Ad Spend (ROAS)"] 또는 &quot;[!UICONTROL Lowest Cost per Acquisition (CPA)]&quot;은(는) 전체 최적화 목표를 달성하는 데 도움이 되는 사용자 지정 목표를 포함해야 합니다. 다음과 같이 사용자 정의 목표를 생성할 수 있습니다. *목표* 위치: [!DNL Advertising Search, Social, & Commerce].

<!-- update image or omit it

![custom goals](/help/dsp/assets/objective-goals.png)
 -->

각 사용자 지정 목표는 하나 이상의 전환 지표와 이러한 지표의 상대 가중치로 구성됩니다. 사용 가능한 전환 지표에는 Adobe Advertising 전환 픽셀을 사용하여 Adobe Analytics을 통해 추적된 모든 지표가 포함됩니다.

예를 들어 세 개의 전환 지표가 캠페인 중 하나의 특정 패키지와 관련이 있다고 가정해 보겠습니다. &quot;PDF 다운로드&quot;(20 USD), &quot;이메일 등록&quot;(30 USD) 및 &quot;주문 확인&quot;(40 USD)입니다. 고객 조치의 일회성 통화 가치에 따라 가중치를 부여하려면 지표의 상대 가중치는 1, 1.5 및 2가 됩니다.

한 번 [사용자 지정 목표 만들기](#custom-goal-create), 다음을 수행할 수 있습니다. [패키지에 할당](/help/dsp/campaign-management/packages/package-settings.md) Adobe Sensei을 사용하여 보고 및 알고리즘 최적화를 위한 .

## 사용자 지정 목표 만들기 {#custom-goal-create}

사용자 지정 목표를 만들려면 DSP 계정이 [!DNL Search, Social, & Commerce] 내에서 동일한 Adobe Experience Cloud 조직 ID를 가진 계정 [!DNL Search, Social, & Commerce] 클라이언트 설정. DSP 계정이 [!DNL Search, Social, & Commerce] 계정을 만든 다음 Adobe 계정 팀에 문의하십시오.

1. 에 로그인 [!DNL Advertising Search, Social, & Commerce] at (북미 사용자) [`https://enterprise-na.efrontier.com`](https://enterprise-na.efrontier.com) 또는 (다른 모든 사용자) [`https://enterprise-intl.efrontier.com`](https://enterprise-intl.efrontier.com).

1. 목표에 포함할 지표가 추적되고 제품에서 사용할 수 있는지 확인하고 표시 이름을 포함하십시오.

   1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Admin] >[!UICONTROL Conversions]**.

   1. 지표를 찾고 다음을 확인합니다. **[!UICONTROL Show in UI and Reports]** 지표에 대해 활성화됩니다.

      >[!NOTE]
      >
      >* [!DNL Analytics] 사용자 지정 이벤트는 다음 명명 규칙을 따릅니다. `custom_event_[*event #*]_[*Analytics report suite ID*]`. 예: `custom_event_16_examplersid`

   1. 지표에 값이 없는 경우 **[!UICONTROL Display Name]** 열을 클릭한 다음 셀을 클릭하고 표시 이름을 입력한 다음 를 클릭합니다 **[!UICONTROL Apply].**

1. 사용자 정의 목표를 다음으로 만들기 *목표*:

   1. 메인 메뉴에서 **[!UICONTROL Search]** > **[!UICONTROL Optimization]>[!UICONTROL New Objectives Beta]**.

   1. 도구 모음에서 를 클릭합니다 ![만들기](/help/dsp/assets/create-search-ui.png "만들기").

   1. 비모바일 장치 및 모바일 장치에 대한 관련 지표 및 상대 숫자 가중치를 포함하여 목표 설정을 입력한 다음 목표를 저장합니다.

      하나 이상의 지표에 지표 유형이 있어야 합니다. *[!UICONTROL Goal]*.

      >[!NOTE]
      >
      >* [!DNL Analytics] 사용자 지정 이벤트는 다음 명명 규칙을 따릅니다. `custom_event_[*event #*]_[*Analytics report suite ID*]`. 예: `custom_event_16_examplersid`
      >* [!DNL Analytics] Adobe Advertising 최적화에 차원 및 세그먼트를 사용할 수 없습니다.

      >[!TIP]
      >
      >최적의 성능을 위해서는 사용자 지정 목표(목표)의 결합된 지표가 하루에 10개 이상의 전환을 수행해야 합니다. 그렇지 않은 경우 제품 페이지나 애플리케이션 시작과 같은 추가 지원 전환 지표를 목표에 추가하는 것이 좋습니다. 다음을 참조하십시오 [사용자 지정 목표 빌드를 위한 우수 사례](#custom-goal-best-practices) 지침을 참조하십시오.

최적화 목표 를 사용하는 패키지에 대한 DSP 패키지 설정에서 &quot;[!UICONTROL Highest Return on Ad Spend (ROAS)"] 또는 &quot;[!UICONTROL Lowest Cost per Acquisition (CPA)],&quot; 이제 목표 이름이 [!UICONTROL Custom Goals] 목록을 표시합니다. 패키지의 사용자 지정 목표로 목표를 선택하면 [!UICONTROL Conversion Metric] 목록에는 목표에 대한 모든 목표 지표가 포함됩니다.

## 사용자 지정 목표 빌드를 위한 우수 사례 {#custom-goal-best-practices}

### 단일 지표를 사용한 사용자 정의 목표

다음 예에서는 단일 전환 지표를 대상으로 하는 목표를 구성하는 방법을 보여 줍니다.

#### 가 있는 캠페인의 예[!UICONTROL Highest Return on Ad Spend (ROAS)]&quot; 최적화 목표

캠페인 목표가 매출인 경우([!UICONTROL Highest Return on Ad Spend (ROAS)])과 모든 장치 유형의 매출은 똑같이 중요한 다음 &quot;[!UICONTROL Revenue]&quot; 비모바일 가중치(비모바일 장치에서 전환된 경우)가 하나(1)이고 모바일 가중치(모바일 장치에서 전환된 경우)가 하나(1)인 지표. 지표 유형 선택 *[!UICONTROL Goal]*.

<!-- update image or delete 

![example of a ROAS custom goal with a single conversion metric](/help/dsp/assets/custom-goal-roas.png)

-->

>[!NOTE]
>
> 모바일 가중치 또는 비모바일 가중치는 1로 추적된 매출 $1에 대해 1의 값과 동일합니다.
>
> 예를 들어 비모바일 가중치가 1인 $250 전환은 전환에 대해 $250로 보고됩니다. 전환 지표에 0.5의 비모바일 가중치가 지정되면 비모바일 장치에서 $250 전환을 Adobe Advertising($250 전환 * 0.5)에서 $125로 보고합니다 [!UICONTROL Non-mobile Weight] = $125).

#### 가 있는 캠페인의 예[!UICONTROL Lowest Cost per Acquisition (CPA)]&quot; 최적화 목표

캠페인 목표가 CPA(취득당 최저 비용)이고 하나의 성공 이벤트(예: &quot;애플리케이션 제출&quot;)만 필요한 경우, 해당 지표를 포함하고 지표 유형을 다음으로 지정하십시오. *[!UICONTROL Goal]*. 가장 좋은 방법은 비이동가중치와 이동가중치를 모두 1로 설정하는 것이다.

<!-- update image or delete 

![example of a CPA custom goal with a single conversion metric](/help/dsp/assets/custom-goal-roas.png)

-->

>[!NOTE]
>
> 모바일 가중치 또는 비모바일 가중치는 1이며, 추적된 각 전환에 대해 1의 값과 동일합니다. 예를 들어 10개의 애플리케이션 제출 전환이 추적되면 10개의 애플리케이션 제출 전환이 보고됩니다. 그러나 전환 지표에 0.5의 비모바일 가중치가 할당되면 Adobe Advertising (10 전환 * 0.5에서 10 비모바일 전환은 5(5)로 보고됩니다 [!UICONTROL Non-mobile Weight] = 5).

### 여러 지표를 사용하는 사용자 정의 목표

사용자 지정 목표에서 여러 지표를 사용하는 두 가지 시나리오가 있습니다.

* 캠페인 목표에는 여러 개의 성공 이벤트가 있습니다. 예를 들어 둘 이상의 온사이트 작업(PDF 다운로드, 연락처 및 이메일 등록)에 대해 광고하고 있을 수 있으며 모든 작업은 CPA 목표에 기여하는 작업입니다. 목표에 세 개의 별도 지표가 포함되어 있고 각각 비모바일 및 모바일 가중치가 1인 경우 [!DNL Adobe Sensei] 알고리즘에서는 각 지표 및 사용자 장치 유형을 동일한 중요도로 처리합니다. 다양한 지표와 장치 유형에 비용이나 중요도가 다른 경우 그에 따라 상대적 가중치를 조정합니다.

<!-- update image or delete it and adjust the wording above

   ![example of a custom goal with multiple metrics](/help/dsp/assets/custom-goal-multiple-properties.png)

-->

* 사용자 지정 목표의 단일 전환 지표는 최적화된 성능에 필요한 하루 최소 10개의 전환을 달성하지 못합니다. 이는 최소 일일 패키지 지출 또는 제한된 수의 자연 전환으로 인해 발생할 수 있습니다. 사용자 지정 목표에 추가 지원 지표를 추가하면 일별 전환 임계값 10개를 달성할 수 있습니다. 10개의 지원 이벤트는 각 가중치가 1보다 작은 경우에도 패키지가 10일 임계값을 충족하는 데 도움이 될 수 있습니다. 그러나 이러한 많은 이벤트를 추가할 필요는 없습니다.

  사용자 지정 목표에 지원 지표를 추가할 때 기본 성공 이벤트에 대한 상대적 중요도에 따라 가중치를 부여하고 데이터 포인트의 수량을 염두에 두십시오. 이렇게 하면 Adobe Sensei 알고리즘이 여러 지표의 균형을 맞추고 목표를 향해 최적화할 수 있습니다.

  다음 예제 목표에는 각각 다른 비모바일 가중치를 갖는 세 개의 지표(애플리케이션 제출 = 1, 애플리케이션 시작 = 0.1, 광고주 랜딩 페이지 = 0.01)가 포함됩니다. 즉, 모바일이 아닌 장치에서 각 애플리케이션 제출 전환은 모바일이 아닌 장치에서 평균 10개의 애플리케이션 시작 전환 및 모바일이 아닌 장치에서 100개의 광고주 랜딩 페이지 전환과 동일한 값을 비즈니스에 제공합니다.

<!-- update image or delete it and adjust the wording above

   ![example of a custom goal with multiple metrics](/help/dsp/assets/custom-goal-multiple-properties2.png)

-->

대신, 랜딩 페이지 방문 횟수를 애플리케이션 제출과 동일하게 가중하면 랜딩 페이지 방문 횟수가 자연히 증가하여 목표를 압도하고 랜딩 페이지 방문 횟수로 기울일 수 있습니다.<!--reword-->

>[!MORELIKETHIS]
>
>* [최적화 목표 및 사용 방법](optimization-goals.md)
>* [패키지 설정](/help/dsp/campaign-management/packages/package-settings.md)
> * [DSP이 캠페인을 최적화하는 방법](optimization-how-dsp-optimizes-campaigns.md)
