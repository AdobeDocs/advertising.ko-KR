---
title: 고객 데이터 목록을 사용하여 고객 일치 대상 관리
description: 만들고 편집하는 방법 알아보기 [!DNL Google Ads] 및 [!DNL Microsoft® Advertising] 고객 데이터 목록의 고객 일치 대상입니다.
exl-id: 594a7ee0-4ac9-4970-b53e-d4624fd7b70c
feature: Search Campaign Management
source-git-commit: 588b6b5887903e5912fc68a18ef142d908026870
workflow-type: tm+mt
source-wordcount: '842'
ht-degree: 0%

---

# 관리 [!DNL Google Ads] 및 [!DNL Microsoft® Advertising] 고객 데이터 목록을 사용하는 고객 일치

다음을 만들 수 있습니다. [!DNL Google Ads] 및 [!DNL Microsoft® Advertising] 고객 데이터 목록의 고객 일치 대상입니다. 다음 항목을 업데이트할 수도 있습니다. [!DNL Google Ads] 또는 [!DNL Microsoft® Advertising] 다음을 제외한 고객 일치 대상 [!DNL Google Ads] 에서 생성된 대상자 [!DNL Adobe] 대상입니다.

## 고객 데이터 목록에서 고객 일치 대상 만들기

*[!DNL Google Ads]및 [!DNL Microsoft® Advertising] 고객 대응에만 적합한 계정*

다음을 만들 수 있습니다. [!DNL Google Ads] 또는 [!DNL Microsoft® Advertising] CRM(고객 관계 관리) 시스템에서 생성한 데이터 파일의 고객 데이터 기반 목록입니다.

대상 [!DNL Microsoft® Advertising] 계정에는 이메일 주소가 포함될 수 있습니다. 대상 [!DNL Google Ads] 계정에는 전자 메일 주소, 우편 주소 또는 전화 번호, 사용자 ID 또는 CRM의 모바일 장치 ID가 포함될 수 있습니다.

>[!NOTE]
>
>Search, Social 및 Commerce는 업로드한 고객 데이터나 [!DNL Adobe] 세그먼트를 만들거나 편집하는 데 사용 [!DNL Google Ads] 또는 [!DNL Microsoft® Advertising] 대상입니다.

1. 고객 데이터가 포함된 파일을 필요한 형식으로 생성합니다.

   이름과 성, 이메일 주소 및 전화 번호는 SHA-256 알고리즘을 사용하여 해시해야 합니다. <!-- Our UI says all, but GGL docs say don't hash user IDs and device IDs. --> 대상 [!DNL Google Ads] 대상, 다음을 참조하십시오. [!DNL Google Ads] 설명서에 대한[해시된 데이터 업로드를 위한 서식 지정 지침](https://support.google.com/google-ads/answer/7476159)허용된 연락처 정보 필드 및 요구 사항 목록에 대해 설명합니다. 대상 [!DNL Microsoft® Advertising] 대상, 다음을 참조하십시오. [!DNL Microsoft® Advertising] 설명서 [고객 일치 목록 준비](https://help.ads.microsoft.com/#apex/ads/en/56921. 선택적으로 다음을 다운로드할 수 있습니다. [!DNL Microsoft® Excel] 연락처 정보에 대한 템플릿입니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**. 하위 메뉴에서 **[!UICONTROL Live]> [!UICONTROL Audiences] >[!UICONTROL Library]**.

1. 데이터 테이블 위의 도구 모음에서 ![만들기](/help/search-social-commerce/assets/add.png "만들기").

1. 광고 네트워크와 계정 이름을 선택한 다음 **[!UICONTROL Continue]**.

1. 대상 정보를 지정합니다.

   1. 다음에서 [!UICONTROL Data Source] 메뉴, 선택 **[!UICONTROL Customer List]**.

   1. 다음을 입력합니다. **[!UICONTROL Audience Name]**.

   1. 파일 업로드:

      1. 다음 항목 선택 [!UICONTROL Data Upload Type]: *[!UICONTROL Emails, Phones, and/or Mailing Addresses]*, *[!UICONTROL User IDs]*, 또는 *[!UICONTROL Mobile Device IDs]*.

         사용자 ID 옵션은 다음 경우에만 사용할 수 있습니다. [!DNL Google Ads] 미국에 옵트인된 광고주 [사용자 ID 세그먼트](https://support.google.com/google-ads/answer/9199250)

      1. (모바일 장치 ID 목록만 해당) **[!UICONTROL OS Type]** (*[!UICONTROL Android™]* 또는 *[!UICONTROL iOS]*)을 입력하고 **[!UICONTROL App ID]**.

         앱 ID는 모바일 운영 체제에서 애플리케이션이 Google Play 또는 Apple App Store에 연결할 수 있도록 하는 데 사용하는 고유 식별자입니다.

         * ([!DNL Android™] apps) [!DNL Android™] 내의 패키지 이름 [!DNL Google Play], 다음에 의해 식별됨:`id=<package_name>`.&quot;

           예를 들어 https://play.google.com/store/apps/details?id=com.example.game에서 패키지 이름은 com.example.game입니다.

         * ([!DNL iOS] apps) 내의 애플리케이션 ID [!DNL iTunes App Store], 다음에 의해 식별됨:`<idNNNNNNNNN>`URL의 끝에 있는 &quot;를 클릭합니다. 또한 다음에서도 사용할 수 있습니다. [!DNL iOS Developer Console].

           예를 들어 https://itunes.apple.com/us/app/id284882215에서 ID는 id284882215입니다.

         개발팀은에 액세스할 수 있습니다. [!UICONTROL App ID] 관련 플랫폼.

      1. 다음에서 [!UICONTROL Select File] 필드, 클릭 **[!UICONTROL Choose File]** 네트워크 또는 장치에서 파일을 선택합니다.

      1. 확인란을 선택하여 약관에 동의함을 나타냅니다. [!DNL Adobe] 및 광고 네트워크 개인정보 처리방침.

      1. (광고주 만들기 [!DNL Google Ads] 유럽 경제 지역(EEA) 또는 영국(영국)에서 비즈니스를 수행하는 대상(선택 사항) EEA 및 영국 사용자로부터 광고 목적으로 데이터를 업로드하는 것에 대한 동의를 확보한 경우 다음 옆에 있는 확인란을 선택합니다. **[!UICONTROL If you are doing business in EEA and/or UK, check this box to send consent status as GRANTED for the user data sent to [!DNL Google Ads] for advertising purposes. If left unchecked, we will send consent status as UNSPECIFIED for the user data sent to [!DNL Google Ads] for advertising purposes.]**

      [!DNL Google Ads] 은 지정되지 않은 동의 상태가 있는 EEA 및 영국 사용자에 대한 모든 데이터를 무시합니다. 이로 인해 데이터 불일치 및 성능 문제가 발생할 수 있습니다.

      1. 클릭 **[!UICONTROL Upload File]**.

   1. 의 수를 지정합니다. **[!UICONTROL Membership Days]**: 사용자 쿠키가 대상에 있는 일 수입니다.

   광고가 사용자와 관련이 있을 것으로 예상되는 시간을 사용합니다. 값을 입력하지 않으면 고객 목록이 만료되지 않습니다.

1. 클릭 **[!UICONTROL Post]**.

>[!NOTE]
>
>* 광고 네트워크에서 파일을 처리하는 데 최대 24시간이 걸릴 수 있습니다.
>* 다음을 참조하십시오 [[!DNL Google Ads] 고객 일치 작동 방식 및 제한 사항에 대한 설명서](https://support.google.com/displayvideo/answer/9539301).

## 고객 데이터 목록을 사용하여 고객 일치 대상 편집

다음을 업데이트할 수 있습니다. [!DNL Google Ads] 또는 [!DNL Microsoft® Advertising] 다음을 제외한 고객 일치 대상 [!DNL Google Ads] 에서 생성된 대상자 [!DNL Adobe] 대상입니다. 대상에 대한 기존 데이터를 모두 추가, 삭제 또는 대체할 데이터를 업로드할 수 있습니다.

데이터는 원래 고객 목록(특정 모바일 운영 체제의 특정 앱에 대한 이메일 주소, 우편 주소, 전화 번호, 사용자 ID 또는 모바일 장치 ID)과 동일한 유형이어야 합니다.

1. 기존 데이터 유형에 필요한 형식으로 고객 데이터가 포함된 파일을 생성합니다.

이름과 성, 이메일 주소 및 전화 번호는 SHA-256 알고리즘을 사용하여 해시해야 합니다. <!-- Our UI says all, but GGL docs say don't hash user IDs and device IDs. --> 대상 [!DNL Google Ads] 대상, 다음을 참조하십시오. [!DNL Google Ads] 설명서에 대한[해시된 데이터 업로드를 위한 서식 지정 지침](https://support.google.com/google-ads/answer/7476159)허용된 연락처 정보 필드 및 요구 사항 목록에 대해 설명합니다. 대상 [!DNL Microsoft® Advertising] 대상, 다음을 참조하십시오. [!DNL Microsoft® Advertising] 설명서 [고객 일치 목록 준비](https://help.ads.microsoft.com/#apex/ads/en/56921. 선택적으로 다음을 다운로드할 수 있습니다. [!DNL Microsoft® Excel] 연락처 정보에 대한 템플릿입니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**. 하위 메뉴에서 **[!UICONTROL Live]> [!UICONTROL Audiences] >[!UICONTROL Library]**.

1. 편집할 대상 옆에 있는 확인란을 선택합니다.

1. 데이터 테이블 위의 도구 모음에서 ![편집](/help/search-social-commerce/assets/edit.png).

1. 작업을 선택합니다. *[!UICONTROL Add]* 업로드한 데이터가 이미 존재하지 않는 한 기존 데이터에 추가하려면, *[!UICONTROL Delete]* (업로드된 데이터가 이미 있는 경우 기존 데이터에서 삭제) 또는 *[!UICONTROL Replace]* (기존 데이터를 모두 삭제하고 업로드된 데이터로 대체합니다.)

1. 파일 업로드:

   1. 다음에서 [!UICONTROL Select File] 필드, 클릭 **[!UICONTROL Choose File]** 네트워크 또는 장치에서 파일을 선택합니다.

   1. 확인란을 선택하여 약관에 동의함을 나타냅니다. [!DNL Adobe] 및 광고 네트워크 개인정보 처리방침.

   1. 클릭 **[!UICONTROL Upload File]**.

1. 클릭 **[!UICONTROL Post]**.

>[!NOTE]
>
>광고 네트워크는 대상에 대한 업데이트를 처리하는 데 시간이 걸릴 수 있습니다.

>[!MORELIKETHIS]
>
>* [대상자 기본 정보](audience-about.md)
>* [만들기 [!DNL Google Ads] 의 고객 일치 대상 [!DNL Adobe] 대상](google-audience-from-adobe-audience.md)
>* [만들기 [!DNL Google Ads] Adobe Campaign 이메일 목록의 고객 일치 대상](google-audience-from-campaign-email-list.md)
>* [동적 리마케팅 대상자 관리](audience-dynamic-remarketing-manage.md)
