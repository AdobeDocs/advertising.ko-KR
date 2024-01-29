---
title: 배치에 대한 사이트, 광고, 빈도 및 재고 세부 정보 보기
description: 배치에 대한 타겟팅된 사이트, 광고, 빈도 및 인벤토리 데이터를 보는 방법에 대해 알아봅니다.
feature: DSP Placements
exl-id: b58b442c-2fb8-4a78-9be9-d85aa83136e2
source-git-commit: 1ac58da2d538cc682161ebc944a0412ad4a8af17
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 0%

---

# 배치에 대한 사이트, 광고, 빈도 및 재고 세부 정보 보기

각 배치에 대해 다음 작업을 수행할 수 있습니다 [(세부 사항 보기) 열기 [!UICONTROL Inspector])](placement-details-view.md), 는 배치의 모든 타겟팅된 사이트, 광고 및 거래를 나열합니다. 또한 배치에 대한 빈도 데이터도 포함됩니다. 탭에서 데이터를 선택적으로 내보낼 수 있습니다.

![배치 검사기](/help/dsp/assets/placement-inspector.png)

## 배치의 정보 [!UICONTROL Inspector] {#placement-inspector}

* **[!UICONTROL Sites]:** 배치가 인상을 받은 모든 사이트입니다.

  다음 [!UICONTROL Sites] 탭에는 검색 및 필터 기능, 기본 페이지에서 사용할 수 있는 동일한 표준 및 사용자 정의 열 보기 옵션, [!UICONTROL Exclude] 배치에서 사이트를 빠르게 제외할 수 있도록 각 행의 단추

* **[!UICONTROL Ads]:** 배치의 모든 광고.

  다음 [!UICONTROL Ads] 탭에는 검색 및 필터 기능, 기본 페이지에서 사용할 수 있는 동일한 표준 및 사용자 정의 열 보기 옵션, 각 행의 빠른 작업 버튼이 포함되어 있습니다. [!UICONTROL Pause] (따라서 광고를 빠르게 일시 중지할 수 있습니다.)

* **[!UICONTROL Frequency]:** 다음을 포함한 배치의 각 광고 빈도 수준에 대한 데이터:
   * 광고 빈도 수준(예: 사용자가 광고를 한 번 본 모든 인스턴스의 경우 &quot;1&quot;)
   * 예상 고유 장치/브라우저 또는 사람 수(지정된 항목에 따라 다름) [!UICONTROL Cross Device Level] (캠페인의 경우) 지정된 빈도 수준에서 노출시킨 사용자
   * 지정된 빈도 수준의 예상 노출 횟수
   * 지정된 빈도 수준의 예상 평균 빈도입니다. 이 값은 (예상 노출 횟수)/(예상 고유 수)와 같습니다.

* **[!UICONTROL Inventory]:** 배치의 타겟이 되는 모든 거래에 대한 정보.

  다음 [!UICONTROL Inventory] 탭에서는 다음과 같은 성능 통계를 표시하여 신속한 문제 해결을 지원합니다. [!UICONTROL Auctions], [!UICONTROL Bids], 및 [!UICONTROL Win Rate]. 탭에는 검색 및 필터 기능, 기본 페이지에서 사용할 수 있는 동일한 표준 및 사용자 정의 열 보기 옵션, 각 행의 빠른 작업 버튼이 포함되어 있습니다. [!UICONTROL Edit], [!UICONTROL View Report], 및 [[!UICONTROL Auction Insights] 추가적인 문제 해결을 위해](/help/dsp/inventory/private-deal-auction-insights.md).

## 를 엽니다. [!UICONTROL Placement Inspector]

1. 상위 캠페인 또는 패키지에 대한 배치 보기를 엽니다.

   * 상위 캠페인 내의 모든 배치 보기:

      1. 메인 메뉴에서 **[!UICONTROL Campaigns]**.

      1. 캠페인의 이름을 클릭합니다.

      1. 다음을 클릭합니다. **[!UICONTROL Placements]** 탭.

   * 상위 패키지 내의 모든 배치 보기:

      1. 메인 메뉴에서 **[!UICONTROL Campaigns]**.

      1. 캠페인의 이름을 클릭합니다.

      1. 다음을 클릭합니다. **[!UICONTROL Packages]** 탭.

      1. 상위 패키지의 이름을 클릭합니다.

1. 커서를 배치 행 위에 놓고 **[!UICONTROL More]**&#x200B;을 클릭하고 옵션을 클릭합니다.

   * 배치가 대상이 되는 모든 사이트를 보려면 **[!UICONTROL Sites]**.

   * 배치의 모든 광고를 보려면 **[!UICONTROL Ads]**.

   * 배치에 대한 빈도 데이터를 보려면 를 클릭합니다 **[!UICONTROL Frequency]**.

   * 배치 대상이 되는 모든 거래를 보려면 **[!UICONTROL Inventory]**.

1. (선택 사항) [열 보기 변경](campaign-data-views-manage.md#column-view-change) 필요한 경우 필요한 지표를 확인합니다.

1. (선택 사항) 탭에서 데이터를 내보내려면 ![자세히](/help/search-social-commerce/assets/more.png "자세히") 오른쪽 상단에서 **[!UICONTROL Export]**.

   데이터는 브라우저의 기본 다운로드 폴더에 XLSM 형식의 보고서로 저장됩니다.

## 인벤토리 문제 해결

| 문제 | 가능한 원인 | 수행할 작업 |
| -----------| ---------- | ---------- |
| [!UICONTROL Zero Auctions] | 게시자가 입찰 요청을 보내지 않았습니다. | 게시자에게 연락하여 거래를 활성화하십시오. |
| | 잘못된 외부 거래 ID를 입력하는 등 거래가 잘못 설정되었습니다. | 거래 세부 사항을 확인하고 거래를 편집합니다. |
| [!UICONTROL Auctions but no Bids] | 배치 타깃팅이 거래에 대한 수신 입찰 요청과 일치하지 않습니다. <br><br> 예를 들어, 배치는 거래에 적합하지 않은 지역을 타깃팅할 수 있습니다. | 타겟팅 불일치를 방지하기 위해 필요에 따라 배치 타겟을 편집합니다. |
| | 게재에 거래에 필요한 미디어 유형의 활성 광고가 없습니다. | 올바른 미디어 유형의 광고를 만들어 배치에 첨부합니다. |
| | 그 자리에는 충분한 예산이 없다. | 수신 요청에 대한 입찰을 허용하도록 배치 예산을 늘립니다. |
| | 배치 플라이트 날짜가 거래의 노출 전달 날짜와 겹치지 않습니다. | 필요에 따라 배치의 플라이트 날짜를 편집합니다. |
| [!UICONTROL Low Win Rate] | 배치의 최대 입찰(층 또는 고정)이 거래에서 요구하는 최소 입찰가보다 낮습니다. | 배치 늘리기 [!UICONTROL Max Bid] 필요한 경우. |
| | 배치에서는 입찰을 제한하는 사전 입찰 필터를 사용합니다. | 더 많은 입찰을 허용하도록 사전 입찰 필터의 임계값을 낮춥니다. |
| | 배치에 대한 대상 타깃팅이 너무 제한적입니다. | 지정된 대상 타겟에 활성 사용자가 충분한지 확인하고, 가능한 경우 대상을 확장합니다. |

>[!MORELIKETHIS]
>
>* [Campaign Management 보기의 성능 보고서 유형](campaign-reports-about.md)
>* [Campaign 데이터 보기 관리](campaign-data-views-manage.md)
