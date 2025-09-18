---
title: Insights 정보
description: 시각화를 통한 성능 통찰력에 대해 알아봅니다.
feature: DSP Campaigns, DSP Packages, DSP Placements
exl-id: 0b7943c4-650c-4515-ae19-4417714ea7dd
source-git-commit: 0f022babeab6c044949760cedc103323eb0cc950
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 0%

---

# Insights 정보

*Beta 기능*

시각화를 통한 높은 수준의 성능 통찰력은 캠페인을 효율적으로 최적화하고 성과를 확장할 수 있는 새로운 기회를 발견하는 데 필요한 정보를 제공합니다. 지정된 광고주의 캠페인 간에 데이터를 보거나 더 낮은 수준으로 드릴다운할 수 있습니다.

성능 인사이트를 사용하여 다음을 수행할 수 있습니다.

* 전략적 계획 수립 및 정보에 입각한 의사 결정을 위한 장기적인 추세를 추적합니다.

* 더 나은 결과를 얻을 수 있는 기회를 식별합니다.

* 원시 데이터를 얻는 것과 실행 가능한 통찰력을 얻는 것 사이의 시간을 줄여 효율성을 향상시킵니다.

Microsoft Excel 스프레드시트(XLSX) 형식으로 시각화하지 않고 탭의 모든 시각화를 PDF 파일로 내보내거나 특정 insight의 데이터를 다운로드할 수 있습니다.

[날짜 범위를 변경하고, 보기를 구성하고, 사용자 지정 보기를 ](/help/dsp/campaign-management/reports/campaign-data-views-manage.md){target="_blank"} 캠페인 관리 보기와 같이 저장할 수도 있습니다.

## Insights 유형

### [!UICONTROL Home] 탭

[!UICONTROL Home] 탭은 광고주의 모든 캠페인에서 주요 표준, 성능 및 조회 지표를 제공합니다. 기본적으로 특정 광고주와 사용자 지정 목표에 대한 교차 배치 데이터가 표시됩니다. 선택적으로 다른 광고주, 다른 사용자 지정 목표 또는 특정 배치에 대한 데이터를 표시하도록 필터를 구성할 수 있습니다. <!-- I don't see campaigns or packages anymore:  You can optionally configure filters to show data for a different advertiser or data for only specific campaigns, packages, custom goals, and placements. --> 인사이트는 다음과 같습니다.

* **[!UICONTROL Trends]:** 고객이 지정한 세 개의 지표(기본적으로 [!UICONTROL Net Spend], [!UICONTROL Impressions] 및 [!UICONTROL Net CPM])에 대한 트렌드 차트입니다.

* **[!UICONTROL Delivery Breakdown]:** 캠페인, 게시자 및 미디어 유형과 같이 고객이 지정한 세 차원별로 특정 지표에 대한 데이터의 분류입니다. 각 차원 분류에 대해 다른 지표를 선택할 수 있습니다.

### [!UICONTROL Household Reach] 탭

[!UICONTROL Household Reach] 탭은 광고주의 모든 캠페인에서 가정용 도달 지표를 제공합니다. 기본적으로 캠페인 간 데이터가 표시됩니다. 선택적으로 다른 광고주, 특정 캠페인, 패키지 또는 배치 전체, 특정 패키지 또는 배치에 대한 데이터를 표시하도록 필터를 구성할 수 있습니다. 인사이트는 다음과 같습니다.

* **[!UICONTROL Trends]:** 고객이 지정한 세 가지 지표(기본적으로 [!UICONTROL Net Spend], [!UICONTROL Unique Reach] 및 [!UICONTROL Net CPM])에 대한 일별 또는 주별 트렌드 차트입니다.

* **[!UICONTROL Incremental Household Reach]:** [!UICONTROL Media Type], [!UICONTROL Device Type] 또는 [!UICONTROL Inventory Type]까지 증가하는 가족 단위 도넛형 도넛형 차트입니다. *가구 증가 도달*&#x200B;은(는) 단일 미디어, 장치 또는 인벤토리 유형을 통해서만 도달 가능한 가구로 정의됩니다.

* **[!UICONTROL Reach Breakdown]:** [!UICONTROL Media Type], [!UICONTROL Device Type] 또는 [!UICONTROL Inventory Type]까지 증가하는 고유한 가구 도달 횟수와 겹치는 가구 도달 횟수입니다.

  *가구 증가 도달*&#x200B;은(는) 단일 미디어, 장치 또는 인벤토리 유형을 통해서만 도달 가능한 가구로 정의됩니다. *겹치는 가구 연결*&#x200B;은(는) 여러 미디어, 장치 또는 인벤토리 유형에 의해 연결된 가구로 정의됩니다.

* **[!UICONTROL Top Performers]:** [!UICONTROL Unique Reach], [!UICONTROL Net Spend] 및 [!UICONTROL Cost per Reach]별 성과가 가장 좋은 캠페인, 배치, 패키지, 게시자, 사이트/앱, 미디어 유형, 인벤토리 유형 또는 장치 유형입니다.

* **[!UICONTROL Performance Analysis]:** 패키지, 게시자 또는 사이트/앱별 [!UICONTROL Cost per Reach] 및 [!UICONTROL Net Spend] 이 insight을 사용하여 중요한 증분 도달 가능성을 보여 주는 패키지, 게시자 또는 사이트/앱을 확인하십시오.

  각 버블의 크기는 증분 도달 점수를 나타내며, 버블이 클수록 평균 증분 도달 점수가 높습니다. 버블에 대한 전체 엔티티 이름 및 주요 지표를 보려면 버블 위에 커서를 놓습니다.

  영향 수준은 다음과 같습니다.

   * **높은 영향:** 예산을 늘리는 것이 좋습니다.
   * **영향 중재**
   * **제한된 영향:**&#x200B;에 주의가 필요합니다.

### [!UICONTROL Household Conversion] 탭

[!UICONTROL Household Conversion] 탭은 광고주의 모든 캠페인<!-- active only? -->에서 가구 전환 지표를 제공합니다. 기본적으로 특정 광고주 및 특정 전환 지표에 대한 캠페인 간 데이터가 표시됩니다. 선택적으로 다른 광고주나 전환 지표, 특정 캠페인, 패키지 또는 배치 전체, 특정 패키지 또는 배치에 대한 데이터를 표시하도록 필터를 구성할 수 있습니다. 인사이트는 다음과 같습니다.

* **[!UICONTROL Trends]:** 고객이 지정한 세 가지 지표(기본적으로 [!UICONTROL Net Spend], [!UICONTROL Conversions] 및 [!UICONTROL Net CPM])에 대한 일별 또는 주별 트렌드 차트입니다.

* **[!UICONTROL Conversion Participation Overview]:** 대부분의 가정 전환을 초래하는 미디어 유형, 인벤토리 유형 및 장치 유형을 보여주는 막대 차트입니다.

  전환 확인 기간(30일) 내에 전달된 노출은 전환 참여에 유효한 것으로 간주됩니다.

* **[!UICONTROL Top Performers]:** 고객이 지정한 세 가지 지표(기본적으로 [!UICONTROL Net Spend], [!UICONTROL CPA] 및 [!UICONTROL Conversions])에 대한 성능을 유도하는 캠페인, 패키지, 배치, 게시자, 사이트/앱, 미디어 유형 및 인벤토리 유형의 테이블입니다. 상위 수행자가 먼저 나열됩니다.

* **[!UICONTROL Performance Analysis]:** 패키지, 게시자 또는 사이트/앱별 [!UICONTROL CPA] 및 [!UICONTROL Net Spend] 이 insight을 사용하여 중요한 증분 도달 가능성을 보여 주는 패키지, 게시자 또는 사이트/앱을 확인하십시오.

  각 버블의 크기는 증분 도달 점수를 나타내며, 버블이 클수록 평균 증분 도달 점수가 높습니다. 버블에 대한 전체 엔티티 이름 및 주요 지표를 보려면 버블 위에 커서를 놓습니다.

  영향 수준은 다음과 같습니다.

   * **높은 영향:** 예산을 늘리는 것이 좋습니다.
   * **영향 중재**
   * **제한된 영향:**&#x200B;에 주의가 필요합니다.

## 성능 인사이트 열기

* (모든 캠페인에 대한 인사이트를 열려면) 기본 메뉴에서 **[!UICONTROL Insights BETA]**&#x200B;을(를) 클릭합니다.

* (특정 캠페인, 패키지 또는 배치에 대한 인사이트를 열려면) [!UICONTROL Campaigns], [!UICONTROL Packages] 또는 [!UICONTROL Placements] 보기에서 엔터티 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Insights]**&#x200B;을(를) 클릭합니다.

* (특정 배치에 대한 인사이트를 열려면) [!UICONTROL Campaigns], [!UICONTROL Packages] 또는 [!UICONTROL Placements] 보기에서 엔터티 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Analyze]** > **[!UICONTROL Insights]** 을 클릭합니다.

## 탭에 필터 적용

1. 탭 상단의 도구 모음에서 ![필터 단추](/help/dsp/assets/filter.png)를 클릭합니다.

1. 왼쪽 열에서 차원을 선택한 다음 오른쪽 열에서 하나 이상의 값을 선택합니다.

   한 번에 한 명의 광고주만 선택할 수 있습니다.

1. **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 데이터 범위를 더 좁히려면 도구 모음에서 엔티티 유형을 선택한 다음 특정 엔티티 값(단일 캠페인, 패키지 또는 배치)을 선택합니다.

## insight에 대해 보고된 Dimension 변경

* 드롭다운 메뉴에서 insight의 왼쪽 상단으로 차원을 선택합니다.

## insight에 대해 보고된 지표 변경

전환 지표의 경우, Adobe Advertising 추적 및 Adobe Analytics 추적 전환 모두에 대해 지원을 사용할 수 있습니다.

1. insight 오른쪽 상단에서 ![지표 설정](/help/dsp/assets/metric-settings.png "지표 설정")을 클릭합니다.

1. 지표를 선택한 다음 **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

## 탭에 대한 모든 시각화를 PDF 파일로 내보내기

* 탭 위에서 **[!UICONTROL ...]** > **[!UICONTROL Export]**&#x200B;을(를) 클릭합니다.

  파일은 브라우저의 기본 다운로드 폴더에 저장됩니다.

## XLSX 파일에 특정 Insight 다운로드

* insight 오른쪽 상단에서 ![다운로드](/help/creative/assets/download.png "다운로드")를 클릭합니다.

  파일은 브라우저의 기본 다운로드 폴더에 저장됩니다.

>[!MORELIKETHIS]
>
>* [사용자 지정 보고서 정보](/help/dsp/reports/report-about.md)
>* [캠페인 관리 보기의 성능 보고서 유형](/help/dsp/campaign-management/reports/campaign-reports-about.md)
>* [사용 가능한 보고서 열](/help/dsp/reports/report-columns.md)
>* [Campaign 데이터 보기 관리](/help/dsp/campaign-management/reports/campaign-data-views-manage.md)
