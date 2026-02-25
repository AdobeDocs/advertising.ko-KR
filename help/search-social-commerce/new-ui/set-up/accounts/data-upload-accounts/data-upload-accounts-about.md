---
title: null
description: null
source-git-commit: f2b29c2f3a38cadc31a9b3110aa82feadd62e5cc
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# 보고 및 시뮬레이션을 위한 계정 데이터 업로드 기본 정보

<!-- Move all related files into one page? -->

검색, 소셜 및 Commerce에서 API 지원을 제공하지 않는 온라인 광고 네트워크를 사용하는 경우 캠페인 컨텐츠 및 오프라인 비용을 업로드하고, 보고 및 성능 시뮬레이션을 위해 계정에 대한 클릭 및 전환 데이터를 사용할 수 있습니다. [[!DNL Adobe Analytics for Advertising] 통합](/help/integrations/analytics/overview.md)을 사용하는 광고주는 Adobe Analytics 내에서 계정에 대한 데이터를 볼 수도 있습니다.

이 기능은 표준 3계층 캠페인 구조(캠페인, 광고 그룹 또는 광고 세트, 입찰 단위(광고 또는 키워드)를 따르는 광고 네트워크에 사용할 수 있습니다. Adobe DSP의 경우 이 기능은 패키지 및 패키지에 할당된 배치에 사용할 수 있지만 캠페인이나 배치 수준 게재 간격이 있는 배치에는 사용할 수 없습니다.

<!-- But what if you want to use something else? Is that possible currently? --> 네트워크에 대한 기본 지원을 사용할 수 있습니다.

<!-- * Adobe Demand Side Platform (Advertising DSP) [Is any data upload required, or just an initial setup of an S3 bucket and/or something else, and then DSP sends the data automatically? If so, then I may need to reframe this whole chapter accordingly.] -->
<!-- * [!DNL Reddit Ads] -->

* [!DNL Apple Search Ads]
* [!DNL LinkedIn Ads]
* [!DNL TikTok Ads]

이 기능에서는 검색, 소셜 및 Commerce 클릭 추적과 Adobe Advertising 전환 추적이 지원되지 않습니다.

## 검색, 소셜 및 Commerce에서 사용할 수 있는 기능

* 추적 및 보고:

   * 캠페인 관리 보기 내에서 입찰 단위 수준까지 읽기 전용 캠페인 구성 요소.

   * 캠페인 관리 보기 및 사용자 지정 보고서 내에서 광고 그룹 수준 <!-- verify the entity level -->까지 성능 데이터를 제공합니다. [!DNL Adobe Analytics for Advertising]을(를) 사용하는 광고주는 광고주용으로 지정된 Adobe Analytics 보고서 세트 내에서 광고 그룹 수준 <!-- verify the entity level -->까지 성과 데이터를 추가로 가져옵니다.&lt;!— 비용, 클릭, 노출, 매출 등 데이터 유형이 제한되어 있는지 확인합니다. —>

* 포트폴리오에 캠페인을 추가할 때의 성능 시뮬레이션.<!-- How does this even work? Do they need to be in standard or hybrid portfolios, with active or optimized status, and can you mix these campaigns with API-synced campaigns? If so, do we just ignore these campaigns and optimize the others? -->

  Search, Social 및 Commerce은 포트폴리오 내에서 이러한 유형의 캠페인에 대해 아무것도 최적화하지 않으며 입찰도 진행하지 않습니다.

## 오프라인 계정을 설정하는 워크플로우

<!-- subtitle wording? -->

1. [더미 계정 레코드를 설정합니다](/help/search-social-commerce/new-ui/set-up/accounts/data-upload-accounts/data-upload-account-manage.md).

1. 캠페인, 광고 그룹 및 광고에 대한 일 수준의 상태를 포함하여 단일 계정 <!--  in what file format? -->에 대한 데이터 파일을 만듭니다.

데이터는 광고 네트워크에 대한 데이터 요구 사항을 준수해야 하므로 각 엔티티의 데이터 필드는 광고 네트워크에 따라 다를 수 있습니다.

1. <!-- For all ad networks (excluding DSP), -->다음 방법 중 하나로 단일 계정에 대한 초기 데이터를 업로드합니다.

* 장치 또는 네트워크에서 수동으로 파일을 업로드합니다.

* [!DNL Amazon Web Services]&#x200B;(AWS) [!DNL Simple Storage Service]&#x200B;([!DNL S3]) 버킷의 검색, 소셜 및 Commerce 할당 폴더에 데이터를 업로드합니다.

  >[!PREREQUISITES]
  >
  >* Adobe 계정 팀에 문의하여 검색, 소셜 및 Commerce 광고주 계정에 대한 계정 데이터 업로드를 활성화하십시오. 팀은 [!DNL S3] 버킷에 조직별 폴더를 쉽게 만들 수 있으며, 작업이 완료되면 알려 줍니다.<!-- Add more context about the bucket we'll use here or in the intro. Do we have one bucket (potentially with multiple folders) per client, or do we share them (if so, do we need to state how in docs? -->
  >* 계정의 [!DNL S3] 클라우드 저장소 경로, 액세스 키 ID 및 비밀 액세스 키를 검색합니다. 조직의 모든 데이터 업로드 <!-- naming convention?--> 계정에 대해 동일한 액세스 키 ID 및 비밀 액세스 키가 사용됩니다.

1. 매일 새 데이터 파일을 계속 업로드합니다.

1. 30일 동안 데이터를 업로드한 후에는 선택적으로 <!--what type? how should we refer to them? --> 포트폴리오에 캠페인을 추가하고 시뮬레이션을 생성할 수 있습니다.

각 데이터 업로드의 로그를 [보고](upload-log.md)하여 상태를 확인할 수 있습니다. 또한 업로드를 시작했지만 업로드가 완전히 성공하지 못한 경우 알림 설정에 따라 [알림 센터](/help/search-social-commerce/notifications/notification-about.md)를 통해 오류 알림을 받습니다.

<!-- Data validation, and any troubleshooting? -->

>[!MORELIKETHIS]
>
>* [보고 및 시뮬레이션을 위한 계정 데이터 업로드 정보](data-upload-accounts-about.md)
>* [계정 데이터를  [!DNL Amazon] [!DNL S3] 버킷에 업로드](upload-data-from-s3-bucket.md)
>* [계정 데이터를 수동으로 업로드](upload-data-manually.md)
>* [업로드된 계정 데이터 파일 로그 보기](upload-log.md)
>* [데이터 업로드를 위한 광고 네트워크 계정 관리](/help/search-social-commerce/campaign-management/accounts/data-upload-account-manage.md)
