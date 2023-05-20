---
title: 사용 [!DNL Last Event Service] 을 사용하는 JavaScript 라이브러리 [!DNL Web SDK]
description: 을(를) 사용하여에서 전환하는 단계에 대해 알아봅니다. [!DNL Analytics] [!DNL visitorAPI] 라이브러리 대상 [!DNL Experience Platform] [!DNL Web SDK] 라이브러리 [!DNL Analytics for Advertising] 구현.
feature: Integration with Adobe Analytics
exl-id: 764724a2-536a-43b9-955d-28d6146db29a
source-git-commit: 7e614ecb517515217d812926f61ca10437820efd
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---

# 사용 [!DNL Last Event Service] Adobe Experience Platform이 포함된 JavaScript 라이브러리 [!DNL Web SDK]

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

조직에서 기존 Adobe Analytics을 사용하는 경우 `visitorAPI.js` 데이터 수집을 위한 라이브러리에서는 필요한 경우 [Adobe Experience Platform [!DNL Web SDK]](https://experienceleague.adobe.com/docs/experience-platform/edge/home.html) 라이브러리 (`alloy.js`)를 사용하여 를 통해 다양한 Experience Cloud 서비스와 상호 작용할 수 있습니다 [!DNL Edge Network].

다음 [!DNL Analytics for Advertising] [!DNL Last Event Service] JavaScript 라이브러리(있는 그대로)는 뷰스루 및 클릭스루 이벤트를 기록하고 보조 ID( )를 사용하여 연결된 전환에 결합합니다.`SDID`). 다음 [!DNL Web SDK] 그러나 라이브러리는 를 제공하지 않습니다. [!DNL stitch ID]. 을(를) 사용하려면 [!DNL Web SDK] 대상 [!DNL Analytics for Advertising], 1) 을 수정해야 합니다. [!DNL Last Event Service] 웹 페이지에서 사용하는 태그 및 2) [!DNL Web SDK] `sendEvent` 그에 따라 명령합니다.

## 1단계: 편집 [!DNL Last Event Service] 태그를 생성하여 `[!DNL StitchID]`

다음에서 [!DNL Analytics for Advertising] [!DNL Last Event Service] 웹 페이지에서 를 사용하는 태그에 코드를 추가하여 `[!DNL StitchID]` 라이브러리에 번들로 제공된 임의 ID 생성기 사용.

**기존 태그:**

```
<script>
     if("undefined" != typeof AdCloudEvent) 
          AdCloudEvent('IMS ORG Id');
</script>
```

**새 태그:**

```
<script>
     if("undefined" != typeof AdCloudEvent) 
          stitchId = AdCloudEvent('IMS ORG Id').generateRandomId();
</script>
```

## 2단계: 사용 [!DNL Web SDK] 보내기 [!DNL StitchID] 를 XDM 데이터로 사용 [!DNL Analytics]

다음 속성을 [!DNL Web SDK] `sendEvent` 보내기 명령 [!DNL StitchID] 끝 [!DNL Experience Edge] 다음으로: [!DNL Experience Data Model] 다음에 대한 (XDM) 데이터 [!DNL Analytics].<!-- The library will send the StitchID to [!DNL Experience Edge] as `[_adcloud.advertisingStitchID](https://github.com/adobe/xdm/blob/master/docs/reference/adobe/experience/adcloud/stitch.schema.md)`. --> [!DNL Analytics] 은(는) 값을 (으)로 사용합니다. `SDID`.

**추가할 속성:**

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
>* [용 JavaScript 코드 [!DNL Analytics for Advertising]](/help/integrations/analytics/javascript.md)

