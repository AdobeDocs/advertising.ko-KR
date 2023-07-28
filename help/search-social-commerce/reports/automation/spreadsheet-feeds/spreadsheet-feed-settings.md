---
title: 스프레드시트 보고서 피드 설정
description: 스프레드시트 피드의 설정에 대해 알아봅니다.
exl-id: 9a7e0a21-5db4-4829-a191-cacaa51f6cb6
feature: Search Reports
source-git-commit: 052574217d7ddafb8895c74094da5997b5ff83db
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# 스프레드시트 보고서 피드 설정

| 필드 | 설명 |
|---|---|
| [!UICONTROL Feed Name] | 스프레드시트 피드의 이름입니다. |
| [!UICONTROL Report Template] | 필요한 보고서 데이터를 지정하는 보고서 템플릿입니다. 만드는 데 사용한 보고서 템플릿을 선택합니다. [!DNL Excel] 템플릿. 모든 기본 보고서 템플릿이 나열됩니다.<br><br><b>참고:</b> 보고서에 사용된 보고서 템플릿을 변경하거나 템플릿의 열을 업데이트한 경우 새 템플릿을 만들고 업로드해야 합니다 [!DNL Excel] 템플릿. |
| [!UICONTROL Excel Template] | 특수 형식이 지정된 [!DNL Excel] .XLSX 형식으로 만든 템플릿으로, 보고서 템플릿에 지정된 데이터에 적용됩니다. 전체 경로 및 파일 이름을 입력하거나 을 클릭하여 업로드할 파일을 지정합니다. <b>[!UICONTROL Browse]</b> 장치 또는 네트워크에서 파일을 찾습니다. |
| [!UICONTROL Back Fill From] | 에 대한 기존 데이터의 시작일 [!UICONTROL RAW] 탭이 새로 고쳐지고 과거 일 수로 표시됩니다. 최대 90일의 값을 입력합니다. 기본값은 7일입니다.<br><br>예를 들어 값이 7이고 오늘이 3월 7일인 경우 [!UICONTROL RAW] 3월 1일부터 탭이 새로 고쳐집니다( [!UICONTROL Back Fill Until] 매개 변수)를 참조하십시오. 3월 1일 이전 날짜에 대한 기존 데이터 행은 삭제되지 않지만 새로 고쳐지지 않습니다. |
| [!UICONTROL Back Fill Until] | 에 대한 기존 데이터의 종료 날짜 [!UICONTROL RAW] 탭이 새로 고쳐지고 과거 일 수로 표시됩니다. 기본값은 1일입니다.<br><br>예를 들어 이 값이 1이고 오늘이 3월 7일인 경우 [!UICONTROL RAW] 탭이 3월 6일까지(그리고 에서 지정한 시작 날짜부터) 새로 고쳐집니다. [!UICONTROL Back Fill From] 매개 변수)를 참조하십시오. 이 값이 1이면 [!UICONTROL Back Fill Until] 매개 변수는 7이고 오늘은 3월 7일입니다. 그런 다음 의 기존 데이터를 [!UICONTROL RAW] 3월 1일부터 3월 6일까지 탭이 새로 고쳐졌습니다. 두 예에서 3월 6일 이후 날짜에 대한 기존 데이터 행은 삭제되지 않지만 새로 고쳐지지 않습니다. |
| [!UICONTROL Email Recipients] | 보고서를 새로 고칠 때마다 알림을 보낼 이메일 주소 또는 템플릿에 일정이 포함될 때 보고서를 실행할 때마다 이메일 주소. 기본적으로 사용자 계정의 주소를 입력합니다. 여러 주소를 지정하려면 쉼표, 공백 또는 새 줄로 구분합니다. |
| [!UICONTROL Schedule Time] | 스프레드시트 피드를 새로 고치는 시간: 광고주의 시간대에서 08:00 또는 10:00에서 23:00 사이의 모든 시간. 새 스프레드시트 피드의 기본값은 10:00입니다.<br><br><b>참고:</b> 성능상의 이유로 다른 보고서가 생성된 09:00에는 스프레드시트 피드를 새로 고칠 수 없습니다. |
| [!UICONTROL Email Notification] | (이메일 수신자가 지정된 경우) 지정된 주소에 대한 이메일 알림에 포함할 내용:<ul><li><i>피드 첨부</i> — 완료된 보고서의 사본을 XLSX 형식으로 보냅니다. 파일이 10MB를 초과하는 경우 알림에 첨부 파일이 포함되지 않습니다.</li><li><i>알림만</i> (기본값) - 보고서 완료 또는 실패에 대한 알림만 전송하며 해당 보고서에 대한 링크도 함께 보냅니다.</li></ul> |

>[!MORELIKETHIS]
>
>* [스프레드시트 보고서 피드 정보](spreadsheet-feed-about.md)
>* [스프레드시트 보고서 피드 만들기](spreadsheet-feed-create.md)
>* [만들기 [!DNL Excel] 스프레드시트 보고서 피드용 템플릿](spreadsheet-feed-create-excel-template.md)
>* [스프레드시트 보고서 피드 설정 편집](spreadsheet-feed-edit.md)
>* [스프레드시트 보고서 피드 파일 보기 또는 저장](spreadsheet-feed-view-or-save.md)
>* [스프레드시트 보고서 피드 수동 새로 고침](spreadsheet-feed-refresh.md)
>* [스프레드시트 보고서 피드 삭제](spreadsheet-feed-delete.md)
