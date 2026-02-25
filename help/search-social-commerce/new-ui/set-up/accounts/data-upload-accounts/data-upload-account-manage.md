---
title: 데이터 업로드를 위한 광고 네트워크 계정 구성
description: 광고 네트워크 계정에 대한 계정 세부 정보를 설정하고 관리하는 방법을 알아봅니다.
feature: Search Campaign Management
exl-id: 7e8fb475-21f9-446b-a112-e0f27a4c4172
source-git-commit: 00565a6c9e784472fab9c9d223c83b0c7cbb91b1
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# 데이터 업로드를 위한 광고 네트워크 계정 관리

<!-- Edit all, including title and metadata -->

다음은 계정 데이터를 업로드할 광고 네트워크 계정의 계정 세부 정보를 관리하는 지침입니다.

각 광고 네트워크에서 사용할 수 있는 기능에 대한 자세한 내용은 &quot;[지원되는 인벤토리](/help/search-social-commerce/introduction/supported-inventory.md)&quot;를 참조하십시오.

>[!NOTE]
>
>광고 네트워크의 API를 사용하여 검색, 소셜 및 Commerce이 동기화되는 광고 네트워크 계정에 대한 계정 세부 정보를 관리하는 방법에 대한 지침은 대신 &quot;[API 연결을 통해 광고 네트워크 계정 관리](../api-accounts/api-account-manage.md)&quot;를 참조하십시오.

## 계정 세부 정보 만들기 {#create-account}

1. **[!UICONTROL Create Account]**&#x200B;을(를) 클릭합니다.

1. 광고 네트워크 이름을 클릭한 다음 **[!UICONTROL Next]**&#x200B;을(를) 클릭합니다.

1. [계정 설정](#account-settings) 지정:

   1. **[!UICONTROL Account Details]** 탭에서 계정 세부 정보를 편집합니다.

   1. ([[!DNL Adobe Analytics for Advertising] 통합](/help/integrations/analytics/overview.md)을 사용하는 광고주) **[!UICONTROL Set up Adobe Analytics]** 탭을 클릭하고 캠페인 활동 추적 및 보고에 사용할 [!DNL Analytics] 보고 세트를 편집하십시오.

   1. (선택 사항) **[!UICONTROL Upload File]** 탭에서 계정에 대한 데이터 파일을 업로드합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 계정 세부 정보 편집 {#edit-account}

1. 주 메뉴에서 **[!UICONTROL Setup]** \> **[!UICONTROL Accounts]**&#x200B;을(를) 클릭합니다.

1. 다음 방법 중 하나로 계정을 선택합니다.

   * 계정 이름 옆의 확인란을 선택한 다음 일괄 작업 도구 모음에서 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

   * 계정 이름 위에 커서를 놓고 **..**&#x200B;을 클릭한 다음 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. [계정 설정](#account-settings-upload)을(를) 편집합니다.

   1. (선택 사항) **[!UICONTROL Account Details]** 탭에서 계정 세부 정보를 편집합니다.

   1. (선택 사항, [[!DNL Adobe Analytics for Advertising] 통합](/help/integrations/analytics/overview.md)을 사용하는 광고주) **[!UICONTROL Set up Adobe Analytics]** 탭을 클릭하고 캠페인 활동 추적 및 보고에 사용할 [!DNL Analytics] 보고 세트를 편집하십시오.

   1. (선택 사항) **[!UICONTROL Upload File]** 탭에서 계정에 대한 데이터 파일을 업로드합니다.

   <!-- What are the repercussions of changing the suites? Timing of updated data? -->

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 광고 네트워크 계정 활성화 또는 비활성화 {#enable-disable-account}

1. 주 메뉴에서 **[!UICONTROL Setup]** \> **[!UICONTROL Accounts]**&#x200B;을(를) 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * [!UICONTROL Accounts] 보기에서:

      * (계정을 활성화하려면) 계정 이름 옆에 있는 확인란을 선택한 다음 일괄 작업 도구 모음에서 **[!UICONTROL Activate]**&#x200B;을(를) 클릭합니다.

      * (계정을 사용하지 않도록 설정하려면) 계정 이름 옆에 있는 확인란을 선택한 다음 일괄 작업 도구 모음에서 **[!UICONTROL Pause]**&#x200B;을(를) 클릭합니다.

   * (계정 설정에서):

      1. 다음 방법 중 하나로 계정을 선택합니다.

         * 계정 이름 위에 커서를 놓고 **..**&#x200B;을 클릭한 다음 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

         * 계정 이름 옆의 확인란을 선택한 다음 일괄 작업 도구 모음에서 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

      1. **[!UICONTROL Account Details]** 탭에서 **[!UICONTROL Account enabled]**&#x200B;을(를) 끕니다.

      1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 계정 설정 {#account-settings-upload}

### [!UICONTROL Account Details] 탭

**[!UICONTROL Account Name]:** Search, Social 및 Commerce 내에서 계정에 대해 표시될 이름입니다.

>[!NOTE]
>
>Search, Social 및 Commerce-Adobe Analytics 통합이 있고 검색 계정의 이름을 변경한 경우, Adobe 계정 팀에 알려 매핑을 업데이트할 수 있도록 하십시오.

**[!UICONTROL Network Account ID]:** 광고 네트워크에서 할당한 계정 ID입니다. 이 ID는 보고용으로만 사용됩니다. Search, Social 및 Commerce은 광고 네트워크 계정에 직접 연결되지 않습니다.

**[!UICONTROL Currency]:**(기존 계정의 경우 읽기 전용) 계정에 사용되는 통화의 약어입니다.

**[!UICONTROL Time Zone]:**(기존 계정의 경우 읽기 전용) 광고주의 시간대입니다.

**[!UICONTROL Account Synchronization and Management]> [!UICONTROL Account Enabled]:** 검색, 소셜 및 Commerce에서는 지정된 S3 버킷에 대해 자동화된 데이터 가져오기를 허용합니다.

## [!UICONTROL Setup Analytics] 탭

**[!UICONTROL Adobe Analytics Report Suite]:**(Advertisers with an [[!DNL Adobe Analytics for Advertising] integration](/help/integrations/analytics/overview.md); 선택 사항) Search, Social 및 Commerce이 개체 분류 및 계정에 대한 클릭 데이터를 포함하여 광고 네트워크에 대해 업로드한 데이터를 전송하는 하나 이상의 Analytics 보고서 세트입니다.

데이터를 보고서 세트에 표시하려면 (a) 계정에 대해 서버측 AMO ID 기능을 구성해야 하거나 (b) &quot;[!UICONTROL Enable Advertising reporting in Analytics]&quot;에 대한 광고주 수준 설정을 활성화해야 합니다. 또한 Search, Social 및 Commerce에서 데이터를 수신하도록 광고주의 [!DNL Analytics] 계정을 구성해야 합니다. 자세한 내용은 Adobe 계정 팀에 문의하십시오.

### [!UICONTROL Upload File] 탭

(선택 사항) 계정에 대한 데이터 파일을 업로드합니다.<!-- For instructions, see "[Upload offline account data for reporting and simulations](upload-account-data.md)." -->
