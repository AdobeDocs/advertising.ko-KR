---
title: Adobe Experience Cloud 솔루션 및 서비스와의 통합
description: Adobe Experience Cloud 솔루션 및 서비스와의 검색, 소셜 및 상거래 통합에 대해 알아봅니다.
source-git-commit: 0c19479cb8ef4e9e037a46ab72f75b7423de5073
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Adobe Experience Cloud 솔루션 및 서비스와의 통합

Advertising Search, Social 및 Commerce는 다음과 통합됩니다 [!DNL Adobe] 제품.

* [Adobe Experience Platform의 태그](https://experienceleague.adobe.com/docs/experience-platform/tags/extensions/client/overview.html) — 다음을 사용할 수 있습니다 [Adobe Advertising Cloud 확장](https://exchange.adobe.com/apps/ec/100155) Adobe Experience Platform에서 광고 랜딩 페이지에 대한 서드파티 추적 태그뿐만 아니라 Adobe 광고 전환 추적 태그를 만들 수 있습니다. (다음을 수행할 수도 있습니다. [검색, 소셜 및 상거래 내에서 직접 전환 추적 태그 만들기](/help/search-social-commerce/tools/conversion-tag-generate.md).) 태그에 포함할 내용은 Adobe 계정 팀이나 구현 팀에 문의하십시오.

* Adobe Analytics — (옵트인 기능) Adobe 광고 및 [!DNL Analytics] 는 다음과 같은 방법으로 통합됩니다.

   * Adobe 광고 및 [!DNL Analytics] 데이터를 원활하게 공유합니다. [!DNL Analytics] 은 사이트 참여 및 전환 데이터를 매일 검색, 소셜 및 상거래로 전송할 수 있습니다. 여기서 광고 최적화 및 보고를 위해 데이터를 사용할 수 있습니다. 또한 Adobe 광고는 노출 횟수, 클릭 수, 비용을 포함한 광고 트래픽 데이터를 광고 네트워크에서 매일 (으)로 보낼 수 있습니다. [!DNL Analytics]: 모든 보고 도구에서 데이터를 사용할 수 있습니다.

      를 참조하십시오.[지원되는 인벤토리](/help/search-social-commerce/introduction/supported-inventory.md)에 대한 자세한 내용은 &quot; [!DNL Analytics] 각 광고 네트워크 및 광고 유형에 대한 지원. 참조: &quot;[개요 [!DNL Analytics for Advertising]](https://experienceleague.adobe.com/docs/advertising/integrations/analytics/overview.html)데이터 교환에 대한 자세한 내용은 &quot;을 참조하십시오.

      데이터를 교환하려면 광고 및 를 모두 Adobe [!DNL Analytics] 은(는) 처음에 구성해야 합니다. 초기 설정에 대한 자세한 내용은 Adobe 계정 팀에 문의하십시오.

      >[!NOTE]
      >
      >기본적으로 [!DNL Analytics] 지표는 검색, 소셜 및 상거래 화면에 표시되지 않습니다. 다음을 명시적으로 수행해야 합니다. [캠페인 관리 보기, 포트폴리오 및 보고서에서 지표를 사용할 수 있도록 설정](/help/search-social-commerce/admin/transaction-properties/transaction-property-about.md) 다음 이후 [!DNL Adobe] 구현 팀이 선택한 표준 또는 사용자 지정 이벤트를 Adobe 광고에 전달하도록 구성했습니다. 표시된 지표 이름을 변경하지 않고 선택적으로 변경할 수 있습니다 [!DNL Analytics]). UI에서 지표를 볼 수 있도록 하고 지표의 이름을 변경할 수 있습니다. [!UICONTROL Admin] > [!UICONTROL Transaction Properties].

   * 를 사용하는 광고주 [!DNL Analytics] 그러나 Audience Manager은 할 수 없습니다. [만들기 [!DNL Google Ads] 고객 일치 대상](/help/search-social-commerce/campaign-management/campaigns/google-audience-from-adobe-audience.md) 출처: [!DNL Analytics] Adobe Experience Cloud과 공유되는 세그먼트입니다. 자격을 얻으려면 광고주가 다음을 구현해야 합니다. [Adobe Experience Platform ID 서비스](https://experienceleague.adobe.com/docs/id-service/using/home.html) 웹 사이트에 태그를 배포할 수 있습니다. 그런 다음 의 대상자를 사용할 수 있습니다. [!DNL Google Ads] 캠페인 수준 또는 광고 그룹 수준의 캠페인 [타겟](/help/search-social-commerce/campaign-management/campaigns/audience-targets-manage.md) 또는 [제외](/help/search-social-commerce/campaign-management/campaigns/audience-exclusions-manage.md).

* Adobe Audience Manager 세그먼트 - (옵트인 기능) 다음과 같은 작업을 수행할 수 있습니다 [만들기 [!DNL Google Ads] 고객 일치 대상](/help/search-social-commerce/campaign-management/campaigns/google-audience-from-adobe-audience.md) 검색, 소셜 및 상거래를 대상으로 하는 Audience Manager 세그먼트. 여기에는 다음이 포함될 수 있습니다. [!DNL Analytics] Adobe Experience Cloud에 게시되는 세그먼트 및 Adobe Experience Cloud 대상 라이브러리를 사용하여 생성되는 세그먼트입니다. 그런 다음 의 대상자를 사용할 수 있습니다. [!DNL Google Ads] 캠페인 수준 또는 광고 그룹 수준의 캠페인 [타겟](/help/search-social-commerce/campaign-management/campaigns/audience-targets-manage.md) 또는 [제외](/help/search-social-commerce/campaign-management/campaigns/audience-exclusions-manage.md).

   를 참조하십시오.[Adobe Audience Manager과 Advertising 통합 Adobe](https://experienceleague.adobe.com/docs/advertising/integrations/audience-manager/overview.html)&quot; 을 참조하십시오.

* Adobe Target — 검색, 소셜, 상거래 및 [!DNL Target]에서 A/B 테스트 활동 설정 [!DNL Target] 광고의 경우 [!DNL Analytics] Analysis Workspace을 사용하여 테스트 데이터를 볼 수 있습니다.

* Adobe Campaign — 다음과 같은 작업을 수행할 수 있습니다. [만들기 및 업데이트 [!DNL Google Ads] 내의 이메일 목록을 사용하는 고객 일치 [!DNL Campaign]](/help/search-social-commerce/campaign-management/campaigns/google-audience-from-campaign-email-list.md).

* Adobe Experience Cloud 알림 — (Adobe Experience Cloud을 통해 로그인한 경우) 알림 링크([경고 알림](/help/search-social-commerce/assets/notifications-panel.png "경고 알림"))각 페이지의 맨 위에서 모든 Adobe Experience Cloud 시스템 업데이트, 게시물, 언급 및 공유된 에셋을 볼 수 있습니다. Adobe Experience Cloud 액세스에 대한 자세한 내용은 Adobe 계정 팀에 문의하십시오.

