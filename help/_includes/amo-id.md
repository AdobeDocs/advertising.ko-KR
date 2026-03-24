---
source-git-commit: 546e391745b1469efbcc9c2024dfc193224f0ed0
workflow-type: tm+mt
source-wordcount: '111'
ht-degree: 0%

---
# ADOBE ADVERTISING AMO ID

## ADOBE ADVERTISING AMO ID {#amo-id}

AMO ID는 보다 세분화된 수준에서 각각의 고유한 광고 조합을 추적하며, [!DNL Analytics] 및 Customer Journey Analytics 데이터 분류와 Adobe Advertising에서 광고 지표(예: 노출 횟수, 클릭 수 및 비용)의 수집에 사용됩니다.

[!DNL Analytics]의 경우 AMO ID는 [eVar](https://experienceleague.adobe.com/docs/analytics/components/dimensions/evar.html?lang=ko) 또는 rVar 차원(AMO ID)에 저장됩니다.

Customer Journey Analytics의 경우 AMO ID가 `trackingCode` `conversionDetails`[의 일부인 [!UICONTROL Adobe Advertising Cloud ExperienceEvent Full Extension] 개체의 &#x200B;](https://experienceleague.adobe.com/ko/docs/experience-platform/xdm/field-groups/event/advertising-full-extension) 속성에 저장됩니다.

AMO ID를 `s_kwcid`이라고도 하며, &quot;[!DNL squid]&quot;(으)로 발음되기도 합니다.

### AMO ID 형식 {#amo-id-formats}

&quot;Adobe Analytics 구성 요소 안내서&quot;에서 [AMO ID 차원 항목에 대한 형식](https://experienceleague.adobe.com/ko/docs/analytics/components/dimensions/amo-id#dimension-items)을 참조하십시오.

<!-- Legacy content:

Notes for GGL Ads: Verify Creative description. Also, are there more networks now (audience and shopping?) Re "To use the latest AMO ID tracking code, see "[Update the AMO ID tracking code for a [!DNL Google Ads] account](/help/search-social-commerce/campaign-management/accounts/update-amo-id-google.md).: Update terminology there too.

Note: ADD IN Meta:

##### [!DNL Meta]

`s_kwcid=AL!{userid}!45!{{ad.id}}!{{campaign.id}}!{{adset.id}}`

where:

* `{{ad.id}}` is the unique numeric ID for the ad/creative.

* `{{campaign.id}}` is the unique ID for the campaign.

* `{{adset.id}}` is the unique ID for the ad set.

BEGIN LEGACY CONTENT:

#### AMO ID format for [!DNL DSP]

`s_kwcid=AC!${TM_AD_ID}!${TM_PLACEMENT_ID}`

where:

* `AC` indicates the display channel.

* `{TM_AD_ID}` is the Adobe Advertising-generated alphanumeric ad key. It's used as an unique identifier for an ad and serves as a key for translating Adobe Advertising entity metadata into readable [!DNL Analytics] and Customer Journey Analytics dimensions.

* `{TM_PLACEMENT_ID}` is the Adobe Advertising-generated alphanumeric placement key. It's used as an unique identifier for a placement and serves as a key for translating Adobe Advertising entity metadata into readable [!DNL Analytics] and Customer Journey Analytics dimensions.

Example AMO ID: AC!iIMvXqlOa6Nia2lDvtgw!GrVv6o2oV2qQLjQiXLC7

#### AMO ID formats for Search, Social, & Commerce ads {#amo-id-format-search}

The parameters vary by ad network, but the following parameters are common to all:

* `AL` indicates the search channel.

* `{userid}` is a unique user ID assigned to the advertiser.

* `{sid}` is replaced by the numeric ID for the advertiser's ad network account: *3* for [!DNL Google Ads], *10* for [!DNL Microsoft Advertising], *45* for [!DNL Meta], *86* for [!DNL Yahoo! Display Network], *87* for [!DNL Naver], *88* for [!DNL Baidu], *90* for [!DNL Yandex], *94* for [!DNL Yahoo! Japan Ads], *105* for [!DNL Yahoo Native] (deprecated), or *106* for [!DNL Pinterest] (deprecated).

##### [!DNL Baidu]

`s_kwcid=AL!{userid}!88!{creative}!{placement}!{keywordid}`

where:

* `{creative}` is the ad network's unique numeric ID for the creative.
* `{placement}` is the website on which the ad was clicked.
* `{keywordid}` is the ad network's unique numeric ID for the keyword that triggered the ad.

##### [!DNL Google Ads]

These including shopping campaigns using [!DNL Google Merchant Center].

* Accounts that use the latest AMO ID format, which supports campaign- and ad group-level reporting for performance max campaigns and drafts and experiments campaigns:

  `s_kwcid=AL!{userid}!3!{creative}!{matchtype}!{placement}!{network}!{product_partition_id}!{keyword}!{campaignid}!{adgroupid}`

* All other accounts:

  `s_kwcid=AL!{userid}!3!{creative}!{matchtype}!{placement}!{network}!{product_partition_id}!{keyword}`

where:

* `{creative}` is the [!DNL Google Ads] unique numeric ID for the creative.
* `{matchtype}` is the matchtype of the keyword that triggered the ad: `e` for exact, `p` for phrase, or `b` for broad.
* `{placement}` is the domain name of the website on which the ad was clicked. A value is available for ads in placement-targeted campaigns and for ads in keyword-targeted campaigns that are displayed on content sites.
* `{network}` indicates the network from which the click occurred: `g` for [!DNL Google] search (for keyword-targeted ads only), `s` for a search partner (for keyword-targeted ads only), or `d` for the display network (for either keyword-targeted or placement-targeted ads).
* `{product_partition_id}` is the ad network's unique numeric ID for the product group used with product ads.
* `{keyword}` is either the specific keyword that triggered your ad (on search sites) or the best-matching keyword (on content sites).
* `{campaignid}` is the ad network's unique numeric ID for the campaign.
* `{adgroupid}` is the the ad network's unique numeric ID for the ad group.

>[!NOTE]
>
>* For dynamic search ads, {keyword} is populated with the auto target.
>* When you generate tracking for [!DNL Google] shopping ads, a product ID parameter, `{adwords_producttargetid}`, is inserted before the keyword parameter. The product ID parameter doesn't appear in the [!DNL Google Ads] account-level and campaign-level tracking parameters.
>* To use the latest AMO ID tracking code, see "[Update the AMO ID tracking code for a [!DNL Google Ads] account](/help/search-social-commerce/campaign-management/accounts/update-amo-id-google.md)."

##### [!DNL Microsoft Advertising]

* All campaign types:

  `s_kwcid=AL!{userid}!10!{AdId}!!!!{OrderItemId}!!{CampaignId}!{AdGroupId}`

where:

* `{AdId}` is the ad network's unique numeric ID for the creative.
* `{OrderItemId}` is the ad network's numeric ID for the keyword.
* `{CampaignId}` is the ad network's unique numeric ID for the campaign.
* `{AdGroupId}` is the ad network's unique numeric ID for the ad group.

>[!NOTE]
>
> For accounts with campaigns without the [!UICONTROL Auto Upload] tracking option that weren't already migrated to the new format, manually update each landing page suffix to include the above format.
>In the meantime, the legacy formats, as follows, still work: 
>* Search campaigns:
>  `s_kwcid=AL!{userid}!10!{AdId}!{OrderItemId}!!{CampaignId}!{AdGroupId}`
>* Shopping campaigns (using [!DNL Microsoft Merchant Center]):
>  `s_kwcid=AL!{userid}!10!{AdId}!{CriterionId}`
>* Audience network campaigns:
>  `s_kwcid=AL!{userid}!10!{AdId}`

##### [!DNL Yahoo! Japan Ads]

`s_kwcid=AL!{userid}!94!{creative}!{matchtype}!{network}!{keyword}`

where:

* `{creative}` is the ad network's unique numeric ID for the creative.
* `{matchtype}` is the matchtype of the keyword that triggered the ad: `be` for exact, `bp` for phrase, or `bb` for broad.
* `{network}` indicates the network from which the click occurred: `n` for native or `s` for search.
* `{keyword}` is the keyword that triggered your ad.

##### [!DNL Yandex]

`s_kwcid=AL!{userid}!90!{ad_id}!{source_type}!!!{phrase_id}`

where:

* `{ad_id}` is the ad network's unique numeric ID for the creative.
* `{source_type}` is the type of site on which the ad has been displayed: *b* for search, *c* for context (content), or *ct* for category.
* `{phrase_id}` is the ad network's numeric ID for the keyword.

-->
