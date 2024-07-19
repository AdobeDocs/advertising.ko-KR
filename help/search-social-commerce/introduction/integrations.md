---
title: Adobe Experience Cloud 솔루션 및 서비스와의 통합
description: Adobe Experience Cloud 솔루션 및 서비스와의 검색, 소셜 및 Commerce 통합에 대해 알아봅니다.
exl-id: 26456f60-937a-4f39-b5cf-a71c1c1b4833
feature: Search Introduction
source-git-commit: e16bc62127a708de8f4deb1eddfa53a14405cbc2
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 0%

---

# Adobe Experience Cloud 솔루션 및 서비스와의 통합

Advertising Search, Social 및 Commerce이 다음 [!DNL Adobe] 제품과 통합되었습니다.

* [Adobe Experience Platform의 태그](https://experienceleague.adobe.com/docs/experience-platform/tags/extensions/client/overview.html) — Adobe Experience Platform용 [Adobe Advertising Cloud 확장](https://exchange.adobe.com/apps/ec/100155)을 사용하여 광고 랜딩 페이지에 대한 서드파티 추적 태그뿐만 아니라 Adobe Advertising 전환 추적 태그를 만들 수 있습니다. (또한 [Search, Social 및 Commerce 내에서 직접 전환 추적 태그를 만들 수 있습니다](/help/search-social-commerce/tools/conversion-tag-generate.md).) 태그에 포함할 내용은 Adobe 계정 팀이나 구현 팀에 문의하십시오.

* Adobe Analytics — (옵트인 기능) Adobe Advertising과 [!DNL Analytics]은(는) 다음과 같은 방법으로 통합됩니다.

   * Adobe Advertising과 [!DNL Analytics]이(가) 데이터를 원활하게 공유합니다. [!DNL Analytics]은(는) 사이트 참여 및 전환 데이터를 매일 검색, 소셜 및 Commerce으로 보낼 수 있습니다. 해당 데이터는 광고 최적화 및 보고에 사용할 수 있습니다. 또한 Adobe Advertising은 광고 네트워크에서 노출 횟수, 클릭 수, 비용을 포함한 광고 트래픽 데이터를 매일 [!DNL Analytics](모든 보고 도구에서 사용 가능)으로 보낼 수 있습니다.

     각 광고 네트워크 및 광고 유형에 대한 [!DNL Analytics] 지원에 대한 자세한 내용은 &quot;[지원되는 인벤토리](/help/search-social-commerce/introduction/supported-inventory.md)&quot;을(를) 참조하십시오. 데이터 교환에 대한 자세한 내용은 &quot;[개요 [!DNL Analytics for Advertising]](https://experienceleague.adobe.com/docs/advertising/integrations/analytics/overview.html){target="_blank"}&quot;도 참조하세요.

     데이터를 교환하려면 먼저 Adobe Advertising과 [!DNL Analytics]을(를) 모두 구성해야 합니다. 초기 설정에 대한 자세한 내용은 Adobe 계정 팀에 문의하십시오.

     >[!NOTE]
     >
     >기본적으로 [!DNL Analytics] 지표는 검색, 소셜 및 Commerce 화면에 표시되지 않습니다. [!DNL Adobe] 구현 팀이 Adobe Advertising에 전달할 선택된 표준 또는 사용자 지정 이벤트를 구성한 후에는 명시적으로 [캠페인 관리 보기, 포트폴리오 및 보고서에서 지표를 사용할 수 있도록 설정](/help/search-social-commerce/admin/conversion-metrics/conversion-metric-about.md)해야 합니다. 표시된 지표 이름을 [!DNL Analytics]에서 변경하지 않고 선택적으로 변경할 수 있습니다. UI에서 지표를 볼 수 있도록 하고 [!UICONTROL Admin] > [!UICONTROL Conversions]에서 지표의 이름을 변경할 수 있습니다.

   * [!DNL Analytics]이(가) 있지만 Audience Manager이 없는 광고주는 Adobe Experience Cloud과 공유된 [!DNL Analytics]개 세그먼트에서 [만들기 [!DNL Google Ads] 고객 일치 대상](/help/search-social-commerce/campaign-management/campaigns/google-audience-from-adobe-audience.md)을(를) 만들 수 있습니다. 자격을 얻으려면 광고주는 [Adobe Experience Platform ID 서비스](https://experienceleague.adobe.com/docs/id-service/using/home.html)를 구현하고 웹 사이트에 태그를 배포해야 합니다. 그런 다음 [!DNL Google Ads] 캠페인의 대상을 캠페인 수준 또는 광고 그룹 수준 [타겟](/help/search-social-commerce/campaign-management/campaigns/audience-targets-manage.md) 또는 [제외](/help/search-social-commerce/campaign-management/campaigns/audience-exclusions-manage.md)(으)로 사용할 수 있습니다.

* Adobe Audience Manager 세그먼트 - (옵트인 기능) 검색, 소셜 및 Commerce을 대상으로 하는 Audience Manager 세그먼트에서 [고객 일치 대상](/help/search-social-commerce/campaign-management/campaigns/google-audience-from-adobe-audience.md)을 만들 수 있습니다.  [!DNL Google Ads]  여기에는 Adobe Experience Cloud에 게시된 [!DNL Analytics]개의 세그먼트와 Adobe Experience Cloud 대상 라이브러리를 사용하여 만든 세그먼트가 포함될 수 있습니다. 그런 다음 [!DNL Google Ads] 캠페인의 대상을 캠페인 수준 또는 광고 그룹 수준 [타겟](/help/search-social-commerce/campaign-management/campaigns/audience-targets-manage.md) 또는 [제외](/help/search-social-commerce/campaign-management/campaigns/audience-exclusions-manage.md)(으)로 사용할 수 있습니다.

  자세한 내용은 &quot;[Adobe Audience Manager과 Adobe Advertising 통합](https://experienceleague.adobe.com/docs/advertising/integrations/audience-manager/overview.html)&quot;을 참조하십시오.

* Adobe Target — Search, Social, &amp; Commerce과 [!DNL Target] 간의 클릭스루 신호 공유를 구현하고, 광고에 대해 [!DNL Target]에서 A/B 테스트 활동을 설정한 다음 [!DNL Analytics] Analysis Workspace을 사용하여 테스트 데이터를 볼 수 있습니다.

* Adobe Campaign — [!DNL Campaign]](/help/search-social-commerce/campaign-management/campaigns/google-audience-from-campaign-email-list.md) 내에서 전자 메일 목록을 사용하여 [고객 일치 대상을 만들고 업데이트할 수 있습니다 [!DNL Google Ads] .

* Adobe Experience Cloud 알림 — (Adobe Experience Cloud을 통해 로그인한 경우) 각 페이지 상단의 알림 링크([경고 알림](/help/search-social-commerce/assets/notifications-panel.png "경고 알림"))에서 모든 Adobe Experience Cloud 시스템 업데이트, 게시물, 언급 및 공유된 에셋을 볼 수 있습니다. Adobe Experience Cloud 액세스에 대한 자세한 내용은 Adobe 계정 팀에 문의하십시오.
