---
source-git-commit: 0cf325946fdc3852b8b94acb29678bf6c47227a0
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 0%

---
# ADOBE ADVERTISING AMO ID

## ADOBE ADVERTISING AMO ID {#amo-id}

AMO ID는 보다 세분화된 수준에서 각각의 고유한 광고 조합을 추적하며, [!DNL Analytics] 및 Customer Journey Analytics 데이터 분류와 Adobe Advertising에서 광고 지표(예: 노출 횟수, 클릭 수 및 비용)의 수집에 사용됩니다.

[!DNL Analytics]의 경우 AMO ID는 [eVar](https://experienceleague.adobe.com/docs/analytics/components/dimensions/evar.html?lang=ko) 또는 rVar 차원(AMO ID)에 저장됩니다.

Customer Journey Analytics의 경우 AMO ID가 `trackingCode` `conversionDetails`[의 일부인 [!UICONTROL Adobe Advertising Cloud ExperienceEvent Full Extension] 개체의 ](https://experienceleague.adobe.com/ko/docs/experience-platform/xdm/field-groups/event/advertising-full-extension) 속성에 저장됩니다.

AMO ID를 `s_kwcid`이라고도 하며, &quot;[!DNL squid]&quot;(으)로 발음되기도 합니다.

### AMO ID 형식 {#amo-id-formats}

#### [!DNL DSP]에 대한 AMO ID 형식

`s_kwcid=AC!${TM_AD_ID}!${TM_PLACEMENT_ID}`

여기서:

* `AC`은(는) 디스플레이 채널을 나타냅니다.

* `{TM_AD_ID}`은(는) Adobe Advertising에서 생성한 영숫자 광고 키입니다. 광고의 고유 식별자를 사용하며, Adobe Advertising 엔티티 메타데이터를 읽을 수 있는 [!DNL Analytics] 및 Customer Journey Analytics 차원으로 변환하는 데 중요한 역할을 합니다.

* `{TM_PLACEMENT_ID}`은(는) Adobe Advertising에서 생성한 영숫자 배치 키입니다. 배치에 고유한 식별자를 사용하며 Adobe Advertising 엔티티 메타데이터를 읽을 수 있는 [!DNL Analytics] 및 Customer Journey Analytics 차원으로 변환하는 데 중요한 역할을 합니다.

예제 AMO ID: AC!iIMvXqlOa6Nia2lDvtgw!GrVv6o2oV2qQLjQiXLC7

#### 검색, 소셜 및 Commerce 광고용 AMO ID 형식 {#amo-id-format-search}

매개 변수는 광고 네트워크별로 다르지만, 다음 매개 변수는 모두에게 공통입니다.

* `AL`은(는) 검색 채널을 나타냅니다. <!-- what about social/Facebook, and display ads on Google (like Gmail, YouTube)? -->

* `{userid}`은(는) 광고주에게 할당된 고유 사용자 ID입니다.

* `{sid}`은(는) 광고주의 광고 네트워크 계정에 대한 숫자 ID로 대체됩니다. *의 경우* 3[!DNL Google Ads], *의 경우* 10[!DNL Microsoft Advertising], *의 경우* 45[!DNL Meta], *의 경우* 86[!DNL Yahoo! Display Network], *의 경우* 87[!DNL Naver], *의 경우* 87[!DNL Baidu], *의 경우* 90[!DNL Yandex], *의 경우* 94[!DNL Yahoo! Japan Ads], *의 경우* 105[!DNL Yahoo Native]&#x200B;(더 이상 사용되지 않음) 또는 *용* 106[!DNL Pinterest]&#x200B;(더 이상 사용되지 않음).

##### [!DNL Baidu]

`s_kwcid=AL!{userid}!88!{creative}!{placement}!{keywordid}`

여기서:

* `{creative}`은(는) 광고 네트워크의 크리에이티브 고유 숫자 ID입니다.
* `{placement}`은(는) 광고를 클릭한 웹 사이트입니다.
* `{keywordid}`은(는) 광고를 트리거한 키워드에 대한 광고 네트워크의 고유 숫자 ID입니다.

##### [!DNL Google Ads]

여기에는 [!DNL Google Merchant Center]을(를) 사용하는 쇼핑 캠페인이 포함됩니다.

* 성과 최대 캠페인 및 초안 및 실험 캠페인에 대한 캠페인 및 광고 그룹 수준 보고를 지원하는 최신 AMO ID 형식을 사용하는 계정:

  `s_kwcid=AL!{userid}!3!{creative}!{matchtype}!{placement}!{network}!{product_partition_id}!{keyword}!{campaignid}!{adgroupid}`

* 다른 모든 계정:

  `s_kwcid=AL!{userid}!3!{creative}!{matchtype}!{placement}!{network}!{product_partition_id}!{keyword}`

여기서:

<!-- VERIFY CREATIVE description. Also, are there more networks now (audience and shopping?) -->

* `{creative}`은(는) 크리에이티브에 대한 [!DNL Google Ads] 고유 숫자 ID입니다.
* `{matchtype}`은(는) 광고를 트리거한 키워드의 matchtype입니다. exact의 경우 `e`, phrase의 경우 `p`, broad의 경우 `b`.
* `{placement}`은(는) 광고를 클릭한 웹 사이트의 도메인 이름입니다. 배치 타겟팅 캠페인의 광고 및 콘텐츠 사이트에 표시되는 키워드 타겟팅 캠페인의 광고에 대해 값을 사용할 수 있습니다.
* `{network}`은(는) 클릭이 발생한 네트워크를 나타냅니다. `g` 검색(키워드 대상 광고만 해당)의 경우 [!DNL Google], 검색 파트너(키워드 대상 광고만 해당)의 경우 `s`, 디스플레이 네트워크(키워드 대상 광고 또는 배치 대상 광고)의 경우 `d`.
* `{product_partition_id}`은(는) 제품 광고에 사용되는 제품 그룹에 대한 광고 네트워크의 고유 숫자 ID입니다.
* `{keyword}`은(는) 광고를 트리거한 특정 키워드(검색 사이트에서) 또는 가장 일치하는 키워드(콘텐츠 사이트에서)입니다.
* `{campaignid}`은(는) 캠페인에 대한 광고 네트워크의 고유 숫자 ID입니다.
* `{adgroupid}`은(는) 광고 그룹에 대한 광고 네트워크의 고유 숫자 ID입니다.

>[!NOTE]
>
>* 동적 검색 광고의 경우 {keyword}이(가) 자동 타겟으로 채워집니다.
>* [!DNL Google] 쇼핑 광고에 대한 추적을 생성하면 키워드 매개 변수 앞에 제품 ID 매개 변수 `{adwords_producttargetid}`이(가) 삽입됩니다. 제품 ID 매개 변수가 [!DNL Google Ads] 계정 수준 및 캠페인 수준 추적 매개 변수에 표시되지 않습니다.
>* 최신 AMO ID 추적 코드를 사용하려면 &quot;[계정 [!DNL Google Ads] 에 대한 AMO ID 추적 코드 업데이트&quot;를 참조하십시오. ](/help/search-social-commerce/campaign-management/accounts/update-amo-id-google.md)<!-- Update terminology there too. -->

<!--

##### [!DNL Meta]

`s_kwcid=AL!{userid}!45!{{ad.id}}!{{campaign.id}}!{{adset.id}}`

where:

* `{{ad.id}}` is the unique numeric ID for the ad/creative.

* `{{campaign.id}}` is the unique ID for the campaign.

* `{{adset.id}}` is the unique ID for the ad set.

-->

##### [!DNL Microsoft Advertising]

* 모든 캠페인 유형:

  `s_kwcid=AL!{userid}!10!{AdId}!!!!{OrderItemId}!!{CampaignId}!{AdGroupId}`

여기서:

* `{AdId}`은(는) 광고 네트워크의 크리에이티브 고유 숫자 ID입니다.
* `{OrderItemId}`은(는) 키워드에 대한 광고 네트워크의 숫자 ID입니다.
* `{CampaignId}`은(는) 캠페인에 대한 광고 네트워크의 고유 숫자 ID입니다.
* `{AdGroupId}`은(는) 광고 그룹에 대한 광고 네트워크의 고유 숫자 ID입니다.

>[!NOTE]
>
> 새 형식으로 이미 마이그레이션되지 않은 [!UICONTROL Auto Upload] 추적 옵션이 없는 캠페인이 있는 계정의 경우 위의 형식을 포함하도록 각 랜딩 페이지 접미사를 수동으로 업데이트하십시오.
> &#x200B;>당분간은 다음과 같은 레거시 형식이 여전히 작동합니다.
>* 캠페인 검색:
>  &#x200B;>  `s_kwcid=AL!{userid}!10!{AdId}!{OrderItemId}!!{CampaignId}!{AdGroupId}`
>* 쇼핑 캠페인([!DNL Microsoft Merchant Center] 사용):
>  &#x200B;>  `s_kwcid=AL!{userid}!10!{AdId}!{CriterionId}`
>* 대상 네트워크 캠페인:
>  &#x200B;>  `s_kwcid=AL!{userid}!10!{AdId}`

##### [!DNL Yahoo! Japan Ads]

`s_kwcid=AL!{userid}!94!{creative}!{matchtype}!{network}!{keyword}`

여기서:

* `{creative}`은(는) 광고 네트워크의 크리에이티브 고유 숫자 ID입니다.
* `{matchtype}`은(는) 광고를 트리거한 키워드의 matchtype입니다. exact의 경우 `be`, phrase의 경우 `bp`, broad의 경우 `bb`.
* `{network}`은(는) 클릭이 발생한 네트워크를 나타냅니다. `n`(기본) 또는 `s`(검색).
* `{keyword}`은(는) 광고를 트리거한 키워드입니다.

##### [!DNL Yandex]

`s_kwcid=AL!{userid}!90!{ad_id}!{source_type}!!!{phrase_id}`

여기서:

* `{ad_id}`은(는) 광고 네트워크의 크리에이티브 고유 숫자 ID입니다.
* `{source_type}`은(는) 광고가 표시된 사이트 유형입니다. 검색의 경우 *b*, 컨텍스트(콘텐츠)의 경우 *c*, 범주의 경우 *ct*.
* `{phrase_id}`은(는) 키워드에 대한 광고 네트워크의 숫자 ID입니다.
