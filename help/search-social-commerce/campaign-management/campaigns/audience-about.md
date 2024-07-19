---
title: 대상자 기본 정보
description: ' [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 대상자를 추적, 만들기 및 관리하는 옵션에 대해 알아봅니다.'
exl-id: f85cbc82-ddbc-4ecd-a17b-b4cb4808cfbc
feature: Search Campaign Management
source-git-commit: 67fe8581832dc0762d62908d01672e53cc95b847
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---

# 검색, 소셜 및 Commerce에서 [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 대상자 관리 정보

*[!DNL Google Ads]및 [!DNL Microsoft Advertising]만*

대상 라이브러리에는 모든 [!DNL Google Ads] 고객 데이터 기반, 마켓 내 및 유사한 대상과 [!DNL Microsoft Advertising] 리마케팅 및 동적 리마케팅, 사용자 지정, 고객 일치, 마켓 내 및 유사한 대상이 나열됩니다. [!DNL Google Ads]개의 대상 중 하나를 [!DNL Google Ads] 캠페인 수준 및 광고 그룹 수준 대상 및 제외로 사용할 수 있으며, [!DNL Microsoft Advertising]개의 대상 중 하나를 [!DNL Microsoft Advertising] 캠페인 수준 및 광고 그룹 수준 대상 및 (동적 리마케팅 대상만) 제외로 사용할 수 있습니다. 대상 타겟에 대한 입찰 조정을 추가하거나 편집할 수 있습니다.

기존 Adobe Experience Cloud 대상자 및 CRM(고객 관계 관리) 시스템의 다양한 종류의 고객 데이터에서 세그먼트나 이메일 목록을 사용하여 대상자를 만들고 관리할 수도 있습니다.

* **Adobe 대상 세그먼트:** 옵트인 Adobe Audience Manager 또는 Adobe Analytics 계정이 있는 광고주는 [!DNL Adobe] 세그먼트에서 대상을 일치시키는 [!DNL Google Ads]개의 고객 일치 대상을 만들 수 있습니다.

   * (Audience Manager이 없는 [!DNL Analytics] 계정의 광고주) Adobe Experience Cloud과 공유된 [!DNL Analytics] 세그먼트의 사용자 ID를 사용하여 [!DNL Google Ads] 고객 일치 대상을 만들 수 있습니다.

   * (Audience Manager 계정이 있는 광고주) 검색, 소셜 및 Commerce을 대상으로 하는 Audience Manager 세그먼트의 사용자 ID를 사용하여 [!DNL Google Ads]개의 고객 일치 대상을 만들 수 있습니다. 여기에는 Adobe Experience Cloud에 게시된 Adobe Analytics 세그먼트와 Adobe Experience Cloud 대상 라이브러리를 사용하여 만든 세그먼트가 포함될 수 있습니다.

  고객 일치 대상을 만들려면 광고주의 [!DNL Google Ads] 계정이 [사용자 지정 일치에 적합](https://support.google.com/adspolicy/answer/6299717)되고 [사용자 ID 세그먼트](https://support.google.com/google-ads/answer/9199250)를 옵트인해야 합니다. 또한 고객 일치 대상을 만들 수 있도록 검색, 소셜 및 Commerce의 광고주 계정을 구성해야 합니다.

  고객 데이터 기반 대상의 [!DNL Adobe] 세그먼트 데이터 및 쿠키 동기화 파일이 매일 [!DNL Google Ads]에 동기화됩니다.

* **Adobe Campaign 전자 메일 목록:** Adobe 계정 팀에서 [!DNL Campaign] 내의 전자 메일 목록에서 [!DNL Google Ads] 고객 일치 대상을 만들고 업데이트하는 워크플로를 설정하는 데 도움을 줄 수 있습니다.

* **고객 데이터 목록:** 고객 일치 타겟팅에 적합한 [!DNL Google Ads] 또는 [!DNL Microsoft Advertising] 계정이 있는 광고주는 광고 네트워크별 고객 데이터 기반 대상 &lt;!을(를) 만들고 업데이트할 수 있습니다.— 또는 동적 리마케팅 대상 — 기본 식별자가 포함된 CSV 파일을 업로드하여 고객 데이터 기반 대상에 포함됩니까?—> 한 개 이상 포함됩니다.[!DNL Google Ads]

* **동적 리마케팅 목록:** [!DNL Microsoft Advertising] 계정이 있는 광고주는 동적 리마케팅 대상을 만들고 관리할 수 있습니다. 이 대상을 사용하여 여러 가지 방법(예: 제품 뷰어 또는 이전 구매자) 중 하나로 최근에 제품과 상호 작용한 잠재 고객을 리타겟팅할 수 있습니다. 동적 리마케팅 대상자를 사용하려면 웹 페이지에서 광고 네트워크의 JavaScript 전환 및 대상자 추적 태그를 사용해야 합니다. 검색 및 대상 네트워크의 쇼핑 캠페인과 함께 동적 리마케팅 목록을 사용하여 제품 광고로 대상을 재타겟팅하고 검색 캠페인과 함께 텍스트 광고 및 동적 검색 광고로 대상을 재타겟팅합니다. <!--[For [!DNL Google Ads], these are technically included in a customer data-based audience, so word this all carefully when we add support for them.]-->

  >[!NOTE]
  >
  >동적 리마케팅 대상자 타겟에 대한 입찰 수정자가 &quot;[!UICONTROL Auto-optimize Bid Adjustment Values]&quot; 설정이 있는 포트폴리오에서 최적화되지 않았습니다.

>[!NOTE]
>
>Search, Social 및 Commerce은 업로드한 고객 데이터나 [!DNL Google Ads] 또는 [!DNL Microsoft Advertising] 대상자를 만들거나 편집하는 데 사용한 [!DNL Adobe] 세그먼트의 고객 데이터를 저장하지 않습니다.

>[!MORELIKETHIS]
>
>* [고객 일치 대상자 만들기 [!DNL Google Ads] 출처 [!DNL Adobe] 대상자](google-audience-from-adobe-audience.md)
>* [Adobe Campaign 전자 메일 목록에서 고객 일치 대상 만들기 [!DNL Google Ads] 2}](google-audience-from-campaign-email-list.md)
>* [고객 데이터 목록을 사용하여 고객 일치 대상 관리](audience-from-customer-data-list.md)
>* [동적 리마케팅 대상자 관리](audience-dynamic-remarketing-manage.md)
>* [캠페인 및 광고 그룹에 대한 대상자 대상 관리](audience-targets-manage.md)
>* [캠페인 및 광고 그룹에 대한 대상자 제외 관리](audience-exclusions-manage.md)
