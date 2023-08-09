---
title: 사용자 정의 보고서에 대한 FAQ
description: 데이터 문제 해결을 포함하여 성능 보고서에 대한 일반적인 질문에 대한 답변을 살펴볼 수 있습니다.
exl-id: 85707666-7c0f-4aa3-8c91-fb73ef6a5061
feature: Search Reports
source-git-commit: 2903bf783969b3e2d59c0933629cbb170c0a314c
workflow-type: tm+mt
source-wordcount: '3912'
ht-degree: 0%

---

# 사용자 정의 보고서에 대한 FAQ

## 일반 질문

+++보고서 데이터를 사용할 수 있기 전에 보고서의 날짜 범위가 시작되면 어떻게 합니까?
보고서가 생성되지만 데이터를 사용할 수 있는 날짜에 대한 데이터만 포함됩니다. 각 보고서 유형에 데이터를 사용할 수 있는 시기에 대한 자세한 내용은 &quot;[보고서에 사용된 데이터](data-used-for-reports.md).&quot;
+++

+++클릭 날짜 및 거래 날짜 기반 보고서 간의 차이점은 무엇입니까?
트랜잭션 일자별 전환을 보고할 때 데이터는 지정된 기간 동안 트랜잭션 일자가 발생한 트랜잭션을 포함합니다. 이 옵션은 기본 보고서 및 고급 보고서의 기본 설정이며 지정된 기간 내에 얻은 매출액을 보여 줍니다.

클릭 날짜별 전환을 보고할 때 데이터에는 지정된 기간 동안 발생한 클릭으로 인한 트랜잭션이 포함됩니다. 포트폴리오에 클릭과 거래 사이에 상당한 지연이 있는 경우 이 유형의 보고는 포트폴리오에 대한 클릭당 과거 수익을 보여주며, 이를 통해 시간에 따라 예상되는 수익 행동에 대해 파악할 수 있습니다.

![클릭 날짜별 보고와 트랜잭션 날짜별 보고](/help/search-social-commerce/assets/click-date-vs-txn-date.png "클릭 날짜별 보고와 트랜잭션 날짜별 보고")
+++

+++클릭 전환 확인 기간 또는 노출 전환 확인 기간을 변경하면 어떻게 됩니까?
(광고 픽셀 기반 전환 추적 서비스 전용 광고주) 초기 클릭으로 인해 발생하는 이벤트의 데이터가 더 길거나 더 짧은 기간 동안 수집됩니다.

광고주 [전환 확인 기간 클릭](/help/search-social-commerce/glossary.md#c-d) 및 [노출 전환 확인 기간](/help/search-social-commerce/glossary.md#i-j) 전환으로 이벤트가 귀속될 수 있는 유료 클릭 또는 디스플레이 노출(각각) 발생 후 일 수를 결정합니다. 값을 더 길거나 더 짧은 기간으로 변경하는 것은 특히 짧은 또는 긴 클릭-수익 또는 디스플레이 노출-수익 기간이 있는 광고주에게 중요할 수 있습니다.

**모범 사례:** 전환 확인 기간이 클릭하여 수익을 얻는 기간보다 길어야 하며 대부분의 키워드나 광고에 대해 노출 시간부터 수익을 얻는 시간을 표시해야 합니다. 더 짧은 경우 일부 전환은 초기 클릭 또는 노출과 연결되지 않습니다.
+++

+++에서 전환된 결과를 어떻게 알 수 있습니까? [!DNL Google Ads] 광고 확장 또는 제품 목록
을(를) 클릭하여 전환된 을(를) 확인할 수 있습니다. [!DNL Google Ads] 광고 확장(광고 자체가 아님) 또는 를 생성하여 제품 목록에 추가 [!UICONTROL Transaction Report]. 다음 [!UICONTROL Link Type] 열 값은 클릭한 링크의 유형 및 제목을 표시합니다.

* 제품 목록은 다음과 같습니다. `pla:<product ID>`, 예: `pla:8525822`.

* 사이트 링크는 다음과 같이 나열됩니다. `sl:<Sitelink text>`, 예: `sl:See Current Offers`.

  다음을 포함하는 경우 사이트 링크를 식별할 수도 있습니다. [!UICONTROL Tracking URL] 열. 다음 [!UICONTROL Tracking URL] 사이트링크의 경우 속성 포함 `&ev_ltx=sl:<link-name>`.

>[!NOTE]
>
>다음에서 전환: [!DNL Google Ads] 위치 및 전화 확장 기능은 함께 제공되는 광고의 데이터에 포함됩니다. 별도로 보고되지 않습니다.

+++

+++더 &quot;[!UICONTROL Keyword]내 보고서의 &quot;열에 값 &quot;(광고 그룹 컨텐츠) &lt;*광고 그룹 이름*>.&quot;
행에 키워드가 포함되지 않은 콘텐츠 활성화 검색 캠페인, 디스플레이 캠페인 또는 소셜 캠페인에 대한 데이터가 포함되는 경우 [!UICONTROL Keyword] 열은 적용 가능한 광고 그룹 이름을 대신 표시합니다.
+++

+++계절적 또는 시장 변화로 인해 내 보고서에는 비정형 데이터가 표시됩니다. 조건이 변경되면 입찰에 영향을 줍니까?
최적화 기능은 각 입찰 단위에 대한 매출 모델을 매일 구축하여 트렌드를 식별하고 즉시 응답하도록 하며, 모델은 장기 내역 데이터를 통합하여 시즌 성과를 예측하는 데 도움이 됩니다. 포트폴리오의 수익 모델 반감기 설정<!-- add link to glossary? --> 또한 최근 매출 데이터에 가중치가 얼마나 많이 적용되는지도 결정합니다. 비정형 성과 기간에는 반감기를 낮추되 수익 모델을 조정한 후 늘리는 것이 가장 좋습니다. 반감기 조정이 필요한지 여부에 대한 질문이 있는 경우 Adobe 계정 팀에 문의하십시오.

기간 동안의 데이터가 향후 입찰에 전혀 영향을 주지 않도록 하려면 해당 날짜를 모델에서 제외하도록 선택할 수 있습니다. 날짜를 제외하려면 Adobe 계정 팀에 문의하십시오.
+++

+++다음과 같은 특정 계정 속성 지표에 대한 보고서를 만들 수 있습니까? [!UICONTROL Device] 또는 [!UICONTROL Objective Name]?
캠페인 엔티티 보고서용([!UICONTROL Campaign Report], [!UICONTROL Ad Group Report], [!UICONTROL Ad Variation Report], [!UICONTROL Keyword Report], 및 [!UICONTROL Product Group Report]) 지표 데이터는 보고서에 포함하는 속성 열에 의해 동적으로 집계됩니다. 선택적으로 보고서에 대한 키 열을 제거하고 데이터를 집계할 속성 열만 포함할 수 있습니다.

예를 들어 [!UICONTROL Keyword Report] 다음을 포함합니다. [!UICONTROL Ad Group] 및  장치 열을 선택한 다음 기본적으로 보고서는 광고 그룹 및 장치 유형별로 각 키워드에 대한 지표를 집계합니다. 그러나 를 제거하면 [!UICONTROL Keyword] 열보고서를 생성하기 전에 보고서가 지정된 광고 그룹에 대한 지표를 장치 유형별로 동적으로 생성합니다.

>[!NOTE]
>
>이 기능을 사용하여 레이블 분류별로 데이터를 집계할 수 없습니다. 보고서의 레이블 분류 열은 모두 생략됩니다. 대신 [레이블 분류 보고서](/help/search-social-commerce/reports/management/basic-advanced/label-classification-report.md).

+++

## 일반 데이터 문제

+++다른 속성 규칙을 사용하여 생성된 보고서에는 다른 합계가 표시됩니다.
동일한 보고서 매개변수를 사용하지만 속성 규칙이 다른 보고서를 여러 번 생성하는 경우 다음 이유 중 하나로 데이터가 다를 수 있습니다.

* 클릭 날짜 기반 데이터가 지정된 날짜 범위를 벗어날 수 있습니다.

  보고서 매개 변수 &quot;를 사용하는 경우[!UICONTROL Conversions based on click date],&quot; 그러면 지정된 날짜 범위가 트랜잭션 날짜 대신 클릭 날짜에 적용됩니다. 또한 보고서에서 속성 규칙 &quot;첫 번째 이벤트&quot; 또는 &quot;마지막 이벤트&quot;를 사용하는 경우 전환을 초래한 첫 번째 또는 마지막 이벤트가 지정된 날짜 범위를 벗어날 수 있습니다. 예를 들어 사용자가 4월 30일에 Keyword_1을 클릭하고 5월 20일에 Keyword_2를 클릭한 다음 5월 21일에 전환되었다고 가정해 보십시오. 보고서에서 &quot;를 사용하는 경우[!UICONTROL First Event]&quot;속성 규칙과 날짜 범위가 5월 1일부터 21일까지인 경우 첫 번째 이벤트(4월 30일에 Keyword_1 클릭)는 보고서에 포함되지 않습니다. 동일한 날짜 범위로 보고서를 실행하지만[!UICONTROL Last Event]&quot;속성 규칙, 그러면 마지막 클릭이 지정된 날짜 범위 내에서 발생했으므로 전환이 보고서에 포함됩니다.

* 포트폴리오 필터 선택 사항에서는 전환으로 이어지는 일부 이벤트가 제외됩니다.

  포트폴리오의 하위 집합에 대해 보고하는 경우 속성 규칙 중 하나에 전환이 귀속된 이벤트를 포함한 캠페인을 포함하지 않을 수 있습니다. 예를 들어 사용자가 Keyword_1에서 Portfolio_1을 클릭하고 Portfolio_2에서 키워드_2를 클릭한 다음 를 변환한다고 가정해 봅시다. 보고서에서 &quot;를 사용하는 경우[!UICONTROL First Event]&quot;속성 규칙을 설정한 경우 전환에 대한 Portfolio_1이 보고서에 포함되어야 합니다. 그러나 보고서에서 &quot;마지막 이벤트&quot; 속성 규칙을 사용하는 경우 Portfolio_2를 포함해야 합니다.

>[!TIP]
>
>다른 속성 규칙에서 전환 합계를 비교하려면 보고서 매개 변수 를 사용하여 보고서를 실행합니다.[!UICONTROL Conversions based on transaction date]&quot;모든 광고 네트워크 또는 모든 포트폴리오를 선택합니다. 다른 필터를 설정하지 않으면 전환 합계가 일치해야 합니다.

+++

+++합계가 정확하지만 개별 데이터 필드가 올바르지 않습니다.
이 상황은 지표 형식이 정수를 사용할 때 발생할 수 있습니다.

* 다음을 만드는 경우 [사용자 지정 지표](/help/search-social-commerce/common-tasks/custom-metrics/custom-metric-about.md) 형식 사용 *소수점 포함 숫자* (데이터를 정수로 표시) 가중 전환 속성 규칙 을 사용하는 보기 또는 보고서에 포함합니다.[!UICONTROL Weight First Event More], [!UICONTROL Weight Last Event More], 또는 [!UICONTROL Even Distribution])를 입력하면 결과는 소수가 아닌 정수로 표시됩니다. 이 경우 합계가 정확하지만 개별 데이터 필드가 올바르지 않을 수 있습니다. 예를 들어, 순서가 세 이벤트 간에 균등하게 나누어지면 한 개의 순서 (0.33 순서 대신)가 세 이벤트 각각에 기여됩니다. 문제를 해결하려면 [지표 형식 변경](/help/search-social-commerce/common-tasks/custom-metrics/custom-metric-edit.md) 끝 *소수점 이하 2자리수*.

* 마찬가지로 정수로 전송되는 매출 지표가 있는 경우 동일한 문제가 발생합니다. 매출 형식은 데이터를 제출하는 전환 태그에 의해 제어됩니다. 문제를 해결하려면 [사용자 지정 지표 만들기](/help/search-social-commerce/common-tasks/custom-metrics/custom-metric-create.md) 매출 지표로만 구성되고 형식을 갖춘 것 *소수점 이하 2자리수*원래 지표가 아닌 보기 및 보고서에 포함할 수 있습니다.
+++

+++클릭 또는 매출 데이터가 누락되면 이후 입찰에 영향을 주지 않도록 하려면 어떻게 해야 합니까?
검색, 소셜 및 상거래가 광고 네트워크와 동기화되지 않을 때 클릭 데이터 문제가 발생합니다. 계정을 수동으로 동기화하려면 Adobe 계정 팀에 문의하십시오. 하루 동안 클릭 데이터가 누락된 경우 Adobe 계정 팀에 비용 모델에서 해당 날짜를 제외하도록 요청하십시오.

매출 데이터 문제는 추적 또는 피드 파일 문제로 인해 발생할 수 있습니다. 문제를 조사하려면 Adobe 계정 팀에 문의하십시오. 하루 전체에 대한 수입 데이터가 누락된 경우 Adobe 계정 팀에 해당 날을 수입 모델에서 제외하도록 요청하십시오.
+++

+++통화 데이터가 잘못된 형식으로 표시됩니다.
기본적으로 보고서의 모든 통화 데이터는 미국 달러(예: 1,000.00) 형식으로 표시됩니다. 값을 올바른 통화 형식으로 표시하려면(CSV 및 TSV 형식의 통화 기호는 제외), &quot;[!UICONTROL Currency]&quot;열을 보고서에 추가합니다. 보고서에 통화가 다른 계정에 대한 데이터가 포함되어 있으면[!UICONTROL Total]&quot;통화 가치는 통화에 관계없이 열에 있는 모든 숫자의 합계입니다.
+++

+++자연수(1, 2 등)여야 하는 전환 지표에 대한 10진수 값이 표시되는 이유는 무엇입니까?
다음과 같은 경우 십진수 값을 볼 수 있습니다.

* 전환 속성 규칙 매개 변수를 사용하여 보고서를 실행한 경우 [!UICONTROL Last Event] 또는 [!UICONTROL First Event]를 설정하는 경우 전환 경로의 여러 이벤트 간에 매출을 분할할 수 있습니다.

* 다음에서 [!UICONTROL Transaction Report], 여러 개인 경우 [입찰 단위](/help/search-social-commerce/glossary.md#a-b) 서로 다른 일치 유형에서 동일한 거래 ID를 사용하면 추적 ID에 대한 수익이 지정된 클릭 날짜의 클릭 수에 따라 분할됩니다.
+++

## 표준 성능 지표

+++클릭 데이터가 보고서에서 누락되었습니다.
다음은 클릭 데이터가 없는 일반적인 이유입니다.

| 원인 | 감지/분석 | 해결 방법 |
|---|---|---|
| 광고 계정에서 클릭 데이터를 검색하는 프로세스가 실패했습니다. | 이 문제를 감지하는 체계적인 방법은 없지만, 광고 계정에서 비용을 사용했음에도 불구하고 캠페인에 비용이 표시되지 않거나 클릭 정보가 표시되지 않을 수 있습니다. | Adobe 계정 팀에 문의하십시오.<br><br>데이터가 24시간 이상 누락된 경우 데이터를 검색할 때까지 비용 예측에서 해당 일자를 제외합니다. Adobe 계정 팀에서 날짜를 제외할 수 있습니다. |
| 광고주와 광고 네트워크 사이의 과금 문제로 인해 광고 계정이 지출되지 않습니다. | 이 문제를 감지하는 체계적인 방법은 없지만, 캠페인에 비용이나 클릭 정보가 표시되지 않을 수 있습니다. | 청구 문제로 인해 광고 계정을 사용할 수 없었던 것을 알고 있는 경우 비용 예측에서 해당 날짜를 제외하십시오. Adobe 계정 팀에서 날짜를 제외할 수 있습니다. |
+++

+++성능 데이터가 광고 네트워크 편집기의 데이터와 다릅니다.
광고 네트워크에서 이전 데이터에 대한 업데이트를 보낼 때(종종 일부 클릭에 클릭 사기를 원인으로 사용함) 검색, 소셜 및 상거래는 5% 이상의 불일치가 없고 Adobe 계정 팀이 요청을 제출하지 않는 한 데이터를 업데이트하지 않습니다.

또한 날짜 범위 간에 집계된 노출 공유 데이터를 비교할 때 검색, 소셜 및 상거래에 대해 보고하는 데이터는 광고 네트워크에서 보고하는 데이터와 다를 수 있습니다. 이 차이는 검색, 소셜 및 상거래에 의해 데이터를 가져오는 데 사용되는 광고 네트워크의 API에서 데이터가 보고되는 방식 때문입니다. 예를 들어 [!DNL Google Ads] 데이터:

* 대부분의 노출 공유 지표의 경우 [!DNL Google Ads] 10% 미만 또는 90%보다 큰 값에 대해 보고된 값의 하한 또는 상한을 제한합니다. 데이터는 &lt;10%의 경우 0.0999, >90%의 경우 0.9001로 보고됩니다

* 날짜 범위 내에 제한되고 제한되지 않은 데이터가 혼합되어 있는 경우 검색, 소셜 및 상거래 집계는 API에서 그대로 전송된 값을 사용하여 데이터를 공유합니다. 10% 미만이 포함된 행의 경우 0.0999, 90% 이상이 포함된 행의 경우 0.9001을 사용합니다. 이 집계로 인해 의 분산이 발생할 수 있습니다. [!DNL Google Ads] 다음 이유로 인해 미리 집계된 데이터 [!DNL Google Ads] 7% 또는 97%와 같은 실제 백분율 값을 사용할 수 있습니다.
+++

+++보고서의 성능 데이터가 의 데이터와 다름 [!DNL Google Analytics].
두 시스템은 서로 다른 데이터를 측정하므로 서로 다른 데이터를 볼 수 있습니다. For example:

* 검색, 소셜 및 상거래(및 Google 광고)는 클릭을 추적하는 반면, [!DNL Google Analytics] 30분 브라우저 세션당 방문 횟수를 추적합니다. 예를 들어 사용자가 광고를 한 번 클릭하고 뒤로 단추를 클릭한 다음 광고를 다시 클릭하면 검색, 소셜 및 상거래에 두 번의 클릭이 기록되지만 [!DNL Google Analytics] 1회 방문을 기록합니다.

* [!DNL Google Analytics] 모든 트래픽 데이터를 표시하지만 검색, 소셜 및 상거래(및 [!DNL Google Ads])는 잘못된 클릭(예: 지나친 클릭, 반복된 클릭)을 필터링합니다.

* [!DNL Google Analytics] 모든 클릭에 대한 클릭 및 매출 데이터를 포함합니다. Search, Social 및 Commerce에서는 추적 URL이 잘못되거나 누락된 광고 및 키워드에 대한 클릭 및 매출 데이터를 추적할 수 없습니다.
+++

## 전환 지표

+++내 보고서에 전환 데이터가 표시되지 않습니다.
전환이 발생한 전환 지표를 보고서에 포함하지 않을 수 있습니다.
+++

+++보고서에서 수입이 누락되었습니다.

**Adobe Advertising 전환 태그를 사용하는 광고주**

*가능한 원인:*

* 추적 템플릿 또는 대상 URL에 검색, 소셜 및 상거래 클릭 추적 접두사를 접두사로 추가하지 않고 키워드나 광고를 추가했거나 추적 접두사가 잘못되었습니다.

* 변환 추적 태그가 적용 가능한 모든 웹 페이지에서 올바르게 구현되지 않거나 편집되었습니다.

* Search, Social 및 Commerce에서 추적하는 전환 지표는 보고서에서 제외되므로 표시되지 않습니다.

* 클라이언트에 대한 매출 파서가 구현되지 않았습니다.

*가능한 해결 방법 또는 해결 방법:*

1. 보고서 또는 데이터 보기에 올바른 열이 포함되어 있는지 확인합니다. 올바른 열을 추가할 수 없는 경우 사용자 또는 Adobe 계정 팀은 [전환 지표를 보고서에서 사용할 수 있도록 설정](/help/search-social-commerce/admin/conversion-metrics/conversion-metric-edit-available.md).

1. 적용 가능한 모든 웹 페이지에 올바른 전환 추적 태그가 구현되었는지 확인합니다. 필요한 경우 Adobe 계정 팀에 각 적용 가능한 전환 추적 태그에 대한 테스트 트랜잭션을 만들고 트랜잭션 세부 정보(예: )를 캡처하도록 요청합니다. `transactionid` 및 쿠키의 세부 정보(예: `trackingid`, `clickid`등).

1. 다음과 같은 경우 [!UICONTROL Auto Upload] 옵션이 캠페인에 대해 비활성화되고 키워드나 광고를 추가한 다음 각각에 대한 검색, 소셜 및 상거래 클릭 리디렉션 추적을 포함하는 추적 템플릿 또는 대상 URL을 생성했는지 확인합니다. Adobe 계정 팀은 내부 보고서를 실행하여 클릭 추적 URL(추적 템플릿 또는 대상 URL)이 누락되었거나 형식이 잘못되었는지 확인할 수 있습니다.

   필요한 경우 올바른 URL이 포함된 일괄 시트 파일을 만들어 추적을 생성하고 를 사용하여 해당 계정에 파일을 게시합니다. **추적 URL 생성** 옵션을 선택합니다.

   대상 URL은 &quot;http://pixel.everesttech.net&quot; 또는 &quot;https://pixel.everesttech.net&quot;로 시작해야 합니다.

1. 이러한 단계 중 어느 것으로도 문제가 해결되지 않으면 다음 작업을 수행하십시오 [고객 지원 센터 문의](/help/search-social-commerce/get-help.md).

   클라이언트를 시작하지 않았거나 새로 시작한 경우 고객 지원에서 매출 파서가 설정되었는지 확인합니다. 파서가 설정되면 Search, Social 및 Commerce에서 픽셀 변환을 받는지 확인하고 문제를 해결합니다.

**전환 데이터 피드를 보내는 광고주**

*가능한 원인:*

* 피드 파일이 게재되지 않았거나, 완전히 구문 분석되지 않았거나, 피드에 고아 트랜잭션이 포함되어 있습니다.

* 관련 전환 지표는 보고서에서 제외되므로 표시되지 않습니다.

>[!NOTE]
>
>데이터는 일반적으로 피드를 받은 후 2~4시간이 지나야 사용자 인터페이스에 표시됩니다.

*가능한 해결 방법 또는 해결 방법:*

1. 보고서 또는 데이터 보기에 올바른 열이 포함되어 있는지 확인합니다. 올바른 열을 추가할 수 없는 경우 사용자 또는 Adobe 계정 팀은 [전환 지표를 보고서에서 사용할 수 있도록 설정](/help/search-social-commerce/admin/conversion-metrics/conversion-metric-edit-available.md).

1. 실행 [!UICONTROL Portfolio Report]. 비어 있는 경우 [!UICONTROL Campaign Report] 및 [!UICONTROL Search Engine Report] 매출이 해당 보고서에 표시되는지 확인합니다. 이 경우 캠페인이 적절한 포트폴리오에 할당되지 않을 수 있습니다.

1. 파일이 매출 서버로 전송되었는지, 파일이 이전 파일과 동일한 형식 및 파일 이름 지정 규칙을 따랐는지 확인합니다.

   형식 또는 파일 이름 지정 규칙이 변경된 경우 파일을 수정하고 다시 보냅니다.

1. 파일이 전송된 경우 [고객 지원 센터 문의](/help/search-social-commerce/get-help.md).

   고객 지원 센터는 파일이 수신되고 구문 분석되었는지 확인합니다. 파일이 오류 없이 처리된 경우 고아 트랜잭션을 확인합니다.
+++

+++일부 고급 보고서에는 광고주 피드에서 제공한 전환 데이터가 포함되지 않습니다.
다음 [!UICONTROL Geo Distribution Report] 및 [!UICONTROL Domain Referral Report] Adobe Advertising 전환 추적 서비스를 통해 캡처한 데이터를 사용하며 해당 서비스를 사용하는 광고주에게만 생성될 수 있습니다. 보고서에는 Adobe Advertising 전환 추적 시스템 외부에서 추적되는 전환 데이터가 포함되지 않습니다.
+++

+++매출 데이터는 광고주 자신의 매출 데이터와 다릅니다.

**Adobe Advertising 전환 태그를 사용하는 광고주**

*가능한 원인:*

* Search, Social 및 Commerce는 쿠키가 만료되거나 삭제될 때의 수입을 무시하지만 광고주는 이를 유효한 수입으로 간주할 수 있습니다.

* 광고주의 페이지에 대한 트래픽은 광고가 아닌 책갈피나 유기 검색에서 가져왔습니다.

* 변환 추적 태그가 적용 가능한 모든 웹 페이지에서 올바르게 구현되지 않거나 편집되었습니다.

*가능한 해결 방법 또는 해결 방법:*

1. 다음으로 이동 **[!UICONTROL Insights & Reports]>[!UICONTROL Reports]** 및 생성 [!UICONTROL Transaction Report]. 검색, 소셜 및 상거래가 수신한 거래를 광고주의 데이터와 비교합니다.

1. 일부 트랜잭션이 올바르지 않거나 누락된 경우, 관련 전환 추적 태그가 적용 가능한 모든 웹 페이지에 구현되어 있는지, Adobe 계정 팀에서 이를 권장하지 않는 한 편집되지 않았는지 확인하십시오. 웹 사이트가 최근에 업데이트된 경우 태그가 누락되거나 변경될 수 있습니다.

   Search, Social 및 Commerce에서는 이름-값 쌍에 매개 변수가 있는 잘 구성된 URL이 `ef_transaction_properties` 변수 및 변수 내 `src` 의 요소 `img` 태그에 가깝게 배치하십시오.

1. 문제를 확인하고 해결할 수 없는 경우 [고객 지원 센터 문의](/help/search-social-commerce/get-help.md).

   고객 지원 센터는 누락된 거래를 식별한 다음 고아 거래 및 광고에서 발생하지 않은 거래(&quot;상관 관계가 없는 전환&quot;)를 확인합니다.

**를 사용하는 전환 데이터 피드가 있는 광고주 `ef_id` 값**

위의 픽셀 구현에 대해 가능한 원인 및 솔루션을 참조하십시오.

**거래 ID를 사용하는 전환 데이터 피드가 있는 광고주**

*가능한 원인:*

* Search, Social 및 Commerce는 쿠키가 만료되거나 삭제될 때 수익을 무시하지만 광고주는 이를 유효한 수익으로 간주할 수 있습니다.

* 광고주의 페이지에 대한 트래픽은 광고가 아닌 책갈피나 유기 검색에서 가져왔습니다.

* 동일한 거래 ID로 온라인 거래가 발생하기 전에 오프라인 전환이 보고되었습니다. 온라인 거래가 먼저 이루어져야 합니다.

*가능한 해결 방법 또는 해결 방법:*

1. 다음으로 이동 **[!UICONTROL Insights & Reports]>[!UICONTROL Reports]** 및 생성 [!UICONTROL Transaction Report]. 검색, 소셜 및 상거래가 수신한 거래를 광고주의 피드 데이터와 비교합니다.

1. 피드 파일의 트랜잭션이 보고서에서 누락된 경우 오프라인 전환 전에 동일한 트랜잭션 ID(픽셀을 통해 추적됨)를 사용하는 온라인 트랜잭션이 발생했는지 확인합니다.

1. 문제를 확인하고 해결할 수 없는 경우 [고객 지원 센터 문의](/help/search-social-commerce/get-help.md).

   고객 지원 센터에서 데이터 구문 분석 오류 및 [고립 트랜잭션](/help/search-social-commerce/glossary.md#o-p).

**다른 유형의 전환 데이터 피드가 있는 광고주**

*가능한 원인:*

* Search, Social 및 Commerce는 쿠키가 만료되거나 삭제될 때의 수입을 무시하지만 광고주는 이를 유효한 수입으로 간주할 수 있습니다.

* 광고주의 페이지에 대한 트래픽은 광고가 아닌 책갈피나 유기 검색에서 가져왔습니다.

* 다음 항목이 있습니다. [고립 트랜잭션](/help/search-social-commerce/glossary.md#o-p), 따라서 검색, 소셜 및 상거래는 해야 할 모든 매출을 계산하지 않습니다.

* 광고주가 피드에서 보낸 것과 다른 데이터 세트에 대해 검색, 소셜 및 상거래 보고서의 유효성을 검사했습니다.

* 거래 ID(`ev_transid` 값이 전송되지 않았거나 고유하지 않거나 올바르지 않습니다.

* 피드 파일에 중복 추적 ID가 포함되어 있습니다.

* 파일을 구문 분석하는 동안 오류가 발생했습니다.

* 광고주의 중복 제거 로직은 검색, 소셜 및 상거래 로직과 다릅니다.

*가능한 해결 방법 또는 해결 방법:*

1. 다음으로 이동 **[!UICONTROL Insights]및[!UICONTROL Reports > Reports]** 및 생성 [!UICONTROL Transaction Report]. 검색, 소셜 및 상거래가 수신한 거래를 광고주의 데이터와 비교합니다.

1. 일부 트랜잭션이 올바르지 않거나 누락된 경우, a) 피드 파일에 모든 필수 트랜잭션 ID가 포함되어 있고 중복 추적 ID는 없는지, b) 트랜잭션 ID가 고유하고 올바른지 확인하십시오.

1. 문제를 확인하고 해결할 수 없는 경우 [고객 지원 센터 문의](/help/search-social-commerce/get-help.md).

   고객 지원 센터에서 데이터 구문 분석 오류 및 고립된 트랜잭션을 확인합니다.
+++

+++매출 데이터가 Adobe Analytics의 데이터와 다름 참조 [https://experienceleague.adobe.com/docs/advertising/integrations/analytics/data/data-variances.html](https://experienceleague.adobe.com/docs/advertising/integrations/analytics/data/data-variances.html).<!-- change link URL to relative link -->
+++

## 특정 보고서

+++다음과 같아야 함: [!UICONTROL Portfolio Report] 와 동일한 숫자 표시 [!UICONTROL Portfolios] 보기?
다음 [!UICONTROL Portfolio Report] 및 [!UICONTROL Portfolios] 보기의 모든 필터, 보고서 매개 변수 및 보기와 보고서의 데이터 열이 동일하면 보기에는 동일한 데이터가 표시됩니다. 예를 들어 [!UICONTROL Portfolios] 보기에 &quot;&quot;인 포트폴리오가 표시됩니다.[!UICONTROL All but inactive]&quot;날짜 범위&quot;의 경우[!UICONTROL Last 7 days]&quot;기본 데이터 열만 표시된 다음 [!UICONTROL Portfolio Report] 기본 매개변수를 사용하면 동일한 데이터가 표시됩니다. 보고서 매개 변수를 변경하거나 [!UICONTROL Portfolios] 를 보면 데이터 값이 다를 수 있습니다.
+++

+++내 데이터 [!UICONTROL Portfolio Report] 이(가) 내 데이터와 일치하지 않음 [!UICONTROL Search Engine Report] 또는 [!UICONTROL Search Engine Account Report].
다음 [!UICONTROL Portfolio Report] 지정된 포트폴리오에 할당된 캠페인에 대한 데이터만 표시하지만 [!UICONTROL Search Engine Report] 및 [!UICONTROL Search Engine Account Report] 에는 포트폴리오에 할당되지 않은 캠페인용 데이터도 포함될 수 있습니다.
+++

+++어떻게 [!UICONTROL Model Accuracy] > [!UICONTROL Forecast Accuracy Report] 포트폴리오 수준과 다름 [!UICONTROL Model Accuracy Report]?
(에이전시 계정 관리자, Adobe 계정 관리자 및 관리자 사용자만 해당) [!UICONTROL Forecast Accuracy Report] 다음에서 사용 가능 [!UICONTROL Reports] > [!UICONTROL Model Accuracy] 포트폴리오 수준과 동일한 데이터 제공 [!UICONTROL Model Accuracy Report] 여러 포트폴리오에서 실행하고 속성 규칙을 변경할 수 있는 경우를 제외하고, 사용자 지정 매개 변수를 사용하여 보고서를 실행하고 예약할 수도 있으며, 스프레드시트 피드를 만드는 데 사용할 수도 있습니다. 또한 [!UICONTROL Forecast Accuracy Report] 는 현재 목표보다 포트폴리오에 대한 기록 목표를 사용하여 매출 정확도를 평가하고 해당 시간대의 데이터를 더 정확하게 나타내기 때문에 기존 포트폴리오 수준 보고서보다 정확합니다.
+++

+++광고 수준 데이터를에 사용할 수 없음 [!DNL Google Ads] 동적 검색 광고(DSA), 성능 최대, 스마트 쇼핑 및 [!DNL YouTube] 캠페인.
광고 네트워크는 이러한 캠페인을 위해 매출을 개별 광고에 연결하는 데 필요한 식별자를 제공하지 않습니다. 따라서 의 이러한 캠페인 유형에 대해 광고 수준 성과 데이터를 사용할 수 없습니다. [!UICONTROL Ads] 보기 또는 [!UICONTROL Ad Variation Report]. 캠페인에 대한 총 광고 수준 데이터와 캠페인에 대한 총 데이터 간의 불일치를 예상합니다.
+++

+++위치 [!UICONTROL Transaction Report], 데이터 피드에서 가져온 전환 지표 또는 Adobe Advertising 추적 픽셀에서 추적한 전환 지표를 어떻게 알 수 있습니까?
트랜잭션 보고서에서, 사용자 지정 열 &quot;&quot;을(를) 포함하는 경우 포함된 전환 지표가 Adobe Advertising 추적 픽셀에 의해 추적되었는지 여부를 알 수 있습니다.[!UICONTROL Tracking URL].&quot; Adobe Advertising 추적 픽셀이 있는 추적 URL은 &quot;로 시작합니다.`http://pixel.everesttech.net`.&quot;
+++

+++내 데이터 [!UICONTROL Transaction Report] 이(가) 내 데이터와 일치하지 않음 [!UICONTROL Keyword Report].
포트폴리오별로 두 보고서를 모두 생성할 때 다음을 생성하는 경우 데이터가 다릅니다. [!UICONTROL Keyword Report] 현재 캠페인에 데이터를 사용하는 대신 이전 데이터(지정된 날짜 동안 포트폴리오 구성 기반)를 사용합니다. 다음을 생성하는 경우 [!UICONTROL Transaction Report] 포트폴리오별로 포트폴리오에 현재 캠페인에 대한 데이터가 포함됩니다.
+++

## 스프레드시트 피드

+++보고서 출력에 날짜 범위의 혼합이 포함됩니다.
피드가 &quot; 이외의 데이터 집계 레벨을 사용하여 데이터를 집계하는 경우 다른 날짜 범위를 볼 수 있습니다[!UICONTROL Daily].&quot;

이 문제를 해결하려면 매일 집계된 데이터를 포함하도록 스프레드시트 피드를 업데이트합니다. 이 작업에는 보고서 템플릿 업데이트, 템플릿을 사용하여 보고서 생성, 사용자 지정 만들기가 포함됩니다 [!DNL Microsoft® Excel] 보고서를 사용한 다음 새 Excel 템플릿을 포함하도록 피드 설정을 업데이트합니다. 자세한 내용은 &quot;[스프레드시트 보고서 피드 설정 편집](/help/search-social-commerce/reports/automation/spreadsheet-feeds/spreadsheet-feed-edit.md).&quot;
+++

+++스프레드시트 피드로 인해 내부 오류가 발생합니다.
이 오류는 보고서 템플릿의 열을 변경했지만 를 업데이트하지 않으면 발생할 수 있습니다. [!DNL Microsoft® Excel] 템플릿도 함께 사용해야 합니다.

이 문제를 해결하려면 스프레드시트 피드를 업데이트하여 새 열을 포함합니다. 이 작업에는 보고서 템플릿 업데이트, 템플릿을 사용하여 보고서 생성, 사용자 지정 만들기가 포함됩니다 [!DNL Excel] 보고서를 사용한 다음 새 Excel 템플릿을 포함하도록 피드 설정을 업데이트합니다. 자세한 내용은 &quot;[스프레드시트 보고서 피드 설정 편집](/help/search-social-commerce/reports/automation/spreadsheet-feeds/spreadsheet-feed-edit.md).&quot;
+++

+++에서 스프레드시트 피드를 열려고 할 때 [!DNL Excel], [!DNL Excel] 에서 &quot;읽을 수 없는 콘텐츠&quot; 오류를 보고하고, 데이터가 복구된 콘텐츠에서 제거됩니다.
다음의 경우 [!DNL Microsoft® Excel] 템플릿이 시작 날짜별로 데이터를 오름차순으로 정렬하지 않습니다. 스프레드시트 피드에 빈 행이 포함될 수 있습니다. 특히, [!DNL Excel] 에서 &quot;Excel에서 읽을 수 없는 콘텐츠를 찾았습니다.&lt;*보고서 이름*>.xlsx.&#39; 통합 문서의 내용을 복구하시겠습니까? 이 통합 문서의 원본을 신뢰하는 경우 [예]를 클릭하십시오.&quot; &quot;예&quot;를 클릭하면 &quot;제거된 레코드: /xl/worksheets/sheet1.xml 부분의 셀 정보&quot;라는 메시지가 표시되고 스프레드시트 피드에 빈 행이 포함됩니다.

문제를 해결하려면 다음을 편집하십시오. [!DNL Excel] 데이터 정렬 기준 피드와 연결된 템플릿 [!DNL Start date in Ascending (Oldest to Newest) order]를 클릭한 다음 스프레드시트 피드 설정을 통해 업데이트된 템플릿을 업로드합니다. 자세한 내용은 &quot;[스프레드시트 보고서 피드 편집](/help/search-social-commerce/reports/automation/spreadsheet-feeds/spreadsheet-feed-edit.md).&quot;
+++
