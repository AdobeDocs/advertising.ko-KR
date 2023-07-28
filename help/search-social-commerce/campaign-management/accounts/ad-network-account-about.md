---
title: 광고 네트워크 계정 기본 정보
description: 검색, 소셜 및 상거래에서 광고 네트워크 계정에 대해 알아봅니다.
exl-id: fca469f1-502c-415a-897d-03b6e6ba34e8
feature: Search Campaign Management
source-git-commit: 052574217d7ddafb8895c74094da5997b5ff83db
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# 광고 네트워크 계정 기본 정보

*에이전시 계정 관리자, Adobe 계정 관리자 및 관리자 사용자 역할만 해당*

Search, Social 및 Commerce는 지원되는 광고 네트워크에서 광고주의 계정을 추적할 수 있습니다. 계정 추적을 활성화하려면 해당 계정 레코드를 만들어야 합니다. 검색, 소셜 및 상거래가 그것과 동기화되는지 또는 광고에서 입찰 및 예산을 최적화하는지 여부에 관계없이 모든 유형의 계정에 대한 계정 세부 정보를 설정해야 합니다.

## API를 통해 동기화된 계정

*[!DNL Baidu], [!DNL Google Ads], [!DNL Microsoft Advertising] (이전 [!DNL Bing Ads]), [!DNL Yahoo! Display Network], [!DNL Yahoo! Japan Ads], 및 [!DNL Yandex] 계정*

검색, 소셜 및 상거래 동기화 (*동기화*&#x200B;광고 성능을 추적, 보고 및 시각화할 수 있도록 지원되는 광고 네트워크 계정 사용) 를 제외한 모든 광고 네트워크 [!DNL Yahoo! Display Network], 검색, 소셜 및 상거래에서 계정에 대한 캠페인을 선택적으로 관리할 수 있습니다. [!DNL Yahoo! Display Network], 캠페인은 읽기 전용입니다. 모든 광고 네트워크의 경우 포트폴리오에 추가하여 관리 계정의 광고에 대한 입찰을 최적화하는 최적화 기능을 허용할 수 있습니다.

계정의 동기화를 활성화하려면 계정 레코드에 계정 액세스 자격 증명이 포함되어 있어야 하며 활성화되어 있어야 합니다(활성).

동기화 중에 검색, 소셜 및 상거래는 검색, 소셜 및 상거래에서 관리되거나 보고되는 대부분의 속성을 포함하여 광고주의 캠페인 구조와 지원되는 캠페인 엔티티를 가져옵니다. 여기에는 클릭 데이터나 검색, 소셜 및 커머스 외부에서 입력한 입찰 및 입찰 수정자가 포함되지 않으며, 이는 별도로 수집됩니다. 검색, 소셜 및 상거래는 하루에 한 번 광고 네트워크 계정과 자동으로 동기화되며, 또한 광고 네트워크 중 하나에서 새 캠페인을 감지할 때마다 동기화됩니다. 또한 검색, 소셜 및 상거래 내에서 수행한 캠페인 데이터에 대한 모든 변경 사항을 광고 네트워크로 즉시 전송합니다. 필요한 경우 선택적으로 수동 동기화를 요청할 수 있습니다.

동기화된 캠페인을 만들고 편집하는 방법에 대한 자세한 내용은 &quot;Campaign Management&quot;의 장을 참조하십시오.

## 추적 전용 계정

*[!DNL Naver]계정*

추적 캠페인을 사용하면 광고 네트워크에서 직접 구매하는 광고의 성과를 추적, 보고 및 시각화할 수 있습니다. Search, Social 및 Commerce는 데이터를 광고 네트워크와 동기화하지 않으며, 계정에 대해 입찰을 진행하지 않으며, 최적화 또는 시뮬레이션을 제공하지 않습니다.

검색, 소셜 및 상거래를 통해 클릭 수에 전환을 지정할 수 있도록 하려면 계정 레코드에서 추적 옵션을 설정하고 계정 레코드를 활성화합니다. 그런 다음 일괄 시트를 사용하여 광고 및 키워드에 대한 추적 URL을 생성하고 내에 추적 URL을 수동으로 추가할 수 있습니다. [!DNL Naver] 광고 관리자.

에 대한 자세한 내용 보기 [!DNL Naver] 추적 전용 캠페인, 참조: &quot;[구현 [!DNL Naver] 추적 전용 계정](/help/search-social-commerce/campaign-management/naver-tracking-only-account-implement.md).&quot;

>[!MORELIKETHIS]
>
>* [광고 네트워크 계정 관리](ad-network-account-manage.md)
>* [머천트 센터 계정 관리](merchant-account-manage.md)
>* [에 대한 s\_kwcid 추적 코드 업데이트 [!DNL Google Ads] account](update-skwcid-google.md)
