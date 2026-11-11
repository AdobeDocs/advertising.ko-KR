---
title: (새 UI) 포트폴리오의 변경 내역 및 입찰 변경 내역 보기
description: Adobe Advertising 검색, 소셜 및 Commerce에서 포트폴리오 변경 사항 및 입찰 변경 내역을 보고, 날짜 범위를 변경하고, 포트폴리오 변경을 필터링하고, 내역 보고서를 생성, 다운로드 및 삭제하는 방법에 대해 알아봅니다.
feature: Search Portfolios, Search Optimization
hide: true
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: 893a7eac-45bd-56c2-a120-18db6d297dcc
    internal-label: Search Portfolios
  - id: ae57d55f-b168-5358-b114-c3974b1b3d77
    internal-label: Search Optimization
source-git-commit: e7e0221adbb72127a9e6d2354b6a235b233a4a76
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 0%
---
# (새 UI) 포트폴리오의 변경 내역 및 입찰 변경 내역 보기

*Beta 기능*

날짜 범위 동안 포트폴리오에 대한 변경 사항 로그를 볼 수 있습니다. 로그된 작업에는 포트폴리오 생성, 포트폴리오 설정에 대한 모든 변경 사항, 포트폴리오에 할당되거나 포트폴리오에서 할당되지 않은 모든 캠페인, 포트폴리오의 입찰 단위에 적용되거나 제거된 모든 제한, 만료된 포트폴리오의 입찰 단위에 대한 모든 제한 및 포트폴리오에 영향을 주는 기타 작업이 포함됩니다.

[!UICONTROL Change History] 대화 상자에는 포트폴리오 변경에 대한 [!UICONTROL Portfolio Change History] 탭과 입찰 내역에 대한 [!UICONTROL Portfolio Bid Change History] 탭이 있습니다. 기본적으로 두 탭 모두 어제 끝나는 최근 180일을 표시합니다.

범주별로 포트폴리오 변경 사항을 필터링하고 두 탭의 날짜 범위를 변경할 수 있습니다. 데이터를 스프레드시트 파일로 다운로드할 수도 있습니다.

## 포트폴리오의 변경 내역 보기 {#portfolio-change-history}

각 변경 내용에 대한 정보에는 [!UICONTROL Change Date], [!UICONTROL Changed By], [!UICONTROL Change Type] 및 [!UICONTROL Description]이(가) 포함됩니다. 변경 사항은 가장 최근에서 가장 오래된 순으로 나열됩니다.

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Portfolios]**&#x200B;을(를) 클릭합니다.

1. 포트폴리오 행 위에 커서를 놓고 **[!UICONTROL ...]>[!UICONTROL Change History]**&#x200B;을(를) 클릭합니다.

1. [!UICONTROL Change History] 대화 상자에서 **[!UICONTROL Portfolio Change History]** 탭을 봅니다.

1. (선택 사항) 표시되는 정보를 변경합니다.

   * 보고서의 날짜 범위를 변경하려면 ![달력](/help/search-social-commerce/assets/calendar-new.png "달력")을 클릭하십시오.

   * 범주별로 데이터를 필터링하려면 ![필터](/help/search-social-commerce/assets/filter-new.png "필터")를 클릭하십시오. [!UICONTROL All], [!UICONTROL Objective], [!UICONTROL Campaign], [!UICONTROL Target], [!UICONTROL Constraints], [!UICONTROL Optimization Levers] 또는 [!UICONTROL Others].

## 포트폴리오의 입찰 변경 내역 보기 {#portfolio-bid-change-history}

1. [포트폴리오의 변경 기록을 엽니다](#portfolio-change-history).

1. **[!UICONTROL Portfolio Bid Change History]** 탭을 클릭합니다.

1. (선택 사항) 날짜 범위를 변경하려면 ![달력](/help/search-social-commerce/assets/calendar-new.png "달력")을 클릭합니다.

1. (선택 사항) 날짜 열 머리글을 클릭하여 목록을 날짜별로 오름차순 또는 내림차순으로 정렬합니다.

개별 입찰 단위에 대한 내역을 보려면 [포트폴리오의 성과 세부 정보에서 입찰 단위 세부 정보를 여십시오](portfolio-details.md#bid-unit-history). [!UICONTROL Bid Unit ID] 열을 사용할 수 있는 경우 [!UICONTROL Keywords] 보기에서 [입찰 단위 기록을 열 수 있습니다](/help/search-social-commerce/new-ui/manage/keywords/keyword-manage.md#bid-unit-history).

## 포트폴리오 변경 기록에 대한 보고서 관리

포트폴리오 변경 내역에 대한 추가 정보를 [!DNL Microsoft Excel] 통합 문서(XLSX 파일) 형식의 파일로 다운로드할 수 있습니다. 이 보고서에는 숫자 변경 ID, 이전 값과 새 값, 변경 유형(예: &quot;추가됨&quot; 또는 &quot;수정됨&quot;), 작업 유형(예: &quot;예산&quot; 또는 &quot;Portfolio 이름&quot;) 및 적용 가능한 경우 하위 유형, 시간 및 사용자 이름이 포함됩니다.

[!UICONTROL Portfolio Bid Change History] 탭에서 보고서를 생성, 다운로드 및 삭제할 수도 있습니다. 보고서 설정의 제목이 포트폴리오 변경의 경우 [!UICONTROL Portfolio History], 입찰 내역의 경우 [!UICONTROL Portfolio Bid History]입니다.

### 필터링된 데이터 행으로 보고서 생성

1. [포트폴리오의 변경 기록을 열고](#portfolio-change-history) 다운로드하려는 데이터가 있는 탭을 클릭합니다.

1. 오른쪽 상단에서 ![보고서 다운로드](/help/search-social-commerce/assets/download.png "보고서 다운로드")를 클릭합니다.

1. [!UICONTROL Portfolio History] 또는 [!UICONTROL Portfolio Bid History] 설정에서 기본 보고서 이름을 사용하거나 고유한 보고서 이름을 입력한 다음 **[!UICONTROL Generate]**&#x200B;을(를) 클릭합니다.

   기본적으로 보고서 이름에는 기록 유형, 날짜 및 시간이 `YYYYMMDD_HHmm` 형식으로 포함됩니다(예: &quot;portfolioChangeHistory_20260402_1326&quot;). 이름이 이미 있으면 숫자 접미사가 추가됩니다.

   파일이 [!UICONTROL Recently Generated] 목록에 추가됩니다.

1. (선택 사항) 파일이 완료되면 다운로드하려면 파일 이름 옆에 있는 ![다운로드](/help/search-social-commerce/assets/download.png "다운로드")를 클릭합니다.

   브라우저의 일반적인 절차에 따라 파일이 다운로드됩니다.

### 완료된 보고서 다운로드

1. [포트폴리오의 변경 기록을 열고](#portfolio-change-history) 보고서를 생성한 탭을 클릭합니다.

1. 오른쪽 상단에서 ![보고서 다운로드](/help/search-social-commerce/assets/download.png "보고서 다운로드")를 클릭합니다.

1. [!UICONTROL Portfolio History] 또는 [!UICONTROL Portfolio Bid History] 설정의 [!UICONTROL Recently Generated] 목록에서 파일 이름 옆에 있는 ![다운로드](/help/search-social-commerce/assets/download.png "다운로드")를 클릭합니다.

   브라우저의 일반적인 절차에 따라 파일이 다운로드됩니다.

### 완료된 보고서 삭제

1. [포트폴리오의 변경 기록을 열고](#portfolio-change-history) 보고서를 생성한 탭을 클릭합니다.

1. 오른쪽 상단에서 ![보고서 다운로드](/help/search-social-commerce/assets/download.png "보고서 다운로드")를 클릭합니다.

1. [!UICONTROL Portfolio History] 또는 [!UICONTROL Portfolio Bid History] 설정의 [!UICONTROL Recently Generated] 목록에서 파일 이름 옆에 있는 ![삭제](/help/search-social-commerce/assets/delete-new.png "삭제")를 클릭합니다.

>[!MORELIKETHIS]
>
>* [포트폴리오 만들기](portfolio-create.md)
>* [(새 UI) 포트폴리오 편집](portfolio-edit.md)
>* [(새 UI) 포트폴리오 성능 세부 정보 보기](portfolio-details.md)
>* [(새 UI) [!UICONTROL Portfolios] 보기에서 데이터를 다운로드합니다](portfolio-view-report.md)
>* [포트폴리오 정보](portfolio-about.md)
