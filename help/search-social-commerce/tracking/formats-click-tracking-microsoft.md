---
title: ' [!DNL Microsoft Advertising]에 대한 클릭 추적 형식'
description: ' [!DNL Microsoft Advertising] 계정의 클릭 추적 형식에 대해 알아봅니다.'
exl-id: 4970ac33-4978-4768-8701-6fdd3252bbd1
feature: Search Tracking
source-git-commit: 70629247a18a78b12a7fc8b166a0272764bb20b8
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 0%

---

# [!DNL Microsoft Advertising]에 대한 클릭 추적 형식

다음은 Search, Social 및 Commerce에서 [!DNL Microsoft Advertising]에 필요한 기본 추적 템플릿과 랜딩 페이지 접미사(최종 URL 접미사) 형식입니다.

## 템플릿 형식 추적

### 검색 및 대상 네트워크(사이트 링크 제외)

다음 형식은 검색 및 대상 네트워크의 모든 추적 가능한 광고 유형에 적용됩니다.

`http://pixel.everesttech.net/<advertiser_ID>/cq?ev_sid=10&ev_ln={keyword}&ev_ltx={_evltx}&ev_lx={TargetId}&ev_crx={AdId}&ev_mt={MatchType}&ev_dvc={device}&ev_phy={loc_physical_ms}&ev_loc={loc_interest_ms}&ev_cx={CampaignId}&ev_ax={AdGroupId}&ev_ex={adextensionid}&ev_efid={msclkid}:G:s&url={lpurl}`

예:

`http://pixel.everesttech.net/1234/cq?ev_sid=10&ev_ln={keyword}&ev_ltx={_evltx}&ev_lx={TargetId}&ev_crx={AdId}&ev_mt={MatchType}&ev_dvc={device}&ev_phy={loc_physical_ms}&ev_loc={loc_interest_ms}&ev_cx={CampaignId}&ev_ax={AdGroupId}&ev_ex={adextensionid}&ev_efid={msclkid}:G:s&url={lpurl}`

>[!NOTE]
>
>* `<advertiser_ID>`은(는) Adobe Advertising 내의 광고주 고유 ID에 대한 변수입니다.
>
>* 이 형식은 캠페인에 대해 토큰 전달이 활성화되었음을 나타냅니다(기본값). 토큰 전달이 비활성화된 경우 `<advertiser_ID>` 뒤의 `cq?`을(를) `c?`(으)로 바꾸십시오.
>
>* `{TargetId}`은(는) a) 키워드 또는 b) 광고를 트리거한 키워드 및 리마케팅 목록(대상)의 ID를 나타냅니다(예: 키워드 및 리마케팅 목록 모두에 대해 &quot;kwd-123:aud-456&quot; 또는 키워드에만 대해 &quot;kwd-123&quot;).

### 사이트링크

`http://pixel.everesttech.net/<advertiser_ID>/cq?ev_sid=10&ev_ln={keyword}&ev_ltx={_evltx}&ev_lx={TargetId}&ev_crx={AdId}&ev_mt={MatchType}&ev_dvc={device}&ev_phy={loc_physical_ms}&ev_loc={loc_interest_ms}&ev_cx={CampaignId}&ev_ax={AdGroupId}&ev_ex={adextensionid}&ev_efid={msclkid}:G:s&url={lpurl}`

예:

`http://pixel.everesttech.net/1234/cq?ev_sid=10&ev_ln={keyword}&ev_ltx={_evltx}&ev_lx={TargetId}&ev_crx={AdId}&ev_mt={MatchType}&ev_dvc={device}&ev_phy={loc_physical_ms}&ev_loc={loc_interest_ms}&ev_cx={CampaignId}&ev_ax={AdGroupId}&ev_ex={adextensionid}&ev_efid={msclkid}:G:s&url={lpurl}`

>[!NOTE]
>
>* `<advertiser_ID>`은(는) Adobe Advertising 내의 광고주 고유 ID에 대한 변수입니다.
>
>* 이 형식은 캠페인에 대해 토큰 전달이 활성화되었음을 나타냅니다(기본값). 토큰 전달이 비활성화된 경우 `<advertiser_ID>` 뒤의 `cq?`을(를) `c?`(으)로 바꾸십시오.
>
>* `{TargetId}`은(는) a) 키워드 또는 b) 광고를 트리거한 키워드 및 리마케팅 목록(대상)의 ID를 나타냅니다(예: 키워드 및 리마케팅 목록 모두에 대해 &quot;kwd-123:aud-456&quot; 또는 키워드에만 대해 &quot;kwd-123&quot;).
>
>* `{adextensionid}`은(는) 사용되지 않습니다.
>
>* (사이트 링크) [!UICONTROL Transaction Report]을(를) 생성하여 사이트 링크를 클릭했을 때 발생한 전환을 확인할 수 있습니다. 사이트 링크의 [!UICONTROL Link Type] 열 값은 `sl:See Current Offers`과(와) 같이 `sl:<Sitelink text>`입니다.

### 쇼핑 네트워크

다음 형식은 쇼핑 네트워크의 쇼핑 광고에 적용됩니다. 계정, 캠페인, 광고 그룹 또는 제품 그룹 수준에서 추적 템플릿을 지정할 수 있습니다.

`http://pixel.everesttech.net/<advertiser_ID>/cq?ev_sid=10&ev_crx={AdId}&ev_mt={MatchType}&ev_dvc={device}&ev_plx={ProductId}&ev_ptid={CriterionId}&ev_phy={loc_physical_ms}&ev_loc={loc_interest_ms}&ev_ex={feeditemid}&ev_efid={msclkid}:G:s&url={lpurl}`

예:

`http://pixel.everesttech.net/1234/cq?ev_sid=10&ev_crx={AdId}&ev_mt={MatchType}&ev_dvc={device}&ev_plx={ProductId}&ev_ptid={CriterionId}&ev_phy={loc_physical_ms}&ev_loc={loc_interest_ms}&ev_ex={feeditemid}&ev_efid={msclkid}:G:s&url=http%3A//www.example.com`

>[!NOTE]
>
>* `<advertiser_ID>`은(는) Adobe Advertising 내의 광고주 고유 ID에 대한 변수입니다.
>
>* 이 형식은 캠페인에 대해 토큰 전달이 활성화되었음을 나타냅니다(기본값). 토큰 전달이 비활성화된 경우 `<advertiser_ID>` 뒤의 `cq?`을(를) `c?`(으)로 바꾸십시오.
>
>* `{TargetId}`은(는) a) 키워드 또는 b) 광고를 트리거한 키워드 및 리마케팅 목록(대상)의 ID를 나타냅니다(예: 키워드 및 리마케팅 목록 모두에 대해 &quot;kwd-123:aud-456&quot; 또는 키워드에만 대해 &quot;kwd-123&quot;).
>
>* (선택 사항) 계정, 캠페인, 광고 그룹 또는 제품 그룹 수준에서 추적 템플릿을 입력하는 대신 [!DNL Microsoft Merchant Center] 계정 내에서 제품 데이터에 추적 URL을 추가할 수 있습니다. 이렇게 하려면 제품 피드 내의 사용자 지정 열 &quot;[bingads_redirect](https://help.bingads.microsoft.com/#apex/3/en/51084/0)&quot;에 추적 URL과 &quot;`link`&quot; 또는 &quot;`mobile_link`&quot; 필드의 값을 적절하게 포함하십시오. &quot;`bingads_redirect`&quot; 필드의 값은 &quot;`link`&quot; 및 &quot;`mobile_link`&quot; 필드의 값을 대체합니다. 이 방법을 사용하여 생성된 URL에는 검색, 소셜 및 Commerce 계정 또는 캠페인 설정에 지정된 추적 매개 변수가 포함되지 않습니다.

## 랜딩 페이지 접미사(최종 URL 접미사) 형식

>[!NOTE]
>
>하위 수준의 랜딩 페이지 접미사는 계정 수준 접미사를 덮어씁니다. 간편하게 유지 관리할 수 있도록 개별 계정 구성 요소에 대해 다른 추적이 필요하지 않은 경우 계정 수준 접미사만 사용하십시오. 광고 그룹 수준 또는 하위 수준에서 접미사를 구성하려면 광고 네트워크의 편집기를 사용합니다.

### 검색 및 대상 네트워크

Adobe Advertising 전환 추적을 사용하는 계정은 접미사에 광고 네트워크의 클릭 식별자([!DNL Microsoft Advertising]의 경우 `msclkid`)를 포함해야 합니다.

* 광고주가 Adobe Analytics 통합을 사용하는 경우 접미사에 다음을 포함해야 합니다.

  `ef_id={msclkid}:G:s&s_kwcid=AL!{userid}!10!{AdId}!{OrderItemId}`

* 광고주에 Adobe Analytics 통합이 없는 경우 접미사에 다음 내용이 포함되어야 합니다.

  `&ev_efid={msclkid}:G:s`

### 쇼핑 네트워크

Adobe Advertising 전환 추적을 사용하는 계정은 접미사에 광고 네트워크의 클릭 식별자([!DNL Microsoft Advertising]의 경우 `msclkid`)를 포함해야 합니다.

* 광고주가 Adobe Analytics 통합을 사용하는 경우 접미사에 다음을 포함해야 합니다.

  `ef_id={msclkid}:G:s&s_kwcid=AL!{userid}!10!{AdId}!{CriterionId}`

* 광고주에 Adobe Analytics 통합이 없는 경우 접미사에 다음 내용이 포함되어야 합니다.

  `&ev_efid={msclkid}:G:s`

>[!MORELIKETHIS]
>
>* [Adobe Advertising 전환 추적 서비스에 대한 클릭 추적 URL 형식 정보](formats-click-tracking-about.md)
>* [AMO ID 형식](/help/integrations/analytics/ids.md#amo-id-formats)
