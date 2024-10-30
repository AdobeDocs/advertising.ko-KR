---
title: 배치 진단 보고서 보기
description: 배치 설정 및 게재 간격 관련 문제를 진단하는 방법을 알아봅니다.
feature: DSP Placements
exl-id: 95e88c9c-09f2-44f1-9d6c-3fe533963f9a
source-git-commit: fa4cee46135c85849daa7faa4059c77fc753c2c8
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 0%

---

# 배치 진단 보고서 보기

<!-- Does this really belong in the Campaign Management > Reports section or in the Placements section? -->

진단 보고서는 캠페인이 라이브되면 배치 설정 및 게재 간격 관련 문제를 진단하는 데 도움이 됩니다.

## 배치 진단 보고서의 정보

* **[!UICONTROL Change Log]:** 이름, 상태 및 최대 입찰가와 같은 키 배치 설정에 대한 변경 내용을 표시합니다. 각 항목에는 변경한 사람의 날짜 및 사용자 이름이 포함됩니다.

* **[!UICONTROL Ad Approvals]:** 인벤토리 공급자가 광고를 승인했는지 또는 거부했는지 여부를 표시합니다. 선택적으로 광고의 상태를 변경(예: 거부된 광고를 일시 중지)하거나 광고 설정을 열 수 있습니다.

* **[!UICONTROL Non Bids]:** DSP이 배치에 입찰하지 않은 이유를 표시합니다.

## 배치 진단 보고서 열기

1. Diagnostics 보고서를 엽니다.

   1. 배치 설정을 엽니다.

      1. 주 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

      1. 캠페인 이름을 클릭한 다음 **[!UICONTROL Placements]**&#x200B;을(를) 클릭합니다.

      1. 배치 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

   1. 오른쪽 상단에서 ![배치 진단](/help/dsp/assets/placement-diagnostics.png)을 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * 변경 로그를 보려면

      1. **[!UICONTROL Change Log]**&#x200B;을(를) 클릭합니다.

      1. (선택 사항) 보고서 결과를 필터링합니다.

         * 날짜 메뉴에서 보고서 기간을 기본 최근 14일에서 다른 기간(*[!UICONTROL Last 30 days],* *[!UICONTROL Last 60 days],* *[!UICONTROL Last 90 days],* 또는 *[!UICONTROL Last 1 year]*)으로 변경합니다.

         * 왼쪽 메뉴에서 특정 사용자 이름으로 보고서를 필터링합니다.

         * 오른쪽 메뉴에서 특정 배치 설정으로 보고서를 필터링합니다.

   * 광고 승인 상태를 보려면 다음 작업을 수행하십시오.

      1. 오른쪽 상단에서 **[!UICONTROL Ad Approvals]**&#x200B;을(를) 클릭합니다.

      1. (선택 사항) 광고를 일시 중지하거나 활성화하려면 상태 스위치(![광고 열에서 상태 스위치](/help/dsp/assets/status-switch.png))를 클릭합니다.

      1. (선택 사항) 광고 설정을 열려면 광고 옆에 있는 **[!UICONTROL View Ad]**&#x200B;을(를) 클릭합니다.

   * DSP이 배치에 입찰하지 않은 이유를 확인하려면:

      1. 오른쪽 상단에서 **[!UICONTROL Non Bids]**&#x200B;을(를) 클릭합니다.

      1. (선택 사항) 특정 비공개 거래 대상별로 배치를 필터링하려면 거래를 선택합니다. <!-- Admin users only: Optionally filter the deal by one or more regions ([!UICONTROL US-EAST], [!UICONTROL US-WEST]) [!UICONTROL EU-WEST], [!UICONTROL HKG]) by selecting the regions. -->

      1. (선택 사항) 날짜 범위를 변경하려면 날짜 필드를 클릭하고 다른 날짜 또는 날짜 범위를 선택합니다.

<!-- Later, add link to >* Definitions for NBRs (Reading No Bid Reports (NBRs)) -->

>[!MORELIKETHIS]
>
>* [Campaign Management 보기의 성능 보고서 유형](campaign-reports-about.md)
>* [배치 예측 보고서 보기](/help/dsp/campaign-management/reports/placement-forecast.md)
>* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)
