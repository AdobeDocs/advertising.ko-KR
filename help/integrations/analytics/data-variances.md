---
title: ' [!DNL Analytics] 과(와) Adobe Advertising 사이의 예상 데이터 분산'
description: ' [!DNL Analytics] 과(와) Adobe Advertising 사이의 예상 데이터 분산'
feature: Integration with Adobe Analytics
exl-id: 66b49881-bda1-49ef-ab8a-61399b8edd0f
source-git-commit: 6470ed471c60477bf19cf9b125f0250136f31511
workflow-type: tm+mt
source-wordcount: '3358'
ht-degree: 0%

---

# [!DNL Analytics]과(와) Adobe Advertising 사이의 예상 데이터 분산

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

[!DNL Analytics for Advertising] <!-- (A4AdC) --> 통합 트랙이 있는 광고주는 Adobe Advertising 및 Adobe Analytics을 통해 유료 광고를 합니다. 여러 시스템을 통해 미디어, 캠페인 및 채널을 추적할 때 다른 시스템의 동일한 데이터 세트가 완전히 일치하는 경우는 거의 없습니다. 이 문서에서는 Adobe Advertising을 통해 거래된 미디어에 대한 데이터를 [!DNL Analytics] 내에서 미디어가 추적되는 다른 시스템의 데이터와 비교하는 방법에 대해 설명합니다.

>[!NOTE]
>
>이 문서는 Adobe Advertising 및 Analytics에 중점을 두고 있지만, 많은 주요 사항은 다른 추적 솔루션으로 전송할 수도 있습니다.

## 유사한 보고서의 속성 차이점

### 잠재적으로 다른 전환 확인 기간 및 속성 모델

[!DNL Analytics for Advertising] 통합에서는 두 개의 변수([!DNL eVars] 또는 [!DNL rVars] \[예약된 [!DNL eVars]]\)를 사용하여 [EF ID 및 AMO ID](ids.md)을(를) 캡처합니다. 이러한 변수는 단일 전환 확인 기간(클릭스루 및 뷰스루가 기여되는 시간) 및 기여도 분석 모델로 구성됩니다. 달리 지정하지 않는 한, 변수는 Adobe Advertising의 기본 광고주 수준 클릭 전환 확인 기간 및 속성 모델과 일치하도록 구성됩니다.

그러나 전환 확인 기간과 속성 모델은 Analytics([!DNL eVars]을 통해) 및 Adobe Advertising 모두에서 구성할 수 있습니다. 또한 Adobe Advertising에서 속성 모델은 광고주 수준(입찰 최적화를 위해)뿐만 아니라 개별 데이터 보기 및 보고서(보고 목적으로만)에서도 구성할 수 있습니다. 예를 들어 조직에서 최적화를 위해 짝수 배포 속성 모델을 사용하되 Advertising DSP 또는 [!DNL Advertising Search, Social, & Commerce]의 보고서에 대해 마지막 터치 속성을 사용할 수 있습니다. 속성 모델을 변경하면 속성 전환 수가 변경됩니다.

보고 전환 확인 기간 또는 속성 모델이 다른 제품에서는 수정되지 않고 한 제품에서 수정되는 경우 각 시스템의 동일한 보고서에 고유한 데이터가 표시됩니다.

* **다른 전환 확인 기간으로 인한 불일치 예:**

  Adobe Advertising에 60일 클릭 전환 확인 기간이 있고 [!DNL Analytics]에 30일 전환 확인 기간이 있다고 가정합니다. 그리고 사용자가 Adobe Advertising이 추적된 광고를 통해 사이트를 방문하고 45일에 돌아간 다음 전환한다고 가정해 봅시다. Adobe Advertising은 전환이 60일 전환 확인 기간 내에 발생했으므로 초기 방문으로 전환을 지정합니다. 그러나 30일 전환 확인 기간이 만료된 후 전환이 발생했으므로 [!DNL Analytics]은(는) 초기 방문으로 전환을 지정할 수 없습니다. 이 예제에서 Adobe Advertising은 [!DNL Analytics]보다 더 많은 전환 수를 보고합니다.

  [!DNL Analytics]![&#128279;](/help/integrations/assets/a4adc-lookback-example.png)이(가) 아닌 Adobe Advertising에 속하는 전환의 예 

* **다른 특성 모델로 인해 불일치가 발생하는 예:**

  사용자가 전환하기 전에 수입을 전환 유형으로 하여 세 개의 서로 다른 Adobe Advertising 광고와 상호 작용한다고 가정해 봅시다. Adobe Advertising 보고서에서 속성에 대해 고른 분배 모델을 사용하는 경우 모든 광고에서 고르게 매출을 기여합니다. 그러나 [!DNL Analytics]이(가) 마지막 터치 속성 모델을 사용하는 경우 수익이 마지막 광고에 기여합니다. 다음 예에서 Adobe Advertising은 세 개의 광고 각각에 캡처된 매출 30USD 중 심지어 10USD를 기여하는 반면, [!DNL Analytics]은(는) 사용자가 본 마지막 광고에 수입 30USD를 모두 기여합니다. Adobe Advertising의 보고서와 [!DNL Analytics]을(를) 비교하면 특성 차이가 미치는 영향을 알 수 있습니다.

  ![다른 속성 모델을 기반으로 하는 Adobe Advertising 및 [!DNL Analytics]에 속하는 다른 수익](/help/integrations/assets/a4adc-attribution-example.png)

>[!IMPORTANT]
>
>가장 좋은 방법은 Adobe Advertising과 [!DNL Analytics] 모두에서 동일한 전환 확인 기간과 속성 모델을 사용하는 것입니다. 필요에 따라 Adobe 계정 팀과 협력하여 현재 설정을 식별하고 구성을 동기화하십시오.

이와 동일한 개념은 다른 전환 확인 기간 또는 속성 모델을 사용하는 다른 모든 유사한 채널에도 적용됩니다.

#### 뷰스루 추적을 위한 다양한 전환 확인 기간 {#impression-lookback}

Adobe Advertising에서 속성은 클릭과 노출을 기반으로 하며 클릭과 노출에 대해 다양한 전환 확인 기간을 구성할 수 있습니다. 그러나 [!DNL Analytics]에서 속성은 클릭스루와 뷰스루를 기반으로 하며 클릭스루와 뷰스루에 대해 다른 속성 창을 설정할 수 있는 옵션이 없습니다. 초기 사이트 방문에서 각 시작을 추적합니다. 노출은 뷰스루가 발생하기 며칠 전 또는 같은 날에 발생할 수 있으며, 이 시점은 각 시스템에서 속성 창이 시작되는 위치에 영향을 줄 수 있습니다.

일반적으로 대부분의 뷰스루 전환은 두 시스템 모두 크레딧을 고려할 만큼 빠르게 발생합니다. 그러나 일부 전환은 Adobe Advertising 노출 전환 확인 기간 외부이지만 [!DNL Analytics] 전환 확인 기간 내에서 발생할 수 있습니다. 이러한 전환은 [!DNL Analytics]의 뷰스루에 의한 것이지만 Adobe Advertising의 노출에는 의한 것이 아닙니다.

다음 예에서는 방문자가 1일에 광고를 제공하고, 2일에 뷰스루 방문(즉, 이전에 광고를 클릭하지 않고 광고의 랜딩 페이지 방문)을 수행하고, 45일에 전환되었다고 가정해 봅시다. 이 경우 Adobe Advertising은 1-14일(14일 전환 확인 사용)부터 사용자를 추적하고, [!DNL Analytics]은 2-61일(60일 전환 사용)부터 사용자를 추적하며, 45일의 전환은 [!DNL Analytics] 내의 광고에 귀속되지만 Adobe Advertising 내에서는 귀속되지 않습니다.

![Adobe Advertising이 아닌 [!DNL Analytics]에 속하는 뷰스루 전환의 예](/help/integrations/assets/a4adc-viewthrough-example.png)

불일치의 또 다른 원인은 Adobe Advertising 시 클릭 기반 전환으로 인한 가중치와 관련된 사용자 지정 *뷰스루 가중치*&#x200B;를 뷰스루 전환에 할당할 수 있기 때문입니다. 기본 뷰스루 가중치는 40%이며, 이는 뷰스루 변환이 클릭 기반 전환 값의 40%로 계산됨을 의미합니다. [!DNL Analytics]은(는) 뷰스루 전환의 가중치를 제공하지 않습니다. 따라서 예를 들어, 기본 뷰스루 가중치(60USD의 차이)를 사용하는 경우 [!DNL Analytics]에서 캡처된 100USD 매출 Adobe Advertising이 40USD로 할인됩니다.

Adobe Advertising 보고서와 [!DNL Analytics] 보고서 간의 뷰스루 전환을 비교할 때 이러한 차이점을 고려하십시오.

#### 사용 가능한 속성 모델

| Adobe Advertising 속성 | [!DNL Analytics] 속성 | [!DNL eVar]/[!DNL rVar] 할당 |
|--- |--- |--- |
| [!UICONTROL Last Event] | [!UICONTROL Last Touch] | [!UICONTROL Most Recent] |
| [!UICONTROL First Event] | [!UICONTROL First Touch] | [!UICONTROL Original Value] |
| [!UICONTROL Weight First Event More] | 해당 사항 없음 | 해당 사항 없음 |
| [!UICONTROL Even Distribution] | [!UICONTROL Linear] | [!UICONTROL Linear]<br><br>사용하지 않음* |
| [!UICONTROL Weight Last Event More] | 해당 사항 없음 | 해당 사항 없음 |
| [!UICONTROL U-Shaped] | [!UICONTROL U-Shaped] | 해당 사항 없음 |
| 해당 사항 없음 | [!UICONTROL J-Shaped] | 해당 사항 없음 |
| 해당 사항 없음 | [!UICONTROL Inverse-J] | 해당 사항 없음 |
| 해당 사항 없음 | [!UICONTROL Custom] | 해당 사항 없음 |
| 해당 사항 없음 | [!UICONTROL Participation] | 해당 사항 없음 |
| 해당 사항 없음 | [!UICONTROL Algorithmic] | 해당 사항 없음 |

>[!NOTE]
>
>선형 할당의 경우 [!DNL Analytics]은(는) 단일 방문 내의 모든 [!DNL eVar] 값에 균일하게 성공 이벤트를 기여하므로 [!DNL eVar] 만료가 &quot;Visit&quot;인 선형 할당을 사용합니다. 그러나 광고의 경우 선형 기여도 분석을 사용하면 실제로 선형적이지 않고 보다 덜 이상적인 보고에 할당이 발생합니다. 예를 들어 방문자가 세 개의 별도 방문에서 전환하기 전에 세 개의 광고와 상호 작용하는 경우 마지막 방문에서 표시된 광고만 전환에 기여하는 것이며 세 개의 광고 모두가 기여하는 것은 아닙니다.
>
>또한 전환 할당을 &quot;선형&quot;으로 또는 &quot;선형&quot;으로 전환하면 내역 데이터가 표시되지 않고, 이로 인해 보고서에서 데이터가 잘못 표시될 수 있습니다. 예를 들어 선형 할당은 여러 다른 [!DNL eVar] 값에 걸쳐 매출을 나눌 수 있습니다. 할당을 &quot;가장 최근&quot;으로 변경하면 해당 매출의 100%가 가장 최근 단일 값과 연관됩니다. 이 연관성은 잘못된 결론으로 귀하를 이끌 수 있다.
>
>혼동을 방지하기 위해 [!DNL Analytics]은(는) 보고 인터페이스에서 내역 데이터를 사용할 수 없게 합니다. [!DNL eVar]을(를) 다시 초기 할당 설정으로 변경하면 내역 데이터를 볼 수 있습니다. 단, 내역 데이터에 액세스하기 위해 [!DNL eVar] 할당 설정을 변경해서는 안 됩니다. Adobe은 이미 많은 내역 데이터가 있는 [!DNL eVar]에 대한 할당 설정을 변경하는 대신 이미 기록되고 있는 데이터에 대해 새 할당 설정을 적용하려는 경우 새 [!DNL eVar]을(를) 사용하는 것을 권장합니다.

[https://experienceleague.adobe.com/ko/docs/analytics/analyze/analysis-workspace/attribution/models](https://experienceleague.adobe.com/ko/docs/analytics/analyze/analysis-workspace/attribution/models)에서 [!DNL Analytics] 속성 모델 및 해당 정의 목록을 참조하십시오.

[!DNL Search, Social, & Commerce]에 로그인한 경우 목록을 찾을 수 있습니다.

* (북미 사용자) [`https://enterprise-na.efrontier.com/CMDashboard/help/external/tracking/r_appendix_-_how_attribution_rules_are_calculated.htm`](https://enterprise-na.efrontier.com/CMDashboard/help/external/tracking/r_appendix_-_how_attribution_rules_are_calculated.htm)

* (다른 모든 사용자) [`https://enterprise-intl.efrontier.com/CMDashboard/help/external/tracking/r_appendix_-_how_attribution_rules_are_calculated.htm`](https://enterprise-intl.efrontier.com/CMDashboard/help/external/tracking/r_appendix_-_how_attribution_rules_are_calculated.htm)

#### Adobe Advertising의 이벤트 날짜 속성

Adobe Advertising에서 연결된 클릭 날짜/이벤트 날짜(클릭 또는 노출 이벤트의 날짜) 또는 트랜잭션 날짜(전환 날짜)별로 전환 데이터를 보고할 수 있습니다. 클릭/이벤트 날짜 보고의 개념이 [!DNL Analytics]에 없습니다. [!DNL Analytics]에서 추적된 모든 전환은 트랜잭션 날짜별로 보고됩니다. 결과적으로 Adobe Advertising 및 [!DNL Analytics]의 날짜가 다른 동일한 전환이 보고될 수 있습니다. 예를 들어, 1월 1일에 광고를 클릭하고 1월 5일에 전환하는 사용자가 있다고 가정해 보겠습니다. Adobe Advertising에서 이벤트 날짜별 전환 데이터를 보고 있는 경우 전환이 클릭이 발생한 1월 1일에 보고됩니다. [!DNL Analytics]에서 동일한 전환이 1월 5일에 보고됩니다.

![다른 날짜에 속하는 전환의 예](/help/integrations/assets/a4adc-conversions-based-on.png)

## [!DNL Analytics Marketing Channels]의 속성

[[!DNL Analytics Marketing Channels] 보고](https://experienceleague.adobe.com/docs/analytics/components/marketing-channels/analyze-mc.html?lang=ko)를 사용하면 히트 정보의 고유한 측면을 기반으로 다양한 마케팅 채널을 식별하는 규칙을 구성할 수 있습니다. `ef_id` 쿼리 문자열 매개 변수를 사용하여 채널을 식별하면 Adobe Advertising 추적 채널([!UICONTROL Display Click Through], [!UICONTROL Display View Through] 및 [!UICONTROL Paid Search])을 [!DNL Marketing Channels] (으)로 추적할 수 있습니다. <!-- Move most of the above text to "Marketing Channels" chapter once it's created, and add link here. --> 그러나 [!DNL Marketing Channels] 보고서가 Adobe Advertising 채널을 추적할 수 있지만, 여러 가지 이유로 데이터가 Adobe Advertising 보고서와 일치하지 않을 수 있습니다. 자세한 내용은 다음 섹션을 참조하십시오.

>[!NOTE]
>
> 다음 핵심 개념은 [`campaign`](https://experienceleague.adobe.com/docs/analytics/implementation/vars/page-vars/campaign.html?lang=ko) 변수(&quot;추적 코드&quot; 차원 또는 &quot;[!DNL eVar] 0&quot;이라고도 함) 및 사용자 지정 [!DNL eVar] 추적과 같이 Adobe Advertising에서 추적되지 않는 캠페인과 관련된 모든 다중 채널 추적에도 적용됩니다.

### [!DNL Marketing Channels]에서 잠재적으로 다른 속성 모델

대부분의 [!DNL Marketing Channels] 보고서는 [!UICONTROL Last Touch] 속성으로 구성되며, 이 속성으로 검색된 마지막 마케팅 채널에 전환 값의 100%가 할당됩니다. [!DNL Marketing Channels] 보고서 및 Adobe Advertising 보고서에 다른 속성 모델을 사용하면 속성 전환이 일치하지 않습니다.

### [!DNL Marketing Channels]에서 잠재적으로 다른 전환 확인 기간

[!DNL Marketing Channels]에 대한 전환 확인 기간을 사용자 지정할 수 있습니다. 고정된 60일 기간이 일반적이지만 Adobe Advertising에서 전환 확인 기간을 구성할 수 있습니다. 두 제품이 서로 다른 전환 확인 기간을 사용하는 경우 데이터 불일치가 발생할 수 있습니다.

### [!DNL Marketing Channels]의 다른 채널 속성

Adobe Advertising 보고서는 Adobe Advertising(유료 검색: [!DNL Advertising Search, Social, & Commerce]개 광고, 디스플레이: Advertising DSP 광고)를 통해 거래되는 유료 미디어만 캡처하지만, [!DNL Marketing Channels]개 보고서는 모든 디지털 채널을 추적할 수 있습니다. 이로 인해 전환이 속하는 채널이 불일치할 수 있습니다.

예를 들어 유료 검색과 자연어 검색 채널은 각 채널이 상대방을 돕는 공생 관계를 맺는 경우가 많다. [!DNL Marketing Channels] 보고서는 자연어 검색을 추적하지 않기 때문에 Adobe Advertising이 자연어 검색에 대해 일부 전환을 사용하지 않는 특성을 갖습니다.

디스플레이 광고를 보고, 유료 검색 광고를 클릭하고, 이메일 메시지 내부를 클릭한 다음, 30 USD 주문을 하는 고객도 생각해 보십시오. Adobe Advertising과 [!DNL Marketing Channels]이(가) 모두 마지막 터치 속성 모델을 사용하더라도 전환은 여전히 각각에 다르게 연결됩니다. Adobe Advertising에게 [!UICONTROL Email] 채널에 대한 액세스 권한이 없으므로 전환에 대한 유료 검색 크레딧이 제공됩니다. 그러나 [!DNL Marketing Channels]은(는) 세 개의 채널에 모두 액세스할 수 있으므로 전환에 대해 [!UICONTROL Email]을(를) 크레딧합니다.

[!DNL Analytics Marketing Channels]![&#128279;](/help/integrations/assets/a4adc-channel-example.png)과(와) Adobe Advertising의 다른 전환 속성의 예 

Adobe Advertising이 달라질 수 있는 이유에 대한 자세한 내용은 &quot;[채널 데이터가 다른 이유 [!DNL Marketing Channels]](marketing-channels/mc-data-variances.md)&quot;를 참조하십시오.

## Adobe Analytics [!DNL Paid Search Detection]의 데이터 차이점

[!DNL Analytics]의 [legacy [!DNL Paid Search Detection]](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/manage-report-suites/edit-report-suite/report-suite-general/paid-search-detection/paid-search-detection.html?lang=ko) 기능을 통해 회사는 [유료 및 유기 검색 트래픽을 추적하는 규칙을 정의](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/paid-search-detection/t-paid-search-detection.html?lang=ko)할 수 있습니다. [!DNL Paid Search Detection] 규칙은 쿼리 문자열과 참조 도메인을 모두 사용하여 유료 및 자연어 검색 트래픽을 식별합니다. [!DNL Paid Search Detection] 보고서는 지정된 이벤트(예: 장바구니 체크아웃)가 발생하거나 방문이 종료될 때 만료되는 더 큰 [검색 방법](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/finding-methods.html?lang=ko) 보고서 그룹의 일부입니다.

다음은 [!DNL Paid Search Detection] 규칙 집합을 만드는 인터페이스입니다.

[!DNL Analytics]![&#128279;](/help/integrations/assets/a4adc-paid-search-detection.png)에 설정된 유료 검색 감지 규칙의 예

결과 [!DNL Paid Search Detection] 보고서에는 [!UICONTROL Paid Search Engine], [!UICONTROL Paid Search Keywords], [!UICONTROL Natural Search Engine] 및 [!UICONTROL Natural Search Keywords] 보고서가 포함됩니다.

[!DNL Paid Search Detection] 보고서의 데이터에 대한 다음 두 가지 제한 사항을 참고하십시오.

* [!UICONTROL Paid Search Keywords] 및 [!UICONTROL Natural Search Keywords] 보고서에는 사용자가 입찰한 키워드가 아니라 참조 URL로 식별된 검색 쿼리가 표시됩니다. Adobe Advertising 및 [!DNL Analytics] 보고서에는 실제 키워드가 표시되므로 해당 키워드가 [!DNL Paid Search Detection] 키워드 보고서와 일치할 것으로 예상하지 마십시오.

* [!DNL Paid Search Detection] 기능이 처음 만들어졌을 때 참조 URL을 통해 광고주는 원래 검색 쿼리(사용자가 검색 엔진의 검색 막대에 입력한 문자열)를 보다 쉽게 사용할 수 있었습니다. 현재 검색 엔진은 주로 검색 쿼리를 난독화하고, 대부분의 쿼리 데이터가 &quot;지정되지 않음&quot;에 해당하기 때문에 [!DNL Paid Search Detection] 키워드 보고서는 제한된 값입니다.

  [!DNL Analytics for Advertising]을(를) 사용하면 광고주는 [!DNL Analytics]에서 유료 키워드를 추적할 수 있습니다. 참조 도메인은 트래픽을 유도한 검색 엔진을 엔진에 보고합니다. 광고주별 계정 정보가 참조 도메인에 연결되어 있지 않으므로 모든 트래픽이 검색 엔진 아래에 나열됩니다. 동일한 검색 엔진에 여러 계정이 있는 광고주는 계정별 보고를 위해 Adobe Advertising 또는 [!DNL Analytics] 보고를 참조해야 합니다.

### [!DNL Paid Search Detection]을(를) 구성하는 이유

[!DNL Paid Search Detection] 보고서를 사용하면 [[!DNL Analytics Marketing Channels] 보고서](https://experienceleague.adobe.com/docs/analytics/components/marketing-channels/analyze-mc.html?lang=ko)에서 자연어 검색 트래픽을 식별할 수 있습니다. 유료 검색 트래픽과 자연어 검색 트래픽을 구분하는 것은 자연어 검색이 전체 마케팅 생태계에 가져오는 가치를 이해하는 좋은 방법입니다.

## [!DNL Analytics for Advertising]에 대한 클릭스루 데이터 유효성 검사 {#data-validation}

통합하려면 클릭스루 데이터의 유효성을 검사하여 사이트의 모든 페이지가 클릭스루를 제대로 추적하는지 확인해야 합니다.

[!DNL Analytics]에서 [!DNL Analytics for Advertising] 추적을 확인하는 가장 쉬운 방법 중 하나는 &quot;AMO ID 인스턴스 대 클릭 수&quot; 계산된 지표를 사용하여 인스턴스를 클릭 수와 비교하는 것입니다. 이 지표는 다음과 같이 계산됩니다.

```
AMO ID Instances to Clicks = ([!UICONTROL AMO ID Instances] / [!UICONTROL Adobe Advertising Clicks])
```

[!UICONTROL AMO ID Instances]은(는) 사이트에서 [AMO ID](ids.md)을(를) 추적한 횟수를 나타냅니다. 광고를 클릭할 때마다 AMO ID(`s_kwcid`) 매개 변수가 랜딩 페이지 URL에 추가됩니다. 따라서 [!UICONTROL AMO ID Instances] 수는 클릭 수와 유사하며 실제 광고 클릭에 대해 확인할 수 있습니다. 일반적으로 [!DNL Search, Social, & Commerce]에 대한 일치율은 85%이고 [!DNL DSP] 트래픽에 대한 일치율은 30%입니다(클릭스루 [!UICONTROL AMO ID Instances]만 포함하도록 필터링될 때). 검색과 표시 간의 기대치 차이는 예상되는 트래픽 행태로 설명될 수 있다. 검색은 인텐트를 캡처하며, 따라서 사용자는 일반적으로 쿼리에서 검색 결과를 클릭하려고 합니다. 그러나 디스플레이 또는 온라인 비디오 광고를 보는 사용자는 의도하지 않게 광고를 클릭한 다음 사이트에서 바운스되거나 페이지 활동이 추적되기 전에 로드되는 새 창을 포기할 가능성이 높습니다.

Adobe Advertising 보고서에서 [!UICONTROL AMO ID Instances] 대신 &quot;[!UICONTROL EF ID Instances]&quot; 지표를 사용하여 인스턴스를 클릭과 유사하게 비교할 수 있습니다.

```
EF ID Instances to Clicks = ([!UICONTROL EF ID Instances] / [!UICONTROL Adobe Advertising Clicks])
```

AMO ID와 EF ID 간의 일치율이 높을 것으로 예상하지만, AMO ID와 EF ID는 근본적으로 다른 데이터를 추적하므로 100% 패리티를 예상하지 마십시오. 이러한 차이는 총 [!UICONTROL AMO ID Instances]과(와) [!UICONTROL EF ID Instances]에서 약간의 차이를 초래할 수 있습니다. 그러나 [!DNL Analytics]의 총 [!UICONTROL AMO ID Instances]이(가) Adobe Advertising의 [!UICONTROL EF ID Instances]과(와) 1% 이상 다른 경우 Adobe 계정 팀에 도움을 요청하십시오.

AMO ID 및 EF ID에 대한 자세한 내용은 [Analytics에서 사용하는 Adobe Advertising ID](ids.md)를 참조하십시오.

<!--  Need to create a new report to show tracking instances to clicks, instead of clicks to instances as shown, and replace this screenshot.

The following is an example of a workspace to track clicks to instances.

![Example of a workspace to track clicks to instances to clicks](/help/integrations/assets/a4adc-clicks-to-instances-example.png)
-->

### 클릭과 인스턴스 간 불일치 문제 해결

[!UICONTROL EF ID Instances] 대 클릭수 비율이 85% 미만이면 다음을 확인하십시오.

* 계정 또는 하위 수준에 대한 클릭 추적이 누락되었거나 중복 클릭 추적이 있습니까(예: 계정 및 캠페인 수준 모두에서)?

  검색, 소셜 및 Commerce에서 추적 URL을 확인하기 위해 계정에 대한 [일괄 시트를 다운로드](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-download.md)합니다.

  또한 [!DNL Analytics]에서 AMO ID 및 EF IF가 다음과 같이 계산된 &quot;[!DNL AMO ID] ~ [!DNL EF ID]&quot; 계산된 지표를 사용하여 일관되게 추가되었는지 확인할 수 있습니다.

  ```
  [!DNL AMO ID] to [!DNL EF ID] = ([!UICONTROL AMO ID] / [!DNL EF ID])
  ```

  값이 100%보다 크면 AMO ID보다 더 많은 EF ID가 누락되었음을 나타냅니다.

* AMO ID와 EF ID가 캡처되지 않도록 랜딩 페이지에 로드 문제가 있습니까?

* AMO ID와 EF ID가 손실되도록 랜딩 페이지 URL이 리디렉션됩니까?

* 모든 랜딩 페이지에서 구성된 보고서 세트를 사용합니까?

>[!NOTE]
>
>이론적으로 한 인스턴스에 여러 번의 클릭이 있을 수 있습니다. 다른 장치(예: 데스크탑, 모바일 및 태블릿)에서 클릭이 있는지 확인하십시오.

## [!DNL Analytics for Advertising]의 데이터 집합과 Adobe Advertising의 데이터 집합 비교

[AMO ID](ids.md)(s_kwcid 쿼리 문자열 매개 변수)은 [!DNL Analytics]의 보고에 사용되고 [EF ID](ids.md)(ef_id 쿼리 문자열 매개 변수)은 Adobe Advertising의 보고에 사용됩니다. 고유한 값이므로 하나의 값이 랜딩 페이지에 손상되거나 추가되지 않을 수 있습니다.

예를 들어 다음과 같은 랜딩 페이지가 있다고 가정합니다.

```
www.adobe.com/?ef_id=test_ef_id&s_kwcid=test_amo_id
```

여기서 EF ID는 &quot;`test_ef_id`&quot;이고 AMO ID는 &quot;`test_amo_id`&quot;입니다.

사이트 측 리디렉션이 발생하면 URL은 다음과 같이 종료될 수 있습니다.

```
www.adobe.com/?ef_id=test_ef_id&s_kwcid=test_amo_id#redirectAnchorTag
```

여기서 EF ID는 &quot;`test_ef_id`&quot;이고 AMO ID는 &quot;`test_amo_id#redirectAnchorTag`&quot;입니다.

이 예에서 앵커 태그를 추가하면 AMO ID에 예기치 않은 문자가 추가되어 Analytics에서 인식하지 못하는 값이 발생합니다. 이 AMO ID는 분류되지 않으며, AMO ID와 연결된 전환은 [!DNL Analytics] 보고서의 &quot;[!UICONTROL unspecified]&quot; 또는 &quot;[!UICONTROL none]&quot;에 속합니다.

다행히도, 이와 같은 문제들이 일반적이지만, 일반적으로 높은 비율의 불일치는 발생하지 않습니다. 그러나 [!DNL Analytics]의 AMO ID와 Adobe Advertising의 EF ID 간에 큰 차이가 발생하는 경우 Adobe 계정 팀에 도움을 요청하십시오.

## 기타 지표 고려 사항

### 클릭과 방문의 차이점 {#clicks-vs-visits}

유사해 보이지만 클릭과 방문은 서로 다른 데이터를 나타냅니다.

* **클릭:** [!DNL DSP] 또는 검색 엔진은 방문자가 게시자의 웹 사이트에서 광고를 클릭할 때 클릭을 기록합니다.

* **방문:** [!DNL Analytics]은(는) [방문](https://experienceleague.adobe.com/docs/analytics/components/metrics/visits.html?lang=ko)을(를) 사용자의 일련의 페이지 보기로 정의하며, 30분 동안 활동이 없는 경우와 같은 여러 기준 중 하나에 따라 종료됩니다.

정의에 따라 클릭으로 여러 번의 방문이 발생할 수 있습니다.

사용자 1과 사용자 2는 모두 Adobe Advertising 광고를 클릭하여 사이트에 액세스합니다. 사용자 1은 4개의 페이지를 본 다음 하루 동안 이동하므로 처음 클릭할 때 방문이 한 번 발생합니다. 사용자 2는 2페이지를 보고, 45분 점심을 먹고, 돌아가기, 2페이지를 더 보고 나가기, 이 경우 처음 클릭하면 2번의 방문이 발생합니다.

![클릭과 방문 간의 차이점 예](/help/integrations/assets/a4adc-visits-example.png)

### 클릭스루와 클릭스루의 차이점

<!-- Rob to let me know if we should remove this and add more info. to the section on AMO Instances etc. -->

클릭과 클릭스루는 두 가지 다른 지표입니다.

* **클릭:** [!DNL DSP] 또는 검색 엔진은 방문자가 게시자의 웹 사이트에서 광고를 클릭할 때 클릭을 기록합니다.

* **클릭스루:** [!DNL Analytics] 방문자가 대상 웹 사이트에 도달하고, 랜딩 페이지가 로드되고, 페이지 하단에 있는 [!DNL Analytics] 요청이 데이터를 [!DNL Analytics]에 보낼 때 클릭스루를 기록합니다.

우발적 광고 클릭으로 인해 클릭과 클릭스루가 크게 다를 수 있습니다. 디스플레이 광고에서 클릭하는 대부분의 경우 우발적인 클릭이며, 이 우발적인 방문자는 랜딩 페이지가 로드되기 전에 [뒤로] 단추를 누르므로 [!DNL Analytics]이(가) 클릭스루를 기록할 수 없습니다. 이는 모바일 광고, 비디오 광고 및 화면을 채우고 사용자가 페이지를 보기 전에 닫아야 하는 광고와 같이 실수로 클릭할 가능성이 높은 광고에 특히 해당됩니다.

또한 모바일 디바이스에 로드된 사이트는 낮은 대역폭이나 사용 가능한 처리 능력 때문에 클릭스루가 발생할 가능성이 낮으므로 랜딩 페이지를 로드하는 데 더 오래 걸립니다. 클릭 수의 50~70%가 클릭스루로 이어지지 않는 일은 드물지 않습니다. 모바일 환경에서는 브라우저가 느리고 사용자가 페이지를 스크롤하거나 광고를 닫으려고 하는 동안 실수로 광고를 클릭할 가능성이 높기 때문에 차이가 90%까지 클 수 있습니다.

클릭 데이터는 현재 추적 메커니즘(예: 모바일 앱으로 들어가는 클릭 수 또는 모바일 앱으로부터의 클릭 수)으로 클릭스루를 기록할 수 없거나 광고주가 하나의 추적 접근 방식만 배포한 환경에 기록될 수 있습니다(예: 뷰스루 JavaScript 접근 방식을 사용하는 경우 서드파티 쿠키를 차단하는 브라우저는 클릭스루를 추적하지만 추적하지 않음). Adobe에서 클릭 URL 추적 및 뷰스루 JavaScript 추적 접근 방식을 모두 배포하도록 권장하는 주요 이유는 추적 가능한 클릭스루의 범위를 극대화하기 위해서입니다.

### 비 Adobe Advertising Dimension에 대한 Adobe Advertising 트래픽 지표 사용

Adobe Advertising은 Analytics에 [광고 관련 트래픽 지표 및  [!DNL DSP] 및 [!DNL Search, Social, & Commerce]](advertising-metrics-in-analytics.md)의 관련 차원을 제공합니다. Adobe Advertising이 제공한 지표는 지정된 Adobe Advertising 차원에만 적용할 수 있으며 [!DNL Analytics]의 다른 차원에는 데이터를 사용할 수 없습니다.

예를 들어 Adobe Advertising 차원인 계정별로 [!UICONTROL Adobe Advertising Clicks] 및 [!UICONTROL Adobe Advertising Cost] 지표를 보면 계정별로 총 [!UICONTROL Adobe Advertising Clicks] 및 [!UICONTROL Adobe Advertising Cost]이(가) 표시됩니다.

![Adobe Advertising 차원을 사용한 보고서의 Adobe Advertising 지표 예](/help/integrations/assets/a4adc-traffic-supported-dimension.png)

그러나 Adobe Advertising에서 데이터를 제공하지 않는 페이지 내 차원(예: 페이지)으로 [!UICONTROL Adobe Advertising Clicks] 및 [!UICONTROL Adobe Advertising Cost] 지표를 보는 경우 각 페이지의 [!UICONTROL Adobe Advertising Clicks] 및 [!UICONTROL Adobe Advertising Cost]은(는) 0입니다.

![지원되지 않는 차원을 사용하는 보고서의 Adobe Advertising 지표의 예](/help/integrations/assets/a4adc-traffic-unsupported-dimension.png)

### Adobe Advertising이 아닌 Dimension을 사용하여 클릭 대용으로 [!UICONTROL AMO ID Instances] 사용

사이트 내 차원과 함께 [!UICONTROL AMO Clicks]을(를) 사용할 수 없으므로 클릭에 해당하는 값을 찾을 수 있습니다. 방문 횟수를 대체품으로 사용하고 싶을 수 있지만 각 방문자에게 여러 번의 방문이 있을 수 있으므로 방문 횟수는 최선의 옵션이 아닙니다. (&quot;[클릭과 방문 간의 차이점](#clicks-vs-visits)&quot;을(를) 참조하십시오. 대신 AMO ID가 캡처된 횟수인 [!UICONTROL AMO ID Instances]을(를) 사용하는 것이 좋습니다. [!UICONTROL AMO ID Instances]이(가) [!UICONTROL AMO Clicks]과(와) 정확히 일치하지 않지만 사이트의 클릭 트래픽을 측정하는 데 가장 적합한 옵션입니다. 자세한 내용은 &quot; [!DNL Analytics for Advertising][&#128279;](#data-validation)에 대한 클릭스루 데이터 유효성 검사&quot;를 참조하십시오.

지원되지 않는 차원에 대한 [!UICONTROL Adobe Advertising Clicks] 대신 [!UICONTROL AMO ID Instances]의 ![예](/help/integrations/assets/a4adc-amo-id-instances.png)

>[!MORELIKETHIS]
>
>* [개요 [!DNL Analytics for Advertising]](overview.md)
>*  [!DNL Analytics][&#128279;](/help/integrations/analytics/ids.md)에서 사용하는 Adobe Advertising ID
>* Analysis Workspace의 [Adobe Advertising 지표](/help/integrations/analytics/advertising-metrics-in-analytics.md)
>* [[!DNL Analytics] Adobe Advertising의 데이터](/help/integrations/analytics/analytics-data-in-advertising.md)
>* [Adobe Advertising과  [!DNL Marketing Channels]](/help/integrations/analytics/marketing-channels/mc-data-variances.md) 간에 데이터가 다를 수 있는 이유
