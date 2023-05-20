---
title: Adobe Analytics과 Advertising 통합 Adobe
description: Adobe 광고가 Adobe Analytics과 데이터를 교환하는 방법과 검색, 소셜 및 상거래 내에서 데이터를 사용하는 방법에 대해 알아봅니다.
feature: Integration with Adobe Analytics
exl-id: 5b0ecb82-fb5c-48c5-a599-15b548f59461
source-git-commit: 06996ee9eb635fe204c0c3938e6937e8871c8a90
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# Adobe Analytics과 Advertising 통합 Adobe

다음과 같은 방법으로 Adobe 광고를 Analytics와 통합할 수 있습니다.

## 다음 기간 동안 데이터 교환 [!DNL Analytics] 및 Adobe 광고

### 가져오기 [!DNL Analytics] Adobe 광고에 대한 데이터

포함 [[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md),[!DNL Search, Social, & Commerce] 및 DSP 가져오기:

* **[!DNL Analytics]세그먼트:**  에서 생성된 모든 광고주 또는 에이전시 세그먼트에 대한 메타데이터, 계층 데이터 및 고유 대상 데이터 [!DNL Analytics] Experience Cloud에 게시됩니다.

* **[!DNL Analytics]사이트 참여 지표**

* **[!DNL Analytics]표준, 사용자 지정 및 예약된 지표**

### Adobe 광고 데이터 보내기 [!DNL Analytics]

* **Adobe 광고의 트래픽 지표**

* **Adobe 광고의 Dimension**

>[!NOTE]
>
>대상 [!DNL Search, Social, & Commerce], 이 기능은 대부분의 광고 네트워크 및 캠페인 유형에 대해 지원됩니다. 에서 &quot;지원되는 인벤토리&quot;를 참조하십시오. [!DNL Search, Social, & Commerce] 자세한 내용은 안내서 를 참조하십시오.<!-- add link when that's published in ExL -->

### 사용 [!DNL Analytics] 생성할 세그먼트 [!DNL Google Ads Audiences] {#audience-manager-google-audiences}

*을 사용하는 옵트인 광고주 [!DNL Advertising Search, Social, & Commerce] 전용*

<!-- Verify all -->

다음 범위 내 [!DNL Search, Social, & Commerce], 다음을 만들 수 있습니다. [!DNL Google Ads] Google 고객은 기존 을 사용하여 사용자 ID의 대상을 일치시킵니다 [!DNL Analytics] 세그먼트. 여기에는 Adobe Experience Cloud에 게시된 Adobe Analytics 세그먼트와 Adobe Experience Cloud을 사용하여 만든 세그먼트가 포함됩니다 [!DNL Audience Library]. 자세한 내용은 내의 제품 내 도움말을 참조하십시오 [!DNL Search, Social, & Commerce].

[사용자 ID의 고객 일치](https://support.google.com/google-ads/answer/9199250) 웹 사이트 태그 기반 대상처럼 작동하지만, 표준 고객 일치 및 웹 사이트 태그 기반 대상과 구별되는 이점을 얻기 위해 비 PII ID가 고유 대상자 구성원에게 할당됩니다.

필요한 사용자 ID를 만들려면 Adobe Advertising JavaScript 태그를 사용해야 합니다 <!-- with a user ID parameter -->웹 사이트에서. 자세한 내용은 Adobe 계정 팀에 문의하십시오.

![세그먼트 작성 프로세스](/help/integrations/assets/ad_search_user_id_pic.png)

대상자를 만들면 다음에서 사용할 수 있습니다. [!DNL Google Ads] 캠페인 대상: [캠페인 수준 또는 광고 그룹 수준의 타겟 또는 제외](#audience-manager-targets).

### 사용 [!DNL Analytics] 광고를 Target 또는 제외할 세그먼트 {#analytics-targets}

* (옵트인 광고주: [!DNL Search, Social, & Commerce]) 다음을 사용할 수 있습니다. [!DNL Google Ads] 다음 위치에 있었던 대상자 [을(를) 사용하여 생성됨 [!DNL Analytics] 세그먼트](#audience-manager-google-audiences) 를 캠페인 수준 또는 광고 그룹 수준의 타겟 또는 제외로 사용 [!DNL Google Ads] 캠페인.

* (DSP을 사용하는 광고주) 기존 광고주를 사용할 수 있습니다 [!DNL Analytics] 세그먼트를 광고 배치 타겟으로 지정합니다. 재사용 가능한 대상에 세그먼트를 선택적으로 포함할 수 있으며, 이 대상은 여러 배치에 대한 타겟 또는 제외로 사용할 수 있습니다.

* (Advertising Creative가 있는 광고주) 기존 광고주를 사용할 수 있습니다 [!DNL Analytics] 광고 경험에서 특정 크리에이티브를 위한 타겟으로서의 세그먼트.
