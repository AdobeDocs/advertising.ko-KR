---
title: 캠페인 관리
description: 광고 캠페인을 만들고 관리하는 방법을 알아봅니다.
feature: Search Campaign Management
product_v2: id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2: id: aed5e38a-3e62-42fa-8d16-cd080729b2a0
subfeature_v2: id: f3d33161-c519-436e-bbbd-730ba428736b
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 7dc3ea3fe1fcb701d9d064b184922ed96626cd4a
workflow-type: tm+mt
source-wordcount: 2285
ht-degree: 0%

---

# 캠페인 관리

*Beta 기능*

캠페인은 광고 네트워크 계정의 기본 구성 요소입니다. 대부분의 캠페인 유형의 경우, 광고 그룹 또는 광고 세트 세트로 구성됩니다. 캠페인 설정에는 캠페인 예산 매개 변수, 광고 타겟 및 캠페인의 모든 광고에 대한 선택적 추적 매개 변수가 포함됩니다. 캠페인 수준 추적 매개 변수는 계정 수준 매개 변수를 재정의하지만, 그 자체가 더 낮은 수준에서 재정의될 수 있습니다.

[API 연결을 통해 광고 네트워크 계정에 액세스할 수 있도록 설정](/help/search-social-commerce/new-ui/set-up/accounts/api-accounts/api-account-manage.md) 및 검색, 소셜 및 Commerce이 계정 데이터를 광고 네트워크와 동기화하면 [지원되는 캠페인 유형](/help/search-social-commerce/introduction/supported-inventory.md)을 사용하여 새 캠페인을 만들 수 있습니다. 캠페인의 상태를 편집하고 변경할 수도 있습니다.

각 광고 네트워크에서 사용할 수 있는 기능에 대한 자세한 내용은 &quot;[지원되는 인벤토리](/help/search-social-commerce/introduction/supported-inventory.md)&quot;를 참조하십시오.

## [!UICONTROL Campaigns] 보기 정보 {#campaign-view-about}

[!UICONTROL Manage] > [!UICONTROL Campaigns] 보기는 선택한 광고주 계정에 대해 필터링된 보기의 모든 캠페인을 나열합니다. 캠페인 이름을 클릭하여 캠페인에서 광고 그룹 목록을 열 수 있습니다.

[!UICONTROL Campaigns] 보기에서 캠페인 데이터를 추가하고 편집하면 검색, 소셜 및 Commerce이 데이터 변경 내용을 광고 네트워크에 즉시 푸시합니다. 또한 검색, 소셜 및 Commerce은 캠페인 구조 데이터를 가져오고 매일 또는 새 캠페인이 감지되면 더 자주 데이터를 클릭합니다. 동기화된 모든 광고 네트워크의 경우 필요에 따라 온디맨드로 계정을 동기화할 수도 있습니다.

Search, Social 및 Commerce은 동기화된 [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 계정에서 매시간 성능 데이터를 가져오고, 동기화된 다른 광고 네트워크 계정에 대해서는 매일 성능 데이터를 가져옵니다.

### 사용 가능한 작업

* [캠페인 만들기](#campaign-create)

* [행 내에서 캠페인 이름 바꾸기](#campaign-rename)

* [캠페인 설정 편집](#campaign-edit)

* [행 내에서 캠페인 상태 변경 또는 삭제](#campaign-status)

* [포트폴리오에 캠페인을 할당하고 포트폴리오에서 캠페인을 제거합니다.](#campaign-portfolio)

* [[!UICONTROL Campaigns] 보기에서 성능 그래프 보기](#campaign-performance-graph)

* [캠페인에 입찰 제한 할당 및 캠페인에서 제한 할당 해제](#campaign-constraints)

* [캠페인에 대상 제한 할당 및 캠페인에서 대상 제한 할당 해제](#campaign-target-constraints)

* [캠페인에 레이블 분류를 할당하고 캠페인에서 레이블 분류를 제거합니다.](#campaign-classifications)

* [[!UICONTROL Campaigns] 보기에서 데이터 보기 보고서 관리](#campaign-reports)

## 캠페인 만들기 {#campaign-create}

>[!NOTE]
>
>* 캠페인을 만들기 전에 광고주의 웹 페이지에서 [전환 추적 태그를 구현](/help/search-social-commerce/tracking/conversion-tracking-about.md)하십시오.
>* 한 번에 많은 캠페인을 만들려면 <!-- Not available in new UI as of 7/21: the [copy and paste feature](/help/search-social-commerce/campaign-management/campaigns/copy-paste.md) or-->을(를) 사용합니다. [캠페인 일괄 시트](/help/search-social-commerce/new-ui/set-up/bulksheets/about.md).

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Create Campaign]**&#x200B;을(를) 클릭합니다.

1. [Baidu](/help/search-social-commerce/new-ui/manage/campaigns/campaign-settings/campaign-settings-baidu.md), [Google 광고](/help/search-social-commerce/new-ui/manage/campaigns/campaign-settings/campaign-settings-google.md), [LY 광고](/help/search-social-commerce/new-ui/manage/campaigns/campaign-settings/campaign-settings-yahoo-japan.md), [Microsoft Advertising](/help/search-social-commerce/new-ui/manage/campaigns/campaign-settings/campaign-settings-microsoft.md) 또는 [Yandex](/help/search-social-commerce/new-ui/manage/campaigns/campaign-settings/campaign-settings-yandex.md) 캠페인 설정을 지정합니다.

1. **[!UICONTROL Review and Save]**&#x200B;을(를) 클릭합니다.

1. 필요한 경우 ![편집](/help/search-social-commerce/assets/edit-new.png "편집")을 클릭하고 캠페인 설정을 변경합니다.

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

캠페인을 만든 광고 네트워크에 따라, 캠페인이 광고 네트워크에 푸시되기 전에 연결된 광고 그룹 및 광고를 만들어야 할 수 있습니다.

## 캠페인 이름 바꾸기 {#campaign-rename}

전체 캠페인 설정을 열지 않고 캠페인 이름을 빠르게 변경합니다.

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 캠페인 행 위에 커서를 놓고 **[!UICONTROL ...]>[!UICONTROL Rename]**&#x200B;을(를) 클릭합니다.

1. 이름을 편집한 다음 **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

## 캠페인 설정 편집 {#campaign-edit}

개별 캠페인에 대한 설정을 편집할 수 있습니다. 선택한 모든 캠페인에 공통되는 일부 캠페인 세부 사항, 예산 옵션 및 URL 옵션을 포함하여 여러 캠페인에 대한 일부 필드를 한 번에 편집할 수도 있습니다.

>[!TIP]
>
><!-- Not available in new UI as of 7/21: the [copy and paste feature](/help/search-social-commerce/campaign-management/campaigns/copy-paste.md) or-->을(를) 사용하여 데이터를 일괄 편집할 수도 있습니다. [캠페인 일괄 시트](/help/search-social-commerce/new-ui/set-up/bulksheets/about.md).

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * 엔터티 이름 위에 커서를 놓고 **[!UICONTROL ...]>[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

   * 캠페인 옆에 있는 확인란을 선택합니다. 일괄 작업 도구 모음에서 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. [Baidu](/help/search-social-commerce/new-ui/manage/campaigns/campaign-settings/campaign-settings-baidu.md), [Google 광고](/help/search-social-commerce/new-ui/manage/campaigns/campaign-settings/campaign-settings-google.md), [LY 광고](/help/search-social-commerce/new-ui/manage/campaigns/campaign-settings/campaign-settings-yahoo-japan.md), <!-- [Meta Ads](/help/search-social-commerce/new-ui/manage/campaigns/campaign-settings/campaign-settings-meta.md), --> 편집 [Microsoft Advertising](/help/search-social-commerce/new-ui/manage/campaigns/campaign-settings/campaign-settings-microsoft.md) 또는 [Yandex](/help/search-social-commerce/new-ui/manage/campaigns/campaign-settings/campaign-settings-yandex.md) 캠페인 설정.

1. **[!UICONTROL Review and Save]**&#x200B;을(를) 클릭합니다.

1. 필요한 경우 ![편집](/help/search-social-commerce/assets/edit-new.png "편집")을 클릭하고 캠페인 설정을 변경합니다.

1. **[!UICONTROL Update]**&#x200B;을(를) 클릭합니다.

캠페인을 만든 광고 네트워크에 따라, 광고 네트워크에 푸시하기 전에 캠페인에 광고 그룹 및 광고를 포함해야 할 수도 있습니다.

## 캠페인 상태 변경 {#campaign-status}

전체 캠페인 설정을 열지 않고도 캠페인의 상태를 빠르게 변경할 수 있습니다.

지원되는 광고 네트워크에서 활성 캠페인을 일시 중지하여 입찰을 비활성화할 수 있습니다. 나중에 상태를 다시 활성으로 변경하여 입찰을 다시 시작할 수 있습니다.

활성 캠페인이나 일시 중지된 캠페인을 삭제할 수도 있습니다. 삭제된 캠페인은 광고 네트워크에서 삭제됩니다. 이러한 데이터는 데이터 필터에 포함할 때 계속 표시되지만 변경할 수는 없습니다.

### 캠페인 활성화 또는 일시 중지

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 캠페인 행 위에 커서를 놓고 [!UICONTROL Status] 열 옆에 있는 ![편집](/help/search-social-commerce/assets/edit.png "편집")을 클릭합니다.

1. 상태 변경:

   * 일시 중지된 캠페인을 활성화하려면 **[!UICONTROL Active]**&#x200B;을(를) 선택하십시오.

   * 활성 캠페인을 일시 중지하려면 **[!UICONTROL Paused]**&#x200B;을(를) 선택하십시오.

### 캠페인 삭제

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * 캠페인 행 위에 커서를 놓고 **[!UICONTROL ...]>[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

   * 캠페인 행 위에 커서를 놓고 [!UICONTROL Status] 열 옆에 있는 ![편집](/help/search-social-commerce/assets/edit.png "편집")을 클릭합니다. **[!UICONTROL Deleted]**&#x200B;을(를) 선택합니다.

## 포트폴리오에 캠페인 할당 {#campaign-portfolio}

최적화된 포트폴리오에 캠페인을 할당하면 검색, 소셜 및 Commerce에서 캠페인의 키워드 및 광고에 대한 입찰, 캠페인 예산 및 입찰 전략 타겟을 최적화할 수 있습니다. 포트폴리오를 만들 때 또는 포트폴리오의 설정을 편집하여 [!UICONTROL Campaigns] 보기에서 포트폴리오에 캠페인을 할당할 수 있습니다.

일부 캠페인 유형 및 광고 네트워크는 최적화할 수 없습니다. 포트폴리오에 포함할 수 있는 [지원되는 캠페인 유형](/help/search-social-commerce/introduction/supported-inventory.md) 목록을 참조하세요. 또한 [각 캠페인 입찰 전략에 대한 최적화 지원을 확인](/help/search-social-commerce/new-ui/manage/portfolios/portfolio-about.md#optimization-by-bid-strategy)하십시오.

>[!NOTE]
>
>각 캠페인은 하나의 포트폴리오에만 할당할 수 있습니다. 이미 다른 포트폴리오와 연결된 캠페인을 새 포트폴리오에 할당하면 원래 포트폴리오에서 제거됩니다.

### [!UICONTROL Campaigns] 보기에서 기존 포트폴리오에 캠페인 할당

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 각 캠페인 옆의 확인란을 선택하여 단일 포트폴리오에 할당합니다.

1. 일괄 작업 도구 모음에서 **+[!UICONTROL Assign]** > **[!UICONTROL Existing Portfolio]** 을(를) 클릭합니다.

1. 포트폴리오를 선택합니다.

1. **[!UICONTROL Assign Now]**&#x200B;을(를) 클릭합니다.

### [!UICONTROL Campaigns] 보기에서 새 포트폴리오에 캠페인 할당

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 새 포트폴리오를 만들려는 각 캠페인 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **+[!UICONTROL Assign]** > **[!UICONTROL New Portfolio]**&#x200B;을(를) 클릭합니다.

1. [!UICONTROL Create Portfolio] 화면에서 포트폴리오 설정을 지정합니다.

   이전에 선택한 캠페인은 이미 캠페인에 할당되어 있습니다. 포트폴리오에 대한 캠페인 목록을 선택적으로 편집할 수 있습니다.

   포트폴리오 설정에 대한 자세한 내용은 Search, Social 및 Commerce 내에서 사용할 수 있는 최적화 안내서를 참조하십시오.

1. **[!UICONTROL Review and Save]**&#x200B;을(를) 클릭합니다.

### [!UICONTROL Portfolios] 보기에서 포트폴리오에 대한 캠페인 할당 변경

포트폴리오에서 캠페인을 제거하면 검색, 소셜 및 Commerce에서 해당 캠페인에 대한 입찰, 캠페인 예산 및 입찰 전략 타겟을 최적화할 수 없습니다.

작업은 포트폴리오의 변경 내역에 기록됩니다.

최적화에 대한 자세한 내용은 Search, Social 및 Commerce 내에서 사용할 수 있는 최적화 안내서를 참조하십시오.

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Portfolios]**&#x200B;을(를) 클릭합니다.

1. 포트폴리오 옆에 있는 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. 포트폴리오 설정에서 [!UICONTROL Assign Campaigns] 섹션으로 이동하여 캠페인 할당을 변경합니다.

   포트폴리오 설정에 대한 자세한 내용은 Search, Social 및 Commerce 내에서 사용할 수 있는 최적화 안내서를 참조하십시오.

1. **[!UICONTROL Review and Save]**&#x200B;을(를) 클릭합니다.

1. 설정을 검토하고 필요에 따라 변경한 다음 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 캠페인에 대한 입찰 제한 할당 관리 {#campaign-constraints}

각 엔티티에는 하나의 제약조건만 있을 수 있습니다. 구속은 하위 엔티티에 의해 상속되므로 상속된 값을 재정의하지 않는 한 하위 엔티티에 대한 구속을 할당할 필요가 없습니다.

제약 조건을 할당 해제하면 계정 구성 요소 및 모든 하위 구성 요소와의 연결이 제거되며 해당 구성 요소에 대해 제약 조건에 대한 보고서 데이터를 더 이상 사용할 수 없습니다. 제약 조건 할당을 취소해도 제약 조건이나 계정 구성 요소 자체는 삭제되지 않습니다.

>[!NOTE]
>
>활성 제한은 최적화된 레거시 키워드 수준 포트폴리오에서 할당된 입찰 단위에 대해서만 입찰을 제한합니다. 활성 포트폴리오에 있거나, 하이브리드 포트폴리오에 있거나, 포트폴리오에 없는 입찰 단위에 대해서는 무시됩니다.

### 새 [!UICONTROL Campaigns] 보기에서 선택한 캠페인에 입찰 제한 할당

하나 이상의 캠페인에 단일 제한을 할당할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 단일 제한을 할당할 각 캠페인 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **+[!UICONTROL Assign]** > **[!UICONTROL Constraint]**&#x200B;을(를) 클릭합니다.

1. 제약조건을 선택합니다.

1. **[!UICONTROL Assign Now]**&#x200B;을(를) 클릭합니다.

### 기존 [!UICONTROL Campaigns] 보기에서 선택한 검색 입찰 단위에 입찰 제한 할당

1. **[!UICONTROL Search, Social, & Commerce]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**&#x200B;에서 계정 구성 요소 보기를 선택합니다.

1. 각 관련 행 옆에 있는 확인란을 선택합니다.

   여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)&quot;을 참조하십시오.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL More]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Assign]** > **[!UICONTROL Constraint]**&#x200B;을(를) 클릭합니다.

1. 적용 가능한 제한을 선택합니다.

1. (선택 사항) 추가 세부 정보를 입력합니다.

   1. [!UICONTROL Additional Details] 옆에 있는 **[!UICONTROL Open]**&#x200B;을(를) 클릭하여 세부 정보를 확장합니다.

   1. 선택적 **[!UICONTROL Project Name]** 및/또는 선택적 **[!UICONTROL Description]**&#x200B;을(를) 입력하십시오.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

### 새 [!UICONTROL Campaigns] 보기에서 선택한 캠페인에서 입찰 제한 제거

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 제한을 할당 해제할 각 캠페인 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **-[!UICONTROL Unassign]** > **[!UICONTROL Constraint]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

### 기존 [!UICONTROL Campaigns] 보기의 입찰 단위 검색에서 입찰 제한 제거

>[!NOTE]
>
>제약 조건을 삭제하여 나중에 사용할 수 없게 하려면 Search, Social 및 Commerce 내에서 사용할 수 있는 &quot;입찰 제한&quot;에 대한 최적화 안내서 장의 &quot;검색 입찰 단위에 대한 제약 조건 삭제&quot;를 참조하십시오.<!-- verify convention for referencing Optimization Guide here -->

1. **[!UICONTROL Search, Social, & Commerce]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**&#x200B;에서 계정 구성 요소 보기를 선택합니다.

1. 구속을 제거할 각 컴포넌트 옆의 확인란을 선택합니다.

   여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)&quot;을 참조하십시오.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL More]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Unassign]** > **[!UICONTROL Constraint]**&#x200B;을(를) 클릭합니다.

1. 확인 대화 상자에서 **[!UICONTROL Yes, Unassign]**&#x200B;을(를) 선택합니다.

## 캠페인에 대한 대상 제한 할당 관리 {#campaign-target-constraints}

### 새 [!UICONTROL Campaigns] 보기에서 선택한 캠페인에 대상 제한 할당

하나 이상의 캠페인에 단일 타겟 제한을 할당할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 단일 타겟 제한을 할당할 각 캠페인 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **+[!UICONTROL Assign]** > **[!UICONTROL Target Constraint]**&#x200B;을(를) 클릭합니다.

1. 제약조건을 선택합니다.

1. **[!UICONTROL Assign Now]**&#x200B;을(를) 클릭합니다.

### 새 [!UICONTROL Campaigns] 보기에서 선택한 캠페인에서 대상 제약 조건 제거

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 대상 제약 조건을 할당 해제할 각 캠페인 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **-[!UICONTROL Unassign]** > **[!UICONTROL Target Constraint]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

## 캠페인에 레이블 분류 지정 {#campaign-classifications}

>[!NOTE]
>
>레이블 값은 하위 엔티티에 의해 상속되므로 상속된 값을 재정의하지 않는 한 하위 엔티티에 대한 값을 입력하지 마십시오.

### 캠페인에 분류 값 할당

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 레이블 값을 할당할 각 캠페인 옆의 확인란을 선택합니다.

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

### 캠페인에서 레이블 분류 값 제거

분류 값을 제거하면 계정 구성 요소 및 모든 하위 구성 요소와의 연결이 제거됩니다. 분류 값에 대한 보고서 데이터는 해당 구성 요소에서 더 이상 사용할 수 없습니다. 분류 값을 제거해도 값이나 계정 구성 요소는 삭제되지 않습니다.

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 레이블 값을 제거할 각 캠페인 옆의 확인란을 선택합니다.

   여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)&quot;을 참조하십시오.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Unassign]** > **[!UICONTROL Label Classification]**&#x200B;을(를) 클릭합니다.

1. 선택한 엔티티에서 제거할 각 분류 값 옆의 확인란을 선택합니다.

   할당된 모든 값을 선택하려면 **[!UICONTROL Select All]**&#x200B;을(를) 클릭하십시오. 할당된 모든 값을 선택 해제하려면 **[!UICONTROL Deselect All]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Unassign Selected]**&#x200B;을(를) 클릭합니다.

## [!UICONTROL Campaigns] 보기에서 성능 그래프 보기 {#campaign-performance-graph}

지정된 날짜 범위 동안 보기의 모든 캠페인에서 총 3개의 지표를 사용하여 성능 그래프를 열고 구성합니다.

### 성능 그래프 보기

1. 데이터 테이블 위에서 ![차트](/help/search-social-commerce/assets/charts.png "차트")를 클릭합니다.

1. (선택 사항) 차트에 포함할 통화 및 최대 3개의 지표를 지정합니다.

### 표시되는 성능 그래프 숨기기

* 데이터 테이블 위에서 ![차트](/help/search-social-commerce/assets/charts.png "차트")를 클릭합니다.

## [!UICONTROL Campaigns] 보기에서 데이터 보기 보고서 관리 {#campaign-reports}

<!-- Wording??????  Filtered data reports? -->

[!UICONTROL Campaigns] 보기에서 하나 이상의 캠페인에 대한 데이터 행을 포함하는 보고서를 생성한 다음 이 보고서를 Microsoft Excel 워크시트 파일(XLXS 형식)로 다운로드합니다. 이 보고서에는 보기에 표시된 모든 열이 포함됩니다.

생성된 보고서는 삭제할 수 있습니다.

&quot;>* [(기존 UI) 캠페인 관리 보기에서 데이터 다운로드](/help/search-social-commerce/common-tasks/navigation-editing-selection/download.md)&quot; 및 &quot;[(기존 UI) [!UICONTROL Downloads] 메뉴에서 성능 데이터 보고서 또는 일괄 시트 파일 삭제](/help/search-social-commerce/common-tasks/navigation-editing-selection/download-delete-data.md)&quot;도 참조하십시오.

### 필터링된 데이터 행으로 보고서 생성

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 다운로드하려는 데이터의 캠페인을 지정합니다.

   * 특정 캠페인에 대한 데이터를 다운로드하려면 캠페인 옆에 있는 확인란을 선택합니다.

   * 모든 캠페인에 대한 데이터를 다운로드하려면 확인란을 선택할 필요가 없습니다. 기본적으로 모든 캠페인이 포함됩니다.

1. 데이터 테이블 위의 도구 모음에서 ![보고서 다운로드](/help/search-social-commerce/assets/download.png "보고서 다운로드") **[!UICONTROL Reports]**&#x200B;를 클릭합니다.

1. [!UICONTROL Grid Reports] 설정에서 고유한 보고서 이름을 입력한 다음 **[!UICONTROL Generate]**&#x200B;을(를) 클릭합니다.

   기본적으로 파일 이름은 &quot;campaign_YYYYMMDD_NNNN&quot;입니다. 여기서 &quot;NNNN&quot;은 순차적 작업 번호입니다(예: &quot;campaign_20250402_1326).

   파일이 [!UICONTROL Recently Generated] 목록에 추가됩니다.

1. (선택 사항) 파일이 완료되면 다운로드하려면 파일 이름 옆에 있는 ![다운로드](/help/search-social-commerce/assets/download.png "다운로드")를 클릭합니다.

   브라우저의 일반적인 절차에 따라 파일이 다운로드됩니다.

### 완료된 보고서 다운로드

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위의 도구 모음에서 ![보고서 다운로드](/help/search-social-commerce/assets/download.png "보고서 다운로드") **[!UICONTROL Reports]**&#x200B;를 클릭합니다.

1. [!UICONTROL Grid Reports] 대화 상자의 [!UICONTROL Recently Generated] 목록에서 파일 이름 옆에 있는 ![다운로드](/help/search-social-commerce/assets/download.png "다운로드")를 클릭합니다.

   브라우저의 일반적인 절차에 따라 파일이 다운로드됩니다.

### 완료된 보고서 삭제

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위의 도구 모음에서 ![보고서 다운로드](/help/search-social-commerce/assets/download.png "보고서 다운로드") **[!UICONTROL Reports]**&#x200B;를 클릭합니다.

1. [!UICONTROL Grid Reports] 대화 상자의 [!UICONTROL Recently Generated] 목록에서 파일 이름 옆에 있는 ![삭제](/help/search-social-commerce/assets/delete-new.png "삭제")를 클릭합니다.

>[!MORELIKETHIS]
>
>* [검색 입찰 단위에 대한 제약 조건 관리](/help/search-social-commerce/new-ui/goals/constraints-manage.md)
>* [광고 그룹에 대한 제약 조건 할당 관리](/help/search-social-commerce/new-ui/manage/ad-groups/ad-group-constraint-assignments-manage.md)
>* [키워드에 대한 제약 조건 할당 관리](/help/search-social-commerce/new-ui/target/keywords/keyword-constraint-assignments-manage.md)
>* [배치에 대한 제한 할당 관리](/help/search-social-commerce/new-ui/target/placements/placement-constraint-assignments-manage.md)
>* [(레거시 UI) 캠페인 관리 보기에서 데이터를 다운로드합니다](/help/search-social-commerce/common-tasks/navigation-editing-selection/download.md)
>* [(기존 UI) [!UICONTROL Downloads] 메뉴에서 성능 데이터 보고서 또는 일괄 시트 파일을 삭제합니다.](/help/search-social-commerce/common-tasks/navigation-editing-selection/download-delete-data.md)
>* [[!DNL Baidu] 캠페인 설정](/help/search-social-commerce/new-ui/manage/campaigns/campaign-settings/campaign-settings-baidu.md)
>* [[!DNL Google Ads] 캠페인 설정](/help/search-social-commerce/new-ui/manage/campaigns/campaign-settings/campaign-settings-google.md)
>* [[!DNL LY Ads] 캠페인 설정](/help/search-social-commerce/new-ui/manage/campaigns/campaign-settings/campaign-settings-yahoo-japan.md)
>* [[!DNL Microsoft Advertising] 캠페인 설정](/help/search-social-commerce/new-ui/manage/campaigns/campaign-settings/campaign-settings-microsoft.md)
>* [[!DNL Yandex] 캠페인 설정](/help/search-social-commerce/new-ui/manage/campaigns/campaign-settings/campaign-settings-yandex.md)

<!-- >* [[!DNL Meta Ads] campaign settings](/help/search-social-commerce/new-ui/manage/campaigns/campaign-settings/campaign-settings-meta.md) -->

