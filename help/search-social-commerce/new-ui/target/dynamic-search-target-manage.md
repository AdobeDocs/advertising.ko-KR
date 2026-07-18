---
title: ' [!DNL Google Ads] 동적 검색 대상 관리'
description: ' [!DNL Google Ads] 동적 검색 대상을 만들고 관리하는 방법을 알아봅니다.'
exl-id: 5ea68cab-677f-4c7e-8776-24d6546f0b15
feature: Search Campaign Management
TQID: 'https://experienceleague.adobe.com/MsSy-p-WSroc3FyiHx6kvcTohEaWOqJCzqbl91mNwK0'
product_v2: id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2: id: aed5e38a-3e62-42fa-8d16-cd080729b2a0
subfeature_v2: id: f3d33161-c519-436e-bbbd-730ba428736b
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 82db1b4d0d8703229a4002e932d5b2f52f845814
workflow-type: tm+mt
source-wordcount: 718
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

## [!UICONTROL Auto Targets] 보기

[!UICONTROL Auto Targets] 보기는 선택한 광고주 계정에 대해 필터링된 보기의 모든 동적 검색 대상을 나열합니다.

[!UICONTROL Campaigns] > [!UICONTROL Campaigns] > [!UICONTROL Auto Targets] 보기에서 동적 검색 대상의 상태를 만들고 편집하고 변경할 수 있습니다.

대상에 [레이블을 적용](/help/search-social-commerce/campaign-management/label-classifications/classification-values-assign-campaign-management.md)할 수도 있습니다.

### 사용 가능한 작업

<!--
* Create a dynamic search target

* Edit the settings for a dynamic search target

* Change the status of dynamic search targets
-->

* [동적 검색 대상에 제약 조건 할당](#constraint-assign) 및 [동적 검색 대상에서 제약 조건 할당 해제](#constraint-unassign)

* [동적 검색 대상에 레이블 분류를 할당](#classification-values-assign)하고, 동적 검색 대상에서 [레이블 분류를 제거](#classification-values-remove)합니다.

>[!NOTE]
>
>[일괄 시트 파일](/help/search-social-commerce/new-ui/set-up/bulksheets/about.md)을 업로드하고 광고 네트워크에 게시하여 한 번에 많은 양의 대상 데이터(레이블 및 제한 할당 포함)를 만들고 편집할 수 있습니다.

<!--
Not available yet:

## Create a [!DNL Google Ads] dynamic search target

You can create dynamic search targets to define pages in your websites (that is, the domains used in your ads' display URLs) whose content is used to target your dynamic search ads in the same ad group.

You can target all criteria or up to three individual criteria.

>[!NOTE]
>
>To best track performance, create an "[!UICONTROL All Targets]" target for only one ad group per campaign.

>[!TIP]
>
>To create many account components at once, use [campaign bulksheets](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-about.md).

1. In the main menu, click **[!UICONTROL Search, Social, & Commerce] > [!UICONTROL Campaigns] > [!UICONTROL Campaigns]**. In the submenus, click **[!UICONTROL Live] > [!UICONTROL Auto Targets]**.

1. In the toolbar above the data table, click ![Create](/help/search-social-commerce/assets/add.png "Create").

1. Select the ad network, the account, the campaign, and the ad group, and then click **[!UICONTROL Continue]**.

1. Specify the [dynamic search target settings](#dynamic-search-target-settings).

1. Click **[!UICONTROL Post]**.

## Edit [!DNL Google Ads] dynamic search target settings

You can edit the status or maximum bid for a [!DNL Google Ads] dynamic search target. You can't change the criteria that are targeted.

>[!TIP]
>
>To edit large amounts of data at once, use [campaign bulksheets](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-about.md).

1. In the main menu, click **[!UICONTROL Search, Social, & Commerce] > [!UICONTROL Campaigns] > [!UICONTROL Campaigns]**. In the submenus, click **[!UICONTROL Live] > [!UICONTROL Auto Targets]**.

1. Select the check box next to each row to edit.

   For tips on selecting multiple rows, see "[Select multiple rows](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)."

1. In the toolbar above the data table, click ![Edit](/help/search-social-commerce/assets/edit.png "Edit").

1. Specify the [dynamic search target settings](#dynamic-search-target-settings).

   For multiple targets, your changes are applied to all of the selected targets. For the [!UICONTROL Bid field], you have options to change existing values to a specified value or to either increase or decrease the amount by a specified percentage or monetary amount, with a limit.

1. Save the data:

   * (Single targets) Click **[!UICONTROL Post]**.
   
   * (Multiple ad groups) Click **[!UICONTROL Post Now]**.

## Change the status of [!DNL Google Ads] dynamic search targets

You can pause any active dynamic search target in a supported campaign type to stop using them for dynamic search ads in the same ad group. You can later use them as targets by changing the ad status back to active.

You can also delete any dynamic target.

1. In the main menu, click **[!UICONTROL Search, Social, & Commerce] > [!UICONTROL Campaigns] > [!UICONTROL Campaigns]**. In the submenus, click **[!UICONTROL Live] > [!UICONTROL Auto Targets]**.

1. (Optional) Filter the list to include specific dynamic targets.

1. Do either of the following:
   
   * To change the status of one dynamic target, click in the **[!UICONTROL Status]** column and change the status.
   
   * To delete one or more dynamic targets, do the following:
   
     1.  Select the check box next to each dynamic target you want to delete.
     
        For tips on selecting multiple rows, see "[Select multiple rows](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)."
     
     1. In the toolbar, click ![More](/help/search-social-commerce/assets/more.png "More") and select **[!UICONTROL Delete]**.
     
     1. In the confirmation message, click **[!UICONTROL Delete]**.

## [!DNL Google Ads] dynamic search target settings {#dynamic-search-target-settings}

### [!UICONTROL Auto-Target Details]

**[!UICONTROL Auto-targets]:** (Required when you don't specify a website domain and language in the campaign's [!UICONTROL DSA Options] section; read-only for existing targets) Dynamic search targets for the ad group:

* *[!UICONTROL All Targets]* (the default): Targets all indexed pages.

* *\[Specific Targets\]:* Targets up to three criteria for the indexed pages. When you select this, you must specify the criteria by specifying information categories and specific values for which to target ads (for example, "URL contains shoes.example.com"). To specify more than one criteria, click **[!UICONTROL + And]**. Target criteria include:

  * *[!UICONTROL Category]:* To show ads for indexed pages with a specific [!DNL Google Ads] content category.

  * *[!UICONTROL URL]:* To show ads for indexed pages with a specific URL, where the value may be included anywhere within the URL.

  * *[!UICONTROL Page Title]:* To show ads for indexed pages with specific text in the page title.

  * *[!UICONTROL Page Content]:* To show ads for indexed pages with specific content.

**Status:** The status of the target settings:

* *[!UICONTROL Active]* (the default): Enables bidding.

* *[!UICONTROL Paused]:* Disables bidding.

* *[!UICONTROL Deleted]* (existing targets only): Deletes the target settings.

### [!UICONTROL Bids]

**[!UICONTROL Bid]:** The maximum cost per click (CPC) for an ad or cost per 1000 impressions (CPM) for an ad, as applicable for the ad network and campaign pricing model. This value overrides the ad group-level value.

>[!NOTE]
>
>If the target is in an optimized portfolio, then the specified CPC bid is applied for one day. Afterward, the optimization capability places bids according to its own calculations.

-->

## 새 [!UICONTROL Auto Targets] 보기에서 선택한 동적 검색 대상에 제약 조건 할당 {#constraint-assign}

1. 메인 메뉴에서 **[!UICONTROL Target]>[!UICONTROL Auto Targets]**&#x200B;을(를) 클릭합니다.

1. 단일 제약 조건을 지정할 각 동적 검색 대상 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **+[!UICONTROL Assign]** > **[!UICONTROL Constraint]**&#x200B;을(를) 클릭합니다.

1. 제약조건을 선택합니다.

1. **[!UICONTROL Assign Now]**&#x200B;을(를) 클릭합니다.

## 새 [!UICONTROL Auto Targets] 보기에서 선택한 동적 검색 대상에서 제약 조건 할당 해제 {#constraint-unassign}

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Auto Targets]**&#x200B;을(를) 클릭합니다.

1. 제약 조건을 할당 해제할 각 동적 검색 대상 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **-[!UICONTROL Unassign]** > **[!UICONTROL Constraint]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

## 동적 검색 대상에 분류 값 할당 {#classification-values-assign}

>[!NOTE]
>
>레이블 값은 하위 엔티티에 의해 상속되므로 상속된 값을 재정의하지 않는 한 하위 엔티티에 대한 값을 입력하지 마십시오.

1. 메인 메뉴에서 **[!UICONTROL Target]>[!UICONTROL Auto Targets]**&#x200B;을(를) 클릭합니다.

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

## 동적 검색 대상에서 레이블 분류 값 제거{#classification-values-remove}

분류 값을 제거하면 계정 구성 요소 및 모든 하위 구성 요소와의 연결이 제거됩니다. 분류 값에 대한 보고서 데이터는 해당 구성 요소에서 더 이상 사용할 수 없습니다. 분류 값을 제거해도 값이나 계정 구성 요소는 삭제되지 않습니다.

1. 메인 메뉴에서 **[!UICONTROL Target]>[!UICONTROL Auto Targets]**&#x200B;을(를) 클릭합니다.

1. 레이블 값을 제거할 각 동적 검색 대상 옆의 확인란을 선택합니다.

   여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)&quot;을 참조하십시오.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Unassign]** > **[!UICONTROL Label Classification]**&#x200B;을(를) 클릭합니다.

1. 선택한 엔티티에서 제거할 각 분류 값 옆의 확인란을 선택합니다.

   할당된 모든 값을 선택하려면 **[!UICONTROL Select All]**&#x200B;을(를) 클릭하십시오. 할당된 모든 값을 선택 해제하려면 **[!UICONTROL Deselect All]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Unassign Selected]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [(새 UI) 검색 입찰 단위에 대한 제약 조건을 관리합니다](/help/search-social-commerce/new-ui/goals/constraints-manage.md)
>* [(새 UI) 레이블 분류 관리](/help/search-social-commerce/new-ui/reports/label-classifications-manage.md)
