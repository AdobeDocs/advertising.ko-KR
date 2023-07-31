---
title: 검색, 소셜 및 상거래에 대한 전환 추적 옵션
description: 검색, 소셜 및 상거래에 대한 전환 추적 옵션에 대해 알아봅니다.
exl-id: 098efaf8-6ffb-4811-8b20-41c7c85df812
feature: Search Tracking
source-git-commit: 97111c6cd38098cac72b8773390afd254a017d1d
workflow-type: tm+mt
source-wordcount: '837'
ht-degree: 0%

---

# 검색, 소셜 및 상거래에 대한 전환 추적 옵션

검색, 소셜 및 상거래는 다음과 같은 방법으로 추적되는 전환 데이터를 사용할 수 있습니다.

* **Adobe Advertising 추적 전환:** 광고주는 각 전환 페이지에 Adobe Advertising 전환 추적 태그를 삽입합니다. 태그는 변환 데이터를 추적 서버로 전송합니다. 기존 타사 픽셀 또는 최신 자사 픽셀을 사용할 수 있습니다. 를 참조하십시오.[각 전환 추적 메서드 비교](#conversion-tracking-comparison).&quot;

* **Adobe Analytics 전환:** 광고주는 모든 전환에 Adobe Analytics 추적을 사용합니다. 이 옵션을 사용하려면 Adobe Advertising-Adobe Analytics 통합이 필요합니다. 를 참조하십시오.[Adobe Analytics 전환 추적](conversion-tracking-analytics.md)&quot; 을 참조하십시오.

* **[!DNL Google Analytics]전환:** 광고주는 [!DNL Google Analytics] 태그를 사용하여 모든 전환을 추적합니다. 를 참조하십시오.[[!DNL Google Ads] 검색, 소셜 및 상거래의 전환 데이터](/help/search-social-commerce/campaign-management/introduction/google-conversion-data.md)자동으로 동기화되는 전환에 대한 자세한 내용은 &quot;을 참조하십시오.

* **광고주 추적 전환:** (Search, Social 및 Commerce 클라이언트만 해당) 광고주는 온라인 및 오프라인 전환 데이터의 조합이 있는 피드 파일을 Search, Social 및 Commerce에 제공합니다. 를 참조하십시오.[EF ID 피드를 사용한 전환 추적](feed-efid.md)&quot; 및 &quot;[거래 ID 피드를 사용한 전환 추적](feed-transaction-id.md).&quot;

## 각 전환 추적 메서드 비교 {#conversion-tracking-comparison}

브라우저 쿠키 정책이 점점 더 엄격해지고 있으므로 현재 추적 기능을 이해하고 더 긴 기간 동안 최상의 옵션을 식별하는 것이 중요합니다.

| 추적 메서드 | 설명 | 제한 사항 | 이점 | 추천? |
|----|----|----|----|----|
| Adobe Analytics | 를 사용하는 광고주 [Adobe Analytics for Advertising](https://experienceleague.adobe.com/docs/advertising/integrations/analytics/overview.html) 자동으로 가져오기 [!DNL Analytics] 보고 및 최적화를 위한 Adobe Advertising에 표준 및 사용자 지정 이벤트. | <ul><li>[!DNL Safari] 7일 전환 전환 전환만 허용하며, 전환 확인 기간 동안 사이트 방문 횟수 반복 시 재설정됩니다.</li><li> 에서 유사한 제한 사항 예상 [!DNL Chrome] 2024년.</li></ul> | <ul><li>와 원활한 통합 [!DNL Analytics]</li> <li>에서 유료 검색 데이터 보기 [!DNL Analytics] Analysis Workspace</li><li>유료 검색 이상의 이점</li></ul> | 예 |
| 레거시 Adobe Advertising 픽셀 | 광고주는 이전 Adobe Advertising 이미지 또는 JavaScript 픽셀을 전환 페이지에 추가합니다. 픽셀은 광고를 클릭한 사용자가 페이지에 도달하면 실행됩니다. 이 방법은 서드파티 쿠키에 의존합니다. | <ul><li>[!DNL Safari] 는 이 메서드를 사용하여 모든 전환 추적을 차단합니다.</li><li>에서 유사한 제한 사항 예상 [!DNL Chrome] 2024년.</li></ul> | 픽셀이 이미 구현되었습니다. 하지만, 여전히 [추가 ITP 매핑 태그 구현](itp-conversion-mapping-tag.md).<br><br>권장 사항: 자사 픽셀로 전환합니다. | 아니요 |
| Adobe Advertising 자사 픽셀 | 광고주는 다음 작업을 수행합니다. <ul><li>용 JavaScript 라이브러리 구현 [Adobe Experience Cloud ID(ECID) 서비스](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html) 전체 사이트에 게시합니다.</li><li>Adobe Advertising 추가 [ITP 매핑을 사용한 JavaScript 태그](itp-conversion-mapping-tag.md) 를 클릭하여 랜딩 페이지일 수 있는 모든 페이지로 이동합니다(랜딩 페이지는 시간이 지남에 따라 변경될 수 있으므로 이상적으로는 모든 페이지에서). 태그를 사용하면 Adobe Advertising이 랜딩 페이지에서 큰 숫자를 과학적 표기법으로 변환하는 페이지에서 발생하는 전환 이벤트를 추적할 수 있습니다.</li><li>Adobe Advertising 추가 [JavaScript 전환 추적 태그 v3](format-conversion-tag-jsv3.md) 변환 페이지.</li></ul> | <ul><li>[!DNL Safari] 7일 전환 전환 전환만 허용하며, 전환 확인 기간 동안 사이트 방문 횟수 반복 시 재설정됩니다.</li><li>에서 유사한 제한 사항 예상 [!DNL Chrome] 2022년.</li></ul> | [!DNL Safari] 7일 전환 확인 중 전환을 추적합니다. 전환 확인 기간은 전환 확인 기간 동안 사이트 방문 반복에 대해 재설정되므로, 제한이 모든 항목에 영향을 주지는 않습니다 [!DNL Safari] 사용자. | 아니요 |
| EFID 피드 | 광고주의 검색 계정은 Adobe Advertising 고유 ID(토큰)를 사용하여 대상 URL/최종 URL을 생성하도록 설정됩니다. 사용자가 광고를 클릭하면 Adobe Advertising이 고유한 ID( )를 만듭니다.`EFID`)를 클릭하여 최종 URL의 끝에 표시합니다. 광고주의 클라이언트 시스템은 클릭으로 인해 발생한 전환에 대한 고유 식별자로 EFID를 캡처하여 EFID, 트랜잭션 날짜 및 전환 속성을 포함하는 매출 피드의 Adobe Advertising에게 보냅니다. 그런 다음 Adobe Advertising은 EFID를 사용하여 원래 클릭에 대한 전환을 일치시킵니다. | <ul><li>광고주는 EFID를 캡처하고 자동화된 피드를 매일 Adobe Advertising으로 보낼 수 있는 방법을 가져야 합니다.</li><li>전환은 최대 180일(광고주당) 동안 또는 Adobe Advertising 시스템의 제한에 따라 추적할 수 있습니다.</li></ul> | <ul><li>이 메서드는 자사 전환 데이터를 사용하므로 타사 쿠키 제한 사항의 영향을 받지 않습니다.</li><li>온라인 및 오프라인 전환은 하나의 피드로 보낼 수 있습니다.</li><li>사이트에 코드 변경이나 태그가 필요하지 않습니다.</li></ul> | 예 |
| 거래 ID 피드 [콤보 피드] | 광고주는 고유한 거래 ID( )에 대한 매개 변수를 포함하는 Adobe Advertising 픽셀을 추가합니다.`ev_transid=&lt;transid&gt;`)를 클릭하여 회사 웹 페이지를 방문하면 Adobe Advertising이 픽셀이 실행될 때 생성되는 고유한 거래 ID를 캡처합니다. 광고주의 클라이언트 시스템이 [!UICONTROL Transaction ID] 일치하는 오프라인 전환을 위한 매출 피드를 Adobe Advertising에게 보냅니다. [!UICONTROL Transaction ID] 값 | <ul><li>광고주가 이전 픽셀을 사용하는 경우 [!DNL Safari] 실행이 차단되면 오프라인 데이터에 사용하기 위해 ID가 캡처되지 않습니다.</li><li>피드가 자동화되지 않았습니다.</li></ul> | <ul><li>자사 픽셀을 구현하는 경우 [!UICONTROL Transaction ID] 다음 위치에 캡처됨 [!DNL Safari].</li><li>오프라인/승인된 전환 이벤트 추적을 제공합니다.</li></ul> | 아니요 |
| Google 전환 | 다음으로 추적되는 전환 [!DNL Google Analytics] 태그는 API 연결을 통해 Adobe Advertising으로 자동으로 가져옵니다. 각 전환 이름에는 `&quot;GGL_&quot;` 접두사입니다. | <ul><li>Google은 일반적으로 오프라인 데이터를 추적하지 않습니다.</li><li>Microsoft® 광고 전환은 포함되지 않습니다.</li></ul> | Google은 머신 러닝을 사용하여 &quot;외삽합니다.[모델 전환](https://support.google.com/google-ads/answer/10081327).&quot; | 아니요 |

<!--
| Microsoft Advertising Conversions | Conversions tracked with Microsoft Advertising universal event tags (UET) are automatically imported to Adobe Advertising via an API connection. Each conversion name has a &quot;???&quot; prefix. | Microsoft Advertising typically doesn't track offline data. Google conversions aren't included. | ?? | No |
-->

>[!MORELIKETHIS]
>
>* [Adobe Advertising 전환 추적 태그 기본 정보](/help/search-social-commerce/tracking/conversion-tracking-advertising.md)
>* [Adobe Analytics 전환 추적](/help/search-social-commerce/tracking/conversion-tracking-analytics.md)
>* [EF ID 피드를 사용한 전환 추적](/help/search-social-commerce/tracking/feed-efid.md)
>* [거래 ID 피드를 사용한 전환 추적](/help/search-social-commerce/tracking/feed-transaction-id.md)
