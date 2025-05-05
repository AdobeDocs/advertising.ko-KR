---
title: 광고 네트워크 계정 및 캠페인 구현 개요
description: 광고 네트워크 계정 설정, 동기화 및 관리와 관련된 작업에 대해 알아봅니다.
exl-id: 36307e65-81f8-4794-8a75-a37623b294ed
feature: Search Campaign Management
source-git-commit: 0af1c5591a59b9e1813209fea3ac6aaecc0e649b
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 0%

---

# 광고 네트워크 계정 및 캠페인 구현 개요

Adobe은 각 광고주와 함께 작동하여 광고 네트워크 계정 및 캠페인을 설정합니다. 여기에는 광고주의 계정에 연결하고 동기화하도록 검색, 소셜 및 Commerce 구성, 필요에 따라 새 캠페인 및 캠페인 구성 요소 만들기, 구성 요소 광고에 대한 추적 설정, 선택적 포트폴리오에 캠페인을 추가하여 검색, 소셜 및 Commerce이 광고에서 입찰을 최적화할 수 있도록 허용, 초기 비용, 클릭 및 매출 데이터 유효성 검사가 포함됩니다.

캠페인이 활성화되고 선택적으로 포트폴리오에 추가되면 Adobe 계정 관리 팀, 에이전시 팀 또는 광고주(서비스 수준 계약의 약관에 따라)는 각 캠페인을 모니터링하고 광고주의 목표를 충족하기 위해 필요한 경우 관련 구성 요소 및 설정을 변경해야 합니다.

이 페이지에는 동기화된 계정에 대한 캠페인 구조를 설정하는 방법을 포함하여 모든 계정 유형에 대한 정보가 포함되어 있습니다. [!DNL Naver]에 대한 추적 전용 계정 설정에 대한 추가 지침은 &quot;[구현 [!DNL Naver] 추적 전용 계정](/help/search-social-commerce/campaign-management/naver-tracking-only-account-implement.md)&quot;을 참조하세요.

## 계정 및 캠페인에 대한 초기 설정 작업

[!DNL Adobe] 및/또는 귀하의 에이전시가 귀하와 함께 다음 작업을 수행합니다.

1. (새 광고주 계정) 관리 계정을 설정합니다.

   1. 광고주 계정을 설정합니다.

   1. (필요한 경우) 광고주가 캠페인 데이터를 보고 관리하고 보고서를 생성할 수 있는 사용자 계정을 만듭니다.

1. (일부 광고 네트워크) 광고 네트워크의 API와 Search, Social 및 Commerce 사용자 인터페이스를 사용하여 각 계정에 액세스하려면 Search, Social 및 Commerce에 대한 권한을 받습니다.

1. 각 광고 네트워크 계정의 경우:

   1. (필요한 경우) 광고 네트워크에서 계정을 설정합니다.

   1. 계정 액세스 자격 증명과 추적 옵션이 포함된 검색, 소셜 및 Commerce에서 [해당 계정 레코드를 만들어](/help/search-social-commerce/campaign-management/accounts/ad-network-account-manage.md#create-account)계정과 통합하고 계정 상태를 [사용]으로 설정합니다.

      그런 다음 Search, Social 및 Commerce이 광고 네트워크와 동기화됩니다. 계정에 이미 캠페인 데이터가 포함되어 있는 경우 해당 데이터를 약 24시간 내에 사용할 수 있습니다.

   1. ([검색, 소셜 및 Commerce에서 만들거나 편집할 수 있는 광고 유형](/help/search-social-commerce/introduction/supported-inventory.md)) 계정에 캠페인 데이터가 아직 포함되어 있지 않은 경우 광고 유형에 사용할 수 있는 다음 방법 중 하나를 사용하여 검색, 소셜 및 Commerce 내에서 캠페인 구조 및 캠페인 구성 요소를 만듭니다.

      * (Google Ads, Microsoft Advertising, Yahoo! Ads 및 Yandex 계정만 해당) 사용자가 만든 광고 네트워크별 광고 템플릿과 FTP 위치에 업로드한 인벤토리 데이터 파일의 내용에 따라 인벤토리의 각 항목을 대상으로 하는 동적 광고 및 키워드를 만드는 [자동화된 프로세스를 설정합니다.](/help/search-social-commerce/campaign-management/inventory-feeds/inventory-feeds-about.md)

      * (Baidu, Google Ads, Microsoft Advertising, Yahoo! 일본 광고 및 Yandex 계정만 해당) 계정에 대해 원하는 만큼의 데이터가 포함된 [일괄 시트 파일](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-about.md)을 업로드한 다음 광고 네트워크에 게시합니다.

      * (Baidu, Google Ads, Microsoft Advertising, Yahoo! 일본 광고 및 Yandex 계정만 해당) 개별 구성 요소에 대한 데이터를 인터페이스에 직접 입력합니다. 대부분의 캠페인 및 광고 유형의 경우 캠페인 수준, 광고 그룹 수준 및 개별 키워드, 배치 및 광고 수준에서 데이터를 만들 수 있습니다.

      그러나 일부 캠페인 및 광고 유형에는 고유한 워크플로우가 필요합니다. [[!DNL Microsoft Advertising] 쇼핑 캠페인](/help/search-social-commerce/campaign-management/special-workflows/microsoft-shopping-campaigns.md), [[!DNL Google Ads] 동적 검색 광고](/help/search-social-commerce/campaign-management/special-workflows/google-dynamic-search-ads.md), [[!DNL Google Ads] 성과 최대 캠페인](/help/search-social-commerce/campaign-management/special-workflows/google-performance-max-campaigns.md) 및 [[!DNL Google Ads] 쇼핑 캠페인](/help/search-social-commerce/campaign-management/special-workflows/google-shopping-campaigns.md) 설정에 대한 지침을 참조하십시오.

   1. ([!DNL Naver] 추적 전용 계정 전용) 데이터가 포함된 [일괄 시트 파일](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-about.md)을 업로드하여 [!DNL Naver]에 게시하지 않고 검색, 소셜 및 Commerce에서 기존 캠페인, 광고 그룹 및 키워드를 복제합니다.

1. Adobe Advertising이 전환을 추적할 모든 광고에 대한 추적을 설정합니다.

   1. (Adobe Advertising 전환 추적 서비스를 사용하는 광고주) 필요한 경우 검색, 소셜 및 Commerce 클릭 추적 URL을 생성하고 업로드하여 광고에 대한 [클릭 추적을 설정](/help/search-social-commerce/tracking/click-tracking-ways-to-generate.md)하고 선택적으로 키워드, 배치 및 광고 확장을 설정합니다.

      [!DNL Google Ads] 성과 최대 캠페인의 경우 [캠페인의 추적 설정](/help/search-social-commerce/campaign-management/campaigns/campaign-settings-google.md)에서 모든 추적을 설정하십시오.

1. 추적 전용 캠페인의 경우 대신 일괄 시트를 사용하여 대상 URL을 생성한 다음 광고 네트워크의 기본 편집기를 사용하여 생성된 대상 URL을 관련 엔티티에 추가해야 합니다.

   1. 전환 추적을 설정합니다. 구현에 따라, 광고주의 웹 페이지에 전환 추적 태그를 추가하거나 광고주가 별도로 수집한 전환 데이터에 대해 일별 피드 드롭을 설정하는 작업이 여기에 포함될 수 있습니다.

      Adobe Advertising 전환 추적 서비스를 사용하는 경우 Search, Social 및 Commerce 내에서 전환 추적 태그 [를 생성하거나](/help/search-social-commerce/tools/conversion-tag-generate.md) [Adobe Experience Platform 사용](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/advertising/adobe-advertising-cloud.html?lang=ko)을 생성할 수 있습니다.

   1. 추적된 데이터의 유효성을 검사합니다.

   추적 설정에 대한 자세한 내용은 &quot;추적&quot; 장을 참조하십시오.

1. (Adobe Analytics을 사용하는 광고주) 데이터를 교환할 수 있도록 [Adobe Advertising과 Analytics를 통합](https://experienceleague.adobe.com/docs/advertising/integrations/analytics/overview.html?lang=ko)합니다.

1. (Search, Social 및 Commerce에서 입찰, 캠페인 예산 및/또는 캠페인 입찰 전략 타겟을 최적화할 수 있도록 하려면. [지원되는 캠페인 유형](/help/search-social-commerce/introduction/supported-inventory.md)만 해당) [포트폴리오에 캠페인을 할당](/help/search-social-commerce/campaign-management/campaign-assign-to-portfolio.md).

   아직 포트폴리오를 시작하지 않은 경우(입찰 및/또는 예산 최적화) 최적화 기능을 통해 비용 및 수익 모델을 구축할 수 있는 충분한 데이터를 수집하여 포트폴리오를 시작하기 전에 포트폴리오의 기준 성능을 설정할 수 있습니다.

   포트폴리오가 이미 시작된 경우 포트폴리오에 대한 학습을 활성화하십시오. 자세한 내용은 &quot;포트폴리오 전략 조정&quot;을 참조하십시오. 최적화 기능은 캠페인의 입찰 단위에 대한 데이터를 수집하는 동안 새 캠페인을 추가한 후에는 포트폴리오가 휘발될 것으로 예상해야 합니다. 입찰은 1~3주 이내에 자동으로 조정됩니다.

   포트폴리오에 대한 자세한 내용은 Search, Social 및 Commerce 내에서 사용할 수 있는 최적화 안내서를 참조하십시오.<!-- verify convention for referencing Optimization Guide here -->

1. (광고주에 대한 새로운 전환이 추적되는 경우) [보고서, 캠페인 관리 보기 및 포트폴리오 목표에 전환을 사용할 수 있도록 설정](/help/search-social-commerce/admin/conversion-metrics/conversion-metric-about.md)합니다.

1. 각 캠페인에 대해 검색, 소셜 및 Commerce이 광고 네트워크에서 클릭 및 비용 데이터를 수신하는지 확인하고 검색, 소셜 및 Commerce에 표시된 수익 데이터를 광고주의 수익 데이터로 확인합니다.

1. (선택 사항) 예약된 보고서의 보고서 템플릿, 스프레드시트 피드 및 FTP 게재를 설정하여 보고를 자동화합니다.

   자세한 내용은 &quot;보고서&quot; 장을 참조하십시오.

>[!MORELIKETHIS]
>
>* [검색, 소셜 및 Commerce의 캠페인 관리 정보](campaign-management-about.md)
>* [광고 네트워크 캠페인의 성능 모니터링 및 관리](monitor-performance-campaigns.md)
>* [검색, 소셜 및 Commerce의 Google 광고 전환 데이터](google-conversion-data.md)
>* [지원되는 인벤토리](/help/search-social-commerce/introduction/supported-inventory.md)
