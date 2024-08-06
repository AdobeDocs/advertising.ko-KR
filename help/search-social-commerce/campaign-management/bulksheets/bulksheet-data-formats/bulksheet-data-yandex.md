---
title: ' [!DNL Yandex] 계정의 필수 일괄 시트 데이터'
description: ' [!DNL Yandex] 계정의 일괄 시트에 있는 필수 머리글 필드 및 데이터 필드를 참조합니다.'
exl-id: bf5a22dd-75c2-486d-85fd-e042bdb87de3
feature: Search Bulksheets
source-git-commit: 5c750153ff9e4be2d02f572d96b171d7aa293dd9
workflow-type: tm+mt
source-wordcount: '1940'
ht-degree: 0%

---

# 부록 - [!DNL Yandex] 계정에 대한 필수 일괄 시트 데이터

[!DNL Yandex] 캠페인 데이터를 일괄적으로 만들고 업데이트하려면 [!DNL Yandex] 계정용으로 특별히 형식이 지정된 검색, 소셜 및 Commerce 일괄 시트 파일을 사용할 수 있습니다. a) [기존 계정에 대한 일괄 시트 파일을 필요한 파일 형식으로 생성](../bulksheet-download.md)하거나, b) 수동으로 만들 수 있습니다(&quot;[지원되는 일괄 시트 파일 형식](bulksheet-file-formats.md)&quot;에서 지원되는 파일 형식에 대한 일반 정보를 참조하십시오).

{{$include /help/_includes/bulksheet-appendices-intro.md}}

<!-- Hiding because this is probably too long a list to be useful.

## Available header fields

Platform,Acct Name,Campaign Name,Campaign Start Date,Campaign Budget,Delivery Method,Ad Group Name,Ad Title,Ad Description,Base URL,Destination URL,SiteLink Title,SiteLink Base URL,SiteLink Destination URL,Keyword,Max CPC,Match Type,Search Network Status,Content Network Status,Negative Keywords (Yandex),Param1 (Yandex),Param2 (Yandex),Campaign Status,Ad Group Status,Ad Status,Keyword Status,SiteLink Status,Campaign ID,Ad Group ID, Ad ID,Keyword ID,AMO ID, [Advertiser-specific Label Classification],Constraints,EF Error Message

{{$include /help/_includes/bulksheet-headers-note.md}}

-->

## 사용 가능한 데이터 필드

{{$include /help/_includes/bulksheet-appendices-intro-required-data.md}}

>[!TIP]
>
>다음 테이블은 넓습니다. 보기 영역을 확장하려면 왼쪽 창 상단의 ![왼쪽 창 숨기기](/help/dsp/assets/hide-left-pane.png "왼쪽 창 숨기기") 및 오른쪽 창 상단의 ![오른쪽 창 숨기기](/help/dsp/assets/hide-right-pane.png "오른쪽 창 숨기기")을 클릭하여 목차와 오른쪽 창을 일시적으로 숨길 수 있습니다. 표 하단에 있는 스크롤 막대를 사용하여 전체 내용을 볼 수도 있습니다.

| 필드 | 캠페인 | 광고 그룹 | 키워드 | 텍스트 광고 | Sitelink | 설명 |
|----|----|-----|-----|----|----|----|
| [!UICONTROL Platform] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함) 광고 플랫폼. 각 행에 엔티티의 AMO ID가 포함되지 않는 한 필수입니다. |
| [!UICONTROL Acct Name] | 필수/선택 사항 | 필수/선택 사항 | 필수/선택 사항 | 필수/선택 사항 | 필수/선택 사항 | (정보 목적으로 생성된 일괄 시트에 포함) 광고 플랫폼. 각 행에 엔티티의 AMO ID가 포함되지 않는 한 필수입니다. |
| [!UICONTROL Campaign Name] | 필수 | 필수 | 필수 | 필수 | 필수 | 계정에 대한 캠페인을 식별하는 고유한 이름. |
| [!UICONTROL Campaign Start Date] | 필수: 만들기<br>선택 사항: 편집 또는 삭제 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 광고주의 시간대 및 m/d/yyyy, m/d/yy, m-d-yyyy 또는 m-d-yy 형식 중 하나에 캠페인에 대해 입찰이 배치될 수 있는 첫 번째 날짜입니다. 새 캠페인의 기본값은 현재 날짜입니다. |
| [!UICONTROL Campaign Budget] | 필수: 만들기<br>선택 사항: 편집 또는 삭제 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 통화 기호 및 구두점 유무에 관계없이 캠페인에 대한 평생 지출 제한. |
| [!UICONTROL Delivery Method] | 필수: 만들기<br>선택 사항: 편집 또는 삭제 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 매일 캠페인에 대한 광고를 표시하는 속도:<ul><li><i>[!UICONTROL Standard (Distributed)]</i>(새 캠페인의 기본값): 광고 노출 횟수를 하루 전체에 분산합니다.</li><li><i>[!UICONTROL Accelerated]:</i> 예산에 도달할 때까지 가능한 한 자주 광고를 표시합니다. 그 결과, 오늘 오후에 광고가 표시되지 않을 수 있습니다.</li></ul> |
| [!UICONTROL Ad Group Name] | 해당 사항 없음 | 필수 | 필수 | 필수 | 해당 사항 없음 | 광고 그룹. |
| [!UICONTROL Ad Title] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수 | 해당 사항 없음 | 배너 헤드라인(광고). 최대 길이는 33자이고, 단어 하나에는 23자를 초과할 수 없습니다.<br><br><b>참고:</b> 광고 복사본을 변경하면 기존 광고가 삭제되고 새 광고가 만들어집니다. |
| [!UICONTROL Ad Description] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수 | 해당 사항 없음 | 배너 본문(광고)입니다. 최대 길이는 75자이고 한 단어는 22자를 초과할 수 없습니다.<br><br><b>참고:</b> 광고 복사본을 변경하면 기존 광고가 삭제되고 새 광고가 만들어집니다. |
| [!UICONTROL Base URL] | 해당 사항 없음 | 해당 사항 없음 | 선택 사항 | 필수 | 해당 사항 없음 | 최종 사용자가 광고를 클릭할 때 고려할 랜딩 페이지 URL(캠페인이나 계정에 대해 구성된 추가 매개 변수 포함). 최대 길이는 프로토콜을 포함하여 1024자입니다.<br><br>키워드 수준의 기본/최종 URL은 광고 수준 이상의 URL을 재정의합니다. |
| [!UICONTROL Destination URL] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함됨, 광고 네트워크에 게시되지 않음) 대상 URL이 있는 계정의 경우 이 값은 광고를 광고주 웹 사이트의 기본 URL/랜딩 페이지에 연결하는 URL입니다(경우에 따라 클릭을 추적한 다음 사용자를 랜딩 페이지로 리디렉션하는 다른 사이트를 통해). 여기에는 Search, Social 및 Commerce 캠페인 또는 계정에 대해 구성된 추가 매개 변수가 포함됩니다. 추적 URL을 생성한 경우 이 값은 계정 설정 및 캠페인 설정의 추적 매개 변수를 기반으로 합니다. 광고 네트워크별 매개 변수를 추가한 경우 검색, 소셜 및 Commerce에 대해 동일한 매개 변수로 대체될 수 있습니다. |
| [!UICONTROL SiteLink Title] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수 | 사이트링크 텍스트입니다. 새 사이트링크의 경우 사이트링크 행 내에 캠페인 이름을 포함합니다. 광고 그룹 수준 또는 광고 수준 사이트 링크의 경우 광고 그룹 이름 또는 광고 제목과 텍스트도 각각 포함합니다.<br><br><b>참고:</b> 최대 4개의 사이트 링크를 사용할 수 있습니다. |
| [!UICONTROL SiteLink Base URL] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수 | 사이트 링크의 기본 URL입니다. 배너의 기본 URL이어야 합니다. &quot;[!UICONTROL Base URL]&quot;을(를) 참조하십시오. |
| [!UICONTROL SiteLink Destination URL] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 사이트 링크의 대상 URL입니다. 배너의 대상 URL이어야 합니다. &quot;[!UICONTROL Destination URL]&quot;을(를) 참조하십시오. |
| [!UICONTROL Keyword] | 선택 사항 / 해당 사항 없음 | 해당 사항 없음 | 필수 | 해당 사항 없음 | 해당 사항 없음 | 구문(키워드 문자열)입니다. 광고에는 하나 이상의 구문이 있어야 합니다. 각 키워드는 정지어를 제외하고 최대 7개의 단어를 사용할 수 있습니다.<br><br><b>메모:</b><ul><li>캠페인 수준에서 구를 제외하려면 [!UICONTROL Match Type]을(를) [!UICONTROL Negative](으)로 설정합니다.</li><li>구를 변경하면 기존 구가 삭제되고 새 구가 만들어집니다.</li><li>[!DNL Yandex] 키워드 구문 또는 일치 유형을 변경하면 기존 키워드 구문이 삭제되고 새 키워드 구문이 만들어집니다.</li></ul> |
| [!UICONTROL Max CPC] | 해당 사항 없음 | 필수: 만들기<br>선택 사항: 편집 또는 삭제 | 선택 사항 | 해당 사항 없음 | 해당 사항 없음 | 금전적 기호와 구두점을 사용하거나 사용하지 않고 검색 네트워크에서 배너(광고) 클릭에 대해 가장 많이 지불하는 금액인 CPC(최대 클릭당 비용)입니다. 광고 그룹 및 키워드에 대한 값을 설정할 수 있습니다. 새 키워드의 기본값은 광고 그룹 수준에서 상속됩니다. |
| [!UICONTROL Match Type] | 선택 사항 / 해당 사항 없음 | 해당 사항 없음 | 선택 사항: 만들기<br>필수/선택 사항: 편집 또는 삭제 | 해당 사항 없음 | 해당 사항 없음 | 구문에 대한 키워드 일치 옵션: <i>[!UICONTROL Content]</i> 또는 <i>[!UICONTROL Search]</i>. &quot;[!UICONTROL Negative Keywords]&quot; 열을 사용하여 부정적인 키워드를 정의합니다.<br><br><b>참고:</b> [!DNL Yandex] 키워드 구문 또는 일치 유형을 변경하면 기존 키워드 구문이 삭제되고 새 키워드 구문이 만들어집니다. |
| [!UICONTROL Search Network Status] | 선택 사항 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 검색 네트워크에 광고를 배치할지 여부: <i>[!UICONTROL Yes]</i>(기본값) 또는 <i>[!UICONTROL No]</i>. |
| 콘텐츠 네트워크 상태 | 선택 사항 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | [!DNL Yandex] 광고(디스플레이) 네트워크에 광고를 배치할지 여부: <i>[!UICONTROL Yes]</i>(기본값) 또는 <i>[!UICONTROL No]</i>. |
| [!UICONTROL Negative Keywords (Yandex)] | 해당 사항 없음 | 해당 사항 없음 | 선택 사항 | 해당 사항 없음 | 해당 사항 없음 | 광고 그룹의 모든 구문에서 공유되고 앞에 빼기 기호가 있는 음수 키워드(구)(예: `-mykeyword`)입니다. 음수 키워드가 구문의 키워드와 일치하는 경우 음수 키워드는 구문에 적용되지 않습니다. |
| [!UICONTROL Param1 (Yandex)] | 해당 사항 없음 | 해당 사항 없음 | 선택 사항 | 해당 사항 없음 | 해당 사항 없음 | `{param1}` 대체 변수의 값입니다. 최대 255바이트를 포함할 수 있습니다. 기존 값을 삭제하려면 값 `[delete]`(대괄호 포함)을 사용하십시오. |
| [!UICONTROL Param2 (Yandex)] | 해당 사항 없음 | 해당 사항 없음 | 선택 사항 | 해당 사항 없음 | 해당 사항 없음 | `{param2}` 대체 변수의 값입니다. 최대 255바이트를 포함할 수 있습니다. 기존 값을 삭제하려면 값 `[delete]`(대괄호 포함)을 사용하십시오. |
| [!UICONTROL Campaign Status] | 선택 사항: 만들기 또는 편집<br>필수: 삭제 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 캠페인의 표시 상태: <i>[!UICONTROL active]</i>, <i>[!UICONTROL archived]</i>, <i>[!UICONTROL deleted]</i>, <i>[!UICONTROL disapproved]</i>, <i>[!UICONTROL pending]</i> 또는 <i>[!UICONTROL stop]</i>(일시 중지됨). 새 캠페인의 기본값은 <i>[!UICONTROL active]</i>입니다.<br><br><b>메모:</b><ul></li>캠페인이 활성화된 적이 있는 경우 삭제할 수 없습니다. 대신 보관하십시오.</li><li>캠페인은 일부 상황에서 자동으로 보관되거나 제거될 수 있습니다.</li><li>수동으로 상태를 <i>[!UICONTROL disapproved]</i> 또는 <i>[!UICONTROL pending]</i>(으)로 설정하거나 해당 상태를 변경할 수 없습니다.</li></ul> |
| [!UICONTROL Ad Group Status] | 해당 사항 없음 | 선택 사항: 만들기 또는 편집<br>필수: 삭제 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 광고 그룹의 표시 상태: <i>[!UICONTROL active]</i>, <i>[!UICONTROL archived]</i>, <i>[!UICONTROL deleted]</i>, <i>[!UICONTROL disapproved]</i>, <i>[!UICONTROL pending]</i> 또는 <i>[!UICONTROL stop]</i>(일시 중지됨). 새 광고 그룹의 기본값은 <i>[!UICONTROL active]</i>입니다.<br><br><b>메모:</b><ul></li>광고 그룹이 활성화된 적이 있는 경우 삭제할 수 없습니다. 대신 보관하십시오.</li><li>수동으로 상태를 <i>[!UICONTROL disapproved]</i> 또는 <i>[!UICONTROL pending]</i>(으)로 설정하거나 해당 상태를 변경할 수 없습니다.</li></ul> |
| [!UICONTROL Ad Status] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 선택 사항: 만들기 또는 편집<br>필수: 삭제 | 해당 사항 없음 | 배너(광고)의 표시 상태: <i>[!UICONTROL active]</i>, <i>[!UICONTROL archived]</i>, <i>[!UICONTROL deleted]</i>, <i>[!UICONTROL disapproved]</i>, <i>[!UICONTROL pending]</i> 또는 <i>[!UICONTROL stop]</i>(일시 중지됨). 새 배너의 기본값은 <i>[!UICONTROL active]</i>입니다.<br><br><b>참고: 수동으로 상태를 <i>[!UICONTROL disapproved]</i> 또는 <i>[!UICONTROL pending]</i>(으)로 설정하거나 해당 상태를 변경할 수 없습니다. |
| [!UICONTROL Keyword Status] | 해당 사항 없음 | 해당 사항 없음 | 선택 사항: 만들기 또는 편집<br>필수: 삭제 | 해당 사항 없음 | 해당 사항 없음 | 구문(키워드)의 표시 상태: <i>[!UICONTROL active]</i>. 새 구문의 기본값은 <i>[!UICONTROL active]</i>입니다.<br><br><b>참고: 수동으로 상태를 <i>[!UICONTROL disapproved]</i> 또는 <i>[!UICONTROL pending]</i>(으)로 설정하거나 해당 상태를 변경할 수 없습니다. |
| [!UICONTROL SiteLink Status] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 선택 사항: 만들기 또는 편집<br>필수: 삭제 | 사이트 링크의 표시 상태: <i>[*UICONTROL Active]</i> 또는 <i>[*UICONTROL Paused]</i>. 새 사이트 링크의 기본값은 <i>[*UICONTROL Active]</i>입니다. |
| [!UICONTROL Campaign ID] | 해당 사항 없음: 만들기<br>필수/선택 사항: 편집<br>선택 사항: 삭제 | 선택 사항 | 선택 사항 | 선택 사항 | 선택 사항 | 기존 캠페인을 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 캠페인에 대한 AMO ID가 포함되어 있지 않은 한 캠페인 이름을 변경할 때만 필요합니다. |
| [!UICONTROL Ad Group ID] | 해당 사항 없음 | 해당 사항 없음: 만들기<br>필수/선택 사항: 편집<br>선택 사항: 삭제 | 선택 사항 | 선택 사항 | 해당 사항 없음 | 기존 광고 그룹을 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 광고 그룹의 AMO ID가 포함되어 있지 않은 한 광고 그룹 이름을 변경할 때만 필요합니다. |
| [!UICONTROL Ad ID] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음: 만들기<br>필수/선택 사항: 편집 또는 삭제 | 해당 사항 없음 | 기존 키워드를 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 a) 키워드를 식별할 수 있는 충분한 속성 열 또는 b) AMO ID가 포함되지 않는 한 키워드 이름을 변경할 때만 필요합니다. |
| [!UICONTROL Keyword ID] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음: 만들기<br>필수/선택 사항: 편집<br>필수: 삭제 | 해당 사항 없음 | 해당 사항 없음 | 기존 키워드를 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 a) 키워드를 식별할 수 있는 충분한 속성 열 또는 b) AMO ID가 포함되지 않는 한 키워드 이름을 변경할 때만 필요합니다. |
| [!UICONTROL AMO ID] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (생성된 일괄 시트에서) 동기화된 엔터티에 대해 [!DNL Adobe]이(가) 생성한 고유 식별자입니다. 반응형 검색 광고의 경우 [!UICONTROL Ad ID]을(를) 포함하지 않으면 광고를 편집하거나 삭제하려면 AMO ID가 필요합니다. AMO ID가 있는 다른 모든 엔티티 유형의 데이터를 편집하려면 엔티티 ID와 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하려면 AMO ID가 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |
| \[광고주별 레이블 분류\] | 선택 사항 | 선택 사항 | 선택 사항 | 선택 사항 | 해당 사항 없음 | (Color라는 레이블 분류의 경우 &quot;Color&quot;와 같이 광고주별 레이블 분류에 대해 이름이 지정됨) 엔티티와 연결된 지정된 분류의 값입니다. 엔티티당 분류당 하나의 값만 포함할 수 있습니다(예: 캠페인 A의 &quot;색상&quot; 레이블 분류의 경우 &quot;빨간색&quot;). 최대 길이는 100자이고 값에는 ASCII 및 비 ASCII 문자가 포함될 수 있습니다.<br><br>레이블 분류와 해당 레이블 값이 모든 하위 구성 요소에 적용됩니다. 나중에 추가되는 새 구성 요소는 자동으로 레이블과 연결됩니다. 제품 그룹에 대한 레이블 분류는 단위(가장 세부적인) 수준에 적용됩니다.<br><br>분류 이름과 분류 값은 대/소문자를 구분하지 않습니다. |
| [!UICONTROL Constraints] | 선택 사항 | 선택 사항 | 선택 사항 | 해당 사항 없음 | 해당 사항 없음 | 엔티티에 할당된 제약 조건입니다. 엔티티당 하나의 제약조건만 지정할 수 있습니다.<br><br>자식 엔터티에 의해 제약 조건이 상속되므로 상속된 값을 재정의하지 않는 한 자식 엔터티의 값을 입력할 필요가 없습니다. |
| [!UICONTROL EF Error Message] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함됨) 검색, 소셜 및 Commerce에서 행의 데이터에 대한 오류 메시지를 표시하는 자리 표시자입니다. 오류 메시지는 [!UICONTROL EF Errors]개 파일에 포함됩니다. 이 값은 광고 네트워크에 게시되지 않습니다. |

[^1]: Excel은 파일을 열 때 큰 숫자를 과학적 표기법(예: 2115585666의 경우 2.12E+09)으로 변환합니다. 표준 표기법에서 숫자를 보려면 열에서 셀을 선택하고 수식 입력줄 내부를 클릭합니다.

>[!MORELIKETHIS]
>
>* [부록 - 일괄 시트 오류](../bulksheet-errors.md)
>* [일괄 시트에서 수행할 수 있는 작업](bulksheet-operations.md)
>* [지원되는 일괄 시트 파일 형식](bulksheet-file-formats.md)
>* [일괄 시트 파일 다운로드/만들기](../bulksheet-download.md)
>*  [!DNL Naver]](/help/search-social-commerce/tracking/formats-click-tracking-naver.md)에 대한 [클릭 추적 형식
>* [일괄 시트 파일 또는 수정된 오류 파일 업로드](../bulksheet-upload.md)
