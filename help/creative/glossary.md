---
title: 용어집
description: 주요 용어의 정의를 참조하십시오.
feature: Creative Introduction
source-git-commit: fd925c641bef7953aea50813725252c3913757fa
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# 용어집 {#glossary}

*베타가 닫힘*

<!-- more feature metadata?? -->

<!-- ## A-B {#a-b} -->

<!-- not sure I need these "x-through" terms since that we're not creating conversion pixels in this UI, but see if they come up in other text -->

**클릭스루:** 전환을 가져오는 광고 클릭입니다.

**데이터 전달 대상:** 데이터 전달 대상을 사용하면 DSP, 게시자 또는 파트너가 실시간으로 제공하는 데이터를 기반으로 광고 요소를 선택할 수 있습니다. 여기에는 서드파티 데이터가 포함될 수 있습니다.

<!-- verify this -->광고 경험에서 각 데이터 전달 대상은 최대 5개의 키-값 쌍을 포함할 수 있습니다. 해당 수준의 첫 번째 대상 노드에 키와 하나 이상의 값을 지정하고, 동일 수준의 대상 노드에 대해 동일한 키를 사용할 수 있습니다. 각 키-값 쌍은 이 경험의 광고 태그에 매크로로 추가됩니다. 광고 노출 시 DSP, 게시자 또는 파트너는 해당 노출과 관련된 데이터로 값을 바꿀 책임이 있습니다. 정보가 [!DNL Creative]에 다시 전달되므로 경험에 정의된 규칙에 따라 적절한 광고 경험을 표시할 수 있습니다.

예를 들어, 여성이고 세그먼트 1234에 있는 뷰어에 대해 가능한 한 개 이상의 크리에이티브를 타겟팅하려면 대상 노드에 대한 데이터 전달 대상 `gender=female` 및 `segment=1234`을(를) 구성해야 합니다. 노출을 제공하는 DSP은 성별 및 세그먼트 정보로 태그를 채우고 지정된 요구 사항을 충족하는 방문자는 연관된 크리에이티브 중 하나가 표시됩니다.

**참여-통과:** 전환을 가져오는 광고 참여(예: 비디오 보기 또는 광고 확장)입니다.

<!-- or flexible html5 creative variation? -->
**유연한 HTML5 창의성의 변형:** [!UICONTROL Creative Libraries]에서 창의성을 경험에 할당하고 경험 내의 기본 특성을 변경할 때 생성되는 유연한 HTML5 창의성 자산의 파생입니다.

<!-- Not sure if this will be implemented, and how:
You can view all derived creatives, including not only the base creatives you've added but also each child creative derivation, in the card view in [!UICONTROL Creative] > [!UICONTROL Libraries]. In the toolbar, click __?__ , and then select Derived Creatives. [Clarify how to tell which have variations. I can't find any now.]
-->

**뷰스루:** 사용자가 광고를 클릭하지 않아도 전환되는 광고 노출 또는 노출 문자열입니다.
