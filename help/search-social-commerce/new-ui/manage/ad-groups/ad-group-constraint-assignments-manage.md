---
title: 광고 그룹에 대한 제한 할당 관리
description: 광고 그룹에 제약 조건을 할당하는 방법을 알아봅니다.
feature: Search Optimization, Search Campaign Management
hide: true
exl-id: c9960b5a-4b6c-4ef0-8501-5478af2c40da
TQID: https://experienceleague.adobe.com/6z4-Pt25RaQpLiEYdnp-BXD0guz9S2zQLmamf8uSSXU
product_v2: id: a829a185-511f-4bf8-8dcf-9e684f8011cf
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c2296997-5d79-4905-b32e-99b5aa892429id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
source-git-commit: a09cdd9d882dd2f7d18eef6a2065c3c71c5ae9ee
workflow-type: tm+mt
source-wordcount: 389
ht-degree: 0%

---

# (새 UI) 광고 그룹에 대한 제한 할당 관리

*Beta 기능*

캠페인, 광고 그룹, 키워드, 배치, 단위 레벨 제품 그룹 및 동적 검색 대상 등 검색 엔티티에 대한 입찰 구속을 지정하고 제거할 수 있습니다. 각 엔티티에는 하나의 제약조건만 있을 수 있습니다.

구속은 하위 엔티티에 의해 상속되므로 상속된 값을 재정의하지 않는 한 하위 엔티티에 대한 구속을 할당할 필요가 없습니다.

제약 조건을 할당 해제하면 계정 구성 요소 및 모든 하위 구성 요소와의 연결이 제거되며 해당 구성 요소에 대해 제약 조건에 대한 보고서 데이터를 더 이상 사용할 수 없습니다. 제약 조건 할당을 취소해도 제약 조건이나 계정 구성 요소 자체는 삭제되지 않습니다.

## 새 [!UICONTROL Ad Groups] 보기에서 선택한 광고 그룹에 제한 할당

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Ad Groups]**&#x200B;을(를) 클릭합니다.

1. 단일 제한을 할당할 각 광고 그룹 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **+[!UICONTROL Assign]** > **[!UICONTROL Constraint]**&#x200B;을(를) 클릭합니다.

1. 제약조건을 선택합니다.

1. **[!UICONTROL Assign Now]**&#x200B;을(를) 클릭합니다.

## 기존 [!UICONTROL Campaigns] 보기에서 선택한 검색 입찰 단위에 제한 할당

1. **[!UICONTROL Search, Social, & Commerce]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**&#x200B;에서 계정 구성 요소 보기를 선택합니다.

1. 각 관련 행 옆에 있는 확인란을 선택합니다.

   여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)&quot;을 참조하십시오.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL More]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Assign]** > **[!UICONTROL Constraint]**&#x200B;을(를) 클릭합니다.

1. 적용 가능한 제한을 선택합니다.

1. (선택 사항) 추가 세부 정보를 입력합니다.

   1. [!UICONTROL Additional Details] 옆에 있는 **[!UICONTROL Open]**&#x200B;을(를) 클릭하여 세부 정보를 확장합니다.

   1. 선택적 **[!UICONTROL Project Name]** 및/또는 선택적 **[!UICONTROL Description]**&#x200B;을(를) 입력하십시오.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 새 [!UICONTROL Ad Groups] 보기에서 선택한 광고 그룹에서 제한 할당 해제

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Ad Groups]**&#x200B;을(를) 클릭합니다.

1. 제한을 할당 해제할 각 광고 그룹 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **-[!UICONTROL Unassign]** > **[!UICONTROL Constraint]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

## 기존 [!UICONTROL Campaigns] 보기에서 검색 입찰 단위의 제한 할당 해제

>[!NOTE]
>
>제약 조건을 삭제하여 나중에 사용할 수 없게 하려면 Search, Social 및 Commerce 내에서 사용할 수 있는 &quot;입찰 제한&quot;에 대한 최적화 안내서 장의 &quot;검색 입찰 단위에 대한 제약 조건 삭제&quot;를 참조하십시오.<!-- verify convention for referencing Optimization Guide here -->

1. **[!UICONTROL Search, Social, & Commerce]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**&#x200B;에서 계정 구성 요소 보기를 선택합니다.

1. 구속을 제거할 각 컴포넌트 옆의 확인란을 선택합니다.

   여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)&quot;을 참조하십시오.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL More]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Unassign]** > **[!UICONTROL Constraint]**&#x200B;을(를) 클릭합니다.

1. 확인 대화 상자에서 **[!UICONTROL Yes, Unassign]**&#x200B;을(를) 선택합니다.

>[!MORELIKETHIS]
>
>* [(새 UI) 검색 입찰 단위에 대한 제약 조건을 관리합니다](/help/search-social-commerce/new-ui/goals/constraints-manage.md)
>* [(새 UI) 캠페인에 대한 제한 할당 관리](/help/search-social-commerce/new-ui/manage/campaigns/campaign-constraint-assignments-manage.md)
>* [(새 UI) 키워드에 대한 제약 조건 할당 관리](/help/search-social-commerce/new-ui/target/keywords/keyword-constraint-assignments-manage.md)
>* [(새 UI) 배치에 대한 제한 할당 관리](/help/search-social-commerce/new-ui/target/placements/placement-constraint-assignments-manage.md)
