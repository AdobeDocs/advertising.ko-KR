---
title: s_kwcid 추적 매개 변수
description: Adobe Analytics과 Adobe Advertising 데이터를 공유하는 데 사용되는 추적 매개 변수에 대해 알아봅니다.
exl-id: 3f739f1c-3cb7-40d0-86ab-cf66afe6a06f
feature: Search Tracking
source-git-commit: 052574217d7ddafb8895c74094da5997b5ff83db
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---

# s_kwcid 추적 매개 변수

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

<!-- Where should this go? It probably belongs in the Analytics integration chapter, but I'll need to fit it in/create context around it/explain more about implementation and how this works.  SPECIFICALLY, I'll need to update the second section that explains when/where to add the code for DSP clients. -->

Adobe Advertising은 다음을 사용하여 Adobe Analytics과 캠페인에 대한 데이터를 공유합니다. `s_kwcid` append 매개 변수 : 광고 채널 및 광고 네트워크별 요소로 구성됩니다. 매개 변수는 다음 방법 중 하나로 추적 URL에 추가됩니다.

* (권장)<!--; the only option for Advertising DSP-->) 서버측 s_kwcid 기능이 구현되었습니다.

  대상 [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 이(가) 있는 계정 [!UICONTROL Auto Upload] 계정 또는 캠페인에 대해 활성화된 설정을 지정하면, 픽셀 서버는 최종 사용자가 광고를 클릭할 때 랜딩 페이지 접미사에 s_kwcid 매개 변수를 자동으로 추가합니다 <!-- click a search ad or views a display ad --> Adobe Advertising 픽셀 사용.

  기타 광고 네트워크의 경우 또는 [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 이(가) 있는 계정 [!UICONTROL Auto Upload] 비활성화로 설정하면 매개 변수를 계정 수준 추가 매개 변수에 수동으로 추가하고 기본 URL에 추가합니다.

* <!-- (Search, Social, & Commerce only) -->서버측 s_kwcid 기능은 구현되지 않으며 s_kwcid 매개 변수를 ( )에 수동으로 추가해야 합니다.[!DNL Google Ads] 및 [!DNL Microsoft Advertising]) 랜딩 페이지 접미사 또는 (기타 광고 네트워크) 계정 수준 추가 매개 변수.

서버측 s_kwcid 기능을 구현하거나 최상의 비즈니스 옵션을 결정하려면 Adobe 계정 팀에 문의하십시오.

## Advertising DSP 광고용 s_kwcid 형식

`s_kwcid=AC!${TM_AD_ID}!${TM_PLACEMENT_ID}`

여기서:

* `AC` 디스플레이 채널을 나타냅니다.

* `{TM_AD_ID}` 는 영숫자 광고 키입니다.

* `{TM_PLACEMENT_ID}` 는 영숫자 배치 키입니다.

## 검색, 소셜 및 상거래 광고용 s_kwcid 형식

매개 변수는 광고 네트워크별로 다르지만, 다음 매개 변수는 모두에게 공통입니다.

* `AL` 검색 채널을 나타냅니다. <!-- what about social/Facebook, and display ads on Google (like Gmail, YouTube)? -->

* `{userid}` 는 광고주에게 할당된 고유 사용자 ID입니다.

* `{sid}` 는 광고주의 광고 네트워크 계정에 대한 숫자 ID로 대체됩니다. *3* 대상 [!DNL Google Ads], *10* 대상 [!DNL Microsoft Advertising], *45* 대상 [!DNL Meta], *86* 대상 [!DNL Yahoo! Display Network], *87* 대상 [!DNL Naver], *88* 대상 [!DNL Baidu], *90* 대상 [!DNL Yandex], *94* 대상 [!DNL Yahoo! Japan Ads], *105* 대상 [!DNL Yahoo Native] (더 이상 사용되지 않음) 또는 *106* 대상 [!DNL Pinterest] (사용하지 않음).

### [!DNL Baidu]

`s_kwcid=AL!{userid}!{sid}!{creative}!{placement}!{keywordid}`

### [!DNL Google Ads]

다음을 사용하여 쇼핑 캠페인 포함 [!DNL Google Merchant Center].

* 성과 최대 캠페인 및 초안 및 실험 캠페인에 대한 캠페인 및 광고 그룹 수준 보고를 지원하는 최신 s_kwcid 형식을 사용하는 계정:

  `s_kwcid=AL!{userid}!{sid}!{creative}!{matchtype}!{placement}!{network}!{product_partition_id}!{keyword}!{campaignid}!{adgroupid}`

* 다른 모든 계정:

  `s_kwcid=AL!{userid}!{sid}!{creative}!{matchtype}!{placement}!{network}!{product_partition_id}!{keyword}`

>[!NOTE]
>
>* 동적 검색 광고의 경우, {keyword} 가 자동 타겟으로 채워집니다.
>* 에 대한 추적을 생성하는 경우 [!DNL Google] 쇼핑 광고, 제품 ID 매개 변수, `{adwords_producttargetid}`는 키워드 매개 변수 앞에 삽입됩니다. 제품 ID 매개 변수가 [!DNL Google Ads] 계정 수준 및 캠페인 수준 추적 매개 변수.
>* 최신 s_kwcid 추적 코드를 사용하려면 &quot;[에 대한 s_kwcid 추적 코드 업데이트 [!DNL Google Ads] account](/help/search-social-commerce/campaign-management/accounts/update-skwcid-google.md).&quot;

<!--

### [!DNL Meta]

`s_kwcid=AL!{userid}!{sid}!{{ad.id}}!{{campaign.id}}!{{adset.id}}`

where:

* `{{ad.id}}` is the unique numeric ID for the ad/creative.

* `{{campaign.id}}` is the unique ID for the campaign.

* `{{adset.id}}` is the unique ID for the ad set.

-->

### [!DNL Microsoft Advertising]

* 캠페인 검색:

  `s_kwcid=AL!{userid}!{sid}!{AdId}!{OrderItemId}`

* 쇼핑 캠페인(사용) [!DNL Microsoft Merchant Center]):

  `s_kwcid=AL!{userid}!{sid}!{AdId}!{CriterionId}`

* 대상 네트워크 캠페인:

  `s_kwcid=AL!{userid}!{sid}!{AdId}`

### [!DNL Yahoo! Japan Ads]

`s_kwcid=AL!{userid}!{sid}!{creative}!{matchtype}!{network}!{keyword}`

### [!DNL Yandex]

`s_kwcid=AL!{userid}!{sid}!{ad_id}!{source_type}!!!{phrase_id}`

>[!MORELIKETHIS]
>
>* [개요 [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md){target="_blank"}
>* [광고 네트워크 계정 관리](/help/search-social-commerce/campaign-management/accounts/ad-network-account-manage.md)
>* [Baidu 캠페인 설정](/help/search-social-commerce/campaign-management/campaigns/campaign-settings-baidu.md)
>* [Google 광고 캠페인 설정](/help/search-social-commerce/campaign-management/campaigns/campaign-settings-google.md)
>* [Microsoft Advertising 캠페인 설정](/help/search-social-commerce/campaign-management/campaigns/campaign-settings-microsoft.md)
>* [야후! 일본 광고 캠페인 설정](/help/search-social-commerce/campaign-management/campaigns/campaign-settings-yahoo-japan.md)
>* [Yandex 캠페인 설정](/help/search-social-commerce/campaign-management/campaigns/campaign-settings-yandex.md)
