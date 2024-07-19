---
title: '[!UICONTROL Simple Ad Serving] 정보'
description: 이벤트 추적 픽셀을 사용한 [!UICONTROL Simple Ad Serving] 거래에 대해 알아봅니다.
feature: DSP Simple Ad Serving
exl-id: 327a2c93-d729-42e1-856f-f0e05efab7ca
source-git-commit: 7e614ecb517515217d812926f61ca10437820efd
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# [!UICONTROL Simple Ad Serving] 정보

[!UICONTROL Simple Ad Serving]은(는) 하나의 전용 배치를 사용하여 지정된 게시자 및 단일 광고 유형에 대해 보장되고 결정되지 않은 광고 게재 및 보고를 제공합니다. 게시자가 거래 ID를 통해 거래를 실행할 수 없는 경우 [!DNL Simple Ad Serving]을(를) 사용합니다. 모든 타겟팅, 예산 게재 간격 및 한도, 빈도 상한은 게시자가 처리합니다. 이벤트 추적 픽셀을 통해 이러한 거래를 실행합니다.

[!UICONTROL Simple Ad Serving]을(를) 사용하면 각 광고는 게시자가 직접 제공하며(사이트 서비스), DSP은 게시자에게 보낼 이벤트 추적 픽셀을 제공합니다. 게시자는 픽셀과 DSP 광고를 구현해야 합니다. 이벤트 픽셀은 인벤토리 유형에 따라 노출, 클릭스루 및 비디오 재생 이벤트를 측정합니다.

다음 광고 유형을 사용할 수 있습니다.

* 데스크탑 표준 프리롤
* 태블릿 및 모바일 표준 프리롤
* 연결된 TV 표준 프리롤
* 디스플레이
* 오디오

[!UICONTROL Inventory] > [!UICONTROL Deals] 보기에서 [!UICONTROL Simple Ad Serving] 거래를 만들 수 있습니다. DSP은 광고에 대한 하위 유형이 &quot;[!DNL Simple ad serving]&quot;인 배치를 자동으로 생성합니다. 배치는 거래를 타깃팅하지만 추가 타깃팅, 예산 또는 빈도 제한을 허용하지 않습니다. 거래 이름, CPM, 노출 횟수 및 플라이트 날짜와 같은 일부 거래 설정만 편집할 수 있습니다.<!-- If you need multiple tracking tags for a [!UICONTROL Simple Ad Serving] deal, create a duplicate deal. -->

[!UICONTROL Simple Ad Serving] 배치가 계정의 사용 가능한 자금 또는 캠페인 및 패키지 예산을 준수하지 않습니다. 그러나 지출은 해당 예산에 대해 추적되고 계산됩니다. CPM이 $0인 경우에도 이벤트 데이터는 항상 추적됩니다.

>[!MORELIKETHIS]
>
>* [[!UICONTROL Simple Ad Serving] 거래 만들기](simple-deal-create.md)
>* [거래 설정 [!UICONTROL Simple Ad Serving]개 편집](simple-deal-edit.md)
>* [[!UICONTROL Simple Ad Serving] 설정](simple-deal-settings.md)
>* [거래에 대한 자세한 보고서 보기](/help/dsp/inventory/deal-view-report.md)

<!-- add back when reimplemented:
>* [View Event-Tracking Pixels for a [!UICONTROL Simple Ad Serving] Deal](simple-deal-show-pixels.md)
-->
