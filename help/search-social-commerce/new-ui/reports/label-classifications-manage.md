---
title: 레이블 분류 관리
description: 레이블 분류를 사용하여 계정 구성 요소를 그룹화하는 방법에 대해 알아봅니다.
feature: Search Label Classifications
source-git-commit: 84eb5f060a696e057f706c0066c18c9afc1511e1
workflow-type: tm+mt
source-wordcount: '1515'
ht-degree: 0%

---

# 레이블 분류 관리

레이블 분류를 사용하면 계정 구성 요소를 의미 있는 세트로 그룹화할 수 있습니다. 예를 들어 &quot;지역&quot;이라는 상위 레이블 분류를 만들고, 분류 내의 각 지역(예: &quot;영국&quot; 및 &quot;일본&quot;)에 대해 다른 레이블 값을 만든 다음 레이블 값을 [입찰 단위](/help/search-social-commerce/glossary.md#a-b) 또는 상위 캠페인에 할당할 수 있습니다. 그런 다음 레이블 값을 보기와 보고서에 별도의 열로 포함하고 보고서를 다른 분류 그룹과 값으로 하위 피벗할 수 있습니다.

## 레이블 분류의 구성 요소

### 레이블 분류

각 광고주는 최상위 카테고리인 최대 30개의 레이블 분류를 가질 수 있습니다. 레이블 분류를 만들면 분류에 대한 특정 레이블 값을 만들 수 있습니다.

### 레이블 값

각 레이블 분류는 최대 2000개의 값을 가질 수 있습니다. 분류에 대한 특정 레이블 값을 만들면 캠페인, 광고 그룹, 키워드, 광고, 배치 및 제품 그룹 [캠페인 관리 보기에서](#classification-values-assign-campaign-management) 또는 [일괄 시트 사용](#classification-values-assign-bulksheets)에 할당할 수 있습니다.

각 적격 엔티티는 여러 분류에 대한 레이블 값을 가질 수 있지만 분류당 하나의 레이블 값만 가질 수 있습니다. 레이블 값은 하위 엔티티에 상속되지만 재정의할 수 있습니다. 최하위 레벨에 지정된 값은 항상 상위 레벨에 지정된 값을 대체합니다.

## 레이블 분류 보기

[!UICONTROL Reports] > [!UICONTROL Labels Classifications] 보기에는 [!UICONTROL Classifications] 및 [!UICONTROL Label Values] 하위 보기가 포함됩니다. 기본적으로 키워드 수준 레이블 분류 및 값에 대한 데이터가 표시되지만 선택적으로 광고 수준 분류 및 값에 대한 데이터를 볼 수도 있습니다.

## 사용 가능한 작업

* 레이블 분류에 대한 데이터를 봅니다.

* 레이블 분류 값에 대한 데이터를 봅니다.

* [레이블 분류를 만듭니다](#classification-create).

* 캠페인 관리 보기에서 [계정 구성 요소에 분류 값을 할당](#classification-values-assign-campaign-management) 또는 [일괄 시트를 사용](#classification-values-assign-bulksheets)합니다.

* [계정 구성 요소에서 레이블 분류 값을 제거합니다](#classification-values-remove).

* [레이블 분류 값을 삭제](#classification-values-delete)합니다.

* [레이블 분류를 삭제](#classification-delete)합니다.

## 레이블 분류 만들기 {#classification-create}

<!-- Update links to bulksheet columns once I have new files/paths -->

1. **[!UICONTROL Reports]>[!UICONTROL Label Classifications]**&#x200B;을(를) 클릭합니다.

1. 오른쪽 상단에서 **[!UICONTROL Create Classification]**&#x200B;을(를) 클릭합니다.

1. 고유한 레이블 분류 이름을 입력한 다음 **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

   이름은 광고주 계정에 대해 고유해야 하며 [ASCII 문자 32-126](https://www.asciitable.com/)&#x200B;(으)로 구성되어야 하며 최대 길이는 27개의 싱글바이트 문자입니다. 이름은 기존 보고서 열 또는 기존 일괄 시트 열의 이름과 같을 수 없습니다. [Baidu](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-baidu.md), [Google 광고](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-google.md), [Microsoft Advertising](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-microsoft.md), [Naver](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-naver.md), [Yahoo!의 일괄 시트 열 이름을 확인하세요. 일본 광고](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-yahoo-japan.md), [야후! 네트워크 표시](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-yahoo-display-network.md) 및 [Yandex](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-yandex.md).

## 캠페인 관리 보기에서 계정 구성 요소에 분류 값 할당 {#classification-values-assign-campaign-management}

캠페인 관리 보기에서 캠페인, 광고 그룹, 키워드, 광고, 배치, 단위 수준 제품 그룹 및 동적 검색 타겟과 같은 검색 엔티티에 대한 분류 값을 할당하거나 제거할 수 있습니다. 필요한 경우 발령 프로세스 중에 분류 및 분류 값을 생성할 수 있습니다. 각 레이블 분류는 최대 2000개의 값을 가질 수 있습니다.

각 엔티티는 분류당 하나의 레이블 값을 가질 수 있습니다. 예를 들어 Shoes_Campaign의 색상 값은 &quot;빨간색&quot;이고 지역 값은 &quot;Los Angeles&quot;일 수 있지만 색상 또는 지역 값을 여러 개 가질 수는 없습니다.

레이블 값은 하위 엔티티에 의해 상속되므로 상속된 값을 재정의하지 않는 한 하위 엔티티에 대한 값을 입력하지 마십시오.

>[!NOTE]
>
>일부 광고 네트워크 및 캠페인 유형의 키워드 및 광고 복사본은 [변경할 수 없음](/help/search-social-commerce/campaign-management/faqs-campaigns.md)입니다. 즉, 편집하면 기존 엔터티가 삭제되고 새 엔터티가 만들어집니다. 이러한 방식으로 기존 엔티티를 삭제하면 레이블 분류가 새 엔티티에 할당되지 않습니다.

1. **[!UICONTROL Manage]** 또는 **[!UICONTROL Target]** 메뉴에서 엔터티 보기를 엽니다.

1. 각 관련 행 옆에 있는 확인란을 선택합니다.

   여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)&quot;을 참조하십시오.

1. 일괄 작업 도구 모음에서 **+[!UICONTROL Assign]** > **[!UICONTROL Label Classification]**&#x200B;을(를) 클릭합니다.

1. 적용 가능한 각 분류 값에 대해 다음을 수행합니다.

   1. **[!UICONTROL Classifications]** 열에서 분류를 지정합니다.

      * 기존 분류를 사용하려면 분류 이름을 클릭하여 확장합니다.

      * 분류를 만들려면 열 머리글에서 [!UICONTROL +]을(를) 클릭합니다. 입력 필드에 분류 이름을 입력한 다음 ![저장](/help/search-social-commerce/assets/save-checkmark.png "저장")을 클릭하여 분류를 즉시 저장합니다. 새 분류를 사용하려면 분류 이름을 클릭하여 확장합니다.

        이름은 [ASCII 문자 32-126](https://www.asciitable.com/)&#x200B;(으)로 구성되어야 하며 최대 길이는 27개의 싱글바이트 문자입니다.

   1. **[!UICONTROL Value Name]** 열에서 선택한 분류의 값을 지정하십시오.

      * 기존 값을 사용하려면 값을 선택합니다.

      * 값을 만들려면 열 머리글에서 [!UICONTROL +]을(를) 클릭합니다. 입력 필드에 값을 입력한 다음 ![저장](/help/search-social-commerce/assets/save-checkmark.png "저장")을 클릭하여 값을 즉시 저장하고 기본적으로 선택합니다.

        최대 길이는 100자이며 ASCII 및 비 ASCII 문자를 포함할 수 있습니다.

1. **+[!UICONTROL Assign Now]**&#x200B;을(를) 클릭합니다.

## 일괄 시트를 사용하여 계정 구성 요소에 분류 값 할당 {#classification-values-assign-bulksheets}

<!-- Update bulksheet references to ones in new UI -->

일괄 시트를 사용하여 레이블 분류를 검색 엔티티에 대한 값(캠페인, 광고 그룹, 키워드, 광고, 배치, 단위 수준 제품 그룹 및 동적 검색 대상)과 연결할 수 있습니다. 각 레이블 분류는 최대 2000개의 값을 가질 수 있습니다.

각 엔티티는 분류당 하나의 레이블 값을 가질 수 있습니다. 예를 들어 Shoes_Campaign의 색상 값은 &quot;빨간색&quot;이고 지역 값은 &quot;Los Angeles&quot;일 수 있지만 색상 또는 지역 값을 여러 개 가질 수는 없습니다.

레이블 값은 하위 엔티티에 의해 상속되므로 상속된 값을 재정의하지 않는 한 하위 엔티티에 대한 값을 입력하지 마십시오.

>[!NOTE]
>
>일부 광고 네트워크 및 캠페인 유형의 키워드 및 광고 복사본은 [변경할 수 없음](/help/search-social-commerce/campaign-management/faqs-campaigns.md)입니다. 즉, 편집하면 기존 엔터티가 삭제되고 새 엔터티가 만들어집니다. 이러한 방식으로 기존 엔티티를 삭제하면 레이블 분류가 새 엔티티에 할당되지 않습니다.

1. 레이블 분류 값을 할당할 엔터티가 포함된 [일괄 시트를 다운로드합니다](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-download.md).

   * [!UICONTROL Rows and Columns] 탭에서 [!UICONTROL Bulksheet Columns] 창의 [!UICONTROL Campaign] 목록을 확장합니다.

   * [!UICONTROL Label Classification] 목록을 확장합니다.

   * 일괄 시트 파일에 열을 포함할 각 분류를 선택합니다.

     예를 들어 레이블 분류 &quot;색상&quot; 및 &quot;지역&quot;을 포함하는 경우 일괄 시트에는 &quot;색상&quot; 및 &quot;지역&quot; 열이 포함됩니다.

1. 편집기에서 파일을 열고 레이블 값을 연결할 엔티티의 레이블 분류 열에 추가합니다. 각 값의 최대 길이는 100자이며, ASCII 및 비 ASCII 문자를 포함할 수 있습니다.

   다음 섹션에서 예제 값을 참조하십시오.

   값을 추가하는 것 외에도 관련 행에서 기존 값을 제거하여 삭제할 수도 있습니다. 상위 엔티티와 하위 엔티티 모두에서 값을 제거하려면 a) 상위 엔티티 행만 포함하고 기존 분류 값을 제거하거나 b) 상위 엔티티와 하위 엔티티를 모두 포함하고 상위 및 하위 행 모두에서 기존 분류 값을 제거합니다.

1. 연결을 만들려면 [파일을 업로드](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-upload.md)합니다.<!-- Update once the new bulksheet UI is GA -->

업로드된 레이블 값은 관련 엔티티 보기에 표시됩니다.

### 일괄 시트에서 업로드할 레이블 분류 값의 예

이 예에는 레이블 분류 &quot;색상&quot; 및 &quot;지역&quot;에 대한 열이 포함되어 있습니다. 고유한 일괄 시트의 경우 열을 고유한 레이블 분류 이름으로 대체하십시오.

| 계정 | 캠페인 | 광고 그룹 | 키워드 | 광고 | 배치 | 레이블 | 색상 | 지역 |
|---|---|---|---|---|---|---|---|---|
| Acct1 | C1 | | | | | | 녹색 | |
| Acct1 | C1 | AG1 | | | | | | |
| Acct1 | C1 | AG1 | K1 | | | | | 영국 |
| Acct1 | C1 | AG1 | K2 | | | | 빨강 | AU |
| Acct1 | C1 | AG1 | K3 | | | | 파랑 | DE |
| Acct1 | C1 | AG1 | | A1 | | | | |
| Acct1 | C1 | AG1 | | A1 | | | 빨강 | |
| Acct1 | C1 | AG1 | | | P1 | | 빨강 | AU |
| Acct1 | C1 | AG1 | | | P2 | | 파랑 | DE |

## 계정 구성 요소에서 레이블 분류 값 제거 {#classification-values-remove}

분류 값을 제거하면 계정 구성 요소 및 모든 하위 구성 요소와의 연결이 제거됩니다. 분류 값에 대한 보고서 데이터는 해당 구성 요소에서 더 이상 사용할 수 없습니다. 분류 값을 제거해도 값이나 계정 구성 요소는 삭제되지 않습니다.

>[!NOTE]
>
>레이블 분류에서 값을 삭제하려면 &quot;[레이블 분류 값 삭제](#classification-values-delete)&quot;를 참조하십시오.

1. **[!UICONTROL Manage]** 또는 **[!UICONTROL Target]** 메뉴에서 엔터티 보기를 엽니다.

1. 각 관련 행 옆에 있는 확인란을 선택합니다.

   여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)&quot;을 참조하십시오.

1. 일괄 작업 도구 모음에서 **-[!UICONTROL Unassign]** > **[!UICONTROL Label Classification]**&#x200B;을(를) 클릭합니다.

1. 선택한 엔터티에서 제거할 각 분류 값 옆의 확인란을 선택합니다.<!-- As of 2/24/26, no way to tell which entity each value is assigned to -->

   할당된 모든 값을 선택하려면 **[!UICONTROL Select All]**&#x200B;을(를) 클릭하십시오. 할당된 모든 값을 선택 해제하려면 **[!UICONTROL Deselect All]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Unassign Selected]**&#x200B;을(를) 클릭합니다.

## 레이블 분류 값 삭제 {#classification-values-delete}

레이블 분류 값을 삭제하면 나중에 사용할 수 없으며, 값에 대해 보고서 데이터를 더 이상 사용할 수 없습니다. 값과 해당 상위 레이블 분류 및 특정 계정 구성 요소 사이의 모든 할당이 제거되지만 상위 레이블 분류 및 캠페인 구성 요소는 삭제되지 않습니다.

>[!NOTE]
>
>계정 구성 요소에서 분류 값의 연결을 해제하려면 &quot;[계정 구성 요소에서 레이블 분류 값 제거](#classification-values-remove)&quot;를 참조하십시오.

1. **[!UICONTROL Reports]>[!UICONTROL Label Classifications]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Label Values]** 탭을 클릭합니다.

1. (선택 사항) 특정 레이블 값을 포함하도록 목록을 필터링합니다.

1. 삭제할 각 레이블 값 옆에 있는 확인란을 선택합니다.

   한 번에 최대 200개의 행을 삭제할 수 있습니다.

   여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)&quot;을 참조하십시오.

1. 일괄 작업 도구 모음에서 ![삭제](/help/search-social-commerce/assets/delete.png "삭제")를 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

## 레이블 분류 삭제

분류를 삭제하면 하위 값과 계정 구성 요소 간의 모든 연결이 제거됩니다. 삭제된 분류 및 해당 값은 나중에 사용할 수 없습니다. 분류 값에 대한 보고서 데이터를 더 이상 사용할 수 없습니다.

>[!NOTE]
>
>계정 구성 요소에서 분류 값의 연결을 해제하려면 &quot;[계정 구성 요소에서 레이블 분류 값 제거](#classification-values-remove)&quot;를 참조하십시오.

1. **[!UICONTROL Reports]>[!UICONTROL Label Classifications]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 특정 레이블 분류를 포함하도록 목록을 필터링합니다.

1. 삭제할 각 레이블 분류 옆에 있는 확인란을 선택합니다.

   한 번에 최대 200개의 행을 삭제할 수 있습니다.

   여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)&quot;을 참조하십시오.

1. 일괄 작업 도구 모음에서 ![삭제](/help/search-social-commerce/assets/delete.png "삭제")를 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.
