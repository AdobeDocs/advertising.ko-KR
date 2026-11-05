---
title: 대상자 관리
description: 대상 라이브러리에 대해 알아보고 Google 광고 및 Microsoft Advertising에 대해 지원되는 대상을 관리하는 방법을 알아봅니다.
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
topic_v2:
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
    internal-label: Privacy
source-git-commit: 7e7dcde9fb195e04025a1a8d89e792ff562b053f
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 0%
---
# 대상자 관리

*[!DNL Google Ads]및 [!DNL Microsoft Advertising] 계정만*

대상은 동일한 광고 네트워크에서 지원되는 캠페인 및 광고 그룹에 대해 [타겟](audience-targets-manage.md) 또는 [제외](audience-exclusions.md)(으)로 사용할 수 있는 사용자 그룹입니다. 광고 네트워크는 대상이 타겟팅되어야 하는 대상의 크기를 결정합니다.

## [!UICONTROL Library] 보기 정보 {#audience-view-about}

[!UICONTROL Targeting] > [!UICONTROL Audiences] > [!UICONTROL Library] 보기에는 선택한 광고주의 대상이 나열됩니다. [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 대상자를 보려면 **[!UICONTROL Network]** 메뉴에서 **[!UICONTROL All Other Network]**&#x200B;을(를) 선택하십시오.

라이브러리에는 [!DNL Google Ads]개의 고객 데이터 기반, 마켓 내 및 유사 대상과 [!DNL Microsoft Advertising]개의 리마케팅, 동적 리마케팅, 사용자 지정, 고객 일치, 마켓 내 및 유사 대상이 포함되어 있습니다.

데이터를 보려면 [!UICONTROL View Audiences] 권한이 필요합니다. 행을 선택하고 지원되는 대상을 삭제하려면 [!UICONTROL Edit Audience Library] 권한이 필요합니다.

### 사용 가능한 작업

<!--
Restricted to internal beta users:

* [Create a customer match audience from a customer data list](#audience-customer-list-create)

* [Create a Google Ads audience from Adobe audiences](#audience-adobe-create)

* [Create a Microsoft Advertising dynamic remarketing audience](#audience-dynamic-create)

* [Update a customer match audience using a customer data list](#audience-customer-list-edit)

* [Edit a dynamic remarketing audience](#audience-dynamic-edit)
-->

* [동적 리마케팅 대상자 삭제](#audience-delete)

* [선택한 행의 모든 데이터를 클립보드에 복사](#copy-to-clipboard)

## 대상 데이터 소스 {#audience-data-sources}

다음 데이터 소스를 기반으로 대상을 사용할 수 있습니다.

* **Adobe 대상 세그먼트:** 옵트인 Adobe Audience Manager 또는 Adobe Analytics 계정이 있는 광고주는 기존 [!DNL Adobe] 세그먼트를 기반으로 하는 [!DNL Google Ads] 고객 일치 대상을 사용할 수 있습니다.

  * Audience Manager이 없는 [!DNL Analytics] 계정이 있는 광고주의 경우 대상은 Adobe CX Enterprise과 공유된 [!DNL Analytics] 세그먼트의 사용자 ID를 사용합니다.

  * Audience Manager 계정이 있는 광고주의 경우 대상은 검색, 소셜 및 Commerce이 대상으로 있는 Audience Manager 세그먼트의 사용자 ID를 사용합니다. 여기에는 Adobe CX Enterprise에 게시된 [!DNL Analytics]개의 세그먼트와 Adobe CX Enterprise 대상 라이브러리를 사용하여 만든 세그먼트가 포함될 수 있습니다.

  [!DNL Google Ads] 계정은 [고객 일치 가능](https://support.google.com/adspolicy/answer/6299717)이어야 하며 [사용자 ID 세그먼트](https://support.google.com/google-ads/answer/9199250)를 옵트인해야 합니다. Search, Social 및 Commerce의 광고주 계정도 고객 일치 대상을 만들 수 있도록 구성해야 합니다. 이 기능을 활성화하려면 Adobe 계정 팀에 문의하십시오.

  고객 데이터 기반 대상의 [!DNL Adobe] 세그먼트 데이터 및 쿠키 동기화 파일이 매일 [!DNL Google Ads]에 동기화됩니다.

* **Adobe Campaign 전자 메일 목록:** Adobe 계정 팀은 [!DNL Campaign]의 전자 메일 목록에서 [!DNL Google Ads] 고객 일치 대상을 만들고 업데이트하는 워크플로를 설정하는 데 도움을 줄 수 있습니다. 워크플로우가 대상 라이브러리가 아닌 [!DNL Campaign]에서 구성되었습니다. &quot;[Adobe Campaign 이메일 목록에서 고객 일치 대상 만들기](/help/search-social-commerce/campaign-management/campaigns/google-audience-from-campaign-email-list.md)&quot;를 참조하십시오.

* **고객 데이터 목록:** 적격 [!DNL Google Ads] 또는 [!DNL Microsoft Advertising] 계정이 있는 광고주는 CRM(고객 관계 관리) 시스템의 기본 식별자가 포함된 CSV 파일을 기반으로 고객 일치 대상을 사용할 수 있습니다.

* **동적 리마케팅 목록:** [!DNL Microsoft Advertising] 계정이 있는 광고주는 제품 뷰어 또는 이전 구매자와 같이 최근에 제품과 상호 작용한 사용자를 기반으로 대상을 사용할 수 있습니다. 이러한 대상을 사용하려면 관련 웹 페이지에서 광고 네트워크의 JavaScript 전환 및 대상 추적 태그가 필요합니다.

  동적 리마케팅 대상자는 검색 및 대상 네트워크의 쇼핑 캠페인과 함께 사용하여 제품 광고로 사용자를 재타겟팅하고, 검색 캠페인과 함께 사용하여 텍스트 광고 및 동적 검색 광고로 사용자를 재타겟팅할 수 있습니다.

  >[!NOTE]
  >
  >동적 리마케팅 대상자 타겟에 대한 입찰 수정자가 [!UICONTROL Auto-optimize Bid Adjustment Values] 설정이 있는 포트폴리오에서 최적화되지 않았습니다.

>[!NOTE]
>
>Search, Social 및 Commerce은 업로드한 고객 데이터나 대상을 만들거나 편집하는 데 사용한 [!DNL Adobe]개 세그먼트의 고객 데이터를 저장하지 않습니다.

<!--
Restricted to internal beta users: audience creation and library editing.

## Create a customer match audience from a customer data list {#audience-customer-list-create}

*[!DNL Google Ads] and [!DNL Microsoft Advertising] accounts that are eligible for customer match only*

For [!DNL Microsoft Advertising], the file can include email addresses. For [!DNL Google Ads], the file can include email addresses, mailing addresses, telephone numbers, user IDs, or mobile device IDs.

Creating and editing library audiences requires the [!UICONTROL Edit Audience Library] permission in addition to internal beta access.

1. Prepare a CSV file with the customer data in the required format.

   First and last names, email addresses, and telephone numbers must be hashed using SHA-256. Follow the network's formatting requirements for the selected identifier type. See the [Google Ads formatting guidelines](https://support.google.com/google-ads/answer/7476159) or the [Microsoft Advertising instructions for preparing customer match lists](https://help.ads.microsoft.com/#apex/ads/en/56921).

1. In the main menu, click **[!UICONTROL Targeting] > [!UICONTROL Audiences]**, and then click the **[!UICONTROL Library]** tab.

1. Select **[!UICONTROL All Other Network]** from the **[!UICONTROL Network]** menu.

1. Click **[!UICONTROL Create Audience]**.

1. In **[!UICONTROL Basic Settings]**, select the ad network and account.

1. In **[!UICONTROL Data Source]**, select the customer-list option.

1. Enter the **[!UICONTROL Audience Name]** and select the **[!UICONTROL Data Upload Type]**:

   * ([!DNL Microsoft Advertising]) **[!UICONTROL Emails]**.

   * ([!DNL Google Ads]) **[!UICONTROL Emails, Phones, and/or Mailing Addresses]**, **[!UICONTROL User IDs]**, or **[!UICONTROL Mobile Device IDs]**.

     User ID lists are available only to eligible [!DNL Google Ads] advertisers in the U.S. who are opted in for user ID segments.

1. (Mobile device ID lists only) Select the **[!UICONTROL OS Type]** and enter the **[!UICONTROL App ID]**.

   For an Android app, use its package name in [!DNL Google Play], such as `com.example.game` from `https://play.google.com/store/apps/details?id=com.example.game`. For an iOS app, use its application ID from the [!DNL App Store], such as `id284882215`. Your development team can provide the ID.

1. In **[!UICONTROL Select File]**, select the CSV file from your device or network.

1. Select the check box to indicate that you agree with the [!DNL Adobe] and ad network privacy policies.

1. ([!DNL Google Ads]; optional) If you do business in the European Economic Area (EEA) or United Kingdom (UK) and have collected all required user consents, select the consent check box to send the consent status as **[!UICONTROL GRANTED]** for advertising and ad personalization.

   If you leave the check box unselected, the consent status is sent as **[!UICONTROL UNSPECIFIED]**. [!DNL Google Ads] ignores data for EEA and UK users with an unspecified consent status, which can cause data discrepancies and performance issues.

1. Click **[!UICONTROL Upload File]** and wait for the upload to finish.

1. Configure any remaining audience settings, including **[!UICONTROL Membership Days]** when available.

   Membership days specify how long a user's cookie stays in the audience. Use the length of time for which you expect the ad to remain relevant. Customer lists don't expire unless you enter a value.

1. Click **[!UICONTROL Review and Save]**.

1. Review the settings. To change a setting, click **[!UICONTROL Edit]** in the applicable section.

1. Click **[!UICONTROL Create]**.

The ad network may take up to 24 hours to process the file. See the [Google Ads documentation on customer match and its limitations](https://support.google.com/displayvideo/answer/9539301).

## Create Google Ads customer match audiences from Adobe audiences {#audience-adobe-create}

*Advertisers with an Adobe Advertising-Adobe Audience Manager or Adobe Advertising-Adobe Analytics integration only*

Each [!DNL Adobe] audience can be used for only one [!DNL Google Ads] audience. Each new audience has the same name as the original [!DNL Adobe] audience.

1. Complete the prerequisites:

   1. Ask an [!DNL Adobe] administrator or account manager to enable customer match audiences for the advertiser.

   1. Implement the [Adobe Experience Platform Identity Service](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=ko){target="_blank"} version 2.0 or higher.

   1. Deploy the following tag as high as possible on the advertiser's webpages from which the audience should be tracked:

      `<script src="//pixel.everesttech.net/rlsa/<Advertising_Cloud_UserID>" type="text/javascript"> </script>`

      Replace `Advertising_Cloud_UserID` with the advertiser's unique numeric user ID.

   1. Have an authorized user [configure synchronization with the advertiser's organization account in Adobe CX Enterprise](/help/search-social-commerce/admin/sync-adobe-audiences.md).

1. In the main menu, click **[!UICONTROL Targeting] > [!UICONTROL Audiences]**, and then click the **[!UICONTROL Library]** tab.

1. Select **[!UICONTROL All Other Network]** from the **[!UICONTROL Network]** menu, and then click **[!UICONTROL Create Audience]**.

1. In **[!UICONTROL Basic Settings]**, select [!DNL Google Ads] and the account.

1. In **[!UICONTROL Data Source]**, select the Adobe audience option.

1. In **[!UICONTROL Adobe Audience]**, select one or more available segments. You can search the list.

   Segments already used for another [!DNL Google Ads] audience aren't available. If you select multiple segments, a separate audience is created for each segment.

1. Select the available customer list user ID option in **[!UICONTROL Audience Type]**.

1. Select the check box to indicate that you agree with the [!DNL Adobe] and ad network privacy policies.

1. Configure any remaining audience settings, including **[!UICONTROL Membership Days]** when available.

   Remarketing lists have a maximum duration of 540 days. Customer lists don't have a maximum duration; enter 10000 to indicate that the cookie never expires.

1. Click **[!UICONTROL Review and Save]**, review the settings, and then click **[!UICONTROL Create]**.

Search, Social, & Commerce automatically pushes a [!DNL Google] tracking URL back to each source segment so that [!DNL Google] can track the audience. [!DNL Google] may take up to 24 hours to process the audience.

>[!TIP]
>
>For real-time segmentation, use Audience Manager-created audiences. [!DNL Analytics] segments synced to Adobe CX Enterprise may have smaller populations because they're synced daily. Users who qualify for a segment may not be included until the next day.

## Create a Microsoft Advertising dynamic remarketing audience {#audience-dynamic-create}

You can create multiple dynamic remarketing audiences using the same tracking tag.

1. Implement the [Microsoft Advertising universal event tracking (UET) tag with the required product ID and page type parameters](https://help.ads.microsoft.com/#apex/ads/en/56910/1/#exp85) on the relevant webpages. Identify the tag's name.

1. In the main menu, click **[!UICONTROL Targeting] > [!UICONTROL Audiences]**, and then click the **[!UICONTROL Library]** tab.

1. Select **[!UICONTROL All Other Network]** from the **[!UICONTROL Network]** menu, and then click **[!UICONTROL Create Audience]**.

1. In **[!UICONTROL Basic Settings]**, select [!DNL Microsoft Advertising] and the account.

1. In **[!UICONTROL Data Source]**, select the dynamic remarketing list option.

1. Enter the **[!UICONTROL Audience Name]**.

1. In **[!UICONTROL Tag Name]**, select the UET tag on the webpages whose users comprise the audience.

1. In **[!UICONTROL Whom to add to your audience]**, select **[!UICONTROL General Visitors]**, **[!UICONTROL Product Searchers]**, **[!UICONTROL Product Viewers]**, **[!UICONTROL Past Buyers]**, or **[!UICONTROL Shopping Cart Abandoners]**.

1. Configure any remaining audience settings, including **[!UICONTROL Membership Days]** when available. For dynamic remarketing audiences, membership can range from 1-180 days.

1. Click **[!UICONTROL Review and Save]**, review the settings, and then click **[!UICONTROL Create]**.

Dynamic remarketing audiences are eligible for targeting once they include at least 300 users.

## Update a customer match audience using a customer data list {#audience-customer-list-edit}

You can update customer match audiences created from data files, but not [!DNL Google Ads] audiences created from [!DNL Adobe] audiences. You can add or delete members, or replace all existing members. You can't edit multiple library audiences at once.

1. Prepare a CSV file in the required format, using the same data type as the original list. For mobile device IDs, use the same app and operating system.

1. In the main menu, click **[!UICONTROL Targeting] > [!UICONTROL Audiences]**, and then click the **[!UICONTROL Library]** tab.

1. Select **[!UICONTROL All Other Network]** from the **[!UICONTROL Network]** menu.

1. Select the check box next to one audience, and then click **[!UICONTROL Edit]** in the bulk actions toolbar.

1. In **[!UICONTROL Select Action]**, select:

   * **[!UICONTROL Add]:** Add members from the uploaded file who aren't already in the audience.

   * **[!UICONTROL Delete]:** Remove members in the uploaded file from the audience.

   * **[!UICONTROL Replace]:** Replace all existing audience members with the uploaded data.

1. In **[!UICONTROL Select File]**, select the CSV file, accept the privacy policies, and configure the applicable consent setting.

1. Click **[!UICONTROL Upload File]** and wait for the upload to finish.

1. Click **[!UICONTROL Review and Save]**, review the settings, and then click **[!UICONTROL Update]**.

The ad network may take a while to process audience updates.

## Edit a dynamic remarketing audience {#audience-dynamic-edit}

You can change a [!DNL Microsoft Advertising] dynamic remarketing audience's name, UET tag, and visitor type. You can't change its membership duration or edit multiple library audiences at once.

1. In the main menu, click **[!UICONTROL Targeting] > [!UICONTROL Audiences]**, and then click the **[!UICONTROL Library]** tab.

1. Select **[!UICONTROL All Other Network]** from the **[!UICONTROL Network]** menu.

1. Select the check box next to one dynamic remarketing audience, and then click **[!UICONTROL Edit]** in the bulk actions toolbar.

1. Edit the **[!UICONTROL Audience Name]**, **[!UICONTROL Tag Name]**, or **[!UICONTROL Whom to add to your audience]**.

1. Click **[!UICONTROL Review and Save]**, review the settings, and then click **[!UICONTROL Update]**.
-->

## 동적 리마케팅 대상자 삭제 {#audience-delete}

동적 리마케팅 대상자를 한 번에 하나씩 [!DNL Microsoft Advertising]개 삭제할 수 있습니다. 라이브러리에서 다른 [!DNL Google Ads] 또는 [!DNL Microsoft Advertising] 대상 유형을 삭제할 수 없습니다.

1. 주 메뉴에서 **[!UICONTROL Targeting]>[!UICONTROL Audiences]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Library]** 탭을 클릭합니다.

1. **[!UICONTROL Network]** 메뉴에서 **[!UICONTROL All Other Network]**&#x200B;을(를) 선택합니다.

1. 하나의 동적 리마케팅 대상자 옆에 있는 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

## 선택한 행의 모든 데이터를 클립보드에 복사 {#copy-to-clipboard}

보기에 표시되는 적용된 필터 및 열에 따라 선택한 행에 표시되는 정보를 복사합니다. 정보는 탭으로 구분된 값(TSV)으로 저장됩니다.

1. 데이터를 복사할 각 행 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Copy]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [캠페인 및 광고 그룹에 대한 대상자 대상 관리](audience-targets-manage.md)
>* [캠페인 및 광고 그룹에 대한 대상자 제외 관리](audience-exclusions.md)
