---
title: (새 UI) 포트폴리오의 변경 내역 보기
description: 포트폴리오의 변경 기록을 보는 방법에 대해 알아봅니다.
feature: Search Portfolios, Search Optimization
hide: true
source-git-commit: 84eb5f060a696e057f706c0066c18c9afc1511e1
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---

# (새 UI) 포트폴리오의 변경 내역 보기

*Beta 기능*

날짜 범위 동안 포트폴리오에 대한 변경 사항 로그를 볼 수 있습니다. 로그된 작업에는 포트폴리오 생성, 포트폴리오 설정에 대한 모든 변경 사항, 포트폴리오에 할당되거나 포트폴리오에서 할당되지 않은 모든 캠페인, 포트폴리오의 입찰 단위에 적용되거나 제거된 모든 제한, 만료된 포트폴리오의 입찰 단위에 대한 모든 제한 및 포트폴리오에 영향을 주는 기타 작업이 포함됩니다

<!-- Not available as of 5-14: and by the user who performed the action --> 범주별로 데이터를 필터링할 수 있습니다. 날짜별로 목록을 오름차순 또는 내림차순으로 정렬할 수도 있습니다.

데이터를 스프레드시트 파일로 다운로드할 수도 있습니다.

## (새 UI) 포트폴리오의 변경 내역 보기 {#portfolio-change-history}

각 변경 사항에 대한 정보에는 날짜, 변경한 사람의 사용자 이름, 변경 유형 및 변경된 값이 포함됩니다.

1. 메인 메뉴에서 **[!UICONTROL Goals]>[!UICONTROL Conversions]**&#x200B;을(를) 클릭합니다.

1. 포트폴리오 행 위에 커서를 놓고 **[!UICONTROL ...]>[!UICONTROL Change History]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 표시되는 정보를 변경합니다.

   * 보고서의 날짜 범위를 변경하려면 ![달력](/help/search-social-commerce/assets/calendar-new.png "달력")을 클릭하십시오.

   * 변경 유형별로 데이터를 필터링하려면 ![필터](/help/search-social-commerce/assets/filter-new.png "필터")를 클릭하십시오.<!-- Not available as of 5-14: and by the user who performed the action -->.

   * 날짜별로 목록을 오름차순 또는 내림차순으로 정렬하려면 ![정렬](/help/search-social-commerce/assets/sort.png "정렬")을 클릭하세요.

## 변경 이력에 대한 성능 데이터 보고서 관리

포트폴리오 변경 내역에 대한 추가 정보를 [!DNL Microsoft Excel] 통합 문서(XLSX 파일) 형식의 파일로 다운로드할 수 있습니다. 이 보고서에는 숫자 변경 ID, 이전 값과 새 값, 변경 유형(예: &quot;추가됨&quot; 또는 &quot;수정됨&quot;), 작업 유형(예: &quot;예산&quot; 또는 &quot;Portfolio 이름&quot;) 및 적용 가능한 경우 하위 유형, 시간 및 사용자 이름이 포함됩니다.

### 필터링된 데이터 행으로 보고서 생성

1. [포트폴리오의 변경 기록을 엽니다](#portfolio-change-history).

1. 오른쪽 상단에서 ![보고서 다운로드](/help/search-social-commerce/assets/download.png "보고서 다운로드")를 클릭합니다.

1. [!UICONTROL Grid Reports] 설정에서 고유한 보고서 이름을 입력한 다음 **[!UICONTROL Generate]**&#x200B;을(를) 클릭합니다.

   기본적으로 파일의 이름은 &quot;portfolioChangeHistory_YYYYMMDD_NNNN&quot;입니다. 여기서 &quot;NNNN&quot;은 순차적 작업 번호입니다(예: &quot;portfolioChangeHistory_20260402_1326).

   파일이 [!UICONTROL Recently Generated] 목록에 추가됩니다.

1. (선택 사항) 파일이 완료되면 다운로드하려면 파일 이름 옆에 있는 ![다운로드](/help/search-social-commerce/assets/download.png "다운로드")를 클릭합니다.

   브라우저의 일반적인 절차에 따라 파일이 다운로드됩니다.

### 완료된 보고서 다운로드

1. [포트폴리오의 변경 기록을 엽니다](#portfolio-change-history).

1. 오른쪽 상단에서 ![보고서 다운로드](/help/search-social-commerce/assets/download.png "보고서 다운로드")를 클릭합니다.

1. [!UICONTROL Grid Reports] 대화 상자의 [!UICONTROL Recently Generated] 목록에서 파일 이름 옆에 있는 ![다운로드](/help/search-social-commerce/assets/download.png "다운로드")를 클릭합니다.

   브라우저의 일반적인 절차에 따라 파일이 다운로드됩니다.

### 완료된 보고서 삭제

1. [포트폴리오의 변경 기록을 엽니다](#portfolio-change-history).

1. 오른쪽 상단에서 ![보고서 다운로드](/help/search-social-commerce/assets/download.png "보고서 다운로드")를 클릭합니다.

1. [!UICONTROL Grid Reports] 대화 상자의 [!UICONTROL Recently Generated] 목록에서 파일 이름 옆에 있는 ![삭제](/help/search-social-commerce/assets/delete-new.png "삭제")를 클릭합니다.

>[!MORELIKETHIS]
>
>* [포트폴리오 만들기](portfolio-create.md)
>* [(새 UI) 포트폴리오 편집](portfolio-edit.md)
>* [(새 UI) 포트폴리오 성능 세부 정보 보기](portfolio-details.md)
>* [(새 UI) [!UICONTROL Portfolios] 보기에서 데이터를 다운로드합니다](portfolio-view-report.md)
>* [포트폴리오 정보](portfolio-about.md)
