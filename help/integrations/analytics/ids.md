---
title: ' [!DNL Analytics]에서 사용하는 Adobe Advertising ID'
description: ' [!DNL Analytics]에서 사용하는 Adobe Advertising ID'
feature: Integration with Adobe Analytics
exl-id: ff20b97e-27fe-420e-bd55-8277dc791081
source-git-commit: 0cf325946fdc3852b8b94acb29678bf6c47227a0
workflow-type: tm+mt
source-wordcount: '1122'
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

## Adobe Advertising

EF ID는 Adobe Advertising이 활동을 개별 브라우저 또는 장치 수준에서 온라인 클릭 또는 광고 노출과 연결하는 데 사용하는 고유한 토큰입니다. EF ID는 주로 Adobe Advertising 내에서 보고 및 입찰 최적화를 위해 [!DNL Analytics] 데이터 및 Customer Journey Analytics 데이터를 Adobe Advertising에 전송하는 키 역할을 합니다.

[!DNL Analytics]의 경우 EF ID는 [an [!DNL Analytics] [!DNL eVar]](https://experienceleague.adobe.com/docs/analytics/components/dimensions/evar.html) 또는 [!DNL rVar]&#x200B;(예약된 [!DNL eVar]) 차원(Adobe Advertising EF ID)에 저장됩니다.

Customer Journey Analytics의 경우 EF ID는 `trackingIdentities``conversionDetails`[의 일부인 [!UICONTROL Adobe Advertising Cloud ExperienceEvent Full Extension] 개체의 ](https://experienceleague.adobe.com/en/docs/experience-platform/xdm/field-groups/event/advertising-full-extension) 속성에 저장됩니다.

### EF ID 형식 {#ef-id-formats}

>[!NOTE]
>
>EF ID는 대/소문자를 구분합니다. [!DNL Analytics] 또는 Customer Journey Analytics 구현에서 URL 추적을 소문자로 강제하는 경우 Adobe Advertising에서 EF ID를 인식하지 못합니다. 이는 Adobe Advertising 입찰 및 보고에 영향을 주지만 [!DNL Analytics] 또는 Customer Journey Analytics 내의 Adobe Advertising 보고에는 영향을 주지 않습니다.

#### [!DNL Google Ads]개 검색 광고

```
{gclid}:G:s
```

여기서:

* `gclid`은(는) [!DNL Google Click ID]&#x200B;(GCLID)입니다.
* `s`은(는) 네트워크 유형입니다(검색의 경우 &quot;s&quot;).

#### [!DNL Microsoft Advertising]개 검색 광고

```
{msclkid}:G:s
```

여기서:

* `msclkid`은(는) [!DNL Microsoft Click ID]&#x200B;(MSCLKID)입니다.
* `s`은(는) 네트워크 유형입니다(검색의 경우 &quot;s&quot;).

#### 다른 검색 엔진에 광고 및 검색 광고 표시

```
<Adobe Advertising visitor ID>:<timestamp>:<channel type>
```

여기서:

* &lt;*Adobe Advertising 방문자 ID*>은(는) 방문자별 고유 ID입니다(예: UhKVaAAABCkJ0mDt). *서퍼 ID*&#x200B;이라고도 합니다.

* &lt;*timestamp*>는 YYYYMMMDDHHMMSS 형식의 시간입니다(예: 2019년, 08월, 21일, 19:25:33일의 20190821192533).

* &lt;*채널 유형*>은(는) 클릭 또는 노출을 담당하는 채널 유형입니다.

   * DSP 디스플레이 광고 클릭용 `d`(디스플레이 클릭스루)
   * DSP 디스플레이 광고(디스플레이 뷰스루)의 노출에 대한 `i`
   * `s`(검색 광고 클릭(검색 클릭스루)).

예 `EF ID: WcmibgAAAHJK1RyY:1551968087687:d`

### [!DNL Analytics]의 EF ID Dimension

[!DNL Analytics] 보고서에서 [!UICONTROL EF ID] 차원을 검색하고 [!UICONTROL EF ID Instance] 지표를 사용하여 EF ID 데이터를 찾을 수 있습니다.

EF ID에는 Analysis Workspace의 500k 고유 식별자 제한이 적용됩니다. 500k 값에 도달하면 모든 새 추적 코드가 한 줄 항목 제목 &quot;[!UICONTROL Low Traffic]&quot; 아래에 보고됩니다. 보고 충실도가 누락될 수 있으므로 EF ID는 분류되지 않으므로 [!DNL Analytics]의 세그먼트나 보고에 사용하면 안 됩니다.

<!-- ## Adobe Advertising AMO IDs {#amo-id} -->

{{$include /help/_includes/amo-id.md}}

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
