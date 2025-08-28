---
title: Adobe Advertising과 Adobe Customer Journey Analytics 간의 통합 개요
description: Adobe Advertising을 Adobe Customer Journey Analytics과 통합하는 옵션에 대해 알아봅니다.
feature: Integration with Adobe Customer Journey Analytics
exl-id: 57636259-f91a-404f-b972-994af67098b1
source-git-commit: b60834569c795013d989fca81c3799165250094b
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Adobe Advertising과 Customer Journey Analytics 간의 통합 개요

<!-- title? If I change, change refs throughout -->

*Advertising DSP 및[!DNL Advertising Search, Social, & Commerce]*&#x200B;을(를) 사용하는 광고주

Adobe Advertising은 양방향 데이터 공유 및 보고를 위해 Adobe Customer Journey Analytics과 통합됩니다. 통합 설정을 위한 두 가지 옵션이 있습니다.

* [!DNL Analytics for Advertising]과(와) Customer Journey Analytics이 모두 있는 광고주는 [!DNL Analytics for Advertising]을(를) 통해 가지고 있는 것과 동일한 기능을 가지며 Customer Journey Analytics의 시각화가 추가되었습니다.

  Adobe Experience Platform Web SDK(`alloy.js`) 또는 Adobe Experience Cloud Identity 서비스(`visitorAPI.js`)를 사용하여 클릭스루 이벤트를 계속 추적하게 됩니다. Advertising DSP을 사용하는 광고주는 여전히 JavaScript 코드 조각을 사용하여 뷰스루 이벤트를 추적합니다. Customer Journey Analytics에서 사용할 수 있는 데이터는 다음과 같습니다.

   * Customer Journey Analytics의 Adobe Advertising에서 캠페인 성과 데이터

   * Customer Journey Analytics의 [!DNL Google Ads], [!DNL Microsoft Advertising] 및 [!DNL Meta]에서 추적한 사이트 활동 및 전환

   * 최적화 및 보고에 사용할 수 있는 Adobe Advertising의 [!DNL Analytics]에서 가져온 속성 데이터입니다.

  이 사용 사례에서는 선택적으로 [Customer Journey Analytics에서 사용할 AMO ID 및 EF ID에 대한 내역 데이터를 수집](/help/integrations/analytics/rvars-to-evars.md)하는 것 외에는 추가 단계를 수행할 필요가 없습니다.

* (예정된 Beta 기능) [!DNL Analytics for Advertising]이(가) 아닌 Customer Journey Analytics을 사용하는 광고주는 기본적으로 [Adobe Experience Platform [!DNL Web SDK]](https://experienceleague.adobe.com/docs/experience-platform/edge/home.html?lang=ko) 라이브러리(`alloy.js`)를 사용하여 Adobe Advertising과 Customer Journey Analytics 간에 데이터를 교환할 수 있습니다. 쿠키, 해시된 IP 및 범용 ID([!DNL LiveRamp RampIDs] 및 ID5 ID)를 사용하여 사이트 이벤트를 추적하고 사이트 이벤트를 유료 미디어 활동에 연결할 수 있습니다. 캠페인, 광고 그룹, 패키지, 배치 및 키워드 수준에서 다음 데이터를 사용할 수 있습니다.

   * Customer Journey Analytics의 Adobe Advertising에서 캠페인 성과 데이터

     **참고:** [!DNL Apple] 및 [!DNL Tiktok]의 데이터를 사용할 수 없습니다.

   * Customer Journey Analytics의 [!DNL Google Ads], [!DNL Microsoft Advertising] 및 [!DNL Meta]에서 추적한 사이트 활동 및 전환

   * 최적화 및 보고에 사용할 수 있는 Adobe Advertising의 Customer Journey Analytics 속성 데이터

  **참고:** 아직 유기 데이터를 사용할 수 없습니다.

  이 사용 사례에서는 웹 SDK을 사용하여 사이트 이벤트(쿠키, 해시된 IP 주소 또는 범용 ID 사용)를 추적하고 사이트 이벤트를 [!DNL Google Ads], [!DNL Microsoft Advertising] 및 [!DNL Meta]의 유료 미디어 활동과 Adobe DSP에 연결합니다. 데이터 수집에도 Adobe Experience Platform을 사용합니다.

## Adobe Advertising과 Customer Journey Analytics 간의 기본 통합을 시작하는 방법

시작하는 데 필요한 초기 구성을 완료하고 조직의 요구 사항에 따라 구현 및 데이터 사용을 계획하는 데 도움이 되는 Adobe 계정 팀에 문의하십시오.

>[!MORELIKETHIS]
>
>* [필수 구성 요소](prerequisites.md)
>* (Adobe Analytics 사용자) [Adobe Customer Journey Analytics에서 사용할 AMO ID 및 EF ID에 대한 내역 데이터 수집](/help/integrations/analytics/rvars-to-evars.md).
