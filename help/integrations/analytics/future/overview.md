---
title: Adobe Analytics와의 Adobe 광고 통합
description: Adobe 광고가 Adobe Analytics과 데이터를 교환하는 방법과 검색, 소셜 및 상거래 내에서 데이터를 사용하는 방법에 대해 알아봅니다.
feature: Integration with Adobe Analytics
exl-id: 5b0ecb82-fb5c-48c5-a599-15b548f59461
source-git-commit: def6a3a8d1de1f9f80dee6ecd1a18667afc79fd3
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 0%

---

# Adobe Analytics와의 Adobe 광고 통합

다음과 같은 방법으로 Adobe 광고를 Analytics와 통합할 수 있습니다.

## 간 데이터 교환 [!AAnalytics] 및 Adobe 광고

### 가져오기 [!AAnalytics] Adobe 광고에 데이터 삽입

사용 [[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md),[!DNL Search, Social, & Commerce] 및 DSP 가져오기:

* **[!DNL Analytics]세그먼트:**  에서 만들어진 모든 광고주 또는 에이전시의 세그먼트에 대한 메타데이터, 계층 데이터 및 고유한 대상 데이터 [!DNL Analytics] Experience Cloud에 게시되었습니다.

* **[!DNL Analytics]사이트 참여 지표**

* **[!DNL Analytics]표준, 사용자 지정 및 예약된 지표**

### Adobe 광고 데이터를에 보냅니다. [!AAnalytics]

* **Adobe 광고의 트래픽 지표**

* **Adobe 광고의 Dimension**

>[!NOTE]
>
>대상 [!DNL Search, Social, & Commerce], 이 기능은 대부분의 광고 네트워크 및 캠페인 유형에 대해 지원됩니다. 에서 &quot;지원되는 인벤토리&quot;를 참조하십시오. [!DNL Search, Social, & Commerce] 자세한 내용은 안내서 를 참조하십시오.<!-- add link when that's published in ExL -->

### 사용 [!DNL Analytics] 만들 세그먼트 [!DNL Google Ads Audiences] {#audience-manager-google-audiences}

*옵트인 광고주 [!DNL Advertising Search, Social, & Commerce] 전용*

<!-- Verify all -->

내 [!DNL Search, Social, & Commerce], 만들 수 있습니다. [!DNL Google Ads] Google 고객 일치 타겟팅 기존 [!DNL Analytics] 세그먼트 를 참조하십시오. 여기에는 Adobe Experience Cloud에 게시된 Adobe Analytics 세그먼트와 Adobe Experience Cloud을 사용하여 생성된 세그먼트가 포함됩니다 [!DNL Audience Library]. 자세한 내용은 [!DNL Search, Social, & Commerce].

[사용자 ID의 고객 일치 대상](https://support.google.com/google-ads/answer/9199250) 웹 사이트 태그 기반 대상처럼 작동하지만, 비PII ID는 표준 고객 일치 및 웹 사이트 태그 기반 대상자보다 고유한 이점을 위해 고유 대상 구성원에게 할당됩니다.

필요한 사용자 ID를 만들려면 Adobe 광고 JavaScript 태그를 사용해야 합니다 <!-- with a user ID parameter -->클릭합니다. 자세한 내용은 Adobe 계정 팀에 문의하십시오.

![세그먼트 생성 프로세스](/help/integrations/assets/ad_search_user_id_pic.png)

대상자를 만들면 여기에서 대상자를 사용할 수 있습니다. [!DNL Google Ads] 캠페인 [캠페인 수준 또는 광고 그룹 수준 타겟 또는 제외](#audience-manager-targets).

### 사용 [!DNL Analytics] Target 또는 제외시킬 세그먼트 {#analytics-targets}

* (옵트인 광고주 및 [!DNL Search, Social, & Commerce]) 임의의 [!DNL Google Ads] 대상 [다음을 사용하여 생성 [!DNL Analytics] 세그먼트](#audience-manager-google-audiences) 캠페인 수준 또는 광고 그룹 수준 타겟 또는 제외 [!DNL Google Ads] 캠페인.

* (DSP을 사용하는 광고주) 기존 [!DNL Analytics] 세그먼트를 광고 배치 대상으로 사용할 수 있습니다. 선택적으로 재사용 가능한 대상에 세그먼트를 포함할 수 있습니다. 이 세그먼트를 여러 배치에 대한 타겟 또는 제외로 사용할 수 있습니다.

* (Advertising Creative를 사용하는 광고주) 기존 [!DNL Analytics] 세그먼트를 광고 경험에서 특정 크리에이티브를 위한 타겟으로 사용할 수 있습니다.
