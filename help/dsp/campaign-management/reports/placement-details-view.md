---
title: 배치에 대한 사이트, 광고, 빈도 및 재고 세부 정보 보기
description: 배치에 대한 타겟팅된 사이트, 광고, 빈도 및 인벤토리 데이터를 보는 방법에 대해 알아봅니다.
feature: DSP Placements
exl-id: b58b442c-2fb8-4a78-9be9-d85aa83136e2
source-git-commit: 0f022babeab6c044949760cedc103323eb0cc950
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# 배치에 대한 사이트, 광고, 빈도 및 재고 세부 정보 보기

각 배치에 대해 [배치 내 모든 타겟팅된 사이트, 광고 및 거래를 나열하는 (세부 정보 보기 [!UICONTROL Inspector])](placement-details-view.md)을(를) 열 수 있습니다. 또한 배치에 대한 빈도 데이터도 포함됩니다. 탭에서 데이터를 선택적으로 내보낼 수 있습니다.

![배치 검사자](/help/dsp/assets/placement-inspector.png)

## 배치 [!UICONTROL Inspector]의 정보 {#placement-inspector}

* **[!UICONTROL Sites]:** 배치에 노출 횟수가 있는 모든 사이트입니다.

  [!UICONTROL Sites] 탭에는 검색 및 필터 기능, 기본 페이지에서 사용할 수 있는 동일한 표준 및 사용자 지정 열 보기 옵션, 각 행의 [!UICONTROL Exclude] 단추가 포함되어 있으므로 배치에서 사이트를 빠르게 제외할 수 있습니다.

* **[!UICONTROL Ads]:** 배치의 모든 광고.

  [!UICONTROL Ads] 탭에는 검색 및 필터 기능, 기본 페이지에서 사용할 수 있는 동일한 표준 및 사용자 지정 열 보기 옵션, 각 행의 빠른 작업 단추(예: [!UICONTROL View Ad Approvals])가 포함되어 있습니다.

* 다음을 포함하여 배치에 대한 각 광고 빈도 수준의 **[!UICONTROL Frequency]:** 데이터:
   * 광고 빈도 수준(예: 사용자가 광고를 한 번 본 모든 인스턴스의 경우 &quot;1&quot;)
   * 지정된 빈도 수준에서 노출을 받은 예상 고유 장치/브라우저 또는 사용자 수(캠페인에 대해 지정된 [!UICONTROL Cross Device Level]에 따라 다름)
   * 지정된 빈도 수준의 예상 노출 횟수
   * 지정된 빈도 수준의 예상 평균 빈도입니다. 이 값은 (예상 노출 횟수)/(예상 고유 수)와 같습니다.

* **[!UICONTROL Inventory]:** 배치의 타겟이 되는 모든 거래에 대한 정보입니다.

  [!UICONTROL Inventory] 탭에서는 [!UICONTROL Auctions], [!UICONTROL Bids] 및 [!UICONTROL Win Rate]과(와) 같은 성능 통계를 표시하여 문제를 빠르게 해결할 수 있습니다. 탭에는 검색 및 필터 기능, 기본 페이지에서 사용할 수 있는 동일한 표준 및 사용자 지정 열 보기 옵션, 추가 문제 해결을 위한 [!UICONTROL Edit], [!UICONTROL View Report] 및 [[!UICONTROL Auction Insights]을(를) 비롯한 각 행의 빠른 작업 버튼이 포함되어 있습니다](/help/dsp/inventory/private-deal-auction-insights.md).

## [!UICONTROL Placement Inspector] 열기 {#inspector-open}

1. 상위 캠페인 또는 패키지에 대한 배치 보기를 엽니다.

   * 상위 캠페인 내의 모든 배치 보기:

      1. 주 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

      1. 캠페인의 이름을 클릭합니다.

      1. **[!UICONTROL Placements]** 탭을 클릭합니다.

   * 상위 패키지 내의 모든 배치 보기:

      1. 주 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

      1. 캠페인의 이름을 클릭합니다.

      1. **[!UICONTROL Packages]** 탭을 클릭합니다.

      1. 상위 패키지의 이름을 클릭합니다.

1. 커서를 배치 행 위에 놓고 **[!UICONTROL ...]** > **[!UICONTROL Analyze]** > **[!UICONTROL Inspector]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) [필요한 지표를 보려면 필요에 따라 열 보기를 변경](campaign-data-views-manage.md#column-view-change)합니다.

1. (선택 사항) 탭에서 데이터를 내보내려면 오른쪽 상단의 ![자세히](/help/search-social-commerce/assets/more.png "자세히")를 클릭한 다음 **[!UICONTROL Export]**&#x200B;을(를) 클릭합니다.

   데이터는 브라우저의 기본 다운로드 폴더에 XLSM 형식의 보고서로 저장됩니다.

## [!UICONTROL Placement Inspector]의 배치에서 광고 제거 {#remove-ads-placement-inspector}

1. [[!UICONTROL Placement Inspector]](#inspector-open)을(를) 엽니다.

1. **[!UICONTROL Ads]** 탭을 클릭합니다.

1. 광고 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Detach]**&#x200B;을(를) 클릭합니다.

## 인벤토리 문제 해결

| 문제 | 가능한 원인 | 수행할 작업 |
| -----------| ---------- | ---------- |
| [!UICONTROL Zero Auctions] | 게시자가 입찰 요청을 보내지 않았습니다. | 게시자에게 연락하여 거래를 활성화하십시오. |
| | 잘못된 외부 거래 ID를 입력하는 등 거래가 잘못 설정되었습니다. | 거래 세부 사항을 확인하고 거래를 편집합니다. |
| [!UICONTROL Auctions but no Bids] | 배치 타깃팅이 거래에 대한 수신 입찰 요청과 일치하지 않습니다. <br><br> 예를 들어 게재에서 거래에 적합하지 않은 지역을 대상으로 할 수 있습니다. | 타겟팅 불일치를 방지하기 위해 필요에 따라 배치 타겟을 편집합니다. |
| | 게재에 거래에 필요한 미디어 유형의 활성 광고가 없습니다. | 올바른 미디어 유형의 광고를 만들어 배치에 첨부합니다. |
| | 그 자리에는 충분한 예산이 없다. | 수신 요청에 대한 입찰을 허용하도록 배치 예산을 늘립니다. |
| | 배치 플라이트 날짜가 거래의 노출 전달 날짜와 겹치지 않습니다. | 필요에 따라 배치의 플라이트 날짜를 편집합니다. |
| [!UICONTROL Low Win Rate] | 배치의 최대 입찰(층 또는 고정)이 거래에서 요구하는 최소 입찰가보다 낮습니다. | 필요에 따라 배치의 [!UICONTROL Max Bid]을(를) 늘립니다. |
| | 배치에서는 입찰을 제한하는 사전 입찰 필터를 사용합니다. | 더 많은 입찰을 허용하도록 사전 입찰 필터의 임계값을 낮춥니다. |
| | 배치에 대한 대상 타깃팅이 너무 제한적입니다. | 지정된 대상 타겟에 활성 사용자가 충분한지 확인하고, 가능한 경우 대상을 확장합니다. |

>[!MORELIKETHIS]
>
>* [캠페인 관리 보기의 성능 보고서 유형](campaign-reports-about.md)
>* [Campaign 데이터 보기 관리](campaign-data-views-manage.md)
