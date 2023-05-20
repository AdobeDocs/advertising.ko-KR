---
title: Adobe 광고 ID 사용됨 [!DNL Analytics]
description: Adobe 광고 ID 사용됨 [!DNL Analytics]
feature: Integration with Adobe Analytics
exl-id: ff20b97e-27fe-420e-bd55-8277dc791081
source-git-commit: 7f35b3f3b33ed320ac186d219cbd0f826666bb3b
workflow-type: tm+mt
source-wordcount: '1183'
ht-degree: 0%

---

# Adobe 광고 ID 사용됨 [!DNL Analytics]

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

*Advertising DSP 및[!DNL Advertising Search, Social, & Commerce]*

Adobe 광고는 두 개의 ID를 사용하여 온사이트 성과 추적을 수행합니다. *EF ID* 및 *AMO ID*.

광고 노출이 발생하면 Adobe 광고에서 AMO ID 및 EF ID 값을 생성하고 저장합니다. 광고를 본 방문자가 광고를 클릭하지 않고 사이트로 이동하면 [!DNL Analytics] 는 Adobe 광고에서 다음을 통해 이러한 값을 호출합니다. [!DNL Analytics for Advertising] JavaScript 코드. 뷰스루 트래픽의 경우 [!DNL Analytics] 보조 ID 생성(`SDID`): EF ID 및 AMO ID를 [!DNL Analytics]. 클릭스루 트래픽의 경우 이러한 ID는 를 사용하여 랜딩 페이지 URL에 포함됩니다. `s_kwcid` 및 `ef_id` 쿼리 문자열 매개 변수.

Adobe 광고는 다음 기준을 사용하여 웹 사이트에 대한 클릭스루 또는 뷰스루 항목을 구별합니다.

* 뷰스루 항목은 사용자가 광고를 보고 사이트를 방문하지만 클릭하지 않을 때 캡처됩니다. [!DNL Analytics] 다음 두 가지 조건이 충족되는 경우 뷰스루를 기록합니다.
   * 방문자에게 클릭스루가 없습니다. [!DNL DSP] 또는 [!DNL Search, Social, & Commerce] 다음 기간 동안 광고 [전환 확인 기간 클릭](#lookback-a4adc).
   * 방문자가 최소 한 명 이상 본 경우 [!DNL DSP] 다음 기간 동안 광고 [노출 전환 확인 기간](#lookback-a4adc). 마지막 노출은 뷰스루로 전달됩니다.
* 클릭스루 항목은 사이트 방문자가 사이트에 들어가기 전에 광고를 클릭할 때 캡처됩니다. [!DNL Analytics] 다음 조건 중 하나가 발생하면 클릭스루를 캡처합니다.
   * URL에는 Adobe 광고에 의해 랜딩 페이지 URL에 추가된 EF ID 및 AMO ID가 포함되어 있습니다.
   * URL에 추적 코드가 포함되어 있지 않지만 Adobe Advertising JavaScript 코드가 지난 2분 내에 클릭을 감지합니다.

![Adobe 광고 보기 기반 [!DNL Analytics] 통합](/help/integrations/assets/a4adc-view-through-process.png)

*그림 1: Adobe 광고 보기 기반 [!DNL Analytics] 통합*

![Adobe 광고 클릭 URL 기반 [!DNL Analytics] 통합](/help/integrations/assets/a4adc-click-through-process.png)

*그림 2: Adobe 광고 클릭 URL 기반 [!DNL Analytics] 통합*

## Adobe 광고 EF ID

EF ID는 Adobe Advertising이 활동을 온라인 클릭 또는 광고 노출과 연결하는 데 사용하는 고유한 토큰입니다. EF ID는에 저장됩니다. [!DNL Analytics] [eVar](https://experienceleague.adobe.com/docs/analytics/components/dimensions/evar.html) 또는 rVar(예약된 eVar) 차원(Adobe Advertising EF ID)을 추적하며 개별 브라우저 또는 장치 수준에서 각 광고 클릭 또는 노출을 추적합니다. EF ID는 주로 보내기 위한 키 역할을 합니다 [!DNL Analytics] Adobe 광고 내의 보고 및 입찰 최적화를 위한 Adobe 광고에 대한 데이터.

### EF ID 형식

>[!NOTE]
>
>EF ID는 대/소문자를 구분합니다. 다음과 같은 경우 [!DNL Analytics] 구현은 URL 추적을 소문자로 강제하므로 Adobe 광고는 EF ID를 인식하지 못합니다. 이는 Adobe 광고 입찰 및 보고에 영향을 주지만 내 Adobe 광고 보고에는 영향을 주지 않습니다 [!DNL Analytics].

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

* &lt;*Adobe 광고 방문자 ID*>은(는) 방문자당 고유 ID입니다(예: UhKVaAAABCkJ0mDt). (이)라고도 함 *서퍼 ID*.

* &lt;*timestamp*>는 YYYYMMMDDHHMMSS 형식의 시간입니다(예: 2019년, 08월, 21일, 19시간의 20190821192533).:25:33).

* &lt;*채널 유형*>은(는) 클릭 또는 노출을 담당하는 채널 유형입니다.

   * `d` DSP 디스플레이 광고 클릭용(디스플레이 클릭스루)
   * `i` DSP 디스플레이 광고 노출 횟수(디스플레이 뷰스루)
   * `s` 검색 광고 클릭(검색 클릭스루)에 대해 알아보십시오.

예 `EF ID: WcmibgAAAHJK1RyY:1551968087687:d`

### 의 EF ID Dimension [!DNL Analytics]

위치 [!DNL Analytics] 보고서에서 다음을 검색하여 EF ID 데이터를 찾을 수 있습니다 [!UICONTROL EF ID] 차원 및 사용 [!UICONTROL EF ID Instance] 지표.

EF ID에는 Analysis Workspace의 500k 고유 식별자 제한이 적용됩니다. 500k 값에 도달하면 모든 새 추적 코드가 한 줄 항목 제목 &quot;[!UICONTROL Low Traffic].&quot; 보고 충실도가 누락될 수 있기 때문에 EF ID는 분류되지 않으며, 세그먼트 또는 의 보고에 사용해서는 안 됩니다 [!DNL Analytics].

## Adobe 광고 AMO ID

AMO ID는 덜 세분화된 수준에서 각 고유 광고 조합을 추적하여 다음 작업에 사용됩니다. [!DNL Analytics] Adobe 광고에서 데이터 분류 및 광고 지표(노출 횟수, 클릭 수 및 비용 등) 수집 AMO ID는에 저장됩니다. [!DNL Analytics] [eVar](https://experienceleague.adobe.com/docs/analytics/components/dimensions/evar.html) 또는 rVar 차원(AMO ID)이며,에서 보고에만 사용됩니다. [!DNL Analytics].

AMO ID는 `s_kwcid`: 때로 &quot;&quot;로 발음됨[!DNL the squid].&quot;

### 에 대한 AMO ID 포맷 [!DNL DSP]

```
<Channel ID>!<Ad ID>!<Placement ID>
```

여기서:

* &lt;*채널 ID*>은(는) 다음과 같을 수 있습니다.

   * `AC` = Advertising DSP
   * `AL` 대상 [!DNL Advertising Search, Social, & Commerce]

* &lt;*광고 ID*>은(는) 광고에 대해 Adobe Advertising이 생성한 고유 식별자를 사용합니다. Adobe 광고 엔티티 메타데이터를 읽을 수 있도록 변환하는 키 역할을 합니다 [!DNL Analytics] 차원.

* &lt;*배치 ID*> 는 Adobe Advertising에서 생성한 배치에 대한 고유 식별자입니다. Adobe 광고 엔티티 메타데이터를 읽을 수 있도록 변환하는 키 역할을 합니다 [!DNL Analytics] 차원.

예제 AMO ID: AC!iIMvXqlOa6Nia2lDvtgw!GrVv6o2oV2qQLjQiXLC7

### 에 대한 AMO ID 포맷 [!DNL Search, Social, & Commerce]

에 대한 AMO ID [!DNL Search, Social, & Commerce] 각 검색 엔진에 대해 고유한 형식을 따르십시오. 모든 검색 엔진의 형식은 다음으로 시작됩니다.

```
AL!{userid}!{sid}
```

여기서:

* `AL` 는 광고 네트워크의 채널 ID입니다.
* `{userid}` 는 Adobe 광고가 광고주에게 할당하는 고유 숫자 사용자 ID입니다.
* `{sid}` 는 Adobe 광고가 지정된 광고 네트워크에 사용하는 숫자 ID입니다. 예: `3` 대상 [!DNL Google Ads] 또는 `10` 대상 [!DNL Microsoft Advertising].

다음은 두 개의 광고 네트워크에 대한 전체 AMO ID 형식입니다. 다른 광고 네트워크의 AMO ID 형식은 Adobe 계정 팀에 문의하십시오.

에 대한 AMO ID 포맷 [!DNL Google Ads]:

```
AL!{userid}!{sid}!{creative}!{matchtype}!{placement}!{network}!{product_partition_id}!{keyword}!{campaignid}!{adgroupid}
```

여기서:

* `{creative}` 은(는) [!DNL Google Ads] 크리에이티브에 대한 고유 숫자 ID입니다.
* `{matchtype}` 는 광고를 트리거한 키워드의 matchtype입니다. `e` 정확히 말하자면 `p` 구문 또는 `b` 광범위하게.
* `{placement}` 는 광고를 클릭한 웹 사이트의 도메인 이름입니다. 배치 타겟팅 캠페인의 광고 및 콘텐츠 사이트에 표시되는 키워드 타겟팅 캠페인의 광고에 대해 값을 사용할 수 있습니다.
* `{network}` 클릭이 발생한 네트워크를 나타냅니다.  `g` 대상 [!DNL Google] 검색(키워드 타깃팅 광고만 해당), `s` 검색 파트너(키워드 타깃팅 광고만 해당)의 경우 또는 `d` Display Network용(키워드 타기팅 또는 배치 타기팅 광고용)
* `{keyword}` 는 광고를 트리거한 특정 키워드(검색 사이트에서)나 가장 일치하는 키워드(콘텐츠 사이트에서)입니다.

에 대한 AMO ID 포맷 [!DNL Microsoft Advertising]:

```
AL!{userid}!{sid}!{AdId}!{OrderItemId}
```

여기서:

* `{AdId}` 은(는) [!DNL Microsoft Advertising] 크리에이티브에 대한 고유 숫자 ID입니다.
* `{OrderItemId}` 은(는) [!DNL Microsoft Advertising] 키워드에 대한 숫자 ID입니다.

### 의 AMO ID Dimension [!DNL Analytics]

Analytics 보고서에서 를 검색하여 AMO ID 데이터를 찾을 수 있습니다. [!UICONTROL AMO ID] 차원 및 사용 [!UICONTROL AMO ID Instance] 지표. 다음 [!UICONTROL AMO ID] 차원은 캡처된 모든 AMO ID 값을 포함하는 반면, [!UICONTROL AMO ID Instance] 지표는 사이트에서 AMO ID 값을 캡처한 빈도를 나타냅니다. 예를 들어 동일한 검색 광고를 4번 클릭했지만 Analytics가 7개의 사이트 항목을 추적한 경우, [!UICONTROL AMO ID Instance] 은(는) 7이고 은(는) [!UICONTROL Clicks] 4(4)가 됩니다.

내의 모든 보고 또는 감사 [!DNL Analytics], 가장 좋은 방법은 해당 인스턴스와 함께 AMO ID를 사용하는 것입니다. 자세한 내용은 &quot;[데이터 유효성 검사 [!DNL Analytics for Advertising]](data-variances.md#data-validation)&quot; in &quot;예상 데이터 분산 between [!DNL Analytics] 및 Adobe 광고.&quot;

## Analytics 분류 정보

위치 [!DNL Analytics], a [분류](https://experienceleague.adobe.com/docs/analytics/components/classifications/c-classifications.html) 는 계정, 캠페인 또는 광고와 같은 지정된 추적 코드에 대한 메타데이터의 일부입니다. Adobe 광고는 분류를 사용하여 원시 Adobe 광고 데이터를 분류하므로 보고서를 생성할 때 광고 유형이나 캠페인별로 데이터를 다양한 방식으로 표시할 수 있습니다. 분류는 의 Adobe 광고 보고 기준을 형성합니다 [!DNL Analytics] 및 를 AMO 지표와 함께 사용할 수 있습니다. [!UICONTROL AMO Cost], [!UICONTROL AMO Impressions], 및 [!UICONTROL AMO Clicks]와 같은 사용자 지정 및 표준 온사이트 이벤트 포함 [!UICONTROL Visits], [!UICONTROL Leads], [!UICONTROL Orders], 및 [!UICONTROL Revenue].

>[!MORELIKETHIS]
>
>* [개요 [!DNL Analytics for Advertising]](overview.md)
>* [다음 사이에 예상되는 데이터 분산: [!DNL Analytics] 및 Adobe 광고](data-variances.md)

