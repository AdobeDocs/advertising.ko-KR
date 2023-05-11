---
title: 에 대한 FAQ [!UICONTROL Household] 보고서
description: 추가 정보 [!UICONTROL Household] 다른 보고서와 문제 해결 방법을 포함한 보고서 세트에만 표시됩니다.
source-git-commit: 95f81dafbe13f40487bad47f7dd41a6c80c589ee
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# 에 대한 FAQ [!UICONTROL Household] 보고서

## 안녕하세요 [!UICONTROL Household] 도달 범위와 빈도 보고서는 다른 사용자 지정 보고서와 다릅니다.

다음 [!UICONTROL Household] 보고서는 IP 주소를 기반으로 가구 수준의 다양한 차원에 대한 도달, 노출 횟수 및 빈도를 측정합니다. 다른 사용자 지정 보고서는 장치 또는 쿠키 수준에서 생성됩니다.

예를 들어, 한 세대 내의 3개 장치에 한 가지 노출이 제공되더라도 고유한 가구 도달 지표는 1입니다.

### 지원되는 Dimension

다음 [!UICONTROL Household] 보고서는 을 지원합니다 [다음 차원](/help/dsp/reports/report-columns.md): &quot;[!UICONTROL Campaign],&quot; &quot;[!UICONTROL Package],&quot; &quot;[!UICONTROL Placement],&quot; &quot;[!UICONTROL Site/Apps]&quot;(중복 지표에 대한 액세스 권한을 제공하지 않음), &quot;[!UICONTROL Media Type],&quot; &quot;[!UICONTROL Feed Type],&quot; &quot;[!UICONTROL Device],&quot; &quot;[!UICONTROL Publisher],&quot; &quot;[!UICONTROL Audience],&quot; &quot;[!UICONTROL Creative Length],&quot; 및 사용자가 만든 배치 &quot;[!UICONTROL Tags].&quot; |

### 지원되는 지표

다음 [사용 가능한 지표](/help/dsp/reports/report-columns.md) 포함:

* 겹치기 지표: [!UICONTROL Frequency Overlap], [!UICONTROL Measurable Impressions (Overlap)], 및 [!UICONTROL Unique Household (Overlap)].

   겹치기 지표는 보고된 차원이나 차원 조합에만 발생하고 다른 차원에는 발생하지 않는 값입니다. <!-- For example, it might show the ?? -->

* 겹치지 않는 지표: [!UICONTROL Frequency], [!UICONTROL Incremental Household Reached], [!UICONTROL % Incremental Household Reached], [!UICONTROL Impressions], [!UICONTROL Measurable Impressions], 및 [!UICONTROL Unique Household Reached]

전환 지표 및 사용자 지정 목표는 지원되지 않습니다.

## 겹치기 지표와 겹치지 않는 지표 간의 차이점은 무엇입니까?

다음 그림은 세 개의 캠페인(A, B 및 C)에 대한 세 개의 지표(고유 가구 도달, 증분 가구 도달 및 증분 가구(겹치기)를 보여줍니다.

![가계 겹치기 지표 일러스트레이션](/help/dsp/assets/household-overlap-metrics-illustration.png "가계 겹치기 지표 일러스트레이션")

* 고유 가구 수 도달 (합계)은 각 캠페인에서 도달한 고유 가구나 각 원의 총 영역을 제공합니다. 그림에서 A = A + (A+B) + (A+C) +(A+B+C)에 의해 도달한 고유한 가구

* Incremental Family Destination은 캠페인에서만 도달한 Unique Family입니다. 그림에서 A, B, C에 의해 도달한 증분 가계는 각각 A, B, C에 의해 도달한 증분 가가구입니다.

* 증분 가족(겹치기)은 캠페인이나 캠페인 조합이 도달한 고유 가구입니다. 그림에서 A로 도달한 증분 가계는 C+C입니다.

## 워크플로

일반적인 단계를 따라 다음을 수행합니다 [사용자 지정 보고서 만들기](report-create.md).

다음 [!UICONTROL Household] 보고서는 하나의 차원만 포함할 수 있습니다. 또한 a) 사이트/앱을 제외한 모든 차원별로 겹치는 지표 또는 b) 겹치지 않는 지표를 포함할 수 있지만 둘 다 포함할 수는 없습니다.

## 의 몇 가지 제한 사항은 무엇입니까? [!UICONTROL Household] 보고? 

겹치기 지표가 있는 보고서는 최대 3개의 값을 출력합니다. 예를 들어, 지표를 사용하는 경우 [!UICONTROL Unique Household (Overlap)] 10개의 배치의 경우, 개별 배치로 도달한 고유 가구, 두 개의 배치를 결합하여 도달한 공통 가구, 세 개의 배치를 조합하여 도달한 공통 가구를 볼 수 있습니다. 네 개 이상의 배치에서 도달한 공통 가구를 볼 수 없습니다.

캠페인, 패키지 또는 배치 이외의 차원의 경우 보고서는 각 차원에서 최대 10개의 값을 지원합니다. 예를 들어 [!UICONTROL Unique Household Reached] 보고서 [!UICONTROL Audience] 차원일 경우 고유 대상 수가 10보다 작거나 같아야 합니다. 10개 이상의 고유 대상을 포함하는 경우 빈 보고서가 생성됩니다.

## 빈도 값과 고유 도달 값이 내 간에 다른 이유는 무엇입니까 [!UICONTROL Custom] 보고서 및 [!UICONTROL Household] 보고?

의 이러한 지표 [!UICONTROL Household] 보고서는 실제 IP 주소 수를 사용하여 계산되지만 [!UICONTROL Custom] 보고서는 모델을 사용하여 계산된 예상 숫자를 사용합니다. 하지만 10% 이하여야 한다.

## 에 대한 보고서를 어떻게 구성합니까? [!UICONTROL Placement Tags] 차원?

배치에 사용할 태그를 만들려면 [배치 설정 열기](/help/dsp/campaign-management/placements/placement-edit.md) 값을 입력하고 [배치 태그 필드](/help/dsp/campaign-management/placements/placement-settings.md).
 
배치에 여러 태그가 포함된 경우 보고서는 전체 문자열을 하나의 태그로 간주합니다. 보고서에는 각 고유 문자열에 대해 하나의 행이 포함됩니다.

## [!UICONTROL Household] 보고서와 데이터 비교 [!DNL Advanced Measurement Services]

가구 기반 도달 및 빈도에 대한 고급 보고를 위해, [[!DNL Strategic Advertising Consulting] 팀](/help/dsp/introduction/advanced-measurement-services.md) 는 전체적인 전략적 권장 사항과 함께 맞춤형 보고서를 제공할 수 있습니다. 에 대한 자세한 정보 [!DNL Advanced Measurement Services], Adobe 계정 팀에 문의하십시오.

### 이미 사용하고 있다면 [!DNL Advanced Measurement Services], 왜 [!UICONTROL Household] 보고?

다음 [!UICONTROL Household] 보고서를 통해 클라이언트가 가정에서 도달 범위와 빈도 지표를 자동으로 실시간으로 가져올 수 있습니다.

### 두 가지 모두를 사용할 수 있나요 [!UICONTROL Household] 보고서 및 [!DNL Advanced Measurement Services]? 

가장 이상적인 사용 사례는 [!UICONTROL Household] 보고서 및 [!DNL Advanced Measurement Services] 보고 및 컨설팅 서비스를 함께 제공합니다. 다음 사항을 고려하십시오 [!UICONTROL Household] 트랜잭션 보고서 - 일상적인 최적화 및 알림을 위한 것입니다. [!DNL Advanced Measurement Services] 보다 전략적인 것으로, 전체적인 통찰력과 중요한 비즈니스 목표에 관련된 사항을 알려주기 위한 것입니다.

>[!MORELIKETHIS]
>
>* [사용자 지정 보고서 정보](/help/dsp/reports/report-about.md)
>* [사용자 지정 보고서 만들기](/help/dsp/reports/report-create.md)
>* [사용자 지정 보고서 편집](/help/dsp/reports/report-edit.md)
>* [사용자 지정 보고서 설정](/help/dsp/reports/report-settings.md)
>* [사용 가능한 보고서 열](/help/dsp/reports/report-columns.md)

