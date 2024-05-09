---
title: JavaScript 전환 추적 태그 버전 2의 형식
description: JavaScript 전환 추적 태그 버전 2의 형식을 참조합니다.
exl-id: 75e96f97-a3f0-4f5b-8bbb-4b1e8986f01a
feature: Search Tracking
source-git-commit: 4b9cc5956d573b346eacdf71a8ea490c162b4660
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# JavaScript 전환 추적 태그 버전 2의 형식

다음 형식은 HTTPS를 사용하는 사이트에 사용됩니다. HTTP를 사용하는 사이트의 경우 URL은 &quot;http&quot;로 시작해야 합니다.

>[!NOTE]
>
>버전 2와 버전 3을 사용해야 하는 경우에 대한 자세한 내용은 [추적 태그에 대한 FAQ](/help/search-social-commerce/tracking/faqs-conversion-page-view-tracking-tags.md).

```
<script language="javascript" src="https://www.everestjs.net/static/st.v2.js"></script>
<script language="javascript">
var ef_event_type="transaction";
var ef_transaction_properties = "ev_property name=<property name>&ev_transid=<transid>";
/*
 * Do not modify below this line
 */
var ef_segment = "";
var ef_search_segment = "";
var ef_userid="ef-userid";
var ef_pixel_host="pixel.everesttech.net";
var ef_fb_is_app = 0;
var ef_allow_3rd_party_pixels = 1;
effp();
</script>
<noscript><img src="https://pixel.everesttech.net/<ef-userid>/t?ev_property name=<property name>&ev_transid=<transid>" width="1" height="1"/></noscript>
```

여기서:

* `<ef-userid>` 는 검색, 소셜 및 Commerce이 광고주에게 할당하는 고유한 숫자 사용자 ID입니다.

* `<propertyname>` 는 추적할 변환입니다. 예를 들어 &quot;registration&quot;이라는 전환을 추적하는 경우 태그에 매개 변수가 포함됩니다 `ev_registration=<registration>`, 그리고 각 트랜잭션에 대한 실제 매출을 전달해야 합니다(예: `ev_registration=1`). 여러 속성이 추적되면 앰퍼샌드(`&`), 예: `ev_registration=<registration>&ev_sale=<sale>` (예: `ev_registration=1&ev_sale=12.99`). **참고:**  속성 이름에는 특수 문자를 사용할 수 없습니다.

* `<transid>` 는 광고주가 거래를 식별하기 위해 생성하고 전달하는 고유한 거래 ID(예: 실제 주문 ID)입니다. &quot;&quot;에만 포함됩니다.[!UICONTROL Include unique transaction IDs]&quot; 옵션이 선택되어 있습니다.

  Search, Social 및 Commerce에서는 거래 ID를 사용하여 거래 ID와 속성 값이 동일한 중복 거래를 제거합니다. 거래 ID는에 포함됩니다. [!UICONTROL Transaction Report]: 광고주의 데이터로 Adobe Advertising 내 데이터의 유효성을 검사하는 데 사용할 수 있습니다. **참고:** 광고주의 데이터에 트랜잭션당 고유 ID가 포함되지 않은 경우 검색, 소셜 및 Commerce은 여전히 트랜잭션 시간을 기준으로 ID를 생성합니다.

<!-- add more links -->

>[!MORELIKETHIS]
>
>* [Adobe Advertising 전환 추적 태그 기본 정보](/help/search-social-commerce/tracking/conversion-tracking-advertising.md)
>* [Adobe Advertising 변환 태그 생성](/help/search-social-commerce/tools/conversion-tag-generate.md)
>* [전환 및 페이지 보기 추적 태그에 대한 FAQ](/help/search-social-commerce/tracking/faqs-conversion-page-view-tracking-tags.md)
>* [JavaScript 전환 추적 태그 버전 2의 형식](format-conversion-tag-jsv2.md)
>* [JavaScript 전환 추적 태그 버전 3의 형식](format-conversion-tag-jsv3.md)
>* [이미지 변환 추적 태그의 형식](format-conversion-tag-image.md)
