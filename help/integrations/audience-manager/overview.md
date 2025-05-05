---
title: Adobe Audience Manager과 통합 Adobe Advertising
description: Adobe Advertising이 Adobe Audience Manager과 데이터를 교환할 수 있는 다양한 방법에 대해 알아봅니다.
feature: Integration with Adobe Audience Manager
exl-id: 5b0ecb82-fb5c-48c5-a599-15b548f59461
source-git-commit: d0260fc3b10f1944b82cdc4c1e3b8137a695e05e
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 0%

---

# Adobe Audience Manager과 통합 Adobe Advertising

다음과 같은 방법으로 Adobe Advertising을 Audience Manager과 통합할 수 있습니다.

## 광고 타깃팅을 위해 Audience Manager 및 기타 [!DNL Adobe]개 세그먼트 동기화

[!DNL Search, Social, & Commerce]과(와) DSP은 광고주나 에이전시의 모든 Audience Manager 및 기타 [!DNL Adobe]개 대상에 대한 메타데이터, 계층 데이터 및 고유한 대상 데이터를 가져올 수 있습니다. 이 고유한 연결은 Adobe Advertising을 사용하는 마케터만 사용할 수 있습니다. &quot;[광고 타깃팅용 Adobe Audience Manager 세그먼트 가져오기](/help/integrations/audience-manager/import-audiences.md)&quot;를 참조하십시오.

### Audience Manager 및 기타 [!DNL Adobe] 세그먼트를 사용하여 [!DNL Google Ads Audiences] 만들기 {#audience-manager-google-audiences}

[!DNL Advertising Search, Social, & Commerce]만 사용하는 *옵트인 광고주*

[!DNL Search, Social, & Commerce] 내에서 [!UICONTROL Adobe Media Optimizer (HTTP)] 및 [!UICONTROL Adobe Media Optimizer Batch Destination]을(를) 대상으로 하는 기존 Audience Manager 세그먼트를 사용하여 사용자 ID에서 [!DNL Google Ads] 고객 일치 대상을 만들 수 있습니다. [!DNL Media Optimizer]은(는) [!DNL Search, Social, & Commerce]의 이전 이름입니다. 여기에는 Adobe Experience Cloud에 게시된 Adobe Analytics 세그먼트와 Adobe Experience Cloud [!DNL Audience Library]을(를) 사용하여 만든 세그먼트가 포함됩니다. 자세한 내용은 &quot;[대상자 만들기 [!DNL Google Ads] 고객 일치 대상자 [!DNL Adobe] 대상자](/help/search-social-commerce/campaign-management/campaigns/google-audience-from-adobe-audience.md)&quot;를 참조하십시오.

[사용자 ID의 고객 일치 대상](https://support.google.com/google-ads/answer/9199250)은(는) 웹 사이트 태그 기반 대상과 비슷하게 작동하지만, 표준 고객 일치 및 웹 사이트 태그 기반 대상과 구별되는 이점을 얻기 위해 PII ID가 아닌 ID가 고유 대상자 구성원에게 할당됩니다.

필요한 사용자 ID를 만들려면 웹 사이트에서 Adobe Advertising JavaScript 태그 <!-- with a user ID parameter -->을(를) 사용해야 합니다. 자세한 내용은 Adobe 계정 팀에 문의하십시오.

![세그먼트 만들기 프로세스](/help/integrations/assets/ad_search_user_id_pic.png)

대상을 만들면 [!DNL Google Ads] 캠페인에서 [캠페인 수준 또는 광고 그룹 수준 타겟 또는 제외](#audience-manager-targets)(으)로 사용할 수 있습니다.

### Audience Manager 및 기타 [!DNL Adobe] 세그먼트를 사용하여 광고를 타깃팅하거나 제외합니다. {#audience-manager-targets}

* ([!DNL Search, Social, & Commerce]을(를) 사용하는 옵트인 광고주) [!DNL Google Ads] 캠페인에서  [!DNL Adobe] 세그먼트[&#128279;](#audience-manager-google-audiences)를 사용하여 만든 [!DNL Google Ads] 대상을 캠페인 수준 또는 광고 그룹 수준 타겟 또는 제외로 사용할 수 있습니다.

* (DSP을 사용하는 광고주) 기존 [!DNL Adobe] 세그먼트를 광고 배치 대상으로 사용할 수 있습니다. 재사용 가능한 대상에 세그먼트를 선택적으로 포함할 수 있으며, 이 대상은 여러 배치에 대한 타겟 또는 제외로 사용할 수 있습니다.

* (Advertising Creative이 있는 광고주) 기존 [!DNL Adobe] 세그먼트를 광고 경험의 특정 크리에이티브를 위한 대상으로 사용할 수 있습니다.

>[!NOTE]
>
>Audience Manager 및 Experience Cloud [!DNL Audience Library] 인터페이스에서 대상을 만드는 방법과 다양한 대상 유형에 대한 일반적인 사용 사례에 대한 자세한 내용은 &quot;[대상 만들기 옵션](https://experienceleague.adobe.com/docs/experience-cloud-kcs/kbarticles/KA-16471.html)&quot;을 참조하십시오.

## Audience Manager에 DSP Media 노출 데이터 보내기

*DSP만 있는 광고주*

Adobe Audience Manager을 사용하는 DSP 고객은 Audience Manager에 대한 픽셀 호출을 사용하여 광고 캠페인에서 데이터를 캡처할 수 있습니다. 그런 다음 캠페인 데이터를 사용하여 규칙 기반 트레이트를 구축할 수 있습니다. 이 트레이트를 사용하여 고급 세분화, 빈도 관리, 마케팅 분석 및 보고 통찰력과 같은 다양한 DSP 사용 사례를 활성화할 수 있습니다.

자세한 내용은 &quot;[Adobe Audience Manager에 DSP Media 노출 데이터 전송 개요](/help/integrations/audience-manager/media-data-integration/overview.md)&quot;를 참조하십시오.

## Audience Analytics을 통해 사이트 활동에 대한 더 풍부한 통찰력 얻기

[[!DNL Adobe Audience Analytics]](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html)을(를) 가진 Adobe Advertising 고객은 사이트 활동에 대한 보강된 통찰력을 위해 Adobe Advertising이 추적한 데이터와 Audience Manager 세그먼트를 모두 [!DNL Analytics]에 보낼 수 있습니다.

자세한 내용은 &quot;[[!DNL Adobe Audience Analytics] Adobe Advertising 고객에 대해](/help/integrations/audience-manager/audience-analytics.md)&quot;을(를) 참조하십시오.
