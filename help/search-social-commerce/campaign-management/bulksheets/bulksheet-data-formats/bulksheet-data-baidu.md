---
title: 다음에 대한 필수 일괄 시트 데이터 [!DNL Baidu] 계정
description: Bulksheets의 필수 헤더 필드 및 데이터 필드 참조 [!DNL Baidu] 계정.
exl-id: 9066f3d5-5de1-4efe-bd61-6c877e106920
feature: Search Bulksheets
source-git-commit: 052574217d7ddafb8895c74094da5997b5ff83db
workflow-type: tm+mt
source-wordcount: '1882'
ht-degree: 0%

---

# 부록 - 필수 일괄 시트 데이터 [!DNL Baidu] 계정

만들고 업데이트하려면 [!DNL Baidu] 캠페인 데이터를 대량으로 볼 경우, 검색, 소셜 및 커머스 일괄 시트 파일을 사용할 수 있습니다. [!DNL Baidu] 계정. 다음 중 하나를 수행할 수 있습니다. [기존 계정에 대한 일괄 시트 파일 생성](../bulksheet-download.md) 필요한 파일 형식에서 또는 b) 수동으로 생성합니다( &quot; 참조).[지원되는 일괄 시트 파일 형식](bulksheet-file-formats.md)지원되는 파일 형식에 대한 일반 정보는 다음을 참조하십시오.

{{$include /help/_includes/bulksheet-appendices-intro.md}}

<!-- Hiding because this is probably too long a list to be useful.

## Available header fields

Platform,Acct Name,Campaign Name,Campaign Budget,Location,Excluded IPs (Baidu), Ad Serving (Baidu),Ad Group Name,Max CPC,Keyword,Match Type,Ad Title,Description Line 1,Description Line 2,Display URL,Base URL,Destination URL,Custom URL Param,Campaign Status,Ad Group Status,Keyword Status,Ad Status,Location Status,[Advertiser-specific Label Classification],Campaign ID,Ad Group ID,Keyword ID,Ad ID,AMO ID,Error Message

{{$include /help/_includes/bulksheet-headers-note.md}}

-->

## 사용 가능한 데이터 필드

{{$include /help/_includes/bulksheet-appendices-intro-required-data.md}}

| 필드 | 캠페인 | 광고 그룹 | 키워드 | 텍스트 광고 | 위치 Target | 설명 |
|----|----|----|----|----|----|----|
| [!UICONTROL Platform] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함) 광고 플랫폼. 각 행에 엔티티의 AMO ID가 포함되지 않는 한 필수입니다. |
| [!UICONTROL Acct Name] | 필수/선택 사항 | R/O | 필수/선택 사항 | 필수/선택 사항 | 필수/선택 사항 | (정보 목적으로 생성된 일괄 시트에 포함) 광고 플랫폼. 각 행에 엔티티의 AMO ID가 포함되지 않는 한 필수입니다. |
| [!UICONTROL Campaign Name] | 필수 | 필수 | 필수 | 필수 | 필수 | 계정에 대한 캠페인을 식별하는 고유한 이름. |
| [!UICONTROL Campaign Budget] | 필수: 만들기<br>선택 사항: 편집 또는 삭제 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 금전적 기호와 구두점을 포함하거나 포함하지 않는 캠페인에 대한 일일 지출 제한. 이 값은 재정의되지만 계정 예산을 초과할 수 없습니다. |
| [!UICONTROL Location] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수 | 캠페인을 위한 광고를 배치할 지리적 위치입니다. 위치를 제외하려면 빼기 기호(`-`). 캠페인에 대한 특정 값을 입력하지 않으면 모든 위치가 타깃팅됩니다. |
| [!UICONTROL Excluded IPs (Baidu)] | 선택 사항입니다 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 광고가 표시되지 않아야 하는 웹 사이트의 IP 주소. 여러 값은 쉼표로 구분하십시오. |
| [!UICONTROL Ad Serving (Baidu)] | 선택 사항입니다 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 광고 그룹 내에서 다른 광고와 관련하여 활성 광고를 게재하는 빈도:<ul><li><i>회전</i> (새 캠페인의 기본값): 각 광고가 거의 동일한 횟수로 광고 경매에 들어가므로, 검색, 소셜 및 상거래를 통해 클릭스루뿐만 아니라 전환에서도 광고에 점수를 매길 수 있습니다.</li><li><i>최적화:</i> 광고 네트워크는 클릭스루율이 높고 품질 점수가 높은 광고가 조합된 광고를 선호합니다. 이러한 광고는 광고 경매에 더 자주 참여하며 시간이 지남에 따라 단일 광고가 선호됩니다. 이 결과는 비즈니스 및 최적화 목표와 일치하지 않을 수 있습니다.</li></ul> |
| [!UICONTROL Ad Group Name] | 해당 사항 없음 | 필수 | 필수 | 필수 | 해당 사항 없음 | 광고 그룹을 식별하는 고유한 이름. |
| [!UICONTROL Max CPC] | 해당 사항 없음 | O | O | 해당 사항 없음 | 해당 사항 없음 | CPC(최대 클릭당 비용)는 금전적 기호 및 구두점 사용 여부에 관계없이 검색 네트워크에서 광고 클릭에 대해 지불하는 가장 높은 금액입니다. 광고 그룹 및 키워드에 대한 값을 설정할 수 있습니다. 새 키워드의 기본값은 광고 그룹 수준에서 상속됩니다. |
| [!UICONTROL Keyword] | 선택 사항 / 해당 사항 없음 | 선택 사항 / 해당 사항 없음 | 필수 | 해당 사항 없음 | 해당 사항 없음 | 키워드 문자열입니다.<br><br>광고 그룹 또는 캠페인 수준에서 키워드를 제외하려면 [!UICONTROL Match Type] 끝 [!UICONTROL Negative]. 행에 광고 그룹 이름이 포함된 경우 광고 그룹에 대한 키워드는 제외됩니다. 행에 광고 그룹 이름이 포함되지 않으면 전체 캠페인에 대해 키워드가 제외됩니다.<br><br><b>참고:</b>Baidu 키워드를 변경하면 기존 키워드가 삭제되고 새 키워드 ID로 새 키워드가 만들어집니다. 하지만 기존 키워드를 삭제하지 않고 일치 유형을 변경할 수 있습니다. |
| [!UICONTROL Match Type] | 선택 사항 / 해당 사항 없음 | 선택 사항 / 해당 사항 없음 | 선택 사항: 만들기<br>필수/선택 사항: 편집 또는 삭제 | 해당 사항 없음 | 해당 사항 없음 | 키워드에 대한 키워드 일치 옵션: <i>[!UICONTROL Broad]</i>, <i>[!UICONTROL Exact]</i>, <i>[!UICONTROL Phrase]</i>, <i>[!UICONTROL Negative Broad]</i>, 또는 <i>[!UICONTROL Negative Exact]</i>. 캠페인 수준 또는 광고 그룹 수준에서 부정적인 키워드를 정의합니다.<br><br>새 키워드의 경우 기본값은 입니다 <i>[!UICONTROL Broad]</i>. 일치 유형 또는 키워드 ID 값은 여러 일치 유형이 있는 키워드를 편집하는 데만 필요합니다.<br><br><b>참고:</b>에 대한 일치 유형을 변경할 수 있습니다. [!DNL Baidu] 기존 키워드를 삭제하지 않은 키워드. |
| [!UICONTROL Ad Title] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수 | 해당 사항 없음 | 광고의 헤드라인입니다. 최대 길이는 14개의 더블바이트 문자 또는 28개의 싱글바이트 문자입니다.<br><br><b>참고:</b> 광고 사본을 변경하면 기존 광고가 삭제되고 동일한 속성으로 새 광고가 만들어집니다. |
| [!UICONTROL Description Line 1] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수 | 해당 사항 없음 | 광고 본문의 첫 번째 줄입니다. 최소 길이는 4개의 더블바이트 문자 또는 8개의 싱글바이트 문자이고, 최대 길이는 20개의 더블바이트 문자 또는 40개의 싱글바이트 문자이다.<br><br><b>참고:</b> 광고 사본을 변경하면 기존 광고가 삭제되고 동일한 속성으로 새 광고가 만들어집니다. |
| [!UICONTROL Description Line 2] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수 | 해당 사항 없음 | 광고 본문의 두 번째 줄입니다. 최소 길이는 4개의 더블바이트 문자 또는 8개의 싱글바이트 문자이고, 최대 길이는 20개의 더블바이트 문자 또는 40개의 싱글바이트 문자이다.<br><br><b>참고:</b> 광고 사본을 변경하면 기존 광고가 삭제되고 동일한 속성으로 새 광고가 만들어집니다. |
| [!UICONTROL Display URL] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수 | 해당 사항 없음 | 광고에 표시되는 URL. 최대 길이는 35개의 1바이트 문자입니다. |
| [!UICONTROL Base URL] | 해당 사항 없음 | 해당 사항 없음 | 선택 사항입니다 | 필수 | 해당 사항 없음 | 최종 사용자가 광고를 클릭할 때 고려할 랜딩 페이지 URL(캠페인이나 계정에 대해 구성된 추가 매개 변수 포함).<br><br>키워드 수준의 기본/최종 URL은 광고 수준 이상의 URL을 무시합니다. |
| [!UICONTROL Destination URL] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함됨, 광고 네트워크에 게시되지 않음) 대상 URL이 있는 계정의 경우 이 값은 광고를 광고주 웹 사이트의 기본 URL/랜딩 페이지에 연결하는 URL입니다(경우에 따라 클릭을 추적한 다음 사용자를 랜딩 페이지로 리디렉션하는 다른 사이트를 통해). 여기에는 검색, 소셜 및 상거래 캠페인 또는 계정에 대해 구성된 추가 매개 변수가 포함됩니다. 추적 URL을 생성한 경우 이 값은 계정 설정 및 캠페인 설정의 추적 매개 변수를 기반으로 합니다. 네트워크별 매개 변수를 추가한 경우 검색, 소셜 및 상거래에 대해 동일한 매개 변수로 대체될 수 있습니다.<br><br>최종 URL이 있는 계정의 경우 이 열에 와 동일한 값이 표시됩니다. [!UICONTROL Base URL/Final URL column]. |
| [!UICONTROL Custom URL Param] | 해당 사항 없음 | 해당 사항 없음 | 선택 사항입니다 | 선택 사항입니다 | 해당 사항 없음 | 대체할 데이터 `{custom_code}` 동적 변수 : 변수가 검색 계정 또는 캠페인 설정에 대한 추적 매개 변수에 포함된 경우 입니다. 추적 URL에 사용자 지정 값을 삽입하려면 다음을 사용하여 일괄 시트 파일을 업로드합니다 [!UICONTROL Generate Tracking URLs] 옵션을 선택합니다. |
| [!UICONTROL Campaign Status] | 선택 사항: 만들기 또는 편집<br>필수: 삭제 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 캠페인의 표시 상태: <i>[!UICONTROL Active]</i>, <i>[!UICONTROL Paused]</i>, 또는 <i>[!UICONTROL Deleted]</i> (기존 캠페인만 해당). 새 캠페인의 기본값은 입니다. <i>[!UICONTROL Active]</i>. 활성 캠페인이나 일시 중지된 캠페인을 삭제하려면 &quot; 값을 입력합니다.[!UICONTROL Deleted]&quot;. |
| [!UICONTROL Ad Group Status] | 해당 사항 없음 | 선택 사항: 만들기 또는 편집<br>필수: 삭제 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 광고 그룹의 표시 상태: <i>[!UICONTROL Active]</i>, <i>[!UICONTROL Paused]</i>, 또는 <i>[!UICONTROL Deleted]</i> (기존 광고 그룹만 해당). 새 광고 그룹의 기본값은 입니다 <i>[!UICONTROL Active]</i>. 활성 또는 일시 중지된 광고 그룹을 삭제하려면 값 &quot;[!UICONTROL Deleted]&quot;. |
| [!UICONTROL Keyword Status] | 해당 사항 없음 | 해당 사항 없음 | 선택 사항: 만들기 또는 편집<br>필수: 삭제 | 해당 사항 없음 | 해당 사항 없음 | 키워드의 표시 상태: <i>[!UICONTROL Active]</i>, <i>[!UICONTROL Deleted]</i> (기존 키워드만), <i>[!UICONTROL Inactive]</i> (편집할 수 없음), <i>[!UICONTROL Paused]</i> (기존 키워드만) 또는 <i>[!UICONTROL Pending]</i>(편집할 수 없음). 새 키워드의 기본값은 입니다 <i>[!UICONTROL Active]</i>.<br><br>키워드를 삭제하려면 값을 입력합니다 <i>[!UICONTROL Deleted]</i>. |
| [!UICONTROL Ad Status] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 선택 사항: 만들기 또는 편집<br>필수: 삭제 | 해당 사항 없음 | 광고의 표시 상태: <i>[!UICONTROL Active]</i>(새 광고의 기본값), <i>[!UICONTROL Deleted]</i> (기존 광고만), <i>[!UICONTROL Disapproved]</i> (편집할 수 없음), <i>[!UICONTROL Inactive]</i> (편집할 수 없음), <i>[!UICONTROL Paused]</i>, 또는 <i>[!UICONTROL Pending (not editable)]</i>.<br><br>광고를 삭제하려면 값을 입력합니다 <i>[!UICONTROL Deleted]</i>. |
| [!UICONTROL Location Status] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 선택 사항: 만들기 또는 편집<br>필수: 삭제 | 위치 대상의 상태: <i>[!UICONTROL Active]</i> 또는 <i>[!UICONTROL Deleted] (기존 위치만 해당) 새 위치의 기본값은 입니다. <i>[!UICONTROL Active]. 활성 위치를 삭제하려면 값을 입력합니다 <i>[!UICONTROL Deleted]. |
| \[광고주별 레이블 분류\] | 선택 사항입니다 | 선택 사항입니다 | 선택 사항입니다 | 선택 사항입니다 | 해당 사항 없음 | (Color라는 레이블 분류의 경우 &quot;Color&quot;와 같이 광고주별 레이블 분류에 대해 이름이 지정됨) 엔티티와 연결된 지정된 분류의 값입니다. 엔티티당 분류당 하나의 값만 포함할 수 있습니다(예: 캠페인 A의 &quot;색상&quot; 레이블 분류의 경우 &quot;빨간색&quot;). 최대 길이는 100자이고 값에는 ASCII 및 비 ASCII 문자가 포함될 수 있습니다.<br><br>레이블 분류 및 해당 레이블 값은 모든 하위 구성 요소에 적용됩니다. 나중에 추가되는 새 구성 요소는 자동으로 레이블과 연결됩니다. <br><br>분류 이름과 분류 값은 대/소문자를 구분하지 않습니다. |
| [!UICONTROL Constraints] | 선택 사항입니다 | 선택 사항입니다 | 선택 사항입니다 | 해당 사항 없음 | 해당 사항 없음 | 엔티티에 할당된 제약 조건입니다. 엔티티당 하나의 제약조건만 지정할 수 있습니다.<br><br>구속은 하위 엔티티에 의해 상속되므로 상속된 값을 재정의하지 않는 한 하위 엔티티에 대한 값을 입력할 필요가 없습니다. |
| [!UICONTROL Campaign ID] | 해당 사항 없음: 만들기<br>필수/선택 사항: 편집 및 삭제 | 선택 사항입니다 | 선택 사항입니다 | 선택 사항입니다 | 해당 사항 없음 | 기존 캠페인을 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 캠페인에 대한 AMO ID가 포함되지 않은 경우 캠페인 이름을 변경할 때만 필요합니다. |
| [!UICONTROL Ad Group ID] | 해당 사항 없음 | 해당 사항 없음: 만들기<br>필수/선택 사항: 편집 및 삭제 | 선택 사항입니다 | 선택 사항입니다 | 해당 사항 없음 | 기존 광고 그룹을 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 광고 그룹에 대한 AMO ID가 포함되지 않은 경우 광고 그룹 이름을 변경할 때만 필요합니다. |
| [!UICONTROL Keyword ID] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음: 만들기<br>필수/선택 사항: 편집 및 삭제 | 해당 사항 없음 | 해당 사항 없음 | 기존 키워드를 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 a) 키워드를 식별할 수 있는 충분한 속성 열 또는 b) AMO ID가 포함되지 않는 한 키워드 이름을 변경할 때만 필요합니다. |
| [!UICONTROL Ad ID] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음: 만들기<br>필수/선택 사항: 편집 및 삭제 | 해당 사항 없음 | 기존 키워드를 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 a) 키워드를 식별할 수 있는 충분한 속성 열 또는 b) AMO ID가 포함되지 않는 한 키워드 이름을 변경할 때만 필요합니다. |
| [!UICONTROL AMO ID] | 해당 사항 없음: 만들기<br>선택 사항: 편집 및 삭제 | 해당 사항 없음: 만들기<br>선택 사항: 편집 및 삭제 | 해당 사항 없음: 만들기<br>선택 사항: 편집 및 삭제 | 해당 사항 없음: 만들기<br>선택 사항: 편집 및 삭제 | 해당 사항 없음: 만들기<br>선택 사항: 편집 및 삭제 | (생성된 일괄 시트에서) [!DNL Adobe]동기화된 엔터티에 대해 생성된 고유 식별자입니다. 반응형 검색 광고의 경우, 다음을 포함하지 않는 한 광고를 편집하거나 삭제하려면 AMO ID가 필요합니다. [!UICONTROL Ad ID]. AMO ID가 있는 다른 모든 엔티티 유형의 데이터를 편집하려면 엔티티 ID와 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하려면 AMO ID가 필요합니다.<br><br>Search, Social 및 Commerce는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |
| [!UICONTROL EF Error Message] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함됨) 행의 데이터에 대해 검색, 소셜 및 상거래의 오류 메시지를 표시하는 자리 표시자입니다. 오류 메시지는에 포함됩니다. [!UICONTROL EF Errors] 파일. 이 값은 광고 네트워크에 게시되지 않습니다. |
| [!UICONTROL SE Error Message] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함됨) 행의 데이터에 대해 광고 네트워크에서 오류 메시지를 표시하는 자리 표시자입니다. 오류 메시지는에 포함됩니다. [!UICONTROL SE Errors] 파일. 이 값은 광고 네트워크에 게시되지 않습니다. |

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
