---
title: 도구 모음에서 데이터 필터 적용
description: 도구 모음에서 페이지 데이터를 필터링하는 방법을 알아봅니다.
exl-id: fc1dca75-b0e5-48fd-90ee-f09c158e3e8b
feature: Search Common Tasks, Search Custom Data Views
source-git-commit: e517dd5f5fa283ff8a2f57728612937148889732
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# 도구 모음에서 데이터 필터 적용

보기를 원하는 만큼 필터를 적용할 수 있습니다. 모든 필터는 AND 연산자를 사용하여 연결됩니다.

1. 도구 모음에서 를 클릭합니다 ![필터](/help/search-social-commerce/assets/filter.png "필터").

1. 필터 설정에서 다음 중 하나를 수행합니다.

   * 필터를 추가하려면 ![필터 추가](/help/search-social-commerce/assets/add.png "필터 추가") **[!UICONTROL ADD FILTER]**&#x200B;을 클릭하고 다음을 수행합니다.

      1. (선택 사항) 텍스트 문자열로 열 이름을 필터링하려면 **[!UICONTROL ADD FILTER]** 입력 필드.

      1. 열 메뉴에서 열 이름을 선택합니다.

      1. 열에서 필터를 정의합니다.

         * (입력 필드가 없는 필터) ![아래쪽 화살표](/help/search-social-commerce/assets/arrow-down-expand.png "아래쪽 화살표") 두 번째 메뉴 옆에 있는 다음 포함할 각 값 옆에 있는 확인란을 선택합니다.

         * (입력 필드가 있는 필터) 두 번째 메뉴에서 연산자를 선택한 다음 해당 값을 입력합니다.

           예를 들어, &quot;를 선택한 경우[!UICONTROL Clicks]&quot;열을 반환하고 클릭 수가 100개를 초과하는 행만 반환한 다음 선택 *[!UICONTROL greater than]*&quot;및 입력 `100` 입력 필드에서 을 클릭합니다.

           데이터 유형에 따라 사용 가능한 연산자는 다음을 포함할 수 있습니다. *[!UICONTROL greater than]*, *[!UICONTROL less than]*, *[!UICONTROL equals]*, *[!UICONTROL contains]*, *[!UICONTROL doesn't contain]*, *[!UICONTROL starts with]*, *[!UICONTROL ends with]*, *[!UICONTROL no value]*, *[!UICONTROL has value]*, *[!UICONTROL before]*, *[!UICONTROL after]*, 또는 *[!UICONTROL no date].*

           **참고:** 텍스트 값은 대/소문자를 구분하지 않습니다. 예를 들어 이름에 &quot;대출&quot;이 있는 캠페인으로 필터링하면 결과에 &quot;소비자 대출&quot; 및 &quot;대출 신청&quot;이 포함됩니다.

         * ([!UICONTROL Ad Groups], [!UICONTROL Keywords], [!UICONTROL Product Groups], [!UICONTROL Placements], 및 [!UICONTROL Auto Targets] 보기 전용, 선택 사항) 설정을 &quot;[!UICONTROL Include rows with performance data only].&quot;

           **경고:** 옵션을 선택 취소하면 보기에 성능 데이터가 없는 엔티티가 많이 포함된 경우 데이터를 표시하는 데 시간이 더 오래 걸립니다.

   * 기존 필터를 편집하려면 필터를 클릭하고 필터 정의를 변경한 다음 를 클릭합니다 ![필터 업데이트](/help/search-social-commerce/assets/select.png "필터 업데이트").

   * 기존 필터를 제거하려면 **[!UICONTROL X]** 필터 정의 옆에 있습니다.

1. 클릭 **[!UICONTROL Apply]**.
