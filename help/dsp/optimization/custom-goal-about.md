---
title: 사용자 정의 목표 정보
description: 가장 낮은 CPA 또는 가장 높은 ROAS에 최적화된 패키지에서 성공 이벤트를 정의하는 사용자 정의 목표에 대해 알아봅니다.
feature: DSP Optimization
exl-id: 806450b9-ce32-4f5c-a2ac-ba8e435ce36d
source-git-commit: eda0459472c1e4a8297daf69454de0fcb3d4f8ca
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# 사용자 정의 목표 정보

사용자 지정 목표는 광고주가 비즈니스 목표를 달성하는 데 필요한 성공 이벤트를 정의합니다. &quot;(으)로 끝나는 최적화 목표를 사용하는 각 패키지[!UICONTROL - Custom Goal]&quot; (예: &quot;[!UICONTROL Highest ROAS - Custom Goal]&quot;)에는 전체 최적화 목표를 달성하는 데 도움이 되는 사용자 지정 목표가 포함되어야 합니다. 다음과 같이 사용자 정의 목표를 생성할 수 있습니다. *목표* 위치: [!DNL Advertising Search, Social, & Commerce].

![사용자 정의 목표](/help/dsp/assets/objective-goals.png)

각 사용자 지정 목표는 하나 이상의 전환 지표와 이러한 지표의 상대 가중치로 구성됩니다. 사용 가능한 전환 지표에는 Adobe Advertising 전환 픽셀을 사용하여 Adobe Analytics을 통해 추적된 모든 지표가 포함됩니다.

>[!NOTE]
>
>* [!DNL Analytics] Adobe Advertising 최적화에 차원 및 세그먼트를 사용할 수 없습니다.
>* DSP에서 Analytics 이벤트를 사용하려면 Adobe 계정 팀과 협력하여 광고주 수준 통합을 구성하십시오.
>* [!DNL Analytics] 사용자 지정 이벤트는 다음 명명 규칙을 따릅니다. `custom_event_[*event #*]_[*Analytics report suite ID*]`. 예: `custom_event_16_examplersid`

예를 들어 세 개의 전환 지표가 캠페인 중 하나의 특정 패키지와 관련이 있다고 가정해 보겠습니다. &quot;PDF 다운로드&quot;(20 USD), &quot;이메일 등록&quot;(30 USD) 및 &quot;주문 확인&quot;(40 USD)입니다. 고객 행동의 일회성 금전적 가치에 따라 가중치를 부여하고자 하는 경우 해당 속성의 상대적 가중치는 1, 2, 1.5가 된다.

다음을 참조하십시오. [사용자 정의 목표 생성을 위한 우수 사례](custom-goal-best-practices.md) 사용자 지정 목표를 구성하는 방법에 대한 팁입니다.

한 번 [사용자 지정 목표 만들기](custom-goal-create.md), 다음을 수행할 수 있습니다. [패키지에 할당](/help/dsp/campaign-management/packages/package-settings.md) Adobe Sensei을 사용하여 보고 및 알고리즘 최적화를 위한 .

>[!MORELIKETHIS]
>
>* [사용자 지정 목표 만들기](custom-goal-create.md)
>* [사용자 지정 목표 빌드를 위한 우수 사례](custom-goal-best-practices.md)
>* [최적화 목표 및 사용 방법](optimization-goals.md)
>* [패키지 설정](/help/dsp/campaign-management/packages/package-settings.md)
> * [DSP이 캠페인을 최적화하는 방법](optimization-how-dsp-optimizes-campaigns.md)
