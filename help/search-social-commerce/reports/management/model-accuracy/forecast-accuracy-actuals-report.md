---
title: '[!UICONTROL Forecast Accuracy (Actuals) Report]'
description: 에 대해 알아보기 [!UICONTROL Forecast Accuracy (Actuals) Report], 데이터 열 포함.
exl-id: ff49284a-2d13-48bf-a172-3bd461db7a3c
feature: Search Reports, Search Model Accuracy Reports
source-git-commit: 97111c6cd38098cac72b8773390afd254a017d1d
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# 다음 [!UICONTROL Forecast Accuracy (Actuals) Report]

이 보고서는 각 포트폴리오에 대한 광고 네트워크의 실제 노출, 클릭, 비용 및 수익 데이터를 일별로 보여줍니다.

## 사용 가능한 열

다음은 각 보고서에 자동으로 포함되는 열입니다. 열을 추가할 수 없습니다.

| 열 | 기본? | 설명 |
|----|----|----|
| [!UICONTROL Portfolio Group Name] | 기본값 | 포트폴리오가 속한 포트폴리오 그룹의 이름입니다. |
| [!UICONTROL Portfolio ID] | 기본값 | 숫자 포트폴리오 ID입니다. |
| [!UICONTROL EF Portfolio Group ID] | 기본값 | 포트폴리오가 속한 포트폴리오 그룹의 숫자 ID입니다. |
| [!UICONTROL Portfolio] | 기본값 | 포트폴리오입니다. |
| [!UICONTROL Portfolio Status] | 기본값 | 포트폴리오 상태:<ul><li><i>[!UICONTROL Optimize]:</i> 최적화 기능은 관련 캠페인에 대한 클릭 및 매출 데이터를 수집하고, 데이터를 모델링하여 입찰을 최적화하며, 입찰 및/또는 캠페인 예산(최적화 유형 및 캠페인 입찰 전략에 따라)을 최적화하는 것입니다.</li><li><i>[!UICONTROL Active]:</i> 최적화 기능은 관련 캠페인에 대한 클릭 및 매출 데이터를 수집하고 데이터를 모델링하지만 입찰이나 캠페인 예산을 최적화하지 않습니다.</li><li><i>[!UICONTROL Inactive]:</i> 최적화 기능은 보고 목적으로 관련 캠페인에 대한 클릭 데이터를 수집하는 것이지만, 데이터를 모델링하거나 입찰 또는 캠페인 예산을 최적화하지 않습니다. |
| [!UICONTROL Day of Week] | 기본값 | 보고된 요일: <i>[!UICONTROL Sunday]</i>, <i>[!UICONTROL Monday]</i>, <i>[!UICONTROL Tuesday]</i>, <i>[!UICONTROL Wednesday]</i>, <i>[!UICONTROL Thursday]</i>, <i>[!UICONTROL Friday]</i>, 또는 <i>[!UICONTROL Saturday]</i>. |
| [!UICONTROL Event Date] | 기본값 | 보고된 날짜. |
| [!UICONTROL Device] | 기본값 | (Google Ads, Microsoft® Advertising, Yahoo! 네트워크 표시, Yahoo! Japan Ads 및 Yahoo Native 캠페인) 광고가 표시된 디바이스 유형: <i>[!UICONTROL Computers]</i>, <i>[!UICONTROL Mobile]</i>, <i>[!UICONTROL Tablets]</i>, <i>[!UICONTROL Other]</i>, 또는 <i>[!UICONTROL N/A]</i> (값 없음). 다른 광고 네트워크의 행에는 다음 값이 있습니다. <i>[!UICONTROL N/A]</i>.<br><br>검색 캠페인에서 키워드, 광고 및/또는 광고 확장에 대한 추적 템플릿 또는 대상 URL에 디바이스별로 데이터를 추적하기 위한 매개 변수가 포함된 경우(<code>&amp;ev_dvc={device}&amp;ev_dvm={devicemodel}</code>) 광고를 클릭할 때 전환 데이터도 각 장치 유형의 행에 포함됩니다. 그렇지 않으면 전환 데이터가 디바이스 유형에 귀속될 수 없는 경우 &quot;가 있는 별도의 행에 집계됩니다.[!UICONTROL Device]&quot; 값 <i>[!UICONTROL N/A]</i>. |
| [!UICONTROL Revenue] | 기본값 | 총 매출액. |
| [!UICONTROL Impressions] | 기본값 | 총 노출 횟수. |
| [!UICONTROL Clicks] | 기본값 | 총 클릭수입니다. |
| [!UICONTROL Cost] | 기본값 | 총 비용. |

>[!MORELIKETHIS]
>
>* [모델 정확도 보고서 정보](/help/search-social-commerce/reports/management/model-accuracy/model-accuracy-report-about.md)
>* [다음 [!UICONTROL Forecast Accuracy Report]](forecast-accuracy-report.md)
>* [모델 정확도 보고서 생성](model-accuracy-report-generate.md)
>* [모델 정확도 보고서 설정](/help/search-social-commerce/reports/management/model-accuracy/model-accuracy-report-settings.md)
