---
title: Adobe 광고 전환 추적 태그 생성
description: Adobe 광고 전환 태그를 만들어 전환 이벤트를 추적하는 방법에 대해 알아봅니다.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Adobe 광고 전환 추적 태그 생성

*Adobe 광고 전환 추적만 있는 광고주*

추적할 각 지표 세트에 대해 별도의 전환 태그를 생성하고 각 태그를 삽입할 웹 페이지 목록과 함께 광고주 또는 에이전시에 제공합니다.

>[!NOTE]
>
>이 기능은 이미지 태그를 추가하지 않거나 [!DNL JavaScript] 태그를 광고주의 웹 페이지에 추가합니다. 태그는 웹 페이지를 업데이트하기 위한 광고주의 일반적인 절차에 따라 추가해야 합니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Tools] >[!UICONTROL Conversion Tags]**.

1. 다음을 지정합니다. [전환 태그 설정](#conversion-tag-settings).

1. 태그를 생성합니다.

   * 웹 사이트에서 HTTP를 사용하는 경우 **[!UICONTROL Generate Conversion Tag]**.

   * 웹 사이트가 보안 서버(HTTPS)에서 실행되는 경우 **[!UICONTROL Generate Secure Conversion Tag]**.

1. 대화 상자에서 태그를 복사한 다음 필요에 따라 적절한 웹 페이지에 붙여넣습니다.

>[!NOTE]
>
>새 전환 태그의 각 지표는에 자동으로 나열됩니다. [!UICONTROL Admin] > [!UICONTROL Transaction Properties]가 구현되지 않았거나 웹 페이지에 있는 경우에도 클릭을 받지 않았습니다. 이 비헤이비어는 수동으로 또는 다른 곳에서 만든 태그에서 나열되지 않은 지표의 비헤이비어와 다릅니다 [!UICONTROL Admin] > [!UICONTROL Transaction Properties] 이 링크가 있는 웹 페이지 중 하나가 클릭될 때까지. 그러나 모든 경우에 각 지표는 명시적으로 사용할 수 있도록 할 때까지 처음에는 포트폴리오 목표, 보고서 및 보기에서 제외됩니다. 그러나 포트폴리오 목표에 지표를 추가하기 전에 먼저 지표를 사용할 수 있도록 하고 보고서에 추가하여 클릭 수를 받는 시점을 확인하는 것을 고려하십시오.

## Adobe 광고 전환 태그 설정 {#conversion-tag-settings}

**[!UICONTROL Tag Type]:** 만들 태그의 유형:

* *[!UICONTROL Image]:* 웹 페이지에서 최종 사용자에게 보이지 않는 1픽셀 x 1픽셀 투명 이미지(픽셀)를 표시하는 이미지 태그를 만듭니다. 가장 좋은 방법은 사이트에 JavaScript 태그 사용에 대한 정책이 있을 때만 이미지 태그를 사용하는 것입니다.

* *[!UICONTROL JavaScript]:* JavaScript 태그를 만들려면.

태그 유형 간의 차이에 대한 자세한 내용은 &quot;[Adobe 광고 전환 및 페이지 보기 추적 태그에 대한 FAQ](/help/search-social-commerce/tracking/faqs-conversion-page-view-tracking-tags.md).&quot;

**[!UICONTROL Tag Properties]:** 최종 사용자가 전환 태그가 포함된 페이지를 볼 때 추적할 하나 이상의 트랜잭션 속성(지표)입니다. 목록에 지표를 추가하려면 목록에 지표 이름을 입력합니다.[!UICONTROL Add new property]&quot;필드 및 클릭 **[!UICONTROL Add]**.

여러 지표를 추적할 때 앰퍼샌드(`&`)을 클릭하여 제품에서 사용할 수 있습니다 `ev_Property1=<Property1>&ev_Property2=<Property2>`.

>[!NOTE]
>
>이 목록에 추가된 지표는 아무 곳에나 저장되거나 클라이언트의 [!UICONTROL Transaction Properties] 다음에 목록: [!UICONTROL Admin] 탭. 하지만 지표는 클라이언트의 [!UICONTROL Transaction Properties] 는 Adobe 광고가 실제로 지표에 대한 데이터를 수집하면 자동으로 표시되며, 전환 태그가 페이지에 구현되어 최종 사용자가 해당 페이지를 여는 트랜잭션을 완료할 때 발생합니다.

**[!UICONTROL Include unique transaction IDs]:** (선택 사항) 거래 ID 속성(`ev_transid=<transid>`)을 클릭하여 제품에서 사용할 수 있습니다. 이 옵션은 기본적으로 선택되어 있습니다.

이 옵션을 선택하는 경우 광고주가 다음에 대한 고유한 값을 생성해야 합니다. `<transid>` (예: 실제 주문 ID) 트랜잭션이 완료되면 이를 다시 Adobe 광고로 전달합니다. 예: `ev_transid=0123`. Adobe 광고는 거래 ID를 사용하여 거래 ID와 속성 값이 동일한 중복 거래를 제거합니다. 거래 ID에는 앰퍼샌드 기호(`&`), 매개 변수 구분 기호로 예약됩니다. 거래 ID는에 포함됩니다. [다음 [!UICONTROL Transaction Report]](/help/search-social-commerce/reports/management/basic-advanced/transaction-report.md): 광고주의 데이터로 검색, 소셜 및 상거래 내 데이터의 유효성을 검사하는 데 사용할 수 있습니다.

데이터에 트랜잭션당 고유 ID가 포함되지 않은 경우 Adobe 광고는 여전히 트랜잭션 시간을 기준으로 ID를 생성합니다.

>[!NOTE]
>
>다음을 전송하면 [거래 ID 피드](/help/search-social-commerce/tracking/feed-transaction-id.md) 오프라인 전환을 위한 전환 데이터를 사용하여 거래 ID( )를 제출해야 합니다.`ev_transid`)를 참조하십시오.

**[!UICONTROL Page is inside FB app]:** 사용되지 않음

**[!UICONTROL Segment users]:** 사용되지 않음

**[!UICONTROL JS Version]:** ([!DNL JavaScript] 태그 전용) [!DNL JavaScript] 만들 태그: *[!UICONTROL v2]* (기본값) 또는 *[!UICONTROL v3]*.

를 참조하십시오.[Adobe 광고 전환 및 페이지 보기 추적 태그에 대한 FAQ](/help/search-social-commerce/tracking/faqs-conversion-page-view-tracking-tags.md).&quot; 차이점에 대한 자세한 정보를 제공합니다.

>[!MORELIKETHIS]
>
>* [Adobe 광고 전환 추적 태그 정보](/help/search-social-commerce/tracking/conversion-tracking-advertising.md)
>* [추적 태그를 만들고 디코딩하는 도구 정보](tracking-tools-about.md)
>* [전환 및 페이지 보기 추적 태그에 대한 FAQ](/help/search-social-commerce/tracking/faqs-conversion-page-view-tracking-tags.md)
>* [JavaScript 전환 추적 태그 버전 3의 형식](/help/search-social-commerce/tracking/format-conversion-tag-jsv3.md)
>* [JavaScript 전환 추적 태그 버전 2의 형식](/help/search-social-commerce/tracking/format-conversion-tag-jsv2.md)
>* [이미지 변환 추적 태그의 형식](/help/search-social-commerce/tracking/format-conversion-tag-image.md)
>* [Adobe Advertising JavaScript 전환 매핑 태그](/help/search-social-commerce/tracking/itp-conversion-mapping-tag.md)
>* [광고주의 거래 속성 관리 정보](/help/search-social-commerce/admin/transaction-properties/transaction-property-about.md)

