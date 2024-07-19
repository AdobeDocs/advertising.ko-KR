---
title: 크로스 디바이스 솔루션
description: 크로스 디바이스 기능에 대해 자세히 알아보십시오.
feature: DSP Introduction
exl-id: d21917ef-5cac-46f8-8222-099667797683
source-git-commit: e517dd5f5fa283ff8a2f57728612937148889732
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 0%

---

# 크로스 디바이스 솔루션

[!DNL LiveRamp]과(와) Advertising DSP 통합을 사용하면 대상을 브랜드가 추적한 장치뿐만 아니라 사람의 알려진 모든 장치로 확장할 수 있습니다. 또한 통합은 모든 장치에서 빈도 제한 및 속성 측정을 제공합니다.

지원되는 사용자 기반 장치 그래프를 사용하는 경우 다음을 수행할 수 있습니다.

* 채널 및 디바이스에서 대상자를 일치시켜 디바이스가 아닌 사람 및 가정에 광고를 전달합니다.
* 개인 간 빈도를 이해하고 가림으로써 균형과 노출을 조정합니다.
* 채널 또는 디바이스 간에 대상을 노출하거나 전환하는 테스트 전략입니다.

## [!DNL LiveRamp] 장치 그래프의 이점

* 오프라인 고객 데이터를 포함한 결정론적 데이터 풀 제공

* 쿠키 ID와 모바일 장치 ID 간에 균일한 범위 제공

* 주로 미국에서 수집한 데이터 포함

* 빈도 제한 및 속성 측정에 대해 무료

* 확장된 노출 횟수(타깃팅된 대상 세그먼트 내에 있는 장치가 아닌 [!DNL LiveRamp] 장치 그래프를 사용해서만 전달되는 노출 횟수)에 대해 CPM $0.35의 가격으로 책정되었습니다.

  요금은 당신의 계좌요금카드에 반영되어 있습니다

## 사용자 기반 빈도 관리

사용자 기반 빈도 관리를 사용하면 실제 미디어 노출 제어를 위해 디바이스 수준이 아닌 개인 수준에서 빈도 상한을 지정할 수 있습니다.

### 사용자 기반 빈도 관리 활성화

* **캠페인:** 새 캠페인을 만들 때 [!UICONTROL Cross-Device Level] 설정을 지정할 수 있습니다. &quot;[!UICONTROL Same Device]&quot; -> &quot;[!UICONTROL People]&quot;을(를) 활성화하고 장치 그래프를 선택합니다. 지정된 장치 그래프는 배치 수준에서 교차 장치 타겟팅 및 캠페인, 패키지 및 배치 수준에서 사용자 기반 빈도 관리에 사용됩니다. 주파수 캡은 사람의 알려진 모든 장치에 적용됩니다.

자세한 내용은 [캠페인 설정](/help/dsp/campaign-management/campaigns/campaign-settings.md)을 참조하세요.

캠페인을 저장하면 [!UICONTROL Cross Device Level] 설정을 변경할 수 없습니다.

* **패키지:** 선택적으로 패키지 수준에서 추가 빈도 상한을 설정할 수 있습니다. DSP은 campaign 계층 구조에서 가장 엄격한 빈도 상한을 따릅니다.

* **배치:** 선택적으로 배치 수준에서 추가 빈도 상한을 설정할 수 있습니다. DSP은 campaign 계층 구조에서 가장 엄격한 빈도 상한을 따릅니다.

## 사용자 기반 타기팅

사용자 기반 타깃팅을 사용하면 데스크탑 및 모바일에서 고객을 찾을 수 있습니다.

### 사용자 기반 타깃팅 활성화

* **캠페인:** 새 캠페인을 만들 때 [!UICONTROL Cross-Device Level] 설정을 지정할 수 있습니다. &quot;[!UICONTROL Same Device]&quot; -> &quot;[!UICONTROL People]&quot;을(를) 활성화하고 장치 그래프를 선택합니다. 지정된 장치 그래프는 배치 수준에서 장치 간 타깃팅 및 사용자 기반 빈도 관리 모두에 사용됩니다.

자세한 내용은 [캠페인 설정](/help/dsp/campaign-management/campaigns/campaign-settings.md)을 참조하세요.

* **배치:** 지정한 장치 그래프가 있는 캠페인에서 배치에 대한 대상 대상을 선택할 때 [!UICONTROL Cross-Device Targeting] 옵션을 사용하면 지정한 세그먼트에 없는 장치도 캠페인 설정에 지정된 장치 그래프에 따라 개인의 알려진 모든 장치에서 타깃팅을 확장할 수 있습니다.

### 사용자 기반 타깃팅에 대한 보고 설정

사용자 지정 보고서에 다음 지표를 포함할 수 있습니다.

* **확장된 노출 수:**([!UICONTROL Metrics] > [!UICONTROL Std. Metrics] 아래의 [!UICONTROL Build Your Report] 섹션) 장치 그래프를 활용하여 제공된 증분 노출 수(원래 대상 세그먼트 내에서 찾을 수 없음). 이 지표는 타사 장치 그래프 사용과 관련된 적용 가능한 요금을 계산하는 데에도 사용됩니다.

  기간 동안 확장된 노출의 비용을 결정하려면 [!UICONTROL Extended Impressions] 열이 포함된 사용자 지정 보고서를 실행한 다음 총 확장된 노출의 수에 $0.00035($0.35/1,000 노출수)을 곱하십시오.

  집계된 비용은 [!UICONTROL Billable Other Net Spend] 열([!UICONTROL Metrics] > [!UICONTROL Spend] 아래)에도 포함되지만 이 지표에는 추가한 다른 캠페인 비용도 포함됩니다.

* **장치 그래프:**([!UICONTROL Dimensions] > [!UICONTROL Campaign] 아래의 [!UICONTROL Build Your Report] 섹션에서) 특정 캠페인, 패키지 또는 배치에 대해 선택한 장치 그래프입니다.

## 사용자 기반 속성 측정

*Adobe Advertising 전환 추적만 있는 광고주*

사용자 기반 속성을 사용하면 미디어 노출이 발생한 장치가 아닌 다른 장치에서 발생한 전환을 지정할 수 있습니다. 사용자 기반 속성 측정은 DSP, [!DNL Adobe Advertising Creative] 및 [!DNL Adobe Advertising Search, Social, & Commerce]에서 해당 사이트에 Adobe Advertising 전환 픽셀을 구현한 광고주에게 사용할 수 있습니다.

### 사용자 기반 속성 측정 활성화

교차 장치 속성 측정을 활성화하려면 Adobe 계정 팀에 문의하십시오.

### 디바이스 간 전환 속성에 대한 전환 보고서 설정

#### 전환 보고서 설정

장치 그래프가 속성 측정에 대해 활성화되어 있으면 [!UICONTROL Conversion] 보고서에는 다음을 포함하여 각 전환 지표에 대해 최대 3개의 개별 열을 포함할 수 있는 [!UICONTROL Cross-Device Breakout] 설정이 포함됩니다.

* &lt;*전환*>[!UICONTROL (tp)]: 동일한 장치 전환과 장치 간 전환(해당되는 경우)을 모두 포함하는 총 전환(총 인원)을 포함합니다. 보고서에서 &quot;[!UICONTROL (tp)]&quot;이(가) 전환 경로의 전환 지표 이름, 규칙 유형 및 전환 유형(예: &quot;Responses(le)(tl)(tp))에 추가됩니다.

* &lt;*전환*>[!UICONTROL (sd)]: (선택 사항) 전환 경로에서 단일 장치만 추적된 전환만 포함합니다. 보고서에서 &quot;[!UICONTROL (sd)]&quot;이(가) 전환 경로의 전환 지표 이름, 규칙 유형 및 전환 유형(예: &quot;Responses(le)(tl)(sd))에 추가됩니다.

* &lt;*전환*>[!UICONTROL (xd)]: (선택 사항) 전환 경로에서 둘 이상의 장치가 추적된 전환만 포함합니다. 보고서에서 &quot;[!UICONTROL (xd)]&quot;이(가) 전환 경로의 전환 지표 이름, 규칙 유형 및 전환 유형(예: &quot;Responses(le)(tl)(xd))에 추가됩니다.

#### 전환 보고서를 해석하는 방법

평균 이상의 교차 장치 전환을 유도하는 이유를 파악하려면 교차 장치([!UICONTROL (xd)]/[!UICONTROL (tl)])인 총 전환 비율을 높음에서 낮음으로 정렬하십시오. 이 정보를 사용하여 메시징 및 채널 투자를 사용자 동작에 일치시키기 위한 크리에이티브 또는 타기팅 전략을 알릴 수 있습니다.

* 패키지 — 가장 많은 전체 전환을 유도하는 패키지와 높은 장치 간 전환 비율을 갖는 패키지를 확인합니다. 집중 지출을 파악하는 데 도움이 될 수 있습니다.

* 배치 — 배치 성능 및 속성을 비교합니다(예: 모바일 웹 광고는 데스크탑에서 전환을 유도할 수 있음). 기여도 분석을 위한 Device Graph가 없으면 모바일 웹 배치가 데스크탑 전환에 미치는 영향을 놓치거나 사용자의 대다수가 모바일 웹이 아닌 데스크탑에서 전환하는 경우 이 배치가 삭제될 수 있습니다.

* 광고 — 더 높은 전환을 유도하는 광고를 검색하고 웹 브라우저와 모바일 앱 환경 모두에서 광고의 가치와 영향을 수량화합니다.

* 사이트 — 사이트를 수동으로 완전히 제외하지 않고 사이트 간에 최적화합니다. 웹 사이트에서 장치 간 전환을 유도하는 경우 이 동작이 발생하는 장치를 확인할 수 있습니다.

* 거래 — 장치 간 전환을 제공하는 인벤토리 거래를 확인한 다음 해당 거래에 더 많은 장치와 채널을 포함하도록 타깃팅을 확장해야 하는지 여부를 결정하여 수동 최적화를 개선합니다.

>[!MORELIKETHIS]
>
>* [보고서 설정](/help/dsp/reports/report-settings.md)
>* [캠페인 설정](/help/dsp/campaign-management/campaigns/campaign-settings.md)
>* [패키지 설정](/help/dsp/campaign-management/packages/package-settings.md)
>* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)
