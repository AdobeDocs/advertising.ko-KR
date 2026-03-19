---
title: Adobe Advertising ID를 사용하여  [!DNL Marketing Channels] 규칙 만들기
description: Adobe Advertising ID를 사용하여  [!DNL Analytics Marketing Channels]에 대한 처리 규칙을 만드는 방법을 알아봅니다.
feature: Integration with Adobe Analytics
exl-id: 525761b4-607f-4b03-9020-8051009a13c6
source-git-commit: 0813a8bddc1ecf238f4a62c4fcefd8584f32e152
workflow-type: tm+mt
source-wordcount: '1448'
ht-degree: 0%

---

# Adobe Advertising ID를 사용하여 [!DNL Marketing Channels] 처리 규칙 만들기

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

Adobe Advertising ID([AMO ID 및 EF ID](../ids.md))를 사용하여 Adobe Analytics에서 [!DNL Marketing Channels] 처리 규칙을 구성할 수 있습니다. Adobe Advertising 캠페인과 관련된 규칙에 Adobe Advertising ID를 사용합니다. 규칙을 처리하는 순서에 따라 가능한 모든 데이터가 올바르게 캡처되는지 여부가 결정됩니다.

## 처리 규칙의 AMO ID

AMO ID는 [!DNL Analytics] 내에서 Adobe Advertising 데이터를 보고하는 데 사용되는 기본 추적 코드입니다. AMO ID는 [!DNL Analytics] 내에서 세분화된 보고를 제공하기 위해 Adobe에서 관리하는 동적 값의 연결입니다. [!DNL Analytics] [eVar](https://experienceleague.adobe.com/docs/analytics/components/dimensions/evar.html?lang=ko) 또는 rVar 차원(AMO ID)에 저장됩니다. AMO ID는 두 가지 방법으로 [!DNL Analytics]에 설정할 수 있습니다.

* 클릭스루 추적: Adobe Advertising은 링크에 `s_kwcid` 쿼리 문자열 매개 변수를 설정하고 클릭스루가 발생할 때 [!DNL Analytics]이(가) 랜딩 페이지 URL에서 매개 변수를 선택합니다.

* 뷰스루 추적([!DNL DSP]만 해당): [!DNL Last Event Service]이(가) 서버측에서 뷰스루를 감지하여 AMO ID를 [!DNL Analytics]에 보냅니다. 이 경우 URL에 `s_kwcid` 매개 변수가 포함되어 있지 않습니다.

AMO ID 내의 동적 값은 추적된 마케팅 채널을 나타냅니다.

* AMO ID의 접두사를 사용하여 [!DNL Marketing Channels] 내의 최상위 채널을 식별할 수 있습니다.

* AMO ID 본문의 문자 구는 보다 구체적인 캠페인 유형을 나타냅니다.

* 접미사 &quot;vt&quot;는 [!DNL DSP] 뷰스루 트래픽에 대해 있으며 별도의 클릭스루 및 뷰스루 [!DNL DSP] 채널을 만드는 데 사용할 수 있습니다.

AMO ID의 나머지 부분은 무시할 수 있습니다.

| [!UICONTROL AMO ID] | 채널 | 규칙 논리 |
|--------|---------|--------------------|
| !ctv(접미사) | [!UICONTROL DSP Connected TV ViewThrough] | 종료 문자 |
| !d! (본문) | [!UICONTROL Display Network] | 다음 포함 |
| ! (본문) | [!UICONTROL Google Search] | 다음 포함 |
| !s! (본문) | [!UICONTROL Search Partner] | 다음 포함 |
| ! (본문) | [!UICONTROL Smart Shopping Campaign] | 다음 포함 |
| ! (본문) | [!UICONTROL YouTube Video Ad] | 다음 포함 |
| ! (본문) | [!UICONTROL YouTube Search Ad] | 다음 포함 |
| !vp! (본문) | [!UICONTROL Google Video Partners] | 다음 포함 |
| !vt(접미어) | [!UICONTROL DSP ViewThrough] | 종료 문자 |
| 알! (접두사) | [!UICONTROL Paid Search] | 다음으로 시작 |
| ac! (접두사) | [!UICONTROL DSP Display] | 다음으로 시작 |

## 처리 규칙의 EF ID

AMO EF ID(EF ID)는 [!DNL Analytics for Advertising] 통합에서 사용되는 두 번째 추적 코드입니다. 기본 목적은 [!DNL Analytics] 이벤트 데이터를 추적하여 Adobe Advertising에 전달하는 것입니다. 클릭스루 또는 뷰스루가 발생할 때마다, 동일한 방문자에 대해 정확히 동일한 광고라고 하더라도 고유한 EF ID가 생성됩니다. EF ID는 일반적으로 [!DNL Analytics]의 변수 제한당 50만 개의 고유 값을 초과하여 보고에 사용할 수 없으므로 [!DNL Analytics] 보고 사용자 인터페이스에 사용되지 않습니다. Adobe Advertising 지표 및 메타데이터는 EF ID에는 적용되지 않습니다. AMO ID에만 적용됩니다. Adobe Advertising에서 캠페인을 최적화하려면 추가된 추적 세부 기간이 필요하므로 두 ID가 모두 필요합니다.

EF ID 차원은 [!DNL Analytics] 보고에 직접 사용되지 않지만 마케팅 채널을 만드는 데 유용할 수 있습니다. EF ID 접미사는 채널(디스플레이 또는 검색)과 방문이 클릭스루로 시작되었는지 뷰스루로 시작되었는지를 나타냅니다. EF ID의 구분 기호는 AMO ID의 느낌표가 아닌 콜론입니다.

| EF ID 접미사 | 채널 |
|-------|---------|
| :s | [!UICONTROL Paid Search Click-through] |
| :d | [!UICONTROL Display ClickThrough] |
| :i | [!UICONTROL Display ViewThrough] |

## Adobe Advertising에 대한 처리 규칙 예

다음 예제 규칙 세트는 광고 채널(유료 검색, 디스플레이 클릭스루 및 디스플레이 뷰스루)에 대한 규칙에 중점을 둡니다. 유료 검색 감지를 위한 권장 규칙(해당 규칙이 자연어 검색 마케팅 채널 논리와 상호 작용하는 방법 포함)과 자연어 참조 도메인 규칙에 대한 선택적 업데이트도 표시됩니다.

**참고:** 디스플레이는 광고주 환경 설정에 따라 두 채널로 분리하거나 단일 채널로 병합할 수 있습니다.

일반적인 구현에서의 다른 채널들에 대한 광고 채널들의 동작들의 권장 순서를 예시하기 위해 다른 채널들이 예시적인 스크린샷에 포함된다.

>[!IMPORTANT]
>
>규칙을 처리하는 순서에 대한 자세한 내용은 &quot;[작업 순서  [!DNL Marketing Channels] 규칙](#rule-order)&quot;을(를) 참조하십시오.

![처리 규칙 집합의 예](/help/integrations/assets/a4adc-mc-rule-set-example.png)

### 유료 검색 규칙

가장 좋은 방법은 [!UICONTROL Paid Search] 규칙에 대해 &quot;Any&quot; 연산자가 있는 두 가지 조건을 포함하는 것입니다.

* 비용/클릭/노출 데이터에는 AMO ID가 포함되어 있으므로 AMO ID를 포함합니다. AMO ID는 &quot;AL!&quot;로 시작해야 합니다. 클릭/비용/노출 데이터를 [!UICONTROL Paid Search]에 올바르게 할당하려면.<!-- Is this just called AMO ID there, not s_kwcid=XXX? What's the difference? -->

* [!UICONTROL Paid Search] 클릭스루의 URL에는 항상 `s_kwcid` 쿼리 문자열 매개 변수가 포함되므로 방문자가 랜딩 페이지로 다시 이동할 경우 적절한 중복 제거가 발생하도록 이 매개 변수를 포함합니다. &quot;AL!&quot; 포함 클릭/비용/노출 데이터를 `s_kwcid`에 올바르게 할당하려면 [!UICONTROL Paid Search] 전에 완료하십시오.

채널의 값을 AMO ID로 설정하지 마십시오. 대신 참조 도메인, 검색 엔진 + 키워드 또는 페이지와 같은 항목으로 설정합니다. (모든 [!DNL Marketing Channels]과(와) 관련이 있습니다.)

<!-- Explain that comment about relevancy -- do I need to repeat this for each rule example?  -->

![유료 검색 규칙의 예](/help/integrations/assets/a4adc-mc-rule-paid-search.png "유료 검색 규칙의 예")

### 자연어 검색 규칙

[!UICONTROL Natural Search]의 경우 [[!UICONTROL Paid Search] 검색 규칙](https://experienceleague.adobe.com/ko/docs/analytics/admin/admin-tools/manage-report-suites/edit-report-suite/report-suite-general/paid-search-detection/t-paid-search-detection)에 `ef_id` 및 `s_kwcid` 쿼리 문자열 매개 변수가 포함되어 있는지 확인하십시오. (일반적으로 Advertising Search, Social 및 Commerce이 [!DNL Analytics]에 통합되면 자동으로 구성되지만, 통합이 구성된 후 [!DNL Analytics] 관리자가 논리를 변경한 경우를 확인하십시오.)

규칙을 &quot;자연어 검색 감지 규칙과 일치&quot;로 설정합니다(일반적으로 이 채널의 기본 설정임).

![자연어 검색 규칙의 예](/help/integrations/assets/a4adc-mc-rule-natural-search.png "자연어 검색 규칙의 예")

### 클릭스루 규칙 #1 표시

클릭스루만 캡처하여 디스플레이 클릭스루 마케팅 채널을 만듭니다. AMO ID는 클릭스루와 뷰스루 모두에서 동일하기 때문에 이 규칙은 EF ID 변수와 `ef_id` 쿼리 문자열 매개 변수를 사용합니다.

경우에 따라 클릭스루가 URL(기본값)을 통해 추적됩니다. 다른 경우에는 서버측에서 마지막 이벤트 서비스를 통해 클릭스루가 추적되므로 URL에 `ef_id` 매개 변수가 포함되지 않습니다. 따라서 규칙은 EF ID 변수 또는 `ef_id` 쿼리 문자열 매개 변수가 &quot;:d&quot;(으)로 끝나는 조건을 확인합니다. 두 조건 중 하나에 대해 이 규칙을 트리거하려면 &quot;`Any`&quot; 연산자를 사용하십시오.

![첫 번째 디스플레이 클릭스루 규칙의 예](/help/integrations/assets/a4adc-mc-rule-display-ct.png "첫 번째 디스플레이 클릭스루 규칙의 예")

### 자연어 참조 도메인 규칙

(선택 사항) 가장 좋은 방법은 &quot;Any&quot; 연산자와 함께 &quot;방문의 첫 페이지임&quot; 조건을 표준 [!UICONTROL Natural Referring Domains] 규칙에 추가하는 것입니다. 이 규칙은 선택 사항이지만 사용자가 뒤로 단추를 클릭하여 랜딩 페이지로 돌아갈 때 자연 레퍼러의 Edge Case가 설정되지 않도록 하는 데 도움이 될 수 있습니다.

![자연어 참조 도메인 규칙의 예](/help/integrations/assets/a4adc-mc-rule-natural-referring-domains.png "자연어 참조 도메인 규칙의 예")

### CTV 뷰스루 규칙 표시

[!DNL DSP] 연결된 TV(CTV) 뷰스루를 추적하려면 AMO ID가 `"!ctv"`(으)로 끝나는 규칙을 만듭니다. 방문자가 광고를 클릭하지 않았기 때문에 뷰스루 추적에는 URL에 `ef_id` 또는 `s_kwcid`이(가) 포함되지 않으며 규칙에는 하나의 조건만 필요합니다.

![Display CTV ViewThrough 규칙의 예](/help/integrations/assets/a4adc-mc-rule-display-ctv-vt.png "Display CTV ViewThrough 규칙의 예")

### 뷰스루 규칙 표시

Display ViewThrough 채널을 만들려면 EF ID가 &quot;:i&quot;(으)로 끝나는 규칙을 만듭니다. 방문자가 광고를 클릭하지 않았기 때문에 뷰스루 추적에는 URL에 `ef_id` 또는 `s_kwcid`이(가) 포함되지 않으며 규칙에는 하나의 조건만 필요합니다.

![Display ViewThrough 규칙의 예](/help/integrations/assets/a4adc-mc-rule-display-vt.png "Display ViewThrough 규칙의 예")

### 클릭스루 규칙 #2 표시

두 번째 Display ClickThrough 규칙의 경우 **AMO ID 시작을 &quot;AC!&quot;로 설정합니다.**. 이 두 번째 규칙은 Adobe Advertising에서 [!DNL Analytics]&#x200B;(으)로 직접 들어오는 디스플레이 채널에 대한 클릭/비용/노출 데이터를 캡처하는 데 있습니다. 이 데이터는 AMO ID로 인한 것이지만 `ef_id` 쿼리 문자열이 있는 URL은 포함하지 않으므로 이러한 히트는 첫 번째 디스플레이 ClickThrough 규칙이 캡처하는 AMO EF ID와 연결되지 않습니다.

![두 번째 디스플레이 클릭스루 규칙의 예](/help/integrations/assets/a4adc-mc-rule-display-ct2.png "두 번째 디스플레이 클릭스루 규칙의 예")

## [!DNL Marketing Channels] 규칙에 대한 작업 순서 {#rule-order}

![Adobe Advertising 관련 규칙에 적합한 작업 순서](/help/integrations/assets/a4adc-mc-rule-order.png "Adobe Advertising 관련 규칙에 적합한 작업 순서")

* [!UICONTROL Paid Search] *이전* [!UICONTROL Natural Search]에 넣습니다. 그렇지 않으면, 자연어 검색에 유료 검색 데이터가 할당될 수 있다.

* **처음** [!UICONTROL Display ClickThrough] *이전* [!UICONTROL Natural Referring Domains] 및 [!UICONTROL Natural Social]을(를) 넣습니다.

* [!UICONTROL CTV view-throughs]을(를) 사용하는 경우 *이전* [!UICONTROL Display ViewThroughs]에 넣으십시오. 그렇지 않으면 CTV 뷰스루가 디스플레이 뷰스루로 캡처됩니다.

* 동일한 랜딩 이벤트에서 뷰스루와 [!UICONTROL Display ViewThroughs]이(가) 아닌 클릭스루가 발생할 수 있으므로 *을(를)*&#x200B;다음[!UICONTROL Internal] 다른 채널을 [!UICONTROL Direct]과(와) [!DNL Advertising] 앞에 추가합니다. 예를 들어 방문자가 Adobe Advertising 광고를 보고 노출을 받은 다음 [!UICONTROL Natural Search]을(를) 통해 사이트로 이동할 수 있습니다.

  가장 좋은 방법은 뷰스루보다 다른 채널([!UICONTROL Internal] 및 [!UICONTROL Direct] 제외)의 우선 순위를 설정하는 것입니다.

* 일부 광고주는 [!UICONTROL Display ViewThroughs]보다 [!UICONTROL Natural Referring Domains]의 우선 순위를 지정할 수 있습니다. 두 규칙의 처리 순서를 변경하여 이를 수행합니다.

* **초** [!UICONTROL Display ClickThrough] 규칙은 Adobe Advertising에서 [!DNL Analytics]&#x200B;(으)로 직접 들어오는 클릭/비용/노출 데이터를 catch하는 데 있습니다. 이 데이터는 AMO ID에만 속하기 때문에 이러한 히트는 AMO EF ID와 연결되지 않습니다. 이 규칙을 설정하지 않으면 모든 클릭/비용/노출 데이터가 [!UICONTROL Direct]과(와) 일치하지 않는 데이터의 기본 채널인 [!DNL Marketing Channel] 채널에 속합니다. 이 규칙은 뷰스루 규칙을 *이후*&#x200B;해야 합니다. 그렇지 않으면 모든 뷰스루가 선택됩니다.

<!-- WORDING!!!!  Check on this, and if it's necessary still with the other info about order:  If you include additional marketing channels, be sure to run your rules in order of specificity. For example, say you create a processing rule for [!DNL YouTube] video ad traffic tracked by Advertising Search, Social, & Commerce. The AMO ID for video traffic starts with with "AL!" and contain "!ytv!". If you run the rule for Paid Search (for which the AMO ID starts with "AL!") and then run the rule for video traffic, the YouTube video ad traffic would all fall under the Paid Search channel. -->

>[!MORELIKETHIS]
>
>* [기본  [!DNL Analytics Marketing Channels]](mc-overview.md)
>* [채널 데이터가 Adobe Advertising과  [!DNL Marketing Channels]](mc-data-variances.md) 간에 다를 수 있는 이유
>* [사용 [!DNL Analytics Marketing Channels] Adobe Advertising 데이터 사용](mc-ac-data.md)
>* [비디오: Adobe Advertising 보고에  [!DNL Marketing Channels] 사용](https://experienceleague.adobe.com/docs/advertising-learn/tutorials/analytics/analytics-reporting-a4adc.html?lang=ko)
>* [에서 사용하는  [!DNL Analytics]](/help/integrations/analytics/ids.md)Adobe Advertising ID