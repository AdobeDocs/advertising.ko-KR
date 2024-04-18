---
title: 배치에 대한 입찰 승수 관리
description: 지정된 배치 대상의 입찰 배수를 만들고 편집하는 방법에 대해 알아봅니다.
feature: DSP Placements
source-git-commit: 8d1cb46c8756c7312c6bd23e7a30118a8835ffd6
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 0%

---

# 배치에 대한 입찰 승수 관리


<!--

See if any of these procedures are implemented; may need to be edited and/or re-worded based on functionality/UI

-->

이 기능을 사용하여 기존 배치 대상의 입찰 배수를 변경할 수 있습니다.

배치에 대해 선택한 대상을 변경하려면 &quot;[배치 편집](/help/dsp/campaign-management/placements/placement-edit.md).&quot;

## 하나 이상의 배치에 대한 입찰 승수를 관리합니다.

선택한 모든 배치에 대해 값을 수동으로 편집하거나 값이 있는 스프레드시트를 업로드할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Campaigns]**.

1. 캠페인의 이름을 클릭합니다.

1. 하위 메뉴에서 **[!UICONTROL Placements]**.

1. 관리할 각 배치 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 를 클릭합니다 **[!UICONTROL ...]** > **[!UICONTROL Bid Multiplier]**.

1. 수동으로 또는 대상 값이 있는 CSV 파일을 업로드하여 적격 대상의 입찰 승수를 조정합니다.

   * 입찰 승수 값을 수동으로 조정하려면 각 대상별 탭([!UICONTROL Geo], [!UICONTROL Inventory], [!UICONTROL Sites], [!UICONTROL Audience], 및[!UICONTROL Brand Safety]) 배치 대상의 기존 값을 편집합니다.

   선택한 모든 배치에 동일한 변경 내용이 적용됩니다.

   * 기존 값을 덮어쓸 입찰 승수 값으로 CSV 파일을 업로드하려면:

     >[!NOTE]
     >
     >필드를 비워 두면 해당 대상 유형에 대한 모든 값이 삭제됩니다.<!-- Verify and re-word if needed. I'm not sure if you'll be able to have multiple data rows (one per placement) or if there will be only one data row applicable for all. -->

      1. 클릭 **[!UICONTROL CSV Edit]** 오른쪽 상단에 있습니다.

      1. a) 클릭 **[!UICONTROL Download Template]** 입찰 승수 값을 편집하거나 b) 이전에 다운로드한 템플릿을 편집합니다. 편집된 파일을 장치 또는 네트워크에 저장합니다.

      1. a) 편집된 파일을 상자로 드래그하여 놓거나 b) 상자 내부를 클릭하여 장치나 네트워크에서 파일을 선택합니다.

   1. 클릭 **[!UICONTROL Upload]**.

   기본적으로 대상에 대한 입찰 승수는 1.00이며, 이는 입찰이 해당 대상에 대해 조정되지 않음을 의미합니다. 값의 범위는 0.10부터 10.00까지입니다. 예를 들어, 입찰 수정자 0.5는 USD 6 입찰을 USD 3으로 감소시킵니다(0.5 x 6). 다음에 대한 입찰 승수(1.00 이외의 값 사용)를 설정할 수 있습니다. [제한된 타겟 수](#bid-multiplier-limits-by-target).

   경매에서 여러 입찰 수정자를 사용할 수 있는 경우 적용 가능한 모든 입찰 수정자를 곱합니다.

   입찰 수정자는 입찰가를 최대 입찰가 이상으로 증가시키지 않습니다.

1. 클릭 **[!UICONTROL Save]**.

-->

## 스프레드시트를 업로드하여 단일 배치에 대한 입찰 승수를 관리합니다.<!-- Is this still going to exist independently, or will you just do this via the "Bid Multiplier" option in the main context menu for placements? If both options, then reword headings for distinction -->

업로드된 파일의 변경 사항은 기존 입찰 승수 값을 덮어씁니다.<!-- what if you delete a row? -->

1. 메인 메뉴에서 **[!UICONTROL Campaigns]**.

1. 캠페인의 이름을 클릭합니다.

1. 하위 메뉴에서 **[!UICONTROL Placements]**.

1. 배치 이름 옆에 있는 를 클릭합니다  **[!UICONTROL ...]** > **[!UICONTROL Upload Bid Multiplier Excel Sheet]**.

1. 
   <!-- Verify the rest of these steps. -->

1. a) 클릭 **[!UICONTROL Download Template]** 입찰 승수 값을 편집하거나 b) 이전에 다운로드한 템플릿을 편집합니다. 편집된 파일을 장치 또는 네트워크에 저장합니다.

   기본적으로 대상에 대한 입찰 승수는 1.00이며, 이는 입찰이 해당 대상에 대해 조정되지 않음을 의미합니다. 값의 범위는 0.10부터 10.00까지입니다. 예를 들어, 입찰 수정자 0.5는 USD 6 입찰을 USD 3으로 감소시킵니다(0.5 x 6). 다음에 대한 입찰 승수(1.00 이외의 값 사용)를 설정할 수 있습니다. [제한된 타겟 수](#bid-multiplier-limits-by-target).

   경매에서 여러 입찰 수정자를 사용할 수 있는 경우 적용 가능한 모든 입찰 수정자를 곱합니다.

   입찰 수정자는 입찰가를 최대 입찰가 이상으로 증가시키지 않습니다.

1. a) 편집된 파일을 상자로 드래그하여 놓거나 b) 상자 내부를 클릭하여 장치나 네트워크에서 파일을 선택합니다.

1. 클릭 **[!UICONTROL Upload]**.

1. 클릭 **[!UICONTROL Save]**.

## 입찰 승수에 적합한 대상 유형 {#bid-multiplier-by-target}

이(가) 여기서 중복 제거되지 않음

## 대상 유형별 최대 입찰 승수 {#bid-multiplier-limits-by-target}

이(가) 여기서 중복 제거되지 않음

<!--

>[!MORELIKETHIS]
>
>* [About Placement Management](placement-about.md)
>* [Edit a Placement](placement-edit.md)
>* [View the Change Log for a Placement](placement-change-log.md)
>* [Placement Settings](placement-settings.md)
 -->
