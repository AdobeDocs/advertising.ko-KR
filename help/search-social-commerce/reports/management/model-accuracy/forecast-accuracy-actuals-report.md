---
title: '[!UICONTROL Forecast Accuracy (Actuals) Report]'
description: 데이터 열을 포함하여 [!UICONTROL Forecast Accuracy (Actuals) Report]에 대해 알아봅니다.
exl-id: 659e11c7-5fed-4d91-a73f-7c435d36634f
feature: Search Reports, Search Model Accuracy Reports
TQID: https://experienceleague.adobe.com/wQyO42Dt5McqK23z-adEP-BAxxTrBk9RJi0I-4noP0I
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 527ca2bb74de388c13ba1ce5bde3f8be1cead8d0
workflow-type: tm+mt
source-wordcount: 321
ht-degree: 0%

---

# [!UICONTROL Forecast Accuracy (Actuals) Report]

이 보고서는 각 포트폴리오에 대한 광고 네트워크의 실제 노출, 클릭, 비용 및 수익 데이터를 일별로 보여줍니다.

## 사용 가능한 열

다음은 각 보고서에 자동으로 포함되는 열입니다. 열을 추가할 수 없습니다.

| 열 | 기본? | 설명 |
|----|----|----|
| [!UICONTROL Portfolio Group Name] | 기본값 | 포트폴리오가 속한 포트폴리오 그룹의 이름입니다. |
| [!UICONTROL Portfolio ID] | 기본값 | 숫자 포트폴리오 ID입니다. |
| [!UICONTROL EF Portfolio Group ID] | 기본값 | 포트폴리오가 속한 포트폴리오 그룹의 숫자 ID입니다. |
| [!UICONTROL Portfolio] | 기본값 | 포트폴리오입니다. |
| [!UICONTROL Portfolio Status] | 기본값 | 포트폴리오 상태:<ul><li><i>[!UICONTROL Optimize]:</i> 최적화 기능은 관련 캠페인에 대한 클릭 및 매출 데이터를 수집하고, 최적화에 사용된 데이터를 모델링하고, 입찰, 캠페인 예산 및 캠페인 입찰 전략 대상(최적화 유형 및 입찰 전략에 따라)을 최적화하는 것입니다.</li><li><i>[!UICONTROL Active]:</i> 최적화 기능이 관련 캠페인에 대한 클릭 및 매출 데이터를 수집하고 데이터를 모델링하고 있지만 입찰 또는 캠페인 예산을 최적화하지 않습니다.</li><li><i>[!UICONTROL Inactive]:</i> 최적화 기능이 보고 목적으로 관련 캠페인에 대한 클릭 데이터를 수집하고 있지만 데이터를 모델링하거나 입찰 또는 캠페인 예산을 최적화하지 않습니다. |
| [!UICONTROL Day of Week] | 기본값 | 보고된 요일: <i>[!UICONTROL Sunday]</i>, <i>[!UICONTROL Monday]</i>, <i>[!UICONTROL Tuesday]</i>, <i>[!UICONTROL Wednesday]</i>, <i>[!UICONTROL Thursday]</i>, <i>[!UICONTROL Friday]</i> 또는 <i>[!UICONTROL Saturday]</i>. |
| [!UICONTROL Event Date] | 기본값 | 보고된 날짜. |
| [!UICONTROL Device] | 기본값 | (Google Ads, Microsoft Advertising, Yahoo! 네트워크 표시, Yahoo! Japan Ads 및 Yahoo Native 캠페인) 광고가 표시된 장치 유형: <i>[!UICONTROL Computers]</i>, <i>[!UICONTROL Mobile]</i>, <i>[!UICONTROL Tablets]</i>, <i>[!UICONTROL Other]</i> 또는 <i>[!UICONTROL N/A]</i>(값 없음). 다른 광고 네트워크 행의 값은 <i>[!UICONTROL N/A]</i>입니다.<br><br>검색 캠페인에서 키워드, 광고 및/또는 광고 확장에 대한 추적 템플릿 또는 대상 URL에 장치별로 데이터를 추적할 매개 변수가 포함된 경우(<code>&amp;ev_dvc={device}&amp;ev_dvm={devicemodel})</code>) 광고를 클릭할 때 전환 데이터도 각 장치 유형의 행에 포함됩니다. 그렇지 않으면 전환 데이터가 장치 유형에 귀속될 수 없는 경우 &quot;[!UICONTROL Device]&quot; 값이 <i>[!UICONTROL N/A]</i>인 별도의 행에서 집계됩니다. |
| [!UICONTROL Revenue] | 기본값 | 총 매출액. |
| [!UICONTROL Impressions] | 기본값 | 총 노출 횟수. |
| [!UICONTROL Clicks] | 기본값 | 총 클릭수입니다. |
| [!UICONTROL Cost] | 기본값 | 총 비용. |

>[!MORELIKETHIS]
>
>* [모델 정확도 보고서 정보](/help/search-social-commerce/reports/management/model-accuracy/model-accuracy-report-about.md)
>* [[!UICONTROL Forecast Accuracy Report]](forecast-accuracy-report.md)
>* [모델 정확도 보고서 생성](model-accuracy-report-generate.md)
>* [모델 정확도 보고서 설정](/help/search-social-commerce/reports/management/model-accuracy/model-accuracy-report-settings.md)
