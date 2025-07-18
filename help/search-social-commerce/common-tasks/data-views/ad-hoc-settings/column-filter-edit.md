---
title: 열 필터 편집
description: 열 필터를 편집하는 방법을 알아봅니다.
exl-id: 68f816ea-cde2-4df0-b46c-f47fa20a2727
feature: Search Common Tasks, Search Custom Data Views
source-git-commit: a89a6513dfe468b98513b2d47c086a3107e63d47
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---

# 열 필터 편집

<!-- Doesn't include instructions for legacy Portfolios view; not available in Reports views -->

## (새 UI) 관리 보기에서 필터 세트 편집

1. 도구 모음에서 ![필터](/help/search-social-commerce/assets/filter-new.png "필터")를 클릭합니다.

1. 필터 설정에서 다음 중 하나를 수행합니다.

   * 필터를 추가하려면 **[!UICONTROL ADD FILTER]**&#x200B;을(를) 클릭하고 다음을 수행합니다.

      1. (선택 사항) 텍스트 문자열로 열 이름을 필터링하려면 **[!UICONTROL ADD FILTER]** 입력 필드에 검색 문자열을 입력합니다.

      1. 열 메뉴에서 열 이름을 선택합니다.

      1. 열에서 필터를 정의합니다.

         * (입력 필드가 없는 필터) 두 번째 메뉴 옆의 ![아래쪽 화살표](/help/search-social-commerce/assets/arrow-down-expand.png "아래쪽 화살표")를 클릭한 다음 포함할 각 값 옆의 확인란을 선택합니다.

         * (입력 필드가 있는 필터) 두 번째 메뉴에서 연산자를 선택한 다음 해당 값을 입력합니다.

           예를 들어 &quot;[!UICONTROL Clicks]&quot; 열을 선택했으며 클릭수가 100개를 초과하는 행만 반환하려는 경우 *[!UICONTROL greater than]*&quot;을(를) 선택하고 입력 필드에 `100`을(를) 입력합니다.

           데이터 유형에 따라 사용 가능한 연산자에는 *[!UICONTROL greater than]*, *[!UICONTROL less than]*, *[!UICONTROL equals]*, *[!UICONTROL contains]*, *[!UICONTROL doesn't contain]*, *[!UICONTROL starts with]*, *[!UICONTROL ends with]*, *[!UICONTROL no value]*, *[!UICONTROL has value]*, *[!UICONTROL before]*, *[!UICONTROL after]* 또는 *[!UICONTROL no date]이(가) 포함될 수 있습니다.*

           **참고:** 텍스트 값은 대/소문자를 구분하지 않습니다. 예를 들어 이름에 &quot;대출&quot;이 있는 캠페인으로 필터링하면 결과에 &quot;소비자 대출&quot; 및 &quot;대출 신청&quot;이 포함됩니다.

   * 기존 필터를 편집하려면 필터를 클릭한 다음 필터 정의를 변경합니다.

   * 기존 필터를 제거하려면 필터 정의 옆에 있는 **[!UICONTROL -]**&#x200B;을(를) 클릭합니다.

## (기존 UI) 캠페인 관리 보기에서 필터 세트를 편집합니다

1. 도구 모음에서 ![필터](/help/search-social-commerce/assets/filter.png "필터")를 클릭합니다.

1. 필터 설정에서 다음 중 하나를 수행합니다.

   * 필터를 추가하려면 ![필터 추가](/help/search-social-commerce/assets/add.png "필터 추가") **[!UICONTROL ADD FILTER]**&#x200B;를 클릭하고 다음을 수행하십시오.

      1. (선택 사항) 텍스트 문자열로 열 이름을 필터링하려면 **[!UICONTROL ADD FILTER]** 입력 필드에 검색 문자열을 입력합니다.

      1. 열 메뉴에서 열 이름을 선택합니다.

      1. 열에서 필터를 정의합니다.

         * (입력 필드가 없는 필터) 두 번째 메뉴 옆의 ![아래쪽 화살표](/help/search-social-commerce/assets/arrow-down-expand.png "아래쪽 화살표")를 클릭한 다음 포함할 각 값 옆의 확인란을 선택합니다.

         * (입력 필드가 있는 필터) 두 번째 메뉴에서 연산자를 선택한 다음 해당 값을 입력합니다.

           예를 들어 &quot;[!UICONTROL Clicks]&quot; 열을 선택했으며 클릭수가 100개를 초과하는 행만 반환하려는 경우 *[!UICONTROL greater than]*&quot;을(를) 선택하고 입력 필드에 `100`을(를) 입력합니다.

           데이터 유형에 따라 사용 가능한 연산자에는 *[!UICONTROL greater than]*, *[!UICONTROL less than]*, *[!UICONTROL equals]*, *[!UICONTROL contains]*, *[!UICONTROL doesn't contain]*, *[!UICONTROL starts with]*, *[!UICONTROL ends with]*, *[!UICONTROL no value]* 또는 *[!UICONTROL has value]*, *[!UICONTROL before]*, *[!UICONTROL after]* 또는 *[!UICONTROL no date]이(가) 포함될 수 있습니다.*

           **참고:** 텍스트 값은 대/소문자를 구분하지 않습니다. 예를 들어 이름에 &quot;대출&quot;이 있는 캠페인을 검색하는 경우 결과에 &quot;소비자 대출&quot; 및 &quot;대출 신청&quot;이 포함됩니다.

   * 기존 필터를 편집하려면 필터를 클릭한 다음 필터 정의를 변경합니다.

   * 기존 필터를 제거하려면 필터 정의 옆에 있는 ![삭제](/help/search-social-commerce/assets/delete.png "삭제")를 클릭합니다.

1. ([!UICONTROL Keywords] 보기 전용, 선택 사항) &quot;[!UICONTROL Include rows with no performance data]&quot; 설정을 선택하거나 선택 취소합니다.

   >[!WARNING]
   >
   >이 옵션을 선택하면 페이지 로드 시간이 늘어납니다.

1. **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

## 관리 보기에서 단일 필터 편집

1. 데이터 테이블 위에서 필터 정의를 클릭합니다.

1. 열에서 필터를 재정의합니다.

   * (입력 필드가 없는 필터) 두 번째 메뉴 옆의 ![아래쪽 화살표](/help/search-social-commerce/assets/arrow-down-expand.png "아래쪽 화살표")를 클릭하고 포함할 각 값 옆의 확인란을 선택합니다.

   * (입력 필드가 있는 필터) 두 번째 메뉴에서 연산자를 선택한 다음 해당 값을 입력합니다.

     예를 들어 &quot;[!UICONTROL Clicks]&quot; 열을 선택했으며 클릭수가 100개를 초과하는 행만 반환하려는 경우 *[!UICONTROL greater than]*&quot;을(를) 선택하고 입력 필드에 `100`을(를) 입력합니다.

     데이터 형식에 따라 사용 가능한 연산자에는 *[!UICONTROL greater than]*, *다음보다 작음*, *[!UICONTROL equals]*, *[!UICONTROL contains]*, *포함하지 않음* 또는 *다음으로 시작*&#x200B;이 포함될 수 있습니다.

     **참고:** 텍스트 값은 대/소문자를 구분하지 않습니다. 예를 들어 이름에 &quot;대출&quot;이 있는 캠페인을 검색하는 경우 결과에 &quot;소비자 대출&quot; 및 &quot;대출 신청&quot;이 포함됩니다.

>[!MORELIKETHIS]
>
>* [열 제목 메뉴에서 데이터 필터 적용](/help/search-social-commerce/common-tasks/data-views/ad-hoc-settings/column-filter-apply-from-column-heading.md)
>* [도구 모음에서 데이터 필터 적용](/help/search-social-commerce/common-tasks/data-views/ad-hoc-settings/column-filter-apply-from-toolbar.md)
>* [열 필터 제거]&#x200B;(/help/search-social-commerce/common-tasks/data-views/ad-hoc-settings/
