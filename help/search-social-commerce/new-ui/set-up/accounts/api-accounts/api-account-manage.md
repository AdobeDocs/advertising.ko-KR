---
title: (새 UI) 광고 네트워크 계정 관리
description: 광고 네트워크 API를 통해 동기화된 광고 네트워크에 대한 새 UI에서 계정 세부 사항을 설정하고 관리하는 방법에 대해 알아봅니다.
feature: Search Campaign Management
exl-id: a50b2943-7568-401c-be5b-ff6f62629488
source-git-commit: d6416dae58543e1287b7af7df44eada4be023731
workflow-type: tm+mt
source-wordcount: '2129'
ht-degree: 0%

---

# (새 UI) API 연결을 통해 광고 네트워크 계정을 관리합니다

<!-- Besides just logging into an account, do you have to make any other choices once you're logged in (such as to give speciic permissions to SSC?  And what about oAuth tokens -- do we still use them? -->

*Beta 기능*

<!-- Move out info about Naver into a separate page -->

다음은 검색, 소셜 및 Commerce이 광고 네트워크의 API를 사용하여 동기화하는 광고 네트워크 계정을 관리하는 지침입니다.

<!-- Move out info about Naver into a separate page -->

각 광고 네트워크에서 사용할 수 있는 기능에 대한 자세한 내용은 &quot;[지원되는 인벤토리](/help/search-social-commerce/introduction/supported-inventory.md)&quot;를 참조하십시오.

## 광고 네트워크 계정 세부 정보 만들기 {#create-account}

계정 동기화를 활성화하려면 계정 액세스 자격 증명과 추적 옵션을 포함하고 *활성화됨* 상태로 해당 계정 레코드를 만들어야 합니다.

>[!NOTE]
>
>광고 네트워크에서 실제 계정을 만들려면 광고 네트워크의 웹 사이트로 이동합니다.

1. 주 메뉴에서 **[!UICONTROL Setup]** \> **[!UICONTROL Accounts]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Create Account]**&#x200B;을(를) 클릭합니다.

1. 광고 네트워크 이름을 클릭한 다음 **[!UICONTROL Next]**&#x200B;을(를) 클릭합니다.

1. ([!DNL Yandex]을(를) 제외한 모든 광고 네트워크) 광고주의 자격 증명을 사용하여 광고 네트워크에 로그인합니다. &quot;이 계정에 대한 계정 추적&quot; 옵션을 선택합니다. 그런 다음 오른쪽 상단에서 **[!UICONTROL Next]**&#x200B;을(를) 클릭합니다.

1. [계정 설정](#account-settings-api) 지정:

   1. **[!UICONTROL Select Accounts]** 탭에서 일반 계정 설정을 지정합니다. [!DNL Yandex] 계정의 경우 계정 자격 증명을 지정하십시오.

   1. **[!UICONTROL Setup Tracking]** 탭을 클릭하고 추적 설정을 입력합니다.

   1. ([[!DNL Adobe Analytics for Advertising] 통합](/help/integrations/analytics/overview.md)을(를) 사용하는 광고주) **[!UICONTROL Set up Adobe Analytics]** 탭을 클릭하고 캠페인 활동 추적 및 보고에 사용할 모든 [!DNL Analytics] 보고 세트를 선택합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

   계정의 모든 캠페인에 대한 최근 비용 및 클릭 데이터는 검색, 소셜 및 Commerce 내에서 시간별로 업데이트됩니다. 기본적으로 데이터는 광고 네트워크에 따라 지난 5~10일 동안 사용할 수 있습니다. 그러나 필요한 경우 프로젝트 실행 팀이 최대 60일 동안의 데이터를 검색할 수 있습니다.

## 광고 네트워크 계정 세부 정보 편집 {#edit-account}

계정 설정을 다시 인증하여 연결을 새로 고치거나 권한을 업데이트하려면 계정에서 활동을 활성화하거나 비활성화하고, 계정에서 기본 추적 매개 변수를 변경하거나, 추적 및 보고에 사용할 [!DNL Analytics] 보고서 세트를 변경한 다음 계정 세부 정보를 편집합니다.

>[!NOTE]
>
>광고 네트워크에서 실제 계정을 편집하려면 광고 네트워크의 웹 사이트로 이동합니다.

1. 주 메뉴에서 **[!UICONTROL Setup]** \> **[!UICONTROL Accounts]**&#x200B;을(를) 클릭합니다.

1. 다음 방법 중 하나로 계정을 선택합니다.

   * 계정 이름 옆의 확인란을 선택한 다음 일괄 작업 도구 모음에서 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

   * 계정 이름 위에 커서를 놓고 **..**&#x200B;을 클릭한 다음 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. [계정 설정](#account-settings-api)을(를) 편집합니다.

   1. (선택 사항) **[!UICONTROL Account Details]** 탭에서 계정 세부 정보를 편집합니다.

   1. (선택 사항) **[!UICONTROL Setup Tracking]** 탭을 클릭하고 추적 설정을 편집합니다.

   1. (선택 사항, [[!DNL Adobe Analytics for Advertising] 통합](/help/integrations/analytics/overview.md)을 사용하는 광고주) **[!UICONTROL Set up Adobe Analytics]** 탭을 클릭하고 캠페인 활동 추적 및 보고에 사용할 [!DNL Analytics] 보고 세트를 편집하십시오.

   <!-- What are the repercussions of changing the suites? Timing of updated data? -->

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

   >[!NOTE]
   >
   >Search, Social 및 Commerce은 새 계정 데이터를 광고 네트워크의 데이터와 동기화해야 합니다. 이 문제는 하루에 한 번, 또는 검색, 소셜 및 Commerce이 광고 네트워크의 변경 사항을 감지하면 더 자주 자동으로 발생합니다.

## 광고 네트워크 계정 재인증 {#reauthenticate}

광고 네트워크 연결을 새로 고치거나 계정에 대한 권한을 업데이트하려면 계정을 다시 인증하십시오.

1. (동일한 브라우저 애플리케이션에서 동일한 광고 네트워크의 다른 계정에 로그인한 경우) 광고주의 계정이 아닌 다른 계정에서 로그아웃합니다.

1. 주 메뉴에서 **[!UICONTROL Setup]** \> **[!UICONTROL Accounts]**&#x200B;을(를) 클릭합니다.

<!-- For Bing and Yandex, the right-click menu includes "Re authenticate." Clarify why just those types -->

1. 다음 방법 중 하나로 계정을 선택합니다.

   * 계정 이름 옆의 확인란을 선택한 다음 일괄 작업 도구 모음에서 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

   * 계정 이름 위에 커서를 놓고 **..**&#x200B;을 클릭한 다음 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Account Details]** 탭에서 **[!UICONTROL Re authenticate]**&#x200B;을(를) 클릭하고 광고주의 자격 증명을 사용하여 광고 네트워크에 로그인합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 광고 네트워크 계정 활성화 또는 비활성화 {#enable-disable-account}

광고 네트워크 계정을 활성화하면 Search, Social 및 Commerce이 캠페인 데이터를 계정과 동기화하고(지원되는 경우) 포트폴리오의 캠페인에 대한 자동화된 입찰 및/또는 캠페인 예산을 푸시합니다. 광고 네트워크 계정을 비활성화하면 검색, 소셜 및 Commerce이 계정에서 모든 활동을 중지합니다. 계정이 활성화된 동안 수집된 데이터는 여전히 저장되지만 캠페인 관리 보기 및 보고서에는 계정이 비활성화된 기간에 대한 데이터가 포함되지 않습니다. 나중에 계정을 다시 활성화하여 계정으로 활동을 재개할 수 있습니다.

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

## 광고 네트워크 계정 설정 {#account-settings-api}

계정 설정은 광고 네트워크에 따라 다릅니다. 아래의 일부 설정은 표시되지 않을 수 있습니다.

<!--
 When you're creating new accounts only; not sure that you'll have anything to do here once you've authenticated

### Authenticate tab

-->

### [!UICONTROL Select Accounts]/[!UICONTROL Account Details] 탭

**[!UICONTROL Account Name]:** Search, Social 및 Commerce 내에서 계정에 대해 표시될 이름입니다.

>[!NOTE]
>
>Search, Social 및 Commerce-Adobe Analytics 통합이 있고 검색 계정의 이름을 변경한 경우, Adobe 계정 팀에 매핑을 업데이트하도록 요청하십시오.

**[!DNL [광고 네트워크] 계정]:**(계정을 만드는 동안 표시) 동기화할 광고 네트워크 계정입니다.

**[로그인 세부 정보]:**(Yandex 계정만 해당) 사용할 계정 자격 증명:

* **[!UICONTROL Login]:** 계정에 대한 API 액세스를 사용하도록 설정하는 로그인 이름 또는 ID입니다.

* **[!UICONTROL Password]:** 계정의 암호입니다.

* **[!UICONTROL Access Key]:** 사용할 개발자 계정에 대한 액세스 키입니다.

* **[!UICONTROL Application ID]:** 계정에 사용할 개발자 토큰입니다. 모든 [!DNL Yandex] 계정에 동일한 토큰이 사용됩니다.

* **[!UICONTROL Purse Campaign ID]:**([!DNL Yandex] 계정(공유 계정 설정만 사용 안 함, 선택 사항) 계정의 모든 광고 캠페인에 대한 비용을 지불하는 데 사용되는 캠페인의 숫자 ID입니다.

* **[!UICONTROL Finance Token]:**([!DNL Yandex]개의 계정에 공유 계정 설정만 비활성화됨, 선택 사항) 금융 관련 API 호출에 사용할 개발자 토큰(예: 포트폴리오 최적화에 필요한 경우 광고주 캠페인 간 전자 지갑에서 돈을 다시 할당하는 데 사용).

**[!UICONTROL Network Account ID]:**([!DNL Yandex]을(를) 제외한 모든 광고 네트워크) 광고 네트워크에서 할당한 계정 ID.

>[!NOTE]
>
>광고 네트워크 관리자 계정은 여기에서 지원되지 않습니다. [!DNL Microsoft Advertising]의 관리자 계정을 식별하려면 각각 기본 계정 ID 또는 MCC 계정 필드를 사용하십시오. [관리자 계정  [!DNL Google Ads] 의 자격 증명을 설정하려면](/help/search-social-commerce/admin/manager-accounts.md) \> [!UICONTROL Admin]&#x200B;(으)로 이동하십시오.[!UICONTROL Manager Accounts]

**[!UICONTROL Currency]:**(읽기 전용) 계정에 사용되는 통화의 약어입니다. 이 값은 레코드를 저장하면 광고 네트워크의 계정에 대해 구성된 통화로 자동으로 채워집니다.

**[!UICONTROL Time Zone]:** 광고주의 시간대입니다. 이 값은 레코드를 저장하면 광고주의 검색, 소셜 및 Commerce 계정에 대해 구성된 시간대로 자동으로 채워집니다.

**[!UICONTROL Login]:**(읽기 전용) 계정에 로그인하는 데 사용되는 사용자 계정입니다.

**[!UICONTROL Account Synchronization and Management]> [!UICONTROL Account Enabled]:** 검색, 소셜 및 Commerce은 캠페인 데이터를 계정과 동기화하고(지원되는 경우) 포트폴리오의 캠페인에 대한 자동 입찰 및/또는 캠페인 예산을 푸시합니다.

## [!UICONTROL Setup Tracking] 탭

<!-- This should be the name of the whole left side of options -- they're all enabled/disabled depending on whether you enable our tracking -->

**[!UICONTROL Search, Social, & Commerce Tracking]:** 추적을 사용할지 여부는 Adobe Advertising 전환 추적 서비스를 사용하십시오. 이 방법은 고유한 클릭 추적 ID를 생성하고, 사용자를 클라이언트의 랜딩 페이지로 보내기 전에 추적 목적으로 Adobe Advertising 서버로 리디렉션합니다. 이 메서드에는 선택적으로 사용자 지정할 수 있는 기본 추적 옵션이 있으며, 각 URL에 추가할 매개 변수를 지정할 수도 있습니다.

이 기능을 사용하려면 **[추적 사용]**&#x200B;을 켜세요.

>[!NOTE]
>
>* 이 설정을 변경하는 경우 계정에 대한 추적 URL을 다시 생성해야 합니다.
>* 캠페인 수준 추적 옵션은 계정 수준 설정을 무시합니다.

**[!UICONTROL Tracking Type]:**(검색, 소셜 및 Commerce 추적이 활성화된 경우) 최종 사용자를 최종 URL 또는 대상 URL로 리디렉션하는 방법입니다. 선택한 옵션은 계정 또는 캠페인의 모든 입찰 단위에 적용할 수 있습니다. 기본 계정 수준 설정은 광고주의 추적 설정에서 상속되고, 기본 캠페인 수준 설정은 계정 설정에서 상속됩니다.

* *[!UICONTROL Standard]:* 최종 사용자를 지정된 URL로 리디렉션합니다.

* *[!UICONTROL Token]:* 최종 사용자를 URL로 리디렉션하고 클릭(`ef_id`)에 대한 Search, Social 및 Commerce ID도 토큰으로 사용되는 쿼리 문자열 매개 변수로 기록합니다. 오프라인 트랜잭션을 보고하거나, 검색, 소셜 및 Commerce에서 Adobe Analytics과 데이터를 교환하거나, [!DNL Apple Safari] 브라우저 내에서 발생하는 모든 전환을 추적하려는 경우 이 옵션을 선택하십시오.

>[!NOTE]
>
>* [!UICONTROL Standard]에서 [!UICONTROL Token]&#x200B;(으)로 전환하거나 그 반대로 전환하는 경우 계정에 대한 추적 URL을 다시 생성해야 합니다.
>* 캠페인 수준에서 계정 수준 설정을 재정의할 수 있습니다.

**[!UICONTROL Auto Update]:**(검색, 소셜 및 Commerce 추적이 활성화된 경우) 브라우저 및 서버 간 호환성을 위해 추적 URL을 표준화합니다. 검색, 소셜 및 Commerce은 다음 동기화 동안 광고 네트워크에 다음을 자동으로 업로드합니다. (a) 추적 템플릿에 대한 검색, 소셜 및 Commerce 추적 매개 변수와 최종 URL에 추가된 동일한 매개 변수 또는 (b) 검색, 소셜 및 Commerce 추적 코드에 포함된 새 대상 URL. [Adobe Advertising-Adobe Analytics 통합](https://experienceleague.adobe.com/docs/advertising/integrations/analytics/overview.html?lang=ko) 및 서버측 AMO ID(s_kwcid) 구성이 있는 광고주의 경우 업로드에는 [&#x200B; 및 &#x200B;](/help/integrations/analytics/ids.md#amo-id) 계정에 대한 [!DNL Google Ads]AMO ID 매개 변수[!DNL Microsoft Advertising]도 포함됩니다. 기본 계정 수준 설정은 광고주의 추적 설정에서 상속됩니다. 캠페인 수준에서 계정 수준 설정을 재정의할 수 있습니다.

추적 URL은 동기화되지 않은 엔티티(즉, 추가된 새 엔티티 및 속성이 변경된 기존 엔티티)에 대해서만 매일 업데이트됩니다. 따라서 기존 광고주/계정/캠페인에 대해 이 설정을 비활성화에서 활성화로 변경하면 이미 동기화 중인 기존 엔티티에 대한 추적 URL이 업데이트되지 않습니다. 동기화 중인 기존 엔터티의 URL에 추적을 추가하려면 Adobe 계정 팀에 연락하여 1회 수동 동기화 프로세스를 요청하십시오. 자동 업로드 프로세스는 향후 변경 사항을 처리합니다.

**[!UICONTROL URL Encoding]:**(검색, 소셜 및 Commerce 추적이 활성화된 경우, 대상 URL만 있는 계정) 최종 사용자의 브라우저 주소 표시줄 내의 기본 URL을 인코딩합니다(`%3D` 대신 `=`).

**[!UICONTROL Tracking Level]:**(검색, 소셜 및 Commerce 추적이 활성화된 경우, 계정 및 캠페인 수준에서 사용할 수 있으며 병렬 추적이 활성화된 광고 네트워크에는 적용되지 않음) 리디렉션(관련 있는 경우)을 추가하고 관련 URL에 매개 변수를 추가하여 클릭 및 매출을 추적해야 하는 수준:

* *[!UICONTROL Keyword]:* 키워드 수준에서만 데이터를 추적합니다. [!DNL Yandex]에 사용할 수 없습니다.

* *[!UICONTROL Ad]:* 광고 수준에서만 데이터를 추적합니다. [!DNL Naver]에 사용할 수 없습니다.

* *[!UICONTROL Keyword and Ad]:* 키워드 및 광고 수준 모두에서 데이터를 추적하려면. [!DNL Naver] 및 [!DNL Yandex]에 사용할 수 없습니다.

**[!UICONTROL Landing Page Suffix]** ([!DNL Google Ads] 및 [!DNL Microsoft Advertising] 계정만 해당; 선택 사항) 정보를 추적하기 위해 최종 URL 끝에 추가할 모든 매개 변수. 비즈니스에서 추적해야 하는 모든 매개 변수를 포함합니다.

예: `param1=value1&param2=value2`

Adobe Advertising 클릭 추적을 사용하는 계정은 접미사에 광고 네트워크의 클릭 식별자(`msclkid`의 경우 [!DNL Microsoft Advertising], Google의 경우 `gclid`)를 포함해야 합니다. Adobe Analytics 통합이 있는 계정은 AMO ID 매개 변수(`s_kwcid`(으)로 시작)를 사용해야 합니다. 계정에 서버측 AMO ID 구현이 있는 경우 사용자가 광고를 클릭하면 매개 변수가 자동으로 추가됩니다. 그렇지 않으면 여기에 매개 변수를 수동으로 추가해야 합니다. [다음에 필요한 접미사 형식 [!DNL Google Ads]](/help/search-social-commerce/tracking/formats-click-tracking-google.md) 및 [다음에 필요한 접미사 형식 [!DNL Microsoft Advertising]](/help/search-social-commerce/tracking/formats-click-tracking-microsoft.md)을(를) 참조하십시오.

>[!NOTE]
>
>* 이 필드는 [!UICONTROL Auto Update] 추적 설정에 의해 업데이트되지 않습니다.
>* 하위 수준의 최종 URL 접미사는 계정 수준 접미사를 덮어씁니다. 간편하게 유지 관리할 수 있도록 개별 계정 구성 요소에 대해 다른 추적이 필요하지 않은 경우 계정 수준 접미사만 사용하십시오. 광고 그룹 수준 또는 하위 수준에서 접미사를 구성하려면 광고 네트워크의 편집기를 사용합니다.

**계정 추적 URL**: ([!DNL Google Ads], [!DNL Microsoft Advertising] 및 [!DNL Yahoo! Japan Ads] 계정만 해당; 선택 사항) 모든 랜딩 외부 도메인 리디렉션 및 추적 매개 변수를 지정하고 매개 변수에 최종/랜딩 페이지 URL도 임베드하는 계정의 기본 추적 템플릿입니다. 예: 리디렉션을 포함하는 `{lpurl}?source={network}&id=5` 또는 `http://www.trackingservice.example.com/?url={lpurl}?source={network}&id=5`.

* 최종 URL을 포함하려면 다음을 수행하십시오.

   * ([!DNL Google Ads] 및 [!DNL Microsoft Advertising]만 해당) 추적 템플릿의 최종 URL을 나타내는 매개 변수 목록은 [!DNL Microsoft Advertising]설명서[[!DNL Microsoft Advertising] 의 &quot;사용 가능한 &#x200B;](https://help.ads.microsoft.com/#apex/3/en/56799) 매개 변수&quot;에 대한 섹션에서 ([!DNL Google Ads]만 해당) [!DNL ValueTrack]설명서[[!DNL Google Ads]  또는 (](https://support.google.com/google-ads/answer/6305348)만 해당) &quot;추적 템플릿 전용&quot; 매개 변수를 참조하십시오.

   * ([!DNL Yahoo! Japan Ads]만 해당) `!{lpurl}` 매개 변수를 사용하여 랜딩 페이지 URL을 나타냅니다.

* 필요에 따라 URL 매개 변수와 캠페인에 대해 정의된 사용자 지정 매개 변수를 앰퍼샌드(&amp;)로 구분하여 포함할 수 있습니다(예: `{lpurl}?matchtype={matchtype}&device={device}`).

* 원할 경우 서드파티 리디렉션 및 추적을 추가할 수 있습니다.

* 캠페인 설정에 &quot;[!UICONTROL EF Redirect]&quot; 및 &quot;[!UICONTROL Auto Upload]&quot;이(가) 포함된 경우 레코드를 저장할 때 Search, Social 및 Commerce에 자체 리디렉션 및 추적 코드 접두사가 자동으로 추가됩니다.

>[!NOTE]
>
>* [!DNL Google Ads]의 경우 병렬 추적을 활성화하는 소스의 클릭에 대체되지 않는 매크로를 사용하지 마십시오. 광고주가 매크로를 사용해야 하는 경우 Adobe 계정 팀은 고객 지원 팀 또는 구현 팀과 협력하여 매크로를 추가해야 합니다.
>* 가장 세분화된 수준의 추적 템플릿은 모든 상위 수준의 값을 재정의합니다. 예를 들어 계정 설정과 키워드 설정 모두에 값이 포함된 경우 키워드 값이 적용됩니다.
>* 광고, 사이트링크 또는 키워드 수준에서 추적 템플릿을 업데이트하는 경우 관련 광고가 다시 제출되어 검토됩니다. 승인을 위해 광고를 다시 제출하지 않고도 계정, 캠페인 또는 광고 그룹 수준에서 추적 템플릿을 업데이트할 수 있습니다.

## [!UICONTROL Setup Analytics] 탭

**[!UICONTROL Adobe Analytics Report Suite]:**(Advertisers with an [[!DNL Adobe Analytics for Advertising] integration](/help/integrations/analytics/overview.md); 선택 사항) Search, Social 및 Commerce이 개체 분류 및 계정에 대한 클릭 데이터를 포함하여 광고 네트워크에서 수집하는 데이터를 전송하는 하나 이상의 Analytics 보고서 세트입니다. 이 기능은 지원되는 광고 네트워크에서만 사용할 수 있습니다.

데이터를 보고서 세트에 표시하려면 (a) 계정에 대해 서버측 AMO ID 기능을 구성해야 하거나 (b) &quot;[!UICONTROL Enable Advertising reporting in Analytics]&quot;에 대한 광고주 수준 설정을 활성화해야 합니다. 또한 Search, Social 및 Commerce에서 데이터를 수신하도록 광고주의 [!DNL Analytics] 계정을 구성해야 합니다. 자세한 내용은 Adobe 계정 팀에 문의하십시오.

>[!MORELIKETHIS]
>
>* [광고 네트워크 계정 정보](../ad-network-account-about.md)
>* [판매자 센터 계정 관리](/help/search-social-commerce/campaign-management/accounts/merchant-account-manage.md)
>* [a [!DNL Google Ads] account](/help/search-social-commerce/campaign-management/accounts/update-amo-id-google.md)에 대한 s_kwcid 추적 코드 업데이트
