---
title: '[!UICONTROL Forecast Accuracy Report]'
description: 데이터 열을 포함하여 예측 정확도 보고서에 대해 알아봅니다.
exl-id: 2bb36728-ae14-441b-bcda-fa457f5cf664
feature: Search Reports, Search Model Accuracy Reports
source-git-commit: 97111c6cd38098cac72b8773390afd254a017d1d
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---

# 다음 [!UICONTROL Forecast Accuracy Report]

이 보고서는 지정된 포트폴리오에 대한 일별 비용 및 수익 모델의 정확도를 보여줍니다. 기본적으로 각 포트폴리오에 대한 일일 예측 및 실제 수익, 비용, 클릭 수 및 예측의 정확도를 포함합니다. 여기에는 현재 포트폴리오에 매핑된 캠페인의 데이터가 포함됩니다.

이전 18개월의 데이터를 볼 수 있습니다.

>[!NOTE]
>
>* 이 보고서는 포트폴리오 수준과 동일한 데이터를 제공합니다 [!UICONTROL Model Accuracy Report] 여러 포트폴리오에서 실행하고 속성 규칙을 변경할 수 있는 경우를 제외하고, 사용자 지정 매개 변수를 사용하여 보고서를 실행하고 예약할 수도 있으며, 스프레드시트 피드를 만드는 데 사용할 수도 있습니다.
>
>* 가장 좋은 방법은 를 보는 것입니다. [!UICONTROL Forecast Accuracy Report] 포트폴리오의 지출 전략과 관계없이 대부분의 포트폴리오에는 고유의 요일 트렌드가 표시되기 때문에 최소 지난 7일 동안 지속됩니다. 최적화 기능은 이 트렌드를 고려하여 그에 따라 지출을 할당합니다.
>
>* 비용 예측의 경우 지난 7일 동안 10%의 편차가 허용되는 것으로 간주되므로 예측된 지출의 90%에서 110% 사이인 실제 지출이 좋습니다. 매출 예측의 경우 지난 7일 동안의 15% 편차가 허용되는 것으로 간주되므로 예측된 지출의 85%에서 115% 사이인 실제 매출은 좋습니다. 편차가 더 큰 예보는 조사해야 한다.
>
>* 포트폴리오의 키워드가 입찰 전환 제한과 연결된 경우 포트폴리오는 입찰 전환으로 인해 발생하는 총 금액만큼 과소 또는 과소 소비됩니다. 그 결과 예측비용 열은 증감된 지출만큼 목표 지출에서 벗어나게 된다.

## 사용 가능한 열

다음은 각 보고서에 사용할 수 있는 열입니다. 기본 열은 기본적으로 자동으로 포함됩니다. 다음에서 사용 가능한 사용자 정의 열을 추가할 수 있습니다. [!UICONTROL Columns] 섹션에 자세히 설명되어 있습니다.

| 열 | 기본? | 설명 |
|----|----|----|
| [!UICONTROL Portfolio] | 기본값 | 포트폴리오입니다. |
| [!UICONTROL Day of Week] | 기본값 | 보고된 요일: <i>[!UICONTROL Sunday]</i>, <i>[!UICONTROL Monday]</i>, <i>[!UICONTROL Tuesday]</i>, <i>[!UICONTROL Wednesday]</i>, <i>[!UICONTROL Thursday]</i>, <i>[!UICONTROL Friday]</i>, 또는 <i>[!UICONTROL Saturday]</i>. |
| [!UICONTROL Start Date] | 기본값 | 보고된 첫 번째 날. |
| [!UICONTROL End Date] | 기본값 | 마지막으로 보고된 날짜입니다. |
| [!UICONTROL Predicted Revenue] | 기본값 | 포트폴리오의 예상 매출액. |
| [!UICONTROL Revenue] | 기본값 | 포트폴리오의 실제 수익. |
| [!UICONTROL Revenue Accuracy] | 기본값 | 수익률 예측의 정확도(백분율로 표시). |
| [!UICONTROL Predicted Cost] | 기본값 | 포트폴리오에 대한 예상 비용입니다. |
| [!UICONTROL Cost] | 기본값 | 포트폴리오의 실제 비용. |
| [!UICONTROL Cost Accuracy] | 기본값 | 백분율로 표시되는 비용 예측의 정확성. |
| [!UICONTROL Predicted Clicks] | 기본값 | 포트폴리오에 대해 예측된 클릭 수입니다. |
| [!UICONTROL Clicks] | 기본값 | 포트폴리오에 대한 실제 클릭 수입니다. |
| [!UICONTROL Click Accuracy] | 기본값 | 백분율로 표시되는 클릭 예측의 정확도입니다. |
| [!UICONTROL EF Portfolio Group ID] | 기본값 | 포트폴리오가 속한 포트폴리오 그룹의 숫자 ID입니다. |
| [!UICONTROL Portfolio Group Name] | 기본값 | 포트폴리오가 속한 포트폴리오 그룹의 이름입니다. |
| [!UICONTROL Portfolio ID] | 기본값 | 숫자 포트폴리오 ID입니다. |

>[!MORELIKETHIS]
>
>* [모델 정확도 보고서 정보](/help/search-social-commerce/reports/management/model-accuracy/model-accuracy-report-about.md)
>* [다음 [!UICONTROL Forecast Accuracy (Actuals) Report]](forecast-accuracy-actuals-report.md)
>* [모델 정확도 보고서 생성](model-accuracy-report-generate.md)
>* [모델 정확도 보고서 설정](/help/search-social-commerce/reports/management/model-accuracy/model-accuracy-report-settings.md)
