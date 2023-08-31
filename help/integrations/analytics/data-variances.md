---
title: '다음 사이에 예상되는 데이터 분산: [!DNL Analytics] 및 Adobe Advertising'
description: '다음 사이에 예상되는 데이터 분산: [!DNL Analytics] 및 Adobe Advertising'
feature: Integration with Adobe Analytics
exl-id: 66b49881-bda1-49ef-ab8a-61399b8edd0f
source-git-commit: e564ea441e5ea0d25ee7f99962e72192750c5c40
workflow-type: tm+mt
source-wordcount: '3265'
ht-degree: 0%

---

# 다음 사이에 예상되는 데이터 분산: [!DNL Analytics] 및 Adobe Advertising

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

를 사용하는 광고주 [!DNL Analytics for Advertising] <!-- (A4AdC) --> 통합은 Adobe Advertising 및 Adobe Analytics을 통해 유료 광고를 추적합니다. 여러 시스템을 통해 미디어, 캠페인 및 채널을 추적할 때 다른 시스템의 동일한 데이터 세트가 완전히 일치하는 경우는 거의 없습니다. 이 문서에서는 Adobe Advertising을 통해 거래된 미디어의 데이터를 미디어가 추적되는 다양한 시스템의 데이터와 비교하는 방법에 대해 설명합니다 [!DNL Analytics].

>[!NOTE]
>
>이 문서는 Adobe Advertising 및 Analytics에 중점을 두고 있지만, 많은 주요 사항은 다른 추적 솔루션으로 전송할 수도 있습니다.

## 유사한 보고서의 속성 차이점

### 잠재적으로 다른 전환 확인 기간 및 속성 모델

다음 [!DNL Analytics for Advertising] 통합은 두 개의 변수([!DNL eVars] 또는 [!DNL rVars] \[예약됨 [!DNL eVars]]\) 캡처할 [EF ID 및 AMO ID](ids.md). 이러한 변수는 단일 전환 확인 기간(클릭스루 및 뷰스루가 기여되는 시간) 및 기여도 분석 모델로 구성됩니다. 달리 지정하지 않는 한, 변수는 Adobe Advertising의 기본 광고주 수준 클릭 전환 확인 기간 및 속성 모델과 일치하도록 구성됩니다.

그러나 전환 확인 기간과 속성 모델은 두 Analytics 모두에서 ( 를 통해) 구성할 수 있습니다. [!DNL eVars]) 및 Adobe Advertising. 또한 Adobe Advertising에서 속성 모델은 광고주 수준(입찰 최적화를 위해)뿐만 아니라 개별 데이터 보기 및 보고서(보고 목적으로만)에서도 구성할 수 있습니다. 예를 들어 조직은 최적화를 위해 짝수 분배 속성 모델을 사용하되 Advertising DSP 또는 의 보고서에 마지막 터치 속성을 사용하는 것을 선호할 수 있습니다. [!DNL Advertising Search, Social, & Commerce]. 속성 모델을 변경하면 속성 전환 수가 변경됩니다.

보고 전환 확인 기간 또는 속성 모델이 다른 제품에서는 수정되지 않고 한 제품에서 수정되는 경우 각 시스템의 동일한 보고서에 고유한 데이터가 표시됩니다.

* **서로 다른 전환 확인 기간으로 인해 발생하는 불일치의 예:**

  Adobe Advertising에 60일 클릭 전환 확인 기간이 있고 [!DNL Analytics] 에는 30일 전환 확인 기간이 있습니다. 그리고 사용자가 Adobe Advertising이 추적된 광고를 통해 사이트를 방문하고 45일에 돌아간 다음 전환한다고 가정해 봅시다. Adobe Advertising은 전환이 60일 전환 확인 기간 내에 발생했으므로 전환을 초기 방문으로 지정합니다. [!DNL Analytics]그러나 30일 전환 확인 기간이 만료된 후 전환이 발생했으므로 초기 방문으로 전환을 지정할 수 없습니다. 이 예에서 Adobe Advertising은 보다 많은 전환 수를 보고합니다. [!DNL Analytics] 그럴 거예요

  ![Adobe Advertising에 속하지만 그렇지 않은 전환의 예 [!DNL Analytics]](/help/integrations/assets/a4adc-lookback-example.png)

* **다른 속성 모델로 인해 발생하는 불일치의 예:**

  사용자가 전환하기 전에 수입을 전환 유형으로 하여 세 개의 서로 다른 Adobe Advertising 광고와 상호 작용한다고 가정해 봅시다. Adobe Advertising 보고서가 속성에 대해 고른 배포 모델을 사용하는 경우 모든 광고에서 고르게 매출을 연결합니다. If [!DNL Analytics] 는 마지막 터치 속성 모델을 사용하지만, 매출을 마지막 광고에 귀속시킵니다. 다음 예에서 Adobe Advertising은 세 개의 광고 각각에 캡처된 매출 30USD 중 10USD를 기여합니다. [!DNL Analytics] 사용자가 본 마지막 광고에 대한 매출 30USD의 모든 속성을 표시합니다. Adobe Advertising 및 의 보고서를 비교할 때 [!DNL Analytics], 속성 차이의 영향을 확인할 수 있습니다.

  ![Adobe Advertising 및 로 인한 다양한 수익 [!DNL Analytics] 다양한 속성 모델 기반](/help/integrations/assets/a4adc-attribution-example.png)

>[!IMPORTANT]
>
>가장 좋은 방법은 Adobe Advertising 및 속성 모두에서 동일한 전환 확인 기간 및 속성 모델을 사용하는 것입니다 [!DNL Analytics]. 필요에 따라 Adobe 계정 팀과 협력하여 현재 설정을 식별하고 구성을 동기화하십시오.

이와 동일한 개념은 다른 전환 확인 기간 또는 속성 모델을 사용하는 다른 모든 유사한 채널에도 적용됩니다.

#### 뷰스루 추적을 위한 다양한 전환 확인 기간 {#impression-lookback}

Adobe Advertising에서 속성은 클릭과 노출을 기반으로 하며 클릭과 노출에 대해 다양한 전환 확인 기간을 구성할 수 있습니다. 위치 [!DNL Analytics]하지만 기여도 분석은 클릭스루와 뷰스루를 기반으로 하므로 클릭스루와 뷰스루에 대해 다른 기여도 분석 창을 설정할 수 있는 옵션이 없습니다. 초기 사이트 방문에서 각 시작에 대해 추적합니다. 노출은 뷰스루가 발생하기 전 같은 날 또는 여러 날에 발생할 수 있으며, 이는 각 시스템에서 속성 창이 시작되는 위치에 영향을 줄 수 있습니다.

일반적으로 대부분의 뷰스루 전환은 두 시스템 모두 크레딧을 고려할 만큼 빠르게 발생합니다. 그러나 일부 전환은 Adobe Advertising 노출 전환 확인 기간 외부이지만 [!DNL Analytics] 전환 확인 기간. 이러한 전환은 의 뷰스루에 기인합니다. [!DNL Analytics] 하지만 Adobe Advertising의 인상은 그렇지 않습니다.

다음 예에서는 방문자가 1일에 광고를 제공하고, 2일에 뷰스루 방문(즉, 이전에 광고를 클릭하지 않고 광고의 랜딩 페이지 방문)을 수행하고, 45일에 전환되었다고 가정해 봅시다. 이 경우 Adobe Advertising은 1-14일(14일 전환 확인 사용)부터 사용자를 추적합니다. [!DNL Analytics] 은 근무일 2-61에서 사용자를 추적하며(60일 전환 확인 사용), 45일의 전환은 다음 기간 내의 광고에 귀속됩니다. [!DNL Analytics] Adobe Advertising 내에서는 사용할 수 없습니다.

![에 속하는 뷰스루 전환의 예 [!DNL Analytics] Adobe Advertising 제외](/help/integrations/assets/a4adc-viewthrough-example.png)

불일치의 추가 원인은 Adobe Advertising에서 사용자 지정 뷰스루 변환을 할당할 수 있기 때문입니다 *뷰스루 가중치* 이는 클릭 기반 전환으로 인한 가중치와 관련이 있습니다. 기본 뷰스루 가중치는 40%이며, 이는 뷰스루 변환이 클릭 기반 전환 값의 40%로 계산됨을 의미합니다. [!DNL Analytics] 에서는 뷰스루 전환에 대한 이러한 가중치를 제공하지 않습니다. 예를 들어 100 USD 매출 주문은에서 캡처됩니다. [!DNL Analytics] 기본 뷰스루 가중치(60USD의 차이)를 사용하는 경우 Adobe Advertising에서 40USD로 할인됩니다.

Adobe Advertising과 간의 뷰스루 전환을 비교할 때 다음 차이점을 고려하십시오 [!DNL Analytics] 보고서.

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
>선형 할당의 경우 [!DNL Analytics] 모든 성공 이벤트를 동일하게 속성 지정 [!DNL eVar] 단일 방문 내의 값이므로 [!DNL eVar] &quot;방문&quot;의 만료. 그러나 광고의 경우 선형 기여도 분석을 사용하면 실제로 선형적이지 않고 보다 덜 이상적인 보고에 할당이 발생합니다. 예를 들어 방문자가 세 개의 별도 방문에서 전환하기 전에 세 개의 광고와 상호 작용하는 경우 마지막 방문에서 표시된 광고만 전환에 기여하는 것이며 세 개의 광고 모두가 기여하는 것은 아닙니다.
>
>또한 전환 할당을 &quot;선형&quot;으로 또는 &quot;선형&quot;으로 전환하면 내역 데이터가 표시되지 않으므로 보고서에서 데이터가 잘못 표시될 수 있습니다. 예를 들어 선형 할당은 여러 다른 항목에 걸쳐 매출을 나눌 수 있습니다 [!DNL eVar] 값. 할당을 &quot;가장 최근&quot;으로 변경하면 해당 매출의 100%가 가장 최근 단일 값과 연관됩니다. 이 연관성은 잘못된 결론으로 귀하를 이끌 수 있다.
>
>혼동을 막기 위해 [!DNL Analytics] 보고 인터페이스에서 내역 데이터를 사용할 수 없게 됩니다. 을 변경하면 내역 데이터를 볼 수 있습니다. [!DNL eVar] 변경하지 말아야 하지만 초기 할당 설정으로 돌아갑니다. [!DNL eVar] 할당 설정을 통해 이전 데이터에 액세스할 수 있습니다. Adobe은 새 를 사용할 것을 권장합니다 [!DNL eVar] 에 대한 할당 설정을 변경하는 대신 이미 기록되고 있는 데이터에 새 할당 설정을 적용하려는 경우 [!DNL eVar] 여기에는 이미 상당한 양의 이전 데이터가 있습니다.

목록 보기 [!DNL Analytics] 다음 위치에서 기여도 분석 모델 및 해당 정의 [https://experienceleague.adobe.com/docs/analytics-platform/using/cja-workspace/attribution/models.html](https://experienceleague.adobe.com/docs/analytics-platform/using/cja-workspace/attribution/models.html).

에 로그인한 경우 [!DNL Search, Social, & Commerce], 목록을 찾을 수 있습니다

* (북아메리카의 사용자) [`https://enterprise-na.efrontier.com/CMDashboard/help/external/tracking/r_appendix_-_how_attribution_rules_are_calculated.htm`](https://enterprise-na.efrontier.com/CMDashboard/help/external/tracking/r_appendix_-_how_attribution_rules_are_calculated.htm)

* (다른 모든 사용자) [`https://enterprise-intl.efrontier.com/CMDashboard/help/external/tracking/r_appendix_-_how_attribution_rules_are_calculated.htm`](https://enterprise-intl.efrontier.com/CMDashboard/help/external/tracking/r_appendix_-_how_attribution_rules_are_calculated.htm)

#### Adobe Advertising의 이벤트 날짜 속성

Adobe Advertising에서 연결된 클릭 날짜/이벤트 날짜(클릭 또는 노출 이벤트의 날짜) 또는 트랜잭션 날짜(전환 날짜)별로 전환 데이터를 보고할 수 있습니다. 클릭/이벤트 날짜 보고의 개념이에 없습니다. [!DNL Analytics]; 모든 전환에서 추적됨 [!DNL Analytics] 트랜잭션 날짜별로 보고됩니다. 그 결과, 동일한 전환이 Adobe Advertising 및 의 다른 날짜에 보고될 수 있습니다 [!DNL Analytics]. 예를 들어, 1월 1일에 광고를 클릭하고 1월 5일에 전환하는 사용자가 있다고 가정해 보겠습니다. Adobe Advertising에서 이벤트 날짜별 전환 데이터를 보고 있는 경우 클릭이 발생한 1월 1일에 전환이 보고됩니다. 위치 [!DNL Analytics], 동일한 전환이 1월 5일에 보고됩니다.

![다른 날짜에 속하는 전환의 예](/help/integrations/assets/a4adc-conversions-based-on.png)

## 의 속성 [!DNL Analytics Marketing Channels]

[[!DNL Analytics Marketing Channels] 보고](https://experienceleague.adobe.com/docs/analytics/components/marketing-channels/analyze-mc.html) 히트 정보의 고유한 측면을 기반으로 다양한 마케팅 채널을 식별하는 규칙을 구성할 수 있습니다. Adobe Advertising 추적 채널([!UICONTROL Display Click Through], [!UICONTROL Display View Through], 및 [!UICONTROL Paid Search]) as [!DNL Marketing Channels] 를 사용하여 `ef_id` 채널을 식별하기 위한 쿼리 문자열 매개 변수입니다. <!-- Move most of the above text to "Marketing Channels" chapter once it's created, and add link here. --> 하지만 [!DNL Marketing Channels] 보고서는 Adobe Advertising 채널을 추적할 수 있으며, 여러 가지 이유로 데이터가 Adobe Advertising 보고서와 일치하지 않을 수 있습니다. 자세한 내용은 다음 섹션을 참조하십시오.

>[!NOTE]
>
> 다음 핵심 개념은 다음과 같이 Adobe Advertising에서 추적되지 않는 캠페인과 관련된 모든 다중 채널 추적에도 적용됩니다. [`campaign`](https://experienceleague.adobe.com/docs/analytics/implementation/vars/page-vars/campaign.html) 변수(&quot;추적 코드&quot; 차원 또는 &quot;라고도 함)[!DNL eVar] 0&quot;) 및 사용자 지정 [!DNL eVar] 추적.

### 에서 잠재적으로 다른 속성 모델 [!DNL Marketing Channels]

가장 [!DNL Marketing Channels] 보고서는 [!UICONTROL Last Touch] 마지막으로 감지된 마케팅 채널에 전환 값의 100%가 지정되는 속성. 에 대해 다양한 속성 모델 사용 [!DNL Marketing Channels] 보고서와 Adobe Advertising 보고서는 속성 전환의 불일치를 초래합니다.

### 의 잠재적으로 다른 전환 확인 기간 [!DNL Marketing Channels]

에 대한 전환 확인 기간 [!DNL Marketing Channels] 을 사용자 지정할 수 있습니다. 고정된 60일 기간이 일반적이지만 Adobe Advertising에서 전환 확인 기간을 구성할 수 있습니다. 두 제품이 서로 다른 전환 확인 기간을 사용하는 경우 데이터 불일치가 발생할 수 있습니다.

### 의 다른 채널 속성 [!DNL Marketing Channels]

Adobe Advertising 보고서는 Adobe Advertising을 통해 거래되는 유료 미디어만 캡처합니다(유료 검색 대상 [!DNL Advertising Search, Social, & Commerce] 광고 및 Advertising DSP 광고용 디스플레이), [!DNL Marketing Channels] 보고서는 모든 디지털 채널을 추적할 수 있습니다. 이로 인해 전환이 속하는 채널이 불일치할 수 있습니다.

예를 들어 유료 검색과 자연어 검색 채널은 각 채널이 상대방을 돕는 공생 관계를 맺는 경우가 많다. 다음 [!DNL Marketing Channels] 보고서는 자연어 검색을 추적하지 않으므로 Adobe Advertising이 전환하지 않는 자연어 검색에 일부 전환을 사용합니다.

디스플레이 광고를 보고, 유료 검색 광고를 클릭하고, 이메일 메시지 내부를 클릭한 다음, 30 USD 주문을 하는 고객도 생각해 보십시오. Adobe Advertising 및 [!DNL Marketing Channels] 두 가지 모두 마지막 터치 속성 모델을 사용하므로 전환은 여전히 각각에 대해 다르게 분류됩니다. Adobe Advertising에게 다음에 대한 액세스 권한이 없습니다. [!UICONTROL Email] 채널에 포함되므로 전환에 대해 유료 검색을 크레딧합니다. [!DNL Marketing Channels]하지만 은 세 채널 모두에 액세스할 수 있으므로 크레딧이 제공됩니다 [!UICONTROL Email] 변환용.

![Adobe Advertising의 다양한 전환 속성 예 [!DNL Analytics Marketing Channels]](/help/integrations/assets/a4adc-channel-example.png)

지표가 달라질 수 있는 이유에 대한 자세한 내용은 &quot;[Adobe Advertising과 간에 채널 데이터가 다를 수 있는 이유 [!DNL Marketing Channels]](marketing-channels/mc-data-variances.md).&quot;

## Adobe Analytics의 데이터 차이점 [!DNL Paid Search Detection]

다음 [legacy [!DNL Paid Search Detection]](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/manage-report-suites/edit-report-suite/report-suite-general/paid-search-detection/paid-search-detection.html) 의 기능 [!DNL Analytics] 회사가 다음을 수행할 수 있도록 허용 [유료 및 유기 검색 트래픽을 추적하는 규칙 정의](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/paid-search-detection/t-paid-search-detection.html) 지정된 검색 엔진의 경우. 다음 [!DNL Paid Search Detection] 규칙은 쿼리 문자열과 참조 도메인을 모두 사용하여 유료 및 자연어 검색 트래픽을 식별합니다. 다음 [!DNL Paid Search Detection] 보고서는 다음 중 큰 그룹의 일부입니다. [검색 방법](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/finding-methods.html) 보고서: 지정된 이벤트(예: 장바구니 체크아웃)가 발생하거나 방문이 종료될 때 만료됩니다.

다음은 를 만들기 위한 인터페이스입니다 [!DNL Paid Search Detection] 규칙 집합:

![에 설정된 유료 검색 감지 규칙의 예 [!DNL Analytics]](/help/integrations/assets/a4adc-paid-search-detection.png)

결과 [!DNL Paid Search Detection] 보고서에는 [!UICONTROL Paid Search Engine], [!UICONTROL Paid Search Keywords], [!UICONTROL Natural Search Engine], 및 [!UICONTROL Natural Search Keywords] 보고서.

의 데이터에 대한 다음 두 가지 제한 사항을 참고하십시오 [!DNL Paid Search Detection] 보고서:

* 다음 [!UICONTROL Paid Search Keywords] 및 [!UICONTROL Natural Search Keywords] 보고서는 사용자가 입찰한 키워드가 아니라 참조 URL로 식별된 검색 쿼리를 표시합니다. Adobe Advertising 및 [!DNL Analytics] 보고서는 실제 키워드를 표시하므로 키워드를 [!DNL Paid Search Detection] 키워드 보고서.

* 다음의 경우 [!DNL Paid Search Detection] 원래 기능이 만들어졌으므로 참조 URL을 통해 광고주는 원래 검색 쿼리(사용자가 검색 엔진의 검색 막대에 입력한 문자 문자열)를 보다 쉽게 사용할 수 있었습니다. 현재 검색 엔진은 주로 검색 쿼리를 난독화하고 [!DNL Paid Search Detection] 대부분의 쿼리 데이터가 &quot;지정되지 않음&quot;에 해당하기 때문에 키워드 보고서는 제한된 값입니다.

  포함 [!DNL Analytics for Advertising], 광고주는 여전히 의 유료 키워드를 추적할 수 있습니다. [!DNL Analytics]. 참조 도메인은 트래픽을 유도한 검색 엔진을 엔진에 보고합니다. 광고주별 계정 정보가 참조 도메인에 연결되어 있지 않으므로 모든 트래픽이 검색 엔진 아래에 나열됩니다. 동일한 검색 엔진에 여러 개의 계정이 있는 광고주는 Adobe Advertising 또는 [!DNL Analytics] 계정별 보고에 대한 보고입니다.

### 구성 이유 [!DNL Paid Search Detection]?

다음 [!DNL Paid Search Detection] 보고서를 사용하면 의 자연어 검색 트래픽을 [[!DNL Analytics Marketing Channels] 보고서](https://experienceleague.adobe.com/docs/analytics/components/marketing-channels/analyze-mc.html). 유료 검색 트래픽과 자연어 검색 트래픽을 구분하는 것은 자연어 검색이 전체 마케팅 생태계에 가져오는 가치를 이해하는 좋은 방법입니다.

## 클릭스루 데이터 유효성 검사 [!DNL Analytics for Advertising] {#data-validation}

통합하려면 클릭스루 데이터의 유효성을 검사하여 사이트의 모든 페이지가 클릭스루를 제대로 추적하는지 확인해야 합니다.

위치 [!DNL Analytics]를 검색하는 가장 쉬운 방법 중 하나 [!DNL Analytics for Advertising] 추적은 &quot;클릭 수&quot;를 사용하여 클릭 수를 인스턴스와 비교하는 것입니다. [!UICONTROL AMO ID Instances]&quot;계산된 지표: 다음과 같이 계산됩니다.

```
Clicks to [!UICONTROL AMO ID Instances] = ([!UICONTROL AMO ID Instances] / Adobe Advertising Clicks)
```

[!UICONTROL AMO ID Instances] 다음 횟수를 나타냅니다. [AMO ID](ids.md) 사이트에서 추적됩니다. 광고를 클릭할 때마다 AMO ID(`s_kwcid`) 매개 변수가 랜딩 페이지 URL에 추가됩니다. 의 수 [!UICONTROL AMO ID Instances]따라서 는 클릭 수와 유사하며 실제 광고 클릭에 대해 확인할 수 있습니다. 에 대해 일반적으로 80%의 일치율이 표시됩니다. [!DNL Search, Social, & Commerce] 및 30%의 일치율 [!DNL DSP] 트래픽(클릭스루만 포함하도록 필터링될 때) [!UICONTROL AMO ID Instances]). 검색과 표시 간의 기대치 차이는 예상되는 트래픽 행태로 설명될 수 있다. 검색은 인텐트를 캡처하며, 따라서 사용자는 일반적으로 쿼리에서 검색 결과를 클릭하려고 합니다. 그러나 디스플레이 또는 온라인 비디오 광고를 보는 사용자는 의도하지 않게 광고를 클릭한 다음 사이트에서 바운스되거나 페이지 활동이 추적되기 전에 로드되는 새 창을 포기할 가능성이 높습니다.

Adobe Advertising 보고서에서 &quot;&quot;를 사용하여 클릭 수를 인스턴스와 유사하게 비교할 수 있습니다.[!UICONTROL ef_id_instances]대신 &quot;지표 [!UICONTROL AMO ID Instances]:

```
Clicks to [EF ID Instances = (ef_id_instances / Clicks)
```

AMO ID와 EF ID 간의 높은 일치율을 예상해야 하지만, AMO ID와 EF ID는 근본적으로 다른 데이터를 추적하므로 100% 패리티를 예상하지 마십시오. 이러한 차이는 합계에 약간의 차이를 초래할 수 있습니다 [!UICONTROL AMO ID Instances] 및 [!UICONTROL EF ID Instances]. 합계인 경우 [!UICONTROL AMO ID Instances] 위치: [!DNL Analytics] 다음과 다름: [!UICONTROL EF ID Instances] 그러나 1% 이상 Adobe Advertising 시 도움이 필요하면 Adobe 계정 팀에 문의하십시오.

AMO ID 및 EF ID에 대한 자세한 내용은 [Analytics에서 사용하는 Adobe Advertising ID](ids.md).

다음은 인스턴스 클릭을 추적하는 작업 영역의 예입니다.

![인스턴스 클릭을 추적하는 작업 영역의 예](/help/integrations/assets/a4adc-clicks-to-instances-example.png)

## 의 데이터 세트 비교 [!DNL Analytics for Advertising] 및 Adobe Advertising

다음 [AMO ID](ids.md) (s_kwcid 쿼리 문자열 매개 변수)가에서 보고에 사용됩니다. [!DNL Analytics]및 [EF ID](ids.md) Adobe Advertising 보고에 사용됩니다. 고유한 값이므로 하나의 값이 랜딩 페이지에 손상되거나 추가되지 않을 수 있습니다.

예를 들어 다음과 같은 랜딩 페이지가 있다고 가정합니다.

```
www.adobe.com/?ef_id=test_ef_id&s_kwcid=test_amo_id
```

여기서 EF ID는 &quot;`test_ef_id`&quot;및 AMO ID는 &quot;`test_amo_id`.&quot;

사이트 측 리디렉션이 발생하면 URL은 다음과 같이 종료될 수 있습니다.

```
www.adobe.com/?ef_id=test_ef_id&s_kwcid=test_amo_id#redirectAnchorTag
```

여기서 EF ID는 &quot;`test_ef_id`&quot;및 AMO ID는 &quot;`test_amo_id#redirectAnchorTag`.&quot;

이 예에서 앵커 태그를 추가하면 AMO ID에 예기치 않은 문자가 추가되어 Analytics에서 인식하지 못하는 값이 발생합니다. 이 AMO ID는 분류되지 않으며 이 ID와 연결된 전환은 &quot;[!UICONTROL unspecified]&quot; 또는 &quot;[!UICONTROL none]&quot; 위치 [!DNL Analytics] 보고서.

다행히도, 이와 같은 문제들이 일반적이지만, 일반적으로 높은 비율의 불일치는 발생하지 않습니다. 그러나 의 AMO ID 간에 큰 차이가 발생하는 경우 [!DNL Analytics] 및 Adobe Advertising의 EF ID에 대한 지원은 Adobe 계정 팀에 문의하십시오.

## 기타 지표 고려 사항

### 클릭과 방문의 차이점 {#clicks-vs-visits}

유사해 보이지만 클릭과 방문은 서로 다른 데이터를 나타냅니다.

* **클릭:** [!DNL DSP] 또는 검색 엔진은 방문자가 게시자의 웹 사이트에서 광고를 클릭할 때 클릭을 기록합니다.

* **방문:** [!DNL Analytics] 다음을 정의합니다. [방문](https://experienceleague.adobe.com/docs/analytics/components/metrics/visits.html) 30분 동안 활동이 없는 경우와 같은 여러 기준 중 하나에 따라 종료되는 사용자의 일련의 페이지 보기입니다.

정의에 따라 클릭으로 여러 번의 방문이 발생할 수 있습니다.

사용자 1과 사용자 2는 모두 Adobe Advertising 광고를 클릭하여 사이트에 액세스합니다. 사용자 1은 4개의 페이지를 본 다음 하루 동안 이동하므로 처음 클릭할 때 방문이 한 번 발생합니다. 사용자 2는 2페이지를 보고, 45분 점심을 먹고, 돌아가기, 2페이지를 더 보고 나가기, 이 경우 처음 클릭하면 2번의 방문이 발생합니다.

![클릭과 방문 간의 차이점 예](/help/integrations/assets/a4adc-visits-example.png)

### 클릭스루와 클릭스루의 차이점

<!-- Rob to let me know if we should remove this and add more info. to the section on AMO Instances etc. -->

클릭과 클릭스루는 두 가지 다른 지표입니다.

* **클릭:** [!DNL DSP] 또는 검색 엔진은 방문자가 게시자의 웹 사이트에서 광고를 클릭할 때 클릭을 기록합니다.

* **클릭스루:** [!DNL Analytics] 방문자가 대상 웹 사이트에 도달하고, 랜딩 페이지가 로드되고, [!DNL Analytics] 페이지 하단의 요청은 데이터를으로 전송합니다. [!DNL Analytics].

우발적 광고 클릭으로 인해 클릭과 클릭스루가 크게 다를 수 있습니다. 디스플레이 광고의 대부분의 클릭은 우발적 클릭이며 이러한 우발적 방문자가 랜딩 페이지가 로드되기 전에 [뒤로] 버튼을 누르는 것을 관찰했습니다. [!DNL Analytics] 클릭스루를 기록할 수 없습니다. 이는 모바일 광고, 비디오 광고 및 화면을 채우고 사용자가 페이지를 보기 전에 닫아야 하는 광고와 같이 실수로 클릭할 가능성이 높은 광고에 특히 해당됩니다.

또한 모바일 디바이스에 로드된 사이트는 낮은 대역폭이나 사용 가능한 처리 능력 때문에 클릭스루가 발생할 가능성이 낮으므로 랜딩 페이지를 로드하는 데 더 오래 걸립니다. 클릭 수의 50~70%가 클릭스루로 이어지지 않는 일은 드물지 않습니다. 모바일 환경에서는 브라우저가 느리고 사용자가 페이지를 스크롤하거나 광고를 닫으려고 하는 동안 실수로 광고를 클릭할 가능성이 높기 때문에 차이가 90%까지 클 수 있습니다.

클릭 데이터는 현재 추적 메커니즘(예: 모바일 앱으로 들어가는 클릭 수 또는 모바일 앱으로부터의 클릭 수)으로 클릭스루를 기록할 수 없거나 광고주가 하나의 추적 접근 방식만 배포한 환경에 기록될 수 있습니다(예: 뷰스루 JavaScript 접근 방식을 사용할 경우 서드파티 쿠키를 차단하는 브라우저는 클릭스루가 아닌 클릭 수를 추적합니다). Adobe에서 클릭 URL 추적 및 뷰스루 JavaScript 추적 접근 방식을 모두 배포하도록 권장하는 주요 이유는 추적 가능한 클릭스루의 범위를 최대화하기 위해서입니다.

### 비 Adobe Advertising Dimension에 대한 Adobe Advertising 트래픽 지표 사용

Adobe Advertising은 Analytics에 [광고 특정 트래픽 지표 및 관련 차원 [!DNL DSP] 및 [!DNL Search, Social, & Commerce]](advertising-metrics-in-analytics.md). Adobe Advertising이 제공한 지표는 지정된 Adobe Advertising 차원에만 적용할 수 있고 의 다른 차원에는 데이터를 사용할 수 없습니다. [!DNL Analytics].

예를 들어 [!UICONTROL Adobe Advertising Clicks] 및 [!UICONTROL Adobe Advertising Cost] 계정별 지표: Adobe Advertising 차원으로서, 합계 [!UICONTROL Adobe Advertising Clicks] 및 [!UICONTROL Adobe Advertising Cost] 계정별.

![Adobe Advertising 차원을 사용한 보고서의 Adobe Advertising 지표 예](/help/integrations/assets/a4adc-traffic-supported-dimension.png)

그러나 를 보는 경우에는 [!UICONTROL Adobe Advertising Clicks] 및 [!UICONTROL Adobe Advertising Cost] Adobe Advertising이 데이터를 제공하지 않는 페이지 내 차원(예: 페이지)별 지표 [!UICONTROL Adobe Advertising Clicks] 및 [!UICONTROL Adobe Advertising Cost] 각 페이지의 값은 0이 됩니다.

![지원되지 않는 차원을 사용하는 보고서의 Adobe Advertising 지표의 예](/help/integrations/assets/a4adc-traffic-unsupported-dimension.png)

### 사용 [!UICONTROL AMO ID Instances] Adobe Advertising이 아닌 Dimension을 사용한 클릭 대용

를 사용할 수 없기 때문에 [!UICONTROL Adobe Advertising Clicks] 온사이트 차원을 사용하면 클릭과 동일한 값을 찾을 수 있습니다. 방문 횟수를 대체품으로 사용하고 싶을 수 있지만 각 방문자에게 여러 번의 방문이 있을 수 있으므로 방문 횟수는 최선의 옵션이 아닙니다. ( &quot; 참조[클릭과 방문의 차이점](#clicks-vs-visits).&quot; 대신 을 사용하는 것이 좋습니다. [!UICONTROL AMO ID Instances]: AMO ID가 캡처된 횟수입니다. While [!UICONTROL AMO ID Instances] 일치하지 않음 [!UICONTROL Adobe Advertising Clicks] 맞습니다. 사이트에서의 클릭 트래픽을 측정하는 데 가장 적합한 옵션입니다. 자세한 내용은 &quot;[데이터 유효성 검사 [!DNL Analytics for Advertising]](#data-validation).&quot;

![예 [!UICONTROL AMO ID Instances] 대신 [!UICONTROL Adobe Advertising Clicks] 지원되지 않는 차원의 경우](/help/integrations/assets/a4adc-amo-id-instances.png)

>[!MORELIKETHIS]
>
>* [개요 [!DNL Analytics for Advertising]](overview.md)
>* [사용한 Adobe Advertising ID [!DNL Analytics]](/help/integrations/analytics/ids.md)
>* [Analysis Workspace에서 지표 Adobe Advertising](/help/integrations/analytics/advertising-metrics-in-analytics.md)
>* [[!DNL Analytics] Adobe Advertising의 데이터](/help/integrations/analytics/analytics-data-in-advertising.md)
>* [Adobe Advertising과 간에 데이터가 다를 수 있는 이유 [!DNL Marketing Channels]](/help/integrations/analytics/marketing-channels/mc-data-variances.md)
