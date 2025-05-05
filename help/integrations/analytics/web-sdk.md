---
title: ' [!DNL Web SDK]에서  [!DNL Last Event Service] JavaScript 라이브러리 사용'
description: ' [!DNL Analytics for Advertising] 구현을 위해  [!DNL Analytics] [!DNL visitorAPI] 라이브러리에서  [!DNL Experience Platform] [!DNL Web SDK] 라이브러리로 전환하는 단계에 대해 알아봅니다.'
feature: Integration with Adobe Analytics
exl-id: 764724a2-536a-43b9-955d-28d6146db29a
source-git-commit: e517dd5f5fa283ff8a2f57728612937148889732
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# Adobe Experience Platform [!DNL Web SDK]에서 [!DNL Last Event Service] JavaScript 라이브러리 사용

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

조직에서 데이터 수집을 위해 레거시 Adobe Analytics `visitorAPI.js` 라이브러리를 사용하는 경우 선택적으로 [!DNL Edge Network]을(를) 통해 다양한 Experience Cloud 서비스와 상호 작용할 수 있는 [Adobe Experience Platform [!DNL Web SDK]](https://experienceleague.adobe.com/docs/experience-platform/edge/home.html) 라이브러리(`alloy.js`)를 사용하는 것으로 전환할 수 있습니다.

[!DNL Analytics for Advertising] [!DNL Last Event Service] JavaScript 라이브러리는 있는 그대로 뷰스루 및 클릭스루 이벤트를 기록하고 보조 ID(`SDID`)를 사용하여 연결된 전환에 결합합니다. 그러나 [!DNL Web SDK] 라이브러리는 [!DNL stitch ID]을(를) 제공하지 않습니다. [!DNL Analytics for Advertising]에 대해 [!DNL Web SDK]을(를) 사용하려면 1) 웹 페이지에서 사용하는 [!DNL Last Event Service] 태그와 2) [!DNL Web SDK] `sendEvent` 명령을 적절하게 수정해야 합니다.

## 1단계: [!DNL Last Event Service] 태그를 편집하여 `[!DNL StitchID]` 생성

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

## 2단계: [!DNL Web SDK]을(를) 사용하여 [!DNL Analytics]에 대한 XDM 데이터로 [!DNL StitchID]을(를) 보냅니다.

[!DNL Web SDK] `sendEvent` 명령 내에 다음 속성을 삽입하여 [!DNL Analytics]에 대한 [!DNL Experience Data Model] (XDM) 데이터로 [!DNL Experience Edge]에 [!DNL StitchID]을(를) 보냅니다.<!-- The library sends the StitchID to [!DNL Experience Edge] as `[_adcloud.advertisingStitchID](https://github.com/adobe/xdm/blob/master/docs/reference/adobe/experience/adcloud/stitch.schema.md)`. --> [!DNL Analytics]이(가) 값을 `SDID`(으)로 사용합니다.

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
>* [JavaScript 코드  [!DNL Analytics for Advertising]](/help/integrations/analytics/javascript.md)
