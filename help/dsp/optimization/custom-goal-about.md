---
title: 사용자 지정 목표
description: 최저 CPA 또는 가장 높은 ROAS에 맞게 최적화된 패키지에서 성공 이벤트를 정의하는 사용자 지정 목표에 대해 알아봅니다.
feature: DSP Optimization
exl-id: 806450b9-ce32-4f5c-a2ac-ba8e435ce36d
source-git-commit: 7e614ecb517515217d812926f61ca10437820efd
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---

# 사용자 지정 목표

사용자 지정 목표는 광고주가 비즈니스 목표를 충족하는 데 필요한 성공 이벤트를 정의합니다. 최적화 목표를 사용하는 각 패키지 &quot;[!UICONTROL Highest ROAS - Custom Goal]&quot; 또는 &quot;[!UICONTROL Lowest CPA - Custom Goal]&quot;에는 전체 최적화 목표를 달성하는 데 도움이 되는 사용자 지정 목표가 포함되어야 합니다. 사용자 지정 목표를 *목표* in [!DNL Adobe Advertising Search].

![사용자 지정 목표](/help/dsp/assets/objective-goals.png)

각 사용자 지정 목표는 하나 이상의 지표로 구성됩니다. 또는 *트랜잭션 속성*&#x200B;및 해당 거래 속성의 상대 가중치입니다. 사용 가능한 트랜잭션 속성에는 Adobe 광고 변환 픽셀을 사용하여 Adobe Analytics을 통해 추적된 모든 지표가 포함됩니다.

>[!NOTE]
>
>* [!DNL Analytics] 차원 및 세그먼트를 Adobe 광고 최적화에 사용할 수 없습니다.
>* DSP에서 Analytics 이벤트를 사용하려면 [!DNL Adobe] 계정 팀이 광고주 수준 통합을 구성합니다.
>* [!DNL Analytics] 사용자 지정 이벤트는 다음 이름 지정 규칙을 따릅니다. `custom_event_[*event #*]_[*Analytics report suite ID*]`. 예: `custom_event_16_examplersid`


예를 들어 다음 세 가지 지표(거래 속성)가 캠페인 중 하나의 특정 패키지와 관련이 있다고 가정합니다. PDF 다운로드(미화 20USD), &quot;이메일 등록&quot;(30USD) 및 &quot;주문 확인&quot;(미화 40USD) 값. 고객 작업의 1회 통화 값에 따라 가중치를 제공하려는 경우 속성의 상대적 가중치는 1, 2 및 1.5가 됩니다.

자세한 내용은 [사용자 지정 목표 생성에 대한 우수 사례](custom-goal-best-practices.md) 를 참조하십시오.

일단 [사용자 지정 목표 만들기](custom-goal-create.md), 다음 작업을 수행할 수 있습니다. [패키지에 할당](/help/dsp/campaign-management/packages/package-settings.md) Adobe Sensei을 사용한 보고 및 알고리즘 최적화의 경우

>[!MORELIKETHIS]
>
>* [사용자 지정 목표 만들기](custom-goal-create.md)
>* [사용자 지정 목표 구축에 대한 우수 사례](custom-goal-best-practices.md)
>* [최적화 목표 및 사용 방법](optimization-goals.md)
>* [패키지 설정](/help/dsp/campaign-management/packages/package-settings.md)
> * [DSP이 캠페인을 최적화하는 방법](optimization-how-dsp-optimizes-campaigns.md)

