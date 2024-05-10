---
title: 판매자 계정 관리
description: 머천트 센터 계정에 대한 계정 세부 정보를 설정하고 관리하는 방법에 대해 알아봅니다.
exl-id: 7d940e45-ea49-470b-98d0-0196593228cb
feature: Search Campaign Management
source-git-commit: e517dd5f5fa283ff8a2f57728612937148889732
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 0%

---

# 판매자 계정 관리

*에이전시 계정 관리자, Adobe 계정 관리자 및 관리자 사용자 역할만 해당*

Search, Social 및 Commerce은 광고주의 Google 판매자 센터 또는 Microsoft 판매자 센터 계정에 대해 매일 제품 데이터를 다운로드하고 표시할 수 있습니다. 또한 Search, Social 및 Commerce은 판매자 계정의 컨텐츠를 기반으로 광고 생성을 자동화할 수 있습니다.Search, Social 및 Commerce에서 제품 데이터를 직접 사용하려면 계정 액세스 자격 증명과 액세스 권한을 포함하는 해당 계정 레코드를 생성해야 합니다 *활성화됨*.

>[!NOTE]
>
>판매자 계정 레코드를 제거할 수 없습니다. 계정 유형을 다음으로 변경하여 계정에 대한 액세스를 비활성화할 수 있습니다. *비활성화됨*.

## 판매자 계정 세부 정보 만들기 {#create-merchant-account}

*에이전시 계정 관리자, Adobe 계정 관리자 및 관리자 사용자 역할만 해당*

제품 데이터를 보고 판매자 계정에 대한 추적 템플릿을 생성하고 이 데이터를 기반으로 광고를 만들려면 계정 액세스 자격 증명과 계정에 대한 액세스 권한이 포함된 해당 계정 레코드를 만들어야 합니다 *활성화됨*.

>[!NOTE]
>
>판매자 네트워크에 실제 계정을 만들려면 해당 네트워크의 웹 사이트로 이동합니다.

1. 메인 메뉴에서 **[!UICONTROL Search]** \> **[!UICONTROL Campaigns]** \> **[!UICONTROL Products]**: 다음에 열립니다. [!UICONTROL Accounts] 탭.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL Create Account]**.

1. 다음을 지정합니다. [판매자 계정 설정](#merchant-account-settings):

   1. 다음에서 [!UICONTROL Product Source] 메뉴에서 판매자 센터를 선택합니다.

   <!--

   1. ([!DNL Meta Ads] accounts only) Log in to the [!DNL Meta Ads] account.

   And are there additional steps just for Meta? If so, create a separate procedure for it.
   
   -->

   1. (필수 사항: [!DNL Google Ads] 계정, 선택 사항 [!DNL Microsoft Advertising] 계정) 검색, 소셜 및 Commerce에서 [[!DNL OAuth] 인증 프로토콜](https://oauth.net/2/):

      1. ([!DNL Microsoft Advertising] 계정 전용) 선택 **[!UICONTROL oAuth]**.

      1. 클릭 **[!UICONTROL Enable Connection]**.

      1. (광고주 계정에 로그인하지 않은 경우) 광고주 계정에 로그인합니다. 가장 좋은 방법은 판매자 센터 계정에 대한 콘텐츠 API 액세스에 자격 증명을 사용하는 것입니다.

      1. 액세스/권한 요청 화면에서 버튼을 클릭하여 권한을 확인합니다.

      1. 열려 있는 팝업 창에서 인증 문자열을 복사하고 문자열을 **[!UICONTROL oAuth Token]** 필드.

      1. 다른 계정 설정을 지정합니다.

1. 클릭 **[!UICONTROL Save]**.

   계정의 모든 제품에 대한 특성 데이터는 다음 일별 동기화 프로세스(사용자의 현지 시간대에서 약 06:00) 후 검색, 소셜 및 Commerce에서 사용할 수 있습니다. 그런 다음 제품 데이터를 사용하여 인벤토리 피드를 사용하여 광고 생성을 자동화할 수 있습니다.

## 판매자 계정 세부 정보 편집 {#edit-merchant-account}

*에이전시 계정 관리자, Adobe 계정 관리자 및 관리자 사용자 역할만 해당*

계정 자격 증명이 변경되거나 머천트 계정에 대한 데이터 검색 및 사용을 중단하려는 경우 계정 상세내역을 편집합니다.

>[!NOTE]
>
>판매자 네트워크에서 실제 계정을 편집하려면 해당 네트워크의 웹 사이트로 이동합니다.

1. 메인 메뉴에서 **[!UICONTROL Search]\> [!UICONTROL Campaigns] \>[!UICONTROL Products]**: 다음에 열립니다. [!UICONTROL Accounts] 탭.

1. 계정 이름 옆에 있는 ![설정 보기/편집](/help/search-social-commerce/assets/settings.png "설정 보기/편집").

1. 편집 [판매자 계정 설정](#merchant-account-settings).

1. 클릭 **[!UICONTROL Save]**.

>[!NOTE]
>
>Search, Social 및 Commerce은 새 계정 데이터를 판매자 네트워크의 데이터와 동기화해야 합니다. 이 작업은 사용자의 현지 시간대에서 매일 06:00에 한 번 자동으로 수행됩니다.

## 판매자 계정에 대한 액세스 비활성화 {#disable-merchant-account}

*에이전시 계정 관리자, Adobe 계정 관리자 및 관리자 사용자 역할만 해당*

판매자 계정을 비활성화하면 Search, Social 및 Commerce이 계정에 로그인하지 않으므로 업데이트된 제품 데이터를 검색하지 않습니다. 계정이 활성화된 동안 수집된 데이터는 여전히 저장되며, 제품 데이터를 사용하여 만든 기존 광고는 피드 템플릿 및 피드 데이터 설정에 따라 업데이트, 일시 중지 또는 삭제되지 않습니다.

1. 메인 메뉴에서 **[!UICONTROL Search]** \> **[!UICONTROL Campaigns]** \> **[!UICONTROL Products]** : 다음에 열립니다. [!UICONTROL Accounts] 탭.

1. 계정 이름 옆에 있는 ![설정 보기/편집](/help/search-social-commerce/assets/settings.png "설정 보기/편집").

1. 변경 [!UICONTROL EF Account Type] 끝 **[!UICONTROL Disabled]**.

1. 클릭 **[!UICONTROL Save]**.

## 판매자 계정 설정 {#merchant-account-settings}

>[!NOTE]
>
>에이전시 계정 관리자만 [!DNL Adobe] 계정 관리자 및 관리자 역할은 판매자 계정 설정을 구성할 수 있습니다.

**[!UICONTROL Product Source]:** 판매자 네트워크. 기존 계정의 값을 변경할 수 없습니다.

**[!UICONTROL OAuth Token]:** ([!DNL Google Merchant Center] 계정 전용) 를 사용하여 로그인을 승인하는 계정의 토큰 [[!DNL OAuth] 인증 프로토콜](https://oauth.net/2/).

**[!UICONTROL Auth Type]:** ([!DNL Microsoft Advertising]/[!DNL Microsoft Merchant Center] 만 해당) 다음을 사용하여 계정에 대한 로그인 승인 여부:

* *[!UICONTROL Client login]:* 클라이언트의 로그인을 사용합니다.

* *[!UICONTROL oAuth]* (기본값): [[!DNL OAuth] 인증 프로토콜](https://oauth.net/2/).

**[!UICONTROL Access Key]:** ([!DNL Microsoft Merchant Center] 만 해당) 개발자 계정이 사용할 액세스 키입니다.

**[!UICONTROL Account Name]:** 검색, 소셜 및 Commerce 내에서 계정에 대해 표시되는 이름입니다.

**[!UICONTROL Login]:** 로그인 이름 또는 계정 ID.

**[!UICONTROL Password]:** 계정 암호입니다.

**[!UICONTROL Confirm Password]:** 계정 암호입니다.

**[!UICONTROL EF Account Type]:** Search, Social 및 Commerce이 계정에 액세스하는지 여부:

* *[!UICONTROL Enabled]* (기본값): Search, Social 및 Commerce은 계정에 로그인하여 제품 데이터를 검색할 수 있습니다.

* *[!UICONTROL Disabled]:* Search, Social 및 Commerce은 계정에 로그인하지 않으므로 업데이트된 제품 데이터를 검색하지 않습니다. 계정이 활성화된 동안 수집된 데이터는 여전히 저장되며, 제품 데이터를 사용하여 만든 기존 광고는 피드 템플릿 및 피드 데이터 설정에 따라 업데이트, 일시 중지 또는 삭제되지 않습니다.

**[!UICONTROL Account ID]:** 판매자 계정 ID. 지정된 로그인 정보가 있는 계정이 하나만 있는 경우 이 값은 선택 사항입니다.

**[!UICONTROL Time Zone]:** 광고주의 시간대. 광고주의 검색, 소셜 및 Commerce 계정 정보(계정이 생성될 때 설정됨)에 대해 구성된 동일한 시간대를 사용합니다. 기존 계정의 값을 변경할 수 없습니다.

>[!MORELIKETHIS]
>
>* [광고 네트워크 계정 기본 정보](ad-network-account-about.md)
>* [광고 네트워크 계정 관리](ad-network-account-manage.md)
