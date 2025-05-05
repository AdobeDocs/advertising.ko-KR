---
title: ' [!DNL Google Ads] 동적 검색 광고 구현'
description: ' [!DNL Google Ads] 동적 검색 광고 설정 워크플로에 대해 알아봅니다.'
exl-id: 69e5069f-3f82-4ee3-841a-0c1292677223
feature: Search Campaign Management
source-git-commit: 283fced2b3faa64b6383b6ab2a41696cba0da06f
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 0%

---

# [!DNL Google Ads] 동적 검색 광고 구현

광고 수준 또는 키워드 및 광고 수준 추적만 포함하는 *[!DNL Google Ads]개의 검색 전용 캠페인*

동적 검색 광고는 키워드 대신 웹 사이트의 콘텐츠를 사용하여 광고를 표시할 시기를 결정합니다. 광고 그룹에 대해 별도의 동적 검색 타겟을 설정하거나 웹 사이트 콘텐츠를 사용하여 광고를 타겟팅하는 캠페인 수준 설정을 선택하여 콘텐츠가 동적 검색 광고를 타겟팅하는 데 사용되는 웹 사이트의 페이지를 정의할 수 있습니다.

개별적으로 또는 일괄 시트를 사용하여 동적 검색 광고를 설정할 수 있습니다. 다음 지침에는 개별 엔티티 만들기에 대한 링크가 포함되어 있습니다.

## [!DNL Google Ads]개의 동적 검색 광고를 설정하는 단계

1. 동적 검색 광고에 대한 [캠페인을 만들기](/help/search-social-commerce/campaign-management/campaigns/campaign-manage.md):

   1. 처음에는 캠페인 예산을 일일 검색 캠페인 지출의 10%로 설정합니다.

      광고가 가치를 입증하면 나중에 예산을 늘릴 수 있습니다.

   1. (웹 사이트의 콘텐츠를 기반으로 [!DNL Google Ads]에 동적 검색 광고를 표시하려면) 캠페인 설정의 [!UICONTROL DSA Options] 섹션에서 루트 도메인 및 도메인 언어를 지정합니다.

      >[!NOTE]
      >
      >타겟팅할 [!DNL Google Ads] 유기 검색 인덱스로 도메인을 인덱싱해야 합니다. 또한 도메인에 여러 언어로 된 페이지가 포함되어 있고 이러한 페이지를 모두 타겟팅하려면 각 언어에 대해 별도의 캠페인을 만듭니다.

      웹 사이트 도메인을 사용하여 광고를 타깃팅하지 않는 경우 각 광고 그룹에 대해 동적 검색 타겟을 만듭니다(4단계 참조). 대상을 [개별적으로](/help/search-social-commerce/campaign-management/campaigns/dynamic-search-target-manage.md)만들거나 [일괄 시트](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-about.md)를 사용할 수 있습니다.

   1. 캠페인이 검색 채널을 타겟팅하고 표시 네트워크가 아닌 [!DNL Google Ads] 검색 네트워크만 타겟팅하는지 확인하십시오. 이러한 설정은 [!UICONTROL Networks and Devices] 탭에서 사용할 수 있습니다.

   1. (선택 사항) [!UICONTROL Negatives] 탭에서 키워드를 제외합니다.

   1. (선택 사항) 계정 수준 추적 템플릿을 무시하지만 더 낮은 수준에서 재정의할 수 있는 캠페인 수준 추적 템플릿을 구성합니다.

      (서버측 추적이 없는 Adobe Analytics을 사용하는 광고주) 검색, 소셜 및 Commerce에서 Analytics로의 역방향 피드에 대한 추적을 포함하려면 AMO ID 추적 코드를 계정 수준 추가 매개 변수에 추가하고, 이렇게 하면 코드를 최종 URL에 추가합니다. &quot; [!DNL Analytics][&#128279;](/help/integrations/analytics/ids.md)에서 사용하는 Adobe Advertising ID&quot;를 참조하십시오.&quot;

1. 다음 단계를 포함하여 캠페인 내에서 [광고 그룹을 만듭니다](/help/search-social-commerce/campaign-management/campaigns/ad-group-manage.md).

   1. [!UICONTROL Ad Group Type]을(를) **[!UICONTROL Search Dynamic].**(으)로 설정합니다.

   1. 모든 광고에 대한 기본 입찰을 설정합니다.

      구성 시 개별 동적 검색 타겟에 대한 기본 입찰을 재정의할 수 있습니다.

   1. (선택 사항) 상위 수준의 모든 추적 템플릿을 무시하지만 광고 수준에서 재정의할 수 있는 광고 그룹 수준 추적 템플릿을 구성합니다.

      캠페인 수준에서 Adobe Analytics 추적을 추가하고 광고 그룹에 포함하려면 여기에 추가하십시오. 1e단계를 참조하십시오.

1. 광고 그룹 내에서 [각 동적 검색 광고를 만듭니다](/help/search-social-commerce/campaign-management/campaigns/ad-manage.md).

   [!DNL Google Ads]은(는) 각 광고의 헤드라인, 표시 URL 및 랜딩 페이지 URL을 동적으로 생성합니다. 더 높은 수준의 추적 템플릿을 무시하는 광고 수준 추적 템플릿에 리디렉션 및 추적을 선택적으로 추가할 수 있습니다.
더 높은 수준의 Adobe Analytics 추적을 광고 수준 추적으로 재정의하려면 여기에 추가하십시오. 1e단계 및 2c단계를 참조하십시오.

1. (캠페인 설정의 DSA 옵션 섹션에 루트 도메인과 도메인 언어를 포함하지 않을 때 필요하며, 그렇지 않으면 선택 사항) 광고 그룹에 대해 [동적 검색 대상](/help/search-social-commerce/campaign-management/campaigns/dynamic-search-target-manage.md)을 만듭니다. 광고 그룹 수준 입찰을 타겟 수준 입찰로 선택적으로 대체할 수 있습니다.

   타겟은 광고 네트워크가 웹 사이트에 있는 페이지의 전체 또는 하위 집합을 사용하여 동적 검색 광고를 타깃팅할지 여부를 정의합니다. 성능을 가장 잘 추적하려면 동적 검색 대상당 하나의 광고 그룹으로 캠페인을 구성하고 모든 기준을 타깃팅하는 광고 그룹을 포함하십시오.

1. 필요에 따라 [캠페인 설정을 편집](/help/search-social-commerce/campaign-management/campaigns/campaign-manage.md)하여 캠페인 예산을 조정하고 추가 키워드를 캠페인에서 제외하여 트래픽을 세분화합니다.
