---
source-git-commit: d1e2e92532b1f930420436c66c687676a2b7de6a
workflow-type: tm+mt
source-wordcount: '93'
ht-degree: 0%

---
# Adobe Advertising

EF ID는 Adobe Advertising이 활동을 개별 브라우저 또는 장치 수준에서 온라인 클릭 또는 광고 노출과 연결하는 데 사용하는 고유한 토큰입니다. EF ID는 주로 Adobe Advertising 내에서 보고 및 입찰 최적화를 위해 [!DNL Analytics] 데이터 및 Customer Journey Analytics 데이터를 Adobe Advertising에 전송하는 키 역할을 합니다.

[!DNL Analytics]의 경우 EF ID는 [an [!DNL Analytics] [!DNL eVar]](https://experienceleague.adobe.com/docs/analytics/components/dimensions/evar.html?lang=ko) 또는 [!DNL rVar]&#x200B;(예약된 [!DNL eVar]) 차원(Adobe Advertising EF ID)에 저장됩니다.

Customer Journey Analytics의 경우 EF ID는 `trackingIdentities`의 일부인 `conversionDetails` 개체의 [!UICONTROL Adobe Advertising Cloud ExperienceEvent Full Extension] 속성에 저장됩니다.
