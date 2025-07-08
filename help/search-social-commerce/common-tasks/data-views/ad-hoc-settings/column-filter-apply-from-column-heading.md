---
title: 열 제목 메뉴에서 데이터 필터 적용
description: 열 제목 메뉴에서에서 페이지 데이터를 필터링하는 방법을 알아봅니다.
exl-id: 508f254a-d859-4155-9bbd-84e0442f01d5
feature: Search Common Tasks, Search Custom Data Views
source-git-commit: a89a6513dfe468b98513b2d47c086a3107e63d47
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# 열 제목 메뉴에서 데이터 필터 적용

<!-- Doesn't include instructions for legacy Portfolios or Reports views -->

한 번에 하나씩, 열에 원하는 만큼 필터를 적용할 수 있습니다.<!-- True only for entity names, I think: All filters are joined using the AND operator. --> 사용 가능한 모든 지표를 사용하여 한 번에 두 개 이상의 필터를 추가하려면 &quot;[도구 모음에서 데이터 필터 적용](column-filter-apply-from-toolbar.md)&quot;을 참조하십시오.

1. 열 제목의 오른쪽에서 ![아래쪽 화살표](/help/search-social-commerce/assets/arrow-down-dropdown.png "아래쪽 화살표")를 클릭한 다음 **[!UICONTROL Add Filter]**&#x200B;을(를) 클릭합니다.

1. 열에서 필터를 정의합니다.

   * (입력 필드가 없는 필터) 포함할 각 값 옆에 있는 확인란을 선택한 다음 ![필터 업데이트](/help/search-social-commerce/assets/select.png "추가")를 클릭합니다.

   * (입력 필드가 있는 필터) 두 번째 메뉴에서 연산자를 선택하고 해당 값을 입력한 다음 ![필터 업데이트](/help/search-social-commerce/assets/select.png "추가")를 클릭합니다.

     예를 들어 &quot;[!UICONTROL Clicks]&quot; 열을 선택했으며 클릭수가 100개를 초과하는 행만 반환하려면 *[!UICONTROL greater than]*&quot;을(를) 선택하고 입력 필드에 `100`을(를) 입력하십시오. 데이터 유형에 따라 사용 가능한 연산자에는 *[!UICONTROL greater than]*, *[!UICONTROL less than]*, *[!UICONTROL equals]*, *[!UICONTROL contains]*, *[!UICONTROL doesn't contain]*, *[!UICONTROL starts with]*, *[!UICONTROL ends with]*, *[!UICONTROL no value]*, *[!UICONTROL has value]*, *[!UICONTROL before]*, *[!UICONTROL after]* 또는 *[!UICONTROL no date]이 포함될 수 있습니다.*

     >[!NOTE]
     >
     >* 텍스트 값은 대/소문자를 구분하지 않습니다. 예를 들어 이름에 &quot;대출&quot;이 있는 캠페인으로 필터링하면 결과에 &quot;소비자 대출&quot; 및 &quot;대출 신청&quot;이 포함됩니다.
     >* 열당 하나의 간단한 숫자 필터(예: [!UICONTROL Impressions] \> 100)만 적용할 수 있습니다.

>[!MORELIKETHIS]
>
>* [도구 모음에서 데이터 필터 적용](/help/search-social-commerce/common-tasks/data-views/ad-hoc-settings/column-filter-apply-from-toolbar.md)
>* [열 필터 편집](/help/search-social-commerce/common-tasks/data-views/ad-hoc-settings/column-filter-edit.md)
>* [열 필터 제거]&#x200B;(/help/search-social-commerce/common-tasks/data-views/ad-hoc-settings/
