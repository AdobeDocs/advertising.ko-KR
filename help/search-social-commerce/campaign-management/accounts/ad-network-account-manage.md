---
title: 광고 네트워크 계정 관리
description: 광고 네트워크 계정에 대한 계정 세부 정보를 설정하고 관리하는 방법을 알아봅니다.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '2088'
ht-degree: 0%

---

# 광고 네트워크 계정 관리

다음은 광고 네트워크 계정 세부 사항을 만들고 편집하고 [!DNL oAuth] 계정용 토큰 및 계정 비활성화

## 광고 네트워크 계정 세부 정보 만들기 {#create-account}

*에이전시 계정 관리자, Adobe 계정 관리자 및 관리자 사용자 역할만 해당*

계정 동기화 또는 추적을 활성화하려면 계정 액세스 자격 증명 및 추적 옵션이 포함되고 상태가 인 해당 계정 레코드를 만들어야 합니다 *활성*. 각 광고 네트워크에 사용할 수 있는 기능에 대한 자세한 내용은 &quot;[지원되는 인벤토리](/help/search-social-commerce/introduction/supported-inventory.md).&quot;

>[!NOTE]
>
>광고 네트워크에서 실제 계정을 만들려면 광고 네트워크의 웹 사이트로 이동합니다.

1. 메인 메뉴에서 **[!UICONTROL Search]** \> **[!UICONTROL Campaigns]** \> **[!UICONTROL Campaigns]**. 하위 메뉴에서 **[!UICONTROL Live]** \> **[!UICONTROL Accounts]**.

1. 데이터 테이블 위의 도구 모음에서 ![만들기](/help/search-social-commerce/assets/add.png "만들기").

1. 다음을 지정합니다. [계정 설정](#account-settings):

   1. 광고 네트워크의 이름을 클릭한 다음 를 클릭합니다 **[!UICONTROL Next]**.

   1. 다음에서 **[!UICONTROL Account Details]** 섹션에서 계정 세부 정보를 입력합니다.

      로그인 인증 유형 을 사용하는 광고 네트워크의 경우 &quot;[!UICONTROL oAuth],&quot; 검색, 소셜 및 상거래를 통해 [OAuth 인증 프로토콜](http://tools.ietf.org/html/draft-ietf-oauth-v2-22):

      1. 다음을 입력합니다. **[!UICONTROL Login]** 계정 값을 입력하고 필요한 경우 암호를 입력한 다음 **[!UICONTROL Authenticate]**.

         가장 좋은 방법은 계정에 대한 API 액세스에 로그인을 사용하는 것입니다. 암호화하고 저장할 때 Adobe 계정 팀이 필요에 따라 토큰을 새로 고칠 수 있도록 암호를 입력합니다.

      1. (광고주의 계정에 로그인하지 않은 경우) 광고주의 광고 계정에 로그인합니다. 가장 좋은 방법은 계정에 대한 API 액세스에 자격 증명을 사용하는 것입니다.

      1. 권한/액세스 요청 화면에서 버튼을 클릭하여 권한을 확인합니다.

      1. 열려 있는 팝업 창에서 인증 문자열을 복사하고 문자열을 **[!UICONTROL oAuth Token]** 필드.

      1. 나머지 계정 세부 정보를 지정합니다.
   1. 클릭 **[!UICONTROL Set Account Tracking]**&#x200B;을 클릭하고 추적 설정을 입력합니다.


1. 클릭 **[!UICONTROL Post]**.

   계정의 모든 캠페인에 대한 최근 비용 및 클릭 데이터는 약 24시간 내에 검색, 소셜 및 상거래 내에서 사용할 수 있습니다. 기본적으로 데이터는 광고 네트워크에 따라 지난 5~10일 동안 사용할 수 있습니다. 그러나 필요한 경우 프로젝트 실행 팀이 최대 60일 동안의 데이터를 검색할 수 있습니다.

## 광고 네트워크 계정 세부 정보 편집 {#edit-account}

*에이전시 계정 관리자, Adobe 계정 관리자 및 관리자 사용자 역할만 해당*

계정 자격 증명이 변경되면 계정에서 기본 추적 매개 변수를 변경하거나 계정에 대한 활동을 활성화하거나 비활성화한 다음 계정 세부 정보를 편집합니다.

>[!NOTE]
>
>광고 네트워크에서 실제 계정을 편집하려면 광고 네트워크의 웹 사이트로 이동합니다.

1. 메인 메뉴에서 **[!UICONTROL Search]** \> **[!UICONTROL Campaigns]** \> **[!UICONTROL Campaigns]**. 하위 메뉴에서 **[!UICONTROL Live]** \> **[!UICONTROL Accounts]**.

1. 계정 이름 위에 커서를 놓고 ![자세히](/help/search-social-commerce/assets/more-filters.png "자세히")을 선택한 다음 을 선택합니다 **[!UICONTROL Edit]**.

1. 편집 [계정 설정](#account-settings):

   1. (선택 사항) 계정 세부 사항을 편집합니다.

   1. (선택 사항) **[!UICONTROL Set Account Tracking]**&#x200B;을 클릭하고 추적 설정을 편집합니다.

1. 클릭 **[!UICONTROL Post]**.

   >[!NOTE]
   >
   >Search, Social 및 Commerce는 새 계정 데이터를 광고 네트워크의 데이터와 동기화해야 합니다. 이 문제는 하루에 한 번 자동으로 발생하며, 검색, 소셜 및 상거래에서 광고 네트워크의 변경 사항을 감지하면 더 자주 발생합니다.

## 검색 계정에 대한 oAuth 액세스 토큰 새로 고침 {#refresh-oauth-tokens}

*에이전시 계정 관리자, Adobe 계정 관리자 및 관리자 사용자 역할만 해당*

검색, Social 및 Commerce가 [OAuth 인증 프로토콜](http://tools.ietf.org/html/draft-ietf-oauth-v2-22) 계정 자격 증명이 변경되거나 검색, 소셜 및 상거래의 새로운 기능을 지원하기 위해 추가 액세스가 필요한 경우 계정에 대한 새 액세스 토큰을 받아야 합니다.

새 기능에 새 토큰이 필요한 경우 Adobe 계정 팀에 알려줍니다.

1. (동일한 브라우저 애플리케이션에서 동일한 광고 네트워크의 다른 계정에 로그인한 경우) 광고주의 계정이 아닌 다른 계정에서 로그아웃합니다.

1. 메인 메뉴에서 **[!UICONTROL Search]** \> **[!UICONTROL Campaigns]** \> **[!UICONTROL Campaigns]**. 하위 메뉴에서 **[!UICONTROL Live]** \> **[!UICONTROL Accounts]**.

1. 계정 이름 위에 커서를 놓고 ![자세히](/help/search-social-commerce/assets/more-filters.png "자세히")을 선택한 다음 을 선택합니다 **[!UICONTROL Edit]**.

1. 새 액세스 토큰 가져오기:

   1. 클릭 **[!UICONTROL Get oAuth Token]**.

   1. (광고주의 계정에 로그인하지 않은 경우) 광고주의 광고 계정에 로그인합니다. 가장 좋은 방법은 계정에 대한 API 액세스에 자격 증명을 사용하는 것입니다.

   1. 권한/액세스 요청 화면에서 버튼을 클릭하여 권한을 확인합니다.

   1. 열려 있는 팝업 창에서 인증 문자열을 복사하고 문자열을 **[!UICONTROL oAuth Token]** 필드.

1. 클릭 **[!UICONTROL Post]**.

## 광고 네트워크 계정 활성화 또는 비활성화 {#enable-disable-account}

*에이전시 계정 관리자, Adobe 계정 관리자 및 관리자 사용자 역할만 해당*

광고 네트워크 계정을 활성화하면 Search, Social 및 Commerce가 캠페인 데이터를 계정과 동기화하고(지원되는 경우) 포트폴리오의 캠페인에 대한 자동화된 입찰 및/또는 캠페인 예산을 푸시합니다.광고 네트워크 계정을 비활성화하면 Search, Social 및 Commerce가 계정에서 모든 활동을 중지합니다. 계정이 활성화된 동안 수집된 데이터는 여전히 저장되지만 캠페인 관리 보기 및 보고서에는 계정이 비활성화된 기간에 대한 데이터가 포함되지 않습니다. 나중에 계정을 다시 활성화하여 계정으로 활동을 재개할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Search]** \> **[!UICONTROL Campaigns]** \> **[!UICONTROL Campaigns]**. 하위 메뉴에서 **[!UICONTROL Live]** \> **[!UICONTROL Accounts]**.

1. 다음 중 하나를 수행합니다.

   * (단일 계정의 상태를 변경하려면) 계정 이름 위에 커서를 놓고 ![자세히](/help/search-social-commerce/assets/more-filters.png "자세히")을 선택한 다음 을 선택합니다 **[!UICONTROL Edit]**. 변경 **[!UICONTROL Status]** 끝 *활성화됨* 또는 *비활성화됨*&#x200B;을 클릭한 다음 을 클릭합니다 **[!UICONTROL Post]**.

   * (하나 이상의 계정에 대한 상태를 변경하려면) 다음을 수행합니다.

      1. 각 계정 옆의 확인란을 선택합니다.

         여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md).&quot;

      1. 데이터 테이블 위의 도구 모음에서 ![활성화 아이콘](/help/search-social-commerce/assets/activate.png "활성화 아이콘") 계정을 활성화하려면 또는 ![비활성화 아이콘](/help/search-social-commerce/assets/disable.png "비활성화 아이콘") 계정을 비활성화합니다.

## 광고 네트워크 계정 설정 {#account-settings}

>[!NOTE]
>
>에이전시 계정 관리자만 [!DNL Adobe] 계정 관리자 및 관리자 사용자는 계정 설정을 구성할 수 있습니다.

### 계정 세부 정보

**[!UICONTROL SE Account ID]:** (를 제외한 모든 계정 [!DNL Naver] 및 [!DNL Yandex] 계정, 새 계정에만 편집 가능) 광고 네트워크에서 할당한 계정 ID입니다.

>[!NOTE]
>
>광고 네트워크 관리자 계정은 여기에서 지원되지 않습니다. 다음에 대한 관리자 계정을 식별하려면 [!DNL Microsoft Advertising] 또는 [!DNL Yandex], 각각 기본 계정 ID 또는 MCC 계정 필드를 사용합니다. 종료 [에 대한 자격 증명 설정 [!DNL Google Ads] 관리자 계정](/help/search-social-commerce/admin/manager-accounts.md)로 이동합니다. [!UICONTROL Admin] \> [!UICONTROL Manager Accounts].

**[!UICONTROL Account Name]:** 검색, 소셜 및 상거래 내에서 계정에 대해 표시할 이름입니다.

>[!NOTE]
>
>Search, Social 및 Commerce-Adobe Analytics 통합이 있고 검색 계정의 이름을 변경한 경우, Adobe 계정 팀에 알려 매핑을 업데이트할 수 있도록 하십시오.

**[!UICONTROL Login Details]: \[로그인 유형\]** - ([!DNL Microsoft Advertising]/[!DNL Microsoft Merchant Center] 만 해당) 다음을 사용하여 계정에 대한 로그인 승인 여부:

* *[!UICONTROL oAuth]* (기본값): [[!DNL OAuth] 인증 프로토콜](http://tools.ietf.org/html/draft-ietf-oauth-v2-22).

* *[!UICONTROL Password]:* 클라이언트의 암호를 사용합니다.

대상 [!DNL Microsoft Advertising] 계정, 만 [!DNL oAuth]-authorized logins 를 사용할 수 있습니다.

**[!UICONTROL Login Details]: [!UICONTROL Login]:** (를 제외한 모든 광고 네트워크 [!DNL Naver]) 계정에 대한 API 액세스를 활성화하는 로그인 이름 또는 ID입니다.

**[!UICONTROL Login Details]: [!UICONTROL OAuth Token]:** ([!DNL Microsoft Advertising] [!DNL oAuth]사용 및 을 제외한 다른 모든 네트워크 [!DNL Baidu], [!DNL Meta], 및 [!DNL Yandex]) 를 사용하여 로그인을 승인하는 계정의 토큰 [[!DNL OAuth] 인증 프로토콜](http://tools.ietf.org/html/draft-ietf-oauth-v2-22).

**[!UICONTROL Login Details]: [!UICONTROL Password]:** (를 제외한 모든 광고 네트워크 [!DNL Naver]) 계정의 암호입니다. 의 암호 사용 계정 [!DNL Baidu], [!DNL Microsoft Advertising], [!DNL Yahoo! Japan Ads], 및 [!DNL Yandex], 이 필드는 필수입니다. 대상 [!DNL oAuth]-enabled accounts, 이 필드는 선택 사항입니다. 계정 관리자가 필요에 따라 토큰을 새로 고칠 수 있도록 암호를 암호화하고 저장할 때 이 필드를 사용합니다.

**[!UICONTROL Login Details]: [!UICONTROL Access Key]:** ([!DNL Baidu] 및 [!DNL Yandex] 계정 전용) 사용할 개발자 계정에 대한 액세스 키입니다.

**[!UICONTROL Currency]:** 계정에 사용되는 통화의 약어입니다. 이 필드는 새 항목에서 편집할 수 있습니다. [!DNL Naver] 계정. 다른 모든 검색 네트워크의 경우, 레코드를 저장하면 광고 네트워크의 계정에 대해 구성된 통화로 값이 자동으로 채워집니다.

**[!UICONTROL Landing Page Suffix]** ([!DNL Google Ads] 및 [!DNL Microsoft Advertising] accounts only; 선택 사항) 정보를 추적하기 위해 최종 URL 끝에 추가하는 모든 매개 변수. 비즈니스에서 추적해야 하는 모든 매개 변수를 포함합니다.

예: `param1=value1&param2=value2`

Adobe 광고 클릭 추적을 사용하는 계정에는 광고 네트워크의 클릭 식별자(`msclkid` 대상 [!DNL Microsoft Advertising]; `gclid` (Google의 경우) 접미사. Adobe Analytics 통합이 있는 계정은 `s_kwcid` 매개 변수. 계정에 서버측 s\_kwcid 구현이 있는 경우 사용자가 광고를 클릭하면 매개 변수가 자동으로 추가됩니다. 그렇지 않으면 여기에 매개 변수를 수동으로 추가해야 합니다. 다음을 참조하십시오. [필수 접미어 형식 [!DNL Google Ads]](/help/search-social-commerce/tracking/formats-click-tracking-google.md) 및 [필수 접미어 형식 [!DNL Microsoft Advertising]](/help/search-social-commerce/tracking/formats-click-tracking-microsoft.md).

>[!NOTE]
>
>* 이 필드는 다음에 의해 업데이트되지 않습니다. [!UICONTROL Auto Upload] 추적 설정입니다.
>* 하위 수준의 최종 URL 접미사는 계정 수준 접미사를 덮어씁니다. 간편하게 유지 관리할 수 있도록 개별 계정 구성 요소에 대해 다른 추적이 필요하지 않은 경우 계정 수준 접미사만 사용하십시오. 광고 그룹 수준 또는 하위 수준에서 접미사를 구성하려면 광고 네트워크의 편집기를 사용합니다.


**시간대:** (를 제외한 모든 광고 네트워크 [!DNL Baidu] 및 [!DNL Yahoo! Display Network]) 광고주의 시간대. 이 필드는 편집할 수 있으며 새 필드에는 선택 사항입니다 [!DNL Naver] 계정. 다른 모든 검색 네트워크의 경우, 레코드를 저장하면 광고주의 검색, 소셜, 상거래 계정에 대해 구성된 시간대로 값이 자동으로 채워집니다.

**상태:** 검색, 소셜 및 상거래 내 계정 상태:

* *활성화됨:* Search, Social 및 Commerce는 캠페인 데이터를 계정과 동기화하고(지원되는 경우) 포트폴리오의 캠페인에 대한 자동화된 입찰 및/또는 캠페인 예산을 푸시합니다.
* *비활성화됨:* Search, Social 및 Commerce는 계정에서 모든 활동을 중지합니다. 계정이 활성화된 동안 수집된 데이터는 여전히 저장되지만 캠페인 관리 보기 및 보고서에는 계정이 일시 중지된 기간 동안의 데이터가 포함되지 않습니다. 나중에 계정을 다시 활성화하여 계정으로 활동을 재개할 수 있습니다.

**추적 템플릿** - ([!DNL Google Ads], [!DNL Microsoft Advertising], 및 [!DNL Yahoo! Japan Ads] 계정만 해당; 선택 사항) 계정의 기본 추적 템플릿으로, 모든 오프랜딩 도메인 리디렉션 및 추적 매개 변수를 지정하고 또한 매개 변수에 최종/랜딩 페이지 URL을 포함합니다. 예: `{lpurl}?source={network}&id=5` 또는 `http://www.trackingservice.example.com/?url={lpurl}?source={network}&id=5` 리디렉션을 포함합니다.

* 최종 URL을 포함하려면 다음을 수행하십시오.

   * ([!DNL Google Ads] 및 [!DNL Microsoft Advertising] 만 해당) 추적 템플릿의 최종 URL을 나타내는 매개 변수 목록에 대해서는 ([!DNL Microsoft Advertising] 만) [[!DNL Microsoft Advertising] 설명서](https://help.ads.microsoft.com/#apex/3/en/56799) 또는 ([!DNL Google Ads] 만 해당) 의 &quot;사용 가능한 ValueTrack 매개 변수&quot;에 대한 섹션에서 &quot;추적 템플릿만&quot; 매개 변수 [[!DNL Google Ads] 설명서](https://support.google.com/google-ads/answer/6305348).

   * ([!DNL Yahoo! Japan Ads] 만 해당) 매개 변수 사용 `!{lpurl}` 랜딩 페이지 URL을 나타냅니다.

* 필요에 따라 URL 매개 변수와 캠페인에 대해 정의된 사용자 지정 매개 변수를 앰퍼샌드(&amp;)로 구분하여 포함할 수 있습니다. `{lpurl}?matchtype={matchtype}&device={device}`.

* 원할 경우 서드파티 리디렉션 및 추적을 추가할 수 있습니다.

* 캠페인 설정에 &quot;&quot;가 포함된 경우[!UICONTROL EF Redirect]&quot; 및 &quot;[!UICONTROL Auto Upload],&quot; Search, Social 및 Commerce는 레코드를 저장할 때 자체 리디렉션 및 추적 코드 접두사를 자동으로 추가합니다.

>[!NOTE]
>
>* 대상 [!DNL Google Ads]병렬 추적을 활성화하는 소스의 클릭에 대체되지 않는 매크로를 사용하지 마십시오. 광고주가 매크로를 사용해야 하는 경우 Adobe 계정 팀은 고객 지원 팀 또는 구현 팀과 협력하여 매크로를 추가해야 합니다.
>* 가장 세분화된 수준의 추적 템플릿은 모든 상위 수준의 값을 재정의합니다. 예를 들어 계정 설정과 키워드 설정 모두에 값이 포함된 경우 키워드 값이 적용됩니다.
>* 광고, 사이트링크 또는 키워드 수준에서 추적 템플릿을 업데이트하는 경우 관련 광고가 다시 제출되어 검토됩니다. 승인을 위해 광고를 다시 제출하지 않고도 계정, 캠페인 또는 광고 그룹 수준에서 추적 템플릿을 업데이트할 수 있습니다.


**[!UICONTROL Master Account ID]:** ([!DNL Microsoft Advertising] 계정 전용) 계정과 연결된 기관/관리 계정의 ID입니다.

**[!UICONTROL MCC Account]:** ([!DNL Yandex] 계정만 해당(선택 사항) 계정과 연결된 기관/관리 계정. 기존 연결을 제거하려면 &quot;[!UICONTROL No MCC Account].&quot;

**[!UICONTROL Application ID]:** ([!DNL Yandex] 계정 전용) 계정에 사용할 개발자 토큰입니다. 모든 항목에 동일한 토큰이 사용됨 [!DNL Yandex] 계정.

**[!UICONTROL Purse Campaign ID]:** ([!DNL Yandex] 공유 계정 설정이 비활성화된 계정만 해당, 선택 사항) 계정의 모든 광고 캠페인에 대한 비용을 지불하는 데 사용될 캠페인에 대한 숫자 ID입니다.

**[!UICONTROL Finance Token]:** ([!DNL Yandex] 공유 계정 설정이 비활성화된 계정만 해당(선택 사항) 포트폴리오 최적화에 필요할 때 광고주의 캠페인 간에 지갑에서 돈을 다시 할당하는 것과 같이, 금융 관련 API 호출에 사용할 개발자 토큰입니다.

### 계정 추적

<!-- **[!UICONTROL Tracking Type]:** -->

{{$include /help/_includes/tracking-type.md}}

<!-- **[!UICONTROL Redirect Type]:** -->

{{$include /help/_includes/redirect-type.md}}

<!-- **[!UICONTROL Auto Upload]:** -->

{{$include /help/_includes/auto-upload.md}}

<!-- **[!UICONTROL Encode Base URL]:** -->

{{$include /help/_includes/encode-base-url.md}}

<!-- **[!UICONTROL Tracking Level]:** -->

{{$include /help/_includes/tracking-level.md}}

**[!UICONTROL Track Product Group]:** (대상 [!UICONTROL EF Redirect] 만) 구현되지 않음

<!-- **[!UICONTROL Append Parameters]:** -->

{{$include /help/_includes/append-parameters.md}}

* **S\_kwcid 형식** - (기존 [!DNL Google Ads] Adobe Advertising-Adobe Analytics을 통합하고 s\_kwcid가 이미 마이그레이션되지 않은 광고주를 위한 계정)

이 계정은 s\_kwcid 추적 코드에 대한 레거시 형식을 사용하며, 이를 통해 Adobe 광고에서 Adobe Analytics과 계정에 대한 데이터를 공유할 수 있습니다. 다음 [최신 형식](/help/search-social-commerce/tracking/skwcid-tracking-parameter.md) 캠페인 및 광고 그룹 수준에서 정확하게 보고하는 데 필요한 캠페인 ID 및 광고 그룹 ID에 대한 매개 변수를 포함합니다. [!DNL Google Ads] analytics의 성과 최대 캠페인, 초안 및 실험 캠페인:

`s_kwcid=AL!{userid}!3!{creative}!{matchtype}!{placement}!{network}!{product_partition_id}!{keyword}!{campaignid}!{adgroupid}`

이 계정이 캠페인 및 광고 그룹 수준에서 보고해야 하는 경우 [!UICONTROL Edit] (연필) 아이콘 및 **[!UICONTROL Migrate to new s\_kwcid format]** 을 클릭하여 새 형식으로 변경합니다. 이러한 캠페인 유형을 포함하지 않는 계정의 경우, 새로운 포맷으로의 마이그레이션은 선택 사항이지만 권장됩니다.

전체 지침은 &quot;[에 대한 s\_kwcid 추적 코드 업데이트 [!DNL Google Ads] account](/help/search-social-commerce/campaign-management/accounts/update-skwcid-google.md).&quot;

**보고서 세트 이름** - (토큰 전용 EF 리디렉션, Adobe Advertising-Adobe Analytics 통합을 사용하는 광고주, 선택 사항) 엔티티 분류 및 계정에 대한 클릭 데이터를 포함하여 검색, 소셜 및 상거래가 광고 네트워크에서 수집하는 데이터를 전송하는 하나 이상의 Analytics 보고서 세트입니다. 이 기능은 지원되는 광고 네트워크에서만 사용할 수 있습니다.

데이터를 보고서 세트에 표시하려면 (a) 계정용으로 서버측 s\_kwcid를 구성해야 하거나 (b) 광고주 수준 설정을 &quot;[!UICONTROL Enable tracking for SAINT feeds]&quot;을(를) 활성화해야 합니다. 또한 광고주의 Analytics 계정이 검색, 소셜 및 상거래에서 데이터를 수신하도록 구성되어 있어야 합니다. 자세한 내용은 Adobe 계정 관리자에게 문의하십시오.

>[!MORELIKETHIS]
>
>* [광고 네트워크 계정 기본 정보](ad-network-account-about.md)
>* [머천트 센터 계정 관리](merchant-account-manage.md)
>* [에 대한 s\_kwcid 추적 코드 업데이트 [!DNL Google Ads] account](update-skwcid-google.md)

