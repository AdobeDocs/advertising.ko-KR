---
title: URL 목록 관리
description: 배치 타깃팅용 URL 목록을 만들고 관리하는 방법을 알아봅니다.
feature: DSP Placements
source-git-commit: ea33d6fa7612f1c9631c223e5bf0ec80bb5f8d96
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 0%

---

# URL 목록 관리

배치 타깃팅을 위해 웹 사이트 및 앱 URL 목록을 만들고 관리할 수 있습니다. 배치 설정 내에서 특정 URL 목록을 타겟팅하거나 제외합니다.

## URL 목록 보기

1. 메인 메뉴에서 **[!UICONTROL Resources]** > **[!UICONTROL URL Lists]**&#x200B;을(를) 클릭합니다.

1. 목록 이름을 클릭합니다.

1. (선택 사항) 선택한 목록을 XLSX([!DNL Microsoft Excel] 스프레드시트) 형식으로 내보내려면 ![내보내기](/help/dsp/assets/export.png "내보내기") **[!UICONTROL Export]**&#x200B;를 클릭합니다.

   브라우저의 일반적인 절차에 따라 파일이 다운로드됩니다.

## URL 목록 만들기

1. 메인 메뉴에서 **[!UICONTROL Resources]** > **[!UICONTROL URL Lists]**&#x200B;을(를) 클릭합니다.

1. 오른쪽 상단에서 **[!UICONTROL Create].**&#x200B;을(를) 클릭합니다

1. **[!UICONTROL List name]**&#x200B;을(를) 입력한 다음 **[!UICONTROL Create].**&#x200B;을(를) 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * 추가할 URL을 수동으로 입력하거나 붙여넣으려면:

      1. **[!UICONTROL Bulk Add URLs]** > **[!UICONTROL Copy/Paste URLs]**&#x200B;을(를) 클릭합니다.

      1. 각 URL이 별도의 줄에 있는 최대 10,000개의 URL을 입력하거나 붙여 넣습니다.

      1. **[!UICONTROL Validate]**&#x200B;을(를) 클릭하여 URL이 유효한지 확인합니다.

         잘못된 URL이 식별됩니다. 계속하는 경우 유효한 URL만 추가됩니다.

      1. **[!UICONTROL Add to list]**&#x200B;을(를) 클릭합니다.

   * 파일에서 URL을 추가하려면 다음 작업을 수행하십시오.

      1. **[!UICONTROL Bulk Add URLs]** > **[!UICONTROL Import File]**&#x200B;을(를) 클릭합니다.

      1. URL이 포함된 로컬 CSV 파일을 끌어다 놓고 각 URL을 별도의 줄에 놓습니다.

         파일에는 열 머리글 행 없이 하나의 데이터 열만 포함되어야 합니다. 기존 목록을 내보내고 행을 편집한 경우 파일을 다시 가져오기 전에 머리글 행과 두 번째 및 세 번째 열을 제거합니다. 계속하면 잘못된 값이 있는 행이 추가되지 않습니다.

      1. **[!UICONTROL Add to list]**&#x200B;을(를) 클릭합니다.

         알림 메시지는 작업이 완료되는 시기를 나타냅니다. 업데이트된 목록을 보려면 페이지를 새로 고침하십시오.

      1. 추가된 URL 수 및 실패한 값 수를 포함하여 작업 상태를 보려면 다음과 같이 하십시오.

         1. 상단 메뉴 모음 오른쪽에 있는 ![작업](/help/dsp/assets/downloads.png)을 클릭합니다.

         1. (행이 추가되지 않은 경우) 실패한 값이 있는 오류 파일을 다운로드하려면 작업 옆에 있는 **[!UICONTROL Download]**&#x200B;을(를) 클릭합니다.

            파일은 브라우저의 다운로드 폴더에 저장됩니다.

   * 특정 URL을 제거하려면 다음 중 하나를 수행하십시오.

      * 제거할 URL을 선택하려면 다음을 수행하십시오.

         1. 목록에서 제거할 각 거래 옆의 확인란을 선택합니다.

         1. **[!UICONTROL Remove from List]**&#x200B;을(를) 클릭합니다.

         1. 확인 메시지에서 **[!UICONTROL Remove]**&#x200B;을(를) 클릭합니다.

      * 제거할 URL을 입력하거나 붙여넣으려면:

         1. **[!UICONTROL Bulk Remove URLs]** > **[!UICONTROL Copy/Paste URLs]**&#x200B;을(를) 클릭합니다.

         1. 각 URL이 별도의 줄에 있는 최대 10,000개의 URL을 입력하거나 붙여 넣습니다.

         1. **[!UICONTROL Validate]**&#x200B;을(를) 클릭하여 URL이 유효하고 현재 목록에 포함되어 있는지 확인합니다.

         1. **[!UICONTROL Remove from list]**&#x200B;을(를) 클릭합니다.

   * 모든 URL을 제거하려면:

      1. **[!UICONTROL Bulk Remove URLs]** > **[!UICONTROL Copy/Paste URLs]**&#x200B;을(를) 클릭합니다.

      1. **[!UICONTROL Remove All URLs]**&#x200B;을(를) 클릭합니다.

      1. **[!UICONTROL Remove]**&#x200B;을(를) 클릭합니다.

## URL 목록 편집

1. 메인 메뉴에서 **[!UICONTROL Resources]** > **[!UICONTROL URL Lists]**&#x200B;을(를) 클릭합니다.

1. 목록 이름을 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * 추가할 URL을 수동으로 입력하거나 붙여넣으려면:

      1. **[!UICONTROL Bulk Add URLs]** > **[!UICONTROL Copy/Paste URLs]**&#x200B;을(를) 클릭합니다.

      1. 각 URL이 별도의 줄에 있는 최대 10,000개의 URL을 입력하거나 붙여 넣습니다.

      1. **[!UICONTROL Validate]**&#x200B;을(를) 클릭하여 URL이 유효한지 확인합니다.

         잘못된 URL이 식별됩니다. 계속하는 경우 유효한 URL만 추가됩니다.

      1. **[!UICONTROL Add to list]**&#x200B;을(를) 클릭합니다.

   * 파일에서 URL을 추가하려면 다음 작업을 수행하십시오.

      1. **[!UICONTROL Bulk Add URLs]** > **[!UICONTROL Import File]**&#x200B;을(를) 클릭합니다.

      1. URL이 포함된 로컬 CSV 파일을 끌어다 놓고 각 URL을 별도의 줄에 놓습니다.

         파일에는 열 머리글 행 없이 하나의 데이터 열만 포함되어야 합니다. 기존 목록을 내보내고 행을 편집한 경우 파일을 다시 가져오기 전에 머리글 행과 두 번째 및 세 번째 열을 제거합니다. 계속하면 잘못된 값이 있는 행이 추가되지 않습니다.

      1. **[!UICONTROL Add to list]**&#x200B;을(를) 클릭합니다.

         알림 메시지는 작업이 완료되는 시기를 나타냅니다.

      1. 추가된 URL 수 및 실패한 값 수를 포함하여 작업 상태를 보려면 다음과 같이 하십시오.

         1. 상단 메뉴 모음 오른쪽에 있는 ![작업](/help/dsp/assets/downloads.png)을 클릭합니다.

         1. (행이 추가되지 않은 경우) 실패한 값이 있는 오류 파일을 다운로드하려면 작업 옆에 있는 **[!UICONTROL Download]**&#x200B;을(를) 클릭합니다.

            파일은 브라우저의 다운로드 폴더에 저장됩니다.

   * 특정 URL을 제거하려면 다음 중 하나를 수행하십시오.

      * 제거할 URL을 선택하려면 다음을 수행하십시오.

         1. 목록에서 제거할 각 거래 옆의 확인란을 선택합니다.

         1. **[!UICONTROL Remove from List]**&#x200B;을(를) 클릭합니다.

         1. 확인 메시지에서 **[!UICONTROL Remove]**&#x200B;을(를) 클릭합니다.

      * 제거할 URL을 입력하거나 붙여넣으려면:

         1. **[!UICONTROL Bulk Remove URLs]** > **[!UICONTROL Copy/Paste URLs]**&#x200B;을(를) 클릭합니다.

         1. 각 URL이 별도의 줄에 있는 최대 10,000개의 URL을 입력하거나 붙여 넣습니다.

         1. **[!UICONTROL Validate]**&#x200B;을(를) 클릭하여 URL이 유효하고 현재 목록에 포함되어 있는지 확인합니다.

         1. **[!UICONTROL Remove from list]**&#x200B;을(를) 클릭합니다.

   * 모든 URL을 제거하려면:

      1. **[!UICONTROL Bulk Remove URLs]** > **[!UICONTROL Copy/Paste URLs]**&#x200B;을(를) 클릭합니다.

      1. **[!UICONTROL Remove All URLs]**&#x200B;을(를) 클릭합니다.

      1. **[!UICONTROL Remove]**&#x200B;을(를) 클릭합니다.

## URL 목록 내보내기

1. 메인 메뉴에서 **[!UICONTROL Resources]** > **[!UICONTROL URL Lists]**&#x200B;을(를) 클릭합니다.

1. 목록 이름을 클릭합니다.

1. ![내보내기](/help/dsp/assets/export.png "내보내기") **[!UICONTROL Export]**&#x200B;를 클릭합니다.

   브라우저의 일반 절차에 따라 파일이 XLSX([!DNL Microsoft Excel] 스프레드시트) 형식으로 다운로드됩니다.

>[!MORELIKETHIS]
>
>* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)
>* [계정 수준 및 광고주 수준의 차단된 사이트 목록 정보](/help/dsp/admin/blocked-sites-list-about.md)
>* [계정 수준 또는 광고주 수준의 차단된 사이트 목록 편집](/help/dsp/admin/blocked-sites-list-edit.md)
