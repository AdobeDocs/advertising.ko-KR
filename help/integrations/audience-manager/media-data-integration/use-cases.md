---
title: 사용 사례
description: Audience Manager과 Advertising DSP 미디어 데이터를 공유하는 사용 사례에 대해 알아봅니다
feature: Integration with Adobe Audience Manager
exl-id: 1d961799-b8be-499a-8db6-b59762d96bf1
source-git-commit: 7f35b3f3b33ed320ac186d219cbd0f826666bb3b
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 0%

---

# Adobe Audience Manager에서 미디어 노출 데이터 캡처를 위한 사용 사례

*Advertising DSP만 있는 광고주*

*Adobe Advertising-Adobe Audience Manager 통합만 있는 광고주*

다음은 Audience Manager에서 Advertising DSP 미디어 노출 데이터 <!-- ad impression data? -->을(를) 캡처하여 이점을 얻을 수 있는 몇 가지 방법입니다.

## 최신성 및 빈도 관리

Audience Manager에서 노출 데이터를 캡처하면 특정 광고나 캠페인에 노출된 사용자 세그먼트를 생성하여 빈도 관리를 향상시킬 수 있습니다. 빈도를 높이려는 경우 광고 타겟팅에 또는 빈도를 제한하려는 경우 광고 억제에 이러한 세그먼트를 사용할 수 있습니다.

또한 Audience Manager [!DNL Segment Builder]을(를) 사용하면 실행 가능한 신호가 포함된 [규칙 기반 특성](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/traits/trait-builder/create-onboarded-rule-based-traits.html)에 [최신성 및 빈도 컨트롤](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/segments/recency-and-frequency.html)을(를) 적용할 수 있습니다. 예를 들어 미디어 캠페인 내에서 특정 크리에이티브가 사용자에게 표시되는 횟수를 제한할 수 있습니다. 이 방법을 알아보려면 &quot;[장치 간 즉시 억제](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/profile-merge-rules/instant-cross-device-suppression.html)&quot;을(를) 읽으십시오.<!-- The AM pulled this paragraph verbatim from AEM doc; I change only a word or two. -->

## 순차적 메시징

노출 데이터를 캡처하여 캠페인 또는 광고에 노출된 사용자 세그먼트를 만들고 순차적 메시지 또는 억제에 이 세그먼트를 사용할 수 있습니다. 예를 들어, `123` 크리에이티브를 보았지만 `456` 크리에이티브를 표시하여 클릭하거나 전환하지 않은 사용자를 재타겟팅할 수 있습니다.

Audience Manager에서 이 예제를 실행하려면 다음 단계를 수행합니다.<!-- The AM pulled this example/procedure verbatim from AEM doc; I changed only a word or two. -->

1. 트레이트를 만들어 크리에이티브를 본 사용자를 캡처합니다.

   예를 들어 트레이트 이름을 `Creative Trait 123`로 지정하려면 다음 트레이트 규칙을 사용하십시오.

   ```
   d_creative == 123 AND d_event == imp
   ```

1. 클릭하거나 전환하는 사용자를 캡처할 트레이트를 만듭니다.

   예를 들어 이 트레이트의 이름을 `Click and Converter`(으)로 지정하려면 다음 트레이트 규칙을 사용하십시오.

   ```
   d_event == click OR d_event=conv
   ```

1. `Retarget Users`(이)라는 세그먼트를 만들어 Creative `123`을(를) 보았지만 클릭하거나 전환하지 않은 사용자로 채웁니다. 다음 트레이트 규칙을 사용합니다.

   ```
   Creative Trait 123 AND NOT Click and Converter
   ```

1. 세그먼트 `Retarget Users`을(를) 대상에 매핑하고 대상에 있는 사용자를 Creative `456`(으)로 타깃팅합니다.

## [!DNL Adobe Audience Analytics] 및 캠페인 노출 데이터

Audience Manager 내에서 캠페인 노출 및 클릭 데이터를 사용할 수 있게 되면 특정 캠페인이나 전술로 노출되거나 상호 작용한 사용자의 트레이트 및 세그먼트를 만들 수 있습니다. [[!DNL Audience Analytics] 통합](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html)을 사용하면 추가 분석을 위해 Audience Manager 세그먼트를 [!DNL Analytics]과(와) 동기화할 수 있습니다. 잠재적 사용 사례는 다음과 같습니다.

* **DSP과 [!DNL Advertising Search, Social, & Commerce] 광고 간의 상호 작용 분석:** 표준 [[!DNL Analytics for Advertising] 통합](/help/integrations/analytics/overview.md)에서는 DSP과 [!DNL Search, Social, & Commerce] 간의 상호 작용에 대한 통찰력을 제공하지 않습니다. 두 채널 모두 AMO ID 속성 규칙을 따르는 AMO ID를 사용하므로 검색 클릭은 디스플레이 뷰스루를 무시합니다. Audience Manager에서 DSP 노출 세그먼트를 만들어 [!DNL Audience Analytics]을(를) 사용하여 [!DNL Analytics]의 DSP과 [!DNL Search, Social, & Commerce] 광고 간의 상호 작용을 분석할 수 있습니다.

* **빈도 분석:** 사용자가 특정 광고나 Audience Manager에 노출된 횟수를 기반으로 하여 광고에서 세그먼트를 만들 수 있습니다. 그런 다음 Analytics에서 다양한 노출 세그먼트를 분석하여 DSP 노출 수에 따라 사용자 행동이 어떻게 변하는지 확인할 수 있습니다.

## [!DNL Audience Optimization Reports]

[Audience Manager [!DNL Audience Optimization Reports]](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reporting/audience-optimization-reports/audience-optimization-reports.html)을(를) 활용하여 캠페인 전반의 세그먼트에 대한 잠재적인 성과 기회를 식별할 수 있습니다. 이러한 보고서는 캠페인 노출, 클릭 및 전환 데이터를 세그먼트 지표와 결합하여 세그먼트 중심의 최적화와 효과적인 채널 혼합을 알려줍니다.

### 관련 Audience Optimization 보고서 유형

| 보고서 | 설명 |
| ------ | ----------- |
| [[!UICONTROL Segment Performance] 보고서](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reporting/audience-optimization-reports/audience-optimization-advertisers/segment-performance.html) | 노출 횟수와 전환율을 기준으로 매핑된 세그먼트와 매핑되지 않은 세그먼트를 비교합니다. |
| [[!UICONTROL Trend Analysis and Volume Analysis]개 보고서]9https://experienceleague.adobe.com/docs/audience-manager/user-guide/reporting/audience-optimization-reports/audience-optimization-advertisers/trend-analysis-volume-analysis.html) | 노출 횟수, 클릭스루 비율 및 전환율에 대한 데이터를 광범위한 광고 차원에 반환합니다. |
| [[!UICONTROL Optimal Frequency] 보고서](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reporting/audience-optimization-reports/audience-optimization-advertisers/optimal-frequency.html) | 제공된 노출 횟수와 전환 수 간에 최적의 균형을 찾는 데 도움이 됩니다. 이를 통해 축소 수익을 보기 전에 표시할 노출 횟수를 조정할 수 있습니다. |
| [[!UICONTROL Unique User Reach] 보고서](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reporting/audience-optimization-reports/audience-optimization-advertisers/unique-user-reach.html) | 각 버블의 크기가 선택한 차원의 고유 사용자 수에 직접 비례하여 조정되는 버블 차트. |

### 고려 사항

* [!DNL Audience Optimization Reports]명의 사용자에게 RBAC(역할 기반 액세스 제어)가 있는 경우 [!DNL Adobe Customer Care]은(는) 광고주 ID와 조직의 Audience Manager 데이터 소스 통합 코드 간의 매핑을 구성해야 합니다. 그런 다음 관리자 사용자는 다른 사용자에게 RBAC 권한을 제공할 수 있습니다.

* [!DNL Audience Optimization Reports]에서 전환 보고를 수행하려면 최종 사용자가 일부 설정해야 합니다. 사용자는 메타데이터 파일을 채워야 합니다.

* [!DNL Audience Optimization Reports]은(는) 캠페인 메타데이터(예: 캠페인 이름 또는 배치 이름) 변경을 지원하지 않습니다.

* 검색 광고 클릭은 노출과 상관 관계가 있는 경우에만 [!DNL Audience Optimization Reports]에 포함됩니다. 즉, 검색 클릭은 노출 횟수에 따른 전환으로 처리됩니다. 따라서 많은 검색 클릭이 [!DNL Audience Optimization Reports]에 포함되지 않을 수 있습니다.

>[!MORELIKETHIS]
>
>* [Adobe Audience Manager에 DSP Media 노출 데이터 전송 개요](overview.md)
>* [Advertising DSP 캠페인에서 클릭 및 노출 데이터 수집](collect.md)
