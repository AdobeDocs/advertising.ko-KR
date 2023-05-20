---
title: 사용 [!DNL Marketing Channels] Adobe 광고 데이터 포함
description: 에서 Adobe 광고 데이터를 사용하는 방법 알아보기 [!DNL Analytics Marketing Channels].
feature: Integration with Adobe Analytics
exl-id: 522c7f01-1138-477d-8018-36030caab55e
source-git-commit: 7e614ecb517515217d812926f61ca10437820efd
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---

# 사용 [!DNL Analytics Marketing Channels] Adobe 광고 데이터 포함

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

Adobe 광고 및 를 모두 사용 [!DNL Analytics Marketing Channels] 보고서에서는 디지털 미디어가 사이트 활동에 미치는 영향에 대한 중요한 통찰력을 얻을 수 있습니다.

<!-- from video: By using Marketing Channels with your Adobe Advertising data, you can get a more holistic view of how your advertising efforts are affecting site behavior. In particular, you can see the value of your view-through and click-through data, and how your advertising assists or is assisted by other channels. -->

다음 그림은 Adobe 광고 및 [!DNL Marketing Channels] 한 방문자의 여정을 구성하는 개별 방문을 추적합니다. 에서 광고 보고서 Adobe [!DNL Analytics] AMO ID를 사용하여 Adobe 광고를 통해 거래되는 유료 디스플레이, 검색, 소셜 및 상거래 채널 광고로만 제한됩니다. 그러나 [!DNL Marketing Channels] 에서 구성한 모든 채널을 추적합니다. [!DNL Marketing Channels] 처리 규칙.

![광고 및 Adobe 방법 [!DNL Marketing Channels] 방문자의 여정에서 개별 방문 추적](/help/integrations/assets/a4adc-mc-sample-journey2.png)

첫 번째 방문에서 사용자는 이메일 캠페인을 통해 웹 사이트에 들어가 10번의 페이지 보기를 실행한 후 떠났다. 두 번째 방문에서 사용자는 디스플레이 광고를 통해 사이트에 들어갔고, 10개의 페이지 보기를 실행한 다음 떠났습니다. 세 번째 방문에서 사용자는 자연어 검색을 통해 사이트에 들어갔고, 5개의 페이지 보기를 실행했으며, $250 전환을 실행했습니다. 간의 추적 차이점에 주목합니다. [!DNL Marketing Channels] 및 Adobe 광고. 이 여정에서 Adobe 광고가 추적하는 유일한 채널은 [!UICONTROL Display]. Adobe 광고가 다음을 추적합니다. [!UICONTROL Display] 채널 방문 및 속성은 후속 참여 데이터(예: 페이지 보기 수) 및 해당 광고의 영향으로의 전환을 다시 지정합니다. [!DNL Marketing Channels]반면 은 모든 채널을 전체 볼 수 있도록 합니다.

AMO ID는 방문자의 여정을 통해 유지되므로 AMO ID 데이터를 사용하여 Adobe 광고가 다른 마케팅 채널에 미치는 영향을 확인할 수 있습니다. AMO ID [기본적으로 60일 동안 지속](/help/integrations/analytics/overview.md), 하지만 필요에 따라 지속성을 구성할 수 있습니다.

## 미디어 성과를 분석하기 위해 Adobe 광고 및 마케팅 채널 데이터를 결합하는 방법

다음 범위 내 [!DNL Analytics], 유료 광고 데이터를 지속하는 Adobe 광고와 을 결합할 수 있습니다. [!DNL Marketing Channels] 포괄적인 방문 데이터를 통해 미디어 성능을 보다 잘 분석하여 고객 여정에 보다 효과적으로 영향을 미칠 수 있습니다.

다음 분석에서는 Adobe 광고 데이터를 사용하여 디스플레이 광고가 사이트 전환에 미치는 영향을 다양한 버전으로 보여줍니다. 세 열 모두 동일한 전환 지표를 사용하지만 각 열은 다른 스토리를 전달합니다.

* 열 1은 방문자의 여정 전체에서 영구적인 AMO ID 데이터를 봅니다. 열 1은 한 시점에서 641개의 애플리케이션 시작이 뷰스루 또는 클릭스루 이벤트를 통해 Adobe 광고 광고에 연결되어 있었음을 나타냅니다. 이 보기는 다른 보기가 필요하지 않습니다. [!DNL Marketing Channels] 기여도 분석을 고려합니다.

* 다음에서 [!DNL Marketing Channels] 그러나 641 Applications Starts의 데이터 세트는 다른 마케팅 채널에 연결됩니다. 마지막 두 열에는 641 응용 프로그램 시작이 포함되며 데이터가 [!UICONTROL Display Click-Through] 및 [!UICONTROL Display View-Through] 채널, 마지막 터치 속성 모델에서 발생하는 전환을 보여 줍니다.

![디스플레이 광고가 사이트 전환에 미치는 영향의 예](/help/integrations/assets/a4adc-mc-display-impact.png)

이 분석을 한 단계 더 발전시킬 수 있습니다. 마케팅 채널별로 Adobe 광고 행을 더 세분하여 Adobe 광고 전환이 641 애플리케이션 시작에 기여하는 위치를 확인할 수 있습니다. 이러한 전환 중 5개가 마지막 터치 디스플레이 클릭스루에 속하고 19개가 마지막 터치 디스플레이 뷰스루에 속한다는 것은 이미 알고 있습니다. 따라서 617 Applications Starts가 다른 마케팅 채널에 귀속됩니다. Advertising DSP 라인 항목 위에 마지막 터치 채널 차원을 드래그 앤 드롭하여 나머지 애플리케이션 시작에 대한 채널 속성을 표시하고 디스플레이 채널의 크로스 채널 영향을 표시할 수 있습니다.

![마지막 터치 채널 차원을 추가하는 방법](/help/integrations/assets/a4adc-mc-display-impact-ltc.png)

이제 나머지 응용 프로그램 시작의 속성 방식을 확인할 수 있습니다. 이메일에는 AMO ID가 지속되는 357개의 마지막 터치 애플리케이션 시작에 대한 크레딧이 제공됩니다. 이러한 유형의 분석을 사용하면 Adobe 광고 표시 광고가 모든 채널에 미치는 영향을 확인할 수 있습니다. 데이터 세트 및 속성 모델이 하나뿐인 경우에는 이 유형의 통찰력을 사용할 수 없습니다.

![디스플레이 채널의 크로스 채널 영향 예](/help/integrations/assets/a4adc-mc-display-impact-x-channel.png)

스택 그래프를 &quot;100% 스택&quot;으로 설정하여 시간에 따른 트렌드 데이터를 표시함으로써 분석을 더욱 향상시킬 수 있습니다. 이 시각화를 사용하면 디스플레이 마케팅 캠페인의 영향을 더 많이 받는 마지막 터치 마케팅 채널을 더욱 쉽게 모니터링할 수 있습니다.

![디스플레이 채널의 트렌드 크로스 채널 영향의 예](/help/integrations/assets/a4adc-mc-display-impact-x-channel-trend.png)

>[!MORELIKETHIS]
>
>* [의 기본 사항 [!DNL Analytics Marketing Channels]](mc-overview.md)
>* [Adobe 광고 ID를 사용하여 만들기 [!DNL Marketing Channels] 처리 규칙](mc-ids.md)
>* [Adobe 광고와 간에 채널 데이터가 다를 수 있는 이유 [!DNL Marketing Channels]](mc-data-variances.md)
>* [비디오: 사용 [!DNL Marketing Channels] Adobe 광고 보고용](https://experienceleague.adobe.com/docs/advertising-learn/tutorials/analytics/analytics-reporting-a4adc.html)
>* [개요 [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md)

