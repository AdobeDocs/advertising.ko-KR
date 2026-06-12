---
title: (새 UI) 스프레드시트 보고서 피드 관리
description: 사용자 지정 형식의 스프레드시트에서 일별 성능 데이터를 제공하는 스프레드시트 보고서 피드를 생성, 구성, 새로 고침, 보기 및 삭제하는 방법에 대해 알아봅니다.
feature: Search Reports
source-git-commit: 38ee8dfbaf82d8f1d212a931956398444e61060f
workflow-type: tm+mt
source-wordcount: '1492'
ht-degree: 0%

---

# (새 UI) 스프레드시트 보고서 피드 관리

*기본 보고서 및 모델 정확도 보고서에만 해당*

<!-- Update link to notifications once available -->

스프레드시트 피드는 [!DNL Microsoft Excel] XLSX의 사용자 지정 스프레드시트 형식으로 모든 기본 보고서 및 모델 정확도 보고서에 대한 일일 성능 데이터를 제공합니다. 일반 보고서 템플릿에서 만드는 특수 형식의 [!DNL Excel] 스프레드시트 템플릿을 사용하여 스프레드시트 피드를 설정할 수 있습니다. 매일 집계되는 새로운 원시 데이터를 사용하여 지정된 시간에 스프레드시트가 자동으로 새로 고쳐집니다. 원시 데이터는 스프레드시트 템플릿에 포함한 모든 열과 그래프를 채웁니다. 스프레드시트 피드 파일을 사용할 수 있거나 파일 생성이 실패하면 보고서 템플릿의 각 이메일 수신자는 사용자가 구성한 [보고서에 대한 알림 설정](/help/search-social-commerce/notifications/notification-about.md)을 기반으로 알림을 받습니다.

피드를 구성하여 최대 90일의 데이터를 새로 고치고 기존의 모든 데이터가 유지되며 계속 누적됩니다.

[!UICONTROL Reports] > [!UICONTROL Spreadsheets Feeds] 보기에는 사용자가 만든 모든 스프레드시트 피드가 나열됩니다. 이 보기에서 스프레드시트 피드를 생성하거나, 피드를 수동으로 새로 고치거나, 피드를 삭제할 수 있습니다.

## 사용 가능한 작업

* [스프레드시트 보고서 피드용  [!DNL Excel] 템플릿 만들기](#spreadsheet-feed-create-excel-template)

* [스프레드시트 보고서 피드 만들기](#spreadsheet-feed-create)

* [스프레드시트 보고서 피드 설정 편집](#spreadsheet-feed-edit)

* [스프레드시트 보고서 피드 파일 보기 또는 저장](#spreadsheet-feed-view-or-save)

* [스프레드시트 보고서 피드 수동 새로 고침](#spreadsheet-feed-refresh)

* [스프레드시트 보고서 피드 삭제](#spreadsheet-feed-delete)

## 스프레드시트 보고서 피드용 [!DNL Excel] 템플릿 만들기 {#spreadsheet-feed-create-excel-template}

<!-- Add x-refs when available -->

스프레드시트 피드를 만들려면 먼저 일반 보고서 템플릿을 사용하여 특수 형식의 [!DNL Microsoft Excel] 스프레드시트 템플릿을 만들어야 합니다. 선택적으로 추가 열 및 그래프를 포함하도록 [!DNL Excel] 스프레드시트를 사용자 지정할 수 있습니다.

1. **[!UICONTROL Reports]>[!UICONTROL Scheduled Reports]**&#x200B;에서 &quot;[!UICONTROL Daily]&quot;의 [!UICONTROL Date Aggregation] 단위와 원하는 다른 모든 데이터 매개 변수를 사용하여 원하는 보고서 유형을 생성하고 보고서를 템플릿으로 저장합니다.

   >[!NOTE]
   >
   > * [!UICONTROL Portfolio], [!UICONTROL Search Engine], [!UICONTROL Search Engine Account], [!UICONTROL Campaign], [!UICONTROL Ad Group], [!UICONTROL Ad Variation], [!UICONTROL Keyword] 및 [!UICONTROL Forecast Accuracy] 보고서에 대한 스프레드시트 피드를 만들 수 있습니다. [!UICONTROL Ad Group Report]을(를) 사용하는 경우 더 빠른 결과를 위해 포함된 광고 그룹의 수를 제한하십시오.
   > * 템플릿에 정의된 [!UICONTROL Date Range] 단위가 사용되지 않습니다. 나중에 스프레드시트 피드를 구성할 때 데이터를 새로 고칠 날짜를 정의합니다.

1. 보고서가 생성되면 **[!UICONTROL Reports]>[!UICONTROL Scheduled Reports]**(으)로 이동하여 보고서 출력의 TSV 또는 XLS 버전을 파일로 내보냅니다.

1. [!DNL Excel]에서 보고서에 대한 사용자 지정 템플릿을 만듭니다.

   1. [!DNL Excel]에서 보고서 파일을 엽니다.

   1. 통합 문서 준비:

      1. 보고서 매개 변수를 표시하는 상위 행을 삭제합니다. XLS 파일의 경우 &quot;[!UICONTROL Total]&quot; 행도 삭제합니다. 선택적으로 일부 데이터 행을 삭제할 수 있지만 a) 원래 순서의 모든 열이 있는 데이터 헤더 행과 b) 하나 이상의 데이터 행을 유지합니다. 수동으로 데이터를 추가하지 마십시오.

         >[!NOTE]
         >
         > 마지막 열에는 0이 아닌 값이 포함되어야 합니다.

      1. 시작 날짜별로 데이터를 오름차순으로 정렬합니다(가장 오래된 항목부터 가장 최근 항목까지).

      1. 워크시트 탭 이름을 &quot;[!UICONTROL Sheet1]&quot;에서 &quot;[!UICONTROL RAW]&quot;(으)로 변경합니다.&quot;

         이 특정 탭 이름을 사용하면 데이터를 새로 고칠 수 있습니다.

      1. (선택 사항) 필요한 경우 보고서 템플릿의 열 오른쪽에 사용자 정의 열을 추가합니다.

   1. (선택 사항) 별도의 워크시트에서 피벗 테이블을 만듭니다. 작업이 완료되면 피벗 테이블의 셀을 마우스 오른쪽 단추로 클릭하고 **[!UICONTROL Pivot Table Options]**&#x200B;을(를) 선택하고 **[!UICONTROL Data]** 탭을 클릭한 다음 **[!UICONTROL Refresh data when opening the file]**&#x200B;을(를) 선택합니다.

   1. 파일을 .XLSX 형식의 [!DNL Excel] 스프레드시트로 저장합니다.

## 스프레드시트 보고서 피드 만들기 {#spreadsheet-feed-create}

1. [보고서 데이터로 채울 [!DNL Excel] 템플릿을 만듭니다](#spreadsheet-feed-create-excel-template).

1. 스프레드시트 피드를 만듭니다.

   1. 메인 메뉴에서 **[!UICONTROL Reports]>[!UICONTROL Spreadsheet Feeds]**&#x200B;을(를) 클릭합니다.

   1. 오른쪽 상단에서 **[!UICONTROL Create Spreadsheet]**&#x200B;을(를) 클릭합니다.

   1. **[!UICONTROL Create Spreadsheet Feed]** 대화 상자에서 [스프레드시트 피드 설정](#spreadsheet-feed-settings)을 지정합니다.

   1. **[!UICONTROL Submit]**&#x200B;을(를) 클릭합니다.

   1. (선택 사항) 피드의 [!UICONTROL Update Status]이(가) *[!UICONTROL Finished]*&#x200B;이면 피드 옆에 있는 **[!UICONTROL XLSX]**&#x200B;을(를) 클릭한 다음 브라우저의 일반 절차에 따라 파일을 열거나 저장합니다.

      >[!NOTE]
      >
      >피드와 연결된 보고서 템플릿이 나중에 삭제되면 피드도 삭제됩니다.

      구성된 [!UICONTROL Schedule Time]에서 매일 스프레드시트 피드가 자동으로 새로 고쳐집니다. 보고서 템플릿에 이메일 수신자의 주소가 포함된 경우 스프레드시트를 새로 고치면 해당 주소에 알림이 전송됩니다.

## 스프레드시트 보고서 피드 설정 편집 {#spreadsheet-feed-edit}

>[!NOTE]
>
> 보고서 템플릿의 열을 편집하거나 새 보고서 템플릿 또는 업데이트된 보고서 템플릿을 사용하는 경우 그에 따라 [!DNL Excel] 템플릿을 업데이트하고 다시 업로드해야 합니다.

1. (선택 사항) 스프레드시트 피드에 사용된 보고서 템플릿 또는 [!DNL Excel] 템플릿을 업데이트하려면 다음을 수행하십시오.

   * (선택 사항) 피드에 대해 다른 보고서 템플릿 또는 업데이트된 보고서 템플릿을 사용하려면 [보고서 템플릿에 대해 새로 만들기 [!DNL Excel] 템플릿을 만듭니다](#spreadsheet-feed-create-excel-template).

     다음 단계에서 보고서 템플릿과 새 [!DNL Excel] 파일을 모두 업로드합니다.

   * (선택 사항) 사용자 지정 열을 [!DNL Excel] 템플릿에 추가하려면 보고서 템플릿의 열 오른쪽에 열을 삽입한 다음 파일을 .XLSX 형식의 [!DNL Excel] 스프레드시트로 저장합니다. 다음 단계에서 새 [!DNL Excel] 파일을 업로드해야 합니다.

1. 메인 메뉴에서 **[!UICONTROL Reports]>[!UICONTROL Spreadsheet Feeds]**&#x200B;을(를) 클릭합니다.

1. 스프레드시트 피드 설정을 변경합니다.

   1. 스프레드시트 피드 이름 옆에 있는 확인란을 선택합니다.

   1. 일괄 작업 도구 모음에서 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

   1. [!UICONTROL Create Spreadsheet Feed]<!-- sic --> 대화 상자에서 [스프레드시트 피드 설정](#spreadsheet-feed-settings)을 변경합니다.

   1. **[!UICONTROL Submit]**&#x200B;을(를) 클릭합니다.

   1. (선택 사항) 피드의 [!UICONTROL Update Status]이(가) *[!UICONTROL Finished]*&#x200B;이면 피드 옆에 있는 **[!UICONTROL XLSX]**&#x200B;을(를) 클릭한 다음 브라우저의 일반 절차에 따라 파일을 열거나 저장합니다.

   >[!NOTE]
   >
   > 피드와 연결된 보고서 템플릿이 나중에 삭제되면 피드도 삭제됩니다.

   스프레드시트 피드는 광고주의 시간대에 매일 08:00에 자동으로 새로 고쳐집니다. 보고서 템플릿에 이메일 수신자의 주소가 포함된 경우 스프레드시트를 새로 고치면 해당 주소에 알림이 전송됩니다.

## 스프레드시트 보고서 피드 설정 {#spreadsheet-feed-settings}

| 필드 | 설명 |
|---|---|
| [!UICONTROL Feed Name] | 스프레드시트 피드의 이름입니다. |
| [!UICONTROL Report Template] | 필요한 보고서 데이터를 지정하는 보고서 템플릿입니다. [!DNL Excel] 템플릿을 만드는 데 사용한 보고서 템플릿을 선택하십시오. 모든 기본 보고서 템플릿이 나열됩니다.<br><br><b>참고:</b> 보고서에 사용되는 보고서 템플릿을 변경하거나 템플릿의 열을 업데이트한 경우 새 [!DNL Excel] 템플릿을 만들고 업로드해야 합니다. |
| [!UICONTROL Excel Template] | 보고서 템플릿에 지정된 데이터에 적용되는 .XLSX 형식으로 만든 특수 형식의 [!DNL Excel] 템플릿입니다. 전체 경로와 파일 이름을 입력하거나 <b>[!UICONTROL Browse]</b>을(를) 클릭하여 장치 또는 네트워크에서 파일을 찾아 업로드할 파일을 지정하십시오. |
| [!UICONTROL Back Fill From] | [!UICONTROL RAW] 탭의 기존 데이터를 새로 고치는 시작일로, 과거 일 수로 표시됩니다. 최대 90일의 값을 입력합니다. 기본값은 7일입니다.<br><br>예를 들어 값이 7이고 오늘이 3월 7일인 경우 3월 1일부터 [!UICONTROL RAW] 탭의 기존 데이터가 새로 고쳐집니다([!UICONTROL Back Fill Until] 매개 변수로 지정된 종료 날짜까지). 3월 1일 이전 날짜에 대한 기존 데이터 행은 삭제되지 않지만 새로 고쳐지지 않습니다. |
| [!UICONTROL Back Fill Until] | [!UICONTROL RAW] 탭의 기존 데이터를 새로 고치는 종료 날짜입니다. 과거 일 수로 표시됩니다. 기본값은 1일입니다.<br><br>예를 들어 이 값이 1이고 오늘이 3월 7일인 경우 [!UICONTROL RAW] 탭의 기존 데이터가 3월 6일(그리고 [!UICONTROL Back Fill From] 매개 변수에 지정된 시작 날짜부터 시작)까지 새로 고쳐집니다. 이 값이 1이고 [!UICONTROL Back Fill Until] 매개 변수가 7이며 오늘이 3월 7일인 경우 [!UICONTROL RAW] 탭의 기존 데이터가 3월 1일부터 3월 6일까지 새로 고쳐집니다. 두 예에서 3월 6일 이후 날짜에 대한 기존 데이터 행은 삭제되지 않지만 새로 고쳐지지 않습니다. |
| [!UICONTROL Email Recipients] | 보고서를 새로 고칠 때마다 알림을 보낼 이메일 주소 또는 템플릿에 일정이 포함될 때 보고서를 실행할 때마다 이메일 주소. 기본적으로 사용자 계정의 주소를 입력합니다. 여러 주소를 지정하려면 쉼표, 공백 또는 새 줄로 구분합니다. |
| [!UICONTROL Schedule Time] | 스프레드시트 피드를 새로 고치는 시간: 08:00에서 또는 광고주의 시간대로 10:00에서 23:00 사이의 모든 시간입니다. 새 스프레드시트 피드의 기본값은 10:00입니다.<br><br><b>참고:</b> 성능상의 이유로 다른 보고서가 생성되면 09:00에 스프레드시트 피드를 새로 고칠 수 없습니다. |
| [!UICONTROL Email Notification] | (이메일 수신자가 지정된 경우) 지정된 주소에 대한 이메일 알림에 포함할 내용:<ul><li><i>[!UICONTROL Attach feed]</i> — 완료된 보고서의 사본을 XLSX 형식으로 보냅니다. 파일이 10MB를 초과하는 경우 알림에 첨부 파일이 포함되지 않습니다.</li><li><i>[!UICONTROL Notification Only]</i>(기본값) — 보고서 완료 또는 실패에 대한 알림만 보내려면 보고서에 대한 링크와 함께 보냅니다.</li></ul> |

## 스프레드시트 보고서 피드 파일 보기 또는 저장 {#spreadsheet-feed-view-or-save}

생성된 스프레드시트 피드를 보거나 파일에 저장할 수 있습니다. 스프레드시트 피드 파일이 [!DNL Microsoft Excel] XLSX 형식입니다.

1. 메인 메뉴에서 **[!UICONTROL Reports]>[!UICONTROL Spreadsheet Feeds]**&#x200B;을(를) 클릭합니다.

1. 피드 옆에 있는 **[!UICONTROL XLSX]**&#x200B;을(를) 클릭한 다음 브라우저의 일반 절차에 따라 파일을 열거나 저장합니다.

## 스프레드시트 보고서 피드 수동 새로 고침 {#spreadsheet-feed-refresh}

>[!NOTE]
>
>스프레드시트 피드는 로컬 시간대에서 매일 08:00에 자동으로 새로 고쳐집니다.

1. 메인 메뉴에서 **[!UICONTROL Reports]>[!UICONTROL Spreadsheet Feeds]**&#x200B;을(를) 클릭합니다.

1. 새로 고침할 각 피드 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Run Spreadsheet]**&#x200B;을(를) 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 피드의 [!UICONTROL Update Status]이(가) *[!UICONTROL Finished]*&#x200B;이면 피드 옆에 있는 **[!UICONTROL XLSX]**&#x200B;을(를) 클릭한 다음 브라우저의 일반 절차에 따라 파일을 열거나 저장합니다.

## 스프레드시트 보고서 피드 삭제 {#spreadsheet-feed-delete}

>[!NOTE]
>
>피드와 연결된 보고서 템플릿이 삭제되면 피드가 자동으로 삭제됩니다.

1. 메인 메뉴에서 **[!UICONTROL Reports]>[!UICONTROL Spreadsheet Feeds]**&#x200B;을(를) 클릭합니다.

1. 삭제할 각 피드 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.
