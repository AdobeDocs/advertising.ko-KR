---
title: 열 필터 편집
description: 열 필터를 편집하는 방법을 알아봅니다.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# 열 필터 편집

## 필터 세트 편집

1. 클릭 ![필터](/help/search-social-commerce/assets/filter.png "필터") 을 클릭합니다.

1. 필터 설정에서 다음 중 하나를 수행합니다.

   * 필터를 추가하려면 ![필터 추가](/help/search-social-commerce/assets/add.png "필터 추가") **[!UICONTROL ADD FILTER]** 을 클릭하고 다음을 수행합니다.

      1. (선택 사항) 텍스트 문자열로 열 이름을 필터링하려면 **[!UICONTROL ADD FILTER]** 입력 필드.

      1. 열 메뉴에서 열 이름을 선택합니다.

      1. 열에서 필터를 정의합니다.

         * (입력 필드가 없는 필터) ![아래쪽 화살표](/help/search-social-commerce/assets/arrow-down-expand.png "아래쪽 화살표") 두 번째 메뉴 옆에 포함할 각 값 옆의 확인란을 선택한 다음 을 클릭합니다 ![필터 업데이트](/help/search-social-commerce/assets/select.png "필터 업데이트").

         * (입력 필드가 있는 필터) 두 번째 메뉴에서 연산자를 선택하고 해당 값을 입력한 다음 을 클릭합니다. ![필터 업데이트](/help/search-social-commerce/assets/select.png "필터 업데이트").

            예를 들어, &quot;를 선택한 경우[!UICONTROL Clicks]&quot;열을 반환하고 클릭 수가 100개를 초과하는 행만 반환한 다음 선택 *[!UICONTROL greater than]*&quot;및 입력 `100` 입력 필드에서 을 클릭합니다.

            데이터 유형에 따라 사용 가능한 연산자는 다음을 포함할 수 있습니다. *[!UICONTROL greater than]*, *[!UICONTROL less than]*, *[!UICONTROL equals]*, *[!UICONTROL contains]*, *[!UICONTROL doesn't contain]*, *[!UICONTROL starts with]*, *[!UICONTROL ends with]*, *[!UICONTROL no value]*, 또는 *[!UICONTROL has value]*, *[!UICONTROL before]*, *[!UICONTROL after]*, 또는 *[!UICONTROL no date].*

            **참고:** 텍스트 값은 대/소문자를 구분하지 않습니다. 예를 들어 이름에 &quot;대출&quot;이 있는 캠페인을 검색하는 경우 결과에 &quot;소비자 대출&quot; 및 &quot;대출 신청&quot;이 포함됩니다.
   * 기존 필터를 편집하려면 필터를 클릭하고 필터 정의를 변경한 다음 를 클릭합니다 ![필터 업데이트](/help/search-social-commerce/assets/select.png "필터 업데이트").

   * 기존 필터를 제거하려면 **[!UICONTROL X]** 필터 정의 옆에 있습니다.


1. ([!UICONTROL Keywords] 보기 전용, 선택 사항) &quot;&quot;로 설정할 설정을 선택하거나 선택 취소합니다.[!UICONTROL Include rows with no performance data].&quot;

   >[!WARNING]
   >
   >이 옵션을 선택하면 페이지 로드 시간이 늘어납니다.

1. 클릭 **[!UICONTROL Apply]**.

## 단일 필터 편집

1. (필요한 경우) 데이터 테이블 위에 있는 필터 세트에서 ![자세히](/help/search-social-commerce/assets/more-filters.png "자세히") 필터 세트를 확장합니다.

1. 데이터 테이블 위에서 필터 정의를 클릭합니다.

1. 적용할 필터 편집:

   1. (선택 사항) 열 메뉴에서 열 이름을 편집합니다.

   1. (선택 사항) 열에서 필터를 재정의합니다.

      * (입력 필드가 없는 필터) ![아래쪽 화살표](/help/search-social-commerce/assets/arrow-down-expand.png "아래쪽 화살표") 두 번째 메뉴 옆에 포함할 각 값 옆의 확인란을 선택한 다음 을 클릭합니다 ![필터 업데이트](/help/search-social-commerce/assets/select.png "필터 업데이트").

      * (입력 필드가 있는 필터) 두 번째 메뉴에서 연산자를 선택하고 해당 값을 입력한 다음 을 클릭합니다. ![필터 업데이트](/help/search-social-commerce/assets/select.png "필터 업데이트").

         예를 들어, &quot;를 선택한 경우[!UICONTROL Clicks]&quot;열을 반환하고 클릭 수가 100개를 초과하는 행만 반환한 다음 선택 *[!UICONTROL greater than]*&quot;및 입력 `100` 입력 필드

         데이터 유형에 따라 사용 가능한 연산자는 다음을 포함할 수 있습니다. *[!UICONTROL greater than]*, *보다 작음*, *[!UICONTROL equals]*, *[!UICONTROL contains]*, *포함하지 않음*, 또는 *다음으로 시작.*

         **참고:** 텍스트 값은 대/소문자를 구분하지 않습니다. 예를 들어 이름에 &quot;대출&quot;이 있는 캠페인을 검색하는 경우 결과에 &quot;소비자 대출&quot; 및 &quot;대출 신청&quot;이 포함됩니다.
