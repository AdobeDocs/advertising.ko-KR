---
title: 일괄 시트를 사용하여 캠페인 데이터 관리 기본 정보
description: 광고 네트워크에서 사용할 수 있는 일괄 시트 기능, 일괄 시트 워크플로우 및 오류 처리에 대해 알아봅니다.
exl-id: 34a16ee3-9eba-4b8b-a5ca-65318f4ee6c5
feature: Search Bulksheets
source-git-commit: d0f1c413134a0868ddec79ded7672af316267edd
workflow-type: tm+mt
source-wordcount: '774'
ht-degree: 0%

---

# 일괄 시트를 사용하여 캠페인 데이터 관리 기본 정보

일괄 시트는 캠페인 데이터를 특정 형식으로 포함하는 파일로, 캠페인 및 광고 그룹 구조 데이터 및 텍스트 광고를 빠르게 만들거나 수정하는 데 사용할 수 있습니다. 하나 이상의 계정, 특정 캠페인 및 광고 그룹 또는 특정 텍스트 광고, 배치 및 제품 그룹에 대한 데이터가 포함된 일괄 시트를 생성(다운로드)할 수 있습니다. 일괄 시트를 사용하여 큰 데이터 세트를 관리하거나 작은 변경 작업을 수행할 수 있습니다. 각 광고 네트워크에는 서로 다른 정보 열이 필요합니다.

원하는 만큼 데이터를 사용하여 일괄 시트를 생성하거나 선택적으로 수동으로 생성하여 업로드할 수 있습니다(&quot;일괄 시트의 필수/포함 데이터&quot; 챕터 참조).

일괄 시트를 만들면 수정해야 하는 끊어진 랜딩 페이지나 추가 또는 편집할 데이터를 식별할 수 있습니다. 그런 다음 파일을 편집하여 검색, 소셜 및 Commerce에 업로드할 수 있으며 관련 광고 네트워크에 즉시 또는 나중에 게시되도록 예약할 수 있습니다. 사용 가능한 일괄 시트를 즉시 또는 나중에 게시할 수도 있습니다.

선택적으로 검색 및 자동 게시를 위해 일괄 시트 파일을 지정된 FTP 계정에 업로드할 수 있습니다. 디렉토리는 매 시간마다 스캔되며 새 파일은 수신되는 순서대로 검색 네트워크에 게시됩니다.

모든 일괄 시트, 랜딩 페이지 유효성 검사 오류 파일 및 기타 오류 파일은 이전에 삭제하지 않는 한 생성된 후 30일 후에 자동으로 삭제됩니다.

## 광고 네트워크별 기능

* **다운로드, 업로드 및 게시:** [!DNL Baidu], [!DNL Google Ads], [!DNL Microsoft Advertising] 및 [!DNL Yandex] 계정

* **다운로드 및 업로드만:** [!DNL Naver] 계정

  [!DNL Naver] 데이터를 Search, Social 및 Commerce 내에서 사용할 수 있도록 업로드할 수 있지만 광고 네트워크에 게시할 수 없습니다. 기존(동기화되지 않은) 데이터를 다운로드할 수도 있습니다.

* **데이터만 다운로드:** [!DNL Pinterest], [!DNL Yahoo Native] 및 [!DNL Yahoo! Display Network] 계정

  기존(동기화되지 않은) 데이터를 다운로드할 수 있습니다.

## 일괄 시트 사용 개요

동기화된 계정에 일괄 시트를 사용하는 의 표준 단계는 다음과 같습니다.

<!-- insert image
  [EDIT/RECREATE FILE to replace "search engine"]
-->

1. [하나 이상의 계정, 캠페인 또는 광고 그룹에 대한 데이터를 일괄 시트 파일로 다운로드](bulksheet-download.md). 선택적으로 광고 네트워크별 일괄 시트를 수동으로 채우고 파일을 업로드할 수 있습니다.

1. 파일의 기본(최종) URL 또는 대상 URL에서 [랜딩 페이지의 유효성 검사](bulksheet-validate-landing-pages.md).

1. 데이터를 추가하거나 수정해야 하는 경우:

   1. [파일을 바탕 화면으로 내보내기](bulksheet-export.md)하고 [!DNL Microsoft Excel]에서 편집합니다.

   1. [편집된 파일을 수동으로 업로드](bulksheet-upload.md)하여 검색, 소셜 및 Commerce을 수행하거나 [파일을 지정된 FTP 계정에 업로드](bulksheet-ftp-account.md)하여 자동으로 게시합니다.

1. (수동으로 업로드한 파일의 경우) [파일을 업로드할 때 또는 나중에 광고 네트워크에 게시](bulksheet-post.md)합니다.

1. (필요한 경우) 새 오류 파일을 다운로드하고 행을 수정한 다음 파일을 다시 게시합니다.

## 캠페인 데이터 업로드 및 게시 오류 관리

검색, 소셜 및 Commerce은 필요할 때 생성하는 추적 URL을 포함하여 캠페인 벌크 시트에서 가능한 한 많은 데이터 행을 업로드하고 게시합니다.

일괄 시트 작업 중에 오류가 발생하면 다음 두 가지 유형의 오류 파일 중 하나가 생성됩니다.

* **[!UICONTROL EF Errors]:** 파일 또는 파일의 개별 행을 업로드하거나 처리할 수 없는 경우 `<uploaded file name>_ef_errors.<extension used for the bulksheet>`이라는 오류 파일이 만들어집니다. 개별 행에 문제가 있는 경우 해당 행을 포함하여 각 오류에 대한 설명을 통해 수정할 수 있습니다.

* **[!UICONTROL SE Errors]:** 파일이 게시되었지만 광고 네트워크에서 일부 또는 모든 데이터를 허용하지 않는 경우 `<uploaded file name>_se_errors.<extension used for the bulksheet>`이라는 오류 파일이 만들어집니다. 모든 행이 아닌 일부가 수락되면 오류 파일에 게시되지 않은 행과 각 오류에 대한 설명이 표시되므로 수정할 수 있습니다. 오류 메시지는 각 행의 마지막 세 열에 표시됩니다.

>[!NOTE]
>
>광고 네트워크의 광고 정책을 위반하지만 면제를 받을 수 있는 [!DNL Google Ads] 광고를 게시하는 경우 해당 광고는 자동으로 면제 요청으로 다시 전송됩니다. 면제 요청이 실패하면 위반에 대한 정보가 오류 파일에 포함됩니다.

두 유형의 오류 파일을 다운로드하고, 행에서 직접 수정한 다음 파일을 다시 업로드하고 게시할 수 있습니다.

오류 파일은 이전에 삭제하지 않으면 30일 후 자동으로 삭제됩니다.

## 각 파일에 대한 정보

다운로드한 모든 데이터 파일, 업로드한 파일 및 오류 파일은 [!UICONTROL Search, Social, & Commerce] > [!UICONTROL Bulksheets]에서 사용할 수 있습니다.

각 파일에 대한 정보에는 현재 작업 상태 및 완료된 작업의 비율, 작업 생성일, 지정된 광고 네트워크에 게시되었거나 게시될 날짜(해당하는 경우), 예약된 삭제 날짜, 작업을 시작한 사용자의 로그인 이름 등이 포함됩니다.

>[!MORELIKETHIS]
>
>* [일괄 시트 파일 다운로드/만들기](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-download.md)
>* [일괄 시트 또는 수정된 오류 파일 업로드](bulksheet-upload.md)
>* [일괄 시트 또는 수정된 오류 파일 게시](bulksheet-post.md)
>* [생성되거나 업로드된 일괄 시트 파일 내보내기](bulksheet-export.md)
