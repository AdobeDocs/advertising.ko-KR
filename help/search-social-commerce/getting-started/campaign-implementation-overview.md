---
title: 광고 네트워크 계정 및 캠페인 설정
description: 광고 네트워크 연결, 캠페인, 추적, 전환 지표 및 선택적 포트폴리오 최적화에 대한 설정 워크플로를 따르십시오.
feature: Search Getting Started, Search Campaign Management
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: aed5e38a-3e62-42fa-8d16-cd080729b2a0
    internal-label: Search, Social, & Commerce
  - id: 54967645-9f46-5896-8af7-b943b426aadf
    internal-label: Search Getting Started
  - id: 76ac9ff6-5d89-5acb-bc0b-875761bb3320
    internal-label: Search Campaign Management
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
    internal-label: Optimization
source-git-commit: 76a8d8b448441e4d7380ebc4f007aa8b5a2ab5f5
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%
---
# 광고 네트워크 계정 및 캠페인 설정

*Beta 기능*

[!DNL Adobe] 및 에이전시가 사용자와 협력하여 광고 네트워크 계정을 연결하고, 캠페인을 준비하고, 추적을 구성하고, 성능 데이터를 확인합니다. 검색, 소셜 및 Commerce에서 적격 캠페인을 최적화하려면 워크플로에 포트폴리오 설정도 포함됩니다.

이 체크리스트는 광범위한 [구현 워크플로](implemention-overview.md)에 대한 계정 및 캠페인 세부 정보를 제공합니다. 수행할 수 있는 작업은 사용 권한과 각 광고 네트워크 및 캠페인 유형에 대해 지원되는 [기능에 따라 다릅니다](/help/search-social-commerce/introduction/supported-inventory.md).

## 워크플로우 설정

1. **액세스 및 계정 요구 사항을 확인합니다.**

   관리자와 함께 적절한 광고주에 대한 액세스 권한과 작업에 필요한 권한을 확인합니다. &quot;[검색, 소셜 및 Commerce에 대한 사용자 관리](/help/search-social-commerce/user-administration.md)&quot;를 참조하십시오.

   필요한 경우 광고 네트워크의 웹 사이트에서 실제 광고 네트워크 계정을 만듭니다. 검색, 소셜 및 Commerce에서 계정 레코드를 만들어도 광고 네트워크에서는 계정이 만들어지지 않습니다.

1. **각 광고 네트워크 계정을 연결하거나 등록합니다.**

   [!UICONTROL Manage] > [!UICONTROL Accounts]에서 [계정 유형](/help/search-social-commerce/manage/accounts/ad-network-account-about.md)에 대한 워크플로를 사용합니다.

   * **API 연결:** [계정 세부 정보를 만들고](/help/search-social-commerce/manage/accounts/api-accounts/api-account-manage.md#create-account), 네트워크별 인증을 완료하고 추적 옵션을 구성하고 계정을 사용하도록 설정합니다. [인증 및 액세스 상태](/help/search-social-commerce/manage/accounts/api-accounts/api-account-manage.md#authentication-status)를 확인하세요. 인증에 성공했다고 해서 필요한 모든 권한이 부여된 것은 아닙니다.

   * **데이터 업로드:** [계정 세부 정보를 만들고 캠페인 및 성과 데이터를 업로드](/help/search-social-commerce/manage/accounts/data-upload-accounts/data-upload-account-manage.md). 이러한 계정은 광고 네트워크와 동기화되지 않거나 포트폴리오 최적화를 지원합니다.

   * **[!DNL Naver]추적 전용:** [추적 전용 계정 워크플로](/help/search-social-commerce/manage/accounts/template-account-manage.md)를 따르십시오. 일괄 시트를 사용하여 추적 URL을 생성하고 광고 네트워크의 편집기에 적용합니다. 계정은 포트폴리오 최적화를 동기화하거나 지원하지 않습니다.

1. **캠페인 구조를 검토하거나 만듭니다.**

   API 연결 계정의 경우 동기화된 캠페인 및 해당 구성 요소를 검토하십시오. 필요한 경우 [수동 동기화를 요청](/help/search-social-commerce/manage/accounts/api-accounts/sync-api-accounts.md)합니다.

   지원되는 캠페인 유형의 경우 [!UICONTROL Manage] > [!UICONTROL Campaigns]을(를) 사용하여 [캠페인을 만들거나 편집](/help/search-social-commerce/manage/campaigns/campaign-manage.md)하십시오. 필요한 [광고 그룹](/help/search-social-commerce/manage/ad-groups/ad-group-manage.md), [광고](/help/search-social-commerce/manage/ads/ad-manage.md) 및 기타 지원되는 구성 요소를 만듭니다. 지원되는 대량 작업에 [일괄 시트](/help/search-social-commerce/set-up/bulksheets/about.md)를 사용할 수도 있습니다.

   캠페인을 활성화하기 전에 필요한 네트워크별 설정을 완료합니다. 광고 네트워크의 자체 인터페이스에서 지원되지 않는 구성 요소를 관리합니다.

1. **시작 전 추적을 구성하고 유효성을 검사합니다.**

   구현과 일치하는 [전환 추적 메서드](/help/search-social-commerce/tracking/conversion-tracking-about.md)를 선택하십시오. 필요한 경우 [클릭 추적 URL을 생성하고 적용](/help/search-social-commerce/tracking/click-tracking-ways-to-generate.md) 및 [전환 추적 태그를 생성](/help/search-social-commerce/goals/conversions/conversion-tag-generate.md)합니다.

   필요한 [통합](/help/integrations/home.md) 또는 [전환 피드](/help/search-social-commerce/tracking/tracking-about.md)를 구성하고 전환이 예상대로 귀속될 수 있는지 확인하십시오. 추적 전용 캠페인의 경우 광고 네트워크 편집기에서 생성된 추적 URL을 적용합니다.

1. **전환 지표를 검토합니다.**

   [!UICONTROL Goals] > [!UICONTROL Conversions]에서 [추적된 지표를 검토하고 관리 보기, 보고서 및 목표에 필요한 지표를 표시](/help/search-social-commerce/goals/conversions/conversion-metrics-manage.md#conversion-metrics-change-available)합니다. 필요한 경우 지표를 구분하기 위해 표시 이름을 변경합니다.

1. **(선택 사항) 포트폴리오 최적화를 준비합니다.**

   캠페인과 입찰 전략이 [포트폴리오 최적화에 적격한지 확인](/help/search-social-commerce/manage/portfolios/portfolio-about.md#optimization-by-bid-strategy).

   적절한 전환 지표를 사용하는 [목표를 만들거나 선택](/help/search-social-commerce/goals/objectives/objective-about.md)합니다. [!UICONTROL Manage] > [!UICONTROL Portfolios]에서 필요한 목표, 지출 전략 및 최적화 설정을 사용하여 [포트폴리오를 만들거나](/help/search-social-commerce/manage/portfolios/portfolio-create.md) [기존 포트폴리오를 편집](/help/search-social-commerce/manage/portfolios/portfolio-edit.md)하십시오.

   [포트폴리오에 캠페인을 할당](/help/search-social-commerce/manage/campaigns/campaign-manage.md#campaign-portfolio). 각 캠페인은 하나의 포트폴리오에만 속할 수 있으며 포트폴리오의 모든 캠페인은 동일한 통화를 사용해야 합니다.

1. **캠페인 데이터의 유효성을 검사하고 성과 기준을 설정합니다.**

   각 캠페인에 비용, 클릭 및 전환 데이터를 사용할 수 있는지 확인합니다. 적용 가능한 경우 전환 데이터를 [!DNL Google Ads] 및 [!DNL Microsoft Advertising]을(를) 포함한 적절한 소스와 비교합니다. 보고서를 비교할 때 일관된 날짜 범위 및 속성 설정을 사용합니다.

   새 포트폴리오의 경우 데이터를 수집하고 모델링하려면 [활성화](/help/search-social-commerce/manage/portfolios/portfolio-change-status.md)하십시오. 최적화를 활성화하기 전에 데이터 및 포트폴리오 설정의 유효성을 검사하십시오.

1. **(선택 사항) 시작 포트폴리오 최적화.**

   포트폴리오가 준비되면 [상태를 최적화됨](/help/search-social-commerce/manage/portfolios/portfolio-change-status.md)(으)로 변경하고 필수 구성 요소와 확인 메시지를 검토하십시오. 그런 다음 검색, 소셜 및 Commerce은 해당 설정 및 지원되는 캠페인 입찰 전략에 따라 포트폴리오를 최적화합니다.

1. **진행 중인 모니터링 및 보고를 구성합니다.**

   [데이터 보기를 사용자 지정](/help/search-social-commerce/common-tasks/data-views/data-views-about.md), [사용자 지정 경고를 설정](/help/search-social-commerce/common-tasks/alerts-manage.md) 및 [예약된 보고서를 생성](/help/search-social-commerce/reports/management/report-manage.md)합니다. 필요한 경우 [보고서 템플릿](/help/search-social-commerce/reports/report-templates-manage.md) 및 [스프레드시트 피드](/help/search-social-commerce/reports/spreadsheet-feeds-manage.md)를 사용하여 보고를 자동화합니다.

   시작 후 [캠페인 및 포트폴리오 모니터링 및 조정](/help/search-social-commerce/manage/manage-about.md#monitor-performance)을 계속합니다.

>[!MORELIKETHIS]
>
>* [Search, Social 및 Commerce 구현 개요](implemention-overview.md)
>* [캠페인 및 포트폴리오 관리 정보](/help/search-social-commerce/manage/manage-about.md)
>* [[!DNL Google Ads] 검색, 소셜 및 Commerce의 전환 데이터](/help/search-social-commerce/tracking/google-conversion-data.md)
>* [[!DNL Microsoft Advertising] 검색, 소셜 및 Commerce의 전환 데이터](/help/search-social-commerce/tracking/microsoft-conversion-data.md)
