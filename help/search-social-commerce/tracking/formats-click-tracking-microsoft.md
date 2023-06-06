---
title: 클릭 추적 형식 [!DNL Microsoft Advertising]
description: 의 클릭 추적 형식에 대해 알아봅니다. [!DNL Microsoft Advertising] 계정.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 0%

---

# 클릭 추적 형식 [!DNL Microsoft Advertising]

다음은 검색, 소셜 및 상거래에 필요한 기본 추적 템플릿과 랜딩 페이지 접미사(최종 URL 접미사) 형식입니다 [!DNL Microsoft Advertising].

## 템플릿 형식 추적

### 검색 및 대상 네트워크(사이트 링크 제외)

다음 형식은 검색 및 대상 네트워크의 모든 추적 가능한 광고 유형에 적용됩니다.

`http://pixel.everesttech.net/<advertiser_ID>/cq?ev_sid=10&ev_ln={keyword}&ev_ltx={_evltx}&ev_lx={TargetId}&ev_crx={AdId}&ev_mt={MatchType}&ev_dvc={device}&ev_phy={loc_physical_ms}&ev_loc={loc_interest_ms}&ev_cx={CampaignId}&ev_ax={AdGroupId}&ev_ex={adextensionid}&ev_efid={msclkid}:G:s&url={lpurl}`

예:

`http://pixel.everesttech.net/1234/cq?ev_sid=10&ev_ln={keyword}&ev_ltx={_evltx}&ev_lx={TargetId}&ev_crx={AdId}&ev_mt={MatchType}&ev_dvc={device}&ev_phy={loc_physical_ms}&ev_loc={loc_interest_ms}&ev_cx={CampaignId}&ev_ax={AdGroupId}&ev_ex={adextensionid}&ev_efid={msclkid}:G:s&url={lpurl}`

>[!NOTE]
>
>* `<advertiser_ID>` 는 Adobe 광고 내의 광고주의 고유 ID에 대한 변수입니다.
>
>* 이 형식은 캠페인에 대해 토큰 전달이 활성화되었음을 나타냅니다(기본값). 토큰 전달이 비활성화된 경우 을(를) 대체합니다. `cq?` 이후 `<advertiser_ID>` 포함 `c?`.
>
>* `{TargetId}` 는 a) 키워드 또는 b) 광고를 트리거한 키워드 및 리마케팅 목록(대상)의 ID를 나타냅니다(예: 키워드 및 리마케팅 목록 모두에 대해 &quot;kwd-123:aud-456&quot; 또는 키워드에만 &quot;kwd-123&quot;).


### 사이트링크

`http://pixel.everesttech.net/<advertiser_ID>/cq?ev_sid=10&ev_ln={keyword}&ev_ltx={_evltx}&ev_lx={TargetId}&ev_crx={AdId}&ev_mt={MatchType}&ev_dvc={device}&ev_phy={loc_physical_ms}&ev_loc={loc_interest_ms}&ev_cx={CampaignId}&ev_ax={AdGroupId}&ev_ex={adextensionid}&ev_efid={msclkid}:G:s&url={lpurl}`

예:

`http://pixel.everesttech.net/1234/cq?ev_sid=10&ev_ln={keyword}&ev_ltx={_evltx}&ev_lx={TargetId}&ev_crx={AdId}&ev_mt={MatchType}&ev_dvc={device}&ev_phy={loc_physical_ms}&ev_loc={loc_interest_ms}&ev_cx={CampaignId}&ev_ax={AdGroupId}&ev_ex={adextensionid}&ev_efid={msclkid}:G:s&url={lpurl}`

>[!NOTE]
>
>* `<advertiser_ID>` 는 Adobe 광고 내의 광고주의 고유 ID에 대한 변수입니다.
>
>* 이 형식은 캠페인에 대해 토큰 전달이 활성화되었음을 나타냅니다(기본값). 토큰 전달이 비활성화된 경우 을(를) 대체합니다. `cq?` 이후 `<advertiser_ID>` 포함 `c?`.
>
>* `{TargetId}` 는 a) 키워드 또는 b) 광고를 트리거한 키워드 및 리마케팅 목록(대상)의 ID를 나타냅니다(예: 키워드 및 리마케팅 목록 모두에 대해 &quot;kwd-123:aud-456&quot; 또는 키워드에만 &quot;kwd-123&quot;).
>
>* `{adextensionid}` 은(는) 사용되지 않습니다.
>
>* (사이트 링크) 를 생성하여 사이트 링크를 클릭했을 때 발생한 전환을 확인할 수 있습니다. [!UICONTROL Transaction Report]. 다음 [!UICONTROL Link Type] 사이트 링크의 열 값은 입니다. `sl:<Sitelink text>`, 예: `sl:See Current Offers`.


### 쇼핑 네트워크

다음 형식은 쇼핑 네트워크의 쇼핑 광고에 적용됩니다. 계정, 캠페인, 광고 그룹 또는 제품 그룹 수준에서 추적 템플릿을 지정할 수 있습니다.

`http://pixel.everesttech.net/<advertiser_ID>/cq?ev_sid=10&ev_crx={AdId}&ev_mt={MatchType}&ev_dvc={device}&ev_plx={ProductId}&ev_ptid={CriterionId}&ev_phy={loc_physical_ms}&ev_loc={loc_interest_ms}&ev_ex={feeditemid}&ev_efid={msclkid}:G:s&url={lpurl}`

예:

`http://pixel.everesttech.net/1234/cq?ev_sid=10&ev_crx={AdId}&ev_mt={MatchType}&ev_dvc={device}&ev_plx={ProductId}&ev_ptid={CriterionId}&ev_phy={loc_physical_ms}&ev_loc={loc_interest_ms}&ev_ex={feeditemid}&ev_efid={msclkid}:G:s&url=http%3A//www.example.com`

>[!NOTE]
>
>* `<advertiser_ID>` 는 Adobe 광고 내의 광고주의 고유 ID에 대한 변수입니다.
>
>* 이 형식은 캠페인에 대해 토큰 전달이 활성화되었음을 나타냅니다(기본값). 토큰 전달이 비활성화된 경우 을(를) 대체합니다. `cq?` 이후 `<advertiser_ID>` 포함 `c?`.
>
>* `{TargetId}` 는 a) 키워드 또는 b) 광고를 트리거한 키워드 및 리마케팅 목록(대상)의 ID를 나타냅니다(예: 키워드 및 리마케팅 목록 모두에 대해 &quot;kwd-123:aud-456&quot; 또는 키워드에만 &quot;kwd-123&quot;).
>
>* (선택 사항) 계정, 캠페인, 광고 그룹 또는 제품 그룹 수준에서 추적 템플릿을 입력하는 대신 [!DNL Microsoft Merchant Center] 계정입니다. 이렇게 하려면 의 값과 함께 추적 URL을 포함합니다.`link`&quot; 또는 &quot;`mobile_link`&quot;사용자 정의 열의 해당 필드&quot;[bingads_redirect](https://help.bingads.microsoft.com/#apex/3/en/51084/0)&quot;를 입력합니다. 의 값`bingads_redirect`&quot;필드가 &quot;&quot;의 값을 대체합니다.`link`&quot; 및 &quot;`mobile_link`&quot; 필드. 이 방법을 사용하여 생성된 URL에는 검색, 소셜 및 상거래 계정 또는 캠페인 설정에 지정된 추적 매개 변수가 포함되지 않습니다.


## 랜딩 페이지 접미사(최종 URL 접미사) 형식

>[!NOTE]
>
>하위 수준의 랜딩 페이지 접미사는 계정 수준 접미사를 덮어씁니다. 간편하게 유지 관리할 수 있도록 개별 계정 구성 요소에 대해 다른 추적이 필요하지 않은 경우 계정 수준 접미사만 사용하십시오. 광고 그룹 수준 또는 하위 수준에서 접미사를 구성하려면 광고 네트워크의 편집기를 사용합니다.

### 검색 및 대상 네트워크

Adobe 광고 전환 추적을 사용하는 계정에는 광고 네트워크의 클릭 식별자(`msclkid` 대상 [!DNL Microsoft Advertising]) 접미사:

* 광고주가 Adobe Analytics 통합을 사용하는 경우 접미사에 다음을 포함해야 합니다.

   `ef_id={msclkid}:G:s&s_kwcid=AL!{userid}!{sid}!{AdId}!{OrderItemId}`

* 광고주에 Adobe Analytics 통합이 없는 경우 접미사에 다음 내용이 포함되어야 합니다.

   `&ev_efid={msclkid}:G:s`

### 쇼핑 네트워크

Adobe 광고 전환 추적을 사용하는 계정에는 광고 네트워크의 클릭 식별자(`msclkid` 대상 [!DNL Microsoft Advertising]) 접미사:

* 광고주가 Adobe Analytics 통합을 사용하는 경우 접미사에 다음을 포함해야 합니다.

   `ef_id={msclkid}:G:s&s_kwcid=AL!{userid}!{sid}!{AdId}!{CriterionId}`

* 광고주에 Adobe Analytics 통합이 없는 경우 접미사에 다음 내용이 포함되어야 합니다.

   `&ev_efid={msclkid}:G:s`

>[!MORELIKETHIS]
>
>* [Adobe 광고 전환 추적 서비스에 대한 클릭 추적 URL 형식 정보](formats-click-tracking-about.md)
>* [s\_kwcid 추적 코드 형식](skwcid-tracking-parameter.md)

