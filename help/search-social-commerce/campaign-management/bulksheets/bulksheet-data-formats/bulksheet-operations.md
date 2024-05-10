---
title: 일괄 시트에서 수행할 수 있는 작업
description: 일괄 시트를 사용하여 캠페인 데이터를 추가, 편집 및 삭제하는 방법에 대한 일반 정보를 참조하십시오.
exl-id: 17ec9307-6dfd-45cb-b8bd-d0d7fcbf2d41
feature: Search Bulksheets
source-git-commit: 67fe8581832dc0762d62908d01672e53cc95b847
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---

# 일괄 시트에서 수행할 수 있는 작업

다음에 대한 일괄 시트를 통해 캠페인 데이터를 추가, 편집 및 삭제할 수 있습니다. [지원되는 광고 네트워크](../bulksheet-about.md#bulksheet-functionality-by-network).

추가, 편집 또는 삭제하려는 각 캠페인 구성 요소(캠페인, 광고 그룹, 키워드 또는 텍스트 광고)나 추가, 편집 또는 삭제하려는 속성에 대해 별도의 데이터 라인을 포함합니다. 예를 들어, 광고 그룹 1개, 키워드 1개, 광고(총 4개 구성 요소)가 있는 캠페인을 만들려면 4개의 개별 데이터 라인이 필요합니다. 을(를) 편집하려면 [!UICONTROL Ad Group Name] 그러나 광고 그룹(하나의 구성 요소)의 경우 한 줄만 있으면 됩니다. 마찬가지로, 하나의 광고 그룹(하나의 구성 요소)에 대해 서로 다른 네 가지 속성을 편집하려면 한 줄만 있으면 됩니다.

다음 규칙은 캠페인 구성 요소 및 해당 속성을 사용하는 작업에 적용됩니다.

* 추가 중:

   * 구성 요소를 추가하려면 해당 구성 요소를 추가하는 데 필요한 모든 필드를 포함하고 선택적으로 구성 요소의 속성에 대한 필드를 포함합니다.

   * 기존 구성 요소에 대한 속성(예: [!UICONTROL Ad Group End Date] 광고 그룹의 경우 해당 구성 요소(광고 그룹)를 편집하는 데 필요한 모든 필드와 속성 필드( )를 포함하십시오.[!UICONTROL Ad Group End Date]).

* 기존 구성 요소의 속성을 편집하려면 해당 구성 요소를 편집하는 데 필요한 모든 필드와 속성 필드를 포함하십시오.

  등록 정보 필드를 비워 두면 기존 값이 유지됩니다.

* 삭제 중:

   * 기존 구성 요소를 삭제하려면 해당 구성 요소를 편집하고 상태를 (으)로 변경하는 데 필요한 모든 필드를 포함하십시오. [!UICONTROL Deleted]. 예를 들어 [!DNL Google Ads] 광고 그룹, 다음을 포함해야 합니다. [!UICONTROL Campaign Name], [!UICONTROL Ad Group Name], [!UICONTROL Ad Group Status] (값: <i>[!UICONTROL Deleted]</i>, 및 [!UICONTROL Ad Group ID].

   * ([!UICONTROL Param1], [!UICONTROL Param2], 및 [!UICONTROL Param3] 값 전용) 기존 항목 삭제 [!DNL paramN] 키워드 값, 키워드를 편집하는 데 필요한 모든 필드를 포함하고 기존 필드도 삭제합니다. [!DNL paramN] 값 입력 `[delete]` (대괄호 포함) 을 입력합니다.

   * (허용된 속성 필드) 구성 요소의 기존 속성 값을 삭제하려면 해당 구성 요소를 편집하는 데 필요한 모든 필드를 포함하고 값을 입력하여 속성 값도 삭제합니다 `[delete]` (대괄호를 포함). 허용되는 필드는 다음과 같습니다.

      * ([!UICONTROL Google Ads] 만) [!UICONTROL Description Line 1], [!UICONTROL Description Line 2]

      * ([!DNL Google Ads] 및 [!DNL Microsoft Advertising] 만) [!UICONTROL Product Scope Filter], [!UICONTROL Base URL/Final URL], [!UICONTROL Tracking Template]

>[!NOTE]
>
>작업에 적용할 수 없는 값을 필드에 포함하면 필드에 입력한 값이 무시됩니다.

>[!MORELIKETHIS]
>
>* [일괄 시트를 사용하여 캠페인 데이터 관리 기본 정보](../bulksheet-about.md)
>* [지원되는 일괄 시트 파일 형식](bulksheet-file-formats.md)
>* [부록 - 일괄 시트 오류](../bulksheet-errors.md)
>* [일괄 시트 파일 다운로드/만들기](../bulksheet-download.md)
