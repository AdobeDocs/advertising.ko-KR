---
title: 용어집
description: 주요 용어의 정의를 참조하십시오.
feature: Creative Introduction
source-git-commit: 4e61ce32862411a7a83c66773e41d032770ad861
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# 용어집 {#glossary}

*베타가 닫힘*

<!-- more feature metadata?? -->

<!-- ## A-B {#a-b} -->

<!-- not sure I need these "x-through" terms since that we're not creating conversion pixels in this UI, but see if they come up in other text -->

**클릭스루:** 전환을 가져오는 광고 클릭입니다.

**데이터 전달 대상:** 데이터 전달 대상을 사용하면 DSP, 게시자 또는 파트너가 실시간으로 제공하는 데이터를 기반으로 광고 요소를 선택할 수 있습니다. 여기에는 서드파티 데이터가 포함될 수 있습니다.

<!-- verify this -->광고 경험에서 각 데이터 전달 대상은 최대 5개의 키-값 쌍을 포함할 수 있습니다. 해당 수준의 첫 번째 대상 노드에 키와 하나 이상의 값을 지정하고, 동일 수준의 대상 노드에 대해 동일한 키를 사용할 수 있습니다. 각 키-값 쌍은 이 경험의 광고 태그에 매크로로 추가됩니다. 광고 노출 시 DSP, 게시자 또는 파트너는 값을 해당 노출과 관련된 데이터로 바꿀 책임이 있습니다. 정보가 [!DNL Creative]에 다시 전달되므로 경험에 정의된 규칙에 따라 적절한 광고 경험을 표시할 수 있습니다.

예를 들어, 여성이고 세그먼트 1234에 있는 뷰어에 대해 가능한 한 개 이상의 크리에이티브를 타겟팅하려면 대상 노드에 대한 데이터 전달 대상 `gender=female` 및 `segment=1234`을(를) 구성해야 합니다. 노출을 제공하는 DSP은 태그를 성별 및 세그먼트 정보로 채우고 지정된 요구 사항을 충족하는 방문자는 연결된 크리에이티브 중 하나를 보게 됩니다.

**광고 참여:** 전환을 가져오는 광고 참여(예: 회전식 광고 스크롤 또는 광고 확장)입니다. 이 유형의 이벤트는 랜딩 페이지 또는 랜딩 페이지의 이벤트에 도달하기 위해 광고를 클릭하는 것과 별개입니다.

<!-- or flexible html5 creative variation? Not sure we need to mention this since there's no place to view the different variations per se:

**variation of a flexible HTML5 creative:** A derivation of a flexible HTML5 creative asset in your [!UICONTROL Creative Libraries], which is generated when you assign the creative to an experience and change any of the default attributes within the experience.
-->

**뷰스루:** 사용자가 광고를 클릭하지 않아도 전환되는 광고 노출 또는 노출 문자열입니다.
