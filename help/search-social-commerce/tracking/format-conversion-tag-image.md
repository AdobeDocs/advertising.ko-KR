---
title: 이미지 변환 추적 태그의 형식
description: 이미지 변환 추적 태그의 형식을 참조합니다.
exl-id: e23107e1-b719-4572-a471-13e51387465d
feature: Search Tracking
source-git-commit: 4b9cc5956d573b346eacdf71a8ea490c162b4660
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# 이미지 변환 추적 태그의 형식

>[!NOTE]
>
>이미지 태그와 JavaScript 태그를 사용하는 시기에 대한 자세한 내용은 추적 태그에 대한 [FAQ](/help/search-social-commerce/tracking/faqs-conversion-page-view-tracking-tags.md)를 참조하십시오.

* HTTP가 있는 사이트에 대한 비보안 태그:

  `<img src="http://pixel.everesttech.net/px2/<ef-userid>?px_evt=s&s=<segmentid>&px_evt=t&ev_propertyname=<propertyname>&ev_transid=<transid>" width="1" height="1"/>`

* HTTPS가 있는 사이트에 대한 보안 태그:

  `<img src="https://pixel.everesttech.net/px2/<ef-userid>?px_evt=s&s=<segmentid>&px_evt=t&ev_propertyname=<propertyname>&ev_transid=<transid>" width="1" height="1"/>`

여기서:

* `<ef-userid>`은(는) 검색, 소셜 및 Commerce이 광고주에게 할당하는 고유한 숫자 사용자 ID입니다.

* `<propertyname>`은(는) 추적할 변환입니다. 예를 들어 &quot;등록&quot;이라는 전환을 추적하는 경우 태그에 매개 변수 `ev_registration=<registration>`이(가) 포함되며 각 거래(예: `ev_registration=1`)에 대한 실제 매출을 전달해야 합니다. 여러 속성을 추적하면 `ev_registration=<registration>&ev_sale=<sale>`(예: `ev_registration=1&ev_sale=12.99`)과 같은 앰퍼샌드(`&`)로 연결됩니다. **참고:** 속성 이름에 특수 문자가 포함되지 않을 수 있습니다.

* `<transid>`은(는) 광고주가 트랜잭션을 식별하기 위해 생성하고 전달하는 고유한 트랜잭션 ID(예: 실제 주문 ID)입니다. &quot;[!UICONTROL Include unique transaction IDs]&quot; 옵션을 선택한 경우에만 포함됩니다.

  Search, Social 및 Commerce에서는 거래 ID를 사용하여 거래 ID와 속성 값이 동일한 중복 거래를 제거합니다. 거래 ID는 [!UICONTROL Transaction Report]에 포함되어 있으며 광고주의 데이터로 Adobe Advertising 내에서 데이터의 유효성을 검사하는 데 사용할 수 있습니다. **참고:** 광고주의 데이터에 트랜잭션당 고유 ID가 포함되지 않은 경우 검색, 소셜 및 Commerce은 여전히 트랜잭션 시간을 기준으로 ID를 생성합니다.

<!-- add more links -->

>[!MORELIKETHIS]
>
>* [Adobe Advertising 전환 추적 태그 정보](/help/search-social-commerce/tracking/conversion-tracking-advertising.md)
>* [Adobe Advertising 변환 태그 생성](/help/search-social-commerce/tools/conversion-tag-generate.md)
>* 전환 및 페이지 보기 추적 태그에 대한 [FAQ](/help/search-social-commerce/tracking/faqs-conversion-page-view-tracking-tags.md)
>* [JavaScript 전환 추적 태그 버전 2](format-conversion-tag-jsv2.md)의 형식
>* [JavaScript 전환 추적 태그 버전 3](format-conversion-tag-jsv3.md)의 형식
