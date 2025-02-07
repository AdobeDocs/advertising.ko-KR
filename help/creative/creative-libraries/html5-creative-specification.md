---
title: HTML5 크리에이티브 사양
description: Advertising Creative을 위해 HTML5 크리에이티브 사양 을 참조하십시오.
feature: Creative Standard Creatives
source-git-commit: fd925c641bef7953aea50813725252c3913757fa
workflow-type: tm+mt
source-wordcount: '1158'
ht-degree: 0%

---

# HTML5 Advertising Creative 크리에이티브 사양

이 문서에서는 [!DNL Creative] 내의 HTML 5 크리에이티브에 대한 요구 사항 및 API 지원에 대해 간략하게 설명합니다. API를 사용하면 크리에이티브 게재 시 속성을 구성할 수 있는 HTML5 크리에이티브를 개발할 수 있습니다.

## 범위

[!DNL Creative]은(는) 페이지의 설정된 테두리 내에 표시되는 리치 미디어 크리에이티브가 아닌 HTML5 배너를 지원합니다. 다음 유형의 HTML5 광고 유형을 사용할 수 있습니다.

<!--Remove to simplify:

* **Simple HTML5:** Supports a single landing page URL that can be configured during creative creation and trafficking.

* **Static HTML5:** Supports up to 5 landing page URLs that can be configured during creative creation and trafficking.

-->

* **HTML5:** 창의적 생성 및 트래픽 분석 중에 구성할 수 있는 랜딩 페이지 URL을 최대 5개까지 지원합니다.

* **유연한 HTML5:** 창의적 작성 및 트래픽 관리 중에 구성할 수 있는 랜딩 페이지 URL을 최대 5개까지 지원하며, 창의적 작성 및 트래픽 관리 중에 창의적 특성을 수정할 수 있습니다.

## 요구 사항

### 폴더 및 압축 요구 사항

* 크리에이티브는 ZIP 파일(.ZIP 형식)로 패키징되어야 합니다. 중첩된 ZIP 파일은 지원되지 않으므로 외부 압축 폴더 내에 압축 폴더를 포함하지 마십시오.

* ZIP 파일에는 [!DNL Creative] JavaScript 라이브러리에 대한 참조를 포함하는 HTML 파일(기본 HTML 표시 파일)이 하나 이상 있어야 합니다. 기본 HTML 파일은 루트 폴더 또는 하위 폴더에 있을 수 있습니다.

* 기본 HTML 파일에는 특수 문자가 포함되지 않으면 이름을 지정할 수 있지만, `index.html`이(가) 권장됩니다.

* 최종 크리에이티브를 렌더링하는 데 필요한 모든 지원 에셋은 HTML 표시 파일과 동일한 폴더에 있거나 기본 폴더의 하위 폴더에 있어야 합니다.

* 해당 크리에이티브에 대해 참조되지 않은 파일을 크리에이티브에 포함하지 마십시오.

### Advertising Creative JavaScript 파일 포함

기본 HTML 파일(다른 파일 없음)에는 JavaScript 파일 `AMOLibrary.js`에 대한 참조가 포함되어야 합니다. 다음 주소를 사용하여 `<head>` 섹션의 첫 번째 줄에 있는 파일을 호출합니다.

`https://ads.everesttech.net/ads/static/local/AMOLibrary.js`

이 파일에는 종료 이벤트의 로컬 테스트가 문제 없이 발생하도록 하는 함수가 포함되어 있습니다.

<!-- Remove to simplify:

### Simple HTML5 creative requirements

#### Support for click-through URLS in simple HTML5

The `<head>` section of the main HTML file must include a JavaScript variable name `clickTag` or `clickTAG`. The value of the variable should be the landing page URL. See the following example.

```
<script type=”text/javascript”>
var clickTag = “http://www.example.com”;
</script>
```

>[!NOTE]
>
>The static URL you include in the HTML5 creative is used for local testing purposes only and will be overwritten. When you upload an HTML5 creative, you'll define the default landing page for the `clickTag` variable. When you assign an uploaded HTML5 creative to an ad experience, you can optionally override the default landing page for the `clickTag` variable, and [!DNL Creative] adds click tracking to the URL when you save the experience.

-->

<!-- Renamed to simplify:
### Static HTML5 creative requirements
-->

### HTML5 크리에이티브 요구 사항

#### 정적 HTML5에서 클릭스루 URL 지원

##### `amo.registerClick(clkVar, clkUrl)`

클릭스루 URL과 각 URL을 참조하는 데 사용되는 관련 매개 변수(`clickTag`)를 등록합니다. [!DNL Creative] 광고 서버에 클릭 추적을 추가할 위치를 알려 줍니다. 이 API를 사용하여 각각 해당 랜딩 페이지 URL을 갖는 최대 5개의 클릭 태그 변수를 등록할 수 있습니다.

>[!NOTE]
>
>HTML5 크리에이티브에 포함하는 정적 URL은 로컬 테스트용으로만 사용되며 덮어씁니다. HTML5 크리에이티브를 업로드할 때 각 `clickTag` 변수에 대한 기본 랜딩 페이지를 정의합니다. 업로드된 HTML5 크리에이티브를 광고 경험에 할당할 때 선택적으로 각 `clickTag` 변수에 대한 기본 랜딩 페이지를 재정의할 수 있습니다. [!DNL Creative]은(는) 경험을 저장할 때 클릭 추적을 URL에 추가합니다.

###### 매개 변수

* `clkVar` — 큰따옴표로 묶인 클릭 변수(일반적으로 &quot;clickTag&quot;)의 이름입니다.

* `clkUrl` — 큰따옴표로 묶인 이 클릭 변수의 랜딩 페이지 URL입니다.

###### 사용

기본 HTML 파일의 `<head>` 섹션에서 `amo.registerClick()`을(를) 호출합니다.

###### 예

`amo.registerClick("clickTag","http://www.example.com")`

##### `amo.onAdClick(clk, event)`

종료 이벤트를 트리거하여 사용자를 `clickTag`에 대해 구성된 랜딩 페이지로 리디렉션합니다. 로컬 테스트 중에 이 함수는 개발자에게 함수에 전달되는 URL이 등록되었는지 여부를 알립니다.

###### 매개 변수

* `clkTag` — `amo.registerClick()` 함수를 사용하여 랜딩 페이지 URL을 할당하는 데 사용하는 클릭 변수의 이름으로 작은 따옴표로 묶여 있습니다.

* `event` — (선택 사항) JavaScript &quot;click&quot; 이벤트 개체입니다. 이는 클릭 좌표를 기록하며, 이는 창의적 성과를 분석하는 데 추가로 사용될 수 있다.

###### 사용

기본 HTML 파일의 `<body>` 섹션에서 `amo.onAdClick()`을(를) 호출합니다.

###### 예시

`amo.onAdClick('clickTag')` 또는 `amo.onAdClick('clickTag',clickEvt)`

### 유연한 HTML5 크리에이티브 요구 사항

#### 유연한 HTML5에서 클릭스루 URL 지원

##### `amo.registerClick(clkVar, clkUrl)`

클릭스루 URL과 각 URL을 참조하는 데 사용되는 관련 매개 변수(`clickTag`)를 등록합니다. [!DNL Creative] 광고 서버에 클릭 추적을 추가할 위치를 알려 줍니다. 이 API를 사용하여 각각 해당 랜딩 페이지 URL을 갖는 최대 5개의 클릭 태그 변수를 등록할 수 있습니다.

>[!NOTE]
>
>HTML5 크리에이티브에 포함하는 정적 URL은 로컬 테스트용으로만 사용되며 덮어씁니다. HTML5 크리에이티브를 업로드할 때 각 `clickTag` 변수에 대한 기본 랜딩 페이지를 정의합니다. 업로드된 HTML5 크리에이티브를 광고 경험에 할당할 때 선택적으로 각 `clickTag` 변수에 대한 기본 랜딩 페이지를 재정의할 수 있습니다. [!DNL Creative]은(는) 경험을 저장할 때 클릭 추적을 URL에 추가합니다.

###### 매개 변수

* `clkVar` — 큰따옴표로 묶인 클릭 변수(일반적으로 &quot;clickTag&quot;)의 이름입니다.

* `clkUrl` — 큰따옴표로 묶인 이 클릭 변수의 랜딩 페이지 URL입니다.

###### 사용

기본 HTML 파일의 `<head>` 섹션에서 `amo.registerClick()`을(를) 호출합니다.

###### 예

`amo.registerClick("clickTag","http://www.example.com")`

##### `amo.onAdClick(clk, event)`

종료 이벤트를 트리거하여 사용자를 `clickTag`에 대해 구성된 랜딩 페이지로 리디렉션합니다. 로컬 테스트 중에 이 함수는 개발자에게 함수에 전달되는 URL이 등록되었는지 여부를 알립니다.

###### 매개 변수

* `clkTag` — `amo.registerClick()` 함수를 사용하여 랜딩 페이지 URL을 할당하는 데 사용하는 클릭 변수의 이름으로 작은 따옴표로 묶여 있습니다.

* `event` — (선택 사항) JavaScript &quot;click&quot; 이벤트 개체입니다. 이는 클릭 좌표를 기록하며, 이는 창의적 성과를 분석하는 데 추가로 사용될 수 있다.

###### 사용

기본 HTML 파일의 `<body>` 섹션에서 `amo.onAdClick()`을(를) 호출합니다.

###### 예시

`amo.onAdClick('clickTag')` 또는 `amo.onAdClick('clickTag',clickEvt)`

#### 유연한 HTML5에서 크리에이티브 속성 지원

##### `amo.registerAttribute(key, type, value)`

광고 또는 경험 작성 시 변경할 수 있는 광고 속성을 정의합니다. 광고 또는 경험 작성 시 구성할 수 있는 최대 20개의 광고 속성을 정의할 수 있습니다.

>[!NOTE]
>
>이 방법에 정의된 값은 로컬 개발에만 사용되며 라이브 광고 서비스에는 사용되지 않습니다.

###### 매개 변수

* `key` — 속성의 영숫자 이름입니다. 영문자로 시작해야 합니다.

* `type` — 특성 유형(`TEXT` 또는 `IMAGE`).

* `value` — 테스트를 위한 특성의 값입니다. `IMAGE` 형식의 특성에 대해 값은 이미지 파일에 대한 상대 경로여야 합니다.

###### 사용

로컬 모드에서 테스트하는 동안 하나의 Creative 특성, 유형 및 값을 등록하려면 `amo.registerAttribute()`을(를) 호출하십시오. 샘플 값으로 사용되는 모든 이미지 파일은 업로드된 패키지와 함께 ZIP 파일에 패키지되어야 합니다.

##### `amo.attributes`

크리에이티브 속성 변수 이름 및 값을 쿼리하기 위한 JSON 개체. 객체 키는 속성 이름이 되고, 값은 해당 속성의 값이 됩니다.

로컬 테스트 모드에서 키-값 쌍은 `amo.registerAttribute` API에 의해 등록된 쌍입니다. 제작의 경우, 창의적 생성 및 트래픽 처리 시 창의적 속성 변수 이름과 값을 구성해야 합니다.

### 크리에이티브 콘텐츠 요구 사항

Advertising DSP에서 사용할 수 있는 대부분의 디스플레이 교환에는 다음과 같은 크리에이티브 요구 사항이 있습니다.

* 단색 테두리가 모든 광고 이미지를 둘러싸야 합니다.

* 광고 확장은 허용되지 않습니다.

* 랜딩 페이지는 새 창에서 열려야 합니다.

* 랜딩 페이지 도메인과 하위 도메인은 35자를 초과할 수 없습니다. **참고:** 최종 랜딩 페이지 URL은 HTML5 에셋 자체가 아니라 DSP에 정의되어 있습니다.

* 광고 제공에 대한 모든 면책조항은 랜딩 페이지뿐만 아니라 광고 자체에 포함되어야 합니다.

<!-- * (Dynamic HTML5 creatives) Do not use `window.open` to handle clicks in your code. Always use `amo.onDynAdClick` to handle click-throughs. -->

## JSON 개체 및 배열로서의 예제 콘텐츠

### JSON 개체로서의 콘텐츠 예

<!-- Should I update these to current/real URLs? Sent email to Apoorva 1/22. -->

```
{
"name": "Adobe Creative",
"description": "Creative",
"picture_url": "http://wwwimages.adobe.com/content/dam/acom/en/products/creativecloud/max2016/images/cc-overview-assets-720x472.png",
"product_url": "http://www.adobe.com/creativecloud.html?promoid=ZP46FD38&mv=other"
}
```

### JSON 배열로서의 콘텐츠 예

<!-- Should I update these to current/real URLs? Sent email to Apoorva 1/22. -->

```
[{
"name": "Adobe Creative",
"description": "Creative",
"picture_url": "http://wwwimages.adobe.com/content/dam/acom/en/products/creativecloud/max2016/images/cc-overview-assets-720x472.png",
"product_url": "http://www.adobe.com/creativecloud.html?promoid=ZP46FD38&mv=other"
},

{
"name": "Adobe Creative",
"description": "Creative",
"picture_url": "http://wwwimages.adobe.com/content/dam/acom/en/products/creativecloud/max2016/images/cc-overview-mobile-720x520.png",
"product_url": "http://adobe.com/"
}

]
```

## 예제 HTML5 크리에이티브

### 폴더 구조 예(압축 해제 후)

* index.html

* /assets (폴더)

   * bg.jpg (JPG, PNG, SVG 또는 GIF 이미지)

### 단순 HTML5 크리에이티브용 HTML 파일(index.html) 예

```
<!DOCTYPE html>
<html>
<head>
  <script type="text/javascript" src="https://ads.everesttech.net/ads/static/local/AMOLibrary.js"></script>
  <script type="text/javascript">
  amo.registerClick("clickTag","http://www.example.com");
  </script>
</head>
<body>
  <a href="javascript:amo.onAdClick('clickTag')">
  <img src="assets/bg.jpg" width="300" height="250" style="position:absolute;top:0px;left:0px;">
  </a>
</body>
</html>
```

### 정적 HTML5 크리에이티브용 예제 HTML 파일(index.html)

```
<!DOCTYPE html>
<html>
<head>
  <script type="text/javascript" src="https://ads.everesttech.net/ads/static/local/AMOLibrary.js"></script>
  <script type="text/javascript">
  amo.registerClick("clickTag","http://www.example.com");
  amo.registerClick("clickTag2","http://www.example2.com");
  amo.registerClick("clickTag3","http://www.example3.com");
  amo.registerClick("clickTag4","http://www.example4.com");
  amo.registerClick("clickTag5","http://www.example5.com");
  </script>
</head>
<body>
  <a href="javascript:amo.onAdClick('clickTag')">
  <img src="assets/bg.jpg" width="300" height="250" style="position:absolute;top:0px;left:0px;">
  </a>
</body>
</html>
```

>[!MORELIKETHIS]
>
>* [Creative 라이브러리에 표준 크리에이티브 추가](/help/creative/creative-libraries/creative-add-standard.md)
