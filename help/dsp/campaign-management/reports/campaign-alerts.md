---
title: 경고 보기
description: 캠페인 및 캠페인 구성 요소에 대한 경고 및 권장 해결 방법을 보는 방법을 알아봅니다.
feature: DSP Campaigns, DSP Packages, DSP Placements, DSP Ads, DSP Campaign Data Views
exl-id: 667bf1c3-3bad-4a1a-b907-0c9bfe5362a9
source-git-commit: 39f77087769eda3cc200447aeb0a6d1648e23b42
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 0%

---

# 경고 보기

DSP을 사용하면 캠페인이나 캠페인 구성 요소에 문제가 있는 경우를 식별할 수 있습니다. 각 문제에 대해 DSP은 타임스탬프와 문제 해결을 위한 권장 조치를 갖춘 경고를 만듭니다. 경고 이유에는 구성 문제(예: 배치에 광고가 첨부되지 않았거나 거래가 잘못 설정된 경우), 광고 거부, 캠페인 상태 문제(예: 광고 게재 불량 또는 성능 저하)가 포함됩니다. 경고는 캠페인, 패키지, 배치, 광고 및 거래 수준에서 사용할 수 있습니다.

경고는 다음 위치에서 사용할 수 있습니다.

* [!UICONTROL Pulse Panel], [!UICONTROL Campaigns] 및 패키지 세부 정보, [!UICONTROL Packages] 및 [!UICONTROL Placements] 보기의 [!UICONTROL Ads] 아이콘은 해당 보기의 항목에 사용할 수 있는 경고가 있는지 여부를 나타냅니다. 아이콘에 파란색 점이 있는 경우(![경고를 사용할 수 있을 때의 펄스 패널 아이콘](/help/dsp/assets/alerts-panel.png "경고를 사용할 수 있을 때의 펄스 패널 아이콘")), 경고를 사용할 수 있습니다. 점이 표시되지 않으면(![사용 가능한 경고가 없을 때 Pulse Panel 아이콘](/help/dsp/assets/alerts-panel-empty.png "사용 가능한 경고가 없을 때 Pulse Panel 아이콘")) 경고를 사용할 수 없습니다.

* 동일한 보기의 데이터 테이블에는 항목 또는 해당 구성 요소에 문제가 있는 시기를 나타내는 &quot;[!UICONTROL Alerts]&quot; 열이 포함되어 있습니다. 경고 표시기에는 &quot;위험&quot;(![중요](/help/dsp/assets/indicator-critical.png "중요")), &quot;경고&quot;(![경고](/help/dsp/assets/indicator-warning.png "경고")) 및 &quot;정보&quot;(![정보](/help/dsp/assets/indicator-information.png "정보"))가 포함됩니다.

필요에 따라 설정을 편집하여 문제를 해결할 수 있도록 경고에 대한 관련 캠페인 관리 보기를 열 수 있습니다.

개별 경고를 무시하도록 선택하여 [!UICONTROL Pulse] 패널에서 제거할 수도 있습니다.

기본 문제가 해결되면 경고 및 경고 표시기가 자동으로 사라집니다.

## [!UICONTROL Pulse Panel]에서 경고 보기

1. 주 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * (보기에 적용할 수 있는 모든 경고의 경우) 캠페인 관리 보기의 도구 모음 오른쪽에 있는 ![경고를 사용할 수 있을 때 [패널 펄스] 아이콘](/help/dsp/assets/alerts-panel.png "경고를 사용할 수 있을 때 [패널 펄스] 아이콘")을 클릭합니다.

   * (특정 캠페인에 대한 모든 경고의 경우) 캠페인 행에 대한 경고 표시기를 클릭한 다음 **[!UICONTROL View in Pulse panel]**&#x200B;을(를) 클릭합니다.

   * (특정 패키지, 배치 또는 광고에 대한 모든 경고의 경우) 다음을 수행하십시오.

      1. 캠페인 이름을 클릭합니다.

      1. 하위 메뉴에서 **[!UICONTROL Packages]**, **[!UICONTROL Placements]** 또는 **[!UICONTROL Ads]**&#x200B;을(를) 클릭하여 관련 캠페인 구성 요소 보기를 엽니다.

      1. 패키지, 배치 또는 광고 행에 대한 경고 표시기를 클릭한 다음 **[!UICONTROL View in Pulse Panel]**&#x200B;을(를) 클릭합니다.

   타겟팅된 거래를 포함하여 캠페인 및 해당 구성 요소와 관련된 모든 경고가 나열됩니다. 기본적으로 중요한 경고가 먼저 나열됩니다.

1. (선택 사항) 첫 번째 감지 날짜에 따라 경고를 그룹화하거나 경고 상태, 구성 요소 상태, 구성 요소 유형 또는 특정 캠페인 이름별로 경고를 필터링하려면 패널의 오른쪽 상단에 있는 ![필터 단추](/help/dsp/assets/filter.png)를 클릭하고 필터 옵션을 선택한 다음 **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

1. 특정 경고 유형에 대해 영향을 받는 모든 캠페인 구성 요소 목록을 보려면 &quot;[!UICONTROL Package: No Active Placement (*N*)]&quot;과(와) 같은 경고 이름을 클릭하십시오. 권장 작업을 포함하여 영향을 받는 각 구성 요소에 대한 세부 정보를 보려면 [!UICONTROL EXPAND ALL]을(를) 클릭하거나 구성 요소 이름을 클릭하십시오. 권장 변경을 수행할 수 있도록 영향을 받는 구성 요소에 대한 관련 캠페인 관리 보기를 열려면 구성 요소 이름 위에 커서를 놓고 ![보기로 이동](/help/dsp/assets/go-to-view.png "보기로 이동")을 클릭합니다.

1. (선택 사항) 경고를 무시(숨기기)하려면 구성 요소 이름 위에 커서를 놓고 ![무시](/help/dsp/assets/alert-ignore.png "무시")를 클릭한 다음 **[!UICONTROL Ignore alert till next check]**, **[!UICONTROL Ignore alert for 3 days]** 또는 **[!UICONTROL Ignore indefinitely]**&#x200B;을 클릭합니다.

작업을 실행 취소하기 위해 경고를 무시한 후 몇 초 정도 시간이 소요됩니다. 옵션 메시지가 닫히면 작업을 취소할 수 없습니다.

1. (선택 사항) 무시된 경고를 검색하려면 &quot;[!UICONTROL Alert Status]&quot; 또는 &quot;[!UICONTROL All]&quot;의 [!UICONTROL Ignored]을(를) 표시하도록 경고를 필터링하십시오.&quot; 경고를 병합하려면 구성 요소 이름 위에 커서를 놓고 ![무시 취소](/help/dsp/assets/alert-un-ignore.png "무시 취소")를 클릭합니다.

## [!UICONTROL Pulse Panel] 닫기

* 도구 모음 오른쪽에서 ![경고를 사용할 수 있을 때 [펄스 패널] 아이콘](/help/dsp/assets/alerts-panel.png "경고를 사용할 수 있을 때 [펄스 패널] 아이콘") 또는 ![사용 가능한 경고가 없을 때 Pulse Panel 아이콘](/help/dsp/assets/alerts-panel-empty.png "사용 가능한 경고가 없을 때 Pulse Panel 아이콘")을 클릭합니다.

>[!MORELIKETHIS]
>
>* [캠페인 관리 보기의 성능 보고서 유형](campaign-reports-about.md)
