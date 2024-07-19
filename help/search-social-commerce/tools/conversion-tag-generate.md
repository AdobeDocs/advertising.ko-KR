---
title: Adobe Advertising 전환 추적 태그 생성
description: Adobe Advertising 전환 태그를 만들어 전환 이벤트를 추적하는 방법에 대해 알아봅니다.
exl-id: 02492162-96a0-4a91-8896-dd0f72199f79
feature: Search Tools, Search Tracking
source-git-commit: e16bc62127a708de8f4deb1eddfa53a14405cbc2
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---

# Adobe Advertising 전환 추적 태그 생성

*Adobe Advertising 전환 추적만 있는 광고주*

추적할 각 지표 세트에 대해 별도의 전환 태그를 생성하고 각 태그를 삽입할 웹 페이지 목록과 함께 광고주 또는 에이전시에 제공합니다.

>[!NOTE]
>
>이 기능은 광고주의 웹 페이지에 이미지 태그 또는 [!DNL JavaScript] 태그를 추가하지 않습니다. 태그는 웹 페이지를 업데이트하기 위한 광고주의 일반적인 절차에 따라 추가해야 합니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Tools] >[!UICONTROL Conversion Tags]**&#x200B;을(를) 클릭합니다.

1. [변환 태그 설정](#conversion-tag-settings)을 지정하십시오.

1. 태그를 생성합니다.

   * 웹 사이트에서 HTTP를 사용하는 경우 **[!UICONTROL Generate Conversion Tag]**&#x200B;을(를) 클릭합니다.

   * 웹 사이트가 보안 서버(HTTPS)에서 실행되는 경우 **[!UICONTROL Generate Secure Conversion Tag]**&#x200B;을(를) 클릭합니다.

1. 대화 상자에서 태그를 복사한 다음 필요에 따라 적절한 웹 페이지에 붙여넣습니다.

>[!NOTE]
>
>새 전환 태그의 각 지표는 구현되지 않았거나 해당 웹 페이지가 클릭을 받지 않은 경우에도 [!UICONTROL Admin] > [!UICONTROL Conversions]에 자동으로 나열됩니다. 이 동작은 수동으로 만든 태그 또는 다른 곳에서 만든 태그의 동작 중 하나가 클릭될 때까지 [!UICONTROL Admin] > [!UICONTROL Conversions]에 나열되지 않는 것과 다릅니다. 그러나 모든 경우에 각 지표는 명시적으로 사용할 수 있도록 할 때까지 처음에는 포트폴리오 목표, 보고서 및 보기에서 제외됩니다. 그러나 포트폴리오 목표에 지표를 추가하기 전에 먼저 지표를 사용할 수 있도록 하고 보고서에 추가하여 클릭 수를 받는 시점을 확인하는 것을 고려하십시오.

## Adobe Advertising 전환 태그 설정 {#conversion-tag-settings}

**[!UICONTROL Tag Type]:** 만들 태그의 형식:

* *[!UICONTROL Image]:* 이미지 태그를 만들어 최종 사용자가 볼 수 없는 1픽셀 x 1픽셀 투명 이미지(픽셀)를 웹 페이지에 표시합니다. 가장 좋은 방법은 사이트에 JavaScript 태그 사용에 대한 정책이 있을 때만 이미지 태그를 사용하는 것입니다.

* *[!UICONTROL JavaScript]:* JavaScript 태그를 만듭니다.

태그 유형 간의 차이점에 대한 자세한 내용은 &quot;[Adobe Advertising 전환 및 페이지 보기 추적 태그에 대한 FAQ](/help/search-social-commerce/tracking/faqs-conversion-page-view-tracking-tags.md)&quot;를 참조하십시오.

**[!UICONTROL Tag Properties]:** 최종 사용자가 전환 태그가 포함된 페이지를 볼 때 추적할 하나 이상의 전환 지표가 있습니다. 목록에 지표를 추가하려면 &quot;[!UICONTROL Add new property]&quot; 필드에 지표 이름을 입력하고 **[!UICONTROL Add]**&#x200B;을(를) 클릭합니다.

여러 지표를 추적할 때 `ev_Property1=<Property1>&ev_Property2=<Property2>`과(와) 같은 태그의 앰퍼샌드(`&`)에 의해 연결됩니다.

>[!NOTE]
>
>이 목록에 추가된 지표는 아무 곳에나 저장되지 않거나 [!UICONTROL Admin] 탭에서 클라이언트의 [!UICONTROL Conversions] 목록과 통합됩니다. 그러나 Adobe Advertising이 실제로 지표에 대한 데이터를 수집하면 지표가 클라이언트의 [!UICONTROL Conversions] 목록에 자동으로 추가됩니다. 이 오류는 전환 태그가 페이지에 구현되어 있고 최종 사용자가 해당 페이지를 여는 트랜잭션을 완료할 때 발생합니다.

**[!UICONTROL Include unique transaction IDs]:**(선택 사항) 태그에 트랜잭션 ID 속성(`ev_transid=<transid>`)이 포함되어 있습니다. 이 옵션은 기본적으로 선택되어 있습니다.

이 옵션을 선택하는 경우 거래가 완료되면 광고주는 `<transid>`에 대한 고유한 값(예: 실제 주문 ID)을 생성한 다음 `ev_transid=0123`과 같은 Adobe Advertising에 다시 전달해야 합니다. Adobe Advertising은 거래 ID를 사용하여 거래 ID와 속성 값이 동일한 중복 거래를 제거합니다. 트랜잭션 ID에는 매개 변수 구분 기호로 예약된 앰퍼샌드 기호(`&`)를 포함할 수 없습니다. 거래 ID가 [의 [!UICONTROL Transaction Report]](/help/search-social-commerce/reports/management/basic-advanced/transaction-report.md)에 포함되어 있습니다. 광고주의 데이터로 검색, 소셜 및 Commerce 내의 데이터를 확인하는 데 사용할 수 있습니다.

데이터에 트랜잭션당 고유 ID가 포함되지 않으면 Adobe Advertising은 여전히 트랜잭션 시간을 기반으로 ID를 생성합니다.

>[!NOTE]
>
>오프라인 전환을 위한 전환 데이터가 포함된 [거래 ID 피드](/help/search-social-commerce/tracking/feed-transaction-id.md)를 보내는 경우 거래의 오프라인 부분에 대한 피드 데이터에서 거래의 온라인 부분에 대한 거래 ID(`ev_transid`)를 제출해야 합니다.

**[!UICONTROL Page is inside FB app]:** 사용되지 않음

**[!UICONTROL Segment users]:** 사용되지 않음

**[!UICONTROL JS Version]:**([!DNL JavaScript] 태그만) 만들 [!DNL JavaScript] 태그의 버전: *[!UICONTROL v2]*(기본값) 또는 *[!UICONTROL v3]*.

Adobe Advertising 전환 및 페이지 보기 추적 태그에 대한 &quot;[FAQ](/help/search-social-commerce/tracking/faqs-conversion-page-view-tracking-tags.md)&quot;를 참조하십시오. 차이점에 대한 자세한 정보를 제공합니다.

>[!MORELIKETHIS]
>
>* [Adobe Advertising 전환 추적 태그 정보](/help/search-social-commerce/tracking/conversion-tracking-advertising.md)
>* [추적 태그를 만들고 디코딩하는 도구에 대한 정보](tracking-tools-about.md)
>* 전환 및 페이지 보기 추적 태그에 대한 [FAQ](/help/search-social-commerce/tracking/faqs-conversion-page-view-tracking-tags.md)
>* [JavaScript 전환 추적 태그 버전 3](/help/search-social-commerce/tracking/format-conversion-tag-jsv3.md)의 형식
>* [JavaScript 전환 추적 태그 버전 2](/help/search-social-commerce/tracking/format-conversion-tag-jsv2.md)의 형식
>* [이미지 변환 추적 태그의 형식](/help/search-social-commerce/tracking/format-conversion-tag-image.md)
>* [Adobe Advertising JavaScript 전환 매핑 태그](/help/search-social-commerce/tracking/itp-conversion-mapping-tag.md)
>* [광고주의 전환 지표 관리 정보](/help/search-social-commerce/admin/conversion-metrics/conversion-metric-about.md)
