---
title: Adobe Advertising과 Customer Journey Analytics 통합을 위한 사전 요구 사항
description: Adobe Advertising과 Customer Journey Analytics 통합을 위한 사전 요구 사항
feature: Integration with Adobe Customer Journey Analytics
exl-id: 4bd14178-5003-4da6-9034-d070c57f0e9b
source-git-commit: ba23ab97c916f829cf9d640669423dd8e72949c0
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---

# Adobe Advertising과 Customer Journey Analytics 통합을 위한 사전 요구 사항

*Advertising DSP 및[!DNL Advertising Search, Social, & Commerce]*&#x200B;을(를) 사용하는 광고주

Adobe Advertising을 Adobe Customer Journey Analytics과 통합하기 전에 다음 정보를 검토하십시오.

## Customer Journey Analytics에서 Adobe Advertising 데이터를 보고하기 위한 요구 사항

* [!DNL Analytics for Advertising]과(와) Customer Journey Analytics을 모두 사용하는 광고주:

   * Adobe Customer Journey Analytics<!-- any specific version? -->

   * [다른 모든 필수 구성 요소 [!DNL Analytics for Advertising]](/help/integrations/analytics/prerequisites.md).

* [!DNL Analytics for Advertising]이(가) 아닌 Customer Journey Analytics을 사용하는 광고주:

   * Adobe Experience Platform 웹 SDK 라이브러리: `alloy.js`

     웹 SDK에 사용되는 [!DNL Org ID]과(와) Adobe Advertising 광고주 계정에 사용되는 은(는) 같아야 합니다. 이 ID는 Adobe Experience Cloud Debugger의 [요약 탭](https://experienceleague.adobe.com/docs/debugger/using-v2/summary.html)에서 찾을 수 있습니다.

     ![Experience Cloud Debugger 요약 화면](/help/integrations/assets/a4adc-debugger-summary.png)

     Experience Platform 데이터 스트림 및 XDM 스키마를 만들려면 Experience Platform 사이트 관리자의 지원이 필요합니다.

   * Adobe Customer Journey Analytics<!-- any specific version? -->

     데이터 세트에 대한 연결을 설정하고 보고를 구성하려면 내부 웹 분석가의 지원이 필요합니다.

>[!TIP]
>
>데이터 충실도를 향상시키려면 각 라이브러리의 최신 버전을 사용하십시오.

>[!MORELIKETHIS]
>
>* [개요](overview.md)
>* (Adobe Analytics 사용자) [Adobe Customer Journey Analytics에서 사용할 AMO ID 및 EF ID에 대한 내역 데이터 수집](/help/integrations/analytics/rvars-to-evars.md).
