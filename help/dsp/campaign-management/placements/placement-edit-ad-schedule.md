---
title: 배치에 대한 광고 일정 편집
description: 배치에 첨부된 광고의 광고 일정을 변경하는 방법에 대해 알아봅니다.
feature: DSP Placements
exl-id: 4c981d57-032f-4cde-858a-e9ac2bf2e6f2
source-git-commit: ae1a58bd0aed430cd2914146dfb2850bc8125025
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---

# 배치에 대한 광고 일정 편집

## 하나 이상의 배치에 대한 광고 일정 편집

를 사용하여 여러 배치에 첨부된 광고의 예약된 비행 날짜 및 광고 순환을 변경할 수 있습니다. [!DNL Microsoft Excel] 스프레드시트입니다. 각 광고는 여러 비행 중에 활성화될 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Campaigns]**.

1. 캠페인의 이름을 클릭합니다.

1. 하위 메뉴에서 **[!UICONTROL Placements]**.

1. 광고 데이터를 다운로드할 각 배치 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 를 클릭합니다 **[!UICONTROL ...]** > **[!UICONTROL Download Custom Ad Schedule Sheet]**.

1. 파일을 사용할 수 있으면 **[!UICONTROL Download]** 브라우저의 일반적인 절차에 따라 워크시트 파일(XLSX 형식)을 다운로드할 수 있는 브라우저 페이지 맨 위에 있는 알림입니다.

   ![준비 알림 다운로드](/help/dsp/assets/download-ready.png "준비 알림 다운로드")

1. 다운로드한 파일을 열고 해당 비행에 포함할 각 광고 행에 대한 비행 정보 필드를 편집한 다음 업데이트된 파일을 저장합니다.

   * **[!UICONTROL Flight N Start Date]** / **[!UICONTROL Flight N End Date]** (예: [!UICONTROL Flight 1 Start Date] 및 [!UICONTROL Flight 1 End Date]): 비행의 첫 번째 날짜와 마지막 날짜입니다. 각 날짜에 대해 YYYY-MM-DD 형식을 사용합니다. 비어 있는 플라이트 날짜 필드가 있는 모든 광고는 비참여 광고로 처리됩니다.

   * **[!UICONTROL Flight N Weight]** (예: [!UICONTROL Flight 1 Weight]): 비행에 대한 광고를 회전하는 방법. 값 입력:

      * 비행에 대한 광고를 균등하게 회전하려면 다음을 입력합니다. `[!UICONTROL Even]`.

      * 비행에 대한 광고를 불균일하게 회전하려면 각 광고를 회전시킬 상대적 가중치를 백분율로 입력합니다(예: `40` 40%의 경우). 비행기의 총 무게는 100이어야 합니다.

1. 편집된 광고 일정 템플릿을 업로드합니다.

   1. 적용 가능한 각 배치 옆의 확인란을 선택합니다.

   1. 일괄 작업 도구 모음에서 를 클릭합니다 **[!UICONTROL ...]** > **[!UICONTROL Upload Custom Ad Schedule Sheet]**&#x200B;을 클릭하고 업로드할 파일을 지정합니다.

## 단일 배치에 대한 광고 일정 편집

<!-- Some placements don't have this option. Clarify which placement types aren't eligible -- just simple ad serving placements (PG ones seem okay)? And anything else? -->

배치에 첨부된 광고의 예약된 비행 날짜 및 광고 순환을 변경할 수 있습니다. 각 광고는 여러 비행 중에 활성화될 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Campaigns]**.

1. 캠페인의 이름을 클릭합니다.

1. 하위 메뉴에서 **[!UICONTROL Placements]**.

1. 배치 이름 옆에 있는 를 클릭합니다  **[!UICONTROL ...]** > **[!UICONTROL Ad schedule]**.

1. 다음 중 하나를 수행합니다.

   * 항공편을 추가하려면 **[!UICONTROL Add Flight]**&#x200B;를 클릭한 다음 시작 날짜와 종료 날짜를 지정합니다.

   * 기존 비행을 광고에 추가하려면 **[!UICONTROL +]** (비행 열의 광고 행).

   * 광고에서 기존 항공편을 제거하려면 **[!UICONTROL x]** (비행 열의 광고 행).

      * (여러 광고의 비행 시간이 동일한 경우) 광고를 불균일하게 회전하려면 다음을 클릭하십시오. **[!UICONTROL Even Rotation]** 그런 다음 각 광고를 회전할 상대적 가중치를 백분율로 입력합니다.

        총 가중치는 100이어야 합니다.

1. 오른쪽 상단에서 **[!UICONTROL Continue]**.

1. 비행 세부 사항을 검토한 다음 **[!UICONTROL Save & Finish]**.

>[!MORELIKETHIS]
>
>* [배치 관리 정보](placement-about.md)
>* [배치 편집](placement-edit.md)
>* [배치에 대한 변경 로그 보기](placement-change-log.md)
>* [배치 설정](placement-settings.md)
