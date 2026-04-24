---
title: Create [!DNL Google Ads] customer match audiences from [!DNL Adobe] audiences
description: Learn how to create [!DNL Google Ads] customer match audiences from your existing Adobe Analytics and Audience Manager audiences.
exl-id: 7de95ebb-24b0-459f-83c0-7b85b0c0576d
feature: Search Campaign Management
TQID: https://experienceleague.adobe.com/Ep3X-eo2kcGlW3NsV3CJEKBkEapa-oAv0HLexc1xnhM
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2:
  - id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 7845129ba6566c1aaaf160cc6f9ad33bf1731f75
workflow-type: tm+mt
source-wordcount: 586
ht-degree: 0%

---

# Create [!DNL Google Ads] customer match audiences from Adobe Analytics and Audience Manager audiences

*[!DNL Google Ads]accounts that are eligible for customer match only*

*Adobe Advertising-Adobe Audience Manager 또는 Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

Opted-in advertisers can create [!DNL Google Ads] customer match audiences using user IDs from a) [!DNL Analytics] segments that are shared with Adobe CX Enterprise and b) Audience Manager segments that have Search, Social, &amp; Commerce as a destination, including [!DNL Analytics] segments that are published to Adobe CX Enterprise and segments that are created using the Adobe CX Enterprise Audience Library. Search, Social, &amp; Commerce automatically pushes a [!DNL Google] tracking URL back to each [!DNL Analytics] or Audience Manager segment so that [!DNL Google] can track the audience.

Each [!DNL Adobe] audience can be used for only one [!DNL Google] audience.

Each new [!DNL Google] audience has the same name as the original [!DNL Adobe] audience. [!DNL Google] determines how large the audience must be to be targetable.

>[!TIP]
>
>For real-time segmentation, use Audience Manager-created audiences. Segments created in [!DNL Analytics] and synced to Adobe CX Enterprise may have smaller populations because they&#39;re only synced daily; a surfer who qualifies for a segment may not be included in the segment until the next day. Segments from [!DNL Analytics] have a data source of &quot;report suite - .&quot;

>[!NOTE]
>
>Search, Social, &amp; Commerce doesn&#39;t store any of the customer data from your [!DNL Adobe] segments used to create or edit a [!DNL Google] audience.

1. Complete the prerequisites as needed:

   1. (To create user ID remarketing list audiences) An [!DNL Adobe] admin user or account manager must select the advertiser-level setting to enable customer match audiences.

   1. Implement the [Adobe Experience Platform Identity Service](https://experienceleague.adobe.com/docs/id-service/using/home.html) version 2.0 or higher.

   1. Deploy the following tag as high as possible on the advertiser&#39;s webpages from which the audience should be tracked

      `<script src="//pixel.everesttech.net/rlsa/<Advertising_Cloud_UserID>" type="text/javascript"> </script>`

      where `Advertising_Cloud_UserID` is the unique numeric user ID assigned to the advertiser.

      Example: `<script src="//pixel.everesttech.net/rlsa/1234" type="text/javascript"> </script>`

   1. (If not already completed) An authorized user must configure the advertiser&#39;s account to [sync with the advertiser&#39;s organization account in Adobe CX Enterprise](/help/search-social-commerce/admin/sync-adobe-audiences.md).

1. 메인 메뉴에서 **[!UICONTROL Search, Social, & Commerce]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다. 하위 메뉴에서 **[!UICONTROL Live]> [!UICONTROL Audiences] >[!UICONTROL Library]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위의 도구 모음에서 ![만들기](/help/search-social-commerce/assets/add.png "만들기")를 클릭합니다.

1. 광고 네트워크 및 계정 이름을 선택한 다음 **[!UICONTROL Continue]**&#x200B;을(를) 클릭합니다.

1. 대상 정보를 지정합니다.

   1. **[!UICONTROL Data Source]** 메뉴에서 **[!UICONTROL Adobe Audience]**&#x200B;을(를) 선택합니다.

   1. [!DNL Google] 대상을 기준으로 할 [!UICONTROL Adobe Audience]을(를) 선택하십시오.

      >[!NOTE]
      >
      >다른 [!DNL Google] 대상에 이미 사용된 [!DNL Adobe]개의 대상은 사용할 수 없습니다.

      필요한 경우 최소 3자의 특정 텍스트 문자열이 포함된 대상을 검색할 수 있습니다. 일치하는 대상을 선택하려면 **[!UICONTROL Include]**&#x200B;을(를) 클릭하십시오.

      여러 [!DNL Adobe]개의 대상을 선택하면 각각에 대해 별도의 [!DNL Google]개의 대상이 만들어집니다.

   1. 만들 **[!UICONTROL Audience Type]** 선택: **[!UICONTROL Customer List_User ID]**.

      광고주의 [!DNL Google Ads] 계정은 [사용자 지정 일치에 적합](https://support.google.com/adspolicy/answer/6299717)해야 하며 [사용자 ID 리마케팅](https://support.google.com/google-ads/answer/9199250)을 옵트인해야 합니다.

   1. [!DNL Adobe] 약관 및 광고 네트워크 개인정보 처리방침에 동의함을 나타내려면 확인란을 선택하십시오.

   1. 사용자 쿠키가 대상에 있는 일 수인 **[!UICONTROL Membership Days]**&#x200B;을(를) 지정합니다.

      광고가 사용자와 관련이 있을 것으로 예상되는 시간을 사용합니다. 리마케팅 목록의 최대 기간은 540일입니다. 고객 목록에는 최대 기간이 없습니다. 쿠키가 만료되지 않음을 나타내려면 값을 10000.

   1. **[!UICONTROL Post]**&#x200B;을(를) 클릭합니다.

>[!NOTE]
>
>* [!DNL Google]에서 파일을 처리하는 데 최대 24시간이 걸릴 수 있습니다.
>
>* 고객 일치의 작동 방식과 제한 사항에 대해서는 [[!DNL Google Ads] 설명서를 참조하십시오](https://support.google.com/displayvideo/answer/9539301).

>[!MORELIKETHIS]
>
>* [대상자 정보](audience-about.md)
>* [Adobe Campaign 전자 메일 목록에서 고객 일치 대상 만들기 [!DNL Google Ads] 2&rbrace;](google-audience-from-campaign-email-list.md)
>* [고객 데이터 목록을 사용하여 고객 일치 대상 관리](audience-from-customer-data-list.md)
>* [동적 리마케팅 대상자 관리](audience-dynamic-remarketing-manage.md)
