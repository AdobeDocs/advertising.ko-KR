---
title: ' [!DNL Analytics for Advertising]을(를) 구현하기 위한 필수 구성 요소 및 키 정보'
description: ' [!DNL Analytics for Advertising]을(를) 구현하기 위한 필수 구성 요소 및 키 정보'
feature: Integration with Adobe Analytics
exl-id: 7c477900-ebb0-4c0e-811a-ab8bc6069599
source-git-commit: 1559c2cb83e32d90f4b2fe959d07c4e588d9becf
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 0%

---

# [!DNL Analytics for Advertising] 구현을 위한 필수 구성 요소 및 주요 정보

*Advertising DSP 및[!DNL Advertising Search, Social, & Commerce]*&#x200B;을(를) 사용하는 광고주

Adobe Advertising을 Adobe Analytics과 통합하기 전에 다음 정보를 검토하십시오.

## [!DNL Analytics]에서 Adobe Advertising 데이터를 보고하기 위한 요구 사항

* 다음 중 하나를 수행합니다.
   * Adobe Experience Platform 웹 SDK: `alloy.js`
   * Experience Cloud ID 서비스: `visitorAPI.js` 버전 2.0 이상
* 모든 버전의 Adobe Analytics([!DNL Prime], [!DNL Premium] 또는 [!DNL Ultimate] 포함)
* Adobe Analytics: `appMeasurement.js` 버전 2.1 이상
* (Advertising DSP 고객) 뷰스루 방문을 추적하기 위해 웹 페이지에 배포된 [Advertising DSP JavaScript 코드 조각](javascript.md).

>[!TIP]
>
>데이터 충실도를 향상시키려면 각 라이브러리의 최신 버전을 사용하십시오.

## Adobe Advertising과 Analytics 세그먼트 공유를 위한 요구 사항

* Experience Cloud ID 서비스: `visitorAPI.js` 버전 2.1 이상
* Adobe Analytics: `appMeasurement.js` 버전 1.8 이상

## Adobe Advertising에서 [!DNL Analytics] 데이터를 보고하기 위한 요구 사항

Adobe Advertising 구현 팀에 다음 사항을 제공합니다.

* 유료 미디어 활동에 대한 보고 및 최적화 및 Adobe Advertising 보고를 위한 사이트 활동 피딩에 사용할 [!DNL Analytics] 보고서 세트 ID
* 회사의 Experience Cloud 조직 ID(조직 ID).

이 두 ID는 모두 Adobe Experience Cloud Debugger의 [요약 탭](https://experienceleague.adobe.com/docs/debugger/using-v2/summary.html)에서 찾을 수 있습니다.

![Experience Cloud Debugger 요약 화면](/help/integrations/assets/a4adc-debugger-summary.png)

## Adobe Advertising의 [!DNL Analytics] 데이터 {#lookback-a4adc}

보고 및 최적화를 위해 [!DNL Analytics] 데이터가 Adobe Advertising으로 전송되기 때문에 데이터는 Adobe Advertising의 광고주에 대해 구성된 노출 및 클릭 전환 확인 기간을 포함한 속성 규칙의 적용을 받습니다.

![Adobe Advertising의 광고주 수준 전환 확인 기간 설정](/help/integrations/assets/a4adc-lookbacks.png)

* Adobe Advertising 속성 클릭 전환 확인 기간: 전환이 전환으로 귀속될 수 있는 첫 번째 클릭 이후 일 수입니다. 기본적으로 이 값은 60일이며 최대값은 90일입니다
* Adobe Advertising 속성 노출 전환 확인 기간: 광고 노출 발생 후 전환이 노출에 기여할 수 있는 일 수입니다. 기본적으로 이 값은 14일이며 최대값은 30일입니다

  >[!NOTE]
  >
  > 노출 전환 확인 기간은 [!DNL Analytics for Advertising]이(가) 아닌 Adobe Advertising 보고에만 해당됩니다.

[!DNL Analytics for Advertising] JavaScript은 이러한 설정을 사용하여 뷰스루 항목이나 클릭스루 항목을 유효한 항목으로 간주할 이전 시간을 결정합니다. 뷰스루 및 클릭스루를 결정하는 방법에 대한 자세한 내용은 &quot;[Analytics에서 사용하는 Adobe Advertising ID](ids.md)&quot;을(를) 참조하십시오.

## [!DNL Analytics]의 Adobe Advertising 데이터

[!DNL Analytics]은(는) 클릭스루와 뷰스루 모두에 적용되는 광고주의 [!DNL eVar] 지속성 설정에 따라 Analytics 히트 내에 Adobe Advertising ID(AMO ID)를 설정합니다. 지속성 설정은 Adobe Advertising 백 엔드에서 구성되며 Adobe 계정 팀이 변경할 수 있습니다.

* [!DNL Analytics for Advertising] [!DNL eVar] 만료: AMO ID의 경우 기본적으로 60일

>[!NOTE]
>
>다른 기간에 대한 데이터를 세그먼트화하려면 Analysis Workspace 내에서 다른 전환 확인 기간을 사용하여 [사용자 지정 세그먼트를 설정](https://experienceleague.adobe.com/docs/analytics/components/segmentation/segmentation-workflow/seg-build.html)할 수 있습니다.

## 지원되는 광고 환경

* 검색
* 표시
* 비디오
* 온라인 비디오
* 연결된 TV
* 기본

각 채널에서 지원되는 최신 광고 환경은 Adobe 계정 팀에 문의하십시오.

## 구현하기 전에 알아야 할 사항

* Adobe Advertising 구현 팀이 통합을 설정합니다.

* 이 통합에 대해 추가 비용이 청구되지 않으며, 서버 호출로 인해 추가 [!DNL Analytics] 또는 Adobe Advertising 비용이 발생하지 않습니다.

* [!DNL Analytics for Advertising]은(는) 광고 서버에 종속되지 않습니다. 광고 서버에서 뷰스루 또는 클릭스루가 발생할 수 있으며 사이트 시작 시 적절한 ID가 생성됩니다.

* 통합은 [!DNL Analytics]개의 표준 및 사용자 지정 이벤트만 후속 유료 미디어 및 광고 노력의 입찰 최적화를 위한 Adobe Advertising에 전달합니다. [!DNL Analytics]개의 세그먼트, 계산된 지표 및 [!DNL eVars]을(를) 입찰 최적화를 위한 Adobe Advertising에 전달하지 않습니다.

* Adobe Advertising은 Adobe Advertising에 구성된 [클릭 및 뷰스루 전환 확인 기간](#lookback-a4adc)을 기반으로 사용자가 사이트에 들어가기 전에 클릭하거나 본 마지막 광고를 기반으로 [!DNL Analytics] 내에 영구 ID를 만듭니다. 사이트 방문자의 프로필 내에 두 유형의 사이트 시작 상호 작용이 모두 있고 클릭이 전환 확인 기간 내에 있는 경우, 방문자의 클릭스루 ID는 사이트 보고를 위해 뷰스루 ID를 무시합니다.

* Adobe Analytics의 [!DNL Analytics for Advertising] 전환 추적은 구성 가능한 추적 전환 확인 기간(기본적으로 60일)을 사용합니다. Adobe Advertising 보고서는 이 추적 전환 확인 기간의 종료를 통한 사이트 전환 및 참여를 반영합니다.

* 모든 광고 유형이 지원됩니다. <!--Clarify what this might include. It used to include CTV, but not anymore: However, not all ad environments are supported. -->

* [!DNL Analytics] 전환은 현재 추적되며 동일한 장치의 방문자에게만 연결됩니다.

* [!DNL Analytics for Advertising]은(는) 인앱 뷰스루 전환을 지원하지 않습니다.

* [!DNL Analytics]의 서버측 전달 구현을 사용하는 광고주에게는 뷰스루 추적이 지원되지 않습니다.

### 보조 ID

사이트에 대해 Experience Cloud ID 서비스가 구현되면 [!DNL Analytics] 또는 Adobe Advertising의 데이터가 포함된 히트에 보조 ID가 포함됩니다.

예: `sdid=2F3C18E511F618CC-45F83E994AEE93A0`

정확한 데이터 통합을 위해 콘텐츠를 전달하거나 목표 지표를 기록하기 위해 [!DNL Analytics for Advertising] 활동에서 사용하는 모든 Adobe Advertising 호출에는 동일한 보충 ID를 공유하는 해당 [!DNL Analytics] 히트가 있어야 합니다.

[!DNL Analytics]에서 문제를 해결하는 경우 [!DNL Analytics]개의 히트에 대한 보조 ID가 있는지 확인하십시오. [Adobe Experience Cloud Debugger](https://experienceleague.adobe.com/docs/debugger/using-v2/summary.html)에서 이 ID는 Adobe Advertising 탭에서 `sdid` 매개 변수로 표시됩니다.

>[!NOTE]
>
> 이 구현은 [!DNL Analytics for Target] 통합과 유사하게 작동합니다.

>[!MORELIKETHIS]
>
>* [개요 [!DNL Analytics for Advertising]](overview.md)
>* [Advertising용 Analytics용 JavaScript 코드](/help/integrations/analytics/javascript.md)
