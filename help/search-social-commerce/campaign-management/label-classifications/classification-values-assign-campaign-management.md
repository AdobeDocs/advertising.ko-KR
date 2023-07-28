---
title: 캠페인 관리 보기에서 계정 구성 요소에 분류 값 할당
description: 계정 구성 요소에 분류 값을 할당하는 방법을 알아봅니다.
exl-id: 7e55d7d8-5e12-409b-ad5d-c53cbf24c7c9
feature: Search Label Classifications
source-git-commit: 052574217d7ddafb8895c74094da5997b5ff83db
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# 캠페인 관리 보기에서 계정 구성 요소에 분류 값 할당

캠페인 관리 보기에서 캠페인, 광고 그룹, 키워드, 광고, 배치, 단위 수준 제품 그룹 및 동적 검색 타겟과 같은 검색 엔티티에 대한 분류 값을 할당하거나 제거할 수 있습니다. 필요한 경우 발령 프로세스 중에 분류 및 분류 값을 생성할 수 있습니다. 각 레이블 분류는 최대 2000개의 값을 가질 수 있습니다.

각 엔티티는 분류당 하나의 레이블 값을 가질 수 있습니다. 예를 들어 Shoes_Campaign의 색상 값은 &quot;빨간색&quot;이고 지역 값은 &quot;Los Angeles&quot;일 수 있지만 색상 또는 지역 값을 여러 개 가질 수는 없습니다.

레이블 값은 하위 엔티티에 의해 상속되므로 상속된 값을 재정의하지 않는 한 하위 엔티티에 대한 값을 입력하지 마십시오.

>[!NOTE]
>
>일부 광고 네트워크 및 캠페인 유형에 대한 키워드 및 광고 사본은 다음과 같습니다 [변경할 수 없음](/help/search-social-commerce/campaign-management/faqs-campaigns.md)를 지정하면 기존 엔티티가 삭제되고 새 엔티티가 만들어집니다. 이러한 방식으로 기존 엔티티를 삭제하면 레이블 분류가 새 엔티티에 할당되지 않습니다.

1. 클릭 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**&#x200B;을 선택한 다음 계정 구성 요소 보기를 선택합니다.

1. 다음 중 하나를 수행합니다.

   * (단일 엔티티에 값을 할당하려면) 엔티티 이름 위에 커서를 놓고 ![메뉴 단추](/help/search-social-commerce/assets/arrow-dropdown-menu.png "메뉴 단추")을 선택한 다음 을 선택합니다 **[!UICONTROL Classification]**.

   * (하나 이상의 엔티티에 값을 할당하려면 다음을 수행합니다.

      * 각 관련 행 옆에 있는 확인란을 선택합니다.

        여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md).&quot;

      * 데이터 테이블 위의 도구 모음에서 ![자세히](/help/search-social-commerce/assets/more.png "자세히")을 클릭한 다음 을 클릭합니다 **[!UICONTROL Classification]**.

1. 다음에서 [!UICONTROL Assignment Details]을 클릭하고, 다음 중 하나를 수행합니다.

   * 기존 분류 값을 새 값으로 변경하려면 다음을 선택합니다 **[!UICONTROL Set To]**.

     각 값의 최대 길이는 100자이며, ASCII 및 비 ASCII 문자를 포함할 수 있습니다.

   * 기존 값을 제거하지 않고 지정된 분류 값을 할당하려면 **[!UICONTROL Assign]**.

   * 현재 지정된 특정 분류 값을 제거하려면 다음을 선택합니다. **[!UICONTROL Remove]**.

     분류 값을 제거하면 지정된 계정 구성 요소에서 해당 값에 대한 보고서 데이터를 더 이상 사용할 수 없습니다.

   * 지정된 분류 값을 삭제하려면 **[!UICONTROL Delete]**.

     분류 값을 삭제하면 나중에 사용할 수 없으며 보고서 데이터는 더 이상 값에 사용할 수 없습니다. 값과 특정 계정 구성 요소 사이의 모든 할당이 제거되지만 계정 구성 요소는 삭제되지 않습니다.

1. 적용 가능한 각 분류 값에 대해 다음을 수행합니다.

   1. 다음에서 **[!UICONTROL Classification]** 열에서 분류 이름을 지정합니다.

      * 기존 분류를 사용하려면 분류 이름을 클릭하여 확장합니다.

      * 분류를 만들려면 [!UICONTROL +]. 입력 필드에 분류 이름을 입력한 다음 을 클릭합니다. ![저장](/help/search-social-commerce/assets/select.png "저장") 분류를 즉시 저장합니다.

        이름은 다음으로 구성되어야 합니다. [32-126](https://www.asciitable.com/), 최대 길이는 27개의 1바이트 문자입니다.

   1. 다음에서 **[!UICONTROL Value Name]** 열에서 값의 이름을 지정합니다.

      * 기존 값을 사용하려면 값 이름을 클릭하여 선택합니다.

      * 값을 만들려면 [!UICONTROL +]. 입력 필드에 값을 입력한 다음 ![저장](/help/search-social-commerce/assets/select.png "저장") 값을 즉시 저장합니다.

        최대 길이는 100자이며 ASCII 및 비 ASCII 문자를 포함할 수 있습니다.

1. (선택 사항) 추가 세부 정보를 입력합니다.

   1. 다음 **[!UICONTROL Additional Details]**, 클릭 ![열기](/help/search-social-commerce/assets/chevron-up.png "열기") 을 클릭하여 세부 정보를 확장합니다.

   1. 선택 사항 입력 **[!UICONTROL Project Name]** 및/또는 선택 사항 **[!UICONTROL Description]**.

1. 클릭 **[!UICONTROL Save]**.

>[!MORELIKETHIS]
>
>* [레이블 분류 정보](classification-about.md)
>* [레이블 분류 만들기](classification-create.md)
>* [일괄 시트를 사용하여 계정 구성 요소에 분류 값 할당](classification-values-assign-bulksheets.md)
>* [계정 구성 요소에서 레이블 분류 값 제거](classification-values-remove.md)
>* [레이블 분류 값 삭제](classification-values-delete.md)
>* [레이블 분류 삭제](classification-delete.md)
