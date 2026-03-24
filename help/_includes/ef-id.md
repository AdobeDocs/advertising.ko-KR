---
source-git-commit: 546e391745b1469efbcc9c2024dfc193224f0ed0
workflow-type: tm+mt
source-wordcount: '160'
ht-degree: 0%

---
# Adobe Advertising

## Adobe Advertising

EF ID는 Adobe Advertising이 활동을 개별 브라우저 또는 장치 수준에서 온라인 클릭 또는 광고 노출과 연결하는 데 사용하는 고유한 토큰입니다. EF ID는 주로 Adobe Advertising 내에서 보고 및 입찰 최적화를 위해 [!DNL Analytics] 데이터 및 Customer Journey Analytics 데이터를 Adobe Advertising에 전송하는 키 역할을 합니다.

[!DNL Analytics]의 경우 EF ID는 [an [!DNL Analytics] [!DNL eVar]](https://experienceleague.adobe.com/docs/analytics/components/dimensions/evar.html) 또는 [!DNL rVar]&#x200B;(예약된 [!DNL eVar]) 차원(Adobe Advertising EF ID)에 저장됩니다.

Customer Journey Analytics의 경우 EF ID는 `trackingIdentities` `conversionDetails`[의 일부인 [!UICONTROL Adobe Advertising Cloud ExperienceEvent Full Extension] 개체의 &#x200B;](https://experienceleague.adobe.com/en/docs/experience-platform/xdm/field-groups/event/advertising-full-extension) 속성에 저장됩니다.

### EF ID 형식 {#ef-id-formats}

&quot;Adobe Analytics 구성 요소 안내서&quot;에서 [EF ID 차원 항목에 대한 형식](https://experienceleague.adobe.com/en/docs/analytics/components/dimensions/amo-ef-id#dimension-items)을 참조하십시오.

>[!NOTE]
>
>EF ID는 대/소문자를 구분합니다. [!DNL Analytics] 또는 Customer Journey Analytics 구현에서 URL 추적을 소문자로 강제하는 경우 Adobe Advertising에서 EF ID를 인식하지 못합니다. 이는 Adobe Advertising 입찰 및 보고에 영향을 주지만 [!DNL Analytics] 또는 Customer Journey Analytics 내의 Adobe Advertising 보고에는 영향을 주지 않습니다.

<!-- Legacy content:

#### [!DNL Google Ads] search ads

```
{gclid}:G:s
```

where:

* `gclid` is the [!DNL Google Click ID] (GCLID).
* `s` is the network type ("s" for search).

#### [!DNL Microsoft Advertising] search ads

```
{msclkid}:G:s
```

where:

* `msclkid` is the [!DNL Microsoft Click ID] (MSCLKID).
* `s` is the network type ("s" for search).

#### Display ads and search ads on other search engines 

```
<Adobe Advertising visitor ID>:<timestamp>:<channel type>
```

where:

* <*Adobe Advertising visitor ID*> is a unique ID per visitor (such as UhKVaAAABCkJ0mDt). Also called the *surfer ID*.

* <*timestamp*> is the time in the format YYYYMMDDHHMMSS (such as 20190821192533 for Year 2019, Month 08, Day 21, Time 19:25:33).

* <*channel type*> is the channel type responsible for the click or exposure:

    * `d` for a click on a DSP display ad (display click-through)
    * `i` for an impression of a DSP display ad (display view-through)
    * `s` for a click on a Search ad (search click-through).

Example `EF ID: WcmibgAAAHJK1RyY:1551968087687:d`

-->
