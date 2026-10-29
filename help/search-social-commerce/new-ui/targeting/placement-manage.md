---
title: 배치 관리
description: Google 광고 배치 및 부정적인 배치를 만들고 관리하며 배치에 제한을 할당하는 방법을 알아봅니다.
feature: Search Optimization, Search Campaign Management
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: aed5e38a-3e62-42fa-8d16-cd080729b2a0
    internal-label: Search, Social, & Commerce
  - id: ae57d55f-b168-5358-b114-c3974b1b3d77
    internal-label: Search Optimization
  - id: 76ac9ff6-5d89-5acb-bc0b-875761bb3320
    internal-label: Search Campaign Management
subfeature_v2:
  - id: f3d33161-c519-436e-bbbd-730ba428736b
    internal-label: Campaign management
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
    internal-label: Optimization
source-git-commit: d3e38179ae119f35c184bee398edaaf456fab563
workflow-type: tm+mt
source-wordcount: '1390'
ht-degree: 0%
---
# 배치 관리

*Beta 기능*

*[!DNL Google Ads]개의 계정만*

배치는 디스플레이 네트워크에서 광고가 표시될 수 있는 위치입니다. 배치 설정에는 최대 입찰 및 선택적 추적 매개 변수가 포함됩니다. 배치 수준 설정은 광고 그룹 또는 캠페인 설정을 덮어씁니다. 네거티브 배치는 지정된 사이트에 광고가 표시되지 않도록 합니다.

[API 연결을 통해 광고 네트워크 계정에 액세스할 수 있도록 설정](/help/search-social-commerce/new-ui/manage/accounts/api-accounts/api-account-manage.md) 및 검색, 소셜 및 Commerce이 계정 데이터를 광고 네트워크와 동기화하면 디스플레이 네트워크를 대상으로 하는 [지원되는 캠페인 유형](/help/search-social-commerce/introduction/supported-inventory.md)에서 광고 그룹에 대한 배치를 만들 수 있습니다. 배치 상태를 편집 및 변경하고, 음수 배치를 생성 및 삭제할 수도 있습니다.

>[!NOTE]
>
>[!DNL Google Ads]은(는) 배치에 대한 광고 수준 성능 데이터를 제공하지 않습니다.

## [!UICONTROL Placements] 보기 정보 {#placement-view-about}

[!UICONTROL Targeting] > [!UICONTROL Placements] 보기에는 선택한 광고주 계정에 대한 두 개의 탭이 있습니다.

* [!UICONTROL Placements] 탭에는 필터링된 보기에 있는 모든 바인딩 가능한 배치가 나열됩니다.

* [!UICONTROL Negatives] 탭에는 필터링된 보기의 모든 부정적인 배치가 나열됩니다.

페이지를 보려면 [!UICONTROL View Placements] 권한이 필요합니다. 배치 또는 부정적인 배치를 만들고, 배치를 편집하고, 배치 상태를 변경하고, 배치 또는 부정적인 배치를 삭제하려면 [!UICONTROL Edit Placements] 권한이 필요합니다.

### 사용 가능한 작업

* [배치 만들기](#placement-create)

* [부정적인 배치 만들기](#placement-negative-create)

* [배치 설정 편집](#placement-edit)

* [배치 및 음수 배치의 상태 변경 또는 삭제](#placement-status)

* [선택한 행의 모든 데이터를 클립보드에 복사](#copy-to-clipboard)

* [배치에 제한 할당 및 배치에서 제한 할당 해제](#placement-constraints)

* [배치에 레이블 분류 할당](/help/search-social-commerce/new-ui/set-up/label-classifications-manage.md)

## 배치 만들기 {#placement-create}

>[!TIP]
>
>한 번에 많은 배치를 만들려면 [캠페인 일괄 시트](/help/search-social-commerce/new-ui/set-up/bulksheets/about.md)를 사용하십시오.

1. 메인 메뉴에서 **[!UICONTROL Targeting]>[!UICONTROL Placements]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Placements]** 탭에서 **[!UICONTROL Create Placement]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Basic Settings]** 단계에서 네트워크, 계정, 캠페인 및 광고 그룹을 선택합니다.

1. [배치 설정](#placement-create-settings)을 입력하십시오.

   여러 배치를 만들려면 웹 사이트 URL을 쉼표로 구분합니다.

1. **[!UICONTROL Review and Save]**&#x200B;을(를) 클릭합니다.

1. 설정을 검토합니다. 설정을 변경하려면 해당 섹션에서 ![편집](/help/search-social-commerce/assets/edit-new.png "편집") **[!UICONTROL Edit]**&#x200B;을(를) 클릭하고 설정을 변경합니다.

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

## 부정적인 배치 만들기 {#placement-negative-create}

디스플레이 네트워크를 대상으로 하는 [!DNL Google Ads] 캠페인 또는 광고 그룹에 대해 부정적인 배치를 만들 수 있습니다.

>[!NOTE]
>
>[광고 그룹 설정](/help/search-social-commerce/new-ui/manage/ad-groups/ad-group-manage.md) 및 [캠페인 설정](/help/search-social-commerce/new-ui/manage/campaigns/campaign-manage.md)에서 부정적인 배치를 만들고 편집할 수도 있습니다.

>[!TIP]
>
>한 번에 많은 수의 네거티브 배치를 만들려면 [캠페인 일괄 시트](/help/search-social-commerce/new-ui/set-up/bulksheets/about.md)를 사용하십시오.

1. 메인 메뉴에서 **[!UICONTROL Targeting]>[!UICONTROL Placements]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Negatives]** 탭에서 **[!UICONTROL Create Negative]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Campaign Negative]** 또는 **[!UICONTROL Ad Group Negative]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Basic Settings]** 단계에서 네트워크, 계정, 캠페인 및 광고 그룹을 선택합니다(광고 그룹 수준의 부정적인 배치).

1. **[!UICONTROL Manage Websites]** 단계에서 `www.example.com` 또는 `example.com/shoes`과(와) 같은 부정적인 웹 사이트 URL을 입력합니다.

   여러 URL은 쉼표로 구분하십시오. 이 양식은 주제 또는 범주 문자열이 아닌 웹 사이트 URL을 허용합니다.

1. **[!UICONTROL Review and Save]**&#x200B;을(를) 클릭합니다.

1. 설정을 검토합니다. 설정을 변경하려면 해당 섹션에서 ![편집](/help/search-social-commerce/assets/edit-new.png "편집") **[!UICONTROL Edit]**&#x200B;을(를) 클릭하고 설정을 변경합니다.

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

## 배치 설정 편집 {#placement-edit}

하나 이상의 배치에 대한 상태, 입찰, 기본 URL 및 추적 템플릿을 편집할 수 있습니다. 타겟팅된 웹 사이트 URL을 변경하거나 삭제된 배치를 편집할 수 없습니다.

>[!TIP]
>
>한 번에 많은 양의 배치 데이터를 편집하려면 [캠페인 일괄 시트](/help/search-social-commerce/new-ui/set-up/bulksheets/about.md)를 사용하세요.

1. 메인 메뉴에서 **[!UICONTROL Targeting]>[!UICONTROL Placements]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Placements]** 탭에서 편집할 각 배치 옆에 있는 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Edit Placements]** 패널에서 [배치 설정](#placement-edit-settings)을 편집합니다.

   여러 배치의 경우 변경 사항이 선택한 모든 배치에 적용됩니다. 입찰을 특정 값으로 설정하거나 특정 비율이나 금액을 한도로 증가 또는 감소시킬 수 있습니다. URL의 경우 기존 값을 바꾸거나, 텍스트를 찾아서 바꾸거나, 접두어를 추가하거나, 접미어를 추가할 수 있습니다.

   선택한 배치에서 여러 통화를 사용하는 경우 입찰 편집이 비활성화됩니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 배치 및 음수 배치 상태 변경 {#placement-status}

입찰이 가능한 활성 배치를 일시 중지하여 입찰을 비활성화할 수 있습니다. 나중에 상태를 다시 활성으로 변경하여 입찰을 다시 시작할 수 있습니다.

활성 또는 일시 중지된 배치나 음수 배치를 삭제할 수도 있습니다. 삭제된 배치는 광고 네트워크에서 삭제됩니다. 이러한 데이터는 데이터 필터에 포함할 때 계속 표시되지만 변경할 수는 없습니다.

### 배치 활성화 또는 일시 중지

1. 메인 메뉴에서 **[!UICONTROL Targeting]>[!UICONTROL Placements]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Placements]** 탭에서 선택적으로 목록을 필터링한 다음 상태를 변경할 각 배치 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Placement Details]** 섹션에서 **[!UICONTROL Status]**&#x200B;을(를) 변경합니다.

   * 일시 중지된 배치를 활성화하려면 **[!UICONTROL Active]**&#x200B;을(를) 선택하십시오.

   * 활성 배치를 일시 중지하려면 **[!UICONTROL Paused]**&#x200B;을(를) 선택하십시오.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

### 배치 또는 음수 배치 삭제

1. 메인 메뉴에서 **[!UICONTROL Targeting]>[!UICONTROL Placements]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Placements]** 또는 **[!UICONTROL Negatives]** 탭에서 선택적으로 목록을 필터링한 다음 삭제할 각 배치 또는 음수 배치 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

## 선택한 행의 모든 데이터를 클립보드에 복사 {#copy-to-clipboard}

보기에 표시되는 적용된 필터 및 열에 따라 선택한 행에 표시되는 정보를 복사합니다. 정보는 탭으로 구분된 값(TSV)으로 저장됩니다.

1. 데이터를 복사할 각 행 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Copy]**&#x200B;을(를) 클릭합니다.

## 배치에 대한 제한 할당 관리 {#placement-constraints}

캠페인, 광고 그룹, 키워드, 배치, 단위 수준 제품 그룹 및 동적 검색 타겟에 대한 입찰 제한을 할당 및 제거할 수 있습니다. 각 엔티티에는 하나의 제약조건만 있을 수 있습니다.

구속은 하위 엔티티에 의해 상속되므로 상속된 값을 재정의하지 않는 한 하위 엔티티에 대한 구속을 할당할 필요가 없습니다.

제약 조건을 할당 해제하면 계정 구성 요소 및 모든 하위 구성 요소와의 연결이 제거되며 해당 구성 요소에 대해 제약 조건에 대한 보고서 데이터를 더 이상 사용할 수 없습니다. 제한 지정을 취소해도 제한 또는 계정 구성 요소 자체는 삭제되지 않습니다.

>[!NOTE]
>
>* 나중에 변경할 수 없는 광고에 대한 키워드 또는 광고 사본을 편집하여 새 키워드 또는 광고를 만드는 경우 새 엔티티에 제약 조건이 할당되지 않습니다.
>* 활성 제한은 최적화된 레거시 키워드 수준 포트폴리오에서 할당된 입찰 단위에 대해서만 입찰을 제한합니다. 활성 포트폴리오에 있거나, 하이브리드 포트폴리오에 있거나, 포트폴리오에 없는 입찰 단위에 대해서는 무시됩니다.

### 배치에 제한 할당 {#placement-constraint-assign}

하나 이상의 배치에 단일 제한을 지정할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Targeting]>[!UICONTROL Placements]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Placements]** 탭에서 단일 제약 조건을 할당할 각 배치 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Assign]>[!UICONTROL Bid Constraint]**&#x200B;을(를) 클릭합니다.

1. 제약조건을 선택합니다.

1. **[!UICONTROL Assign Now]**&#x200B;을(를) 클릭합니다.

### 배치에서 제한 할당 해제 {#placement-constraint-unassign}

제한 지정을 취소해도 삭제되지 않습니다. 제약 조건을 삭제하여 나중에 사용할 수 없게 하려면 &quot;[검색 입찰 단위에 대한 제약 조건 관리](/help/search-social-commerce/new-ui/goals/constraints-manage.md#constraint-change-status)&quot;를 참조하십시오.

1. 메인 메뉴에서 **[!UICONTROL Targeting]>[!UICONTROL Placements]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Placements]** 탭에서 제약 조건 할당을 취소할 각 배치 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Unassign]>[!UICONTROL Bid Constraint]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

## 배치 설정 {#placement-settings}

### 배치를 만들 때 설정 {#placement-create-settings}

#### [!UICONTROL Basic Settings]

**[!UICONTROL Network]:** 광고 네트워크입니다. [!DNL Google Ads]만 지원됩니다.

**[!UICONTROL Account]:** 광고 네트워크 계정입니다.

**[!UICONTROL Campaign]:** 캠페인입니다.

**[!UICONTROL Ad Group]:** 광고 그룹입니다.

#### [!UICONTROL Placement Details]

광고가 표시될 수 있는 디스플레이 네트워크의 사이트 **[!UICONTROL Placements]:**&#x200B;개. 올바른 웹 사이트 URL(예: `www.example.com`, `example.com` 또는 `example.com/shoes`)을 입력하십시오. 여러 URL은 쉼표로 구분하십시오. URL에 물음표(`?`)를 포함할 수 없습니다.

대신 웹 사이트를 제외하려면 [!UICONTROL Targeting] > [!UICONTROL Placements] > [!UICONTROL Negatives] 탭에서 [부정적인 배치를 만들거나](#placement-negative-create) 광고 그룹 및 캠페인 설정을 사용하십시오.

**[!UICONTROL Status]:** 배치의 표시 상태: *[!UICONTROL Active]*(입찰을 사용) 또는 *[!UICONTROL Paused]*(입찰을 사용 안 함).

#### [!UICONTROL Bids]

**[!UICONTROL Bid]:**(선택 사항) 캠페인 입찰 전략에 따라 배치 기반 광고의 클릭당 최대 비용(CPC) 또는 천 단위 조회 노출당 비용(vCPM)입니다. 이 값은 광고 그룹 수준의 입찰을 무시합니다.

#### [!UICONTROL Tracking URLs]

{{$include /help/_includes/base-url-keyword-ad-sitelink.md}}

{{$include /help/_includes/base-url-google-note.md}}

{{$include /help/_includes/tracking-template-google.md}}

>[!NOTE]
>
>새 UI 만들기 양식을 사용하려면 기본 URL 및 추적 템플릿이 지정되면 `http://` 또는 `https://`(으)로 시작해야 합니다.

### 배치를 편집할 때 설정 {#placement-edit-settings}

[!UICONTROL Edit Placements] 패널은 선택한 하나 이상의 배치에 대해 다음 설정을 지원합니다. 타겟팅된 웹 사이트 URL은 변경할 수 없습니다.

#### [!UICONTROL Placement Details]

**[!UICONTROL Status]:** *[!UICONTROL Active]* 또는 *[!UICONTROL Paused]*.

#### [!UICONTROL Bid Details]

**[!UICONTROL Bid adjustment]:** 입찰가를 변경하는 방법:

* *[!UICONTROL Set to]:* 기존 입찰가를 지정된 값으로 바꿉니다.

* *[!UICONTROL Increase]:* 지정한 금액 또는 백분율만큼 기존 입찰가를 늘립니다.

* *[!UICONTROL Decrease]:* 지정한 금액 또는 백분율만큼 기존 입찰가를 줄입니다.

**[!UICONTROL Modifier type]:**(증가 또는 감소의 경우) 조정에서 *[!UICONTROL Currency]*&#x200B;을(를) 사용하는지 *[!UICONTROL Percentage]*&#x200B;을(를) 사용하는지 여부.

**[!UICONTROL Set value]:** 새 입찰 또는 조정 금액입니다. 최소값은 0.01입니다.

**[!UICONTROL Max limit]:**(증가 또는 감소의 경우, 선택 사항) 조정된 입찰에 대한 제한입니다. 증가의 경우 최대 입찰가이고 감소의 경우 최소 입찰가입니다. 최소 제한 값은 0.01입니다.

선택한 배치에서 여러 통화를 사용하는 경우 입찰 편집이 비활성화됩니다.

#### [!UICONTROL Tracking Urls]

**[!UICONTROL Base Url]**, **[!UICONTROL Tracking Template]:** 각 필드에 대해 값을 수정하는 방법을 선택하십시오.

* *[!UICONTROL Set To]:* 값을 바꿉니다. `http://` 또는 `https://`(으)로 시작하는 올바른 웹 사이트 URL을 입력하십시오.

* *[!UICONTROL Find/Replace]:* 값 내에서 지정된 텍스트를 바꿉니다. 찾을 텍스트와 대체 텍스트를 입력합니다.

* *[!UICONTROL Add Suffix]:* 값에 텍스트를 추가합니다. 접미어 텍스트를 입력합니다.

* *[!UICONTROL Add Prefix]:* 값의 시작 부분에 텍스트를 추가합니다. 접두어 텍스트를 입력합니다.

>[!NOTE]
>
>모든 새 기본 URL은 `http://` 또는 `https://`(으)로 시작하는 올바른 URL이어야 합니다.

>[!MORELIKETHIS]
>
>* [검색 입찰 단위에 대한 제약 조건 관리](/help/search-social-commerce/new-ui/goals/constraints-manage.md)
>* [레이블 분류 관리](/help/search-social-commerce/new-ui/set-up/label-classifications-manage.md)
