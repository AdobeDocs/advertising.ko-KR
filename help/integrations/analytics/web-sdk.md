---
title: Using the [!DNL Last Event Service] JavaScript library with [!DNL Web SDK]
description: Learn the steps to switch from using the [!DNL Analytics] [!DNL visitorAPI] library to the [!DNL Experience Platform] [!DNL Web SDK] library for your [!DNL Analytics for Advertising] implementation.
feature: Integration with Adobe Analytics
exl-id: 764724a2-536a-43b9-955d-28d6146db29a
TQID: https://experienceleague.adobe.com/zT1lQV1yotCfJJdzTBGzSspsNEKQEB5ulxYE0qyWa9Q
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2:
  - id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: d3cdead0-685a-4489-9250-4bb709942f66
source-git-commit: 7845129ba6566c1aaaf160cc6f9ad33bf1731f75
workflow-type: tm+mt
source-wordcount: 202
ht-degree: 0%

---

# Adobe Experience Platform [!DNL Web SDK]에서 [!DNL Last Event Service] JavaScript 라이브러리 사용

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

If your organization uses the legacy Adobe Analytics `visitorAPI.js` library for data collection, you can optionally switch to using the [Adobe Experience Platform [!DNL Web SDK]](https://experienceleague.adobe.com/docs/experience-platform/edge/home.html?lang=ko) library (`alloy.js`), which allows you to interact with the various Adobe CX Enterprise services through the [!DNL Edge Network].

[!DNL Analytics for Advertising] [!DNL Last Event Service] JavaScript 라이브러리는 있는 그대로 뷰스루 및 클릭스루 이벤트를 기록하고 보조 ID(`SDID`)를 사용하여 연결된 전환에 결합합니다. 그러나 [!DNL Web SDK] 라이브러리는 [!DNL stitch ID]을(를) 제공하지 않습니다. [!DNL Analytics for Advertising]에 대해 [!DNL Web SDK]을(를) 사용하려면 1) 웹 페이지에서 사용하는 [!DNL Last Event Service] 태그와 2) [!DNL Web SDK] `sendEvent` 명령을 적절하게 수정해야 합니다.

## Step 1: Edit your [!DNL Last Event Service] tag to generate a `[!DNL StitchID]`

웹 페이지에서 사용하는 [!DNL Analytics for Advertising] [!DNL Last Event Service] 태그에서 라이브러리에 번들로 제공된 임의의 ID 생성기를 사용하여 `[!DNL StitchID]`을(를) 생성하는 코드를 추가하십시오.

**기존 태그:**

```
<script>
     if("undefined" != typeof AdCloudEvent) 
          AdCloudEvent('IMS ORG Id','rsid');
</script>
```

**새 태그:**

```
<script>
     if("undefined" != typeof AdCloudEvent) 
          stitchId = AdCloudEvent('IMS ORG Id','rsid').generateRandomId();
</script>
```

## Step 2: Use [!DNL Web SDK] to send the [!DNL StitchID] as XDM data for [!DNL Analytics]

Insert the following property within your [!DNL Web SDK] `sendEvent` command to send the [!DNL StitchID] to [!DNL Experience Edge] as [!DNL Experience Data Model] (XDM) data for [!DNL Analytics].<!-- The library sends the StitchID to [!DNL Experience Edge] as `[_adcloud.advertisingStitchID](https://github.com/adobe/xdm/blob/master/docs/reference/adobe/experience/adcloud/stitch.schema.md)`. --> [!DNL Analytics]이(가) 값을 `SDID`(으)로 사용합니다.

추가할 **속성:**

```
     "_adcloud": {
       "advertisingStitchID": stitchId
     }
```

**예:**

```
<script>
  alloy("sendEvent", {
    "xdm": {
      "commerce": {
        "order": {
                ………
        }
     },
     "_adcloud": {
       "advertisingStitchID": stitchId
     }
    }
  });
</script>
```

>[!MORELIKETHIS]
>
>* [개요 [!DNL Analytics for Advertising]](overview.md)
>*  [!DNL Analytics for Advertising][&#128279;](/help/integrations/analytics/javascript.md)에 대한 JavaScript 코드
