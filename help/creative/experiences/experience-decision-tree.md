---
title: 의사 결정 트리 레이아웃
description: 타깃팅이 있는 경험의 의사 결정 트리 레이아웃에 대해 알아봅니다.
feature: Creative Experiences
exl-id: 1d997422-8177-4a6b-b56a-e1c742b96ad2
source-git-commit: 7bcafc7c70333bb6f523873ed08f2bc5123823f7
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# [!DNL Creative] 경험에 대한 의사 결정 트리 레이아웃

경험에 대해 &quot;[!UICONTROL Targeting]&quot; 옵션을 활성화하면 의사 결정 트리를 사용하여 경험을 설정합니다.

처음에는 각 결정 트리가 루트 수준인 &quot;모두&quot;로 시작합니다. 하나 이상의 대상 노드를 추가한 다음 의사 결정 트리의 각 분기에 있는 최종 노드에 크리에이티브 번들을 할당할 수 있습니다. 기본적으로 결정 트리는 세로로 표시되지만, 대신 선택적으로 가로로 트리를 볼 수 있습니다.

![대상이 없는 수직 결정 트리의 예](/help/creative/assets/experience-decision-tree-no-targets.png "대상이 없는 수직 결정 트리의 예")

![대상이 없는 가로 결정 트리의 예](/help/creative/assets/experience-decision-tree-no-targets-horizontal.png "대상이 없는 가로 결정 트리의 예")

<!--
>[!NOTE]
>
>You can optionally assign creative bundles to the root level, without targets. However, the [XXXX workflow](experience-create-no-targeting.md) XXXXX is better XXX.<!-- Explain the diff and why to choose the other option. -->
-->

## 용어

**트리:** 가지가 있는 트리로서 전체 의사 결정 구조입니다.

**대상 노드:** 분기 내의 대상입니다.

**리프 노드:** 최종 대상 노드에 할당된 크리에이티브 집합입니다.

## 의사 결정 트리의 타겟

각 의사 결정 트리는 최대 5개 수준의 대상을 가질 수 있습니다. 각 타겟 수준에는 동일한 타겟 유형(대상 세그먼트, 지리적 위치 유형, 지정된 데이터 패스 키의 값, 지정된 리타겟팅 픽셀의 속성 또는 디바이스 카테고리)을 가진 하나 이상의 노드가 각각 있는 여러 분기가 포함될 수 있습니다. 기본 이미지 크리에이티브 또는 비디오 크리에이티브를 지정한 각 광고 크기의 크리에이티브 번들을 최하위 레벨 대상 노드에 할당할 수 있습니다.

![대상이 있는 의사 결정 트리의 예](/help/creative/assets/experience-decision-tree.png "대상이 있는 의사 결정 트리의 예")

최종 레벨에 대상 노드를 추가할 때 새 노드에 대한 대상을 지정합니다. 지정된 대상과 일치하지 않는 모든 사용자에 대해 추가 형제 노드인 &quot;Everything Else&quot;가 자동으로 만들어집니다. 그런 다음 동일한 유형의 다른 대상이 있는 동위 노드를 추가할 수 있습니다.

그러나 기존 레벨 사이에 대상 노드를 삽입하면 새 레벨에 대한 첫 번째 노드가 처음에 &quot;모두&quot;에 할당됩니다. 특정 대상을 식별하려면 동일한 레벨에 실제 대상을 지정하는 동일 수준의 동일 수준의 동일 수준의 대상 노드를 생성합니다. 이 작업은 대상 노드를 만들고 &quot;All&quot; 노드를 &quot;Everything Else&quot; 노드(이전에 All에 할당된 모든 크리에이티브 번들을 포함)로 바꿉니다. 그런 다음 동일한 유형의 다른 대상이 있는 동위 노드를 추가할 수 있습니다.

모든 상위 노드에 대해 선택적으로 모든 하위 대상 노드 및 Creative 번들을 복사하여 동일한 레벨의 다른 노드에 붙여넣을 수 있습니다. 붙여넣은 노드를 기존 프레임워크에 추가하거나 기존 프레임워크를 기존 프레임워크로 대체할 수 있습니다.

## 의사 결정 트리의 크리에이티브

경험의 각 최종 대상 노드에 크리에이티브 번들을 할당합니다.

크리에이티브 번들이 있는 각 노드 내에서, 포함된 크리에이티브를 선택적으로 a) 클릭스루 비율 또는 사용자 지정 목표를 최적화하기 위해 알고리즘적으로 회전하거나, b) 지정된 가중치에 따라 또는 c) 특정 순서로 회전할 수 있습니다. 동일한 옵션의 조합을 사용하여 지정된 시간 시퀀스에서 크리에이티브를 선택적으로 회전할 수도 있습니다.

개별 크리에이티브에 대해 필요에 따라 랜딩 페이지 URL, 노출 추적 URL 및 클릭 추적 URL을 선택적으로 사용자 지정할 수 있습니다. <!-- Not in the UI as of 1/31: For flexible HTML5 creatives, you can customize any of the flexible attributes. -->

>[!MORELIKETHIS]
>
>* [Advertising Creative 2.0의 경험 정보](experience-about.md)
>* [타깃팅으로 경험 만들기](/help/creative/experiences/experience-create-targeting.md)
>* [타깃팅된 경험 설정](/help/creative/experiences/experience-settings-targeting.md)
