---
title: 세대 보고서에 대한 FAQ
description: 가구 보고서가 다른 보고서 및 문제 해결과 어떻게 다른지 포함하여 가구 도달 범위, 빈도 및 전환 데이터에 대해 자세히 알아보십시오.
exl-id: 3ffd178e-de41-4663-b85f-bd8ce3eb0dad
source-git-commit: e16bc62127a708de8f4deb1eddfa53a14405cbc2
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 0%

---

# 세대 보고서에 대한 FAQ

## [!UICONTROL Household Reach & Frequency] 보고서

### [!UICONTROL Household Reach & Frequency] 보고서는 다른 사용자 지정 보고서와 어떻게 다릅니까?

[!UICONTROL Household Reach & Frequency] 보고서 측정은 IP 주소를 기반으로 하는 가구 수준의 다양한 차원에 걸쳐 도달, 노출, 빈도를 측정합니다. 다른 사용자 지정 보고서는 장치 또는 쿠키 수준에서 생성됩니다.

예를 들어 한 세대 내의 세 개의 장치에 한 번의 노출이 제공되더라도 고유 세대 도달 지표는 1입니다.

#### 지원되는 Dimension

[!UICONTROL Household Reach & Frequency] 보고서는 [다음 차원](/help/dsp/reports/report-columns.md)을 지원합니다. &quot;[!UICONTROL Campaign],&quot; &quot;[!UICONTROL Package],&quot; &quot;[!UICONTROL Placement],&quot; &quot;[!UICONTROL Site/Apps]&quot;(중복 지표에 대한 액세스 권한 제공 안 함), &quot;[!UICONTROL Media Type],&quot; &quot;[!UICONTROL Feed Type],&quot; &quot;[!UICONTROL Device],&quot; &quot;[!UICONTROL Publisher],&quot; &quot;[!UICONTROL Audience],&quot;[!UICONTROL Creative Length]&quot; 및 사용자가 만든 배치 &quot;[!UICONTROL Tags].&quot; |

#### 지원되는 지표

[사용 가능한 지표](/help/dsp/reports/report-columns.md)에는 다음이 포함됩니다.

* 중복 지표: [!UICONTROL Frequency Overlap], [!UICONTROL Measurable Impressions (Overlap)] 및 [!UICONTROL Unique Household (Overlap)].

  겹치기 지표는 보고된 차원이나 차원 조합에 대해서만 발생하고 다른 차원에 대해서는 발생하지 않는 값입니다. <!-- For example, it might show the ?? -->

* 겹치지 않는 지표: [!UICONTROL Frequency], [!UICONTROL Incremental Household Reached], [!UICONTROL % Incremental Household Reached], [!UICONTROL Impressions], [!UICONTROL Measurable Impressions] 및 [!UICONTROL Unique Household Reached]

전환 지표 및 사용자 지정 목표는 지원되지 않습니다.

### 겹치는 지표와 겹치지 않는 지표의 차이점은 무엇입니까?

다음 그림은 세 캠페인(A, B, C)에 대한 세 가지 지표(고유 세대 도달, 증분 세대 도달 및 증분 세대(중복))를 보여줍니다.

![가구 중복 지표의 그림](/help/dsp/assets/household-overlap-metrics-illustration.png "가구 중복 지표의 그림")

* 고유 세대 도달(합계)은 각 캠페인 또는 각 원의 총 영역에서 도달한 고유 세대를 제공합니다. 그림에서 A가 도달한 고유 가구 = A + (A+B) + (A+C) + (A+B+C)가 도달한 증분 가구

* 증분 가구 도달은 캠페인에서만 도달한 고유 가구입니다. 그림에서 A, B, C가 도달한 증분 가구는 각각 A, B, C가 도달한 증분 가구이다.

* 증분 가구(겹치기)는 캠페인 또는 캠페인의 조합으로 도달한 고유 가구입니다. 그림에서 A, C가 도달한 증분 가구는 A+C이다.

### 워크플로

일반적인 단계에 따라 [사용자 지정 보고서를 만듭니다](report-create.md).

[!UICONTROL Household Reach & Frequency] 보고서에는 하나의 차원만 포함될 수 있습니다. 또한 a) 사이트/앱을 제외한 모든 차원별 중복 지표 또는 b) 비중복 지표를 포함할 수 있지만 둘 다 포함할 수는 없습니다.

### [!UICONTROL Household Reach & Frequency] 보고서의 일부 제한 사항은 무엇입니까?

겹치기 지표가 있는 보고서는 최대 3개의 값 교차를 출력합니다. 예를 들어 10개의 배치에 대해 [!UICONTROL Unique Household (Overlap)] 지표를 사용하는 경우 개별 배치에 의해 도달된 고유한 가구, 두 배치의 조합에 의해 도달된 일반적인 가구, 세 배치의 조합에 의해 도달된 일반적인 가구를 볼 수 있습니다. 4개 이상의 배치에 의해 도달된 일반적인 가구를 볼 수 없다.

캠페인, 패키지 또는 배치 이외의 차원의 경우 보고서는 각 차원에서 최대 10개의 값을 지원합니다. 예를 들어 [!UICONTROL Audience] 차원에 대한 [!UICONTROL Unique Household Reached] 보고서를 생성하려면 고유한 대상의 수가 10보다 작거나 같아야 합니다. 10개 이상의 고유 대상을 포함하는 경우 빈 보고서가 생성됩니다.

### [!UICONTROL Custom] 보고서와 [!UICONTROL Household Reach & Frequency] 보고서 간에 빈도 및 고유 도달 값이 다른 이유는 무엇입니까?

[!UICONTROL Household] 보고서의 이러한 지표는 IP 주소의 실제 수를 사용하여 계산되지만 [!UICONTROL Custom] 보고서의 지표는 모델을 사용하여 계산된 예상 수를 사용합니다. 그러나 불일치율은 10% 미만이어야 합니다.

### [!UICONTROL Placement Tags] 차원에 대한 보고서를 구성하려면 어떻게 해야 합니까?

배치용 태그를 만들려면 [배치 설정을 열고](/help/dsp/campaign-management/placements/placement-edit.md) [배치 태그 필드에 값을 입력하십시오](/help/dsp/campaign-management/placements/placement-settings.md).

배치에 여러 태그가 포함되어 있는 경우 보고서는 전체 문자열을 하나의 태그로 간주합니다. 보고서에는 각 고유 문자열에 대해 하나의 행이 포함됩니다.

## [!UICONTROL Household Conversions] 보고서

### [!UICONTROL Household Conversions] 보고서에서 지원되는 속성 메서드 유형은 무엇입니까?

두 가지 유형의 속성 메서드가 지원됩니다.

* [!UICONTROL Unique]: 전환 경로에 있는 차원 값(예: 장치 또는 배치)의 횟수를 카운트합니다.

* [!UICONTROL Multi-Touch Attribution (MTA)]: 전환 경로에 있는 차원 값(예: 장치 또는 배치)의 발생 빈도에 따라 각 전환의 크레딧을 배포합니다. 예를 들어 전환 전에 CTV에 8개, 모바일에 2개로 총 10개의 노출이 있었다면 크레딧의 80%(0.8)는 CTV 화면에, 0.2는 모바일에 제공됩니다.

### 가구 전환 보고는 Adobe Analytics의 CTV 뷰스루 보고와 어떻게 다릅니까?

[!DNL Analytics]의 CTV 뷰스루 데이터는 [!DNL Analytics] 추적 기능을 제공하며, 가구 전환 데이터는 Adobe Advertising 전환 추적을 사용하여 수집된 데이터를 사용합니다. 또한 [!DNL Analytics]의 DSP 속성 논리에서는 마지막 이벤트만 사용하지만 가구 전환 보고에서는 고유한 및 MTA라는 두 가지 다른 속성 방법을 지원합니다.

### [!DNL Analytics for Advertising]과(와) 사용자 지정 보고서 모두에서 CTV 뷰스루 데이터를 볼 수 있습니까?

[!DNL Analytics for Advertising]이(가) 없는 광고주는 가구 전환 보고에 가구 전환 보고서만 사용할 수 있습니다.

조직에 [!DNL Analytics for Advertising]이(가) 있는 경우 두 유형의 보고를 함께 사용하십시오. CTV 뷰스루 보고는 광범위한 채널 분석, 사이트 동작 등에 적합하지만, 사용자 지정 보고서는 전환율을 유도하는 요인을 나타내기 위해 세부적인 보기(미디어 유형, 게시자 등으로 분류된 데이터 포함)를 제공합니다.

## [!UICONTROL Household Reach & Frequency] 및 [!UICONTROL Household Conversions]개 보고서와 [!DNL Advanced Measurement Services]의 데이터 비교

가족 단위 기반 도달 범위와 빈도 또는 전환에 대한 고급 보고를 위해 [[!DNL Strategic Advertising Consulting] 팀](/help/dsp/introduction/advanced-measurement-services.md)은(는) 전체적인 전략적 권장 사항과 함께 사용자 지정성이 높은 보고서를 제공할 수 있습니다. [!DNL Advanced Measurement Services]에 대한 자세한 내용은 Adobe 계정 팀에 문의하십시오.

### 이미 [!DNL Advanced Measurement Services]을(를) 사용하고 있다면 [!UICONTROL Household Reach & Frequency] 및 [!UICONTROL Household Conversions] 보고서를 사용해야 하는 이유는 무엇입니까?

[!UICONTROL Household Reach & Frequency] 및 [!UICONTROL Household Conversions] 보고서를 통해 클라이언트는 가구 수준의 도달, 빈도 및 전환 지표를 각각 실시간으로 자율적으로 가져올 수 있습니다.

### [!UICONTROL Household Reach & Frequency] 및 [!UICONTROL Household Conversions] 보고서와 [!DNL Advanced Measurement Services]을(를) 모두 사용할 수 있습니까?

가장 좋은 사용 사례는 [!UICONTROL Household] 보고서와 [!DNL Advanced Measurement Services] 보고 및 컨설팅 서비스를 함께 사용하는 것입니다. 매일 최적화를 알리기 위한 트랜잭션 보고서로 [!UICONTROL Household]을(를) 고려하며, 중요한 비즈니스 목표와 관련된 전체적인 학습과 성과를 알리기 위한 보다 전략적인 [!DNL Advanced Measurement Services]을(를) 고려합니다.

>[!MORELIKETHIS]
>
>* [사용자 지정 보고서 정보](/help/dsp/reports/report-about.md)
>* [사용자 지정 보고서 만들기](/help/dsp/reports/report-create.md)
>* [사용자 지정 보고서 편집](/help/dsp/reports/report-edit.md)
>* [사용자 지정 보고서 설정](/help/dsp/reports/report-settings.md)
>* [사용 가능한 보고서 열](/help/dsp/reports/report-columns.md)
