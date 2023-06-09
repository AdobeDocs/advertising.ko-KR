---
title: 만들기 [!DNL Google Ads] 의 고객 일치 대상 [!DNL Adobe] 대상
description: 만드는 방법 알아보기 [!DNL Google Ads] 기존 Adobe Analytics의 대상과 Audience Manager 대상의 대상을 고객이 일치시킵니다.
source-git-commit: 7089f7fe75b551953026ac6cca4ac7aafa06ba7b
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# 만들기 [!DNL Google Ads] Adobe Analytics 및 Audience Manager 대상의 고객 일치

*[!DNL Google Ads]고객 대응에만 적합한 계정*

*Advertising-Adobe Audience Manager 또는 Adobe Advertising-Adobe Analytics 통합만 있는 Adobe*

옵트인 광고주가 다음을 만들 수 있습니다. [!DNL Google Ads] a)의 사용자 ID를 사용하는 고객 일치 [!DNL Analytics] Adobe Experience Cloud과 공유되는 세그먼트 및 b) 검색, 소셜, 상거래를 대상으로 하는 Audience Manager 세그먼트 [!DNL Analytics] Adobe Experience Cloud에 게시되는 세그먼트 및 Adobe Experience Cloud 대상 라이브러리를 사용하여 생성되는 세그먼트입니다. Search, Social 및 Commerce가 [!DNL Google] 각 URL로 다시 추적 [!DNL Analytics] 또는 세그먼트를 Audience Manager 하여 [!DNL Google] 대상자를 추적할 수 있습니다.

각 [!DNL Adobe] 대상은 한 개만 사용할 수 있습니다. [!DNL Google] 대상입니다.

새로 만들 때마다 [!DNL Google] audience의 이름이 original과 같습니다. [!DNL Adobe] 대상입니다. [!DNL Google] 대상자를 얼마나 많이 타깃팅해야 하는지 결정합니다.

>[!TIP]
>
>실시간 세그멘테이션의 경우 Audience Manager이 만든 대상자를 사용합니다. 다음에서 생성된 세그먼트 [!DNL Analytics] 및 Adobe Experience Cloud에 동기화되는 인구는 매일 동기화되기 때문에 더 적을 수 있습니다. 세그먼트에 대한 자격이 되는 서퍼는 다음 날까지 세그먼트에 포함되지 않을 수 있습니다. 의 세그먼트 [!DNL Analytics] &quot;보고서 세트 - .&quot;의 데이터 소스가 있습니다.

>[!NOTE]
>
>Search, Social 및 Commerce는 의 고객 데이터를 저장하지 않습니다. [!DNL Adobe] 세그먼트를 만들거나 편집하는 데 사용 [!DNL Google] 대상입니다.

1. 필요에 따라 사전 요구 사항을 완료합니다.

   1. (사용자 ID 리마케팅 목록 대상자를 만들려면) [!DNL Adobe] 관리자 사용자 또는 계정 관리자가 광고주 수준 설정을 선택하여 고객 일치 대상을 활성화해야 합니다. 설정은 Audience Manager이 있는 광고주와 가 있는 광고주마다 다릅니다. [!DNL Analytics] 만 해당.

   1. 구현 [Adobe Experience Platform ID 서비스](https://experienceleague.adobe.com/docs/id-service/using/home.html) 버전 2.0 이상

   1. 대상자를 추적해야 하는 광고주의 웹 페이지에 가능한 한 높은 다음 태그를 배포합니다

      `<script src="//pixel.everesttech.net/rlsa/<Advertising_Cloud_UserID>" type="text/javascript"> </script>`

      위치 `Advertising_Cloud_UserID` 는 광고주에게 할당된 고유 사용자 ID입니다. 예:  `<script src="//pixel.everesttech.net/rlsa/1234" type="text/javascript"> </script>`

   1. (아직 완료되지 않은 경우) 승인된 사용자는 광고주의 계정을 [Adobe Experience Cloud에서 광고주의 조직 계정과 동기화](/help/search-social-commerce/admin/sync-adobe-audiences.md).

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**. 하위 메뉴에서 **[!UICONTROL Live]> [!UICONTROL Audiences] >[!UICONTROL Library]**.

1. 데이터 테이블 위의 도구 모음에서 ![만들기](/help/search-social-commerce/assets/add.png "만들기").

1. 광고 네트워크와 계정 이름을 선택한 다음 **[!UICONTROL Continue]**.

1. 대상 정보를 지정합니다.

   1. 다음에서 **[!UICONTROL Data Source]** 메뉴, 선택 **[!UICONTROL Adobe Audience]**.

   1. 다음 항목 선택 [!UICONTROL Adobe Audience] 의 기반으로 사용할 [!DNL Google] 대상입니다.

      >[!NOTE]
      >
      >[!DNL Adobe] 다른 사용자에게 이미 사용된 대상 [!DNL Google] 대상을 사용할 수 없습니다.

      필요한 경우 최소 3자의 특정 텍스트 문자열이 포함된 대상을 검색할 수 있습니다. 일치하는 대상을 보려면 다음을 클릭하십시오. **[!UICONTROL Include]** 을 눌러 선택합니다.

      여러 개를 선택하는 경우 [!DNL Adobe] 대상, 별도의 항목 [!DNL Google] 대상자는 각각에 대해 생성됩니다.

   1. 다음 항목 선택 **[!UICONTROL Audience Type]** 만들려면 다음을 수행하십시오. **[!UICONTROL Customer List_User ID]**.

      광고주의 [!DNL Google Ads] 계정은 다음과 같아야 합니다. [사용자 정의 일치 가능](https://support.google.com/adspolicy/answer/6299717) 을(를) 위해 옵트인함 [사용자 ID 리마케팅](https://support.google.com/google-ads/answer/9199250).

   1. 확인란을 선택하여 약관에 동의함을 나타냅니다. [!DNL Adobe] 및 광고 네트워크 개인정보 처리방침.

   1. 의 수를 지정합니다. **[!UICONTROL Membership Days]**: 사용자 쿠키가 대상에 있는 일 수입니다.

      광고가 사용자와 관련이 있을 것으로 예상되는 시간을 사용합니다. 리마케팅 목록의 최대 기간은 540일입니다. 고객 목록에는 최대 기간이 없습니다. 쿠키가 만료되지 않음을 나타내려면 값을 10000.

   1. 클릭 **[!UICONTROL Post]**.

>[!NOTE]
>
>* [!DNL Google] 파일을 처리하는 데 최대 24시간이 소요될 수 있습니다.
>
>* 다음을 참조하십시오 [[!DNL Google Ads] 고객 일치 작동 방식 및 제한 사항에 대한 설명서](https://support.google.com/displayvideo/answer/9539301).

>[!MORELIKETHIS]
>
>* [대상자 기본 정보](audience-about.md)
>* [만들기 [!DNL Google Ads] Adobe Campaign 이메일 목록의 고객 일치 대상](google-audience-from-campaign-email-list.md)
>* [고객 데이터 목록을 사용하여 고객 일치 대상 관리](audience-from-customer-data-list.md)
>* [동적 리마케팅 대상자 관리](audience-dynamic-remarketing-manage.md)
