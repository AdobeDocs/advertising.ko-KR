---
title: 의 기본 사항 [!DNL Marketing Channels]
description: 에 대한 주요 정보 알아보기 [!DNL Analytics Marketing Channels] that [!DNL Analytics for Advertising] 사용자가 이해해야 합니다.
feature: Integration with Adobe Analytics
exl-id: de02dff5-86ce-41e8-89c6-3c11f6375b77
source-git-commit: 29b49e8fa54580d7cdd62f9a10fd2616def4694b
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# 의 기본 사항 [!DNL Analytics Marketing Channels]

이 페이지에서는 다음에 대한 주요 정보를 설명합니다. [!DNL Analytics Marketing Channels] that [!DNL Analytics for Advertising] 사용자가 이해해야 합니다.

에 대한 전체 설명서 [!DNL Marketing Channels], 참조 &quot;[시작 [!DNL Marketing Channels]](https://experienceleague.adobe.com/docs/analytics/components/marketing-channels/c-getting-started-mchannel.html).&quot;

## 개요 [!DNL Marketing Channels]

[!DNL Marketing Channels] 는 Adobe Analytics의 주요 기능입니다. [!DNL Marketing Channels] 보고서는 고객이 보고 기간을 통해 웹 사이트에 도달하는 방식과 각 채널이 매출이나 현장 동작에 미치는 영향을 보여줍니다.

교차 방문 여정의 다음 예를 생각해 보십시오. 웹 사이트에 대한 각 방문은 방문자가 시작한 마케팅 채널에 의해 표시됩니다. 첫 번째 터치 채널이라고도 하는 첫 번째 방문은 이메일입니다. 방문 2에 표시되는 것은 참여 채널이며, 자연어 검색은 마지막 터치 채널로 간주됩니다. 를 사용하는 경우 [!UICONTROL Last Touch Attribution] 다음 범위 내 [!UICONTROL Attribution IQ], 자연어 검색은 $250 전환 이벤트에 대한 전체 크레딧을 받습니다. Experience Cloud ID 서비스를 사용하면 이러한 개별 방문을 함께 연결하여 단일 방문자에 의해 하나의 여정을 표시할 수 있습니다.

![마케팅 채널의 교차 방문 전환 여정 예](/help/integrations/assets/a4adc-mc-sample-journey.png)

사용 [!UICONTROL Marketing Channels] 처리 규칙 을 사용하면 트래픽을 유도하는 채널을 결정하고 사용자가 사이트를 방문할 때 각 채널을 추적하는 논리 세트를 만들 수 있습니다. 예를 들어 [!UICONTROL Email] 채널은 클릭 시 생성된 고유한 추적 코드에 의해 표시되며, Adobe Analytics에 의해 기록되면 방문이 이메일 마케팅 캠페인에서 시작된 것으로 분류됩니다.

## 처리 규칙 및 마케팅 채널 설정 방법

사용자가 웹 사이트를 방문할 때마다 URL을 통해 클릭하거나 주소 표시줄에 직접 입력해야 합니다. 사용자가 웹 사이트에 들어오면, [!DNL Analytics] 방문을 유도한 채널을 확인하는 데 사용할 수 있는 정보를 추적합니다.

종종 마케터는 쿼리 문자열 매개 변수 추적 코드를 채널 URL에 추가하여 채널이 사이트에 미치는 영향을 추적합니다. 다음을 구성할 수 있습니다. [!DNL Marketing Channels] 처리 규칙 을 사용하여 특정 추적 매개 변수 및 값을 수신하여 추가 추적 없이 채널을 결정합니다. 예를 들어 모든 이메일 캠페인 URL이 형식을 따르는 경우 `www.adobe.com?cid=email…` (여기서 URL은 쿼리 문자열 매개 변수와 값을 포함합니다.) `cid=email`)를 설정하는 경우, 이 추적 코드를 수신하고 [!UICONTROL Email] 채널.

다른 채널에는 추적 가능한 URL 경로가 없으며 식별을 위해 추가 논리가 필요합니다. 예를 들어, [!UICONTROL Earned Social]- 소셜 네트워크에서 다른 사용자가 유기적으로 공유한 링크를 클릭하는 것은 추적해야 할 중요한 채널입니다. 그러나 마케터는 쿼리 문자열 매개 변수 추적 코드를 공유된 URL에 추가할 수 없습니다. 이 경우 관심 있는 소셜 네트워크의 참조 도메인과 유료 추적 코드의 부재를 수신하여 채널을 확인하는 처리 규칙을 만들 수 있습니다. 그런 다음 이러한 요구 사항을 충족하는 방문은 마케팅 채널 보고서 내에서 Earned Social으로 추적됩니다.

Adobe은 분석 팀과 함께 포괄적인 집합 구성을 권장합니다. [!DNL Marketing Channels] 처리 규칙을 사용하여 비즈니스와 관련된 모든 채널을 추적합니다. 이렇게 하면 강력한 속성 보고를 생성할 수 있습니다.

Adobe Advertising이 사용자 지정 마케팅 채널을 만드는 데 필요한 신호에 어떻게 기여할 수 있는지 이해하려면 &quot;[광고 ID를 사용하여 만들기 [!DNL Marketing Channels] 규칙](mc-ids.md).&quot;

>[!MORELIKETHIS]
>
>* [Adobe Advertising ID를 사용하여 만들기 [!DNL Marketing Channels] 처리 규칙](mc-ids.md)
>* [Adobe Advertising과 간에 채널 데이터가 다를 수 있는 이유 [!DNL Marketing Channels]](mc-data-variances.md)
>* [사용 [!DNL Analytics Marketing Channels] Adobe Advertising 데이터 포함](mc-ac-data.md)
>* [비디오: 사용 [!DNL Marketing Channels] Adobe Advertising 보고용](https://experienceleague.adobe.com/docs/advertising-learn/tutorials/analytics/analytics-reporting-a4adc.html)
>* [개요 [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md)
