---
title: 사용한 Adobe Advertising ID [!DNL Analytics]
description: 사용한 Adobe Advertising ID [!DNL Analytics]
feature: Integration with Adobe Analytics
exl-id: ff20b97e-27fe-420e-bd55-8277dc791081
source-git-commit: 0d48ceda77783cd8b5fd9e609da424dcfa94f278
workflow-type: tm+mt
source-wordcount: '1688'
ht-degree: 0%

---

# 사용한 Adobe Advertising ID [!DNL Analytics]

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

*Advertising DSP 및[!DNL Advertising Search, Social, & Commerce]*

Adobe Advertising은 두 개의 ID를 사용하여 온사이트 성능 추적을 수행합니다. *EF ID* 및 *AMO ID*.

광고 노출 시 Adobe Advertising은 AMO ID 및 EF ID 값을 생성하여 저장합니다. 광고를 본 방문자가 광고를 클릭하지 않고 사이트로 이동하면 [!DNL Analytics] Adobe Advertising에서 [!DNL Analytics for Advertising] JavaScript 코드. 뷰스루 트래픽의 경우 [!DNL Analytics] 보조 ID 생성(`SDID`): EF ID 및 AMO ID를 [!DNL Analytics]. 클릭스루 트래픽의 경우 이러한 ID는 를 사용하여 랜딩 페이지 URL에 포함됩니다. `ef_id` 및 `s_kwcid` (AMO ID의 경우) 쿼리 문자열 매개 변수입니다.

Adobe Advertising은 다음 기준을 사용하여 웹 사이트에 대한 클릭스루 또는 뷰스루 항목을 구별합니다.

* 뷰스루 항목은 사용자가 광고를 보고 사이트를 방문하지만 클릭하지 않을 때 캡처됩니다. [!DNL Analytics] 다음 두 가지 조건이 충족되는 경우 뷰스루를 기록합니다.

   * 방문자에게 클릭스루가 없습니다. [!DNL DSP] 또는 [!DNL Search, Social, & Commerce] 다음 기간 동안 광고 [전환 확인 기간 클릭](#lookback-a4adc).

   * 방문자가 최소 한 명 이상 본 경우 [!DNL DSP] 다음 기간 동안 광고 [노출 전환 확인 기간](#lookback-a4adc). 마지막 노출은 뷰스루로 전달됩니다.

* 클릭스루 항목은 사이트 방문자가 사이트에 들어가기 전에 광고를 클릭할 때 캡처됩니다. [!DNL Analytics] 다음 조건 중 하나가 발생하면 클릭스루를 캡처합니다.

   * URL에는 Adobe Advertising으로 랜딩 페이지 URL에 추가된 EF ID 및 AMO ID가 포함되어 있습니다.

   * URL에 추적 코드가 포함되어 있지 않지만 Adobe Advertising JavaScript 코드가 지난 2분 내에 클릭을 감지합니다.

![Adobe Advertising 보기 기반 [!DNL Analytics] 통합](/help/integrations/assets/a4adc-view-through-process.png)

*그림 1: Adobe Advertising 보기 기반 [!DNL Analytics] 통합*

![Adobe Advertising 클릭 URL 기반 [!DNL Analytics] 통합](/help/integrations/assets/a4adc-click-through-process.png)

*그림 2: Adobe Advertising 클릭 URL 기반 [!DNL Analytics] 통합*

## ADOBE ADVERTISING EF ID

EF ID는 Adobe Advertising이 활동을 온라인 클릭 또는 광고 노출과 연결하는 데 사용하는 고유한 토큰입니다. EF ID는에 저장됩니다. [an [!DNL Analytics] [!DNL eVar]](https://experienceleague.adobe.com/docs/analytics/components/dimensions/evar.html) 또는 [!DNL rVar] (예약됨 [!DNL eVar]) 차원(Adobe Advertising EF ID)을 추적하며 개별 브라우저 또는 장치 수준에서 각 광고 클릭 또는 노출을 추적합니다. EF ID는 주로 보내기 위한 키 역할을 합니다 [!DNL Analytics] 보고 및 Adobe Advertising 내 입찰 최적화를 위한 Adobe Advertising 데이터.

### EF ID 형식

>[!NOTE]
>
>EF ID는 대/소문자를 구분합니다. 다음과 같은 경우 [!DNL Analytics] 구현은 URL 추적을 소문자로 강제하므로 Adobe Advertising은 EF ID를 인식하지 못합니다. 이는 Adobe Advertising 입찰 및 보고에 영향을 주지만 내부 Adobe Advertising 보고에는 영향을 주지 않습니다 [!DNL Analytics].

#### [!DNL Google Ads] 광고 검색

```
{gclid}:G:s
```

여기서:

* `gclid` 은(는) [!DNL Google Click ID] (GCLID).
* `s` 는 네트워크 유형입니다(검색의 경우 &quot;s&quot;).

#### Microsoft Advertising 검색 광고

```
{msclkid}:G:s
```

여기서:

* `msclkid` 은(는) [!DNL Microsoft Click ID] (MSCLKID).
* `s` 는 네트워크 유형입니다(검색의 경우 &quot;s&quot;).

#### 다른 검색 엔진에 광고 및 검색 광고 표시

```
<Adobe Advertising visitor ID>:<timestamp>:<channel type>
```

여기서:

* &lt;*Adobe Advertising 방문자 ID*>은(는) 방문자당 고유 ID입니다(예: UhKVaAAABCkJ0mDt). (이)라고도 함 *서퍼 ID*.

* &lt;*timestamp*>는 YYYYMMMDDHHMMSS 형식의 시간입니다(예: 2019년, 08월, 21일, 19시간의 20190821192533).:25:33).

* &lt;*채널 유형*>은(는) 클릭 또는 노출을 담당하는 채널 유형입니다.

   * `d` DSP 디스플레이 광고 클릭용(디스플레이 클릭스루)
   * `i` DSP 디스플레이 광고 노출 횟수(디스플레이 뷰스루)
   * `s` 검색 광고 클릭(검색 클릭스루)에 대해 알아보십시오.

예 `EF ID: WcmibgAAAHJK1RyY:1551968087687:d`

### 의 EF ID Dimension [!DNL Analytics]

위치 [!DNL Analytics] 보고서에서 다음을 검색하여 EF ID 데이터를 찾을 수 있습니다 [!UICONTROL EF ID] 차원 및 사용 [!UICONTROL EF ID Instance] 지표.

EF ID에는 Analysis Workspace의 500k 고유 식별자 제한이 적용됩니다. 500k 값에 도달하면 모든 새 추적 코드가 한 줄 항목 제목 &quot;[!UICONTROL Low Traffic].&quot; 보고 충실도가 누락될 수 있기 때문에 EF ID는 분류되지 않으며, 세그먼트 또는 의 보고에 사용해서는 안 됩니다 [!DNL Analytics].

## ADOBE ADVERTISING AMO ID {#amo-id}

AMO ID는 덜 세분화된 수준에서 각 고유 광고 조합을 추적하여 다음 작업에 사용됩니다. [!DNL Analytics] Adobe Advertising에서 데이터 분류 및 광고 지표(노출 횟수, 클릭 수 및 비용 등) 수집 AMO ID는에 저장됩니다. [!DNL Analytics] [eVar](https://experienceleague.adobe.com/docs/analytics/components/dimensions/evar.html) 또는 rVar 차원(AMO ID)이며,에서 보고에만 사용됩니다. [!DNL Analytics].

AMO ID는 `s_kwcid`: 때로 &quot;&quot;로 발음됨[!DNL the squid].&quot;

### AMO ID 구현 방법 {#amo-id-implement}

매개 변수는 다음 방법 중 하나로 추적 URL에 추가됩니다.

* (권장) 서버측 삽입 기능이 구현된 경우.

   * DSP 고객: 픽셀 서버는 최종 사용자가 Adobe Advertising 픽셀로 디스플레이 광고를 볼 때 s_kwcid 매개 변수를 랜딩 페이지 접미사에 자동으로 추가합니다.

   * 검색, 소셜 및 상거래 고객:

      * 대상 [!DNL Google Ads] 및 [!DNL Microsoft® Advertising] 이(가) 있는 계정 [!UICONTROL Auto Upload] 계정 또는 캠페인에 대해 이 설정을 활성화하면, 픽셀 서버는 최종 사용자가 Adobe Advertising 픽셀이 있는 광고를 클릭할 때 s_kwcid 매개 변수를 랜딩 페이지 접미사에 자동으로 추가합니다.

      * 기타 광고 네트워크의 경우 또는 [!DNL Google Ads] 및 [!DNL Microsoft® Advertising] 이(가) 있는 계정 [!UICONTROL Auto Upload] 비활성화됨 설정, 수동으로 매개 변수 추가 [계정 수준 추가 매개 변수](/help/search-social-commerce/campaign-management/accounts/ad-network-account-manage.md){target="_blank"}를 추가합니다.

* 서버측 삽입 기능이 구현되지 않은 경우:

   * DSP 고객: [JavaScript 코드](javascript.md) 자동으로 클릭스루 및 뷰스루를 기록합니다. 브라우저가 타사 쿠키를 지원하지 않는 경우에도 다음 광고 유형에 대한 클릭 기반 전환을 추적할 수 있습니다.

      * 대상 [!DNL Flashtalking] 광고 태그, 수동으로에 추가 매크로 삽입[추가 [!DNL Analytics for Advertising] 매크로 위치 [!DNL Flashtalking] 광고 태그](/help/integrations/analytics/macros-flashtalking.md).&quot;

      * 대상 [!DNL Google Campaign Manager 360] 광고 태그, 수동으로에 추가 매크로 삽입[추가 [!DNL Analytics for Advertising] 매크로 위치 [!DNL Google Campaign Manager 360] 광고 태그](/help/integrations/analytics/macros-google-campaign-manager.md).&quot;

   * 검색, 소셜 및 상거래 고객:

      * 대상 ([!DNL Google Ads] 및 [!DNL Microsoft® Advertising]) 광고, AMO ID 매개 변수를 랜딩 페이지 접미사에 수동으로 추가합니다(이상적으로 [계정 수준](/help/search-social-commerce/campaign-management/accounts/ad-network-account-manage.md){target="_blank"} 개별 계정 구성 요소에 대해 다른 추적이 필요하지 않은 경우.

      * 다른 모든 광고 네트워크의 광고에 대해서는 AMO ID 매개 변수를 [계정 수준 추가 매개 변수](/help/search-social-commerce/campaign-management/accounts/ad-network-account-manage.md){target="_blank"}를 추가합니다.

서버측 삽입 기능을 구현하거나 비즈니스에 가장 적합한 옵션을 결정하려면 Adobe 계정 팀에 문의하십시오.

### AMO ID 형식 {#amo-id-formats}

#### 에 대한 AMO ID 포맷 [!DNL DSP]

`s_kwcid=AC!${TM_AD_ID}!${TM_PLACEMENT_ID}`

여기서:

* `AC` 디스플레이 채널을 나타냅니다.

* `{TM_AD_ID}` 는 Adobe Advertising이 생성한 영숫자 광고 키입니다. 광고에 대한 고유 식별자로, Adobe Advertising 엔티티 메타데이터를 읽을 수 있도록 변환하는 역할을 합니다 [!DNL Analytics] 차원.

* `{TM_PLACEMENT_ID}` 는 Adobe Advertising이 생성한 영숫자 배치 키입니다. 배치에 고유 식별자를 사용하며 Adobe Advertising 엔티티 메타데이터를 읽을 수 있도록 변환하는 데 키 역할을 합니다 [!DNL Analytics] 차원.

예제 AMO ID: AC!iIMvXqlOa6Nia2lDvtgw!GrVv6o2oV2qQLjQiXLC7

#### 검색, 소셜 및 상거래 광고에 대한 AMO ID 형식 {#amo-id-format-search}

매개 변수는 광고 네트워크별로 다르지만, 다음 매개 변수는 모두에게 공통입니다.

* `AL` 검색 채널을 나타냅니다. <!-- what about social/Facebook, and display ads on Google (like Gmail, YouTube)? -->

* `{userid}` 는 광고주에게 할당된 고유 사용자 ID입니다.

* `{sid}` 는 광고주의 광고 네트워크 계정에 대한 숫자 ID로 대체됩니다. *3* 대상 [!DNL Google Ads], *10* 대상 [!DNL Microsoft Advertising], *45* 대상 [!DNL Meta], *86* 대상 [!DNL Yahoo! Display Network], *87* 대상 [!DNL Naver], *88* 대상 [!DNL Baidu], *90* 대상 [!DNL Yandex], *94* 대상 [!DNL Yahoo! Japan Ads], *105* 대상 [!DNL Yahoo Native] (더 이상 사용되지 않음) 또는 *106* 대상 [!DNL Pinterest] (사용하지 않음).

##### [!DNL Baidu]

`s_kwcid=AL!{userid}!{sid}!{creative}!{placement}!{keywordid}`

여기서:

* `{creative}` 는 광고 네트워크에 대한 크리에이티브용 고유 숫자 ID입니다.
* `{placement}` 는 광고를 클릭한 웹 사이트입니다.
* `{keywordid}` 는 광고를 트리거한 키워드에 대한 광고 네트워크의 고유 숫자 ID입니다.

##### [!DNL Google Ads]

다음을 사용하여 쇼핑 캠페인 포함 [!DNL Google Merchant Center].

* 성과 최대 캠페인 및 초안 및 실험 캠페인에 대한 캠페인 및 광고 그룹 수준 보고를 지원하는 최신 AMO ID 형식을 사용하는 계정:

  `s_kwcid=AL!{userid}!{sid}!{creative}!{matchtype}!{placement}!{network}!{product_partition_id}!{keyword}!{campaignid}!{adgroupid}`

* 다른 모든 계정:

  `s_kwcid=AL!{userid}!{sid}!{creative}!{matchtype}!{placement}!{network}!{product_partition_id}!{keyword}`

여기서:

<!-- VERIFY CREATIVE description. Also, are there more networks now (audience and shopping?) -->

* `{creative}` 은(는) [!DNL Google Ads] 크리에이티브에 대한 고유 숫자 ID입니다.
* `{matchtype}` 는 광고를 트리거한 키워드의 matchtype입니다. `e` 정확히 말하자면 `p` 구문 또는 `b` 광범위하게.
* `{placement}` 는 광고를 클릭한 웹 사이트의 도메인 이름입니다. 배치 타겟팅 캠페인의 광고 및 콘텐츠 사이트에 표시되는 키워드 타겟팅 캠페인의 광고에 대해 값을 사용할 수 있습니다.
* `{network}` 클릭이 발생한 네트워크를 나타냅니다. `g` 대상 [!DNL Google] 검색(키워드 타깃팅 광고만 해당), `s` 검색 파트너(키워드 타깃팅 광고만 해당)의 경우 또는 `d` 디스플레이 네트워크용(키워드 타기팅 또는 배치 타기팅 광고)
* `{product_partition_id}` 는 제품 광고에 사용되는 제품 그룹에 대한 광고 네트워크의 고유 숫자 ID입니다.
* `{keyword}` 는 광고를 트리거한 특정 키워드(검색 사이트에서)나 가장 일치하는 키워드(콘텐츠 사이트에서)입니다.
* `{campaignid}` 은 캠페인에 대한 광고 네트워크의 고유 숫자 ID입니다.
* `{adgroupid}` 는 광고 그룹에 대한 광고 네트워크의 고유 숫자 ID입니다.

>[!NOTE]
>
>* 동적 검색 광고의 경우, {keyword} 가 자동 타겟으로 채워집니다.
>* 에 대한 추적을 생성하는 경우 [!DNL Google] 쇼핑 광고, 제품 ID 매개 변수, `{adwords_producttargetid}`는 키워드 매개 변수 앞에 삽입됩니다. 제품 ID 매개 변수가 [!DNL Google Ads] 계정 수준 및 캠페인 수준 추적 매개 변수.
>* 최신 AMO ID 추적 코드를 사용하려면 &quot;[에 대한 AMO ID 추적 코드 업데이트 [!DNL Google Ads] account](/help/search-social-commerce/campaign-management/accounts/update-amo-id-google.md).&quot; <!-- Update terminology there too. -->

<!--

##### [!DNL Meta]

`s_kwcid=AL!{userid}!{sid}!{{ad.id}}!{{campaign.id}}!{{adset.id}}`

where:

* `{{ad.id}}` is the unique numeric ID for the ad/creative.

* `{{campaign.id}}` is the unique ID for the campaign.

* `{{adset.id}}` is the unique ID for the ad set.

-->

##### [!DNL Microsoft Advertising]

* 캠페인 검색:

  `s_kwcid=AL!{userid}!{sid}!{AdId}!{OrderItemId}`

* 쇼핑 캠페인(사용) [!DNL Microsoft Merchant Center]):

  `s_kwcid=AL!{userid}!{sid}!{AdId}!{CriterionId}`

* 대상 네트워크 캠페인:

  `s_kwcid=AL!{userid}!{sid}!{AdId}`

여기서:

* `{AdId}` 는 광고 네트워크에 대한 크리에이티브용 고유 숫자 ID입니다.
* `{OrderItemId}` 는 키워드에 대한 광고 네트워크의 숫자 ID입니다.
* `{CriterionId}` 는 제품 광고에 사용되는 제품 그룹에 대한 광고 네트워크의 숫자 ID입니다.

##### [!DNL Yahoo! Japan Ads]

`s_kwcid=AL!{userid}!{sid}!{creative}!{matchtype}!{network}!{keyword}`

여기서:

* `{creative}` 는 광고 네트워크에 대한 크리에이티브용 고유 숫자 ID입니다.
* `{matchtype}` 는 광고를 트리거한 키워드의 matchtype입니다. `be` 정확히 말하자면 `bp` 구문 또는 `bb` 광범위하게.
* `{network}` 클릭이 발생한 네트워크를 나타냅니다. `n` 기본 또는 `s` 검색용.
* `{keyword}` 는 광고를 트리거한 키워드입니다.

##### [!DNL Yandex]

`s_kwcid=AL!{userid}!{sid}!{ad_id}!{source_type}!!!{phrase_id}`

여기서:

* `{ad_id}` 는 광고 네트워크에 대한 크리에이티브용 고유 숫자 ID입니다.
* `{source_type}` 는 광고가 표시된 사이트 유형입니다. *b* 검색의 경우, *c* 컨텍스트(컨텐츠)용 또는 *ct* 범주.
* `{phrase_id}` 는 키워드에 대한 광고 네트워크의 숫자 ID입니다.

### 의 AMO ID Dimension [!DNL Analytics]

Analytics 보고서에서 를 검색하여 AMO ID 데이터를 찾을 수 있습니다. [!UICONTROL AMO ID] 차원 및 사용 [!UICONTROL AMO ID Instances] 지표. 다음 [!UICONTROL AMO ID] 차원은 캡처된 모든 AMO ID 값을 포함하는 반면, [!UICONTROL AMO ID Instances] 지표는 사이트에서 AMO ID 값을 캡처한 빈도를 나타냅니다. 예를 들어 동일한 검색 광고를 4번 클릭했지만 Analytics가 7개의 사이트 항목을 추적한 경우, [!UICONTROL AMO ID Instances] 은(는) 7이고 은(는) [!UICONTROL Clicks] 4(4)가 됩니다.

내의 모든 보고 또는 감사 [!DNL Analytics], 가장 좋은 방법은 해당 인스턴스와 함께 AMO ID를 사용하는 것입니다. 자세한 내용은 &quot;[클릭스루 데이터 유효성 검사 [!DNL Analytics for Advertising]](data-variances.md#data-validation)&quot; in &quot;예상 데이터 분산 between [!DNL Analytics] 및 Adobe Advertising.&quot;

## Analytics 분류 정보

위치 [!DNL Analytics], a [분류](https://experienceleague.adobe.com/docs/analytics/components/classifications/c-classifications.html) 는 계정, 캠페인 또는 광고와 같은 지정된 추적 코드에 대한 메타데이터의 일부입니다. Adobe Advertising은 분류를 사용하여 원시 Adobe Advertising 데이터를 분류하므로 보고서를 생성할 때 광고 유형이나 캠페인별로 데이터를 다양한 방식으로 표시할 수 있습니다. 분류는 의 Adobe Advertising 보고 기준을 형성합니다 [!DNL Analytics] 및 를 AMO 지표와 함께 사용할 수 있습니다. [!UICONTROL Adobe Advertising Cost], [!UICONTROL Adobe Advertising Impressions], 및 [!UICONTROL AMO Clicks]와 같은 사용자 지정 및 표준 온사이트 이벤트 포함 [!UICONTROL Visits], [!UICONTROL Leads], [!UICONTROL Orders], 및 [!UICONTROL Revenue].

>[!MORELIKETHIS]
>
>* [개요 [!DNL Analytics for Advertising]](overview.md)
>* [다음 사이에 예상되는 데이터 분산: [!DNL Analytics] 및 Adobe Advertising](data-variances.md)
