---
title: 에 대한 FAQ [!UICONTROL Household] 보고서
description: 에 대해 자세히 알아보기 [!UICONTROL Household] 다른 보고서와 차이점 및 문제 해결 방법을 포함한 보고서입니다.
source-git-commit: 95f81dafbe13f40487bad47f7dd41a6c80c589ee
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# 에 대한 FAQ [!UICONTROL Household] 보고서

## 방법 [!UICONTROL Household] 다른 사용자 지정 보고서와 다른 도달 및 빈도 보고서

다음 [!UICONTROL Household] 보고서 측정은 IP 주소를 기반으로 한 가구 수준의 다양한 차원에 걸쳐 도달, 노출 및 빈도를 측정합니다. 다른 사용자 지정 보고서는 장치 또는 쿠키 수준에서 생성됩니다.

예를 들어 한 세대 내의 세 개의 장치에 한 번의 노출이 제공되더라도 고유 세대 도달 지표는 1입니다.

### 지원되는 Dimension

다음 [!UICONTROL Household] 보고서는 [다음 차원](/help/dsp/reports/report-columns.md): &quot;[!UICONTROL Campaign],&quot; &quot;[!UICONTROL Package],&quot; &quot;[!UICONTROL Placement],&quot; &quot;[!UICONTROL Site/Apps]&quot;(중복 지표에 대한 액세스 권한을 제공하지 않음),&quot;[!UICONTROL Media Type],&quot; &quot;[!UICONTROL Feed Type],&quot; &quot;[!UICONTROL Device],&quot; &quot;[!UICONTROL Publisher],&quot; &quot;[!UICONTROL Audience],&quot; &quot;[!UICONTROL Creative Length],&quot; 및 사용자가 만든 배치 &quot;[!UICONTROL Tags].&quot; |

### 지원되는 지표

다음 [사용 가능한 지표](/help/dsp/reports/report-columns.md) 포함:

* 중복 지표: [!UICONTROL Frequency Overlap], [!UICONTROL Measurable Impressions (Overlap)], 및 [!UICONTROL Unique Household (Overlap)].

   겹치기 지표는 보고된 차원이나 차원 조합에 대해서만 발생하고 다른 차원에 대해서는 발생하지 않는 값입니다. <!-- For example, it might show the ?? -->

* 겹치지 않는 지표: [!UICONTROL Frequency], [!UICONTROL Incremental Household Reached], [!UICONTROL % Incremental Household Reached], [!UICONTROL Impressions], [!UICONTROL Measurable Impressions], 및 [!UICONTROL Unique Household Reached]

전환 지표 및 사용자 지정 목표는 지원되지 않습니다.

## 겹치는 지표와 겹치지 않는 지표의 차이점은 무엇입니까?

다음 그림은 세 캠페인(A, B, C)에 대한 세 가지 지표(고유 세대 도달, 증분 세대 도달 및 증분 세대(중복))를 보여줍니다.

![가구 중복 지표의 그림](/help/dsp/assets/household-overlap-metrics-illustration.png "가구 중복 지표의 그림")

* 고유 세대 도달(합계)은 각 캠페인 또는 각 원의 총 영역에서 도달한 고유 세대를 제공합니다. 그림에서 A가 도달한 고유 가구 = A + (A+B) + (A+C) + (A+B+C)가 도달한 증분 가구

* 증분 가구 도달은 캠페인에서만 도달한 고유 가구입니다. 그림에서 A, B, C가 도달한 증분 가구는 각각 A, B, C가 도달한 증분 가구이다.

* 증분 가구(겹치기)는 캠페인 또는 캠페인의 조합으로 도달한 고유 가구입니다. 그림에서 A, C가 도달한 증분 가구는 A+C이다.

## 워크플로

일반적인 단계에 따라 [사용자 지정 보고서 만들기](report-create.md).

다음 [!UICONTROL Household] 보고서에는 하나의 차원만 포함될 수 있습니다. 또한 a) 사이트/앱을 제외한 모든 차원별 중복 지표 또는 b) 비중복 지표를 포함할 수 있지만 둘 다 포함할 수는 없습니다.

## 의 몇 가지 제한 사항 [!UICONTROL Household] 보고? 

겹치기 지표가 있는 보고서는 최대 3개의 값 교차를 출력합니다. 예를 들어 지표를 사용하는 경우 [!UICONTROL Unique Household (Overlap)] 10개의 배치에 대해 개별 배치에 의해 도달된 고유한 가구, 임의의 두 배치의 조합에 의해 도달된 일반적인 가구, 및 임의의 세 배치의 조합에 의해 도달된 일반적인 가구를 볼 수 있습니다. 4개 이상의 배치에 의해 도달된 일반적인 가구를 볼 수 없다.

캠페인, 패키지 또는 배치 이외의 차원의 경우 보고서는 각 차원에서 최대 10개의 값을 지원합니다. 예를 들어 [!UICONTROL Unique Household Reached] 다음에 대한 보고서 [!UICONTROL Audience] 차원의 고유한 대상 수는 10보다 작거나 같아야 합니다. 10개 이상의 고유 대상을 포함하는 경우 빈 보고서가 생성됩니다.

## 내 도달 횟수와 고유 도달 거리가 서로 다른 이유는 무엇입니까? [!UICONTROL Custom] 보고서 및 [!UICONTROL Household] 보고?

의 다음 지표 [!UICONTROL Household] 보고서는 IP 주소의 실제 수를 사용하여 계산되지만 의 지표는 [!UICONTROL Custom] 보고서 모델을 사용하여 계산된 예상 숫자를 사용합니다. 그러나 불일치율은 10% 미만이어야 합니다.

## 보고서 구성 방법 [!UICONTROL Placement Tags] 차원?

배치용 태그를 생성하려면 다음을 수행합니다. [배치 설정 열기](/help/dsp/campaign-management/placements/placement-edit.md) 및 다음에 값 입력 [배치 태그 필드](/help/dsp/campaign-management/placements/placement-settings.md).
 
배치에 여러 태그가 포함되어 있는 경우 보고서는 전체 문자열을 하나의 태그로 간주합니다. 보고서에는 각 고유 문자열에 대해 하나의 행이 포함됩니다.

## [!UICONTROL Household] 보고서 및 데이터 비교 [!DNL Advanced Measurement Services]

가구 기반 도달 및 빈도에 대한 고급 보고를 위해 [[!DNL Strategic Advertising Consulting] 팀](/help/dsp/introduction/advanced-measurement-services.md) 는 전체적인 전략적 권장 사항과 함께 고도로 사용자 정의 가능한 보고서를 제공할 수 있습니다. 에 대한 자세한 내용 [!DNL Advanced Measurement Services], Adobe 계정 팀에 문의하십시오.

### 이미 사용하고 있는 경우 [!DNL Advanced Measurement Services], 를 사용해야 하는 이유 [!UICONTROL Household] 보고?

다음 [!UICONTROL Household] 보고서는 클라이언트가 가구 수준의 도달 범위와 빈도 지표를 실시간으로 자율적으로 가져올 수 있도록 합니다.

### 두 가지를 모두 사용할 수 있습니까 [!UICONTROL Household] 보고 및 [!DNL Advanced Measurement Services]? 

이상적인 사용 사례는 두 가지를 모두 사용하는 것입니다. [!UICONTROL Household] 보고서 및 [!DNL Advanced Measurement Services] 보고 및 컨설팅 서비스 다음을 고려하십시오. [!UICONTROL Household] 일상적인 최적화를 알리기 위한 트랜잭션으로 보고 [!DNL Advanced Measurement Services] 보다 전략적으로, 중요한 비즈니스 목표와 관련된 전체적인 학습과 요령을 알리기 위함입니다.

>[!MORELIKETHIS]
>
>* [사용자 정의 보고서 정보](/help/dsp/reports/report-about.md)
>* [사용자 지정 보고서 만들기](/help/dsp/reports/report-create.md)
>* [사용자 지정 보고서 편집](/help/dsp/reports/report-edit.md)
>* [사용자 지정 보고서 설정](/help/dsp/reports/report-settings.md)
>* [사용 가능한 보고서 열](/help/dsp/reports/report-columns.md)
