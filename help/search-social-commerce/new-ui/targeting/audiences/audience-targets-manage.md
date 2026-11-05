---
title: 캠페인 및 광고 그룹에 대한 대상자 타겟 관리
description: Google 광고 및 Microsoft Advertising에 대한 대상 타겟 및 입찰 조정을 관리하는 방법을 알아봅니다.
feature: Search Campaign Management
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
source-git-commit: 7e7dcde9fb195e04025a1a8d89e792ff562b053f
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%
---
# 캠페인 및 광고 그룹에 대한 대상자 타겟 관리

*[!DNL Google Ads]및 [!DNL Microsoft Advertising] 계정만*

[!DNL Google Ads]개의 캠페인과 광고 그룹 및 [!DNL Microsoft Advertising]개의 광고 그룹이 동일한 광고 네트워크에서 특정 [대상자](audience-manage.md)를 타깃팅할 수 있습니다. 광고 네트워크는 대상이 타겟팅되어야 하는 대상의 크기를 결정합니다.

대상자 타겟은 기존 대상자를 캠페인 또는 광고 그룹과 연결합니다. 기존 타겟의 입찰 조정 및 상태를 편집할 수 있습니다.

>[!NOTE]
>
>[대상 제외](audience-exclusions.md)는 항상 대상을 재정의합니다.

## [!UICONTROL Targets] 보기 정보 {#audience-targets-view-about}

[!UICONTROL Targeting] > [!UICONTROL Audiences] > [!UICONTROL Targets] 보기는 선택한 광고주에 대해 필터링된 보기의 대상 대상을 나열합니다.

데이터를 보려면 [!UICONTROL View Audiences] 권한이 필요합니다. 대상을 편집, 상태 변경 및 삭제하려면 [!UICONTROL Edit Audience Targets] 권한이 필요합니다.

### 사용 가능한 작업

<!--
Restricted to internal beta users:

* [Configure audience targets](#audience-targets-create)
-->

* [대상 타겟 입찰 조정 및 상태 편집](#audience-targets-edit)

* [대상 타겟의 상태 변경 또는 삭제](#audience-targets-status)

* [선택한 행의 모든 데이터를 클립보드에 복사](#copy-to-clipboard)

<!--
Restricted to internal beta users: audience target creation.

## Configure audience targets {#audience-targets-create}

Creating targets requires the [!UICONTROL Edit Audience Targets] permission in addition to internal beta access.

1. In the main menu, click **[!UICONTROL Targeting] > [!UICONTROL Audiences]**, and then click the **[!UICONTROL Targets]** tab.

1. Click **[!UICONTROL Create Target]**.

1. In **[!UICONTROL Basic Settings]**, select the ad network and account.

1. Select one or more audiences from the account. You can search the list.

   [!DNL Google Ads] customer match audiences are available only for search and shopping campaigns.

1. Select the campaigns or ad groups to target:

   * Select each applicable campaign or ad group for inclusion.

   * To view a campaign's ad groups, expand the campaign.

   * Use the list's search controls to find specific campaigns or ad groups.

   You can't configure a target for both a parent campaign and a child ad group that automatically uses the target.

1. Click **[!UICONTROL Review and Save]**.

1. Review the selections. To make changes, click **[!UICONTROL Edit]** in the applicable section.

1. Click **[!UICONTROL Create]**.

1. (Optional) [Set a bid adjustment](#audience-targets-edit) for the new targets.
-->

## 대상 타겟 입찰 조정 및 상태 편집 {#audience-targets-edit}

한 번에 하나 이상의 대상 타겟을 편집할 수 있습니다. 변경 사항은 선택한 모든 대상에 적용됩니다.

>[!NOTE]
>
>상위 캠페인이 CPC 입찰 전략을 사용하고 대상자 타겟에 대한 입찰 조정 값을 자동 최적화하도록 구성된 포트폴리오에 있는 경우 검색, 소셜 및 Commerce은 입찰 수정자를 자동으로 최적화합니다. [!DNL Microsoft Advertising] 동적 리마케팅 대상 대상에 대한 입찰 수정자가 최적화되지 않았습니다.

1. 주 메뉴에서 **[!UICONTROL Targeting]>[!UICONTROL Audiences]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Targets]** 탭을 클릭합니다.

1. 편집할 각 대상 옆의 확인란을 선택합니다.

   여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)&quot;을 참조하십시오.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Bid Modifier]** 또는 **[!UICONTROL Status]** 또는 둘 다 편집합니다. [편집 설정](#audience-targets-edit-settings)을 참조하세요.

   기존 값을 유지하려면 필드를 변경하지 않고 그대로 둡니다.

1. (선택 사항) **[!UICONTROL ADDITIONAL DETAILS]**&#x200B;을(를) 확장하고 **[!UICONTROL Project Name]** 및 **[!UICONTROL Description]**&#x200B;을(를) 입력합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

**[!UICONTROL Bid Adjustment]** 열에서 값을 클릭하여 데이터 테이블에서 직접 단일 대상의 입찰 조정을 편집할 수도 있습니다.

## 대상 타겟의 상태 변경 또는 삭제 {#audience-targets-status}

활성 대상 대상을 일시 중지하여 해당 대상에 대한 입찰을 비활성화한 후 나중에 활성화하여 입찰을 다시 시작할 수 있습니다. 활성 또는 일시 중지된 타겟을 삭제할 수도 있습니다.

1. 주 메뉴에서 **[!UICONTROL Targeting]>[!UICONTROL Audiences]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Targets]** 탭을 클릭합니다.

1. (선택 사항) 특정 대상 타겟을 포함하도록 목록을 필터링합니다.

1. 상태를 변경할 각 대상 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 다음 중 하나를 클릭합니다.

   * **[!UICONTROL Activate]**&#x200B;을(를) 클릭하여 선택한 대상을 활성화합니다.

   * **[!UICONTROL Pause]**&#x200B;을(를) 클릭하여 선택한 대상을 일시 중지합니다.

   * **[!UICONTROL Delete]**&#x200B;하여 선택한 대상을 삭제합니다.

1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

## 선택한 행의 모든 데이터를 클립보드에 복사 {#copy-to-clipboard}

보기에 표시되는 적용된 필터 및 열에 따라 선택한 행에 표시되는 정보를 복사합니다. 정보는 탭으로 구분된 값(TSV)으로 저장됩니다.

1. 데이터를 복사할 각 행 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Copy]**&#x200B;을(를) 클릭합니다.

## 대상자 타겟 편집 설정 {#audience-targets-edit-settings}

**[!UICONTROL Bid Modifier]:** 대상 입찰 조정을 변경하는 방법:

* *[!UICONTROL Set To]:* 기존 입찰 조정을 지정된 비율로 바꿉니다.

* *[!UICONTROL Increase]:* 지정한 비율만큼 기존 값을 늘립니다.

* *[!UICONTROL Decrease]:* 지정한 비율만큼 기존 값을 줄입니다.

[!UICONTROL Increase] 및 [!UICONTROL Decrease]에 대해 음수가 아닌 값을 입력하십시오.

설정된 값의 경우 0%는 입찰가를 조정하지 않습니다. 다른 지원되는 값은 -90%에서 900%까지입니다. 예를 들어 키워드 수준의 입찰이 1 USD이고 대상 입찰 조정이 50%인 경우 해당 대상에 대한 입찰은 1.50 USD으로 증가합니다.

**[!UICONTROL Status]:** **[!UICONTROL Active]**&#x200B;을(를) 선택하여 입찰을 활성화하거나 **[!UICONTROL Paused]**&#x200B;을(를) 선택하여 대상에 대한 입찰을 비활성화합니다.

>[!MORELIKETHIS]
>
>* [대상자 관리](audience-manage.md)
>* [캠페인 및 광고 그룹에 대한 대상자 제외 관리](audience-exclusions.md)
