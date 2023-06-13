---
title: 다음에 대한 일괄 시트 데이터 [!DNL Yahoo! Display Network] 계정
description: 다운로드한 일괄 시트의 헤더 필드 및 데이터 필드 참조 [!DNL Yahoo! Display Network] 계정.
source-git-commit: a59b477a6f8a616851d85bf89b58434d4d56cd83
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---

# 부록 - 다음에 대한 일괄 시트 데이터 [!DNL Yahoo! Display Network] 계정

<!-- 
[Re-add "Required" to title, file name, and TOC if you add the ability to create/edit campaigns using YDN bulksheets. Then will also need to add more text below, like for the other SEs.]
-->

다음에 대한 데이터를 다운로드할 수 있습니다. [!DNL Yahoo! Display Network] 계정은 대량으로 저장되지만 일괄 시트를 광고 네트워크에 업로드하거나 게시할 수 없습니다.

<!-- Hiding because this is probably too long a list to be useful.

## Available header fields

The following example shows data in comma-delimited values. If you're using tab-separated values, then the data looks different.

Platform,Acct Name,Campaign Name,Ad Group Name,Ad Name, Ad Title,Description Line 1,Description Line 2,Base URL/Final URL,Destination URL,[Advertiser-specific Label Classification],Bid Rules,Constraints,Campaign Status,Ad Group Status,Ad Status,Campaign ID,Ad Group ID,Ad ID,AMO ID,EF Error Message

-->

## 사용 가능한 데이터 필드

| 필드 | 캠페인 | 광고 그룹 | 광고 | 설명 |
|----|----|----|----|----|
| [!UICONTROL Platform] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함) 광고 플랫폼. |
| [!UICONTROL Acct  Name] | 포함된 경우 | 포함된 경우 | 포함된 경우 | 광고 네트워크 계정을 식별하는 고유한 이름. |
| [!UICONTROL Campaign Name] | 포함된 경우 | 포함된 경우 | 포함된 경우 | 계정에 대한 캠페인을 식별하는 고유한 이름. |
| [!UICONTROL Ad Group Name] | 해당 사항 없음 | 포함된 경우 | 포함된 경우 | 광고 그룹을 식별하는 고유한 이름. |
| [!UICONTROL Ad Name] | 해당 사항 없음 | 해당 사항 없음 | 포함된 경우 | 광고 그룹 내에서 광고를 식별하는 고유한 이름. 최대 길이는 50자입니다. |
| [!UICONTROL Ad Title] | 해당 사항 없음 | 해당 사항 없음 | 포함된 경우 | 광고의 헤드라인입니다. |
| [!UICONTROL Description Line 1] | 해당 사항 없음 | 해당 사항 없음 | 포함된 경우 | 광고 본문의 첫 번째 줄입니다. |
| [!UICONTROL Description Line 2] | 해당 사항 없음 | 해당 사항 없음 | 포함된 경우 | 광고 본문의 두 번째 줄입니다. |
| [!UICONTROL Base URL/Final URL] | 해당 사항 없음 | 해당 사항 없음 | 포함된 경우 | 최종 사용자가 광고를 클릭할 때 고려할 랜딩 페이지 URL(캠페인이나 계정에 대해 구성된 추가 매개 변수 포함). 키워드 수준의 기본/최종 URL은 광고 수준 이상의 URL을 무시합니다. |
| [!UICONTROL Destination URL] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함됨, 광고 네트워크에 게시되지 않음) 대상 URL이 있는 계정의 경우 이 값은 광고를 광고주 웹 사이트의 기본 URL/랜딩 페이지에 연결하는 URL입니다(경우에 따라 클릭을 추적한 다음 사용자를 랜딩 페이지로 리디렉션하는 다른 사이트를 통해). 여기에는 검색, 소셜 및 상거래 캠페인 또는 계정에 대해 구성된 추가 매개 변수가 포함됩니다. 추적 URL을 생성한 경우 이 값은 계정 설정 및 캠페인 설정의 추적 매개 변수를 기반으로 합니다. 광고 네트워크별 매개 변수를 추가한 경우 검색, 소셜 및 상거래에 대해 동일한 매개 변수로 대체될 수 있습니다. |
| \[광고주별 레이블 분류\] | 포함된 경우 | 포함된 경우 | 포함된 경우 | (Color라는 레이블 분류의 경우 &quot;Color&quot;와 같이 광고주별 레이블 분류에 대해 이름이 지정됨) 엔티티와 연결된 지정된 분류의 값입니다. |
| [!UICONTROL Constraints] | 포함된 경우 | 포함된 경우 | 해당 사항 없음 | 엔티티에 할당된 제약 조건입니다. |
| [!UICONTROL Campaign Status] | 포함된 경우 | 해당 사항 없음 | 해당 사항 없음 | 캠페인의 표시 상태: <i>[!UICONTROL Active]</i>, <i>[!UICONTROL Paused]</i>, 또는 <i>[!UICONTROL Deleted]</i>. |
| [!UICONTROL Ad Group Status] | 해당 사항 없음 | 포함된 경우 | 해당 사항 없음 | 광고 그룹의 표시 상태: <i>[!UICONTROL Active]</i>, <i>[!UICONTROL Paused]</i>, 또는 <i>[!UICONTROL Deleted]</i>. |
| [!UICONTROL Keyword Status] | 해당 사항 없음 | 해당 사항 없음 | 포함된 경우 | 키워드의 표시 상태: <i>[!UICONTROL Active]</i>, <i>[!UICONTROL Paused]</i>, 또는 <i>[!UICONTROL Deleted]</i> (기존 키워드만). |
| [!UICONTROL Campaign ID] | 포함된 경우 | 포함된 경우 | 포함된 경우 | 기존 캠페인을 식별하는 고유 ID입니다. |
| [!UICONTROL Ad Group ID] | 해당 사항 없음 | 포함된 경우 | 포함된 경우 | 기존 광고 그룹을 식별하는 고유 ID입니다. |
| [!UICONTROL Keyword ID] | 해당 사항 없음 | 해당 사항 없음 | 포함된 경우 | 기존 키워드를 식별하는 고유 ID입니다. |
| [!UICONTROL AMO ID] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (생성된 일괄 시트에서) 동기화된 엔티티에 대해 Adobe이 생성한 고유 식별자입니다. |
| [!UICONTROL EF Error Message] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함됨) 행의 데이터에 대해 검색, 소셜 및 상거래의 오류 메시지를 표시하는 자리 표시자입니다. 오류 메시지는에 포함됩니다. [!UICONTROL EF Errors] 파일. |

<table style="table-layout:auto">

>[!MORELIKETHIS]
>
>* [일괄 시트 파일 다운로드/만들기](../bulksheet-download.md)
