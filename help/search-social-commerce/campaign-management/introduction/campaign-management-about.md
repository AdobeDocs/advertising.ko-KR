---
title: 검색, 소셜 및 Commerce의 캠페인 관리 기본 정보
description: 검색, 소셜 및 Commerce의 캠페인 관리 기능에 대해 알아봅니다.
exl-id: 19e36e73-fcb6-4ff3-980b-fc05042725fd
feature: Search Campaign Management
source-git-commit: e16bc62127a708de8f4deb1eddfa53a14405cbc2
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 0%

---

# 검색, 소셜 및 Commerce의 캠페인 관리 기본 정보

검색, 소셜 및 Commerce을 사용하면 검색, 표시/컨텐츠, 소셜, 쇼핑, 대상자 및 성과 최대 캠페인을 한 곳에서 추적 및/또는 관리할 수 있습니다. 광고 네트워크 및 캠페인 유형에 따라 사용 가능한 기능에는 광고 네트워크와의 동기화, 기능 생성 및 편집, 추적 및 전환 속성, 보고, 입찰 및 예산 최적화가 포함될 수 있습니다. 각 광고 네트워크에서 사용할 수 있는 기능에 대한 자세한 내용은 &quot;[지원되는 인벤토리](/help/search-social-commerce/introduction/supported-inventory.md)&quot;를 참조하십시오.

[!UICONTROL Campaigns] 보기에서 캠페인 데이터를 추가하고 편집하면 검색, 소셜 및 Commerce이 데이터 변경 내용을 광고 네트워크에 즉시 푸시합니다. 또한 검색, 소셜 및 Commerce은 캠페인 구조 데이터를 가져오고 매일 한 번(또는 새 캠페인이 감지되면 더 자주) 동기화된 광고 네트워크 계정에서 클릭 데이터를 요청대로 요청 시 가져옵니다.

## 광고 네트워크 계정에 대한 액세스 설정

광고주의 광고 네트워크 계정에서 광고 성과를 추적하고 잠재적으로 광고를 입찰하기 위해 Adobe 계정 팀 [검색, 소셜 및 Commerce에서 해당 계정 레코드를 만듭니다](/help/search-social-commerce/campaign-management/accounts/ad-network-account-manage.md). 계정 레코드에는 추적 옵션이 포함됩니다.

광고 네트워크의 API를 통해 동기화된 계정의 경우 계정 레코드에는 계정 액세스 자격 증명도 포함됩니다. 계정이 활성화되면 계정 데이터는 광고 네트워크에서 가져옵니다. 그런 다음 기존 계정 데이터를 보고 캠페인 구조 및 광고 데이터를 만들고 편집할 수 있습니다.

## 클릭을 전환에 연결하려면 클릭 추적

Adobe Advertising 전환 추적 서비스를 사용하는 경우 랜딩 페이지 접미사에 검색, 소셜 및 Commerce 클릭 추적 코드, 추적 템플릿 및 광고, 키워드, 배치, 사이트링크 및 제품 목록에 대한 최종/대상 URL을 포함해야 합니다. 캠페인 설정에 &quot;[!UICONTROL EF Redirect]&quot; 및 &quot;[!UICONTROL Auto Upload]&quot;이(가) 포함된 [지원되는 광고 네트워크 및 캠페인 유형](/help/search-social-commerce/introduction/supported-inventory.md)의 경우 레코드를 저장할 때 검색, 소셜 및 Commerce에서 자동으로 리디렉션 및 추적 코드를 추가하므로 수동으로 추가할 필요가 없습니다. 그렇지 않으면 코드를 추적 템플릿 또는 최종 URL에 수동으로 추가해야 합니다.

추적에 대한 자세한 내용은 &quot;추적&quot; 장을 참조하십시오.

## 입찰 및 예산 관리 자동화

[지원되는 광고 네트워크 및 캠페인 유형](/help/search-social-commerce/introduction/supported-inventory.md)의 경우 캠페인을 포트폴리오로 그룹화할 수 있습니다. 각 포트폴리오는 특정 비즈니스 목표와 특정 예산 또는 성과 목표를 가지고 있습니다. 표준 포트폴리오에서 검색, 소셜 및 Commerce은 CPC 키워드 입찰과 캠페인 예산을 최적화합니다. 하이브리드 포트폴리오에는 검색, 소셜 및 Commerce의 최적화 기술과 광고 네트워크가 결합되어 있습니다.

사용 가능한 포트폴리오 옵션 및 포트폴리오 설정 방법에 대한 자세한 내용은 Search, Social 및 Commerce 내에서 사용할 수 있는 &quot;Portfolio&quot;에 대한 최적화 안내서 장을 참조하십시오.<!-- verify convention for referencing Optimization Guide here -->

## 캠페인 관리 보기

캠페인 관리 보기를 통해 검색 계정을 모니터링하고 관리할 수 있습니다. 다음 보기를 사용할 수 있습니다.

* **[!UICONTROL Campaigns]** — [!UICONTROL Campaigns] 보기에는 연결된 각 광고 네트워크 계정의 데이터가 표시됩니다. 모든 광고 네트워크 계정 및 개별 계정, 캠페인, 광고 그룹, 키워드, 광고, 쇼핑 제품 그룹, 배치, 자동 타겟(동적 검색 타겟), 대상, 광고 확장 라이브러리 및 관련 계정 엔티티에서 비용, 클릭, 노출 및 매출 데이터를 볼 수 있습니다. [지원되는 광고 네트워크에서 지원되는 캠페인 유형](/help/search-social-commerce/introduction/supported-inventory.md)의 경우 인터페이스에서 개별 캠페인 및 캠페인 구성 요소에 대한 데이터를 직접 만들고 편집할 수 있습니다. 선택적으로 대부분의 하위 보기의 데이터를 스프레드시트 파일로 내보낼 수 있습니다.

  >[!NOTE]
  >
  >[!DNL Google Ads] 동적 검색 광고(DSA), 성능 최대, 스마트 쇼핑 및 [!DNL YouTube] 캠페인에 대한 광고 수준 데이터를 사용할 수 없습니다.

* **[!UICONTROL Products]** — [!UICONTROL Products] 보기에는 동기화된 각 [[!DNL Google] 또는 [!DNL Microsoft] 판매자 센터 계정에 대한 데이터가 표시됩니다](/help/search-social-commerce/campaign-management/accounts/merchant-account-manage.md). 기본 [!UICONTROL Accounts] 하위 보기는 동기화된 모든 계정을 나열합니다. 일부 사용자 유형은 이 보기에서 새 계정을 추가할 수 있습니다. [!UICONTROL Products] 하위 보기는 계정 내의 각 제품을 나열합니다.

* **[!UICONTROL Advanced (ACM)]** — [!DNL Advanced] ([!DNL AMC], 고급 Campaign Management) 보기에서, 사용자가 만든 광고 네트워크별 광고 템플릿과 FTP 위치에 업로드한 [!DNL Google Merchant Center] 계정 또는 인벤토리 데이터 파일의 내용에 따라 인벤토리의 각 항목을 대상으로 하는 [동적 광고 및 키워드](/help/search-social-commerce/campaign-management/inventory-feeds/inventory-feeds-about.md)를 만드는 자동화된 프로세스를 설정할 수 있습니다. 하위 보기는 광고주에 대한 각 피드 템플릿에 대한 세부 정보를 보여주며, 피드 템플릿을 통해 전파되었지만 광고 네트워크에 게시되지 않은 피드에 포함된 각 캠페인, 광고 그룹, 키워드 및 광고를 보여줍니다.

* **[!UICONTROL Bulksheets]** — [!UICONTROL Bulksheets] 보기를 사용하여 [지원되는 광고 네트워크](/help/search-social-commerce/introduction/supported-inventory.md)에서 계정에 대해 원하는 만큼의 데이터를 포함하는 [일괄 시트 파일](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-about.md)을 만든 다음 광고 네트워크에 게시합니다.

* **[!UICONTROL Audiences]** — [보기 [!UICONTROL Audiences]개](/help/search-social-commerce/campaign-management/campaigns/audience-about.md)는 다양한 유형의 사용자 목록에서 생성된 [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 대상을 모두 나열합니다. 기존 Adobe Experience Cloud 대상 및 고객 이메일 목록에서 [!DNL Google Ads]개의 대상을 만들 수 있습니다. [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 광고에 대한 대상 타겟 및 제외를 보고 관리할 수도 있습니다.

* **[!UICONTROL Label Classifications]** — 이 보기를 사용하여 [레이블 분류](/help/search-social-commerce/campaign-management/label-classifications/classification-about.md)를 만들고 삭제할 수 있습니다. 이렇게 하면 레이블을 의미 있는 집합으로 그룹화하는 데 도움이 될 수 있습니다.

>[!MORELIKETHIS]
>
>* [광고 네트워크 계정 및 캠페인 구현 개요](campaign-implemention-overview.md)
>* [광고 네트워크 캠페인의 성능 모니터링 및 관리](monitor-performance-campaigns.md)
>* [검색, 소셜 및 Commerce의 Google 광고 전환 데이터](google-conversion-data.md)
