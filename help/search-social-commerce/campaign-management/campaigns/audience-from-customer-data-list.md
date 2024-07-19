---
title: 고객 데이터 목록을 사용하여 고객 일치 대상 관리
description: 고객 데이터 목록에서  [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 고객 일치 대상을 만들고 편집하는 방법을 알아봅니다.
exl-id: 594a7ee0-4ac9-4970-b53e-d4624fd7b70c
feature: Search Campaign Management
source-git-commit: 67fe8581832dc0762d62908d01672e53cc95b847
workflow-type: tm+mt
source-wordcount: '842'
ht-degree: 0%

---

# 고객 데이터 목록을 사용하여 [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 고객 일치 대상 관리

고객 데이터 목록에서 [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 고객 일치 대상을 만들 수 있습니다. [!DNL Adobe] 대상에서 만든 [!DNL Google Ads]개의 대상을 제외한 모든 [!DNL Google Ads] 또는 [!DNL Microsoft Advertising] 고객 일치 대상을 업데이트할 수도 있습니다.

## 고객 데이터 목록에서 고객 일치 대상 만들기

고객 일치 항목에만 적합한 *[!DNL Google Ads]및 [!DNL Microsoft Advertising] 계정*

CRM(고객 관계 관리) 시스템에서 생성한 데이터 파일에서 [!DNL Google Ads] 또는 [!DNL Microsoft Advertising] 고객 데이터 기반 목록을 만들 수 있습니다.

[!DNL Microsoft Advertising] 계정의 경우 파일에 전자 메일 주소를 포함할 수 있습니다. [!DNL Google Ads] 계정의 경우 파일에 전자 메일 주소, 우편 주소 또는 전화 번호, 사용자 ID 또는 CRM의 모바일 장치 ID가 포함될 수 있습니다.

>[!NOTE]
>
>Search, Social 및 Commerce은 업로드한 고객 데이터나 [!DNL Google Ads] 또는 [!DNL Microsoft Advertising] 대상자를 만들거나 편집하는 데 사용한 [!DNL Adobe] 세그먼트의 고객 데이터를 저장하지 않습니다.

1. 고객 데이터가 포함된 파일을 필요한 형식으로 생성합니다.

   이름과 성, 이메일 주소 및 전화 번호는 SHA-256 알고리즘을 사용하여 해시해야 합니다. <!-- Our UI says all, but GGL docs say don't hash user IDs and device IDs. --> [!DNL Google Ads]명의 대상자에 대해 허용된 연락처 정보 필드 및 요구 사항 목록을 보려면 &quot;[해시된 데이터를 업로드하기 위한 서식 지정 지침](https://support.google.com/google-ads/answer/7476159)&quot;의 [!DNL Google Ads] 설명서를 참조하십시오. [!DNL Microsoft Advertising]명의 대상자에 대해서는 [고객 일치 목록 준비](https://help.ads.microsoft.com/#apex/ads/en/56921)에 있는 [!DNL Microsoft Advertising] 설명서를 참조하십시오. 필요한 경우 연락처 정보에 대한 [!DNL Microsoft Excel] 템플릿을 다운로드할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다. 하위 메뉴에서 **[!UICONTROL Live]> [!UICONTROL Audiences] >[!UICONTROL Library]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위의 도구 모음에서 ![만들기](/help/search-social-commerce/assets/add.png "만들기")를 클릭합니다.

1. 광고 네트워크 및 계정 이름을 선택한 다음 **[!UICONTROL Continue]**&#x200B;을(를) 클릭합니다.

1. 대상 정보를 지정합니다.

   1. [!UICONTROL Data Source] 메뉴에서 **[!UICONTROL Customer List]**&#x200B;을(를) 선택합니다.

   1. **[!UICONTROL Audience Name]** 입력.

   1. 파일 업로드:

      1. [!UICONTROL Data Upload Type]: *[!UICONTROL Emails, Phones, and/or Mailing Addresses]*, *[!UICONTROL User IDs]* 또는 *[!UICONTROL Mobile Device IDs]*&#x200B;을(를) 선택하십시오.

         사용자 ID 옵션은 [사용자 ID 세그먼트](https://support.google.com/google-ads/answer/9199250)에 대해 옵트인된 미국의 [!DNL Google Ads]개 광고주에게만 제공됩니다

      1. (모바일 장치 ID 목록만 해당) **[!UICONTROL OS Type]**(*[!UICONTROL Android™]* 또는 *[!UICONTROL iOS]*)을(를) 선택하고 **[!UICONTROL App ID]**&#x200B;을(를) 입력합니다.

         앱 ID는 모바일 운영 체제에서 애플리케이션이 Google Play 또는 Apple App Store에 연결할 수 있도록 하는 데 사용하는 고유 식별자입니다.

         * ([!DNL Android™]개 앱) [!DNL Google Play] 내의 [!DNL Android™] 패키지 이름으로, &quot;`id=<package_name>`&quot;(으)로 식별됩니다.

           예를 들어 https://play.google.com/store/apps/details?id=com.example.game에서 패키지 이름은 com.example.game입니다.

         * ([!DNL iOS]개 앱) [!DNL iTunes App Store] 내의 응용 프로그램 ID로, URL 끝에 &quot;`<idNNNNNNNNN>`&quot;(으)로 식별됩니다. [!DNL iOS Developer Console]에서도 사용할 수 있습니다.

           예를 들어 https://itunes.apple.com/us/app/id284882215에서 ID는 id284882215입니다.

         개발 팀에서 관련 플랫폼에 대한 [!UICONTROL App ID]에 액세스할 수 있습니다.

      1. [!UICONTROL Select File] 필드에서 **[!UICONTROL Choose File]**&#x200B;을(를) 클릭하고 네트워크나 장치에서 파일을 선택합니다.

      1. [!DNL Adobe] 및 광고 네트워크 개인정보 처리방침 약관에 동의함을 나타내려면 확인란을 선택하십시오.

      1. (EEA(European Economic Area) 또는 영국(UK)에서 비즈니스를 수행하는 [!DNL Google Ads]명의 대상을 만드는 광고주; 선택 사항) EEA 및 영국 사용자로부터 광고 목적으로 데이터를 업로드하는 것에 대한 동의를 수집한 경우 **[!UICONTROL If you are doing business in EEA and/or UK, check this box to send consent status as GRANTED for the user data sent to [!DNL Google Ads] for advertising purposes. If left unchecked, we will send consent status as UNSPECIFIED for the user data sent to [!DNL Google Ads] for advertising purposes.]** 옆에 있는 확인란을 선택합니다

      [!DNL Google Ads]은(는) 지정되지 않은 동의 상태를 가진 EEA 및 영국 사용자에 대한 모든 데이터를 무시합니다. 이로 인해 데이터 불일치 및 성능 문제가 발생할 수 있습니다.

      1. **[!UICONTROL Upload File]**&#x200B;을(를) 클릭합니다.

   1. 사용자 쿠키가 대상에 있는 일 수인 **[!UICONTROL Membership Days]**&#x200B;을(를) 지정합니다.

   광고가 사용자와 관련이 있을 것으로 예상되는 시간을 사용합니다. 값을 입력하지 않으면 고객 목록이 만료되지 않습니다.

1. **[!UICONTROL Post]**&#x200B;을(를) 클릭합니다.

>[!NOTE]
>
>* 광고 네트워크에서 파일을 처리하는 데 최대 24시간이 걸릴 수 있습니다.
>* 고객 일치의 작동 방식과 제한 사항에 대해서는 [[!DNL Google Ads] 설명서를 참조하십시오](https://support.google.com/displayvideo/answer/9539301).

## 고객 데이터 목록을 사용하여 고객 일치 대상 편집

[!DNL Adobe] 대상에서 만든 [!DNL Google Ads]개의 대상을 제외한 모든 [!DNL Google Ads] 또는 [!DNL Microsoft Advertising] 고객 일치 대상을 업데이트할 수 있습니다. 대상에 대한 기존 데이터를 모두 추가, 삭제 또는 대체할 데이터를 업로드할 수 있습니다.

데이터는 원래 고객 목록(특정 모바일 운영 체제의 특정 앱에 대한 이메일 주소, 우편 주소, 전화 번호, 사용자 ID 또는 모바일 장치 ID)과 동일한 유형이어야 합니다.

1. 기존 데이터 유형에 필요한 형식으로 고객 데이터가 포함된 파일을 생성합니다.

이름과 성, 이메일 주소 및 전화 번호는 SHA-256 알고리즘을 사용하여 해시해야 합니다. <!-- Our UI says all, but GGL docs say don't hash user IDs and device IDs. --> [!DNL Google Ads]명의 대상자에 대해 허용된 연락처 정보 필드 및 요구 사항 목록을 보려면 &quot;[해시된 데이터를 업로드하기 위한 서식 지정 지침](https://support.google.com/google-ads/answer/7476159)&quot;의 [!DNL Google Ads] 설명서를 참조하십시오. [!DNL Microsoft Advertising]명의 대상자에 대해서는 [고객 일치 목록 준비](https://help.ads.microsoft.com/#apex/ads/en/56921)에 있는 [!DNL Microsoft Advertising] 설명서를 참조하십시오. 필요한 경우 연락처 정보에 대한 [!DNL Microsoft Excel] 템플릿을 다운로드할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다. 하위 메뉴에서 **[!UICONTROL Live]> [!UICONTROL Audiences] >[!UICONTROL Library]**&#x200B;을(를) 클릭합니다.

1. 편집할 대상 옆에 있는 확인란을 선택합니다.

1. 데이터 테이블 위의 도구 모음에서 ![편집](/help/search-social-commerce/assets/edit.png)을 클릭합니다.

1. *[!UICONTROL Add]*(업로드된 데이터가 존재하지 않는 경우 기존 데이터에 추가), *[!UICONTROL Delete]*(업로드된 데이터가 존재하는 경우 기존 데이터에서 삭제) 또는 *[!UICONTROL Replace]*(기존 데이터를 모두 삭제하고 업로드된 데이터로 바꾸기) 작업을 선택합니다.

1. 파일 업로드:

   1. [!UICONTROL Select File] 필드에서 **[!UICONTROL Choose File]**&#x200B;을(를) 클릭하고 네트워크나 장치에서 파일을 선택합니다.

   1. [!DNL Adobe] 및 광고 네트워크 개인정보 처리방침 약관에 동의함을 나타내려면 확인란을 선택하십시오.

   1. **[!UICONTROL Upload File]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Post]**&#x200B;을(를) 클릭합니다.

>[!NOTE]
>
>광고 네트워크는 대상에 대한 업데이트를 처리하는 데 시간이 걸릴 수 있습니다.

>[!MORELIKETHIS]
>
>* [대상자 정보](audience-about.md)
>* [고객 일치 대상자 만들기 [!DNL Google Ads] 출처 [!DNL Adobe] 대상자](google-audience-from-adobe-audience.md)
>* [Adobe Campaign 전자 메일 목록에서 고객 일치 대상 만들기 [!DNL Google Ads] 2}](google-audience-from-campaign-email-list.md)
>* [동적 리마케팅 대상자 관리](audience-dynamic-remarketing-manage.md)
