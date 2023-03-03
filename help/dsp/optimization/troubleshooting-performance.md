---
title: 문제 해결 성능
description: 일반적인 성능 문제를 참조하여 이를 해결하는 방법에 대해 알아보십시오.
feature: DSP Optimization
exl-id: b87f8556-1908-40c1-9f98-fbdc6d9b59b1
source-git-commit: 14f78b89dea8cc680756232c6116975c652feee5
workflow-type: tm+mt
source-wordcount: '519'
ht-degree: 0%

---

# 문제 해결 성능

| 문제 | 가능한 원인 | 수행할 작업 |
| --- | --- | --- |
| 배치에 지출 없음 | 게재에 광고가 포함되지 않으며/거나 광고가 활성화되지 않습니다. | 예상되는 모든 광고가 배치에 첨부되고 승인되었으며 활성 상태인지 확인합니다.<br><br>또한 배치에 사용자 지정 광고 일정이 포함되어 있는지 확인하십시오. 이러한 일정은 각 광고의 비행 기간을 제한할 수 있습니다. 배치 보기에서 배치에 대한 광고 일정을 보려면  **[!UICONTROL ...]** > **[!UICONTROL Ad schedule]** 을 클릭합니다. |
|  | 영향을 받는 날짜가 구성된 비행 날짜 내에 없습니다. | 비행 날짜가 캠페인, 패키지 및 배치 수준에서 유효한지 &#x200B; 확인하십시오. |
|  | 예산 목표가 달성되었거나 충분히 높지 않습니다. | 캠페인, 패키지 및 배치 수준에서 예산 설정을 확인합니다. |
|  | 그 계좌에는 자금이 충분하지 않다. | 계정에 충분한 자금이 공급되었는지 확인하려면 다음 위치로 이동하십시오. **[!UICONTROL Settings]** > **[!UICONTROL Account]** and look at the amount금액 of [!UICONTROL Usable Funds]. 자금을 더 추가해야 하는 경우 Adobe 계정 팀에 문의하십시오. |
|  | 사용 가능한 인벤토리가 없습니다. | 지정된 인벤토리 소스([!UICONTROL Public], [!UICONTROL Private], 또는 [!UICONTROL On Demand]):<ul><li>올바르게 설정합니다.</li><li>경매를 통한 활성 및 전송.</li><li>해당 광고 및 배치 유형과 호환됩니다.</li></ul><br>재고 출처가 모두 유효하고 활성 상태인 경우, 가능한 경우 추가 또는 모든 재고 출처를 대상으로 지정합니다. |
|  | 사용 가능한 사용자가 없습니다. | 지정된 대상 타겟에 활성 사용자가 충분히 포함되어 있는지 확인하십시오. 대상이 없다면 대상을 더 추가하여 대상을 확장합니다. |
| 배치 비용 절감 | 다음 [!UICONTROL Non Bids] 배치 진단 보고서의 섹션은 배치가 입찰되지 않은 가능한 이유를 보여줍니다. | [리뷰 [!UICONTROL Non Bids] 보고서](/help/dsp/campaign-management/reports/placement-diagnostics.md) 왜 배치를 입찰하지 않았는지 이해하기 위해서.  <!-- add link/edit text when file available: See the [in-depth guide to possible Non-Bid Reasons (NBR)](link) for more information. --> |
|  | 배치는 를 사용합니다 [사전 입찰 필터](/help/dsp/campaign-management/placements/placement-settings.md) 입찰을 제한합니다. | 사전 입찰 필터의 임계값을 5% 낮춰 지출과 성능의 균형을 평가합니다. <!-- wording? and are users just supposed to manually monitor whether it makes a difference? --><br><br>사전 입찰 필터, 지역, 인벤토리 및 대상과 같은 여러 배치 타겟을 사용하면 입찰과 지출을 누적적으로 제한할 수 있습니다. |
|  | 이 배치는 승률이 낮습니다. | 늘리기 [!UICONTROL Max Bid] 승률을 높이기 위해.<br><br><b>참고:</b> 재고 가격은 배치 타겟팅에 따라 달라질 수 있습니다.<br><br>10%의 승률은 건강한 것으로 간주된다. |
|  | 적은 수의 재고를 사용할 수 있습니다. | 가능한 경우 추가 또는 모든 재고 소스를 Target.<br><br>사전 입찰 필터, 지역, 인벤토리 및 대상과 같은 여러 배치 타겟을 사용하면 입찰과 지출을 누적적으로 제한할 수 있습니다. |
|  | 사용 가능한 사용자 수가 적습니다. | 지정된 대상 타겟에 활성 사용자가 충분히 포함되어 있는지 확인하십시오. 대상이 없다면 대상을 더 추가하여 대상을 확장합니다.<br><br>사전 입찰 필터, 지역, 인벤토리 및 대상과 같은 여러 배치 타겟을 사용하면 입찰과 지출을 누적적으로 제한할 수 있습니다. |
|  | 패키지에는 많은 활성 배치가 포함되어 있습니다. | 패키지 내 활성 배치 수를 줄이거나 전체 패키지 예산을 늘립니다.<br><br>패키지에 배치가 많지만 예산이 충분하지 않은 경우 DSP이 각 배치에 충분한 예산을 할당하지 못할 수 있습니다. 각 배치에는 최소 2USD/일을 사용할 수 있는 기회가 있어야 합니다. 예를 들어 패키지의 예산이 10 USD/일인 경우 5개 이하의 배치를 포함하는 것이 가장 좋습니다. &#x200B; |

{style=&quot;table-layout:auto&quot;}

>[!MORELIKETHIS]
>
>* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)
>* [패키지 설정](/help/dsp/campaign-management/packages/package-settings.md)
>* [캠페인 설정](/help/dsp/campaign-management/campaigns/campaign-settings.md)

