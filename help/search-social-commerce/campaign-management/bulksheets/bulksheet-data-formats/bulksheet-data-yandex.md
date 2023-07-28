---
title: 다음에 대한 필수 일괄 시트 데이터 [!DNL Yandex] 계정
description: Bulksheets의 필수 헤더 필드 및 데이터 필드 참조 [!DNL Yandex] 계정.
exl-id: c43ea56b-5435-4bbf-8764-beda1bb9b410
feature: Search Bulksheets
source-git-commit: 052574217d7ddafb8895c74094da5997b5ff83db
workflow-type: tm+mt
source-wordcount: '1857'
ht-degree: 1%

---

# 부록 - 필수 일괄 시트 데이터 [!DNL Yandex] 계정

만들고 업데이트하려면 [!DNL Yandex] 캠페인 데이터를 대량으로 볼 경우, 검색, 소셜 및 커머스 일괄 시트 파일을 사용할 수 있습니다. [!DNL Yandex] 계정. 다음 중 하나를 수행할 수 있습니다. [기존 계정에 대한 일괄 시트 파일 생성](../bulksheet-download.md) 필요한 파일 형식에서 또는 b) 수동으로 생성합니다( &quot; 참조).[지원되는 일괄 시트 파일 형식](bulksheet-file-formats.md)지원되는 파일 형식에 대한 일반 정보는 다음을 참조하십시오.

{{$include /help/_includes/bulksheet-appendices-intro.md}}

<!-- Hiding because this is probably too long a list to be useful.

## Available header fields

Platform,Acct Name,Campaign Name,Campaign Start Date,Campaign Budget,Delivery Method,Ad Group Name,Ad Title,Ad Description,Base URL,Destination URL,SiteLink Title,SiteLink Base URL,SiteLink Destination URL,Keyword,Max CPC,Match Type,Search Network Status,Content Network Status,Negative Keywords (Yandex),Param1 (Yandex),Param2 (Yandex),Campaign Status,Ad Group Status,Ad Status,Keyword Status,SiteLink Status,Campaign ID,Ad Group ID, Ad ID,Keyword ID,AMO ID, [Advertiser-specific Label Classification],Constraints,EF Error Message

{{$include /help/_includes/bulksheet-headers-note.md}}

-->

## 사용 가능한 데이터 필드

{{$include /help/_includes/bulksheet-appendices-intro-required-data.md}}

| 필드 | 캠페인 | 광고 그룹 | 키워드 | 텍스트 광고 | Sitelink | 설명 |
|----|----|-----|-----|----|----|----|
| [!UICONTROL Platform] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함) 광고 플랫폼. 각 행에 엔티티의 AMO ID가 포함되지 않는 한 필수입니다. |
| [!UICONTROL Acct Name] | 필수/선택 사항 | 필수/선택 사항 | 필수/선택 사항 | 필수/선택 사항 | 필수/선택 사항 | (정보 목적으로 생성된 일괄 시트에 포함) 광고 플랫폼. 각 행에 엔티티의 AMO ID가 포함되지 않는 한 필수입니다. |
| [!UICONTROL Campaign Name] | 필수 | 필수 | 필수 | 필수 | 필수 | 계정에 대한 캠페인을 식별하는 고유한 이름. |
| [!UICONTROL Campaign Start Date] | 필수: 만들기<br>선택 사항: 편집 또는 삭제 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 광고주의 시간대 및 m/d/yyyy, m/d/yy, m-d-yyyy 또는 m-d-yy 형식 중 하나에 캠페인에 대해 입찰이 배치될 수 있는 첫 번째 날짜입니다. 새 캠페인의 기본값은 현재 날짜입니다. |
| [!UICONTROL Campaign Budget] | 필수: 만들기<br>선택 사항: 편집 또는 삭제 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 통화 기호 및 구두점 유무에 관계없이 캠페인에 대한 평생 지출 제한. |
| [!UICONTROL Delivery Method] | 필수: 만들기<br>선택 사항: 편집 또는 삭제 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 매일 캠페인에 대한 광고를 표시하는 속도:<ul><li><i>[!UICONTROL Standard (Distributed)]</i> (새 캠페인의 기본값): 광고 노출을 하루 전체에 분산합니다.</li><li><i>[!UICONTROL Accelerated]:</i> 예산에 도달할 때까지 가능한 한 자주 광고를 표시합니다. 그 결과, 오늘 오후에 광고가 표시되지 않을 수 있습니다.</li></ul> |
| [!UICONTROL Ad Group Name] | 해당 사항 없음 | 필수 | 필수 | 필수 | 해당 사항 없음 | 광고 그룹. |
| [!UICONTROL Ad Title] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수 | 해당 사항 없음 | 배너 헤드라인(광고). 최대 길이는 33자이고, 단어 하나에는 23자를 초과할 수 없습니다.<br><br><b>참고:</b> 광고 사본을 변경하면 기존 광고가 삭제되고 새 광고가 만들어집니다. |
| [!UICONTROL Ad Description] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수 | 해당 사항 없음 | 배너 본문(광고)입니다. 최대 길이는 75자이고 한 단어는 22자를 초과할 수 없습니다.<br><br><b>참고:</b> 광고 사본을 변경하면 기존 광고가 삭제되고 새 광고가 만들어집니다. |
| [!UICONTROL Base URL] | 해당 사항 없음 | 해당 사항 없음 | 선택 사항입니다 | 필수 | 해당 사항 없음 | 최종 사용자가 광고를 클릭할 때 고려할 랜딩 페이지 URL(캠페인이나 계정에 대해 구성된 추가 매개 변수 포함). 최대 길이는 프로토콜을 포함하여 1024자입니다.<br><br>키워드 수준의 기본/최종 URL은 광고 수준 이상의 URL을 무시합니다. |
| [!UICONTROL Destination URL] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함됨, 광고 네트워크에 게시되지 않음) 대상 URL이 있는 계정의 경우 이 값은 광고를 광고주 웹 사이트의 기본 URL/랜딩 페이지에 연결하는 URL입니다(경우에 따라 클릭을 추적한 다음 사용자를 랜딩 페이지로 리디렉션하는 다른 사이트를 통해). 여기에는 검색, 소셜 및 상거래 캠페인 또는 계정에 대해 구성된 추가 매개 변수가 포함됩니다. 추적 URL을 생성한 경우 이 값은 계정 설정 및 캠페인 설정의 추적 매개 변수를 기반으로 합니다. 네트워크별 매개 변수를 추가한 경우 검색, 소셜 및 상거래에 대해 동일한 매개 변수로 대체될 수 있습니다. |
| [!UICONTROL SiteLink Title] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수 | 사이트링크 텍스트입니다. 새 사이트링크의 경우 사이트링크 행 내에 캠페인 이름을 포함합니다. 광고 그룹 수준 또는 광고 수준 사이트 링크의 경우 광고 그룹 이름 또는 광고 제목과 텍스트도 각각 포함합니다.<br><br><b>참고:</b> 최대 4개의 사이트 링크를 가질 수 있습니다. |
| [!UICONTROL SiteLink Base URL] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수 | 사이트 링크의 기본 URL입니다. 배너의 기본 URL이어야 합니다. 를 참조하십시오.[!UICONTROL Base URL].&quot; |
| [!UICONTROL SiteLink Destination URL] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 사이트 링크의 대상 URL입니다. 배너의 대상 URL이어야 합니다. 를 참조하십시오.[!UICONTROL Destination URL].&quot; |
| [!UICONTROL Keyword] | 선택 사항 / 해당 사항 없음 | 해당 사항 없음 | 필수 | 해당 사항 없음 | 해당 사항 없음 | 구문(키워드 문자열)입니다. 광고에는 하나 이상의 구문이 있어야 합니다. 각 키워드는 정지어를 제외하고 최대 7개의 단어를 사용할 수 있습니다.<br><br><b>참고:</b><ul><li>캠페인 수준에서 구를 제외하려면 다음을 설정하십시오. [!UICONTROL Match Type] 끝 [!UICONTROL Negative].</li><li>구를 변경하면 기존 구가 삭제되고 새 구가 만들어집니다.</li><li>변경 [!DNL Yandex] 키워드 구 또는 일치 유형은 기존 키워드 구를 삭제하고 새 키워드 구를 만듭니다.</li></ul> |
| [!UICONTROL Max CPC] | 해당 사항 없음 | 필수: 만들기<br>선택 사항: 편집 또는 삭제 | 선택 사항입니다 | 해당 사항 없음 | 해당 사항 없음 | 금전적 기호와 구두점을 사용하거나 사용하지 않고 검색 네트워크에서 배너(광고) 클릭에 대해 가장 많이 지불하는 금액인 CPC(최대 클릭당 비용)입니다. 광고 그룹 및 키워드에 대한 값을 설정할 수 있습니다. 새 키워드의 기본값은 광고 그룹 수준에서 상속됩니다. |
| [!UICONTROL Match Type] | 선택 사항 / 해당 사항 없음 | 해당 사항 없음 | 선택 사항: 만들기<br>필수/선택 사항: 편집 또는 삭제 | 해당 사항 없음 | 해당 사항 없음 | 구문에 대한 키워드 일치 옵션: <i>[!UICONTROL Content]</i> 또는 <i>[!UICONTROL Search]</i>. &quot;&quot;를 사용하여 부정적 키워드 정의[!UICONTROL Negative Keywords]&quot;열.<br><br><b>참고:</b> 변경 [!DNL Yandex] 키워드 구 또는 일치 유형은 기존 키워드 구를 삭제하고 새 키워드 구를 만듭니다. |
| [!UICONTROL Search Network Status] | 선택 사항입니다 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 검색 네트워크에 광고를 배치할지 여부: <i>[!UICONTROL Yes]</i> (기본값) 또는 <i>[!UICONTROL No]</i>. |
| 콘텐츠 네트워크 상태 | 선택 사항입니다 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 다음에 광고를 게재할지 여부: [!DNL Yandex] advertising(display) 네트워크: <i>[!UICONTROL Yes]</i> (기본값) 또는 <i>[!UICONTROL No]</i>. |
| [!UICONTROL Negative Keywords (Yandex)] | 해당 사항 없음 | 해당 사항 없음 | 선택 사항입니다 | 해당 사항 없음 | 해당 사항 없음 | 빼기 기호(예: `-mykeyword`). 음수 키워드가 구문의 키워드와 일치하는 경우 음수 키워드는 구문에 적용되지 않습니다. |
| [!UICONTROL Param1 (Yandex)] | 해당 사항 없음 | 해당 사항 없음 | 선택 사항입니다 | 해당 사항 없음 | 해당 사항 없음 | 값 `{param1}` 대체 변수입니다. 최대 255바이트를 포함할 수 있습니다. 기존 값을 삭제하려면 값을 사용합니다 `[delete]` (대괄호를 포함). |
| [!UICONTROL Param2 (Yandex)] | 해당 사항 없음 | 해당 사항 없음 | 선택 사항입니다 | 해당 사항 없음 | 해당 사항 없음 | 값  `{param2}` 대체 변수입니다. 최대 255바이트를 포함할 수 있습니다. 기존 값을 삭제하려면 값을 사용합니다 `[delete]` (대괄호를 포함). |
| [!UICONTROL Campaign Status] | 선택 사항: 만들기 또는 편집<br>필수: 삭제 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 캠페인의 표시 상태: <i>[!UICONTROL active]</i>, <i>[!UICONTROL archived]</i>, <i>[!UICONTROL deleted]</i>, <i>[!UICONTROL disapproved]</i>, <i>[!UICONTROL pending]</i>, 또는 <i>[!UICONTROL stop]</i> (일시 중지됨). 새 캠페인의 기본값은 입니다. <i>[!UICONTROL active]</i>.<br><br><b>참고:</b><ul></li>캠페인이 활성화된 적이 있는 경우 삭제할 수 없습니다. 대신 보관하십시오.</li><li>캠페인은 일부 상황에서 자동으로 보관되거나 제거될 수 있습니다.</li><li>상태를 수동으로 다음으로 설정할 수 없습니다. <i>[!UICONTROL disapproved]</i> 또는 <i>[!UICONTROL pending]</i>, 이러한 상태를 변경하지 마십시오.</li></ul> |
| [!UICONTROL Ad Group Status] | 해당 사항 없음 | 선택 사항: 만들기 또는 편집<br>필수: 삭제 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 광고 그룹의 표시 상태: <i>[!UICONTROL active]</i>, <i>[!UICONTROL archived]</i>, <i>[!UICONTROL deleted]</i>, <i>[!UICONTROL disapproved]</i>, <i>[!UICONTROL pending]</i>, 또는 <i>[!UICONTROL stop]</i> (일시 중지됨). 새 광고 그룹의 기본값은 입니다 <i>[!UICONTROL active]</i>.<br><br><b>참고:</b><ul></li>광고 그룹이 활성화된 적이 있는 경우 삭제할 수 없습니다. 대신 보관하십시오.</li><li>상태를 수동으로 다음으로 설정할 수 없습니다. <i>[!UICONTROL disapproved]</i> 또는 <i>[!UICONTROL pending]</i>, 이러한 상태를 변경하지 마십시오.</li></ul> |
| [!UICONTROL Ad Status] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 선택 사항: 만들기 또는 편집<br>필수: 삭제 | 해당 사항 없음 | 배너(광고)의 표시 상태: <i>[!UICONTROL active]</i>, <i>[!UICONTROL archived]</i>, <i>[!UICONTROL deleted]</i>, <i>[!UICONTROL disapproved]</i>, <i>[!UICONTROL pending]</i>, 또는 <i>[!UICONTROL stop]</i> (일시 중지됨). 새 배너의 기본값은 입니다. <i>[!UICONTROL active]</i>.<br><br><b>참고: 상태를 수동으로 로 설정할 수 없습니다. <i>[!UICONTROL disapproved]</i> 또는 <i>[!UICONTROL pending]</i>, 이러한 상태를 변경하지 마십시오. |
| [!UICONTROL Keyword Status] | 해당 사항 없음 | 해당 사항 없음 | 선택 사항: 만들기 또는 편집<br>필수: 삭제 | 해당 사항 없음 | 해당 사항 없음 | 구(키워드)의 표시 상태: <i>[!UICONTROL active]</i>. 새 구문의 기본값은 입니다. <i>[!UICONTROL active]</i>.<br><br><b>참고: 상태를 수동으로 로 설정할 수 없습니다. <i>[!UICONTROL disapproved]</i> 또는 <i>[!UICONTROL pending]</i>, 이러한 상태를 변경하지 마십시오. |
| [!UICONTROL SiteLink Status] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 선택 사항: 만들기 또는 편집<br>필수: 삭제 | 사이트 링크의 표시 상태: <i>[*UICONTROL 활성]</i> 또는 <i>[*UICONTROL 일시 중단됨]</i>. 새 사이트링크의 기본값은 입니다. <i>[*UICONTROL 활성]</i>. |
| [!UICONTROL Campaign ID] | 해당 사항 없음: 만들기<br>필수/선택 사항: 편집<br>선택 사항: 삭제 | 선택 사항입니다 | 선택 사항입니다 | 선택 사항입니다 | 선택 사항입니다 | 기존 캠페인을 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 캠페인에 대한 AMO ID가 포함되지 않은 경우 캠페인 이름을 변경할 때만 필요합니다. |
| [!UICONTROL Ad Group ID] | 해당 사항 없음 | 해당 사항 없음: 만들기<br>필수/선택 사항: 편집<br>선택 사항: 삭제 | 선택 사항입니다 | 선택 사항입니다 | 해당 사항 없음 | 기존 광고 그룹을 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 광고 그룹에 대한 AMO ID가 포함되지 않은 경우 광고 그룹 이름을 변경할 때만 필요합니다. |
| [!UICONTROL Ad ID] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음: 만들기<br>필수/선택 사항: 편집 또는 삭제 | 해당 사항 없음 | 기존 키워드를 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 a) 키워드를 식별할 수 있는 충분한 속성 열 또는 b) AMO ID가 포함되지 않는 한 키워드 이름을 변경할 때만 필요합니다. |
| [!UICONTROL Keyword ID] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음: 만들기<br>필수/선택 사항: 편집<br>필수: 삭제 | 해당 사항 없음 | 해당 사항 없음 | 기존 키워드를 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 a) 키워드를 식별할 수 있는 충분한 속성 열 또는 b) AMO ID가 포함되지 않는 한 키워드 이름을 변경할 때만 필요합니다. |
| [!UICONTROL AMO ID] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (생성된 일괄 시트에서) [!DNL Adobe]동기화된 엔터티에 대해 생성된 고유 식별자입니다. 반응형 검색 광고의 경우, 다음을 포함하지 않는 한 광고를 편집하거나 삭제하려면 AMO ID가 필요합니다. [!UICONTROL Ad ID]. AMO ID가 있는 다른 모든 엔티티 유형의 데이터를 편집하려면 엔티티 ID와 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하려면 AMO ID가 필요합니다.<br><br>Search, Social 및 Commerce는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |
| \[광고주별 레이블 분류\] | 선택 사항입니다 | 선택 사항입니다 | 선택 사항입니다 | 선택 사항입니다 | 해당 사항 없음 | (Color라는 레이블 분류의 경우 &quot;Color&quot;와 같이 광고주별 레이블 분류에 대해 이름이 지정됨) 엔티티와 연결된 지정된 분류의 값입니다. 엔티티당 분류당 하나의 값만 포함할 수 있습니다(예: 캠페인 A의 &quot;색상&quot; 레이블 분류의 경우 &quot;빨간색&quot;). 최대 길이는 100자이고 값에는 ASCII 및 비 ASCII 문자가 포함될 수 있습니다.<br><br>레이블 분류 및 해당 레이블 값은 모든 하위 구성 요소에 적용됩니다. 나중에 추가되는 새 구성 요소는 자동으로 레이블과 연결됩니다. 제품 그룹에 대한 레이블 분류는 단위(가장 세부적인) 수준에 적용됩니다.<br><br>분류 이름과 분류 값은 대/소문자를 구분하지 않습니다. |
| [!UICONTROL Constraints] | 선택 사항입니다 | 선택 사항입니다 | 선택 사항입니다 | 해당 사항 없음 | 해당 사항 없음 | 엔티티에 할당된 제약 조건입니다. 엔티티당 하나의 제약조건만 지정할 수 있습니다.<br><br>구속은 하위 엔티티에 의해 상속되므로 상속된 값을 재정의하지 않는 한 하위 엔티티에 대한 값을 입력할 필요가 없습니다. |
| [!UICONTROL EF Error Message] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함됨) 행의 데이터에 대해 검색, 소셜 및 상거래의 오류 메시지를 표시하는 자리 표시자입니다. 오류 메시지는에 포함됩니다. [!UICONTROL EF Errors] 파일. 이 값은 광고 네트워크에 게시되지 않습니다. |

<table style="table-layout:auto">

[^1]: Excel은 파일을 열 때 큰 숫자를 과학적 표기법(예: 2.12E+2115585666)으로 변환합니다. 표준 표기법에서 숫자를 보려면 열에서 셀을 선택하고 수식 입력줄 내부를 클릭합니다.

>[!MORELIKETHIS]
>
>* [부록 - 일괄 시트 오류](../bulksheet-errors.md)
>* [일괄 시트에서 수행할 수 있는 작업](bulksheet-operations.md)
>* [지원되는 일괄 시트 파일 형식](bulksheet-file-formats.md)
>* [일괄 시트 파일 다운로드/만들기](../bulksheet-download.md)
>* [클릭 추적 형식 [!DNL Naver]](/help/search-social-commerce/tracking/formats-click-tracking-naver.md)
>* [일괄 시트 파일 또는 수정된 오류 파일 업로드](../bulksheet-upload.md)
