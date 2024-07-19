---
title: 일괄 시트 파일의 랜딩 페이지 유효성 검사
description: 단일 계정 일괄 시트 파일에서 대상 URL의 유효성을 검사하는 방법을 알아봅니다.
exl-id: 191cb1bc-54a9-4c6c-a29c-f3cbae08e0d8
feature: Search Bulksheets
source-git-commit: e16bc62127a708de8f4deb1eddfa53a14405cbc2
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# 일괄 시트 파일의 랜딩 페이지 유효성 검사

*대상 URL만 있는 계정*

단일 계정 일괄 시트 파일의 모든 대상 URL에서 랜딩 페이지의 유효성을 검사할 수 있습니다. 잘못된 페이지를 나타내는 구문 및 URL을 지정하고 선택적으로 랜딩 페이지 리디렉션을 오류로 보고할 수 있습니다. Search, Social 및 Commerce은 지정된 조건과 누락된 랜딩 페이지가 있는지 확인합니다(HTTP 404 또는 &quot;찾을 수 없음&quot; 오류 발생).

검색, 소셜 및 Commerce은 오류를 발견하면 원래 일괄 시트의 모든 행과 랜딩 페이지가 잘못된 모든 행에 대한 오류 메시지를 포함하는 일괄 시트 오류 파일을 만듭니다. 오류는 [!UICONTROL EF Errors] 열에 기록됩니다. 파일 이름 규칙은 `<bulksheet name>__lpv_errors.<extension used for the bulksheet>`입니다.

나중에 파일을 다운로드하여 오류를 수정하고 수정된 파일을 업로드한 다음 수정된 파일을 광고 네트워크 계정에 게시할 수 있습니다.

>[!NOTE]
>
>* 이 기능은 기본 URL/최종 URL 열의 값을 확인하지 않습니다.
>* 일괄 시트 파일을 검증하는 동안 또는 오류가 발견되더라도 게시할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Bulksheets]**&#x200B;을(를) 클릭합니다.

1. 유효성을 검사할 각 파일 옆에 있는 확인란을 선택합니다.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL Validate URLs]**&#x200B;을(를) 클릭합니다.

1. 대화 상자에서 필드에 정보를 입력한 다음 **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

   랜딩 페이지 본문의 **[!UICONTROL Enter case-sensitive text or phrases that indicate an invalid page(one per line)]:** 텍스트가 잘못되었음을 나타냅니다. 여러 값을 지정하려면 별도의 행에 값을 입력합니다.

   **[!UICONTROL Enter invalid landing pages(one per line):]** 랜딩 페이지로 잘못된 페이지의 URL입니다. 여러 값을 지정하려면 별도의 행에 값을 입력합니다.

   **[!UICONTROL User Agent:]** 랜딩 페이지 유효성 검사 에이전트가 랜딩 페이지가 있는 웹 서버에 대해 식별되는 방법입니다. 기본값은 에이전트에서 보기를 익명 [!DNL Mozilla Firefox] 사용자에게 표시하는 속성입니다. 웹 서버에서 익명 [!DNL Mozilla Firefox] 사용자의 요청을 차단하면 다른 에이전트 이름을 입력하십시오. 예를 들어 [!DNL Googlebot]의 경우 `Googlebot/2.1;+http://www.google.com/bot.html`을(를) 입력합니다.

   **[!UICONTROL Report redirects as errors]:** 랜딩 페이지가 다른 페이지로 리디렉션되는 경우(예: 랜딩 페이지가 누락되고 사이트에 대체 페이지가 표시되는 경우) 랜딩 페이지 오류 파일의 [!UICONTROL ER Errors] 열은 랜딩 페이지가 리디렉션되는 URL을 나타냅니다.

작업이 시작되면 새 행이 [!UICONTROL Bulksheets view]에 추가됩니다. 파일이 생성되면 파일에 대한 링크가 포함된 이메일 알림이 전송됩니다. 컴파일된 데이터의 양에 따라 이메일 알림은 몇 분 이상 걸릴 수 있습니다. 파일을 다운로드하여 편집한 다음 다시 업로드하여 게시할 수 있습니다. 또는 파일을 그대로 게시할 수 있습니다. 그러나 파일 생성에 실패하면 오류 파일이 [!UICONTROL Bulksheet Management] 페이지에 나열되고 오류 파일에 대한 링크와 함께 전자 메일 알림이 전송됩니다.

>[!NOTE]
>
>* 큰 파일의 유효성을 검사하는 데 시간이 더 오래 걸립니다.
>* 여러 캠페인에 대한 일괄 시트 파일에는 최대 50만 개의 데이터 행이 포함될 수 있습니다. 여러 캠페인에 대한 데이터를 생성하고 결합된 데이터가 500,000개 이상의 행으로 구성된 경우, 데이터는 캠페인에 의해 `<bulksheet name>_1.tsv`, `<bulksheet name>_2.tsv` 등의 두 개 이상의 파일로 분할됩니다.

>[!MORELIKETHIS]
>
>* [일괄 시트를 사용하여 캠페인 데이터 관리 정보](bulksheet-about.md)
>* [업로드된 일괄 시트 및 오류 파일 삭제](bulksheet-delete.md)
>* [일괄 시트 또는 수정된 오류 파일 게시](bulksheet-post.md)
>* [일괄 시트 작업 중지 진행 중](bulksheet-stop-job.md)
>* [일괄 시트 또는 수정된 오류 파일 업로드](bulksheet-upload.md)
>* [생성되거나 업로드된 일괄 시트 파일 내보내기](bulksheet-export.md)
