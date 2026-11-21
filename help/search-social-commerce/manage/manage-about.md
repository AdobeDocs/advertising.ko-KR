---
title: 캠페인 및 포트폴리오 관리 기본 정보
description: 광고 네트워크 계정, 캠페인, 추적 및 포트폴리오 최적화가 함께 작동하는 방법과 성능을 모니터링하고 개선하는 방법을 알아봅니다.
feature: Search Campaign Management, Search Portfolios
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: aed5e38a-3e62-42fa-8d16-cd080729b2a0
    internal-label: Search, Social, & Commerce
  - id: 76ac9ff6-5d89-5acb-bc0b-875761bb3320
    internal-label: Search Campaign Management
  - id: 893a7eac-45bd-56c2-a120-18db6d297dcc
    internal-label: Search Portfolios
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
    internal-label: Optimization
source-git-commit: 76a8d8b448441e4d7380ebc4f007aa8b5a2ab5f5
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 0%
---
# 캠페인 및 포트폴리오 관리 기본 정보

*Beta 기능*

Search, Social 및 Commerce은 캠페인 관리, 성과 보고 및 포트폴리오 최적화를 하나의 인터페이스로 가져옵니다. 광고 네트워크 및 캠페인 유형에 따라 캠페인 데이터를 동기화하고, 캠페인 구성 요소를 만들고 편집하고, 전환을 추적하고, 입찰, 예산 또는 입찰 전략 타겟을 최적화할 수 있습니다. 각 광고 네트워크에 사용할 수 있는 기능은 [지원되는 인벤토리](/help/search-social-commerce/introduction/supported-inventory.md)를 참조하십시오.

[!UICONTROL Manage] 메뉴를 통해 계정, 캠페인, 광고 그룹, 광고, 키워드, 제품 그룹 및 포트폴리오에 액세스할 수 있습니다. 사용 권한에 따라 사용 가능한 보기 및 작업이 결정됩니다. 전체 메뉴 구성에 대해서는 &quot;[사용자 인터페이스를 구성하는 방법](/help/search-social-commerce/getting-started/user-interface.md)&quot;을 참조하십시오.

## 계정, 캠페인 및 포트폴리오 결합 방식

* **광고 네트워크 계정** 광고주의 데이터를 검색, 소셜 및 Commerce에 연결합니다. [계정 유형](/help/search-social-commerce/manage/accounts/ad-network-account-about.md)에는 API 연결을 통해 동기화된 계정, 데이터를 업로드한 계정 및 템플릿 기반 추적 전용 계정이 포함됩니다. 계정 유형은 데이터를 동기화할지, 캠페인을 관리할지 또는 포트폴리오 최적화를 사용할지 여부를 결정합니다.

* **캠페인**&#x200B;에는 광고를 게재하는 데 사용되는 광고 및 기타 구성 요소가 포함되어 있습니다. 지원되는 캠페인 유형의 경우 [!UICONTROL Manage] 보기에서 [캠페인과 해당 구성 요소를 만들고 관리](/help/search-social-commerce/manage/campaigns/campaign-manage.md)할 수 있습니다. 지원되는 대량 작업에 [일괄 시트](/help/search-social-commerce/set-up/bulksheets/about.md)를 사용할 수도 있습니다.

* **포트폴리오** 그룹 적격 캠페인을 통해 일반적인 비즈니스 목표 및 예산 또는 성과 목표를 달성하도록 최적화합니다. 캠페인은 하나의 포트폴리오에만 속할 수 있으며 포트폴리오의 모든 캠페인은 동일한 통화를 사용해야 합니다. &quot;[포트폴리오 정보](/help/search-social-commerce/manage/portfolios/portfolio-about.md)&quot;를 참조하세요.

Portfolio 할당은 선택 사항입니다. 포트폴리오에 할당하지 않고도 캠페인을 추적하고 보고할 수 있습니다. 모든 광고 네트워크, 캠페인 유형 또는 입찰 전략이 포트폴리오 최적화를 지원하는 것은 아닙니다.

## 캠페인 데이터 동기화

API를 통해 연결된 계정의 경우 검색, 소셜 및 Commerce은 광고 네트워크에서 지원되는 캠페인 구조 및 성능 데이터를 검색합니다. 검색, 소셜 및 Commerce에서 지원되는 캠페인 구성 요소에 대한 변경 사항이 광고 네트워크로 전송됩니다.

필요한 경우 [수동 동기화를 요청](/help/search-social-commerce/manage/accounts/api-accounts/sync-api-accounts.md)할 수 있습니다. 계정이 동기화를 중지하는 경우 [인증 및 액세스 상태](/help/search-social-commerce/manage/accounts/api-accounts/api-account-manage.md#authentication-status)를 검토하십시오.

데이터 업로드 계정 및 추적 전용 계정은 광고 네트워크와 동기화되지 않습니다. [계정 유형](/help/search-social-commerce/manage/accounts/ad-network-account-about.md)에 대한 워크플로를 따라 캠페인 및 성능 데이터를 제공하십시오.

## 추적 및 최적화 설정

[추적](/help/search-social-commerce/tracking/tracking-about.md)은(는) 캠페인 활동을 비즈니스에 중요한 전환에 연결합니다. 구현에 따라 전환 데이터가 Adobe Advertising 태그, Adobe Analytics 통합, 광고 네트워크 추적 또는 데이터 피드에서 제공될 수 있습니다. 구현에 필요한 클릭 추적 및 전환 추적을 구성하고 최적화에 사용하기 전에 데이터의 유효성을 검사합니다.

[!UICONTROL Goals] > [!UICONTROL Conversions]에서 [광고주에 대해 추적된 전환 지표를 검토하고 해당 가시성을 제어할 수 있습니다](/help/search-social-commerce/goals/conversions/conversion-metrics-manage.md). [목표](/help/search-social-commerce/goals/objectives/objective-about.md)에서 적절한 지표를 사용하십시오.

포트폴리오 최적화를 사용하려면 [포트폴리오를 만들고](/help/search-social-commerce/manage/portfolios/portfolio-create.md), 목표 및 적격 캠페인을 할당하고 지출 및 최적화 설정을 구성하십시오. 활성 포트폴리오는 성능 데이터를 수집하고 모델링합니다. 데이터 및 설정이 준비되면 [포트폴리오 상태를 최적화됨으로 변경](/help/search-social-commerce/manage/portfolios/portfolio-change-status.md)하여 최적화를 시작합니다. 수행되는 작업은 포트폴리오 유형과 [캠페인 입찰 전략](/help/search-social-commerce/manage/portfolios/portfolio-about.md#optimization-by-bid-strategy)에 따라 다릅니다.

자세한 설정 순서는 &quot;[광고 네트워크 계정 및 캠페인 설정](/help/search-social-commerce/getting-started/campaign-implementation-overview.md)&quot;을 참조하십시오.

## 캠페인 및 포트폴리오 성과 모니터링 {#monitor-performance}

계정 팀, 에이전시 또는 광고주는 서비스 계약 조건에 따라 성과를 모니터링하고 조정을 수행합니다. 일상적으로:

* [!UICONTROL Manage] 보기에서 캠페인 및 계정 성과를 검토하십시오. [열, 필터 및 날짜 범위를 사용자 지정](/help/search-social-commerce/common-tasks/data-views/data-views-about.md)하여 해당 지표와 엔터티에 집중하세요.

* [!UICONTROL Dashboard] > [!UICONTROL Overview]을(를) 사용하여 [포트폴리오 트렌드 및 성능 변화를 모니터링](/help/search-social-commerce/dashboard/dashboard-overview.md)합니다.

* 조사가 필요한 조건에 대해서는 [사용자 지정 경고](/help/search-social-commerce/common-tasks/alerts-manage.md)를 검토하십시오.

* 캠페인, 키워드, 광고 및 포트폴리오 성능에 대한 [보고서를 생성](/help/search-social-commerce/reports/management/report-manage.md)합니다. 포트폴리오의 경우 실제 성능 및 모델 정확도를 포함하여 [성능 세부 정보를 검토](/help/search-social-commerce/manage/portfolios/portfolio-details.md)하십시오.

* 사용 가능한 경우 [시뮬레이션](/help/search-social-commerce/plan/simulations/simulation-about.md)을 사용하여 다양한 지출 수준의 예측된 효과를 평가하십시오.

* 보고된 전환과 소스 데이터 간의 차이점을 조사합니다. 관련 링크에서 [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 전환 데이터에 대한 지침을 참조하십시오.

## 캠페인 및 포트폴리오 조정

성과 및 비즈니스 목표 변경 사항에 따라 다음을 수행해야 할 수 있습니다.

* 캠페인 설정을 편집하거나, 캠페인 구성 요소를 만들거나 일시 중지하거나, 키워드 세트를 세분화하거나, 다른 광고를 테스트할 수 있습니다. 사용 가능한 작업은 광고 네트워크 및 캠페인 유형에 따라 다릅니다.

* 관련 관리 보기 및 보고서를 사용하여 지리적, 대상 및 배치 타겟팅을 검토합니다.

* 다른 포트폴리오로 캠페인을 최적화해야 하는 경우 [캠페인 할당을 변경](/help/search-social-commerce/manage/campaigns/campaign-manage.md#campaign-portfolio). 다른 포트폴리오에 캠페인을 할당하면 이전 포트폴리오에서 캠페인이 제거됩니다.

* 제품 프로필에서 허용하는 대로 목표, 지출 전략, 제한 또는 최적화 컨트롤을 포함하여 [포트폴리오 설정을 편집](/help/search-social-commerce/manage/portfolios/portfolio-edit.md)합니다.

* 성능 변경을 조사할 때 [변경 기록](/help/search-social-commerce/reports/history-logs.md)을 검토합니다.

>[!MORELIKETHIS]
>
>* [광고 네트워크 계정 및 캠페인 설정](/help/search-social-commerce/getting-started/campaign-implementation-overview.md)
>* [지원되는 인벤토리](/help/search-social-commerce/introduction/supported-inventory.md)
>* [[!DNL Google Ads] 검색, 소셜 및 Commerce의 전환 데이터](/help/search-social-commerce/tracking/google-conversion-data.md)
>* [[!DNL Microsoft Advertising] 검색, 소셜 및 Commerce의 전환 데이터](/help/search-social-commerce/tracking/microsoft-conversion-data.md)
