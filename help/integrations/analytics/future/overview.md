---
title: Adobe Analytics과 Adobe Advertising 통합
description: Adobe Advertising에서 Adobe Analytics과 데이터를 교환하는 방법과 검색, 소셜 및 Commerce 내에서 데이터를 사용하는 방법에 대해 알아봅니다.
feature: Integration with Adobe Analytics
exl-id: 5b0ecb82-fb5c-48c5-a599-15b548f59461
source-git-commit: 94a5b5591aef0aa5ae5d3459d547f52d939d559c
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Adobe Analytics과 Adobe Advertising 통합

다음과 같은 방법으로 Adobe Advertising을 Analytics와 통합할 수 있습니다.

## [!DNL Analytics]과(와) Adobe Advertising 간 데이터 교환

### [!DNL Analytics] 데이터를 Adobe Advertising으로 가져오기

[[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md),[!DNL Search, Social, & Commerce] 및 DSP에서 가져오기:

* **[!DNL Analytics]세그먼트:** 메타데이터, 계층 데이터 및 [!DNL Analytics]에서 만들어 Experience Cloud에 게시한 모든 광고주 또는 에이전시의 세그먼트에 대한 고유 대상 데이터입니다.

* **[!DNL Analytics]사이트 참여 지표**

* **[!DNL Analytics]표준, 사용자 지정 및 예약된 지표**

### [!DNL Analytics]&#x200B;(으)로 Adobe Advertising 데이터 보내기

* **Adobe Advertising의 트래픽 지표**

* **Adobe Advertising의 차원**

>[!NOTE]
>
>[!DNL Search, Social, & Commerce]의 경우 이 기능은 대부분의 광고 네트워크 및 캠페인 유형에 대해 지원됩니다. 자세한 내용은 [!DNL Search, Social, & Commerce] 가이드의 &quot;지원되는 인벤토리&quot;를 참조하십시오.<!-- add link when that's published in ExL -->

### [!DNL Analytics]개의 세그먼트를 사용하여 [!DNL Google Ads]개의 대상 만들기 {#audience-manager-google-audiences}

*만 사용하는 [!DNL Advertising Search, Social, & Commerce]옵트인 광고주*

<!-- Verify all -->

[!DNL Search, Social, & Commerce] 내에서 기존 [!DNL Google Ads] 세그먼트를 사용하여 사용자 ID에서 [!DNL Analytics] Google 고객 일치 대상을 만들 수 있습니다. 여기에는 Adobe Experience Cloud에 게시된 Adobe Analytics 세그먼트와 Adobe Experience Cloud [!DNL Audience Library]을(를) 사용하여 만든 세그먼트가 포함됩니다. 자세한 내용은 &quot;[대상자 만들기 [!DNL Google Ads] 고객 일치 대상자 [!DNL Adobe] 대상자](/help/search-social-commerce/campaign-management/campaigns/google-audience-from-adobe-audience.md)&quot;를 참조하십시오.

[사용자 ID의 고객 일치 대상](https://support.google.com/google-ads/answer/9199250)은(는) 웹 사이트 태그 기반 대상과 비슷하게 작동하지만, 표준 고객 일치 및 웹 사이트 태그 기반 대상과 구별되는 이점을 얻기 위해 PII ID가 아닌 ID가 고유 대상자 구성원에게 할당됩니다.

필요한 사용자 ID를 만들려면 웹 사이트에서 Adobe Advertising JavaScript 태그 <!-- with a user ID parameter -->을(를) 사용해야 합니다. 자세한 내용은 Adobe 계정 팀에 문의하십시오.

![세그먼트 만들기 프로세스](/help/integrations/assets/ad_search_user_id_pic.png)

대상을 만들면 [!DNL Google Ads] 캠페인에서 [캠페인 수준 또는 광고 그룹 수준 타겟 또는 제외](#audience-manager-targets)(으)로 사용할 수 있습니다.

### [!DNL Analytics]개의 세그먼트를 사용하여 광고를 타깃팅하거나 제외합니다. {#analytics-targets}

* ([!DNL Search, Social, & Commerce]을(를) 사용하는 옵트인 광고주) [!DNL Google Ads] 캠페인에서 [세그먼트 [!DNL Analytics] 를 사용하여 ](#audience-manager-google-audiences)만든 [!DNL Google Ads] 대상을 캠페인 수준 또는 광고 그룹 수준 타겟 또는 제외로 사용할 수 있습니다.

* (DSP을 사용하는 광고주) 기존 [!DNL Analytics] 세그먼트를 광고 배치 대상으로 사용할 수 있습니다. 재사용 가능한 대상에 세그먼트를 선택적으로 포함할 수 있으며, 이 대상은 여러 배치에 대한 타겟 또는 제외로 사용할 수 있습니다.

* (Advertising Creative을 사용하는 광고주) 기존 [!DNL Analytics] 세그먼트를 광고 경험의 특정 크리에이티브를 위한 타겟으로 사용할 수 있습니다.
