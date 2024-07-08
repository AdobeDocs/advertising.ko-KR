---
title: 구현을 위한 전제 조건 및 주요 정보 [!DNL Analytics for Advertising]
description: 구현을 위한 전제 조건 및 주요 정보 [!DNL Analytics for Advertising]
feature: Integration with Adobe Analytics
exl-id: 7c477900-ebb0-4c0e-811a-ab8bc6069599
source-git-commit: 8481227a8ccb1f1e6e715e34e14732967110c168
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 0%

---

# 구현을 위한 전제 조건 및 주요 정보 [!DNL Analytics for Advertising]

*광고 DSP 및[!DNL Advertising Search, Social, & Commerce]*

Adobe Systems Advertising을 Adobe Analytics와 통합하기 전에 다음 정보를 검토하십시오.

## 에서 Adobe Systems 광고 데이터를 보고하기 위한 요구 사항 [!DNL Analytics]

* 다음 중 하나입니다.
   * Adobe Experience Platform 웹 SDK: `alloy.js`
   * Experience Cloud Identity 서비스: `visitorAPI.js` 버전 2.0 이상
* 모든 Adobe Analytics 버전( [!DNL Prime], [!DNL Premium], 또는 [!DNL Ultimate])
* Adobe Analytics: `appMeasurement.js` 버전 2.1 이상
* (광고 DSP 고객) [뷰스루 방문을 추적하기 위해 웹 페이지에 배포되는 Advertising DSP JavaScript 스니펫](javascript.md) 입니다.

>[!TIP]
>
>데이터 충실도를 향상시키려면 각 라이브러리의 최신 버전을 사용합니다.

## Analytics 세그먼트를 Adobe Systems Advertising과 공유하기 위한 요구 사항

* Experience Cloud Identity 서비스: `visitorAPI.js` 버전 2.1 이상
* Adobe Analytics: `appMeasurement.js` 버전 1.8 이상

## Adobe Systems Advertising에서 데이터를 보고 [!DNL Analytics] 하기 위한 요구 사항

Adobe Systems Advertising 구현 팀에 다음을 제공합니다.

* Adobe Systems [!DNL Analytics] 광고에서 최적화 및 보고를 위해 페이드 미디어 활동을 보고하고 사이트 활동을 공급하는 데 사용할 보고서 세트 ID입니다.
* 회사의 Experience Cloud 조직 ID(조직 ID)입니다.

Adobe Experience Cloud 디버거의 요약 탭에서 이 두 ID [를 모두 찾을 수 있습니다](https://experienceleague.adobe.com/docs/debugger/using-v2/summary.html).

![Experience Cloud 디버거 요약 화면](/help/integrations/assets/a4adc-debugger-summary.png)

## [!DNL Analytics] Adobe Systems 광고의 데이터 {#lookback-a4adc}

데이터는 보고 및 최적화를 위해 Adobe Systems Advertising으로 전송되기 때문에 [!DNL Analytics] 데이터는 Adobe Systems Advertising에서 광고주에 대해 구성된 노출 횟수 및 클릭 전환 확인 기간을 포함한 기여도 분석 규칙의 적용을 받습니다.

![Adobe Systems Advertising의 광고주 수준 전환 확인 기간 설정](/help/integrations/assets/a4adc-lookbacks.png)

* Adobe Systems 광고 기여도 분석 클릭 전환 확인 기간: 첫 번째 클릭이 발생한 후 클릭이 전환으로 귀속될 수 있는 일 수입니다. 기본적으로 이 값은 60일입니다. 최댓값은 90일입니다
* Adobe Systems 광고 기여도 분석 노출 횟수 전환 확인 기간: 광고 노출 횟수 발생 후 노출 횟수이 전환에 기인할 수 있는 기간(일)입니다. 기본적으로 이 값은 14일입니다. 최댓값은 30일입니다

  >[!NOTE]
  >
  > 노출 횟수 전환 확인 기간은 보고가 아니라 [!DNL Analytics for Advertising]Adobe Systems 광고에만 적용됩니다.

JavaScript 는 [!DNL Analytics for Advertising] 이러한 설정을 사용하여 사이트에 대한 뷰스루 항목 또는 클릭스루 항목을 유효한 것으로 간주할 수 있는 시간을 결정합니다. 뷰스루 및 클릭스루를 결정하는 방법에 대한 자세한 내용은 &quot;[Analytics](ids.md)에서 사용하는 Adobe Systems 광고 ID&quot;를 참조하십시오.

## Adobe Systems의 Adobe Systems 광고 데이터 [!DNL Analytics]

[!DNL Analytics] 는 클릭스루와 뷰스루 모두에 적용되는 광고주의 [!DNL eVar] 지속성 설정에 따라 Analytics 히트 내에서 Adobe Systems 광고 ID(AMO ID)를 설정합니다. 지속성 설정은 Adobe Systems Advertising 백엔드에서 구성되며 Adobe Systems 계정 팀에서 변경할 수 있습니다.

* [!DNL Analytics for Advertising][!DNL eVar] 만료: AMO ID의 경우 기본적으로 60일

>[!NOTE]
>
>다른 일정에 대한 데이터를 세그먼트하려면 Analysis Workspace 내에서 다른 전환 확인 기간으로 사용자 지정 세그먼트를](https://experienceleague.adobe.com/docs/analytics/components/segmentation/segmentation-workflow/seg-build.html) 설정할 수 있습니다[.

## 지원되는 광고 환경

* 검색
* 전시
* 비디오
* 온라인 비디오
* 커넥티드 TV
* 원주민

각 채널에서 지원되는 최신 광고 환경에 대해서는 Adobe Systems 계정 팀에 문의하십시오.

## 구현하기 전에 알아야 할 사항

* Adobe Systems Advertising 구현 팀에서 통합을 설정합니다.

* 이 통합에 대한 추가 비용은 청구되지 않으며, 서버 호출로 인해 추가 [!DNL Analytics] 또는 Adobe Systems 광고 요금이 발생하지 않습니다.

* [!DNL Analytics for Advertising] 광고 서버에 구애받지 않음: 모든 광고 서버에서 뷰스루 또는 클릭스루가 발생할 수 있으며 사이트 진입 시 적절한 ID가 생성됩니다.

* 통합은 후속 페이드 미디어 및 광고 노력의 입찰 최적화를 위해 표준 및 사용자 지정 이벤트만 [!DNL Analytics] Adobe Systems Advertising에 전달합니다. 세그먼트, 계산된 지표 및 [!DNL eVars] 입찰 최적화를 위해 Adobe Systems Advertising에 전달 [!DNL Analytics] 하지 않습니다.

* Adobe Systems Advertising은 사용자 Advertising에 구성된 클릭 및 뷰스루 전환 확인 기간을](#lookback-a4adc) 기반으로 [사용자 이전에 클릭하거나 본 마지막 광고를 기반으로 내에 [!DNL Analytics] 영구 ID를 만듭니다. 사이트 방문자의 프로필 내에 두 가지 유형의 사이트 항목 상호 작용이 모두 있고 클릭이 전환 확인 기간 내에 있는 경우 방문자의 클릭스루 ID가 사이트 보고를 위한 뷰스루 ID를 재정의합니다.

* [!DNL Analytics for Advertising] Adobe Analytics의 전환 추적은 구성 가능한 추적 전환 확인 기간(기본적으로 60일)을 사용합니다. Adobe Systems 광고 보고서는 이 추적 전환 확인 기간이 끝날 때까지 사이트 전환 및 참여 수를 반영합니다.

* 모든 광고 유형이 지원됩니다. 그러나 일부 광고 환경은 지원되지 않습니다.

* [!DNL Analytics] 현재 전환이 추적되고 동일한 디바이스 사용자의 방문자에게만 귀속됩니다.

* [!DNL Analytics for Advertising] 에서 인앱 뷰스루 전환을 지원하지 않습니다.

* 보기스루 추적은 의 [!DNL Analytics]서버측 전달 구현을 사용하는 광고주에 대해 지원되지 않습니다.

### 보충 ID

사이트에 대해 Experience Cloud Identity 서비스가 구현되면 광고 데이터를 [!DNL Analytics] 포함하는 히트Adobe Systems 보충 ID가 포함됩니다.

본보기: `sdid=2F3C18E511F618CC-45F83E994AEE93A0`

정확한 데이터 통합을 위해 활동에서 [!DNL Analytics for Advertising] 컨텐츠를 전달하거나 목표 지표를 기록하는 데 사용하는 모든 Adobe Systems 광고 호출에는 동일한 보충 ID를 공유하는 해당 [!DNL Analytics] 히트가 있어야 합니다.

에서 [!DNL Analytics]문제를 해결할 때 히트에 대한 [!DNL Analytics] 보충 ID가 있는지 확인하십시오. [Adobe Experience Cloud 디버거](https://experienceleague.adobe.com/docs/debugger/using-v2/summary.html)의 경우 Adobe Systems 광고 탭에서 이 ID를 매개 변수로 `sdid` 볼 수 있습니다.

>[!NOTE]
>
> 이 구현 작업은 통합과 유사하게 [!DNL Analytics for Target] 이루어집니다.

>[!MORELIKETHIS]
>
>* [개요 [!DNL Analytics for Advertising]](overview.md)
>* [광고용 Analytics용 JavaScript Code](/help/integrations/analytics/javascript.md)
