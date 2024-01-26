---
title: 배치 진단 보고서 보기
description: 배치 설정 및 게재 간격 관련 문제를 진단하는 방법을 알아봅니다.
feature: DSP Placements
exl-id: 95e88c9c-09f2-44f1-9d6c-3fe533963f9a
source-git-commit: 61ca25565e09bbce505d6f5cb0e5e8b7214eb1e0
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# 배치 진단 보고서 보기

<!-- Does this really belong in the Campaign Management > Reports section or in the Placements section? -->

다음 도구는 캠페인이 라이브되면 배치 설정 및 게재 간격 문제를 진단하는 데 도움이 될 수 있습니다.

* **[!UICONTROL Change Log]:** 이름, 상태 및 최대 입찰가와 같은 주요 배치 설정의 변경 내용을 표시합니다. 각 항목에는 변경한 사람의 날짜 및 사용자 이름이 포함됩니다.
* **[!UICONTROL Ad Approvals]:** 인벤토리 공급자가 광고를 승인했는지 또는 거부했는지 여부를 표시합니다. 선택적으로 광고의 상태를 변경(예: 거부된 광고를 일시 중지)하거나 광고 설정을 열 수 있습니다.
* **[!UICONTROL Non Bids]:** DSP이 배치를 입찰하지 않은 이유를 보여 줍니다.

1. Diagnostics 보고서를 엽니다.
   1. 배치 설정을 엽니다.
      1. 메인 메뉴에서 **[!UICONTROL Campaigns]**.
      1. 캠페인 이름을 클릭한 다음 **[!UICONTROL Placements]**.
      1. 배치 이름 옆에 있는 를 클릭합니다  **[!UICONTROL ...]** > **[!UICONTROL Edit]**.
   1. 오른쪽 상단에서 ![배치 진단](/help/dsp/assets/placement-diagnostics.png).
1. 다음 중 하나를 수행합니다.
   * 변경 로그를 보려면
      1. 클릭 **[!UICONTROL Change Log]**.
      1. (선택 사항) 보고서 결과를 필터링합니다.
         * 날짜 메뉴에서 보고서 기간을 기본 최근 14일에서 다른 기간(*[!UICONTROL Last 30 days],* *[!UICONTROL Last 60 days],* *[!UICONTROL Last 90 days],* 또는 *[!UICONTROL Last 1 year]*).
         * 왼쪽 메뉴에서 특정 사용자 이름으로 보고서를 필터링합니다.
         * 오른쪽 메뉴에서 특정 배치 설정으로 보고서를 필터링합니다.
   * 광고 승인 상태를 보려면 다음 작업을 수행하십시오.
      1. 오른쪽 상단에서 **[!UICONTROL Ad Approvals]**.
      1. (선택 사항) 광고를 일시 중단하거나 활성화하려면 상태 스위치( )를 클릭합니다.![상태 전환](/help/dsp/assets/status-switch.png))을 클릭하여 제품에서 사용할 수 있습니다.
      1. (선택 사항) 광고 설정을 열려면 **[!UICONTROL View Ad]** 광고 옆에.
   * DSP이 배치에 입찰하지 않은 이유를 확인하려면:
      1. 오른쪽 상단에서 **[!UICONTROL Non Bids]**.
      1. (선택 사항) 날짜 범위를 변경하려면 날짜 필드를 클릭하고 다른 날짜 또는 날짜 범위를 선택합니다.

<!-- Later, add link to >* Definitions for NBRs (Reading No Bid Reports (NBRs)) -->

>[!MORELIKETHIS]
>
>* [Campaign Management 보기의 성능 보고서 정보](campaign-reports-about.md)
>* [배치 예측 보고서 보기](/help/dsp/campaign-management/reports/placement-forecast.md)
>* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)
