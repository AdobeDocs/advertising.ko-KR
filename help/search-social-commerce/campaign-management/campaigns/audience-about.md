---
title: 대상자 기본 정보
description: 추적, 생성 및 관리 옵션에 대해 알아보기 [!DNL Google Ads] 및 [!DNL Microsoft® Advertising] 대상.
exl-id: 34169650-9820-4b7d-9ae6-09ff8a8c6f2e
feature: Search Campaign Management
source-git-commit: 9f30518efbbe29f976298fe1fcd962182285679f
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---

# 관리 기본 정보 [!DNL Google Ads] 및 [!DNL Microsoft® Advertising] 검색, 소셜 및 상거래의 대상

*[!DNL Google Ads]및 [!DNL Microsoft® Advertising] 전용*

대상 라이브러리에는 [!DNL Google Ads] 고객 데이터 기반, 시장 내 및 유사한 대상과 [!DNL Microsoft® Advertising] 리마케팅 및 다이내믹 리마케팅, 사용자 지정, 고객 일치, 마켓 내 및 유사한 대상. 다음 중 하나를 사용할 수 있습니다. [!DNL Google Ads] 대상: [!DNL Google Ads] 캠페인 수준 및 광고 그룹 수준의 타겟 및 제외를 사용하며 [!DNL Microsoft® Advertising] 대상: [!DNL Microsoft® Advertising] 캠페인 수준 및 광고 그룹 수준의 타겟 및 (동적 리마케팅 대상만 해당) 제외. 대상 타겟에 대한 입찰 조정을 추가하거나 편집할 수 있습니다.

기존 Adobe Experience Cloud 대상자 및 CRM(고객 관계 관리) 시스템의 다양한 종류의 고객 데이터에서 세그먼트나 이메일 목록을 사용하여 대상자를 만들고 관리할 수도 있습니다.

* **Adobe 대상 세그먼트:** 옵트인 Adobe Audience Manager 또는 Adobe Analytics 계정이 있는 광고주는 [!DNL Google Ads] 의 고객 일치 대상 [!DNL Adobe] 세그먼트:

   * (광고주: [!DNL Analytics] Audience Manager이 없는 계정) 만들 수 있습니다 [!DNL Google Ads] 의 사용자 ID를 사용하는 고객 일치 [!DNL Analytics] Adobe Experience Cloud과 공유되는 세그먼트입니다.

   * (Audience Manager 계정이 있는 광고주) 다음을 만들 수 있습니다 [!DNL Google Ads] 고객이 검색, 소셜 및 상거래를 대상으로 하는 Audience Manager 세그먼트의 사용자 ID를 사용하여 대상을 일치시킵니다. 여기에는 Adobe Experience Cloud에 게시된 Adobe Analytics 세그먼트와 Adobe Experience Cloud 대상 라이브러리를 사용하여 만든 세그먼트가 포함될 수 있습니다.

  고객 일치 대상을 만들려면 광고주의 [!DNL Google Ads] 계정은 다음과 같아야 합니다. [사용자 정의 일치 가능](https://support.google.com/adspolicy/answer/6299717) 을(를) 위해 옵트인함 [사용자 ID 세그먼트](https://support.google.com/google-ads/answer/9199250). 또한 고객 일치 대상을 만들 수 있도록 검색, 소셜 및 상거래의 광고주 계정을 구성해야 합니다.

  [!DNL Adobe] 고객 데이터 기반 대상을 위한 세그먼트 데이터 및 쿠키 동기화 파일이에 동기화됨 [!DNL Google Ads] 매일.

* **Adobe Campaign 이메일 목록:** Adobe 계정 팀은 다음을 만들고 업데이트하는 워크플로를 설정하는 데 도움을 줄 수 있습니다. [!DNL Google Ads] 다음 내의 이메일 목록에서 대상자를 일치시키십시오. [!DNL Campaign].

* **고객 데이터 목록:** 를 사용하는 광고주 [!DNL Google Ads] 또는 [!DNL Microsoft® Advertising] 고객 일치 타겟팅에 적합한 계정은 광고 네트워크별 고객 데이터 기반 대상자를 만들고 업데이트할 수 있습니다 &lt;!>— 또는 동적 리마케팅 대상 — 최소한 고객 데이터 기반 대상에 포함됩니다. [!DNL Google Ads]기본 식별자가 있는 CSV 파일을 업로드하여 ?—>.

* **동적 리마케팅 목록:** 를 사용하는 광고주 [!DNL Microsoft® Advertising] 계정은 동적 리마케팅 대상자를 만들고 관리할 수 있으며, 이 대상자를 사용하여 여러 가지 방법(예: 제품 뷰어 또는 이전 구매자) 중 하나로 최근 제품과 상호 작용한 잠재 고객을 리타겟팅할 수 있습니다. 동적 리마케팅 대상자를 사용하려면 웹 페이지에서 광고 네트워크의 JavaScript 전환 및 대상자 추적 태그를 사용해야 합니다. 검색 및 대상 네트워크의 쇼핑 캠페인과 함께 동적 리마케팅 목록을 사용하여 제품 광고로 대상을 재타겟팅하고 검색 캠페인과 함께 텍스트 광고 및 동적 검색 광고로 대상을 재타겟팅합니다. <!--[For [!DNL Google Ads], these are technically included in a customer data-based audience, so word this all carefully when we add support for them.]-->

  >[!NOTE]
  >
  >동적 리마케팅 대상자 타겟에 대한 입찰 수정자는 &quot;[!UICONTROL Auto-optimize Bid Adjustment Values]&quot; 설정.

>[!NOTE]
>
>Search, Social 및 Commerce는 업로드한 고객 데이터나 [!DNL Adobe] 세그먼트를 만들거나 편집하는 데 사용 [!DNL Google Ads] 또는 [!DNL Microsoft® Advertising] 대상입니다.

>[!MORELIKETHIS]
>
>* [만들기 [!DNL Google Ads] 의 고객 일치 대상 [!DNL Adobe] 대상](google-audience-from-adobe-audience.md)
>* [만들기 [!DNL Google Ads] Adobe Campaign 이메일 목록의 고객 일치 대상](google-audience-from-campaign-email-list.md)
>* [고객 데이터 목록을 사용하여 고객 일치 대상 관리](audience-from-customer-data-list.md)
>* [동적 리마케팅 대상자 관리](audience-dynamic-remarketing-manage.md)
>* [캠페인 및 광고 그룹에 대한 대상자 타겟 관리](audience-targets-manage.md)
>* [캠페인 및 광고 그룹에 대한 대상자 제외 관리](audience-exclusions-manage.md)
