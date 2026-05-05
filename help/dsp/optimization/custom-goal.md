---
title: 사용자 지정 목표에 대한 우수 사례
description: 가장 낮은 CPA 또는 가장 높은 ROAS에 최적화된 패키지에 대한 사용자 지정 목표를 정의하는 모범 사례에 대해 알아봅니다.
feature: DSP Optimization
exl-id: e40b82bc-2558-4e78-b269-9b9a3f0f5219
TQID: https://experienceleague.adobe.com/xSM4vyVErtNbVqF3eMDeHpgEWaMK6hBwQpvijHEs0dc
product_v2: id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2: id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
subfeature_v2: id: af280ddc-b4d0-4416-86be-8f3ea3c6ebe7id: fddd8d8f-3ba1-4a22-b714-69d0e4655be8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
source-git-commit: e2746d58fa512f032a1e4ff851d23876cd63fc93
workflow-type: tm+mt
source-wordcount: 700
ht-degree: 0%

---

# 사용자 지정 목표에 대한 우수 사례

사용자 지정 목표는 광고주가 비즈니스 목표를 달성하는 데 필요한 성공 이벤트를 정의합니다. 최적화 목표 &quot;[!UICONTROL Highest Return on Ad Spend (ROAS)"]&quot; 또는 &quot;[!UICONTROL Lowest Cost per Acquisition (CPA)]&quot;을(를) 사용하는 각 패키지에는 전체 최적화 목표를 달성하는 데 도움이 되도록 사용자 지정 목표가 포함되어야 합니다. 사용자 지정 목표를 *[사용자 지정 목표](/help/dsp/admin/custom-objectives-manage.md)*(으)로 만들 수 있습니다.

<!--
 update image or omit it

![custom goals](/help/dsp/assets/objective-goals.png)
 -->

각 사용자 지정 목표(목표)는 추적 및 최적화할 하나 이상의 전환 지표와 해당 지표의 상대 가중치로 구성됩니다. [!DNL Adobe AI]을(를) 사용하여 보고 및 알고리즘 최적화를 위해 [패키지에 사용자 지정 목표를 할당](/help/dsp/campaign-management/packages/package-settings.md)할 수 있습니다.

사용자 지정 목표를 만들고 관리하려면 &quot;[사용자 지정 목표 관리](/help/dsp/admin/custom-objectives-manage.md)&quot;를 참조하십시오.

## 단일 지표를 사용한 사용자 정의 목표

다음 예에서는 단일 전환 지표를 대상으로 하는 목표를 구성하는 방법을 보여 줍니다.

### 최적화 목표가 &quot;[!UICONTROL Highest Return on Ad Spend (ROAS)]&quot;인 캠페인의 예

캠페인 목표가 매출([!UICONTROL Highest Return on Ad Spend (ROAS)])이고 모든 장치 유형의 매출이 동일하게 중요한 경우 가중치가 1인 &quot;[!UICONTROL Revenue]&quot; 지표를 포함하십시오. 지표 유형 *[!UICONTROL Goal]*&#x200B;을(를) 선택하십시오.

<!--
 update image or delete 

![example of a ROAS custom goal with a single conversion metric](/help/dsp/assets/custom-goal-roas.png)

-->

>[!NOTE]
>
> 1의 가중치는 모든 디바이스에서 디스플레이 광고를 위해 추적된 매출의 각 $1에 대해 1의 값과 동일합니다. 예를 들어 가중치가 1인 $250 전환은 전환에 대해 $250로 보고됩니다. 전환 지표에 가중치 0.5가 지정되면 Adobe Advertising에서 $250 전환은 $125로 보고됩니다($250 전환 * 0.5 [!UICONTROL weight] = $125).

### 최적화 목표가 &quot;[!UICONTROL Lowest Cost per Acquisition (CPA)]&quot;인 캠페인의 예

캠페인 목표가 CPA(취득당 최저 비용)이고 성공 이벤트(예: &quot;애플리케이션 제출&quot;)가 하나만 필요한 경우 해당 지표를 하나 포함하고 지표 유형을 *[!UICONTROL Goal]*(으)로 지정하십시오. 가중치를 1로 설정하는 것이 가장 좋습니다.

<!--
 update image or delete 

![example of a CPA custom goal with a single conversion metric](/help/dsp/assets/custom-goal-roas.png)

-->

>[!NOTE]
>
> 1의 가중치는 모든 디바이스에서 디스플레이 광고를 위해 추적된 각 전환에 대해 1의 값과 동일합니다. 예를 들어 10개의 애플리케이션 제출 전환이 추적되면 10개의 애플리케이션 제출 전환이 보고됩니다. 그러나 전환 지표에 가중치 0.5가 할당되면 Adobe Advertising에서 10개의 전환이 5개(5)로 보고됩니다(10개 전환 * 0.5 [!UICONTROL weight] = 5).

## 여러 지표를 사용하는 사용자 정의 목표

사용자 지정 목표에서 여러 지표를 사용하는 두 가지 시나리오가 있습니다.

* 캠페인 목표에는 여러 개의 성공 이벤트가 있습니다. 예를 들어 두 개 이상의 온사이트 작업(PDF 다운로드, 연락처 및 이메일 등록)을 광고하는 경우 모든 작업은 CPA 목표에 기여하는 작업입니다. 목표에 각각 1의 가중치가 있는 세 개의 개별 지표가 포함되어 있는 경우 [!DNL Adobe AI] 기반 알고리즘은 각 지표 및 사용자 장치 유형을 동일한 중요도로 처리합니다. 서로 다른 지표에 다양한 비용이나 중요도가 있는 경우 그에 따라 상대적 가중치를 조정합니다.

<!--
 update image or delete it and adjust the wording above

   ![example of a custom goal with multiple metrics](/help/dsp/assets/custom-goal-multiple-properties.png)

-->

* 사용자 지정 목표의 단일 전환 지표는 최적화된 성능에 필요한 하루 최소 10개의 전환을 달성하지 못합니다. 최소한의 일일 패키지 지출 또는 제한된 수의 자연 전환으로 인해 전환 수가 줄어들 수 있습니다. 사용자 지정 목표에 추가 지원 지표를 추가하면 일별 전환 임계값 10개를 달성할 수 있습니다. 10개의 지원 이벤트는 각 가중치가 1보다 작은 경우에도 패키지가 10일 임계값을 충족하는 데 도움이 될 수 있습니다. 그러나 이러한 많은 이벤트를 추가할 필요는 없습니다.

  사용자 지정 목표에 지원 지표를 추가할 때 기본 성공 이벤트에 대한 상대적 중요도에 따라 가중치를 부여하고 데이터 포인트의 수량을 염두에 두십시오. 이를 통해 [!DNL Adobe AI] 기반 알고리즘이 여러 지표의 균형을 맞추고 목표를 향해 최적화할 수 있습니다.

  다음 예제 목표에는 각각 다른 가중치를 갖는 세 개의 지표 (애플리케이션 제출 = 1, 애플리케이션 시작 = 0.1, 광고주 랜딩 페이지 = 0.01)가 포함됩니다. 즉, 각 애플리케이션 제출 전환은 평균 10개의 애플리케이션 시작 전환과 100개의 광고주 랜딩 페이지 전환과 동일한 값을 비즈니스에 제공합니다.

<!--
 update image or delete it and adjust the wording above

   ![example of a custom goal with multiple metrics](/help/dsp/assets/custom-goal-multiple-properties2.png)

-->

대신 랜딩 페이지 방문 횟수를 애플리케이션 제출과 동일하게 가중하면 랜딩 페이지 방문 횟수가 자연히 증가하여 목표를 압도하고 랜딩 페이지 방문 횟수로 최적화를 왜곡할 수 있습니다.

>[!MORELIKETHIS]
>
>* [사용자 지정 목표 관리](/help/dsp/admin/custom-objectives-manage.md)
>* [최적화 목표 및 사용 방법](optimization-goals.md)
>* [패키지 설정](/help/dsp/campaign-management/packages/package-settings.md)
>* [DSP에서 캠페인을 최적화하는 방법](optimization-how-dsp-optimizes-campaigns.md)
