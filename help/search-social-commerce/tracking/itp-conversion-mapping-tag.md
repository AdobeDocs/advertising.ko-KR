---
title: Adobe Advertising 전환 매핑 태그
description: Adobe Advertising이 랜딩 페이지가 아닌 페이지에서 발생하는 전환 이벤트를 추적할 수 있는 ITP 2.2용 JavaScript 기반 전환 매핑 태그에 대해 알아봅니다.
exl-id: cbeaf3cd-f1ab-419d-bba8-58a1c8215352
feature: Search Tracking
source-git-commit: e16bc62127a708de8f4deb1eddfa53a14405cbc2
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 0%

---

# Adobe Advertising JavaScript 전환 매핑 태그

*Adobe Advertising 전환 추적만 있는 광고주*

Adobe Advertising JavaScript 기반 전환 매핑 태그 를 Adobe Advertising JavaScript v2 또는 v3 전환 추적 태그 와 함께 사용할 경우, Adobe Advertising은 랜딩 페이지가 아닌 페이지에서 발생하는 전환 이벤트를 추적할 수 있습니다. ITP 2.2 솔루션은 광고주가 소유한 iFrame의 로컬 저장소에 사용자의 쿠키를 저장합니다. 그런 다음 로컬 저장소는 클릭 다운스트림에서 전환 페이지까지 쿠키 값을 유지할 수 있습니다.

전환 매핑 태그를 사용하여 Adobe Advertising이 Apple Safari 및 Mozilla Firefox 브라우저 내에서 발생하는 모든 전환을 추적할 수 있도록 함으로써 자사 쿠키의 지속성을 제한합니다. <!-- For all requirements to track conversions from Safari, see "Track Conversions from Apple Safari Browsers." -->

변환 매핑 태그를 사용하려면 다음을 수행하십시오.

1. [전환 매핑 태그를 배포합니다](#deploy-conversion-mapping-tag).

1. 조직에서 여러 Adobe Experience Cloud Identity Service 조직 ID(이전의 IMS 조직 ID)를 사용하는 경우 조직 ID를 포함하도록 [전환 태그를 업데이트](#update-conversion-tags)하십시오.

1. [태그 배포 유효성 검사](#validate-conversion-mapping).

## ITP 2.2용 JavaScript 전환 매핑 태그 배포 {#deploy-conversion-mapping-tag}

>[!NOTE]
>
>ITP 2.0용 JavaScript 전환 매핑 태그를 사용하는 경우 모든 전환 페이지의 기존 태그를 다음 태그 중 하나로 바꾸십시오.<!-- any other instructions, too? Point them to the other page on Track Conversions from Safari...." -->

* 조직에서 검색, 소셜 및 Commerce 계정에 사용되는 단일 조직 ID를 사용하는 경우 다음 태그를 사용하십시오.

  `<script src="//www.everestjs.net/static/amo-conversion-mapper.js" userid="{AMO User ID}"></script>`

  `{AMO User ID}`을(를) 검색, 소셜 및 Commerce 계정의 고유 사용자 ID로 바꾸는 경우.

* 조직에서 여러 조직 ID를 사용하는 경우 다음 태그를 사용하십시오.

  `<script src="//www.everestjs.net/static/amo-conversion-mapper.js" imsorgid="{xxxxxx@AdobeOrg}" userid="{AMO User ID}"></script>`

  여기서:

   * `{xxxxxx@AdobeOrg}` 값을 페이지의 전환을 추적할 조직 ID로 바꿉니다. 모든 전환 페이지에 동일한 조직 ID를 사용합니다.

   * `{AMO User ID}`을(를) 검색, 소셜 및 Commerce 계정의 고유 사용자 ID로 바꿉니다.

* `imsorgid` 변수를 스크립트 태그에 추가하는 것을 지원하지 않는 태그 관리 시스템을 사용하는 경우 대신 다음 코드를 사용하십시오.

  *조직에서 단일 조직 ID를 사용하는 경우:

  ```
  <script>
  window.ad_cloud = window.ad_cloud || {};
  window.ad_cloud.userid = "{AMO User ID}"
  </script>
  <script src="//www.everestjs.net/static/amo-conversionmapper.js"></script>
  ```

  `{AMO User ID}`을(를) 검색, 소셜 및 Commerce 계정의 고유 사용자 ID로 바꾸는 경우.

   * 조직에서 여러 조직 ID를 사용하는 경우:

     ```
     <script>
     window.ad_cloud = window.ad_cloud || {};
     window.ad_cloud.imsorgid = "{xxxxxx@AdobeOrg}"
     window.ad_cloud.userid = "{AMO User ID}"
     </script>
     <script src="//www.everestjs.net/static/amo-conversionmapper.js"></script>
     ```

     여기서:

      * `{xxxxxx@AdobeOrg}` 값을 페이지의 전환을 추적할 조직 ID로 바꿉니다. 모든 전환 페이지에 동일한 조직 ID를 사용합니다.

      * `{AMO User ID}`을(를) 검색, 소셜 및 Commerce 계정의 고유 사용자 ID로 바꿉니다.

조직 ID 또는 검색, 소셜 및 Commerce 사용자 ID의 값을 모를 경우 Adobe 계정 관리자에게 문의하십시오.

### 예시

```
<script src="//www.everestjs.net/static/amo-conversion-mapper.js" imsorgid="abc12345@AdobeOrg" userid="99999"></script>`
```

```
<script>
window.ad_cloud = window.ad_cloud || {};
window.ad_cloud.imsorgid = "abc12345@AdobeOrg"
window.ad_cloud.userid = "99999"
</script>
<script src="//www.everestjs.net/static/amo-conversion-mapper.js"></script>
```

### 태그를 추가할 위치

검색 클릭으로 랜딩 페이지일 수 있는 모든 페이지에 태그를 추가합니다(랜딩 페이지는 시간이 지남에 따라 변경될 수 있으므로 모든 페이지에서 이상적으로). Adobe Advertising JavaScript v3 전환 추적 태그 앞에 로드해야 합니다.

iframe 또는 컨테이너 태그 내에 배치되면 다음을 수행합니다.

* iframe은 최상위 도메인과 동일한 수준에 있어야 합니다.

* 변환 매핑 태그는 최상위 도메인 아래에 하나의 수준만 있어야 합니다.

## JavaScript 전환 태그 업데이트 {#update-conversion-tags}

조직에서 여러 조직 ID를 사용하는 경우 페이지의 전환이 추적되는 조직 ID를 기존 JavaScript 전환 태그에 추가합니다.

조직에서 한 개의 조직 ID를 사용하는 경우 이 단계는 필요하지 않습니다.

### JavaScript V2 태그

전환 스크립트 태그의 시작 부분에 다음 문자열을 추가합니다.

`ef_imsorgid="{xxxxxx@AdobeOrg}";`

여기서 `{xxxxxx@AdobeOrg}` 값을 페이지의 전환을 추적할 조직 ID로 바꿉니다.

예:

```
<script language="javascript" src="https://www.everestjs.net/static/st.v2.js"></script>
<script language="javascript">
ef_imsorgid = "abc12345@AdobeOrg";
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

### JavaScript 태그

`window.EF`을(를) 정의한 후 다음 문자열을 추가합니다.

`window.EF.imsorgid = "{xxxxxx@AdobeOrg}";`

여기서 `{xxxxxx@AdobeOrg}` 값을 페이지의 전환을 추적할 조직 ID로 바꿉니다.

예:

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
        window.EF = window.EF || {};
        window.EF.imsorgid ="abc12345@AdobeOrg";
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

## 태그 배포의 유효성 검사 {#validate-conversion-mapping}

Adobe 계정 팀에 문의하여 전환 매핑 태그 및 일반 전환 태그(업데이트한 경우)의 유효성을 확인합니다.
