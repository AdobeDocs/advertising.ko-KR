---
title: AMO ID(s_kwcid) 추적 매개 변수
description: Adobe Analytics과 Adobe Advertising 데이터를 공유하는 데 사용되는 추적 매개 변수에 대해 알아봅니다.
exl-id: 3f739f1c-3cb7-40d0-86ab-cf66afe6a06f
feature: Search Tracking
source-git-commit: a150a55fd8d97db83cc269c787a1c67d557b7e3a
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# AMO ID(s_kwcid) 추적 매개 변수

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

<!-- This should go in the Analytics integration chapter > IDs page, under "AMO IDs."  But I'll need to update with when/where to add the code for DSP clients. -->

Adobe Advertising은 AMO ID append 매개 변수라고도 하는 를 사용하여 Adobe Analytics과 캠페인에 대한 데이터를 공유합니다. `s_kwcid` 매개 변수 : 광고 채널과 광고 네트워크별 요소로 구성됩니다.

<!-- add everything below to IDs page -->

매개 변수는 다음 방법 중 하나로 추적 URL에 추가됩니다.

* (권장) 서버측 삽입 기능이 구현됩니다.

  대상 [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 이(가) 있는 계정 [!UICONTROL Auto Upload] 계정 또는 캠페인에 대해 활성화된 설정을 지정하면, 픽셀 서버는 최종 사용자가 광고를 클릭할 때 랜딩 페이지 접미사에 AMO ID 매개 변수를 자동으로 추가합니다 <!-- click a search ad or views a display ad --> Adobe Advertising 픽셀 사용.

  기타 광고 네트워크의 경우 또는 [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 이(가) 있는 계정 [!UICONTROL Auto Upload] 비활성화로 설정하면 AMO ID 매개 변수를 계정 수준 추가 매개 변수에 수동으로 추가하고 기본 URL에 추가합니다.

* <!-- (Search, Social, & Commerce only) -->서버측 삽입 기능은 구현되지 않으며, AMO ID 매개 변수를 ([!DNL Google Ads] 및 [!DNL Microsoft Advertising]) 랜딩 페이지 접미사 또는 (기타 광고 네트워크) 계정 수준 추가 매개 변수.

서버측 삽입 기능을 구현하거나 비즈니스에 가장 적합한 옵션을 결정하려면 Adobe 계정 팀에 문의하십시오.

DSP 및 검색, 소셜, 상거래에 대한 AMO ID 형식은 &quot;[사용한 Adobe Advertising ID [!DNL Analytics]](/help/integrations/analytics/ids.md#amo-id).&quot;

>[!MORELIKETHIS]
>
>* [개요 [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md){target="_blank"}
>* [사용한 Adobe Advertising ID [!DNL Analytics]](/help/integrations/analytics/ids.md#amo-id){target="_blank"}
>* [광고 네트워크 계정 관리](/help/search-social-commerce/campaign-management/accounts/ad-network-account-manage.md)
>* [Baidu 캠페인 설정](/help/search-social-commerce/campaign-management/campaigns/campaign-settings-baidu.md)
>* [Google 광고 캠페인 설정](/help/search-social-commerce/campaign-management/campaigns/campaign-settings-google.md)
>* [Microsoft Advertising 캠페인 설정](/help/search-social-commerce/campaign-management/campaigns/campaign-settings-microsoft.md)
>* [야후! 일본 광고 캠페인 설정](/help/search-social-commerce/campaign-management/campaigns/campaign-settings-yahoo-japan.md)
>* [Yandex 캠페인 설정](/help/search-social-commerce/campaign-management/campaigns/campaign-settings-yandex.md)
