---
title: ' [!DNL Google Ads]에 대한 클릭 추적 형식'
description: ' [!DNL Google Ads] 계정의 클릭 추적 형식에 대해 알아봅니다.'
exl-id: d09c3b4e-1274-45fb-abb6-dddfe60f1477
feature: Search Tracking
source-git-commit: 70629247a18a78b12a7fc8b166a0272764bb20b8
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# [!DNL Google Ads]에 대한 클릭 추적 형식

다음은 Search, Social 및 Commerce에서 [!DNL Google Ads]에 필요한 기본 추적 템플릿과 랜딩 페이지 접미사(최종 URL 접미사) 형식입니다.

## 템플릿 형식 추적

### 사이트링크를 포함한 검색/디스플레이 네트워크

다음 형식은 검색 및 표시 네트워크의 모든 추적 가능한 광고 유형과 사이트링크에 적용됩니다.

`https://pixel.everesttech.net/<advertiser_ID>/cq?ev_sid=3&ev_ln={keyword}&ev_lx={targetid}&ev_crx={creative}&ev_mt={matchtype}&ev_n={network}&ev_ltx={_evltx}&ev_pl={placement}&ev_pos={adposition}&ev_dvc={device}&ev_dvm={devicemodel}&ev_phy={loc_physical_ms}&ev_loc={loc_interest_ms}&ev_cx={campaignid}&ev_ax={adgroupid}&ev_efid={gclid}:G:s&url={<Google ValueTrack parameter for the final URL>}`

예:

`https://pixel.everesttech.net/1234/cq?ev_sid=3&ev_ln={keyword}&ev_lx={targetid}&ev_crx={creative}&ev_mt={matchtype}&ev_n={network}&ev_ltx={_evltx}&ev_pl={placement}&ev_pos={adposition}&ev_dvc={device}&ev_dvm={devicemodel}&ev_phy={loc_physical_ms}&ev_loc={loc_interest_ms}&ev_cx={campaignid}&ev_ax={adgroupid}&ev_efid={gclid}:G:s&url={lpurl}`

>[!NOTE]
>
>* `<advertiser_ID>`은(는) Adobe Advertising 내의 광고주 고유 ID에 대한 변수입니다.
>
>* 이 형식은 캠페인에 대해 토큰 전달이 활성화되었음을 나타냅니다(기본값). 토큰 전달이 비활성화된 경우 `<advertiser_ID>` 뒤의 `cq?`을(를) `c?`(으)로 바꾸십시오.
>
>* 추적 템플릿의 최종 URL을 나타내는 [!DNL ValueTrack] 매개 변수는 `{lpurl}` 또는 `!{unescapedurl}`이어야 합니다.
>
>* (텍스트 광고) 키워드로 입찰하는 경우 `ev_pl` 매개 변수(배치용)에 값이 없습니다. 배치별로 입찰할 때 `ev_ln`(키워드의 경우)에 값이 없습니다. 광고 그룹 또는 다른 차원별로 입찰하는 경우 `ev_ln`과(와) `ev_pl` 모두에 값이 없습니다.
>
>* (동적 검색 광고) `{keyword}`은(는) `_cat:[VALUE]` 또는 `_url:[VALUE]`과(와) 같은 동적 검색 대상 식을 나타냅니다.
>
>* (동적 검색 광고) [!DNL Google Ads]은(는) 최종 URL을 동적으로 결정하므로 입력할 필요가 없습니다.
>
>* (사이트 링크) [!UICONTROL Transaction Report]을(를) 생성하여 사이트 링크를 클릭했을 때 발생한 전환을 확인할 수 있습니다. 사이트 링크의 [!UICONTROL Link Type] 열 값은 `sl:See Current Offers`과(와) 같이 `sl:<Sitelink text>`입니다.

### 쇼핑 네트워크

다음 형식은 쇼핑 네트워크의 쇼핑 광고 및 제품 그룹에 적용됩니다. 계정, 캠페인, 광고 그룹 또는 제품 그룹 수준에서 추적 템플릿을 지정할 수 있습니다.

`https://pixel.everesttech.net/<advertiser_ID>/cq?ev_sid=3&ev_lx={targetid}&ev_ln={keyword}&ev_pl={placement}&ev_crx={creative}&ev_mt={matchtype}&ev_n={network}&ev_ltx={adtype}&ev_plx={product_id}&ev_ptid={product_partition_id}&ev_mid={merchant_id}&ev_cty={product_country}&ev_lan={product_language}&ev_dvc={device}&ev_dvm={devicemodel}&ev_phy={loc_physical_ms}&ev_loc={loc_interest_ms}&ev_cx={campaignid}&ev_ax={adgroupid}&ev_efid={gclid}:G:s&url={<Google ValueTrack parameter for the final URL>}`

예:

`https://pixel.everesttech.net/1234/cq?ev_sid=3&ev_lx={targetid}&ev_ln={keyword}&ev_pl={placement}&ev_crx={creative}&ev_mt={matchtype}&ev_n={network}&ev_ltx={adtype}&ev_plx={product_id}&ev_ptid={product_partition_id}&ev_mid={merchant_id}&ev_cty={product_country}&ev_lan={product_language}&ev_dvc={device}&ev_dvm={devicemodel}&ev_phy={loc_physical_ms}&ev_loc={loc_interest_ms}&ev_cx={campaignid}&ev_ax={adgroupid}&ev_efid={gclid}:G:s&url=http%3A//www.example.com`

>[!NOTE]
>
>* `<advertiser_ID>`은(는) Adobe Advertising 내의 광고주 고유 ID에 대한 변수입니다.
>
>* 이 형식은 캠페인에 대해 토큰 전달이 활성화되었음을 나타냅니다(기본값). 토큰 전달이 비활성화된 경우 `<advertiser_ID>` 뒤의 `cq?`을(를) `c?`(으)로 바꾸십시오.
>
>* 추적 템플릿의 최종 URL을 나타내는 [!DNL ValueTrack] 매개 변수는 `{lpurl}` 또는 `!{unescapedurl}`이어야 합니다.
>
>* [!DNL Google Ads]은(는) Google 판매자 센터 피드의 제품 URL을 최종 URL로 사용하므로 제품 데이터나 제품 그룹의 최종 URL을 입력할 필요가 없습니다.
>
>* [!UICONTROL Transaction Report]을(를) 생성하여 쇼핑 광고를 클릭했을 때 전환된 결과를 확인할 수 있습니다. 제품 광고의 [!UICONTROL Link Type] 열 값은 pla:`<product ID>`(예: `pla:8525822`)입니다.

## 랜딩 페이지 접미사(최종 URL 접미사) 형식

Adobe Advertising 전환 추적을 사용하는 계정은 접미사에 광고 네트워크의 클릭 식별자([!DNL Google Ads]의 경우 `gclid`)를 포함해야 합니다.

* 광고주가 Adobe Analytics 통합을 사용하는 경우 접미사에 다음 중 하나가 포함되어야 합니다.

   * 성과 최대 캠페인, 초안 및 실험 캠페인에 대한 캠페인 및 광고 그룹 수준 보고를 지원하는 최신 [AMO ID 형식](/help/integrations/analytics/ids.md#amo-id-formats)(`s_kwcid`부터 시작)을 사용하는 [!DNL Google Ads] 계정:

     `ef_id={gclid}:G:s&s_kwcid=AL!{userid}!3!{creative}!{matchtype}!{placement}!{network}!{product_partition_id}!{keyword}!{campaignid}!{adgroupid}`

     계정에 서버측 AMO ID 구현이 있고 계정 또는 캠페인 설정 &quot;[!UICONTROL Auto Upload]&quot;이(가) 활성화되어 있으면 매개 변수가 자동으로 추가됩니다. 그렇지 않으면 수동으로 추가해야 합니다. &quot; [!DNL Analytics][&#128279;](/help/integrations/analytics/ids.md#amo-id-implement)에서 사용하는 Adobe Advertising ID&quot;를 참조하십시오.&quot;

   * 다른 모든 [!DNL Google Ads] 계정:

     `ef_id={gclid}:G:s&s_kwcid=AL!{userid}!3!{creative}!{matchtype}!{placement}!{network}!{product_partition_id}!{keyword}`

* 광고주에 Adobe Analytics 통합이 없는 경우 접미사에 다음 내용이 포함되어야 합니다.

  `&ev_efid={gclid}:G:s`

>[!NOTE]
>
>* 하위 수준의 랜딩 페이지 접미사는 계정 수준 접미사를 덮어씁니다. 간편하게 유지 관리할 수 있도록 개별 계정 구성 요소에 대해 다른 추적이 필요하지 않은 경우 계정 수준 접미사만 사용하십시오. 광고 그룹 수준 또는 하위 수준에서 접미사를 구성하려면 광고 네트워크의 편집기를 사용합니다.
>
>* (동적 검색 광고, Adobe Analytics이 있고 서버측 추적이 없는 광고주) Adobe Advertising에서 Analytics로의 역방향 피드에 대한 추적을 포함하려면 AMO ID 추적 코드를 계정 수준 랜딩 페이지 접미사 끝에 추가합니다.

>[!MORELIKETHIS]
>
>* [Adobe Advertising 전환 추적 서비스에 대한 클릭 추적 URL 형식 정보](formats-click-tracking-about.md)
>* [AMO ID 형식](/help/integrations/analytics/ids.md#amo-id-formats)
