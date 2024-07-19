---
title: 스프레드시트 보고서 피드 설정
description: 스프레드시트 피드의 설정에 대해 알아봅니다.
exl-id: 88836c15-81fe-4fe7-8321-2c984b4dcb5d
feature: Search Reports
source-git-commit: e16bc62127a708de8f4deb1eddfa53a14405cbc2
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 0%

---

# 스프레드시트 보고서 피드 설정

| 필드 | 설명 |
|---|---|
| [!UICONTROL Feed Name] | 스프레드시트 피드의 이름입니다. |
| [!UICONTROL Report Template] | 필요한 보고서 데이터를 지정하는 보고서 템플릿입니다. [!DNL Excel] 템플릿을 만드는 데 사용한 보고서 템플릿을 선택하십시오. 모든 기본 보고서 템플릿이 나열됩니다.<br><br><b>참고:</b> 보고서에 사용된 보고서 템플릿을 변경하거나 템플릿의 열을 업데이트한 경우 새 [!DNL Excel] 템플릿을 만들어 업로드해야 합니다. |
| [!UICONTROL Excel Template] | 보고서 템플릿에 지정된 데이터에 적용되는 .XLSX 형식으로 만든 특수 형식의 [!DNL Excel] 템플릿입니다. 전체 경로와 파일 이름을 입력하거나 <b>[!UICONTROL Browse]</b>을(를) 클릭하여 장치 또는 네트워크에서 파일을 찾아 업로드할 파일을 지정하십시오. |
| [!UICONTROL Back Fill From] | [!UICONTROL RAW] 탭의 기존 데이터를 새로 고치는 시작일로, 과거 일 수로 표시됩니다. 최대 90일의 값을 입력합니다. 기본값은 7일입니다.<br><br>예를 들어 값이 7이고 오늘이 3월 7일인 경우 3월 1일부터 [!UICONTROL RAW] 탭의 기존 데이터가 새로 고쳐집니다([!UICONTROL Back Fill Until] 매개 변수로 지정된 종료 날짜까지). 3월 1일 이전 날짜에 대한 기존 데이터 행은 삭제되지 않지만 새로 고쳐지지 않습니다. |
| [!UICONTROL Back Fill Until] | [!UICONTROL RAW] 탭의 기존 데이터를 새로 고치는 종료 날짜입니다. 과거 일 수로 표시됩니다. 기본값은 1일입니다.<br><br>예를 들어 이 값이 1이고 오늘이 3월 7일인 경우 [!UICONTROL RAW] 탭의 기존 데이터가 3월 6일(그리고 [!UICONTROL Back Fill From] 매개 변수에 지정된 시작 날짜부터 시작)까지 새로 고쳐집니다. 이 값이 1이고 [!UICONTROL Back Fill Until] 매개 변수가 7이며 오늘이 3월 7일인 경우 [!UICONTROL RAW] 탭의 기존 데이터가 3월 1일부터 3월 6일까지 새로 고쳐집니다. 두 예에서 3월 6일 이후 날짜에 대한 기존 데이터 행은 삭제되지 않지만 새로 고쳐지지 않습니다. |
| [!UICONTROL Email Recipients] | 보고서를 새로 고칠 때마다 알림을 보낼 이메일 주소 또는 템플릿에 일정이 포함될 때 보고서를 실행할 때마다 이메일 주소. 기본적으로 사용자 계정의 주소를 입력합니다. 여러 주소를 지정하려면 쉼표, 공백 또는 새 줄로 구분합니다. |
| [!UICONTROL Schedule Time] | 스프레드시트 피드를 새로 고치는 시간: 광고주의 시간대에서 08:00 또는 10:00에서 23:00 사이의 모든 시간. 새 스프레드시트 피드의 기본값은 10:00입니다.<br><br><b>참고:</b> 성능상의 이유로 다른 보고서가 생성되는 09:00에 스프레드시트 피드를 새로 고칠 수 없습니다. |
| [!UICONTROL Email Notification] | (이메일 수신자가 지정된 경우) 지정된 주소에 대한 이메일 알림에 포함할 내용:<ul><li><i>피드 첨부</i> — 완료된 보고서의 사본을 XLSX 형식으로 보냅니다. 파일이 10MB를 초과하는 경우 알림에 첨부 파일이 포함되지 않습니다.</li><li><i>알림만</i>(기본값) — 보고서에 대한 링크와 함께 보고서 완료 또는 실패에 대한 알림만 보냅니다.</li></ul> |

>[!MORELIKETHIS]
>
>* [스프레드시트 보고서 피드 정보](spreadsheet-feed-about.md)
>* [스프레드시트 보고서 피드 만들기](spreadsheet-feed-create.md)
>* [스프레드시트 보고서 피드용  [!DNL Excel] 템플릿 만들기](spreadsheet-feed-create-excel-template.md)
>* [스프레드시트 보고서 피드 설정 편집](spreadsheet-feed-edit.md)
>* [스프레드시트 보고서 피드 파일 보기 또는 저장](spreadsheet-feed-view-or-save.md)
>* [스프레드시트 보고서 피드 수동으로 새로 고침](spreadsheet-feed-refresh.md)
>* [스프레드시트 보고서 피드 삭제](spreadsheet-feed-delete.md)
