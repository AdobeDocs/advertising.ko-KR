---
title: 비공개 거래에 대한 경매 인사이트 보기
description: 경매 인사이트를 사용하여 비공개 거래의 거래 구성을 분석하는 방법에 대해 알아봅니다.
feature: DSP Private Inventory, DSP Deal IDs, DSP Programmatic Guaranteed Deals
exl-id: bbb99f6a-0276-4eb8-9607-75500d5634d9
source-git-commit: 1ac58da2d538cc682161ebc944a0412ad4a8af17
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# 비공개 거래에 대한 경매 인사이트 보기

Auction Insights는 보장된 비공개 거래와 보장되지 않은 비공개 거래의 거래 구성을 분석할 수 있는 문제 해결 도구입니다. 이 도구는 데이터 시각화를 사용하여 특정 기간 내에 [주요 경매 특성](#auction-attributes)에 대해 받은 값의 추세와 상대적인 비율을 보여 줍니다.

1. 메인 메뉴에서 **[!UICONTROL Inventory]** > **[!UICONTROL Deals].**&#x200B;을(를) 클릭합니다.

1. 거래 행에서 **[!UICONTROL ...]** > **[!UICONTROL Auction Insights]**&#x200B;을(를) 클릭합니다.

>[!NOTE]
>
>Auction Insights는 배치 [!UICONTROL Inspector] 도구를 통해서도 사용할 수 있습니다. 이를 열려면 [[!UICONTROL Inventory tab]에 대한 [!UICONTROL Inspector]](/help/dsp/campaign-management/reports/placement-details-view.md) 배치를 연 다음 거래 행에서 **[!UICONTROL ...]** > **[!UICONTROL Auction Insights]**&#x200B;을(를) 클릭합니다.

## 경매 속성 {#auction-attributes}

영역 차트는 다음 경매 속성에 사용할 수 있습니다.

* **광고 유형:** 경매에서 요청한 광고 유형(예: 디스플레이 또는 오디오)입니다.

* **브라우저:** 경매가 시작된 브라우저입니다(예: Chrome 또는 Firefox).

* **OS:** 경매가 시작된 운영 체제(예: Android 또는 iOS)입니다.

* **장치 유형:** 경매가 시작된 장치입니다(예: 휴대폰 또는 데스크톱).

* **광고 기간:** 경매에 요청된 최대 광고 기간(예: 15초 또는 30초)입니다.

* **보안:**&#x200B;은(는) 경매에 보안 HTTPS URL 광고 자산이 필요한지 여부를 나타냅니다. 값: <i>보안</i> 또는 <i>비보안</i>.

* **MIME 유형:** 경매에서 요청된 광고 크리에이티브 MIME 유형(예: mp4 또는 mov)입니다.

![경매 인사이트](/help/dsp/assets/auction-insights.png)

>[!NOTE]
>
>특정 속성 값에 대한 필터를 적용하여 결과 범위를 좁힐 수 있습니다.

>[!MORELIKETHIS]
>
>* [개인 인벤토리 정보](private-inventory-about.md)
>* [거래 ID에 대한 배치 및 광고 지정](deal-id-attach-placements.md)
>* [거래에 대한 자세한 보고서 보기](deal-view-report.md)
>* [Campaign Management 보기의 성능 보고서 유형](/help/dsp/campaign-management/reports/campaign-reports-about.md)
