---
title: 열 제목 메뉴에서 데이터 필터 적용
description: 열 제목 메뉴에서에서 페이지 데이터를 필터링하는 방법을 알아봅니다.
exl-id: ad745599-fd98-4f34-b181-085070adb685
feature: Search Common Tasks, Search Custom Data Views
source-git-commit: 9c4dcb19e386d8e1eea541776f5b92c9d500ae9f
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# 열 제목 메뉴에서 데이터 필터 적용

한 번에 하나씩, 열에 원하는 만큼 필터를 적용할 수 있습니다. 모든 필터는 AND 연산자를 사용하여 연결됩니다. 사용 가능한 모든 지표를 사용하여 한 번에 두 개 이상의 필터를 추가하려면 &quot;를 참조하십시오.[도구 모음에서 데이터 필터 적용](column-filter-apply-from-toolbar.md).&quot;

1. 열 제목 오른쪽에서 ![아래쪽 화살표](/help/search-social-commerce/assets/arrow-down-dropdown.png "아래쪽 화살표")을 클릭한 다음 을 클릭합니다 **[!UICONTROL Add Filter]**.

1. 열에서 필터를 정의합니다.

   * (입력 필드가 없는 필터) 포함할 각 값 옆에 있는 확인란을 선택한 다음 을 클릭합니다. ![필터 업데이트](/help/search-social-commerce/assets/select.png "필터 업데이트").

   * (입력 필드가 있는 필터) 두 번째 메뉴에서 연산자를 선택하고 해당 값을 입력한 다음 을 클릭합니다. ![필터 업데이트](/help/search-social-commerce/assets/select.png "필터 업데이트").

     예를 들어, &quot;를 선택한 경우[!UICONTROL Clicks]&quot;열을 반환하고 클릭 수가 100개를 초과하는 행만 반환한 다음 선택 *[!UICONTROL greater than]*&quot;및 입력 `100` 입력 필드에서 데이터 유형에 따라 사용 가능한 연산자는 다음을 포함할 수 있습니다 *[!UICONTROL greater than]*, *[!UICONTROL less than]*, *[!UICONTROL equals]*, *[!UICONTROL contains]*, *[!UICONTROL doesn't contain]*, *[!UICONTROL starts with]*, *[!UICONTROL ends with]*, *[!UICONTROL no value]*, *[!UICONTROL has value]*, *[!UICONTROL before]*, *[!UICONTROL after]*, 또는 *[!UICONTROL no date].*

     >[!NOTE]
     >
     >* 텍스트 값은 대/소문자를 구분하지 않습니다. 예를 들어 이름에 &quot;대출&quot;이 있는 캠페인으로 필터링하면 결과에 &quot;소비자 대출&quot; 및 &quot;대출 신청&quot;이 포함됩니다.
     >* 단순 숫자 필터는 하나만 적용할 수 있습니다(예: [!UICONTROL Impressions] 열당 \> 100).
