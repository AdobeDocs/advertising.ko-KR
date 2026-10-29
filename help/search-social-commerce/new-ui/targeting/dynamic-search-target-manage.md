---
title: '[!DNL Google Ads]개의 동적 검색 대상 관리'
description: '[!DNL Google Ads] 동적 검색 대상을 만들고 관리하는 방법을 알아봅니다.'
exl-id: 5ea68cab-677f-4c7e-8776-24d6546f0b15
feature: Search Campaign Management
TQID: 'https://experienceleague.adobe.com/MsSy-p-WSroc3FyiHx6kvcTohEaWOqJCzqbl91mNwK0'
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: aed5e38a-3e62-42fa-8d16-cd080729b2a0
    internal-label: Search, Social, & Commerce
  - id: 76ac9ff6-5d89-5acb-bc0b-875761bb3320
    internal-label: Search Campaign Management
subfeature_v2:
  - id: f3d33161-c519-436e-bbbd-730ba428736b
    internal-label: Campaign management
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: f907f445c70ce64368dfa7e77d4cd1900ecc7113
workflow-type: tm+mt
source-wordcount: '1504'
ht-degree: 0%
---
# [!DNL Google Ads]개의 동적 검색 대상 관리

*[!DNL Google Ads]개의 계정만*

검색 네트워크를 사용하는 [!DNL Google Ads] 캠페인에 대한 동적 검색 대상의 상태를 만들고 편집하고 변경할 수 있습니다.

## 동적 검색 대상이란 무엇입니까?

동적 검색 타겟은 광고 네트워크가 웹 사이트의 모든 페이지를 사용하는지 또는 페이지의 하위 집합을 사용하여 동적 검색 광고를 타깃팅하는지 여부를 정의합니다. 광고 그룹 수준에서 동적 검색 대상을 구성합니다. 동일한 광고 그룹의 모든 동적 검색 광고에 적용됩니다.

캠페인 설정에 따라 동적 검색 타겟이 필요하거나 선택 사항일 수 있습니다.

* 캠페인의 &quot;[!UICONTROL DSA Options]&quot; 섹션에 웹 사이트 도메인과 언어를 지정하지 않은 경우 동적 검색 대상을 만들어야 합니다.

* 캠페인의 &quot;[!UICONTROL DSA Options]&quot; 섹션에서 웹 사이트 도메인과 언어를 지정할 때 선택적으로 동적 검색 대상을 만들 수 있습니다.

  [!DNL Google Ads]은(는) 이러한 설정으로 지정된 웹 사이트의 콘텐츠를 기반으로 동적 검색 광고를 자동으로 표시합니다.

성능을 가장 잘 추적하려면 동적 검색 대상당 하나의 광고 그룹으로 캠페인을 구성하고 모든 기준을 타깃팅하는 광고 그룹을 포함하십시오.

[!DNL Google Ads] 동적 검색 광고에 대한 자세한 내용은 https://support.google.com/google-ads/answer/2471185을 참조하십시오.

## [!UICONTROL Auto Targets] 보기 {#auto-target-view-about}

[!UICONTROL Targeting] > [!UICONTROL Auto Targets] 보기는 선택한 광고주 계정에 대해 필터링된 보기의 모든 동적 검색 대상을 나열합니다. 동적 검색 타겟을 관리할 수도 있습니다.

데이터를 보려면 [!UICONTROL View Auto Targets] 권한이 필요합니다. 대상을 만들고 입찰 또는 상태를 편집하려면 [!UICONTROL Edit Auto Targets] 권한이 필요합니다.

### 사용 가능한 작업

* [동적 검색 대상 만들기](#auto-target-create)

* [동적 검색 대상에 대한 설정 편집](#auto-target-edit)

* [동적 검색 대상의 상태 변경 또는 삭제](#auto-target-status)

* [선택한 행의 모든 데이터를 클립보드에 복사](#copy-to-clipboard)

* 동적 검색 대상에 [제약 조건을 할당](#constraint-assign)하고 동적 검색 대상에서 [제약 조건을 제거](#constraint-unassign)합니다.

* [동적 검색 대상에 레이블 분류를 할당](#classification-values-assign)하고, 동적 검색 대상에서 [레이블 분류를 제거](#classification-values-remove)합니다.

>[!NOTE]
>
>[일괄 시트 파일](/help/search-social-commerce/new-ui/set-up/bulksheets/about.md)을 업로드하고 광고 네트워크에 게시하여 한 번에 많은 양의 대상 데이터(레이블 및 제한 할당 포함)를 만들고 편집할 수 있습니다.

## [!DNL Google Ads] 동적 검색 대상 만들기 {#auto-target-create}

동적 검색 타겟을 만들어 콘텐츠가 동일한 광고 그룹에서 동적 검색 광고를 타깃팅하는 데 사용되는 웹 사이트(즉, 광고의 디스플레이 URL에 사용되는 도메인)의 페이지를 정의할 수 있습니다.

인덱싱된 모든 페이지를 타겟팅하거나 최대 3개의 기준을 지정할 수 있습니다.

>[!NOTE]
>
>성능을 최상으로 추적하려면 캠페인당 하나의 광고 그룹에만 대해 [!UICONTROL All] 옵션을 사용하여 대상을 만드십시오.

1. 메인 메뉴에서 **[!UICONTROL Targeting]>[!UICONTROL Auto Targets]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위에서 **[!UICONTROL Create Auto Target]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Basic Settings]**&#x200B;에서 광고 네트워크, 계정, 캠페인 및 광고 그룹을 선택합니다.

1. 나머지 [동적 검색 대상 설정](#auto-target-create-settings)을 지정하십시오.

1. **[!UICONTROL Review and Save]**&#x200B;을(를) 클릭합니다.

1. 설정을 검토합니다. 설정을 변경하려면 해당 섹션에서 ![편집](/help/search-social-commerce/assets/edit-new.png "편집") **[!UICONTROL Edit]**&#x200B;을(를) 클릭하고 설정을 변경합니다.

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

## [!DNL Google Ads] 동적 검색 대상 설정 편집 {#auto-target-edit}

하나 이상의 동적 검색 대상에 대한 상태 또는 최대 입찰가를 편집할 수 있습니다. 타겟팅된 기준을 변경할 수 없습니다.

1. 메인 메뉴에서 **[!UICONTROL Targeting]>[!UICONTROL Auto Targets]**&#x200B;을(를) 클릭합니다.

1. 편집할 각 행 옆의 확인란을 선택합니다.

   여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)&quot;을 참조하십시오.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Edit Auto Targets]** 패널에서 [상태 및 입찰 설정](#auto-target-edit-settings)을(를) 편집합니다.

   변경 사항은 선택한 모든 대상에 적용됩니다. 변경하지 않는 설정은 기존 값을 유지합니다.

   선택한 타겟이 여러 통화를 사용하는 경우 입찰 편집이 비활성화됩니다. 상태를 변경할 수 있습니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

입찰 값을 클릭하여 데이터 테이블에서 직접 단일 대상의 입찰을 편집할 수도 있습니다.

## [!DNL Google Ads] 동적 검색 대상의 상태 변경 또는 삭제 {#auto-target-status}

활성 동적 검색 대상을 일시 중지하여 동일한 광고 그룹의 동적 검색 광고에 사용을 중지할 수 있습니다. 나중에 상태를 다시 활성으로 변경하여 대상 사용을 재개할 수 있습니다. 동적 검색 타겟을 삭제할 수도 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Targeting]>[!UICONTROL Auto Targets]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 특정 동적 검색 대상을 포함하도록 목록을 필터링합니다.

1. 다음 중 하나를 수행합니다.

   * 한 대상의 상태를 변경하려면 **[!UICONTROL Status]** 열에서 해당 값을 클릭하고 **[!UICONTROL Active]** 또는 **[!UICONTROL Paused]**&#x200B;을(를) 선택하십시오.

   * 여러 대상의 상태를 변경하려면 각 대상 옆의 확인란을 선택하고 일괄 작업 도구 모음에서 **[!UICONTROL Edit]**&#x200B;을(를) 클릭하고 **[!UICONTROL Edit Auto Targets]** 패널에서 **[!UICONTROL Status]**&#x200B;을(를) 선택한 다음 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

   * 하나 이상의 대상을 삭제하려면 각 대상 옆의 확인란을 선택하고 일괄 작업 도구 모음에서 **[!UICONTROL ...]>[!UICONTROL Delete]**&#x200B;을(를) 클릭한 다음 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

## 선택한 행의 모든 데이터를 클립보드에 복사 {#copy-to-clipboard}

보기에 표시되는 적용된 필터 및 열에 따라 선택한 행에 표시되는 정보를 복사합니다. 정보는 탭으로 구분된 값(TSV)으로 저장됩니다.

1. 데이터를 복사할 각 행 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Copy]**&#x200B;을(를) 클릭합니다.

## 동적 검색 대상에 대한 제한 지정 관리 {#constraints}

### 동적 검색 대상에 제한 지정 {#constraint-assign}

1. 메인 메뉴에서 **[!UICONTROL Targeting]>[!UICONTROL Auto Targets]**&#x200B;을(를) 클릭합니다.

1. 단일 제약 조건을 지정할 각 동적 검색 대상 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **+[!UICONTROL Assign]** > **[!UICONTROL Bid Constraint]**&#x200B;을(를) 클릭합니다.

1. 제약조건을 선택합니다.

1. **[!UICONTROL Assign Now]**&#x200B;을(를) 클릭합니다.

### 선택한 동적 검색 대상에서 제한 제거 {#constraint-unassign}

1. 메인 메뉴에서 **[!UICONTROL Targeting]>[!UICONTROL Auto Targets]**&#x200B;을(를) 클릭합니다.

1. 제약 조건을 할당 해제할 각 동적 검색 대상 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **-[!UICONTROL Unassign]** > **[!UICONTROL Bid Constraint]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

## 동적 검색 대상에 대한 분류 값 관리 {#classification-values}

### 동적 검색 대상에 분류 값 할당 {#classification-values-assign}

>[!NOTE]
>
>레이블 값은 하위 엔티티에 의해 상속되므로 상속된 값을 재정의하지 않는 한 동적 검색 대상에 대한 값을 입력하지 마십시오.

1. 메인 메뉴에서 **[!UICONTROL Targeting]>[!UICONTROL Auto Targets]**&#x200B;을(를) 클릭합니다.

1. 레이블 값을 할당할 각 동적 검색 대상 옆의 확인란을 선택합니다.

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

### 동적 검색 대상에서 레이블 분류 값 제거 {#classification-values-remove}

분류 값을 제거하면 계정 구성 요소 및 모든 하위 구성 요소와의 연결이 제거됩니다. 분류 값에 대한 보고서 데이터는 해당 구성 요소에서 더 이상 사용할 수 없습니다. 분류 값을 제거해도 값이나 계정 구성 요소는 삭제되지 않습니다.

1. 메인 메뉴에서 **[!UICONTROL Targeting]>[!UICONTROL Auto Targets]**&#x200B;을(를) 클릭합니다.

1. 레이블 값을 제거할 각 동적 검색 대상 옆의 확인란을 선택합니다.

   여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)&quot;을 참조하십시오.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Unassign]** > **[!UICONTROL Label Classification]**&#x200B;을(를) 클릭합니다.

1. 선택한 엔티티에서 제거할 각 분류 값 옆의 확인란을 선택합니다.

   할당된 모든 값을 선택하려면 **[!UICONTROL Select All]**&#x200B;을(를) 클릭하십시오. 할당된 모든 값을 선택 취소하려면 **[!UICONTROL Deselect All]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Unassign Selected]**&#x200B;을(를) 클릭합니다.

## [!DNL Google Ads] 동적 검색 대상 설정 {#dynamic-search-target-settings}

### 만드는 동안 사용할 수 있는 설정 {#auto-target-create-settings}

#### [!UICONTROL Auto Target Details]

**자동 타겟:** 콘텐츠가 광고 그룹의 동적 검색 광고를 타깃팅하는 데 사용되는 인덱싱된 페이지:

* *[!UICONTROL All]*(기본값): 인덱싱된 모든 페이지를 대상으로 합니다.

* *[!UICONTROL Specific]:*&#x200B;개의 대상 페이지가 최대 3개의 기준과 일치합니다. 기준을 선택하고 해당 값을 입력합니다. 다른 기준을 추가하려면 **[!UICONTROL And]**&#x200B;을(를) 클릭하십시오. 기준은 AND와 결합되므로 페이지는 지정된 모든 기준과 일치해야 합니다. 기준을 지우려면 **[!UICONTROL Reset]**&#x200B;을(를) 클릭합니다.

  * *[!UICONTROL Category]:* 페이지의 [!DNL Google Ads] 콘텐츠 범주가 지정된 값과 같습니다. 값을 입력합니다.

  * *[!UICONTROL URL]:* 페이지의 URL에 `shoes.example.com`과(와) 같이 지정된 값이 포함되어 있습니다. 올바른 URL을 입력하십시오.

  * *[!UICONTROL Page Title]:* 페이지 제목에 지정된 텍스트가 포함되어 있습니다. 값을 입력합니다.

  * *[!UICONTROL Page Content]:* 페이지 콘텐츠에 지정된 텍스트가 있습니다. 값을 입력합니다.

대상을 만든 후에는 대상 기준을 변경할 수 없습니다.

**[!UICONTROL Status]:** 대상의 상태:

* *[!UICONTROL Active]*(기본값): 입찰을 사용합니다.

* *[!UICONTROL Paused]:*&#x200B;이(가) 입찰을 사용하지 않도록 설정합니다.

**[!UICONTROL Bid]:** 대상에 대한 CPC(클릭당 최대 비용)입니다. 이 값은 광고 그룹 수준의 입찰을 무시합니다. 필드는 선택 사항입니다. 입찰을 입력할 때 최소값은 계정 통화로 0.01입니다.

>[!NOTE]
>
>타겟이 최적화된 포트폴리오에 있는 경우 지정된 CPC 입찰가는 하루 동안 적용됩니다. 이후에 최적화 기능은 자체 계산에 따라 입찰을 배치합니다.

### 편집하는 동안 사용할 수 있는 설정 {#auto-target-edit-settings}

#### [!UICONTROL Auto Target Details]

**[!UICONTROL Status]:** **[!UICONTROL Active]** 또는 **[!UICONTROL Paused]** 선택

#### [!UICONTROL Bid details]

선택한 타겟이 여러 통화를 사용하는 경우 입찰 편집이 비활성화됩니다.

**[!UICONTROL Bid adjustment]:** 최대 입찰가를 변경하는 방법:

* *[!UICONTROL Set to]:* 각 입찰가를 [!UICONTROL Set value]의 금액으로 바꿉니다.

* *[!UICONTROL Increase]:* 각 입찰가를 [!UICONTROL Set value]의 금액 또는 백분율만큼 늘립니다.

* *[!UICONTROL Decrease]:* 각 입찰가를 [!UICONTROL Set value]의 금액 또는 백분율만큼 감소시킵니다.

**[!UICONTROL Modifier type]:**([!UICONTROL Increase] 및 [!UICONTROL Decrease]의 경우) **[!UICONTROL Currency]** 또는 **[!UICONTROL Percentage]**&#x200B;을(를) 선택합니다.

**[!UICONTROL Set value]:** 새 입찰 또는 각 입찰을 변경할 금액 또는 백분율입니다. 최소값은 0.01입니다.

**[!UICONTROL Max limit]:**(선택 사항, [!UICONTROL Increase] 및 [!UICONTROL Decrease]의 경우) 계정 통화로 제한됩니다. 증가의 경우 이는 최대 결과 입찰가입니다. 감소의 경우 이는 최소 결과 입찰가입니다. 제한을 입력할 때 최소값은 0.01입니다.

>[!MORELIKETHIS]
>
>* [(새 UI) 검색 입찰 단위에 대한 제약 조건을 관리합니다](/help/search-social-commerce/new-ui/goals/constraints-manage.md)
>* [(새 UI) 레이블 분류 관리](/help/search-social-commerce/new-ui/set-up/label-classifications-manage.md)
