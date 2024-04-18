---
title: 배치에 대한 입찰 승수 관리
description: 지정된 배치 대상의 입찰 배수를 만들고 편집하는 방법에 대해 알아봅니다.
feature: DSP Placements
source-git-commit: 7a794394d9338cb2608ce3d89c90b122f8eee9dc
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 3%

---

# 배치에 대한 입찰 승수 관리

이 기능을 사용하여 기존 배치 대상의 입찰 배수를 변경할 수 있습니다. 한 번에 한 배치에 대한 입찰 승수를 관리할 수 있습니다.<!-- remove that line once we can edit multiple -->

배치에 대해 선택한 대상을 변경하려면 &quot;[배치 편집](/help/dsp/campaign-management/placements/placement-edit.md).&quot;

<!--  
## Manage the Bid Multipliers for a Single Placement
-->

1. 메인 메뉴에서 **[!UICONTROL Campaigns]**.

1. 캠페인의 이름을 클릭합니다.

1. 하위 메뉴에서 **[!UICONTROL Placements]**.

1. 배치 이름 옆에 있는 를 클릭합니다  **[!UICONTROL ...]** > **[!UICONTROL Bid Multiplier]**.

1. 각 위치로 이동 [target별 탭](#bid-multiplier-by-target) ([!UICONTROL Geo], [!UICONTROL Inventory], [!UICONTROL Sites], [!UICONTROL Audience], 및 [!UICONTROL Brand Safety]) 배치 대상의 기존 값을 편집합니다. 대부분의 대상 카테고리는 왼쪽에 하위 카테고리를 나열합니다. 해당되는 경우 하위 범주를 클릭하여 해당 하위 범주에 대한 입찰 승수를 관리합니다.

   기본적으로 대상에 대한 입찰 승수는 1.00이며, 이는 입찰이 해당 대상에 대해 조정되지 않음을 의미합니다. 값의 범위는 0.10부터 10.00까지입니다. 예를 들어, 입찰 수정자 0.5는 USD 6 입찰을 USD 3으로 감소시킵니다(0.5 x 6). 입찰 수정자는 입찰가를 최대 입찰가 이상으로 증가시키지 않습니다.

   경매에서 여러 입찰 수정자를 사용할 수 있는 경우 적용 가능한 모든 입찰 수정자를 곱합니다.

   다음에 대한 입찰 승수(1.00 이외의 값 사용)를 설정할 수 있습니다. [제한된 타겟 수](#bid-multiplier-limits-by-target).

1. 오른쪽 상단에서 **[!UICONTROL Save]**.

## 입찰 승수에 적합한 대상 유형 {#bid-multiplier-by-target}

제외된 대상이 아닌 포함된 대상에 대해서만 입찰 수정자를 구성할 수 있습니다.

* **지역 대상**: 지역(국가, 주 및 도시), 우편 번호 및 DMA

* **재고 목표**: 공개 인벤토리에 대한 소스 및 피드 [!UICONTROL On Demand] 인벤토리

* **사이트 대상:** 사이트/앱, 사이트 범주(제외되지 않음) 타겟팅

* **대상 타겟:** 세그먼트, 일 단위 및 주제

* **ads.txt 대상:** (ads.txt를 옵트아웃하는 경우) ads.txt 판매자만, ads.txt 직접 판매자 및 ads.txt 판매자와 ads.txt가 없는 사이트만 해당합니다.

## 대상 유형별 최대 입찰 승수 {#bid-multiplier-limits-by-target}

제한된 수의 대상에 대해 (1.00 이외의 값으로) 입찰 승수를 설정할 수 있습니다. 예를 들어 최대 20개의 국가 타겟에 대한 입찰 승수를 설정할 수 있습니다. 입찰 승수를 가질 수 있는 각 대상 유형에 대한 최대 대상 수는 아래에 나와 있습니다.

| 범주 | 매개 변수 | 최대 수 |
| -------- | --------- | ----- |
| 지역 | 국가 | 20 |
| 지역 | 시/도 | 100 |
| 지역 | 도시 | 100 |
| 지역 | 메트로 | 100 |
| 지역 | 우편 번호 | 100 |
| 인벤토리 | 소스 | 100 |
| 인벤토리 | 피드 | 100 |
| 사이트 | 사이트 카테고리 | 100 |
| 사이트 | 사이트/앱 | 100 |
| 대상자 | 세그먼트 | 500 |
| 대상자 | 주제 | 100 |
| 브랜드 안전 | Ads.txt | 해당 사항 없음 |

>[!MORELIKETHIS]
>
>* [배치 관리 정보](placement-about.md)
>* [배치 편집](placement-edit.md)
>* [배치에 대한 변경 로그 보기](placement-change-log.md)
>* [배치 설정](placement-settings.md)
