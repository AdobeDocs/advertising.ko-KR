---
title: 다음에 대한 필수 일괄 시트 데이터 [!DNL Naver] 계정
description: Bulksheets의 필수 헤더 필드 및 데이터 필드 참조 [!DNL Naver] 계정.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '991'
ht-degree: 1%

---

# 부록 - 필수 일괄 시트 데이터 [!DNL Naver] 계정

사용자 채우기 [!DNL Naver] 내에서 일괄 시트 파일을 생성하여 검색, 소셜 및 상거래의 계정 [!DNL Naver]을 클릭한 다음 Search, Social 및 Commerce에 업로드합니다.

{{$include /help/_includes/bulksheet-appendices-intro.md}}

<!-- Hiding because this is probably too long a list to be useful.

## Available header fields

Platform,Acct Name,Campaign Name,Ad Group Name,Keyword,Base URL,Destination URL,[Advertiser-specific Label Classification],Constraints,Campaign Status,Ad Group Status,Keyword Status,Campaign ID,Ad Group ID,Keyword ID,AMO ID,Error Message

{{$include /help/_includes/bulksheet-headers-note.md}}

-->

## 사용 가능한 데이터 필드

{{$include /help/_includes/bulksheet-appendices-intro-required-data.md}}

| 필드 | 캠페인 | 광고 그룹 | 키워드 | 설명 |
|----|----|----|----|----|
| [!UICONTROL Platform] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함) 광고 플랫폼. 각 행에 엔티티의 AMO ID가 포함되지 않는 한 필수입니다. |
| [!UICONTROL Acct Name] | 필수/선택 사항 | 필수/선택 사항 | 필수/선택 사항 | 광고 네트워크 계정을 식별하는 고유한 이름. 각 행에 엔티티의 AMO ID가 포함되지 않는 한 필수입니다. |
| [!UICONTROL Campaign Name] | 필수 | 필수 | 필수 | 계정에 대한 캠페인을 식별하는 고유한 이름. |
| [!UICONTROL Ad Group Name] | 해당 사항 없음 | 필수 | 필수 | 광고 그룹을 식별하는 고유한 이름. |
| [!UICONTROL Keyword] | 해당 사항 없음 | 해당 사항 없음 | 필수 | 키워드 문자열입니다. |
| [!UICONTROL Base URL] | 해당 사항 없음 | 해당 사항 없음 | 선택 사항입니다 | 최종 사용자가 광고를 클릭할 때 고려할 랜딩 페이지 URL(캠페인이나 계정에 대해 구성된 추가 매개 변수 포함).<br><br>키워드 수준의 기본/최종 URL은 광고 수준 이상의 URL을 무시합니다. |
| [!UICONTROL Destination URL] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함됨, 광고 네트워크에 게시되지 않음) 대상 URL이 있는 계정의 경우 이 값은 광고를 광고주 웹 사이트의 기본 URL/랜딩 페이지에 연결하는 URL입니다(경우에 따라 클릭을 추적한 다음 사용자를 랜딩 페이지로 리디렉션하는 다른 사이트를 통해). 여기에는 검색, 소셜 및 상거래 캠페인 또는 계정에 대해 구성된 추가 매개 변수가 포함됩니다. 추적 URL을 생성한 경우 이 값은 계정 설정 및 캠페인 설정의 추적 매개 변수를 기반으로 합니다. 네트워크별 매개 변수를 추가한 경우 검색, 소셜 및 상거래에 대해 동일한 매개 변수로 대체될 수 있습니다.<br><br>최종 URL이 있는 계정의 경우 이 열에 와 동일한 값이 표시됩니다. [!UICONTROL Base URL/Final URL column]. |
| \[광고주별 레이블 분류\] | 선택 사항입니다 | 선택 사항입니다 | 선택 사항입니다 | (Color라는 레이블 분류의 경우 &quot;Color&quot;와 같이 광고주별 레이블 분류에 대해 이름이 지정됨) 엔티티와 연결된 지정된 분류의 값입니다. 엔티티당 분류당 하나의 값만 포함할 수 있습니다(예: 캠페인 A의 &quot;색상&quot; 레이블 분류의 경우 &quot;빨간색&quot;). 최대 길이는 100자이고 값에는 ASCII 및 비 ASCII 문자가 포함될 수 있습니다.<br><br>레이블 분류 및 해당 레이블 값은 모든 하위 구성 요소에 적용됩니다. 나중에 추가되는 새 구성 요소는 자동으로 레이블과 연결됩니다. 제품 그룹에 대한 레이블 분류는 단위(가장 세부적인) 수준에 적용됩니다.<br><br>분류 이름과 분류 값은 대/소문자를 구분하지 않습니다. |
| [!UICONTROL Constraints] | 선택 사항입니다 | 선택 사항입니다 | 선택 사항입니다 | 엔티티에 할당된 제약 조건입니다. 엔티티당 하나의 제약조건만 지정할 수 있습니다.<br><br>구속은 하위 엔티티에 의해 상속되므로 상속된 값을 재정의하지 않는 한 하위 엔티티에 대한 값을 입력할 필요가 없습니다. |
| [!UICONTROL Campaign Status] | 선택 사항: 만들기 또는 편집<br>필수: 삭제 | 해당 사항 없음 | 해당 사항 없음 | 캠페인의 표시 상태: *[!UICONTROL Active]</i>, <i>[!UICONTROL Paused]</i>, 또는 <i>[!UICONTROL Deleted]</i> (기존 캠페인만 해당). 새 캠페인의 기본값은 입니다. <i>[!UICONTROL Active]</i>. 활성 캠페인이나 일시 중지된 캠페인을 삭제하려면 &quot; 값을 입력합니다.[!UICONTROL Deleted]&quot;. |
| [!UICONTROL Ad Group Status] | 해당 사항 없음 | 선택 사항: 만들기 또는 편집<br>필수: 삭제 | 해당 사항 없음 | 광고 그룹의 표시 상태: *[!UICONTROL Active]</i>, <i>[!UICONTROL Paused]</i>, 또는 <i>[!UICONTROL Deleted]</i> (기존 광고 그룹만 해당). 새 광고 그룹의 기본값은 입니다 <i>[!UICONTROL Active]</i>. 활성 또는 일시 중지된 광고 그룹을 삭제하려면 값 &quot;[!UICONTROL Deleted]&quot;. |
| [!UICONTROL Keyword Status] | 해당 사항 없음 | 해당 사항 없음 | 선택 사항: 만들기 또는 편집<br>필수: 삭제 | 키워드의 표시 상태: *[!UICONTROL Active]</i>, <i>[!UICONTROL Paused]</i>, 또는 <i>[!UICONTROL Deleted]</i> (기존 키워드만). 새 키워드의 기본값은 입니다 <i>[!UICONTROL Active]</i>. 활성 또는 일시 중지된 키워드를 삭제하려면 값 &quot;[!UICONTROL Deleted]&quot;. |
| [!UICONTROL Campaign ID] | 해당 사항 없음: 만들기<br>필수/선택 사항: 편집 또는 삭제 | 선택 사항입니다 | 선택 사항입니다 | 기존 캠페인을 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 캠페인에 대한 AMO ID가 포함되지 않은 경우 캠페인 이름을 변경할 때만 필요합니다. |
| [!UICONTROL Ad Group ID] | 해당 사항 없음 | 해당 사항 없음: 만들기<br>필수/선택 사항: 편집 또는 삭제 | 선택 사항입니다 | 기존 광고 그룹을 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 광고 그룹에 대한 AMO ID가 포함되지 않은 경우 광고 그룹 이름을 변경할 때만 필요합니다. |
| [!UICONTROL Keyword ID] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음: 만들기<br>필수/선택 사항: 편집<br>필수: 삭제 | 기존 키워드를 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 a) 키워드를 식별할 수 있는 충분한 속성 열 또는 b) AMO ID가 포함되지 않는 한 키워드 이름을 변경할 때만 필요합니다. |
| [!UICONTROL AMO ID] | 해당 사항 없음: 만들기<br>선택 사항: 편집 또는 삭제 | 해당 사항 없음: 만들기<br>선택 사항: 편집 또는 삭제 | 해당 사항 없음: 만들기<br>선택 사항: 편집 또는 삭제 | (생성된 일괄 시트에서) [!DNL Adobe]동기화된 엔터티에 대해 생성된 고유 식별자입니다. 반응형 검색 광고의 경우, 다음을 포함하지 않는 한 광고를 편집하거나 삭제하려면 AMO ID가 필요합니다. [!UICONTROL Ad ID]. AMO ID가 있는 다른 모든 엔티티 유형의 데이터를 편집하려면 엔티티 ID와 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하려면 AMO ID가 필요합니다.<br><br>Search, Social 및 Commerce는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |
| [!UICONTROL EF Error Message] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함됨) 행의 데이터에 대해 검색, 소셜 및 상거래의 오류 메시지를 표시하는 자리 표시자입니다. 오류 메시지는에 포함됩니다. [!UICONTROL EF Errors] 파일. 이 값은 광고 네트워크에 게시되지 않습니다. |
| [!UICONTROL SE Error Message] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함됨) 행의 데이터에 대해 광고 네트워크에서 오류 메시지를 표시하는 자리 표시자입니다. 오류 메시지는에 포함됩니다. [!UICONTROL SE Errors] 파일. 이 값은 광고 네트워크에 게시되지 않습니다. |

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
>* [구현 [!DNL Naver] 추적 전용 계정](/help/search-social-commerce/campaign-management/naver-tracking-only-account-implement.md)

