---
title: ' [!DNL Analytics for Advertising]에 대한 JavaScript 코드'
description: ' [!DNL Analytics for Advertising]에 대한 JavaScript 코드'
feature: Integration with Adobe Analytics
exl-id: 18bfb32d-2754-44b2-86c1-d102836cc08c
TQID: https://experienceleague.adobe.com/g9onwe1IQl1kbyQ82W2KmODPGUAReKiotxy65yCZcNY
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2:
  - id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
source-git-commit: 7845129ba6566c1aaaf160cc6f9ad33bf1731f75
workflow-type: tm+mt
source-wordcount: 941
ht-degree: 0%

---

# [!DNL Analytics for Advertising]에 대한 JavaScript 코드

*Advertising DSP만 있는 광고주*

Advertising DSP의 경우 [!DNL Analytics for Advertising] 통합은 뷰스루 및 클릭스루 사이트 상호 작용을 추적합니다. 클릭스루 방문은 웹 페이지의 표준 Adobe Analytics 코드에 의해 추적됩니다. [!DNL Analytics] 코드는 랜딩 페이지 URL의 AMO ID 및 EF ID 매개 변수를 캡처하여 예약된 해당 [!DNL eVars]에서 추적합니다. 웹 페이지에 JavaScript 코드 조각을 배포하여 뷰스루 방문을 추적할 수 있습니다.

사이트 방문의 첫 번째 페이지 보기에서 Adobe Advertising JavaScript 코드는 방문자가 이전에 광고를 보거나 클릭했는지 확인합니다. 사용자가 이전에 클릭스루를 통해 사이트로 들어오거나 광고를 보지 않은 경우 방문자가 무시됩니다. 방문자가 광고를 보았으며, Adobe Advertising에 설정된 [전환 확인 기간](/help/integrations/analytics/prerequisites.md#lookback-a4adc) 동안 클릭스루를 통해 사이트에 들어가지 않은 경우, Adobe Advertising JavaScript 코드는 a) [Experience Cloud ID 서비스](https://experienceleague.adobe.com/docs/id-service/using/home.html)를 사용하여 보조 ID(`SDID`)를 생성하거나 b) Adobe Experience Platform [!DNL Web SDK] `generateRandomID` 메서드를 사용하여 `[!DNL StitchID]`을(를) 생성합니다. 두 ID 중 하나를 사용하여 Adobe Advertising의 데이터를 방문자의 Adobe Analytics 히트에 연결합니다. 그런 다음 Adobe Analytics은 Adobe Advertising에서 광고 노출과 연결된 AMO ID 및 EF ID를 쿼리합니다. 그런 다음 AMO ID 및 EF ID가 해당 [!DNL eVars]에서 채워집니다. 이 값은 지정된 기간(기본적으로 60일) 동안 지속됩니다.

[!DNL Analytics]은(는) EF ID를 키로 사용하여 사이트 트래픽 지표(페이지 보기 수, 방문 수, 체류 시간 등) 및 [!DNL Analytics] 사용자 지정 또는 표준 이벤트를 매시간 Adobe Advertising으로 보냅니다. 그런 다음 이러한 [!DNL Analytics] 지표는 Adobe Advertising 속성 시스템을 통해 실행되어 전환을 클릭 및 노출 기록에 연결합니다.

>[!NOTE]
>
>Adobe Advertising JavaScript 추적 로직은 Adobe 측에서 발생하므로 페이지 로드 시간에 거의 영향을 주지 않습니다.
>
>반면 Advertising DSP의 [!DNL Analytics]에 대한 [!DNL DCM] 데이터 커넥터([!DNL Google Campaign Manager 360] 사용)에 대한 논리는 클라이언트측에서 발생합니다. 클라이언트측 결합은 페이지 로드 속도를 줄이고 데이터 손실 위험을 증가시킵니다. 이 문제는 [!DNL Analytics] JavaScript에서 [!DNL DoubleClick]을(를) ping하고 [!DNL DoubleClick]이(가) 마지막 클릭/노출 데이터를 [!DNL Analytics]에 다시 전달할 때까지 기다려야 하기 때문에 발생합니다. [!DNL DSP] 팀이 [!DNL DCM] 데이터 커넥터를 설정할 때 페이지를 지연할 시간을 지정해야 합니다.

<!--
## Deploying the JavaScript code

All users must deploy the standard JavaScript code.

Users who want to convert first-party segments from their customer data platforms to [!DNL RampIDs] or [!DNL ID5] IDs [!!!!VERIFY that it's not needed for importing segments directly from LiveRamp] must also deploy ID partner-specific JavaScript code to match conversions to view-throughs.

### The standard code

The standard JavaScript library consists of two lines that allow [!DNL Analytics] and Adobe Advertising to communicate with each other. If the [!DNL Analytics for Advertising] integration was completed during the Adobe Advertising implementation, then you should have already received this code with instructions on how to deploy it.

#### Implementations that use the Experience Cloud Identity Service `visitorAPI.js` code

```
<script src="https://www.everestjs.net/static/le/last-event-tag-latest.min.js">
<script>
     if("undefined" != typeof AdCloudEvent) 
          AdCloudEvent('IMS ORG Id','rsid');
</script>
```

#### Implementations that use the Experience Platform [!DNL Web SDK] `alloy.js`code

### Additional code to import first-party segments to [!DNL RampIDs] and [!DNL ID5] IDs

   * For [!DNL RampIDs], Contact your Adobe Account Team, who will give you instructions to register for a [!DNL LiveRamp] [!DNL LaunchPad] tag. Registration is free, but you must sign an agreement. Once you register, your Adobe Account Team will generate and provide a unique tag for your organization to implement on your webpages.

    [MAYBE PUT THIS BELOW] Place the [!DNL LaunchPad] tag on every page of your website, preferably as the first script within the page head tags but as high within the page head tags as possible.

   * For [!DNL ID5] IDs: Contact your Adobe Account Team, who will give you instructions to register for the tag with ID5. Registration is free, but you must sign an agreement. Once you register, a member of ID5's technical team will provide a unique tag for your organization to implement on your webpages.
-->

## JavaScript 코드 배포

JavaScript 라이브러리는 [!DNL Analytics]과(와) Adobe Advertising이 서로 통신할 수 있도록 하는 두 줄로 구성됩니다. Adobe Advertising 구현 중에 [!DNL Analytics for Advertising] 통합이 완료된 경우 배포 방법에 대한 지침이 포함된 이 코드를 이미 받았어야 합니다.

### 코드

#### Experience Cloud ID 서비스 `visitorAPI.js` 코드를 사용하는 구현

```
<script src="https://www.everestjs.net/static/le/last-event-tag-latest.min.js">
<script>
     if("undefined" != typeof AdCloudEvent) 
          AdCloudEvent('IMS ORG Id','rsid');
</script>
```

#### Experience Platform [!DNL Web SDK] `alloy.js` 코드를 사용하는 구현

```
<script src="https://www.everestjs.net/static/le/last-event-tag-latest.min.js">
<script>
     if("undefined" != typeof AdCloudEvent) 
          stitchId = AdCloudEvent('IMS ORG Id','rsid').generateRandomId();
</script>
```

### 코드를 배치할 위치

[!DNL Analytics for Advertising] JavaScript 함수는 Experience Cloud ID 서비스 뒤에 와야 하지만 Analytics 앱 측정 코드 앞에 와야 합니다. 이렇게 하면 보조 ID(`SDID`) 또는 `[!DNL StitchID]`이(가) Analytics 호출에 포함됩니다.

![코드 배치](/help/integrations/assets/a4adc-code-placement.png)

### 코드 배포 확인

아래 설명된 대로 Adobe Advertising으로 이동하는 요청과 [!DNL Analytics]&#x200B;(으)로 이동하는 요청 사이의 4가지 ID 값을 비교하여 패킷 스니퍼 유형의 도구([!DNL Charles], [!DNL Fiddler] 또는 [!DNL Chrome Developer Tools])를 사용하여 유효성 검사를 수행할 수 있습니다.

#### [!DNL Chrome Developer Tools]을(를) 사용하여 코드를 확인하는 방법 {#validate-js-chrome}

1. [!DNL Chrome Developer Tools]을(를) 열고 **네트워크** 탭을 클릭합니다.

1. [!DNL Analytics for Advertising] JavaScript이 포함된 웹 사이트 페이지를 로드합니다.

1. [!UICONTROL Network] 탭을 `last`(으)로 필터링하고 다음 두 행을 검토하십시오.

   ![마지막 필터링](/help/integrations/assets/a4adc-code-validation-filter-last.png)

   * 첫 번째 행은 JavaScript 라이브러리에 대한 호출이며 제목이 `last-event-tag-latest.min.js`입니다.
   * 두 번째 행은 Adobe Advertising에 요청을 보내는 호출입니다. `_les_imsOrgId=[your_imsOrgId_here]&_les_url=[your_encoded_url]`(으)로 시작됩니다.

     Adobe Advertising 호출이 표시되지 않는 경우 방문의 첫 번째 페이지 보기가 아닐 수 있습니다. 테스트 목적으로, 다음 호출이 해당 방문의 첫 번째 페이지 보기가 되도록 쿠키를 제거할 수 있습니다.

   1. 응용 프로그램 탭에서 `adcloud` 쿠키를 찾은 다음 값이 `y`이고 30분 후에 만료되는 UTC 에포크 타임스탬프가 있는 `_les_v`(마지막 방문)이 쿠키에 포함되어 있는지 확인합니다.
      1. `adcloud` 쿠키를 삭제하고 페이지를 새로 고칩니다.

1. (Experience Cloud Identity 서비스 `visitorAPI.js` 코드를 사용하는 구현) Analytics 히트를 보려면 `/b/ss`에서 필터링합니다.

   `/b/ss`![&#128279;](/help/integrations/assets/a4adc-code-validation-filter-bss.png)에서 필터링

1. (Experience Platform [!DNL Web SDK] `alloy.js`코드를 사용하는 구현) `/interact`에서 필터링하여 Edge Network에 대한 요청 페이로드에 `advertisingStitchID`이(가) 포함되어 있는지 확인합니다.

   `/interact`![&#128279;](/help/integrations/assets/a4adc-code-validation-filter-interact.png)에서 필터링

1. Compare the ID values between the two hits. All of the values should be in query string parameters except for the report suite ID in the Analytics hit, which is the URL path immediately after `/b/ss/`.

   | ID | Analytics Parameter | Edge Network | Adobe Advertising Parameter |
   | --- | --- | --- | --- |
   | Experience Cloud IMS Org | `mcorgid` |  | `_les_imsOrgid` |
   | Supplemental Data ID | sdid |  | `_les_sdid` |
   | Stitch ID | stitchId | `advertisingStitchID` under the `_adcloud` property |  |
   | Analytics Report Suite | The value after `/b/ss/` | | `_les_rsid` |
   | Experience Cloud Visitor ID | mid |  | `_les_mid` |

   If the ID values match, then the JavaScript implementation is confirmed. Adobe Advertising sends the [!DNL Analytics] server any click-through or view-through tracking details if they exist.

#### [!DNL Adobe Experience Platform Debugger]을(를) 사용하여 코드를 확인하는 방법

1. Open [the [!DNL Adobe Experience Platform Debugger]](https://experienceleague.adobe.com/docs/debugger/using-v2/summary.html) on your homepage.
1. Go to the [!UICONTROL Network] tab.
1. In the [!UICONTROL Solutions Filter] toolbar, click [!UICONTROL Adobe Advertising] and [!UICONTROL Analytics].
1. In the [!UICONTROL Request URL - Hostname] parameter row, locate `lasteventf-tm.everesttech.net`.
1. In the [!UICONTROL Request - Parameters] row, audit the signals generated, similar to Step 3 in &quot;[How to Confirm the Code with [!DNL Chrome Developer Tools]](#validate-js-chrome).&quot;
   * (Experience Cloud Identity 서비스 `visitorAPI.js` 코드를 사용하는 구현) `Sdid` 매개 변수가 Adobe Analytics 필터의 `Supplemental Data ID`과(와) 일치하는지 확인합니다.
   * (Experience Platform [!DNL Web SDK] `alloy.js`코드를 사용하는 구현) `advertisingStitchID` 매개 변수의 값이 Experience Platform Edge Network에 전송된 `Sdid`과(와) 일치하는지 확인하십시오.
   * 코드가 생성되지 않으면 [!UICONTROL Application] 탭에서 Adobe Advertising 쿠키가 제거되었는지 확인하십시오. 페이지가 제거되면 페이지를 새로 고치고 프로세스를 반복합니다.

   [!DNL Platform Cloud Debugger]![&#128279;](/help/integrations/assets/a4adc-js-audit-debugger.png)에서 [!DNL Analytics for Advertising] JavaScript 코드 감사 

>[!MORELIKETHIS]
>
>* [개요 [!DNL Analytics for Advertising]](overview.md)
>* [구현을 위한 필수 구성 요소 및 키 정보 [!DNL Analytics for Advertising]](prerequisites.md)
