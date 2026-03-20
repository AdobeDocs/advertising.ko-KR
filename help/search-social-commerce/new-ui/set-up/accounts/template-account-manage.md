---
title: (새 UI)  [!DNL Naver] 추적 전용 계정 관리
description: ' [!DNL Naver] 계정의 새 UI에서 계정 세부 사항을 설정하고 관리하는 방법에 대해 알아봅니다.'
feature: Search Campaign Management
exl-id: bc4be409-9935-448b-bfba-f93eb30bd5ca
source-git-commit: d6416dae58543e1287b7af7df44eada4be023731
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# (새 UI) 추적에 대해서만 [!DNL Naver] 계정 관리

*Beta 기능*

다음은 광고 네트워크에서 직접 구매하는 광고의 성능을 추적, 보고 및 시각화하기 위해 [[!DNL Naver] 계정](/help/search-social-commerce/campaign-management/naver-tracking-only-account-implement.md)을 관리하는 지침입니다. Search, Social 및 Commerce은 데이터를 광고 네트워크와 동기화하지 않으며, 자동화된 입찰을 제공하지 않으며, 최적화 또는 시뮬레이션의 유형을 제공하지 않습니다.

사용 가능한 기능에 대한 자세한 내용은 &quot;[지원되는 인벤토리](/help/search-social-commerce/introduction/supported-inventory.md)&quot;를 참조하십시오.

## 광고 네트워크 계정 세부 정보 만들기 {#create-account}

계정 추적을 사용하려면 계정 액세스 자격 증명이 포함된 해당 계정 레코드를 *활성화됨* 상태로 만들어야 합니다.

>[!NOTE]
>
>광고 네트워크에서 실제 계정을 만들려면 광고 네트워크의 웹 사이트로 이동합니다.

1. 주 메뉴에서 **[!UICONTROL Setup]** \> **[!UICONTROL Accounts]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Create Account]**&#x200B;을(를) 클릭합니다.

1. 광고 네트워크 이름을 클릭한 다음 **[!UICONTROL Next]**&#x200B;을(를) 클릭합니다.

1. [계정 설정](#account-settings-naver) 지정:

   1. **[!UICONTROL Enter Account Details]** 탭에서 일반 계정 설정을 지정합니다.

   1. ([[!DNL Adobe Analytics for Advertising] 통합](/help/integrations/analytics/overview.md)을(를) 사용하는 광고주) **[!UICONTROL Set up Adobe Analytics]** 탭을 클릭하고 캠페인 활동 추적 및 보고에 사용할 모든 [!DNL Analytics] 보고 세트를 선택합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 광고 네트워크 계정 세부 정보 편집 {#edit-account}

계정 이름을 변경하거나, 계정 상태를 변경하거나, 추적 및 보고에 사용할 [!DNL Analytics] 보고서 세트를 변경하려면 계정 세부 정보를 편집하십시오.

>[!NOTE]
>
>광고 네트워크에서 실제 계정을 편집하려면 광고 네트워크의 웹 사이트로 이동합니다.

1. 주 메뉴에서 **[!UICONTROL Setup]** \> **[!UICONTROL Accounts]**&#x200B;을(를) 클릭합니다.

1. 다음 방법 중 하나로 계정을 선택합니다.

   * 계정 이름 옆의 확인란을 선택한 다음 일괄 작업 도구 모음에서 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

   * 계정 이름 위에 커서를 놓고 **..**&#x200B;을 클릭한 다음 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. [계정 설정](#account-settings-api)을(를) 편집합니다.

   1. (선택 사항) **[!UICONTROL Account Details]** 탭에서 계정 세부 정보를 편집합니다.

   1. (선택 사항, [[!DNL Adobe Analytics for Advertising] 통합](/help/integrations/analytics/overview.md)을 사용하는 광고주) **[!UICONTROL Set up Adobe Analytics]** 탭을 클릭하고 캠페인 활동 추적 및 보고에 사용할 [!DNL Analytics] 보고 세트를 편집하십시오.

   <!-- What are the repercussions of changing the suites? Timing of updated data? -->

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

<!--
 What does this do?

## Enable or disable ad network accounts {#enable-disable-account}

When you enable an ad network account, Search, Social, & Commerce synchronizes campaign data with the account (when supported) and pushes automated bids and/or campaign budgets for campaigns in portfolios. When you disable an ad network account, Search, Social, & Commerce stops all activity on the account. Data collected while the account was active is still stored, but the campaign management views and reports don't include data for the time period in which the account is disabled. You can later re-enable the account to resume activity with the account.

1. In the main menu, click **[!UICONTROL Setup]** \> **[!UICONTROL Accounts]**.

1. Do either of the following:

   * (From the [!UICONTROL Accounts] view):

     * (To enable the account) Select the check box next to the account name, and then click **[!UICONTROL Activate]** in the bulk actions toolbar.

     * (To disable the account) Select the check box next to the account name, and then click **[!UICONTROL Pause]** in the bulk actions toolbar.

   * (From the account settings):
   
     1. Select the account in either of the following ways:
     
        * Hold the cursor over the account name, click **...**, and then click **[!UICONTROL Edit]**.
        
        * Select the check box next to the account name, and then click **[!UICONTROL Edit]** in the bulk actions toolbar.
        
     1. On the **[!UICONTROL Account Details]** tab, turn off **[!UICONTROL Account enabled]**.

     1. Click **[!UICONTROL Save]**.

-->

## 광고 네트워크 계정 설정 {#account-settings-api}

### [!UICONTROL Account Details] 탭

#### [!UICONTROL Enter Account Details]/[!UICONTROL Account Details]

**[!UICONTROL Account Name]:** Search, Social 및 Commerce 내에서 계정에 대해 표시될 이름입니다.

>[!NOTE]
>
>Search, Social 및 Commerce-Adobe Analytics 통합이 있고 검색 계정의 이름을 변경한 경우, Adobe 계정 팀에 매핑을 업데이트하도록 요청하십시오.

**[!UICONTROL Network Account ID]:** 광고 네트워크에서 할당한 계정 ID입니다.

**[!UICONTROL Currency]:** 계정에 사용되는 통화의 약어입니다.

**[!UICONTROL Time Zone]:** 광고주의 시간대입니다.

**[!UICONTROL Account Synchronization and Management]> [!UICONTROL Account Enabled]:** 검색, 소셜 및 Commerce은 캠페인 데이터를 계정과 동기화하고(지원되는 경우) 포트폴리오의 캠페인에 대한 자동 입찰 및/또는 캠페인 예산을 푸시합니다.

## [!UICONTROL Setup Analytics] 탭

**[!UICONTROL Adobe Analytics Report Suite]:**(Advertisers with an [[!DNL Adobe Analytics for Advertising] integration](/help/integrations/analytics/overview.md); 선택 사항) Search, Social 및 Commerce이 개체 분류 및 계정에 대한 클릭 데이터를 포함하여 광고 네트워크에 대해 업로드한 데이터를 전송하는 하나 이상의 Analytics 보고서 세트입니다.

데이터를 보고서 세트에 표시하려면 (a) 계정에 대해 서버측 AMO ID 기능을 구성해야 하거나 (b) &quot;[!UICONTROL Enable Advertising reporting in Analytics]&quot;에 대한 광고주 수준 설정을 활성화해야 합니다. 또한 Search, Social 및 Commerce에서 데이터를 수신하도록 광고주의 [!DNL Analytics] 계정을 구성해야 합니다. 자세한 내용은 Adobe 계정 팀에 문의하십시오.

>[!MORELIKETHIS]
>
>* [추적 전용 계정 구현 [!DNL Naver] 2}](/help/search-social-commerce/campaign-management/naver-tracking-only-account-implement.md)
>* [광고 네트워크 계정 정보](/help/search-social-commerce/new-ui/set-up/accounts/ad-network-account-about.md)
