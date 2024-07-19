---
title: 일괄 시트 오류
description: 각 일괄 시트 오류에 대한 잠재적인 이유를 참조하십시오.
exl-id: dc3559b0-05c0-4896-b9e9-67084f56ab80
feature: Search Bulksheets
source-git-commit: 67fe8581832dc0762d62908d01672e53cc95b847
workflow-type: tm+mt
source-wordcount: '1137'
ht-degree: 0%

---

# 일괄 시트 오류

Search, Social 및 Commerce은 일괄 시트 작업 중에 두 가지 유형의 오류 파일을 생성합니다.

* **SE 오류:** 파일이 게시되었지만 광고 네트워크에서 모든 데이터를 허용하지 않는 경우 `<uploaded file name>_se_errors.<extension used for the bulksheet>` 오류 파일이 만들어집니다. 모든 행이 아닌 일부가 수락되면 오류 파일에 게시되지 않은 행과 각 오류에 대한 설명이 표시되므로 수정할 수 있습니다. 오류는 &quot;[!UICONTROL SE Error Message]&quot; 열에 포함되어 있습니다.

>[!NOTE]
>
>광고 네트워크의 광고 정책을 위반하지만 면제를 받을 수 있는 [!DNL Google Ads] 광고를 게시하는 경우 해당 광고는 자동으로 면제 요청으로 다시 전송됩니다. 면제 요청이 실패하면 위반에 대한 정보가 오류 파일에 포함됩니다.

* **EF 오류:** 일괄 시트 작업에서 파일 또는 파일의 개별 행을 업로드하거나 처리할 수 없는 경우 `<uploaded file name>_ef_errors.<extension used for the bulksheet>`이라는 오류 파일이 만들어집니다. 개별 행에 문제가 있는 경우 해당 행이 포함됩니다.
수정할 수 있도록 각 오류에 대한 설명이 포함되어 있습니다. 오류는 &quot;[!UICONTROL EF Error Message]&quot; 열에 포함되어 있습니다.

## [!UICONTROL SE Error]개 메시지

[!UICONTROL SE Error] 열의 오류는 광고 네트워크에서 직접 발생합니다.

## [!UICONTROL EF Error]개 메시지

다음 오류가 [!UICONTROL EF Errors] 파일의 [!UICONTROL EF Error] 열에 포함될 수 있습니다.

### 오류 다운로드/만들기

| 범주 | 메시지 | 설명 |
|----|----|----|
| 일반 | [!UICONTROL Internal Error: Please Try Creating the bulksheet Again. If Problem Persists Contact Technical Support] | 분류되지 않거나 처리되지 않은 오류로 인해 작업이 완전히 실패했습니다. 문제가 지속되면 Adobe 계정 팀에 문의하여 원인을 확인하십시오. |
| | [!UICONTROL Pre-Sync Failed. Please Try Creating the bulksheet Again. If Problem Persists Contact Technical Support] | 일괄 시트를 만들기 전에 검색, 소셜 및 Commerce이 광고 네트워크와 동기화할 수 없어 일괄 시트가 만들어지지 않았습니다. 문제가 지속되면 Adobe 계정 팀에 문의하십시오. |

### 업로드 오류

| 범주 | 메시지 | 설명 |
|----|----|----|
| 일반 | [!UICONTROL Internal Error: Please Try Uploading the bulksheet Again. If Problem Persists Contact Customer Care] | 작업이 완전히 실패했습니다. 문제가 지속되면 Adobe 계정 팀에 문의하십시오. |
| 모든 엔티티 | [!UICONTROL Invalid Fields.] \[잘못된 필드 및 오류\] | 지정한 데이터가 누락되었거나 잘못되었습니다. |
|  | [!UICONTROL Invalid Reference Given] | 광고 네트워크에 있는 엔티티의 ID 또는 상위 엔티티의 ID(예: 계정 ID)는 Search, Social 및 Commerce의 엔티티에 해당하지 않습니다. 이 문제는 일괄 시트에서 ID를 편집한 경우에 발생할 수 있습니다. |
|  | [!UICONTROL <Entity> is deleted or expired] | 엔티티가 만료되었거나 삭제되었으므로 해당 속성을 변경할 수 없습니다. 누군가 상태를 수동으로 편집한 경우 엔티티가 삭제될 수 있습니다. |
|  | [!UICONTROL <Entity> status should be Active or Paused] | (새 엔티티) 새 엔티티는 &quot;활성&quot; 또는 &quot;일시 중지됨&quot;만 될 수 있습니다. |
|  | [!UICONTROL Duplicate Entries are present] | 각 행에 다른 속성을 가진 동일한 엔티티에 대해 여러 행이 포함됩니다. 변경 사항을 하나의 행으로 통합합니다. |
|  | [!UICONTROL Invalid AMO ID given] | 행에 대한 AMO ID가 존재하지 않습니다. 이 문제는 일괄 시트에서 ID를 편집한 경우 발생할 수 있습니다. |
|  | [!UICONTROL Invalid row given] | 행에 엔티티 유형을 결정하기에 충분한 정보가 포함되지 않습니다. 엔티티 유형에 대한 모든 필수 필드를 포함하도록 행을 편집합니다. |
| 계정 | [!UICONTROL Provide Valid Account Details] | (여러 계정의 일괄 시트) 계정 식별자가 모든 행에 포함되지 않습니다. 각 행에 대해 a) &quot;[!UICONTROL AMO ID]&quot; 또는 b) &quot;[!UICONTROL Account Name]&quot; 및 &quot;[!UICONTROL Platform]&quot; 열 조합 중 하나에 값을 입력하십시오. |
|  | [!UICONTROL Account is disabled. Disabled Accounts cannot be processed] | 검색, 소셜 및 Commerce은 광고 네트워크 계정에 액세스할 수 없으므로 캠페인 데이터를 만들거나 편집할 수 없습니다. 검색 계정에 대한 자격 증명이 올바르고 계정이 활성화되었는지 확인하십시오. |
| 캠페인 | [!UICONTROL Invalid Shopping Country specified] | (쇼핑 캠페인) &quot;[!UICONTROL Sales Country]&quot; 필드의 값이 잘못되었습니다. 유효한 국가 [for [!DNL Google Ads]](https://support.google.com/merchants/answer/160637#countrytable) 및 [for [!DNL Microsoft Advertising]](https://help.ads.microsoft.com/#apex/3/en/51083) 목록을 확인하세요. |
| 모든 캠페인 구성 요소 | [!UICONTROL Campaign creation failed] | 상위 캠페인이 만들어지지 않았으므로 이 엔티티는 만들어지지 않았습니다. 모든 상위 엔티티에 모든 필수 필드가 포함되어 있는지 확인합니다. |
| 광고 그룹 | [!UICONTROL Campaign Row missing] | 지정한 상위 캠페인이 없으므로 광고 그룹이 만들어지지 않았습니다. 새 행에 상위 캠페인을 만듭니다. |
|  | [!UICONTROL New adgroup has both keywords and placement] | 광고 그룹은 키워드 또는 배치 중 하나를 포함할 수 있지만 둘 다 포함할 수는 없습니다. 키워드 및 배치에 대해 별도의 광고 그룹을 만듭니다. |
|  | [!UICONTROL No corresponding keyword for Adgroup] | ([!DNL Yandex]) 광고 그룹에 하나 이상의 키워드가 포함되어 있지 않으므로 광고 그룹을 만들지 못했습니다. |
|  | [!UICONTROL No corresponding creative for Adgroup] | ([!DNL Yandex]) 광고 그룹에 하나 이상의 광고가 포함되어 있지 않으므로 광고 그룹이 만들어지지 않았습니다. |
|  | [!UICONTROL Creative Row Missing] | ([!DNL Yandex]) 광고 그룹에 하나 이상의 광고가 포함되어 있지 않으므로 광고 그룹이 만들어지지 않았습니다. |
| 모든 광고 그룹 구성 요소 | [!UICONTROL Adgroup creation failed] | 상위 광고 그룹을 만들지 못했으므로 이 엔터티를 만들 수 없습니다. 광고 그룹 필드에 오류가 있거나 상위 캠페인이 실패했기 때문일 수 있습니다. 모든 상위 엔티티에 모든 필수 필드가 포함되어 있는지 확인합니다. |
|  | [!UICONTROL Adgroup Row Missing] | 지정한 상위 광고 그룹이 없으므로 엔터티를 만들 수 없습니다. 새 행에 상위 광고 그룹을 만듭니다. |
|  | [!UICONTROL Cannot modify Tracking Template at Keyword / Creative / Site Link level until Account has been migrated to use Upgraded URLs. Please retry after migration] | &quot;[!UICONTROL Tracking Template]&quot; 필드는 최종/고급 URL을 사용하는 계정에만 사용할 수 있습니다. 최종/고급 URL을 사용하도록 계정을 마이그레이션하기 전까지 값을 제거합니다. |
| 광고 | [!UICONTROL Cannot modify attributes other than status code and url for <ad type>] | (텍스트, 확장 텍스트, 제품, 앱 설치 및 동적 검색 이외의 광고 유형) 이 광고 유형의 상태와 URL만 편집할 수 있습니다. |
|  | [!UICONTROL The number of creatives under an AdGroup should not exceed 50] | 각 광고 그룹에는 최대 50개의 광고가 포함될 수 있으며 이 일괄 시트에는 50개 이상의 광고가 포함됩니다. 광고 수를 줄입니다. |
|  | [!UICONTROL Cannot modify an ad which is either deleted/expired or under an deleted/expired campaign] | 광고가 만료되거나 삭제된 상위 엔티티에 있어 편집할 수 없습니다. |
| 키워드 | [!UICONTROL Cannot modify a keyword/website/product which is under deleted Adgroup or Campaign] | 상위 캠페인 또는 광고 그룹이 삭제되거나 만료되었으므로 엔티티를 변경할 수 없습니다. |
| 배치 | [!UICONTROL Cannot modify a keyword/website/product which is under deleted Adgroup or Campaign] | 상위 캠페인 또는 광고 그룹이 삭제되거나 만료되었으므로 엔티티를 변경할 수 없습니다. |
|  | [!UICONTROL Cannot specify placement bids for websites under Display Select enabled Campaign with Search and Display Networks] | (Google 광고) 검색 네트워크의 캠페인에서만 또는 컨텐츠 네트워크에서만 배치(배치)를 입찰할 수 있으며 검색 및 컨텐츠 네트워크를 모두 타깃팅하는 캠페인에서는 입찰할 수 없습니다. |
| 쇼핑 제품 그룹 | [!UICONTROL Cannot delete Everything Else manually. It will be deleted automatically when all Product Group Conditions under the same parent are removed] | 제품 그룹의 각 수준에는 &quot;[!UICONTROL Everything Else]&quot; 그룹이 포함되어야 합니다. &quot;[!UICONTROL Everything Else]&quot; 그룹은 수동으로 삭제할 수 없습니다. 동일한 수준의 다른 모든 제품 그룹을 삭제하면 자동으로 삭제됩니다. |
|  | [!UICONTROL Cannot modify a keyword/website/product which is under deleted Adgroup or Campaign] | 상위 캠페인 또는 광고 그룹이 삭제되거나 만료되었으므로 엔티티를 변경할 수 없습니다. |
| Sitelink | [!UICONTROL Sitelinks Cannot update more than 10 site links per campaign] | ([!DNL Yandex]만 해당) 메시지가 정확하지 않습니다. 각 캠페인에는 최대 4개(10개가 아님) 사이트 링크가 포함될 수 있으며 이 일괄 시트에는 4개 이상이 포함됩니다. 일부 사이트링크를 제거합니다. |
|  | [!UICONTROL Cannot update sitelinks under deleted/expired campaign] | 상위 캠페인이 만료되거나 삭제되었으므로 사이트 링크를 편집할 수 없습니다. |
|  | [!UICONTROL Creative creation failed] | ([!DNL Yandex]) 광고가 만들어지지 않아 사이트 링크를 만들 수 없습니다. |
| 위치 대상 | [!UICONTROL Cannot modify locations under deleted campaigns or adgroups] | 상위 캠페인 또는 광고 그룹이 삭제되거나 만료되었으므로 위치 대상을 편집할 수 없습니다. |
| 제외 | [!UICONTROL Other than status is modified] | 제외 상태(&quot;[!UICONTROL Active]&quot; 또는 &quot;[!UICONTROL Deleted]&quot;)만 편집할 수 있습니다. |
| Google 리마케팅 목록 타겟/대상 | [!UICONTROL Invalid Audience given] | ([!DNL Google Ads] 캠페인만 해당) RLSA 대상이 기존 RLSA(대상자)에 해당하지 않습니다. &quot;[!UICONTROL Audience]&quot; 및 &quot;[!UICONTROL RLSA Target]&quot; 열의 값을 수정하십시오. |

### 게시물 오류

[!UICONTROL EF Errors]개 파일에서만 다음 오류가 발생합니다. 대부분의 게시 오류는 광고 네트워크에서 발생하며 SE 오류 파일에 포함됩니다.

| 범주 | 메시지 | 설명 |
|----|----|----|
| 일반 | [!UICONTROL Internal Error: Please Try Posting the bulksheet Again. If Problem Persists Contact Customer Care] | 작업이 완전히 실패했습니다. 문제가 지속되면 Adobe 계정 팀에 문의하십시오. |
| 모든 엔티티 | [!UICONTROL Entity]이(가) 광고 네트워크에 게시됨 | 엔티티가 광고 네트워크에 게시되었지만 동시에 검색, 소셜 및 Commerce에 동기화되지 않았으므로 엔티티 데이터를 검색, 소셜 및 Commerce에서 즉시 사용할 수 없습니다. 이제 동기화 프로세스가 자동으로 트리거됩니다.<br><br>대량의 데이터가 동기화되면 검색, 소셜 및 Commerce에서 몇 시간 이상 데이터를 사용할 수 없습니다. |
| | [!UICONTROL Skipping <ENTITY> creation since <PARENT ENTITY> creation failed.] | 상위 엔티티를 생성할 수 없으므로 이 하위 엔티티는 생성되지 않았습니다. |

>[!MORELIKETHIS]
>
>* [일괄 시트를 사용하여 캠페인 데이터 관리 정보](bulksheet-about.md)
>* [일괄 시트 파일 다운로드/만들기](bulksheet-download.md)
>* [일괄 시트 파일의 랜딩 페이지 유효성 검사](bulksheet-validate-landing-pages.md)
>* [일괄 시트 파일 또는 수정된 오류 파일 업로드](bulksheet-upload.md)
>* [일괄 시트 또는 수정된 오류 파일 게시](bulksheet-post.md)
