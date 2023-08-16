---
title: AMO ID(s_kwcid) 추적 매개 변수
description: Adobe Analytics과 Adobe Advertising 데이터를 공유하는 데 사용되는 추적 매개 변수에 대해 알아봅니다.
exl-id: 3f739f1c-3cb7-40d0-86ab-cf66afe6a06f
feature: Search Tracking
source-git-commit: 3c91d0a764397fd72192f5a522ac936176047bc2
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# AMO ID(s_kwcid) 추적 매개 변수

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

<!-- This should go in the Analytics integration chapter > IDs page, under "AMO IDs" once I've finalized content for DSP clients.  -->

Adobe Advertising은 AMO ID append 매개 변수라고도 하는 를 사용하여 Adobe Analytics과 캠페인에 대한 데이터를 공유합니다. `s_kwcid` 매개 변수 : 광고 채널과 광고 네트워크별 요소로 구성됩니다.

매개 변수는 다음 방법 중 하나로 추적 URL에 추가됩니다.

* (권장) 서버측 삽입 기능이 구현됩니다.

   * DSP 고객: 픽셀 서버는 최종 사용자가 Adobe Advertising 픽셀로 디스플레이 광고를 볼 때 s_kwcid 매개 변수를 랜딩 페이지 접미사에 자동으로 추가합니다.

   * 검색, 소셜 및 상거래 고객:

      * 대상 [!DNL Google Ads] 및 [!DNL Microsoft® Advertising] 이(가) 있는 계정 [!UICONTROL Auto Upload] 계정 또는 캠페인에 대해 이 설정을 활성화하면, 픽셀 서버는 최종 사용자가 Adobe Advertising 픽셀이 있는 광고를 클릭할 때 s_kwcid 매개 변수를 랜딩 페이지 접미사에 자동으로 추가합니다.

      * 기타 광고 네트워크의 경우 또는 [!DNL Google Ads] 및 [!DNL Microsoft® Advertising] 이(가) 있는 계정 [!UICONTROL Auto Upload] 비활성화로 설정하면 매개 변수를 계정 수준 추가 매개 변수에 수동으로 추가하고 기본 URL에 추가합니다.

* 서버측 삽입 기능은 구현되지 않습니다.

   * DSP 고객:

      * 대상 [!DNL Flashtalking] 광고 태그, 수동으로에 추가 매크로 삽입[추가 [!DNL Analytics for Advertising] 매크로 위치 [!DNL Flashtalking] 광고 태그](/help/integrations/analytics/macros-flashtalking.md).&quot;

      * 대상 [!DNL Google Campaign Manager 360] 광고 태그, 수동으로에 추가 매크로 삽입[추가 [!DNL Analytics for Advertising] 매크로 위치 [!DNL Google Campaign Manager 360] 광고 태그](/help/integrations/analytics/macros-google-campaign-manager.md).&quot;

  <!--  * For all other ads, XXXX. -->

   * 검색, 소셜 및 상거래 고객:

      * 대상 ([!DNL Google Ads] 및 [!DNL Microsoft® Advertising]) 광고, 수동으로 AMO ID 매개 변수를 랜딩 페이지 접미사에 추가합니다.

      * 다른 모든 광고 네트워크의 광고의 경우, AMO ID 매개 변수를 계정 수준 추가 매개 변수에 수동으로 추가하여 기본 URL에 추가합니다.

서버측 삽입 기능을 구현하거나 비즈니스에 가장 적합한 옵션을 결정하려면 Adobe 계정 팀에 문의하십시오.

DSP 및 검색, 소셜, 상거래에 대한 AMO ID 형식은 &quot;[사용한 Adobe Advertising ID [!DNL Analytics]](/help/integrations/analytics/ids.md#amo-id).&quot;

>[!MORELIKETHIS]
>
>* [개요 [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md){target="_blank"}
>* [사용한 Adobe Advertising ID [!DNL Analytics]](/help/integrations/analytics/ids.md#amo-id){target="_blank"}
>* (검색, 소셜 및 상거래) [광고 네트워크 계정 관리](/help/search-social-commerce/campaign-management/accounts/ad-network-account-manage.md)
>* (검색, 소셜 및 상거래) [Baidu 캠페인 설정](/help/search-social-commerce/campaign-management/campaigns/campaign-settings-baidu.md)
>* (검색, 소셜 및 상거래) [Google 광고 캠페인 설정](/help/search-social-commerce/campaign-management/campaigns/campaign-settings-google.md)
>* (검색, 소셜 및 상거래) [Microsoft® Advertising 캠페인 설정](/help/search-social-commerce/campaign-management/campaigns/campaign-settings-microsoft.md)
>* (검색, 소셜 및 상거래) [야후! 일본 광고 캠페인 설정](/help/search-social-commerce/campaign-management/campaigns/campaign-settings-yahoo-japan.md)
>* (검색, 소셜 및 상거래) [Yandex 캠페인 설정](/help/search-social-commerce/campaign-management/campaigns/campaign-settings-yandex.md)
