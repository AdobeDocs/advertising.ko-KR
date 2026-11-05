---
title: 캠페인 및 광고 그룹에 대한 대상자 제외 관리
description: Google 광고 제외를 삭제하는 방법을 포함하여 Google 광고 및 Microsoft Advertising 대상 제외에 대해 알아봅니다.
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
source-wordcount: '269'
ht-degree: 0%
---
# 캠페인 및 광고 그룹에 대한 대상자 제외 관리

*[!DNL Google Ads]및 [!DNL Microsoft Advertising] 계정만*

대상자 제외를 사용하면 캠페인이나 광고 그룹의 광고가 특정 [대상자](audience-manage.md)의 사용자에게 표시되지 않습니다.

[!DNL Google Ads] 계정의 경우 대상 유형을 제외할 수 있습니다. [!DNL Microsoft Advertising] 계정의 경우 동적 리마케팅 대상자만 제외할 수 있습니다.

>[!NOTE]
>
>제외는 항상 [대상 대상](audience-targets-manage.md)을 재정의합니다.

## [!UICONTROL Exclusions] 보기 정보 {#audience-exclusions-view-about}

[!UICONTROL Targeting] > [!UICONTROL Audiences] > [!UICONTROL Exclusions] 보기에는 선택한 광고주에 대해 필터링된 보기의 대상 제외가 나열됩니다.

데이터를 보려면 [!UICONTROL View Audiences] 권한이 필요합니다. 행을 선택하고 지원되는 제외를 삭제하려면 [!UICONTROL Edit Audience Exclusions] 권한이 필요합니다.

### 사용 가능한 작업

<!--
Restricted to internal beta users:

* [Configure audience exclusions](#audience-exclusions-create)
-->

* [대상 제외 삭제](#audience-exclusions-delete)

* [선택한 행의 모든 데이터를 클립보드에 복사](#copy-to-clipboard)

<!--
Restricted to internal beta users: audience exclusion creation.

## Configure audience exclusions {#audience-exclusions-create}

Creating exclusions requires the [!UICONTROL Edit Audience Exclusions] permission in addition to internal beta access.

1. In the main menu, click **[!UICONTROL Targeting] > [!UICONTROL Audiences]**, and then click the **[!UICONTROL Exclusions]** tab.

1. Click **[!UICONTROL Create Exclusion]**.

1. In **[!UICONTROL Basic Settings]**, select the ad network and account.

1. Select one or more audiences from the account. You can search the list.

   [!DNL Google Ads] customer match audiences are available only for search and shopping campaigns.

1. Select the campaigns or ad groups from which to exclude the audiences:

   * Select each applicable campaign or ad group for exclusion.

   * To view a campaign's ad groups, expand the campaign.

   * Use the list's search controls to find specific campaigns or ad groups.

1. Click **[!UICONTROL Review and Save]**.

1. Review the selections. To make changes, click **[!UICONTROL Edit]** in the applicable section.

1. Click **[!UICONTROL Create]**.
-->

## 대상 제외 삭제 {#audience-exclusions-delete}

*[!DNL Google Ads]개 제외만*

[!DNL Google Ads]개 이상의 대상 제외를 삭제할 수 있습니다. 이 보기에서는 [!DNL Microsoft Advertising] 제외를 삭제할 수 없습니다.

1. 주 메뉴에서 **[!UICONTROL Targeting]>[!UICONTROL Audiences]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Exclusions]** 탭을 클릭합니다.

1. (선택 사항) 특정 대상 제외를 포함하도록 목록을 필터링합니다.

1. 삭제할 각 [!DNL Google Ads] 제외 옆의 확인란을 선택하십시오. 선택 항목에 다른 광고 네트워크에서의 제외를 포함하지 마십시오.

   여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)&quot;을 참조하십시오.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

## 선택한 행의 모든 데이터를 클립보드에 복사 {#copy-to-clipboard}

보기에 표시되는 적용된 필터 및 열에 따라 선택한 행에 표시되는 정보를 복사합니다. 정보는 탭으로 구분된 값(TSV)으로 저장됩니다.

1. 데이터를 복사할 각 행 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Copy]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [대상자 관리](audience-manage.md)
>* [캠페인 및 광고 그룹에 대한 대상자 대상 관리](audience-targets-manage.md)
