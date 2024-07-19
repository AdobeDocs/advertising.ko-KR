---
title: 채널 데이터가 Adobe Advertising과  [!DNL Marketing Channels] 간에 다를 수 있는 이유
description: AMO ID로 추적되는 채널 데이터가  [!DNL Analytics Marketing Channels]에서 추적되는 채널 데이터와 다를 수 있는 이유를 알아봅니다.
feature: Integration with Adobe Analytics
exl-id: 72e3aa1e-85ed-485a-b93f-5e67dd0140ce
source-git-commit: 7f35b3f3b33ed320ac186d219cbd0f826666bb3b
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# 채널 데이터가 Adobe Advertising과 [!DNL Marketing Channels] 간에 다를 수 있는 이유

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

Adobe Advertising과 [!DNL Marketing Channels] 데이터 세트의 통합에 대해 학습하는 사용자들의 일반적인 질문은 &quot;AMO ID와 [!DNL Marketing Channels] 간의 데이터 차이를 유발하는 것은 무엇입니까?&quot;입니다. 또는 &quot;데이터가 왜 손상되었습니까? 보고서에서 모든 지표를 일치시켜야 합니다.&quot; 다행히도 불일치는 데이터가 &quot;깨짐&quot;임을 나타내지 않으며 불일치가 예상되고 심지어 원할 수도 있습니다. 통합이 이렇게 설계된 이유를 살펴보겠습니다.

두 데이터 세트의 기본 사용 사례는 서로 다릅니다.

* [!DNL Marketing Channels]: [!DNL Marketing Channels]의 기본 사용 사례는 여러 채널 간의 데이터를 일반적인 속성 모델과 비교하는 것입니다. 분석가는 [!UICONTROL Marketing Channel] 차원을 사용하여 채널이 서로 상호 작용하는 방식에 대한 통찰력을 높일 수 있습니다. 이 통찰력은 각 채널에 투자하는 방법에 대한 거시적 수준의 결정을 유도하는 데 도움이 되며 각 채널의 방문자가 웹 사이트와 상호 작용하는 방법에 대한 통찰력을 유발할 수 있습니다.

  따라서 [!DNL Analytics] [!UICONTROL Marketing Channel] 차원은 모든 채널을 캡처하고 추적하도록 구성됩니다. [!DNL Marketing Channels]은(는) Advertising DSP 뷰스루 및 클릭스루를 캡처하도록 구성할 수도 있으며, 다른 마케팅 채널과 관련해서도 캡처합니다.

* Adobe Advertising AMO ID: Adobe Advertising AMO ID 데이터의 기본 사용 사례는 고급 [!DNL Adobe Sensei] 기반 입찰 알고리즘을 제공하는 것입니다. 알고리즘은 광고 지출을 극대화하고 [!DNL DSP] 캠페인 또는 [!DNL Search, Social, & Commerce] 포트폴리오의 목표를 달성하기 위해 매일 수행되는 수천 개의 마이크로 수준의 입찰 결정을 자동으로 수행합니다. 알고리즘이 캠페인을 연결할 수 있는 전환 데이터가 많을수록 알고리즘이 이러한 입찰 결정을 더 잘 내릴 수 있습니다.

  이 데이터를 수집하기 위해 [!DNL Analytics for Advertising] 통합은 사용자 지정 변수(eVar) 또는 예약된 변수(rVar)로 저장된 Adobe Analytics의 AMO ID 차원에서 클릭스루 및 뷰스루 추적 코드로 변환할 수 있는 원시 AMO ID를 전달합니다. 다른 채널의 클릭스루는 AMO ID 차원에 설정되지 않으므로 AMO ID 차원은 이러한 다른 채널의 항목을 추적할 수 없습니다. 따라서 AMO ID는 [!DNL Marketing Channels] 진입점을 통해 유지됩니다.

Adobe Advertising이 추적된 데이터와 [!DNL Analytics]이(가) 추적된 데이터 간의 가능한 데이터 차이에 대한 자세한 내용은 &quot;[과(와) Adobe Advertising  [!DNL Analytics] 의 예상 데이터 분산](../data-variances.md)&quot;을(를) 참조하십시오.

>[!MORELIKETHIS]
>
>* [과(와) Adobe Advertising  [!DNL Analytics]  사이의 예상 데이터 분산](/help/integrations/analytics/data-variances.md)
>* [기본  [!DNL Analytics Marketing Channels]](mc-overview.md)
>* [Adobe Advertising ID를 사용하여 만들기 [!DNL Marketing Channels] 처리 규칙](mc-ids.md)
>* [Adobe Advertising 데이터로  [!DNL Analytics Marketing Channels] 사용](mc-ac-data.md)
>* [비디오: Adobe Advertising 보고에  [!DNL Marketing Channels] 사용](https://experienceleague.adobe.com/docs/advertising-learn/tutorials/analytics/analytics-reporting-a4adc.html)
