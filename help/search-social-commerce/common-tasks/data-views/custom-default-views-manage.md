---
title: 기본 및 사용자 지정 보기 관리
description: 기본 보기 및 사용자 지정 보기를 맞춤화하는 방법에 대해 알아봅니다.
exl-id: 1f240760-6186-471f-bf1a-3e0ee13ce550
feature: Search Common Tasks, Search Custom Data Views
source-git-commit: 399974645b5083e735ff7aa94eba0a1115b4ddeb
workflow-type: tm+mt
source-wordcount: '4453'
ht-degree: 0%

---

# 기본 및 사용자 지정 보기 관리

<!-- Doesn't include instructions for legacy Portfolios or Reports views -->

기본 보기 및 사용자 지정 보기를 사용하면 검색 캠페인 데이터 보기 내에 표시되는 성능 데이터를 사용자 지정할 수 있습니다. 보기 설정에는 포함할 열, 필터, 날짜 범위, 전환 속성 설정 및 기타 고급 설정이 포함되며, 설정을 일시적으로 적용하거나 저장할 수 있습니다. (예외: 기본 보기에 대한 필터를 저장할 수 없습니다.) 각 기본 및 표준 사용자 지정 보기는 특정 보기(예: [!UICONTROL Portfolios] 또는 [!UICONTROL Campaigns]) 및 특정 광고주 계정에만 적용할 수 있습니다. 기존 사용자 인터페이스에서 각 범용 사용자 지정 보기는 특정 광고주의 엔티티 보기에 적용할 수 있으므로 엔티티 유형에 따라 달라지는 속성 열(예: 엔티티 이름 또는 상태)을 포함할 수 없습니다.

로그인할 때마다 기본적으로 기본 보기가 표시됩니다. 추가적인 사용자 정의 보기를 만들고 언제든지 적용할 수 있습니다. 선택적으로 광고주의 데이터를 볼 수 있는 다른 모든 사용자와 사용자가 만든 사용자 지정 보기를 공유할 수 있습니다. 사용자 정의 보기를 만드는 사람만 삭제할 수 있습니다.

기존 사용자 인터페이스에서 각 보기는 왼쪽 패널의 [!UICONTROL Custom Views] 섹션에서 바로 가기로 사용할 수 있습니다.

## 기본 또는 사용자 지정 보기 적용

### (새 UI) 관리 보기에 기본 또는 사용자 지정 보기 적용

1. 데이터 테이블 위에서 현재 적용된 보기(![보기](/help/search-social-commerce/assets/view.png "보기"))의 이름을 클릭합니다.

1. 필요에 따라 탭([!UICONTROL All Views], [!UICONTROL Private], [!UICONTROL Shared by Me] 및 [!UICONTROL From Others])을 클릭하여 보기를 찾습니다.

1. 뷰 이름 위에 커서를 놓고 **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

### (기존 UI) 캠페인 관리 보기에 기본 또는 사용자 지정 보기를 적용합니다

* (기본 보기) 기본 메뉴에서 **[!UICONTROL Search, Social, & Commerce]** \> **[!UICONTROL Campaigns]** \> **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다. 하위 메뉴에서 **[!UICONTROL Live]** \> **\[entity type\]**&#x200B;을(를) 클릭합니다.

* (사용자 정의 보기) 왼쪽 탐색 패널에서 다음을 수행합니다.

   1. 왼쪽 패널에서 **[!UICONTROL Custom Views]** 메뉴를 클릭하여 확장합니다.

      보기는 적용 가능한 엔터티별로 정렬됩니다.

   1. 사용 가능한 메뉴를 확장합니다.

      &quot;[!UICONTROL Universal Views]&quot;에는 모든 엔터티 보기에서 사용할 수 있는 사용자 지정 보기가 포함되어 있습니다. 다른 모든 사용자 지정 보기는 엔티티 유형별로 그룹화됩니다.

   1. 보기 이름을 클릭합니다.

      뷰가 유니버설이거나 현재 엔티티에 적용되는 경우, 데이터 테이블은 뷰 구성에 따라 다시 표시됩니다. 보기가 다른 엔티티에 적용되는 경우 적용 가능한 엔티티의 데이터가 보기 구성에 따라 표시됩니다.

## 사용자 지정 보기 만들기 {#create-custom-view}

>[!NOTE]
>
>사용자 지정 보기에 대해 지정하는 보기 설정 외에 현재 열 정렬 순서도 저장됩니다.

### (새 UI) 관리 보기에서 사용자 지정 보기를 만듭니다

*[!UICONTROL Simulations], [!UICONTROL Portfolios], [!UICONTROL Campaigns] 및 [!UICONTROL Ad Groups] 보기에서 사용 가능*

사용자 지정 보기는 단일 보기(예: [!UICONTROL Portfolios] 보기)에만 적용됩니다.

1. 데이터 테이블 위에서 현재 적용된 보기(![보기](/help/search-social-commerce/assets/view.png "보기"))의 이름을 클릭합니다.

1. **[!UICONTROL Create View]**&#x200B;을(를) 클릭합니다.

1. [사용자 지정 보기 설정](#view-settings-new-ui)을 지정하십시오.

1. 보기를 저장합니다.

   * 보기를 저장하고 적용하려면 **[!UICONTROL Save & Apply]**&#x200B;을(를) 클릭합니다.

   * 보기를 적용하지 않고 저장하려면 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

### (기존 UI) 캠페인 관리 보기에서 사용자 정의 보기를 만듭니다

사용자 지정 보기는 캠페인 관리 보기에만 적용할 수 있습니다.

1. 데이터 테이블 위의 도구 모음 오른쪽에서 현재 보기의 이름(&quot;[!UICONTROL Default]&quot;)을 클릭합니다.

1. [사용자 지정 보기 설정](#view-settings)을 지정하십시오.

1. **[!UICONTROL Save as New]**&#x200B;을(를) 클릭합니다.

1. 새 보기의 이름을 입력한 다음 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

   >[!TIP]
   >
   >탭과 탭이 적용되는 정보(예: &quot;일시 중지된 캠페인&quot; 또는 &quot;상위 50개 광고&quot;)를 식별하는 데 도움이 되는 이름을 사용합니다.

## 기본 또는 사용자 지정 보기 편집 {#view-edit}

### (새 UI) 기본 또는 사용자 지정 보기 편집

*[!UICONTROL Simulations], [!UICONTROL Portfolios], [!UICONTROL Campaigns] 및 [!UICONTROL Ad Groups] 보기에서 사용 가능*

1. 데이터 테이블 위에서 현재 적용된 보기(![보기](/help/search-social-commerce/assets/view.png "보기"))의 이름을 클릭합니다.

1. 필요에 따라 탭([!UICONTROL All Views], [!UICONTROL Private], [!UICONTROL Shared by Me] 및 [!UICONTROL From Others])을 클릭하여 보기를 찾습니다.

1. 보기 이름 위에 커서를 놓고 ![편집](/help/search-social-commerce/assets/edit-new.png)을 클릭합니다.

1. [사용자 지정 보기 설정](#view-settings-new-ui)을(를) 편집합니다.

1. 보기를 저장합니다.

   * 변경 내용을 적용하지 않고 저장하려면 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

   * 변경 내용을 저장하고 적용하려면 **[!UICONTROL Apply]**.<!-- Should be Save & Apply -->을(를) 클릭합니다

### (기존 UI) 기본 보기 또는 사용자 지정 보기 편집

1. 보기 설정을 엽니다.

   * (이미 보기를 적용한 경우) 데이터 테이블 위의 도구 모음 오른쪽에서 현재 보기의 이름(&quot;[!UICONTROL Default]&quot;)을 클릭합니다.

   * (적용되지 않는 사용자 지정 보기) 왼쪽 패널에서 ![사용자 지정 보기](/help/search-social-commerce/assets/custom-views-left-rail_icon.png "사용자 지정 보기")를 클릭하여 [!UICONTROL Custom Views] 메뉴를 확장합니다. 사용자 지정 보기 이름을 클릭합니다.

1. [보기 설정](#view-settings)을(를) 편집합니다.

   >[!NOTE]
   >
   >기본 보기 설정에 필터를 적용하지만 변경 사항을 저장할 수는 없습니다.

1. 설정을 적용하거나 저장합니다.

   * 보기에 저장하지 않고 설정을 일시적으로 적용하려면 **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

     이 설정은 최상위 관리 보기나 (해당되는 경우) [다른 광고주의 데이터를 보기](/help/search-social-commerce/common-tasks/change-advertiser.md)에서 벗어날 때까지 탭에 적용됩니다.

   * (만든 기본 보기 및 사용자 지정 보기의 경우) 현재 보기에 설정을 저장하려면 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

   * 새 사용자 지정 보기에 설정을 저장하려면 **[!UICONTROL Save As]**&#x200B;을(를) 클릭합니다. [!UICONTROL Enter New Custom View Name] 창에서 새 보기의 이름을 입력한 다음 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## (새 UI) 기본 또는 사용자 정의 보기 복제 {#view-clone}

*[!UICONTROL Simulations], [!UICONTROL Portfolios], [!UICONTROL Campaigns] 및 [!UICONTROL Ad Groups] 보기에서 사용 가능*

1. 데이터 테이블 위에서 현재 적용된 보기(![보기](/help/search-social-commerce/assets/view.png "보기"))의 이름을 클릭합니다.

1. 필요에 따라 탭([!UICONTROL All Views], [!UICONTROL Private], [!UICONTROL Shared by Me] 및 [!UICONTROL From Others])을 클릭하여 보기를 찾습니다.

1. 보기 이름 위에 커서를 놓고 ![복제](/help/search-social-commerce/assets/clone-new.png)를 클릭합니다.

1. 새 보기 이름을 입력하고 필요에 따라 [사용자 지정 보기 설정](#view-settings-new-ui)을 편집하세요.

1. 보기를 저장합니다.

   * 보기를 저장하고 적용하려면 **[!UICONTROL Save & Apply]**&#x200B;을(를) 클릭합니다.

   * 보기를 적용하지 않고 저장하려면 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 기본 보기를 시스템 기본 설정으로 재설정

기본 보기 설정을 복원하면 저장한 모든 설정이 제거되고 시스템 기본 설정이 다시 적용됩니다.

시스템 기본 설정은 관리 보기에 따라 다릅니다. 대부분의 관리 보기의 경우 시스템 기본 보기는 활성화된 계정의 항목 및 활성(예: 활성 캠페인의 활성 광고 그룹만)인 항목에 대한 전날의 데이터를 원가별로 정렬하고 트랜잭션 날짜를 기준으로 전환 데이터와 함께 표시합니다.

* 새 사용자 인터페이스에서:

   1. 데이터 테이블 위에서 현재 적용된 보기(![보기](/help/search-social-commerce/assets/view.png "보기"))의 이름을 클릭합니다.

   1. 필요에 따라 탭([!UICONTROL All Views], [!UICONTROL Private], [!UICONTROL Shared by Me] 및 [!UICONTROL From Others])을 클릭하여 보기를 찾습니다.

   1. 보기 이름 위에 커서를 놓고 ![되돌리기](/help/search-social-commerce/assets/revert-new.png)를 클릭합니다.

* 기존 캠페인 관리 보기에서 다음을 수행합니다.

   1. 왼쪽 패널에서 ![사용자 지정 보기](/help/search-social-commerce/assets/custom-views-left-rail_icon.png "사용자 지정 보기")를 클릭하여 [!UICONTROL Custom Views] 메뉴를 확장합니다.

      보기는 적용 가능한 엔터티별로 정렬됩니다.

   1. 보기 이름 옆에 있는 ![기본 설정으로 복원](/help/search-social-commerce/assets/restore.png "기본 설정으로 복원")을 클릭합니다.

## 사용자 정의 보기 삭제

만든 사용자 정의 보기를 삭제할 수 있습니다.

현재 탭에 적용되는 사용자 지정 보기를 삭제하는 경우, 보기 세트 외부로(예: [!UICONTROL Search] 메뉴의 보기에서 [!UICONTROL Reports] 메뉴로) 이동하거나(해당하는 경우) [다른 광고주에 대한 데이터를 볼 때](/help/search-social-commerce/common-tasks/change-advertiser.md)까지 탭에 사용자 지정 보기가 계속 표시됩니다.

* 새 사용자 인터페이스에서:

   1. 데이터 테이블 위에서 현재 적용된 보기(![보기](/help/search-social-commerce/assets/view.png "보기"))의 이름을 클릭합니다.

   1. 필요에 따라 탭([!UICONTROL All Views], [!UICONTROL Private], [!UICONTROL Shared by Me] 및 [!UICONTROL From Others])을 클릭하여 보기를 찾습니다.

   1. 보기 이름 위에 커서를 놓고 ![삭제](/help/search-social-commerce/assets/delete-new.png)를 클릭합니다.

   1. 확인 메시지에서 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

* 기존 캠페인 관리 보기에서 다음을 수행합니다.

   1. 왼쪽 패널에서 ![사용자 지정 보기](/help/search-social-commerce/assets/custom-views-left-rail_icon.png "사용자 지정 보기")를 클릭하여 [!UICONTROL Custom Views] 메뉴를 확장합니다.

   1. 사용자 지정 보기 이름 위에 커서를 놓고 ![삭제](/help/search-social-commerce/assets/delete.png "삭제")를 클릭합니다.

   1. 확인 메시지에서 **[!UICONTROL Continue]**&#x200B;을(를) 클릭합니다.

## 기본 및 사용자 지정 보기 설정

<!-- Simplify attribution rule definitions here and elsewhere and include links to "How attribution rules are calculated -->

### (새 UI) 기본 및 사용자 지정 보기 설정 {#view-settings-new-ui}

| **탭** | **필드** | **설명** |
| --- | --- | --- |
| [모든 탭 위] | 이름 | 보기의 고유 이름입니다. 기본 보기의 이름은 편집할 수 없습니다.<p><b>팁:</b> 탭과 이 탭이 적용되는 정보를 식별하는 데 도움이 되는 이름을 사용하십시오(예: &quot;일시 중지된 캠페인&quot; 또는 &quot;상위 50개 광고&quot;). |
|   | 다른 사용자와 공유 | (사용자 정의 보기 전용, 선택 사항) 광고주의 데이터를 볼 수 있는 다른 모든 사용자가 보기를 사용할 수 있습니다. 다른 사용자는 보기를 편집하거나 삭제할 수 없지만 설정에서 새 보기를 만들 수 있습니다. |
| 열 | 선택한 열 및 순서 | 표시되는 데이터 열 및 순서:<ul><li> (열을 추가하려면) 사용 가능한 열 목록에서 열 이름을 클릭한 다음 선택한 열 및 정렬 목록으로 끌어 놓거나 ![오른쪽 화살표](/help/search-social-commerce/assets/chevron-right.png)를 클릭하여 이동합니다.</li><li>(열의 가로 위치를 변경하려면) [선택한 열 및 순서 지정] 목록에서 열 이름을 클릭한 다음 원하는 위치로 끌어 놓거나 ![위쪽 화살표](/help/search-social-commerce/assets/chevron-up.png) 또는 ![아래쪽 화살표](/help/search-social-commerce/assets/chevron-down.png)를 클릭하여 이동합니다. 맨 위 열 이름이 왼쪽 열에 나타납니다.</li><li>(열을 제거하려면) 선택한 열 및 순서 지정 목록에서 열 이름을 클릭한 다음 사용 가능한 열 목록으로 끌어 놓거나 ![왼쪽 화살표](/help/search-social-commerce/assets/chevron-left.png)를 클릭하여 이동합니다.</li></ul><b>데이터 필터링</b><p>특정 유형의 데이터만 나열하려면 목록 옆에 있는 아이콘을 클릭합니다.<ul><li>속성 이름 및 ID에 대한 ![속성 아이콘](/help/search-social-commerce/assets/properties-icon-new.png)(예: [!UICONTROL Portfolio Name] 또는 [!UICONTROL Status])</li><li>노출 횟수 및 클릭 수와 같은 표준 트래픽 지표에 대한 ![트래픽 아이콘](/help/search-social-commerce/assets/traffic-metrics-icon-new.png)</li><li>![매출 아이콘](/help/search-social-commerce/assets/revenue-metrics-icon-new.png)(Analytics에서 동기화된 전환 및 사이트 참여 지표를 포함하여 광고주에 대해 추적된 전환 지표용)</li><li>![사용자 지정 아이콘](/help/search-social-commerce/assets/custom-metrics-icon-new.png)(광고주가 만든 사용자 지정 지표의 경우)</li><li>![분류 아이콘](/help/search-social-commerce/assets/classifications-icon-new.png)(레이블 분류용).</li></ul> <b>추가 참고 사항:</b><ul><li>새 지표를 추가, 만들기 또는 편집하려면 &quot;[사용자 지정 지표 만들기](/help/search-social-commerce/common-tasks/custom-metrics/custom-metric-create.md)&quot;, &quot;[사용자 지정 지표 편집](/help/search-social-commerce/common-tasks/custom-metrics/custom-metric-edit.md)&quot; 및 &quot;[사용자 지정 지표 삭제](/help/search-social-commerce/common-tasks/custom-metrics/custom-metric-delete.md)&quot;를 참조하십시오.</li><li>보고서에 통화가 다른 계정에 대한 데이터가 포함되어 있으면 통화 기반 열(예: 비용 및 CPC)에 대한 합계가 포함되지 않습니다.</li><li>[열 제목 메뉴에서 열 집합을 임시로 편집](/help/search-social-commerce/common-tasks/data-views/ad-hoc-settings/column-set-edit-column-heading.md)할 수 있고 [열 집합을 편집 및 정렬[!UICONTROL Columns] 아이콘에서 편집](/help/search-social-commerce/common-tasks/data-views/ad-hoc-settings/column-set-edit-sort-icon.md)할 수 있습니다. (열 아이콘![열 아이콘](/help/search-social-commerce/assets/custom-columns.png ").")</li></ul> |
|   | 정렬 기준: | 데이터를 정렬할 열입니다. 기본값은 각 보고서 유형에 따라 다릅니다. |
|   | 정렬 순서 | 데이터를 **오름차순** 또는 **내림차순** 순서로 정렬할지 여부를 지정합니다. |
| 필터 | [필터 정의] | (선택 사항) 데이터에 적용할 필터. 필터를 적용하면 열의 값이 지정된 조건을 충족하는 경우에만 행이 반환됩니다.<p>적용할 각 필터의 경우:<ol><li>[!UICONTROL Add Filter] 메뉴에서 열 이름을 선택합니다. 이 목록은 사용 가능한 모든 열을 포함하며 열 유형별로 정렬되며 속성 열이 먼저 표시됩니다.</li><li>열에서 필터 정의</li></ol>(입력 필드가 있는 필터) 두 번째 메뉴에서 연산자를 선택한 다음 해당 값을 입력합니다. 값은 대/소문자를 구분하지 않습니다.<p>예를 들어 &quot;클릭 수&quot; 열을 선택했으며 클릭 수가 100개를 초과하는 행만 반환하려는 경우 _\>_&#x200B;을(를) 선택하고 입력 필드에 `100`을(를) 입력합니다.<p>데이터 유형에 따라 사용 가능한 연산자에는 <i>보다 큼</i>, <i>보다 작음</i>, <i>같음</i>, <i>포함</i>, <i>포함하지 않음</i>, <i>다음으로 시작</i>, <i>다음으로 끝남</i>,<i>값 없음</i> 또는 <i>값 있음</i>이 포함될 수 있습니다. <i>이전</i>, <i>이후</i> 또는 <i>날짜 없음</i>.<p>(입력 필드가 없는 필터) 목록 항목 선택 메뉴 옆의 ![아래쪽 화살표](/help/search-social-commerce/assets/arrow-down-expand.png)를 클릭한 다음 포함할 각 값 옆의 확인란을 선택합니다.<p><b>메모:</b><ul><li>기본 보기 설정에 필터를 적용하지만 변경 사항을 저장할 수는 없습니다.</li><li>보기 내에서 [적용 가능한 필터를 일시적으로 변경](/help/search-social-commerce/common-tasks/data-views/ad-hoc-settings/column-filter-apply-from-toolbar.md)할 수도 있습니다.</li></ul> |
| 추가 설정 | 날짜 범위 | (날짜 범위 포함을 선택한 경우)<p>데이터를 생성할 날짜 범위입니다. 다음 옵션 중 하나를 선택합니다.<ul><li><i>[사전 설정 범위]</i>: <i>오늘</i>부터 <i>최근 180일</i> 범위의 일반 시간 증가 목록입니다. 목록에서 하나를 선택하십시오. 기본값은 <i>어제</i>입니다. 참고: <i>마지막 달</i>, <i>마지막 3개월</i> 및 <i>마지막 6개월</i>은(는) 이전 달력에 대한 데이터를 표시합니다.</li><li><i>사용자 지정 날짜 범위:</i> 시작 날짜와 종료 날짜를 지정합니다. 날짜를 MM/DD/YYYY 또는 M/D/YYYY 형식으로 입력하거나 필드 옆에 있는 ![달력 아이콘](/help/search-social-commerce/assets/calendar.png)을 클릭하고 날짜를 선택합니다.</li></ul> |
|   | 비교 | 지정된 날짜 범위의 데이터를 두 번째 날짜 범위의 데이터와 비교합니다. 이 옵션을 선택하는 경우 두 번째 날짜 범위를 지정합니다. 각 일반 데이터 열에 대해 두 개의 열이 더 추가됩니다. 예를 들어 보고서에는 &quot;노출 횟수&quot;에 대한 열이 한 개만 포함되지 않고 &quot;노출 횟수 범위 1&quot;, &quot;노출 횟수 범위 2&quot; 및 &quot;노출 횟수 차이&quot;에 대한 열이 포함됩니다.<p><b>메모:</b><ul><li>파생 지표에 대해서는 차이점 열이 표시되지 않습니다.</li><li>큰 날짜 범위를 비교하는 보고서를 생성하는 데 시간이 더 걸릴 수 있습니다.</li></ul> |
|   | 비교 형식 | ([!UICONTROL Comparison]이(가) 활성화된 경우) &quot;[_데이터 필드_] 차이&quot; 열에서 선택한 두 날짜 범위의 데이터 차이를 표시하는 방법입니다. 다음 옵션 중 하나를 선택합니다.<ul><li><i>Variance</i>(기본값): 차이를 숫자 값으로 표시합니다.</li><li><i>% 변경</i>: 차이를 백분율로 표시합니다.</li></ul> |
|   | 속성 규칙 | (Adobe Advertising 픽셀 기반 전환 추적 서비스가 있는 광고주만 해당) 탭 내에서 전환으로 이어지는 일련의 이벤트에서 전환 데이터(잠재적으로 여러 광고 채널 및 포트폴리오에)를 기여하는 방법을 알아봅니다. 기본적으로 광고주 수준 전환 속성 설정에 지정된 규칙이 선택됩니다.<ul><li> <i>첫 번째 이벤트</i>: 광고주의 클릭 전환 확인 기간 내에 일련의 첫 번째 유료 클릭으로, 또는 유료 클릭이 발생하지 않은 경우 광고주의 노출 확인 기간 내에 마지막 노출로 전환을 지정합니다.</li><li><i>첫 번째 이벤트 가중치 추가</i>: 광고주의 클릭 전환 확인 기간과 노출 전환 확인 기간 내에 발생한 일련의 모든 이벤트에 대한 전환 특성을 지정하지만, 첫 번째 이벤트에 가장 많은 가중치를 제공하고 다음 이벤트에 순차적으로 더 적은 가중치를 제공합니다. 전환 전에 유료 클릭과 노출이 모두 있으면 지정된 노출 재정의 가중치가 노출에 추가로 적용됩니다. 노출 횟수로만 전환되기 전 노출 횟수는 노출 횟수 대체 가중치가 아닌 광고주의 뷰스루 가중치에 따라 가중치가 적용됩니다.</li><li><i>짝수 배포</i>: 광고주의 클릭 전환 확인 기간과 노출 전환 확인 기간 내에 발생한 일련의 각 이벤트에 대해 동일한 속성을 사용합니다. 전환 전에 유료 클릭과 노출이 모두 있으면 지정된 노출 재정의 가중치가 노출에 추가로 적용됩니다. 노출 횟수로만 전환되기 전 노출 횟수는 노출 횟수 대체 가중치가 아닌 광고주의 뷰스루 가중치에 따라 가중치가 적용됩니다.</li><li><i>마지막 이벤트 가중치 추가</i>: 광고주의 클릭 전환 확인 기간과 노출 전환 확인 기간 내에 발생한 일련의 모든 이벤트에 대한 전환 특성을 지정하지만, 마지막 이벤트에 가장 많은 가중치를 제공하고 이전 이벤트에 순차적으로 더 적은 가중치를 제공합니다. 전환 전에 유료 클릭과 노출이 모두 있으면 지정된 노출 재정의 가중치가 노출에 추가로 적용됩니다. 노출 횟수로만 전환되기 전 노출 횟수는 노출 횟수 대체 가중치가 아닌 광고주의 뷰스루 가중치에 따라 가중치가 적용됩니다.</li><li><i>마지막 이벤트</i>(기본값): 광고주의 클릭 전환 확인 기간 내에 일련의 마지막 유료 클릭으로, 또는 유료 클릭이 발생하지 않은 경우 광고주의 노출 확인 기간 내에 마지막 노출로 전환을 지정합니다.</li><li><i>U자형</i>: 광고주의 클릭 전환 확인 기간과 노출 전환 확인 기간 내에 발생한 일련의 모든 이벤트에 대한 전환의 특성을 지정하지만, 첫 번째 이벤트와 마지막 이벤트에 가장 많은 가중치를 적용하고 전환 경로 중간에 있는 이벤트에는 순차적으로 더 적은 가중치를 적용합니다. 전환 전에 유료 클릭과 노출이 모두 있으면 지정된 노출 재정의 가중치가 노출에 추가로 적용됩니다. 노출 횟수로만 전환되기 전 노출 횟수는 노출 횟수 대체 가중치가 아닌 광고주의 뷰스루 가중치에 따라 가중치가 적용됩니다.</li></ul><p><b>메모:</b><ul><li>마지막 이벤트 이외의 모든 속성 규칙은 Adobe Advertising 클릭 추적이 있고 Adobe Advertising 또는 Adobe Analytics의 전환 추적(Analytics 통합 포함)이 있는 광고주에만 사용할 수 있습니다.</li><li>속성 규칙은 모든 채널에서 유료 광고를 클릭하는 데 적용됩니다. 이벤트 수준에서 추적할 수 없는 유료 검색 광고의 노출에는 적용되지 않습니다.</li><li>&quot;마지막 이벤트&quot; 규칙 중 하나를 제외한 모든 속성 규칙을 사용하여 전환 데이터를 보고할 때 전환을 유도하는 이벤트가 여러 포트폴리오에서 발생할 수 있습니다. 이 경우 해당 포트폴리오의 광고 또는 키워드가 보기에 포함된 경우에만 보기에 전환에 대한 데이터가 포함됩니다.</li><li>기본 보기의 경우 입찰 최적화 중에 각 입찰 단위에 대한 [목표 값](/help/search-social-commerce/glossary.md#o-p)(이전의 &quot;가중 수익&quot;)을 계산하는 데 사용되는 기본 속성 규칙을 유지하는 것이 좋습니다.</li></ul> |
|   | 전환 기준 | 전환 데이터를 보고하는 방법:<ul><li><i>클릭 날짜</i>: 지정한 기간 동안 발생한 클릭으로 인해 발생한 트랜잭션을 보려면 포트폴리오에 클릭과 거래 사이에 상당한 지연이 있는 경우 이 옵션은 포트폴리오에 대한 클릭당 기록 매출을 계산하는 데 유용하며 이는 시간이 지남에 따라 예상되는 매출 동작을 나타냅니다.</li><li><i>트랜잭션 날짜</i>(기본값): 트랜잭션 날짜가 지정된 기간 동안 발생한 트랜잭션을 확인합니다. 지정된 기간 내에 얻은 수입을 나타냅니다.</li></ul> |

### (기존 UI) 기본 및 사용자 지정 보기 설정 {#view-settings}

| **탭** | **필드** | **설명** |
| --- | --- | --- |
| [모든 탭 위] | 이름 | 보기의 고유 이름입니다. 기본 보기의 이름은 편집할 수 없습니다.<p><b>팁:</b> 탭과 이 탭이 적용되는 정보를 식별하는 데 도움이 되는 이름을 사용하십시오(예: &quot;일시 중지된 캠페인&quot; 또는 &quot;상위 50개 광고&quot;). |
|   | 유니버설 보기 | (기존 보기의 경우 읽기 전용) 모든 엔티티 보기(캠페인, 광고 등)에서 데이터 설정을 사용할 수 있도록 합니다. 범용 보기에는 지표 및 레이블 분류 열이 포함될 수 있지만 다른 모든 보기 속성은 엔티티 유형별로 다르므로 속성 열(예: 엔티티 이름 및 상태)은 포함될 수 없습니다. 해당되는 경우 모든 필터 기준이 엔티티 보기에 적용되며, 그렇지 않은 경우 무시됩니다. 모든 지표 필터는 로컬에서 평가됩니다(예: 클릭 수 \> 1000인 경우 캠페인 보기에 1000회 이상의 클릭이 있는 캠페인이 표시되고, 광고 그룹 보기에 1000회 이상의 클릭이 있는 광고 그룹이 표시됨).<p>범용 보기의 속성 열은 엔티티의 기본 보기에서 가져옵니다. 기본 보기 설정에서 특정 엔터티의 기본 속성 열을 변경할 수 있습니다.<p>이 옵션을 활성화하거나 비활성화하면 변경 사항을 기존 보기에 저장할 수 없지만 변경 사항으로 새 보기를 만들 수 있습니다. |
|   | 공유 | (기존 사용자 지정 보기만 해당, 선택 사항) 광고주의 데이터를 볼 수 있는 다른 모든 사용자가 보기를 사용할 수 있습니다. 다른 사용자는 보기를 편집하거나 삭제할 수 없지만 설정에서 새 보기를 만들 수 있습니다. 보기 목록에서 다른 사용자가 공유하고 있는 각 보기는 이탤릭체로 표시됩니다(예: &quot;_가장 성과가 좋은 캠페인_&quot;). |
| 열 | 선택한 열 및 순서 | 표시되는 데이터 열 및 순서:<ul><li> (열을 추가하려면) 사용 가능한 열 목록에서 열 이름을 클릭한 다음 선택한 열 및 정렬 목록으로 끌어 놓거나 ![오른쪽 화살표](/help/search-social-commerce/assets/chevron-right.png)를 클릭하여 이동합니다.</li><li>(열의 가로 위치를 변경하려면) [선택한 열 및 순서 지정] 목록에서 열 이름을 클릭한 다음 원하는 위치로 끌어 놓거나 ![위쪽 화살표](/help/search-social-commerce/assets/chevron-up.png) 또는 ![아래쪽 화살표](/help/search-social-commerce/assets/chevron-down.png)를 클릭하여 이동합니다. 맨 위 열 이름이 왼쪽 열에 나타납니다.</li><li>(열을 제거하려면) 선택한 열 및 순서 지정 목록에서 열 이름을 클릭한 다음 사용 가능한 열 목록으로 끌어 놓거나 ![왼쪽 화살표](/help/search-social-commerce/assets/chevron-left.png)를 클릭하여 이동합니다.</li></ul><b>데이터 필터링</b><p>특정 유형의 데이터만 나열하려면 목록 옆에 있는 아이콘을 클릭합니다.<ul><li>상태 등 검색 구성 요소의 속성 이름 및 ID에 대한 ![속성 아이콘](/help/search-social-commerce/assets/properties-icon.png)</li><li>노출 횟수 및 클릭 수와 같은 표준 트래픽 지표에 대한 ![트래픽 아이콘](/help/search-social-commerce/assets/traffic-metrics-icon.png)</li><li>![매출 아이콘](/help/search-social-commerce/assets/revenue-metrics-icon.png)(Analytics에서 동기화된 전환 및 사이트 참여 지표를 포함하여 광고주에 대해 추적된 전환 지표용)</li><li>![사용자 지정 아이콘](/help/search-social-commerce/assets/custom-metrics-icon.png)(광고주가 만든 사용자 지정 파생 지표용)</li><li>![분류 아이콘](/help/search-social-commerce/assets/classifications-icon.png)(레이블 분류용).</li></ul> <b>추가 참고 사항:</b><ul><li>새 지표를 추가, 만들기 또는 편집하려면 &quot;[사용자 지정 지표 만들기](/help/search-social-commerce/common-tasks/custom-metrics/custom-metric-create.md)&quot;, &quot;[사용자 지정 지표 편집](/help/search-social-commerce/common-tasks/custom-metrics/custom-metric-edit.md)&quot; 및 &quot;[사용자 지정 지표 삭제](/help/search-social-commerce/common-tasks/custom-metrics/custom-metric-delete.md)&quot;를 참조하십시오.</li><li>보고서에 통화가 다른 계정에 대한 데이터가 포함되어 있으면 통화 기반 열(예: 비용 및 CPC)에 대한 합계가 포함되지 않습니다.</li><li>[열 제목 메뉴에서 열 집합을 임시로 편집](/help/search-social-commerce/common-tasks/data-views/ad-hoc-settings/column-set-edit-column-heading.md)할 수 있고 [열 집합을 편집 및 정렬[!UICONTROL Columns] 아이콘에서 편집](/help/search-social-commerce/common-tasks/data-views/ad-hoc-settings/column-set-edit-sort-icon.md)할 수 있습니다. (열 아이콘![열 아이콘](/help/search-social-commerce/assets/custom-columns.png ").")</li></ul> |
|   | 정렬 기준: | 데이터를 정렬할 열입니다. 기본값은 각 보고서 유형에 따라 다릅니다. |
|   | 정렬 순서 | 데이터를 **오름차순** 또는 **내림차순** 순서로 정렬할지 여부를 지정합니다. 슬라이더를 이동하여 옵션을 선택합니다. |
| 필터 | [필터 정의] | (선택 사항) 데이터에 적용할 필터. 필터를 적용하면 열의 값이 지정된 조건을 충족하는 경우에만 행이 반환됩니다.<p>적용할 각 필터의 경우:<ol><li>[!UICONTROL Add Filter] 메뉴에서 열 이름을 선택합니다. 이 목록은 사용 가능한 모든 열을 포함하며 열 유형별로 정렬되며 속성 열이 먼저 표시됩니다.</li><li>열에서 필터 정의</li></ol>(입력 필드가 있는 필터) 두 번째 메뉴에서 연산자를 선택한 다음 해당 값을 입력합니다. 값은 대/소문자를 구분하지 않습니다.<p>예를 들어 &quot;클릭 수&quot; 열을 선택했으며 클릭 수가 100개를 초과하는 행만 반환하려는 경우 _\>_&#x200B;을(를) 선택하고 입력 필드에 `100`을(를) 입력합니다.<p>데이터 유형에 따라 사용 가능한 연산자에는 <i>보다 큼</i>, <i>보다 작음</i>, <i>같음</i>, <i>포함</i>, <i>포함하지 않음</i>, <i>다음으로 시작</i>, <i>다음으로 끝남</i>,<i>값 없음</i> 또는 <i>값 있음</i>이 포함될 수 있습니다. <i>이전</i>, <i>이후</i> 또는 <i>날짜 없음</i>.<p>(입력 필드가 없는 필터) 목록 항목 선택 메뉴 옆의 ![아래쪽 화살표](/help/search-social-commerce/assets/arrow-down-expand.png)를 클릭한 다음 포함할 각 값 옆의 확인란을 선택합니다.<p><b>메모:</b><ul><li>기본 보기 설정에 필터를 적용하지만 변경 사항을 저장할 수는 없습니다.</li><li>보기 내에서 [적용 가능한 필터를 일시적으로 변경](/help/search-social-commerce/common-tasks/data-views/ad-hoc-settings/column-filter-apply-from-toolbar.md)할 수도 있습니다.</li></ul> |
|   | 성능 데이터가 있는 행만 포함 | (광고 그룹, 키워드, 제품 그룹, 배치 및 자동 타겟 보기 전용) <p>지정된 날짜 동안의 성능 데이터가 있는 행만 포함합니다. 기본적으로 이 옵션은 페이지 로드 시간을 줄이기 위해 선택됩니다. <p><b>경고</b>: 옵션을 선택 취소한 경우 성능 데이터가 없는 엔터티가 뷰에 많이 있으면 데이터를 표시하는 데 시간이 더 오래 걸립니다.<p> <b>참고</b>: 필터에 대한 변경 내용을 기본 보기 설정에 적용할 수는 있지만 저장할 수는 없습니다. 기본 보기는 항상 성능 데이터가 있는 엔티티만 표시합니다. |
| 날짜 | 날짜 범위 | (날짜 범위 포함을 선택한 경우)<p>데이터를 생성할 날짜 범위입니다. 다음 옵션 중 하나를 선택합니다.<ul><li><i>[사전 설정 범위]</i>: <i>오늘</i>부터 <i>최근 180일</i> 범위의 일반 시간 증가 목록입니다. 목록에서 하나를 선택하십시오. 기본값은 <i>어제</i>입니다. 참고: <i>마지막 달</i>, <i>마지막 3개월</i> 및 <i>마지막 6개월</i>은(는) 이전 달력에 대한 데이터를 표시합니다.</li><li><i>사용자 지정 날짜 범위:</i> 시작 날짜와 종료 날짜를 지정합니다. 날짜를 MM/DD/YYYY 또는 M/D/YYYY 형식으로 입력하거나 필드 옆에 있는 ![달력 아이콘](/help/search-social-commerce/assets/calendar.png)을 클릭하고 날짜를 선택합니다.</li></ul> |
|   | 비교 | 지정된 날짜 범위의 데이터를 두 번째 날짜 범위의 데이터와 비교합니다. 이 옵션을 선택하는 경우 두 번째 날짜 범위를 지정합니다. 각 일반 데이터 열에 대해 두 개의 열이 더 추가됩니다. 예를 들어 보고서에는 &quot;노출 횟수&quot;에 대한 열이 한 개만 포함되지 않고 &quot;노출 횟수 범위 1&quot;, &quot;노출 횟수 범위 2&quot; 및 &quot;노출 횟수 차이&quot;에 대한 열이 포함됩니다.<p><b>메모:</b><ul><li>파생 지표에 대해서는 차이점 열이 표시되지 않습니다.</li><li>큰 날짜 범위를 비교하는 보고서를 생성하는 데 시간이 더 걸릴 수 있습니다.</li></ul> |
|   | 비교 형식 | ([!UICONTROL Comparison]이(가) 활성화된 경우) &quot;[_데이터 필드_] 차이&quot; 열에서 선택한 두 날짜 범위의 데이터 차이를 표시하는 방법입니다. 다음 옵션 중 하나를 선택합니다.<ul><li><i>Variance</i>(기본값): 차이를 숫자 값으로 표시합니다.</li><li><i>% 변경</i>: 차이를 백분율로 표시합니다.</li></ul> |
| 추가 설정 | 기본값 사용 | 광고주 수준 전환 속성 설정에 지정된 속성 설정을 적용합니다. |
|   | 속성 규칙 | (Adobe Advertising 픽셀 기반 전환 추적 서비스가 있는 광고주만 해당) 탭 내에서 전환으로 이어지는 일련의 이벤트에서 전환 데이터(잠재적으로 여러 광고 채널 및 포트폴리오에)를 기여하는 방법을 알아봅니다. 기본적으로 광고주 수준 전환 속성 설정에 지정된 규칙이 선택됩니다.<ul><li> <i>첫 번째 이벤트</i>: 광고주의 클릭 전환 확인 기간 내에 일련의 첫 번째 유료 클릭으로, 또는 유료 클릭이 발생하지 않은 경우 광고주의 노출 확인 기간 내에 마지막 노출로 전환을 지정합니다.</li><li><i>첫 번째 이벤트 가중치 추가</i>: 광고주의 클릭 전환 확인 기간과 노출 전환 확인 기간 내에 발생한 일련의 모든 이벤트에 대한 전환 특성을 지정하지만, 첫 번째 이벤트에 가장 많은 가중치를 제공하고 다음 이벤트에 순차적으로 더 적은 가중치를 제공합니다. 전환 전에 유료 클릭과 노출이 모두 있으면 지정된 노출 재정의 가중치가 노출에 추가로 적용됩니다. 노출 횟수로만 전환되기 전 노출 횟수는 노출 횟수 대체 가중치가 아닌 광고주의 뷰스루 가중치에 따라 가중치가 적용됩니다.</li><li><i>짝수 배포</i>: 광고주의 클릭 전환 확인 기간과 노출 전환 확인 기간 내에 발생한 일련의 각 이벤트에 대해 동일한 속성을 사용합니다. 전환 전에 유료 클릭과 노출이 모두 있으면 지정된 노출 재정의 가중치가 노출에 추가로 적용됩니다. 노출 횟수로만 전환되기 전 노출 횟수는 노출 횟수 대체 가중치가 아닌 광고주의 뷰스루 가중치에 따라 가중치가 적용됩니다.</li><li><i>마지막 이벤트 가중치 추가</i>: 광고주의 클릭 전환 확인 기간과 노출 전환 확인 기간 내에 발생한 일련의 모든 이벤트에 대한 전환 특성을 지정하지만, 마지막 이벤트에 가장 많은 가중치를 제공하고 이전 이벤트에 순차적으로 더 적은 가중치를 제공합니다. 전환 전에 유료 클릭과 노출이 모두 있으면 지정된 노출 재정의 가중치가 노출에 추가로 적용됩니다. 노출 횟수로만 전환되기 전 노출 횟수는 노출 횟수 대체 가중치가 아닌 광고주의 뷰스루 가중치에 따라 가중치가 적용됩니다.</li><li><i>마지막 이벤트</i>(기본값): 광고주의 클릭 전환 확인 기간 내에 일련의 마지막 유료 클릭으로, 또는 유료 클릭이 발생하지 않은 경우 광고주의 노출 확인 기간 내에 마지막 노출로 전환을 지정합니다.</li><li><i>U자형</i>: 광고주의 클릭 전환 확인 기간과 노출 전환 확인 기간 내에 발생한 일련의 모든 이벤트에 대한 전환의 특성을 지정하지만, 첫 번째 이벤트와 마지막 이벤트에 가장 많은 가중치를 적용하고 전환 경로 중간에 있는 이벤트에는 순차적으로 더 적은 가중치를 적용합니다. 전환 전에 유료 클릭과 노출이 모두 있으면 지정된 노출 재정의 가중치가 노출에 추가로 적용됩니다. 노출 횟수로만 전환되기 전 노출 횟수는 노출 횟수 대체 가중치가 아닌 광고주의 뷰스루 가중치에 따라 가중치가 적용됩니다.</li></ul><p><b>메모:</b><ul><li>마지막 이벤트 이외의 모든 속성 규칙은 Adobe Advertising 클릭 추적이 있고 Adobe Advertising 또는 Adobe Analytics의 전환 추적(Analytics 통합 포함)이 있는 광고주에만 사용할 수 있습니다.</li><li>속성 규칙은 모든 채널에서 유료 광고를 클릭하는 데 적용됩니다. 이벤트 수준에서 추적할 수 없는 유료 검색 광고의 노출에는 적용되지 않습니다.</li><li>&quot;마지막 이벤트&quot; 규칙 중 하나를 제외한 모든 속성 규칙을 사용하여 전환 데이터를 보고할 때 전환을 유도하는 이벤트가 여러 포트폴리오에서 발생할 수 있습니다. 이 경우 해당 포트폴리오의 광고 또는 키워드가 보기에 포함된 경우에만 보기에 전환에 대한 데이터가 포함됩니다.</li><li>기본 보기의 경우 입찰 최적화 중에 각 입찰 단위에 대한 [목표 값](/help/search-social-commerce/glossary.md#o-p)(이전의 &quot;가중 수익&quot;)을 계산하는 데 사용되는 기본 속성 규칙을 유지하는 것이 좋습니다.</li></ul> |
|   | 전환 기준 | 전환 데이터를 보고하는 방법:<ul><li><i>클릭 날짜</i>: 지정한 기간 동안 발생한 클릭으로 인해 발생한 트랜잭션을 보려면 포트폴리오에 클릭과 거래 사이에 상당한 지연이 있는 경우 이 옵션은 포트폴리오에 대한 클릭당 기록 매출을 계산하는 데 유용하며 이는 시간이 지남에 따라 예상되는 매출 동작을 나타냅니다.</li><li><i>트랜잭션 날짜</i>(기본값): 트랜잭션 날짜가 지정된 기간 동안 발생한 트랜잭션을 확인합니다. 지정된 기간 내에 얻은 수입을 나타냅니다.</li></ul> |
