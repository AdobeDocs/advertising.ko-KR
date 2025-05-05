---
title: ' [!DNL Marketing Channels]의 기본 사항'
description: ' [!DNL Analytics for Advertising] 사용자가 이해해야 하는  [!DNL Analytics Marketing Channels] 에 대한 주요 정보를 알아봅니다.'
feature: Integration with Adobe Analytics
exl-id: de02dff5-86ce-41e8-89c6-3c11f6375b77
source-git-commit: 29b49e8fa54580d7cdd62f9a10fd2616def4694b
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# [!DNL Analytics Marketing Channels]의 기본 사항

이 페이지에서는 [!DNL Analytics for Advertising] 사용자가 이해해야 하는 [!DNL Analytics Marketing Channels]에 대한 주요 정보를 설명합니다.

[!DNL Marketing Channels]에 대한 전체 설명서는 &quot;[시작하기 [!DNL Marketing Channels]](https://experienceleague.adobe.com/docs/analytics/components/marketing-channels/c-getting-started-mchannel.html?lang=ko)&quot;를 참조하십시오.

## [!DNL Marketing Channels] 개요

[!DNL Marketing Channels]은(는) Adobe Analytics의 주요 기능입니다. [!DNL Marketing Channels] 보고서는 고객이 보고 기간 동안 웹 사이트에 도착하는 방법과 각 채널이 매출이나 현장 동작에 미치는 영향을 보여줍니다.

교차 방문 여정의 다음 예를 생각해 보십시오. 웹 사이트에 대한 각 방문은 방문자가 시작한 마케팅 채널에 의해 표시됩니다. 첫 번째 터치 채널이라고도 하는 첫 번째 방문은 이메일입니다. 방문 2에 표시되는 것은 참여 채널이며, 자연어 검색은 마지막 터치 채널로 간주됩니다. [!UICONTROL Attribution IQ] 내에서 [!UICONTROL Last Touch Attribution]을(를) 사용하는 경우 자연어 검색은 $250 전환 이벤트에 대한 전체 크레딧을 받습니다. Experience Cloud ID 서비스를 사용하면 이러한 개별 방문을 함께 연결하여 단일 방문자에 의해 하나의 여정을 표시할 수 있습니다.

![마케팅 채널의 교차 방문 전환 여정 예](/help/integrations/assets/a4adc-mc-sample-journey.png)

[!UICONTROL Marketing Channels] 처리 규칙을 사용하여 트래픽을 유도하는 채널을 결정하고 사용자가 사이트를 방문할 때 각 채널을 추적하는 논리 집합을 만들 수 있습니다. 예를 들어 [!UICONTROL Email] 채널은 Adobe Analytics에 의해 기록될 때 이메일 마케팅 캠페인에서 시작된 방문으로 분류하는 클릭 시 생성된 고유한 추적 코드로 표시됩니다.

## 처리 규칙 및 마케팅 채널 설정 방법

사용자가 웹 사이트를 방문할 때마다 URL을 통해 클릭하거나 주소 표시줄에 직접 입력해야 합니다. 사용자가 웹 사이트로 이동하면 [!DNL Analytics]은(는) 방문을 유도한 채널을 판별하는 데 사용할 수 있는 정보를 추적합니다.

종종 마케터는 쿼리 문자열 매개 변수 추적 코드를 채널 URL에 추가하여 채널이 사이트에 미치는 영향을 추적합니다. 추가 추적 없이 채널을 결정하기 위해 특정 추적 매개 변수 및 값을 수신하도록 [!DNL Marketing Channels] 처리 규칙을 구성할 수 있습니다. 예를 들어 모든 이메일 캠페인 URL이 `www.adobe.com?cid=email…` 형식을 따르는 경우(URL에 쿼리 문자열 매개 변수와 값 `cid=email`이(가) 있으면) 이 추적 코드를 수신하고 [!UICONTROL Email] 채널에서 방문을 버킷하는 규칙을 만들 수 있습니다.

다른 채널에는 추적 가능한 URL 경로가 없으며 식별을 위해 추가 논리가 필요합니다. 예를 들어 다른 사용자가 소셜 네트워크에서 유기적으로 공유한 링크를 사용자가 클릭하는 [!UICONTROL Earned Social]은(는) 추적해야 할 중요한 채널입니다. 그러나 마케터는 쿼리 문자열 매개 변수 추적 코드를 공유된 URL에 추가할 수 없습니다. 이 경우 관심 있는 소셜 네트워크의 참조 도메인과 유료 추적 코드의 부재를 수신하여 채널을 확인하는 처리 규칙을 만들 수 있습니다. 그런 다음 이러한 요구 사항을 충족하는 방문은 마케팅 채널 보고서 내에서 Earned Social으로 추적됩니다.

Adobe은 분석 팀과 함께 귀하의 비즈니스와 관련된 모든 채널을 추적하는 포괄적인 [!DNL Marketing Channels] 처리 규칙 세트를 작성할 것을 권장합니다. 이렇게 하면 강력한 속성 보고를 생성할 수 있습니다.

Adobe Advertising이 사용자 지정 마케팅 채널을 만드는 데 필요한 신호에 어떻게 기여할 수 있는지 이해하려면 &quot;[Advertising ID를 사용하여 만들기 [!DNL Marketing Channels] 규칙](mc-ids.md)&quot;을 참조하세요.

>[!MORELIKETHIS]
>
>* [Adobe Advertising ID를 사용하여 만들기 [!DNL Marketing Channels] 처리 규칙](mc-ids.md)
>* [Adobe Advertising 데이터와 채널 데이터가 서로 다를 수 있는 이유 [!DNL Marketing Channels]](mc-data-variances.md)
>* [Adobe Advertising 데이터로  [!DNL Analytics Marketing Channels] 사용](mc-ac-data.md)
>* [비디오: Adobe Advertising 보고에  [!DNL Marketing Channels] 사용](https://experienceleague.adobe.com/docs/advertising-learn/tutorials/analytics/analytics-reporting-a4adc.html?lang=ko)
>* [개요 [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md)
