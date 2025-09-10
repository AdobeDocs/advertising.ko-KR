---
title: ' [!DNL Analytics]에서 사용하는 Adobe Advertising ID'
description: ' [!DNL Analytics]에서 사용하는 Adobe Advertising ID'
feature: Integration with Adobe Analytics
exl-id: ff20b97e-27fe-420e-bd55-8277dc791081
source-git-commit: 1d7f66dd2d4775231fb21e3d79a2e337f375679b
workflow-type: tm+mt
source-wordcount: '1531'
ht-degree: 0%

---

# [!DNL Analytics]에서 사용하는 Adobe Advertising ID

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

*Advertising DSP 및[!DNL Advertising Search, Social, & Commerce]*&#x200B;에 적용 가능

Adobe Advertising에서는 현장 성능 추적에 *EF ID*&#x200B;와 *AMO ID*, 이렇게 두 개의 ID를 사용합니다.

광고 노출이 발생하면 Adobe Advertising에서 AMO ID 및 EF ID 값을 생성하고 저장합니다. 광고를 본 방문자가 광고를 클릭하지 않고 사이트로 이동하면 [!DNL Analytics]은(는) [!DNL Analytics for Advertising] JavaScript 코드를 통해 Adobe Advertising에서 이러한 값을 호출합니다. 뷰스루 트래픽의 경우 [!DNL Analytics]에서 보조 ID(`SDID`)를 생성합니다. 보조 ID는 EF ID와 AMO ID를 [!DNL Analytics]에 연결하는 데 사용됩니다. 클릭스루 트래픽의 경우 이러한 ID는 `ef_id` 및 `s_kwcid`(AMO ID의 경우) 쿼리 문자열 매개 변수를 사용하여 랜딩 페이지 URL에 포함됩니다.

Adobe Advertising은 다음 기준을 사용하여 웹 사이트에 대한 클릭스루 또는 뷰스루 항목을 구별합니다.

* 뷰스루 항목은 사용자가 광고를 보고 사이트를 방문하지만 클릭하지 않을 때 캡처됩니다. [!DNL Analytics]은(는) 다음 두 가지 조건이 충족되는 경우 뷰스루를 기록합니다.

   * [!DNL DSP]전환 확인 기간[!DNL Search, Social, & Commerce] 동안 방문자에게 [ 또는 ](/help/integrations/analytics/prerequisites.md#lookback-a4adc) 광고에 대한 클릭스루가 없습니다.

   * 방문자가 [!DNL DSP]노출 전환 확인 기간[ 동안 하나 이상의 ](/help/integrations/analytics/prerequisites.md#lookback-a4adc) 광고를 보았습니다. 마지막 노출은 뷰스루로 전달됩니다.

* 클릭스루 항목은 사이트 방문자가 사이트에 들어가기 전에 광고를 클릭할 때 캡처됩니다. 다음 조건 중 하나가 발생하면 [!DNL Analytics]에서 클릭스루를 캡처합니다.

   * 이 URL에는 Adobe Advertising에서 랜딩 페이지 URL에 추가한 EF ID와 AMO ID가 포함되어 있습니다.

   * URL에 추적 코드가 포함되어 있지 않지만 Adobe Advertising JavaScript 코드는 지난 2분 내에 클릭을 감지합니다.

![Adobe Advertising 보기 기반 [!DNL Analytics] 통합](/help/integrations/assets/a4adc-view-through-process.png)

*그림 1: Adobe Advertising 보기 기반 [!DNL Analytics] 통합*

![Adobe Advertising 클릭 URL 기반 [!DNL Analytics] 통합](/help/integrations/assets/a4adc-click-through-process.png)

*그림 2: Adobe Advertising 클릭 URL 기반 [!DNL Analytics] 통합*

<!-- ## Adobe Advertising EF IDs -->

{{$include /help/_includes/ef-id.md}}

### [!DNL Analytics]의 EF ID Dimension

[!DNL Analytics] 보고서에서 [!UICONTROL EF ID] 차원을 검색하고 [!UICONTROL EF ID Instance] 지표를 사용하여 EF ID 데이터를 찾을 수 있습니다.

EF ID에는 Analysis Workspace의 500k 고유 식별자 제한이 적용됩니다. 500k 값에 도달하면 모든 새 추적 코드가 한 줄 항목 제목 &quot;[!UICONTROL Low Traffic]&quot; 아래에 보고됩니다. 보고 충실도가 누락될 수 있으므로 EF ID는 분류되지 않으므로 [!DNL Analytics]의 세그먼트나 보고에 사용하면 안 됩니다.

## ADOBE ADVERTISING AMO ID {#amo-id}

AMO ID는 덜 세분화된 수준에서 각각의 고유한 광고 조합을 추적하며, [!DNL Analytics] 데이터 분류와 Adobe Advertising의 광고 지표(노출 횟수, 클릭 수 및 비용 등) 수집에 사용됩니다. AMO ID는 [!DNL Analytics] [eVar](https://experienceleague.adobe.com/docs/analytics/components/dimensions/evar.html) 또는 rVar 차원(AMO ID)에 저장되며 [!DNL Analytics]의 보고에만 사용됩니다.

AMO ID를 `s_kwcid`이라고도 하며, &quot;[!DNL squid]&quot;(으)로 발음되기도 합니다.

### AMO ID 형식 {#amo-id-formats}

#### [!DNL DSP]에 대한 AMO ID 형식

`s_kwcid=AC!${TM_AD_ID}!${TM_PLACEMENT_ID}`

여기서:

* `AC`은(는) 디스플레이 채널을 나타냅니다.

* `{TM_AD_ID}`은(는) Adobe Advertising에서 생성한 영숫자 광고 키입니다. 광고의 고유 식별자를 사용하며, Adobe Advertising 엔티티 메타데이터를 읽을 수 있는 [!DNL Analytics] 차원으로 변환하는 데 중요한 역할을 합니다.

* `{TM_PLACEMENT_ID}`은(는) Adobe Advertising에서 생성한 영숫자 배치 키입니다. 배치에 고유한 식별자를 사용하며 Adobe Advertising 엔터티 메타데이터를 읽을 수 있는 [!DNL Analytics] 차원으로 변환하는 데 키 역할을 합니다.

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

### AMO ID 구현 방법 {#amo-id-implement}

매개 변수는 다음 방법 중 하나로 추적 URL에 추가됩니다.

* (권장) 서버측 삽입 기능이 구현된 경우.

   * DSP 고객: 픽셀 서버는 최종 사용자가 Adobe Advertising 픽셀로 디스플레이 광고를 볼 때 랜딩 페이지 접미사에 s_kwcid 매개 변수를 자동으로 추가합니다.

   * 검색, 소셜 및 Commerce 고객:

      * 계정 또는 캠페인에 대해 [!DNL Google Ads] 설정이 활성화된 [!DNL Microsoft Advertising] 및 [!UICONTROL Auto Upload] 계정의 경우, 최종 사용자가 Adobe Advertising 픽셀이 있는 광고를 클릭하면 픽셀 서버가 랜딩 페이지 접미사에 s_kwcid 매개 변수를 자동으로 추가합니다.

      * 다른 광고 네트워크나 [!DNL Google Ads] 설정이 비활성화된 [!DNL Microsoft Advertising] 및 [!UICONTROL Auto Upload] 계정의 경우 [계정 수준 추가 매개 변수](/help/search-social-commerce/campaign-management/accounts/ad-network-account-manage.md){target="_blank"}에 매개 변수를 수동으로 추가하여 기본 URL에 추가합니다.

* 서버측 삽입 기능이 구현되지 않은 경우:

   * DSP 고객: [JavaScript 코드](javascript.md)는 자동으로 클릭스루 및 뷰스루를 기록합니다. 브라우저가 타사 쿠키를 지원하지 않는 경우에도 다음 광고 유형에 대한 클릭 기반 전환을 추적할 수 있습니다.

      * [!DNL Flashtalking] 광고 태그의 경우 &quot;[추가 [!DNL Analytics for Advertising] 추가 [!DNL Flashtalking] 광고 태그](/help/integrations/analytics/macros-flashtalking.md)&quot;에 따라 추가 매크로를 수동으로 삽입하십시오. **참고:** 조직에서 [!DNL Flashtalking]과(와) 직접 파트너 관계를 맺고 데이터 전달 매크로를 사용하여 `s_kwcid`https://support.flashtalking.com/hc/en-us/articles/4409808166419-Accessing-Data-Pass-Macros`ef_id`에 있는 [!DNL Flashtalking] 지원 설명서별로 [ 및 ](https://support.flashtalking.com/hc/en-us/articles/4409808166419-Accessing-Data-Pass-Macros) 추적 매개 변수를 추적하는 경우에는 이 절차가 필요하지 않습니다.

      * [!DNL Google Campaign Manager 360] 광고 태그의 경우 &quot;[추가 [!DNL Analytics for Advertising] 추가 [!DNL Google Campaign Manager 360] 광고 태그](/help/integrations/analytics/macros-google-campaign-manager.md)&quot;에 따라 추가 매크로를 수동으로 삽입하십시오.

   * 검색, 소셜 및 Commerce 고객:

      * ([!DNL Google Ads] 및 [!DNL Microsoft Advertising]) 광고의 경우 개별 계정 구성 요소에 대해 다른 추적이 필요하지 않으면 AMO ID 매개 변수를 랜딩 페이지 접미사에 수동으로 추가하십시오(이상적으로는 [계정 수준](/help/search-social-commerce/campaign-management/accounts/ad-network-account-manage.md){target="_blank"}에서).

      * 다른 모든 광고 네트워크에 있는 광고의 경우 AMO ID 매개 변수를 [계정 수준 추가 매개 변수](/help/search-social-commerce/campaign-management/accounts/ad-network-account-manage.md){target="_blank"}에 수동으로 추가하여 기본 URL에 추가합니다.

서버측 삽입 기능을 구현하거나 비즈니스에 가장 적합한 옵션을 결정하려면 Adobe 계정 팀에 문의하십시오.

### [!DNL Analytics]의 AMO ID Dimension

Analytics 보고서에서 [!UICONTROL AMO ID] 차원을 검색하고 [!UICONTROL AMO ID Instances] 지표를 사용하여 AMO ID 데이터를 찾을 수 있습니다. [!UICONTROL AMO ID] 차원은 캡처된 모든 AMO ID 값을 포함하는 반면, [!UICONTROL AMO ID Instances] 지표는 사이트에서 AMO ID 값을 캡처한 빈도를 나타냅니다. 예를 들어 동일한 검색 광고를 4번 클릭했지만 Analytics가 7개의 사이트 항목을 추적한 경우 [!UICONTROL AMO ID Instances]은(는) 7개가 되고 [!UICONTROL Clicks]은(는) 4개가 됩니다.

[!DNL Analytics] 내의 보고 또는 감사의 경우 가장 좋은 방법은 해당 인스턴스와 함께 AMO ID를 사용하는 것입니다. 자세한 내용은 &quot;[과(와) Adobe Advertising 간의 예상 데이터 차이&quot;에서 &quot; [!DNL Analytics for Advertising]](data-variances.md#data-validation)에 대한 [!DNL Analytics]클릭스루 데이터 유효성 검사&quot;를 참조하십시오.

## Analytics 분류 정보

[!DNL Analytics]에서 [분류](https://experienceleague.adobe.com/docs/analytics/components/classifications/c-classifications.html)는 계정, 캠페인 또는 광고와 같은 지정된 추적 코드에 대한 메타데이터입니다. Adobe Advertising은 분류를 사용하여 원시 Adobe Advertising 데이터를 분류하므로 보고서를 생성할 때 광고 유형이나 캠페인별로 데이터를 다양한 방식으로 표시할 수 있습니다. 분류는 [!DNL Analytics]에서 Adobe Advertising 보고의 기초가 되며 [!UICONTROL Adobe Advertising Cost], [!UICONTROL Adobe Advertising Impressions] 및 [!UICONTROL AMO Clicks]과(와) 같은 AMO 지표와 함께 [!UICONTROL Visits], [!UICONTROL Leads], [!UICONTROL Orders] 및 [!UICONTROL Revenue]과(와) 같은 사용자 지정 및 표준 온사이트 이벤트에서 사용할 수 있습니다.

>[!MORELIKETHIS]
>
>* [개요 [!DNL Analytics for Advertising]](overview.md)
>* [과(와) Adobe Advertising 사이의 예상 데이터 분산 [!DNL Analytics] 과(와) ](data-variances.md)
