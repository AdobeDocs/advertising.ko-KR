---
title: 경험 수준 성과 보고서
description: 경험 수준 성과 보고서를 보는 방법에 대해 알아봅니다.
feature: Creative Experiences
exl-id: 5e7c4c9d-b992-460a-9765-4276027f9a61
source-git-commit: f7e022d8753eb41f5eed8667b9af66085f912bff
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 0%

---

# 경험 수준 성과 보고서

*베타가 닫힘*

모든 경험에 대한 자세한 성능 데이터를 볼 수 있습니다.

## 경험 수준 성과 보고서의 데이터

보고서 보기에는 다음 데이터가 포함됩니다.

* **개요** 탭: 다음을 포함한 전체 경험에 대한 성능 개요:

   * **전체 성능** 섹션:

   * **전체 성능**: 총 노출 횟수, 클릭 수, 클릭스루 비율(CTR), 단일 전환 지표에 대한 뷰스루 전환 및 클릭스루 전환. <!-- Just one, or can you select multiple? And I don't see this as of 2/8:  You can optionally combine two metrics at a time into a single chart. -->

     <!--
     ![Overall performance](/help/creative/assets/experience-report-overall-performance.png "Overall performance"){width="100" zoomable="yes"}
          -->

   * **기본 비율**: (의사 결정 트리 타깃팅만 있는 경험) 타깃팅된 크리에이티브, 타깃팅이 없거나 &quot;기타 사용자&quot;에게 타깃팅된 일반 크리에이티브 및 경험의 기본 크리에이티브로 인한 노출 횟수.

     <!--
     ![Default rate](/help/creative/assets/experience-report-default-rate.png "Default rate"){width="100" zoomable="yes"} 
     -->

   * **성능 분석** 섹션:

      * **지역별 성능:*: 지리적 위치에 따른 개별 지표입니다.

        <!-- You can optionally do the following:
    
      * Click a metric name (such as [!UICONTROL Impressions]) to view that metric.

      * Select the region in the **[!UICONTROL Region]** menu.
      
      -->

        <!--   
      ![Regional performance](/help/creative/assets/experience-report-regional-performance.png "Regional performance"){width="100" zoomable="yes"}
      -->

      * **장치 성능:** 장치 유형, 운영 체제 및 브라우저별 개별 지표입니다. 필요한 경우 장치 범주에 대한 값을 클릭하여 해당 기준으로 제공되는 상위 <!-- NN -->개의 크리에이티브 목록을 확인합니다.

        <!--    
      ![Device performance](/help/creative/assets/experience-report-device-performance.png "Device performance"){width="100" zoomable="yes"}
      -->

* **Creative 성능** 탭*: 다음 항목을 포함하는 크리에이티브 및 번들 또는 광고 태그별 성능 개요:

   * **크리에이티브** 하위 탭: 경험의 각 크리에이티브에 대한 총 노출 횟수, 클릭 수 및 CTR 수입니다.<!-- No breakdown yet for the individual ad elements and/or the served ads. -->

     <!--

     * *Experiences with decision tree targeting:* The total number of impressions, clicks, and CTR for each creative. You can optionally do the following:
     
       * To break out the performance for each ad target, enable **[!UICONTROL Split targeting]**.

       * To switch between the grid view and a trend chart, which includes the addition of view-through conversions and click-through conversions (using the conversions specified in the top toolbar), click ![Chart](/help/creative/assets/chart-view-button.png "Chart") and ![Grid](/help/creative/assets/table-view-button.png "Grid") above the report. [Find out about this:  ..., and total conversions for specified conversion metricsYour conversion metrics are combined into one Conversions column set unless you have made individual metric column sets available within Advertising Cloud Search.]

     * *Experiences without decision tree targeting:* The total number of impressions, clicks, and click-through rate (CTR) for each creative. You can optionally do the following:

       * To switch between the grid view and a trend chart, which includes the addition of view-through conversions and click-through conversions (using the conversions specified in the top toolbar), click ![Chart](/help/creative/assets/chart-view-button.png "Chart") and ![Grid](/help/creative/assets/table-view-button.png "Grid") above the report.

     -->

   * **번들/태그** 하위 탭: 경험의 개별 번들(의사 결정 트리 타깃팅이 있는 경험) 또는 광고 태그(의사 결정 트리 타깃팅이 없는 경험)에 대한 총 노출 횟수, 클릭 수 및 CTR 수입니다.

     <!--
   
     * *Experiences with decision tree targeting:* The total number of impressions, clicks, and CTR for each bundle. You can optionally do the following:
     
       * To break out the performance for each ad target, enable **[!UICONTROL Split targeting]**.

       * To switch between the grid view and a trend chart, which includes the addition of view-through conversions  and click-through conversions (using on the conversions specified in the top toolbar), click ![Chart](/help/creative/assets/chart-view-button.png "Chart") and ![Grid](/help/creative/assets/table-view-button.png "Grid") above the report.

     * *Experiences without decision tree targeting:* The total number of impressions, clicks, and click-through rate (CTR) for each ad tag. You can optionally do the following:

       * To switch between the grid view and a trend chart, which includes the addition of view-through conversions and click-through conversions (using the conversions specified in the top toolbar), click ![Chart](/help/creative/assets/chart-view-button.png "Chart") and ![Grid](/help/creative/assets/table-view-button.png "Grid") above the report.

     -->

## 경험에 대한 성능 보고서 보기

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Experiences]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 특정 경험을 포함하도록 [보기를 사용자 지정](/help/creative/introduction/customize-data-views.md)합니다.

1. 경험을 선택합니다.

   * 카드 보기에서 경험 이름 옆의 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Reports]**&#x200B;을(를) 클릭합니다.

   * 테이블 보기에서 행 위에 커서를 놓고 **[!UICONTROL Reports]**&#x200B;을(를) 클릭합니다.

   [!UICONTROL Overview] 탭이 열립니다.

1. (선택 사항) 오른쪽 상단 도구 모음에서 날짜 범위, 전환 속성 규칙 및 모든 성능 보고서 내에서 보고된 전환을 지정합니다.

   * (선택 사항) 성능 데이터의 날짜 범위를 변경하려면 날짜 메뉴에서 옵션을 선택합니다.

      * 사전 설정 기간을 지정하려면 보고서를 선택하십시오. (*[!UICONTROL Last Month-to-date],* *[!UICONTROL Last 7 days],* *[!UICONTROL Last 30 days],* *[!UICONTROL Last 7 days],* *[!UICONTROL Last 30 days],* *[!UICONTROL Today],* 또는 *[!UICONTROL Yesterday]*.

      * 사용자 지정 날짜 범위를 지정하려면 시작 날짜와 종료 날짜<!-- in the format MM/DD/YYYY or M/D/YYYY,-->를 지정하거나 필드 옆에 있는 ![달력 아이콘](/help/search-social-commerce/assets/calendar.png)을 클릭하고 날짜를 선택합니다.

   * (선택 사항) 전환으로 이어지는 일련의 이벤트에서 전환 데이터의 특성을 지정하는 데 사용되는 규칙을 변경하려면 ![설정](/help/creative/assets/settings.png)을 클릭하고 **[!UICONTROL Attribution Rule]**&#x200B;을(를) 변경합니다.

     속성 규칙에 대한 자세한 내용은 &quot;[속성 규칙을 계산하는 방법](/help/search-social-commerce/reports/attribution-rules.md)&quot;을 참조하십시오.

   * (선택 사항) 보고된 전환을 변경하려면 ![설정](/help/creative/assets/settings.png)을 클릭하고 **[!UICONTROL Conversions]** 메뉴에서 전환 이름을 선택합니다.&lt;!— 한 번? 아니면 여러 번? 이러한 항목이 어떻게 표시되는지 확인하십시오. 이미 여러 개의 전환이 설정된 광고주를 확인해야 합니다. 3/6부터 &quot;모두 선택&quot; —> 만 표시됩니다.

     사용 가능한 전환 열에는 검색, 소셜 및 Commerce 고객인지 여부에 관계없이 Advertising 검색, 소셜 및 Commerce에서 사용할 수 있는 전환이 포함됩니다. 광고주가 [an [!DNL Adobe Analytics for Advertising] 통합](/help/integrations/analytics/overview.md)을 보유한 경우 Adobe Analytics에서 동기화된 전환 및 사이트 참여 지표가 목록에 포함될 수 있습니다. <!--Analytics calculated metrics and advanced calculated metrics aren't available.--> 보고서에 수집된 전환을 포함하는 방법에 대한 자세한 내용은 검색, 소셜 및 Commerce 가이드 항목 &quot;[광고주의 전환 지표 관리에 대한 정보](/help/search-social-commerce/admin/conversion-metrics/conversion-metric-about.md)&quot;를 참조하십시오.

1. [!UICONTROL Overview] 탭에서:

   * (선택 사항) [!UICONTROL Overall Regional Performance] 섹션에서 차트 상의 한 지점 위에 커서를 놓으면 해당 지점의 데이터를 볼 수 있습니다.

   * (선택 사항) [!UICONTROL Regional Performance] 섹션에서 다음 중 하나를 수행합니다.

      * 해당 지표를 보려면 지표 이름(예: [!UICONTROL Impressions])을 클릭하십시오.

      * [!UICONTROL Region] 메뉴에서 지역을 선택합니다.

      * 국가 또는 주 위에 커서를 놓으면 해당 지역의 데이터를 볼 수 있습니다.

   * (선택 사항) [!UICONTROL Device Performance] 섹션에서 다음 중 하나를 수행합니다.

      * 디바이스 범주의 값 위에 커서를 놓으면 해당 기준에 대한 데이터를 볼 수 있습니다.

      * 해당 기준으로 제공되는 상위 <!-- NN-->개의 광고 목록을 보려면 장치 범주에 대한 값을 클릭하십시오.

1. (선택 사항) Creative 및 번들 또는 광고 태그로 데이터를 보려면 **[!UICONTROL Creative Performance]** 탭을 클릭합니다.

   * [!UICONTROL Creatives] 하위 탭에서 다음 중 하나를 수행할 수 있습니다.

      * (선택 사항) 차트 보기와 표 보기 간에 전환하려면 각각 ![차트](/help/creative/assets/chart-view-button.png "차트") 및 ![격자](/help/creative/assets/table-view-button.png "격자")을 클릭합니다.

      * (선택 사항) 차트 보기에서 차트의 한 지점 위에 커서를 놓으면 해당 지점에 대한 데이터가 표시됩니다.

      * (의사 결정 트리 타깃팅만 있는 경험, 선택 사항) 적용된 각 광고 대상에 대한 성능을 분석하려면 **[!UICONTROL Split targeting]**&#x200B;을(를) 활성화합니다.

1. 번들(의사 결정 트리 타깃팅이 있는 경험) 또는 광고 태그(의사 결정 트리 타깃팅이 없는 경험)별로 데이터를 보려면 **[!UICONTROL Bundles]** 하위 탭을 클릭하십시오. 다음 중 원하는 작업을 수행할 수 있습니다.

   * (선택 사항) 차트 보기와 표 보기 간에 전환하려면 각각 ![차트](/help/creative/assets/chart-view-button.png "차트") 및 ![격자](/help/creative/assets/table-view-button.png "격자")을 클릭합니다.

   * (선택 사항) 차트 보기에서 차트의 한 지점 위에 커서를 놓으면 해당 지점에 대한 데이터가 표시됩니다.

   * (의사 결정 트리 타깃팅만 있는 경험, 선택 사항) 적용된 각 광고 대상에 대한 성능을 분석하려면 **[!UICONTROL Split targeting]**&#x200B;을(를) 활성화합니다.

## 경험에 대한 성능 보고서 다운로드

* 성능 보고서 상단의 도구 모음에서 ![다운로드](/help/creative/assets/download.png "다운로드")를 클릭합니다.

  브라우저의 일반 절차에 따라 스프레드시트(XLSX) 형식으로 [!DNL Microsoft Excel] 파일로 파일이 다운로드됩니다.

>[!MORELIKETHIS]
>
>* [사용자 지정 Creative 보고서](/help/creative/report-custom-creative.md)
>* [보기의 모든 경험 다운로드](/help/creative/experiences/experience-download-view.md)
>* [Advertising Creative의 경험 정보](/help/creative/experiences/experience-about.md)
