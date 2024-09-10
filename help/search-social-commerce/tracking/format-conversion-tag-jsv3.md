---
title: JavaScript 전환 추적 태그 버전 3의 형식
description: JavaScript 전환 추적 태그 버전 3의 형식을 참조하십시오.
exl-id: 9fc6bb15-d880-4353-a8c5-260b7932ab34
feature: Search Tracking
source-git-commit: dda4ff8e7538bc742caa50862575cb4e46a1371d
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# JavaScript 전환 추적 태그 버전 3의 형식

다음 형식은 HTTPS를 사용하는 사이트에 사용됩니다. HTTP를 사용하는 사이트의 경우 URL은 &quot;http&quot;로 시작해야 합니다.

>[!NOTE]
>
>버전 2와 버전 3을 사용할 시기에 대한 자세한 내용은 추적 태그에 대한 [FAQ](/help/search-social-commerce/tracking/faqs-conversion-page-view-tracking-tags.md)를 참조하십시오.

```
<script type='text/javascript'>
    (function() {
        var f = function() {
              EF.init({ eventType: "transaction",
                        transactionProperties : "ev_property=<property name>&ev_transid=<transid>",
                        segment : "",
                        searchSegment : "",
                        sku : "",
                        userid : "ef-userid",
                        pixelHost : "pixel.everesttech.net"
                        
                        , allow3rdPartyPixels: 1});
              EF.main();
        };
        window.id5PartnerId=<ID5_PartnerID>
        window.EF = window.EF || {};
        if (window.EF.main) {
            f();
            return;
        }
        window.EF.onloadCallbacks = window.EF.onloadCallbacks || [];
        window.EF.onloadCallbacks[window.EF.onloadCallbacks.length] = f;
        if (!window.EF.jsTagAdded) {
            var efjs = document.createElement('script'); efjs.type = 'text/javascript'; efjs.async = true;
            efjs.src = 'https://www.everestjs.net/static/st.v3.js';
            var s = document.getElementsByTagName('script')[0]; s.parentNode.insertBefore(efjs, s);
            window.EF.jsTagAdded=1;
        }
    })();
</script>
<noscript><img src="https://pixel.everesttech.net/<ef-userid>/t?ev_property=<property name>&ev_transid=<transid>" width="1" height="1"/></noscript>
```

여기서:

* `<ef-userid>`은(는) 검색, 소셜 및 Commerce이 광고주에게 할당하는 고유한 숫자 사용자 ID입니다.

* `<ID5_PartnerID>`은(는) 조직이 [!DNL ID5]과(와) 계약에 서명한 후 받는 조직의 ID5 파트너 ID입니다. 조직에서 DSP을 사용하고 ID5 유니버설 ID와 연결된 사용자를 추적하는 [사용자 지정 세그먼트](/help/dsp/audiences/universal-ids.md)가 있는 경우에만 이 변수를 포함하십시오.

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
>* [이미지 변환 추적 태그의 형식](format-conversion-tag-image.md)
