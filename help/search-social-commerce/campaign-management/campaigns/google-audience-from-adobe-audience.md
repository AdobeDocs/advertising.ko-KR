---
title: ' [!DNL Adobe] 대상에서  [!DNL Google Ads] 고객 일치 대상 만들기'
description: 기존 Adobe Analytics 및 Audience Manager 대상에서  [!DNL Google Ads] 고객 일치 대상을 만드는 방법을 알아봅니다.
exl-id: 7de95ebb-24b0-459f-83c0-7b85b0c0576d
feature: Search Campaign Management
source-git-commit: d0f1c413134a0868ddec79ded7672af316267edd
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Adobe Analytics 및 Audience Manager 대상에서 [!DNL Google Ads]개의 고객 일치 대상 만들기

고객 일치 항목에만 적합한 계정 *[!DNL Google Ads]개*

*Adobe Advertising-Adobe Audience Manager 또는 Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

옵트인 광고주는 a) Adobe Experience Cloud과 공유되는 [!DNL Analytics] 세그먼트 및 b) Adobe Experience Cloud에 게시되는 [!DNL Analytics] 세그먼트와 Adobe Experience Cloud 대상 라이브러리를 사용하여 생성된 세그먼트를 포함하여 검색, 소셜 및 Commerce을 대상으로 하는 Audience Manager 세그먼트의 사용자 ID를 사용하여 [!DNL Google Ads] 고객 일치 대상을 만들 수 있습니다. Search, Social 및 Commerce은 [!DNL Google]이(가) 대상자를 추적할 수 있도록 [!DNL Google] 추적 URL을 각 [!DNL Analytics] 또는 Audience Manager 세그먼트로 자동으로 푸시합니다.

각 [!DNL Adobe] 대상은 하나의 [!DNL Google] 대상에만 사용할 수 있습니다.

각 새 [!DNL Google] 대상의 이름은 원래 [!DNL Adobe] 대상의 이름과 같습니다. [!DNL Google]은(는) 대상자를 타깃팅해야 하는 크기를 결정합니다.

>[!TIP]
>
>실시간 세그멘테이션의 경우 Audience Manager에서 만든 대상자를 사용합니다. [!DNL Analytics]에서 만들어져 Adobe Experience Cloud에 동기화된 세그먼트는 매일 동기화되기 때문에 인구가 더 적을 수 있습니다. 세그먼트 자격이 있는 서퍼는 다음 날까지 세그먼트에 포함되지 않을 수 있습니다. [!DNL Analytics]의 세그먼트에 &quot;보고서 세트 - &quot;의 데이터 소스가 있습니다.

>[!NOTE]
>
>Search, Social 및 Commerce은 [!DNL Google] 대상자를 만들거나 편집하는 데 사용되는 [!DNL Adobe] 세그먼트의 고객 데이터를 저장하지 않습니다.

1. 필요에 따라 사전 요구 사항을 완료합니다.

   1. (사용자 ID 리마케팅 목록 대상자를 만들려면) [!DNL Adobe] 관리자 사용자 또는 계정 관리자가 광고주 수준 설정을 선택하여 고객 일치 대상자를 활성화해야 합니다.

   1. [Adobe Experience Platform ID 서비스](https://experienceleague.adobe.com/docs/id-service/using/home.html) 버전 2.0 이상을 구현합니다.

   1. 대상자를 추적해야 하는 광고주의 웹 페이지에 가능한 한 높은 다음 태그를 배포합니다

      `<script src="//pixel.everesttech.net/rlsa/<Advertising_Cloud_UserID>" type="text/javascript"> </script>`

      여기서 `Advertising_Cloud_UserID`은(는) 광고주에게 할당된 고유한 숫자 사용자 ID입니다.

      예: `<script src="//pixel.everesttech.net/rlsa/1234" type="text/javascript"> </script>`

   1. (아직 완료되지 않은 경우) 승인된 사용자는 광고주의 계정을 [Adobe Experience Cloud의 광고주 조직 계정과 동기화](/help/search-social-commerce/admin/sync-adobe-audiences.md)하도록 구성해야 합니다.

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
>* [Adobe Campaign 전자 메일 목록에서 고객 일치 대상 만들기 [!DNL Google Ads] 2}](google-audience-from-campaign-email-list.md)
>* [고객 데이터 목록을 사용하여 고객 일치 대상 관리](audience-from-customer-data-list.md)
>* [동적 리마케팅 대상자 관리](audience-dynamic-remarketing-manage.md)
