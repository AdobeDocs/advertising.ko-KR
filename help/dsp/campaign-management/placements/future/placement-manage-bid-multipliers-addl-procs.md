---
title: 배치에 대한 입찰 승수 관리
description: 학습 xxx
feature: DSP Placements
source-git-commit: b6758541b59f1fd924a2fe83c769f5ba385409aa
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---

# XXX

## 단일 배치에 대한 입찰 승수 관리

1. 메인 메뉴에서 **[!UICONTROL Campaigns]**.

1. 캠페인의 이름을 클릭합니다.

1. 하위 메뉴에서 **[!UICONTROL Placements]**.

1. 배치 이름 옆에 있는 를 클릭합니다  **[!UICONTROL ...]** > **[!UICONTROL Bid Multiplier]**.

1. 적격 대상에 대한 입찰 승수를 조정합니다.

   * 입찰 승수 값을 수동으로 조정하려면 각 값으로 이동합니다. [target별 탭](#bid-multiplier-by-target) ([!UICONTROL Geo], [!UICONTROL Inventory], [!UICONTROL Sites], [!UICONTROL Audience], 및 [!UICONTROL Brand Safety]) 배치 대상의 기존 값을 편집합니다.

     대부분의 대상 카테고리는 왼쪽에 하위 카테고리를 나열합니다. 해당되는 경우 하위 범주를 클릭하여 해당 하위 범주에 대한 입찰 승수를 관리합니다.

   * 입찰 승수 값이 있는 CSV 파일을 업로드하여 기존 값을 모두 덮어쓰려면 다음을 수행합니다.

      1. 클릭 **[!UICONTROL CSV File Edit]** 오른쪽 상단에 있습니다.

      1. a) 클릭 **[!UICONTROL Download Template]** 를 클릭하고 파일을 편집합니다. 또는 b) 이전에 다운로드한 템플릿을 편집합니다. 편집된 파일을 장치 또는 네트워크에 저장합니다.

         다운로드한 템플릿에는 각 대상 유형(예: 국가, 소스 및 사이트 카테고리)에 대해 하나의 시트가 포함됩니다. 값이 1.0이 아닌 기존 입찰 승수만 포함됩니다.

         * 기존 대상에 대한 입찰 승수를 추가하려면 사용자 인터페이스에 표시되는 동일한 구문과 해당 입찰 승수 값을 사용하여 대상을 입력합니다.

         * 입찰 수정자를 제거하려면 입찰 승수 값을 1.0으로 설정하거나 행에 대한 모든 정보를 삭제합니다.

         ![입찰 승수 스프레드시트 파일의 행 예](/help/dsp/assets/bid-multiplier-spreadsheet.png "입찰 승수 스프레드시트 파일의 행 예")

      1. 클릭 **[!UICONTROL Next]** 로 이동 [!UICONTROL Upload File] 섹션과 a) 편집된 파일을 상자로 드래그하여 놓거나 b) 상자 안을 클릭하여 장치나 네트워크에서 파일을 선택합니다.

      1. 에서 업로드된 데이터 확인 [!UICONTROL Review & Submit] 섹션을 클릭한 다음 **[!UICONTROL Save]**.

## 하나 이상의 배치에 대한 입찰 승수를 관리합니다.

<!-- verify all and edit accordingly -->

1. 메인 메뉴에서 **[!UICONTROL Campaigns]**.

1. 캠페인의 이름을 클릭합니다.

1. 하위 메뉴에서 **[!UICONTROL Placements]**.

1. 관리할 각 배치 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 를 클릭합니다 **[!UICONTROL ...]** > **[!UICONTROL Upload Bid Multiplier Excel Sheet]**.

<!-- Check the following this functionality when available in UAT -->

1. 적격 대상에 대한 입찰 승수를 조정합니다.

   * 입찰 승수 값을 수동으로 조정하려면 각 대상별 탭([!UICONTROL Geo], [!UICONTROL Inventory], [!UICONTROL Sites], [!UICONTROL Audience], 및[!UICONTROL Brand Safety]) 배치 대상의 기존 값을 편집합니다.

   선택한 모든 배치에 동일한 변경 내용이 적용됩니다.

* 입찰 승수 값이 있는 CSV 파일을 업로드하여 기존 값을 모두 덮어쓰려면 다음을 수행합니다.

   1. 클릭 **[!UICONTROL CSV File Edit]** 오른쪽 상단에 있습니다.

   1. a) 클릭 **[!UICONTROL Download Template]** 를 클릭하고 파일을 편집합니다. 또는 b) 이전에 다운로드한 템플릿을 편집합니다. 편집된 파일을 장치 또는 네트워크에 저장합니다.

      다운로드한 템플릿에는 각 대상 유형(예: 국가, 소스 및 사이트 카테고리)에 대해 하나의 시트가 포함됩니다. 값이 1.0이 아닌 기존 입찰 승수만 포함됩니다.

      * 기존 대상에 대한 입찰 승수를 추가하려면 사용자 인터페이스에 표시되는 동일한 구문과 해당 입찰 승수 값을 사용하여 대상을 입력합니다.

      * 입찰 수정자를 제거하려면 입찰 승수 값을 1.0으로 설정하거나 행에 대한 모든 정보를 삭제합니다.

      ![입찰 승수 스프레드시트 파일의 행 예](/help/dsp/assets/bid-multiplier-spreadsheet.png "입찰 승수 스프레드시트 파일의 행 예")

   1. 클릭 **[!UICONTROL CSV Edit]** 오른쪽 상단에 있습니다.

   1. a) 클릭 **[!UICONTROL Download Template]** 입찰 승수 값을 편집하거나 b) 이전에 다운로드한 템플릿을 편집합니다. 편집된 파일을 장치 또는 네트워크에 저장합니다.

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
>* [Edit Placements](placement-edit.md)
>* [View the Change Log for a Placement](placement-change-log.md)
>* [Placement Settings](placement-settings.md)
 -->
