---
title: Adobe Advertising integrations with Adobe Audience Manager
description: Learn about the different ways in which Adobe Advertising can exchange data with Adobe Audience Manager.
feature: Integration with Adobe Audience Manager
exl-id: 5b0ecb82-fb5c-48c5-a599-15b548f59461
TQID: https://experienceleague.adobe.com/4O4O-DmHhClvSiOSxM9blAEvVslzYzRobEyU6RGeMEQ
product_v2: id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2: id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6id: f2860a4b-f905-4545-bead-1bbc92564592
subfeature_v2: id: d1e2786d-1070-4f97-93d7-f5b95de25b2b
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 7845129ba6566c1aaaf160cc6f9ad33bf1731f75
workflow-type: tm+mt
source-wordcount: 517
ht-degree: 0%

---

# Adobe Advertising integrations with Adobe Audience Manager

You can integrate Adobe Advertising with Audience Manager in the following ways.

## Synchronize Audience Manager and other [!DNL Adobe] segments for ad targeting

[!DNL Search, Social, & Commerce] and DSP can pull in metadata, hierarchy data, and unique audience data for all of an advertiser&#39;s or agency&#39;s Audience Manager and other [!DNL Adobe] audiences. This unique connection is available only to marketers using Adobe Advertising. See &quot;[Import Adobe Audience Manager segments for ad targeting](/help/integrations/audience-manager/import-audiences.md).&quot;

### Use Audience Manager and other [!DNL Adobe] segments to create [!DNL Google Ads] audiences {#audience-manager-google-audiences}

*Opted-in advertisers with [!DNL Advertising Search, Social, & Commerce] only*

Within [!DNL Search, Social, & Commerce], you can create [!DNL Google Ads] customer match audiences from user IDs using your existing Audience Manager segments that have [!UICONTROL Adobe Media Optimizer (HTTP)] and [!UICONTROL Adobe Media Optimizer Batch Destination] as destinations. ([!DNL Media Optimizer] is a former name for [!DNL Search, Social, & Commerce].) This includes Adobe Analytics segments that are published to Adobe CX Enterprise and segments that are created using the Adobe CX Enterprise [!DNL Audience Library]. For more information, see &quot;[Create [!DNL Google Ads] customer match audiences from [!DNL Adobe] audiences](/help/search-social-commerce/campaign-management/campaigns/google-audience-from-adobe-audience.md).&quot;

[Customer match audiences from user IDs](https://support.google.com/google-ads/answer/9199250) work like website tag-based audiences, but a non-PII ID is assigned to unique audience members for distinct benefits over standard customer match and website tag-based audiences.

To create the necessary user IDs, you must use an Adobe Advertising JavaScript tag <!-- with a user ID parameter -->on your websites. Contact your Adobe Account Team for more information.

![segment creation process](/help/integrations/assets/ad_search_user_id_pic.png)

Once you create the audiences, you can use them in [!DNL Google Ads] campaigns as [campaign-level or ad group-level targets or exclusions](#audience-manager-targets).

### Use Audience Manager and other [!DNL Adobe] segments to target or exclude ads {#audience-manager-targets}

* (Opted-in advertisers with [!DNL Search, Social, & Commerce]) You can use any [!DNL Google Ads] audiences that were [created using [!DNL Adobe] segments](#audience-manager-google-audiences) as campaign-level or ad group-level targets or exclusions in your [!DNL Google Ads] campaigns.

* (Advertisers with DSP) You can use your existing [!DNL Adobe] segments as targets for your ad placements. 재사용 가능한 대상에 세그먼트를 선택적으로 포함할 수 있으며, 이 대상은 여러 배치에 대한 타겟 또는 제외로 사용할 수 있습니다.

* (Advertising Creative을 사용하는 광고주) 기존 [!DNL Adobe] 세그먼트를 광고 경험의 특정 크리에이티브를 위한 타겟으로 사용할 수 있습니다.

>[!NOTE]
>
>Audience Manager 및 Adobe CX Enterprise [!DNL Audience Library] 인터페이스에서 대상을 만드는 방법과 다양한 대상 유형에 대한 일반적인 사용 사례에 대한 자세한 내용은 &quot;[대상 만들기 옵션](https://experienceleague.adobe.com/docs/experience-cloud-kcs/kbarticles/KA-16471.html)&quot;을 참조하십시오.

## Audience Manager에 DSP 미디어 노출 데이터 보내기

*DSP만 있는 광고주*

Adobe Audience Manager을 사용하는 DSP 고객은 Audience Manager에 대한 픽셀 호출을 사용하여 광고 캠페인의 데이터를 캡처할 수 있습니다. 그런 다음 캠페인 데이터를 사용하여 규칙 기반 트레이트를 구축할 수 있습니다. 이 트레이트를 사용하여 새로운 세그먼트를 정의하여 보다 고급 세그멘테이션, 빈도 관리, 마케팅 분석 및 보고 통찰력과 같은 다양한 DSP 사용 사례를 활성화할 수 있습니다.

자세한 내용은 &quot;[Adobe Audience Manager에 DSP 미디어 노출 데이터 전송 개요](/help/integrations/audience-manager/media-data-integration/overview.md)&quot;를 참조하십시오.

## Audience Analytics을 통해 사이트 활동에 대한 보다 풍부한 통찰력 얻기

[[!DNL Adobe Audience Analytics]](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html)을(를) 가진 Adobe Advertising 고객은 사이트 활동에 대한 풍부한 통찰력을 위해 Adobe Advertising 추적 데이터와 Audience Manager 세그먼트를 모두 [!DNL Analytics]에 보낼 수 있습니다.

자세한 내용은 &quot;[[!DNL Adobe Audience Analytics] Adobe Advertising 고객용](/help/integrations/audience-manager/audience-analytics.md)&quot;을 참조하십시오.
