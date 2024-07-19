---
title: '[!UICONTROL Simple Ad Serving] 거래 설정'
description: '[!UICONTROL Simple Ad Serving] 거래에 사용 가능한 설정에 대해 알아봅니다.'
feature: DSP Simple Ad Serving
exl-id: 20e23182-d3d0-457f-a821-0ad4770a138d
source-git-commit: 14f78b89dea8cc680756232c6116975c652feee5
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# [!UICONTROL Simple Ad Serving] 거래 설정

## 새 [!UICONTROL Simple Ad Serving] 거래

### [!UICONTROL Select Ad Source]

| 매개 변수 | 설명 |
|-----------|-------------|
| **[!UICONTROL Serving Type]** | 이 거래의 미디어 유형: *[!UICONTROL Video],* *[!UICONTROL Display],* 또는 *[!UICONTROL Audio].* |
| **[!UICONTROL Publisher Site Served On]** | 이 재고를 판매하는 게시자의 이름입니다. 이름에 처음 두 개 이상의 문자를 입력하여 게시자를 검색합니다. 목록에 없는 게시자를 추가하려면 Adobe 계정 팀에 문의하십시오. |
| **[!UICONTROL Advertiser]** | 이 거래에 액세스할 수 있는 계정의 단일 광고주입니다. 또한 캠페인 및 (선택적으로) 거래를 사용할 수 있는 패키지를 선택합니다. |
| **[!UICONTROL Media Quality Assessment?]** | (일부 사용자) 서드파티 확인을 위해 다른 DSP에서 광고를 실행할 수 있도록 합니다. <!-- Who can select this? It's disabled for me. Need to see if there are additional fields when this is enabled. --> |
| **[!UICONTROL Ad Source]** | 유일한 옵션은 *[!UICONTROL Site Serve (Event Pixels)]*&#x200B;입니다. |
| **[!UICONTROL Ad Creation]** | (새 거래만 해당):<ul><li>*[!UICONTROL Create New]:* 이 거래에 대한 광고를 만듭니다.</li><li>*[!UICONTROL Select Ads]:* 이 거래에 기존 광고를 사용합니다.</li></ul> |
| **[!UICONTROL Ad Type]** | 이 거래의 광고 유형. 거래에 대한 광고를 만들려면 요청에 따라 광고 크기 또는 기간을 포함하십시오. 사용 가능한 옵션은 미디어 유형에 따라 다릅니다. |

{style="table-layout:auto"}

### [!UICONTROL Select Ad(s)]

(기존 광고를 사용하는 경우) 거래에 포함할 광고입니다. 포함할 각 광고 옆에 있는 확인란을 선택합니다.

### [!UICONTROL Select & Upload [Media Type]]

(새 광고만 해당) Screens에서 새 [타사 광고](/help/dsp/campaign-management/ads/ad-create-multiple.md)를 만들 수 있습니다.

### [!UICONTROL Feed Details]

| 매개 변수 | 설명 |
|-----------|-------------|
| **[!UICONTROL Media CPM]** | 계약에 대한 요금 카드에 반영된 CPM(1000회 노출당 비용) 이 값에 대해서는 Adobe 계정 팀에 문의하십시오. <br><br>거래의 통화도 지정하십시오. 모든 사용자는 USD를 선택하거나, SSP가 추가 통화를 지원하는 경우 DSP 계정에 대한 통화를 선택할 수 있습니다. |
| **[!UICONTROL Third Party Billed Fees]** | (선택 사항) 청구 불가능한 비용으로 추적할 정적 타사 수수료 및 거래에 대한 통화.<br><br>모든 사용자는 USD를 선택할 수 있으며, SSP에서 추가 통화를 지원하는 경우 DSP 계정의 통화를 선택할 수 있습니다. **참고:** 청구 가능 요금은 [!UICONTROL Net CPM] 지표에 반영됩니다. |
| **[!UICONTROL Third Party Fee Description]** | (선택 사항) 타사 요금에 대한 설명입니다. |
| **[!UICONTROL Flight Dates]** | 이 거래를 사용하는 트래픽의 시작 날짜와 종료 날짜입니다. 비행 날짜는 캠페인 비행 날짜 내에 포함되어야 합니다. 광고 태그는 지정된 비행 중에만 응답을 반환합니다.<br><br> 1년 동안 지속되는 별도의 간단한 광고 제공 캠페인을 만들고 그 안에 추적 픽셀을 빌드하는 것이 좋습니다. |
| **[!UICONTROL Impressions]** | (선택 사항) 이 거래를 사용하여 실행할 것으로 예상되는 노출 횟수입니다. 이 값은 추적 목적으로만 사용되고 게재 목표가 충족될 때 플래그하는 데 사용됩니다. 게시자는 실제 광고 게재를 제어합니다. 가장 좋은 방법은 태그를 DSP 내에서 활성 상태로 유지하기 위해 많은 노출수를 입력하여 필요한 경우 갱신 또는 연장할 수 있도록 하는 것입니다. |
| **[!UICONTROL Deal Name]** | 거래 이름. 이름을 입력하거나 *[!UICONTROL Auto Generate Deal Name]*&#x200B;을(를) 선택하여 DSP이 거래 세부 정보를 기반으로 이름을 생성하도록 합니다.<br><br>자동 생성된 이름의 예: `Campaign-desktop_video_preroll_15-24Kitchen-$10_USD-jdoe-SAS` |
| **[!UICONTROL Attached Ads]** | (읽기 전용) 거래의 일부인 광고입니다. 광고를 편집하려면 광고 이름을 클릭합니다. 거래에서 광고를 제거하려면 광고 이름 옆에 있는 **[!UICONTROL X]**&#x200B;을(를) 클릭합니다. |

{style="table-layout:auto"}

<!-- 
## Existing Simple Ad Serving Deals

Changes aren't applied retroactively.
-->

<!-- completely different settings layout, so need a separate section for them -->

<!-- From Abhinav: Editable fields are Name, Start & End date, Impressions & CPM. Changes are not applied retroactively.

But I see:

| Parameter | Description |
|-----------|-------------|

| **[!UICONTROL Are you using Deal ID?] | (Read-only) Whether the deal was set up as a [!UICONTROL Deal ID] (*[!DNL Yes]*)  or a [!UICONTROL Simple Ad Serving] deal (*[!DNL No]*). |
| **[!UICONTROL Inventory Type] | (Read-only) The inventory type for the deal. |
| **[!UICONTROL Feed Name] | The name of the [!UICONTROL Simple Ad Serving] deal. |
| **[!UICONTROL Publisher Ad Server] | (Read-only)  |
| **[!UICONTROL Publisher maximum ad length] | The maximum length of the ad, per the publisher. |
| **[!UICONTROL Publisher minimum ad length] | The minimum length of the ad, per the publisher. |
| **[!UICONTROL Fill Type] | (Read-only)  |
| **[!UICONTROL Contracted CPM] | This field is required if billing through TubeMogul, but enter your CPM in this field to track your actual spend. |
| **[!UICONTROL 3rd party technology CPM] | (Optional)  |
| **[!UICONTROL Planned Flight Dates] | The beginning and end dates for the deal flight. These dates don't control ad delivery but are used to track delivery pacing. **THIS IS CONTRARY TO WHAT THE NEW DEAL SETTINGS ABOVE, FROM ABHINAV, SAY**> |
| **[!UICONTROL Target Impressions] | (Optional) The estimated number of impressions you expect to run using this deal. This value is used for tracking purposes only and to flag when delivery goals are met; the publisher controls actual ad delivery. The best practice is to enter a high number of impressions to keep the tag active within DSP so it can be renewed or extended if needed. |
 -->

>[!MORELIKETHIS]
>
>* [정보 [!UICONTROL Simple Ad Serving]](simple-deal-about.md)
>* [[!UICONTROL Simple Ad Serving] 거래 만들기](simple-deal-create.md)
>* [거래 설정 [!UICONTROL Simple Ad Serving]개 편집](simple-deal-edit.md)
>* [거래에 대한 자세한 보고서 보기](/help/dsp/inventory/deal-view-report.md)

<!-- add back when reimplemented:
>* [View Event-Tracking Pixels for a [!UICONTROL Simple Ad Serving] Deal](simple-deal-show-pixels.md)
-->
