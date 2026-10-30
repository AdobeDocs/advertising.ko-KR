---
title: 경험의 최종 노드에 크리에이티브 번들 지정 및 지정 취소
description: 광고 경험의 각 타겟에 크리에이티브를 할당하는 방법을 알아봅니다.
feature: Creative Experiences
exl-id: 5449a760-6ade-41c0-9cab-bd92026b150b
TQID: 'https://experienceleague.adobe.com/HqTq2fiJadk-QIBwYkOxC2N9sTMm29LIXRzSubPuv9M'
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: d0d9f2ed-c163-44e1-97a1-4ace121416b8
    internal-label: Creative
subfeature_v2:
  - id: f1a0ef49-c5d6-4fdf-b0dc-ae6685afe30b
    internal-label: Creative experiences
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
    internal-label: Optimization
source-git-commit: 8a75f4a164b25ed8e73816c3d853d9650f470118
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%
---
# 경험의 최종 노드에 크리에이티브 번들 지정 및 지정 취소

*의사 결정 트리가 타겟팅된 경험*

경험 의사 결정 트리의 맨 아래 레벨에 있는 대상 노드에 크리에이티브 번들을 할당할 수 있습니다. 타겟을 구성하지 않은 경험의 경우 가장 아래 레벨이 &quot;모두&quot; 아래에 있습니다.

표준 광고 경험의 경우 표준 크리에이티브 번들만 할당할 수 있습니다. 동적 광고 경험의 경우 동적 크리에이티브 번들만 할당할 수 있습니다.

>[!NOTE]
>
>각 최종 노드에 하나 이상의 Creative 번들을 할당하지 않는 경우 [경험을 저장](experience-create-targeting.md)할 때 할당되지 않은 각 노드에 대해 기본 Creative를 사용하도록 선택할 수 있습니다. 경험을 게시하려면 번들을 할당하거나 각 최종 노드에 대한 기본 크리에이티브를 사용해야 합니다.

## AI 기반 편집기 사용(Beta) {#ai-editor}

경험을 [생성](experience-create-targeting.md#ai-editor) 또는 [편집](experience-edit-targeting.md#ai-editor)하는 동안 캔버스 컨트롤을 사용하십시오.

1. 다음 중 하나를 수행합니다.

   * 번들이 없는 최종 노드의 경우 **[!UICONTROL Assign Bundles]**&#x200B;을(를) 클릭합니다.

   * 기존 번들이 있는 노드의 경우 Creative Leaf 노드에서 **[!UICONTROL ...]** > **[!UICONTROL Edit Bundles]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Assign Bundles]** 탭에서 할당할 각 번들 옆의 확인란을 선택하고 할당을 취소할 각 번들 옆의 확인란을 선택 취소합니다.

   경험에 대한 관련 유형의 번들(표준 또는 동적)만 나열됩니다.

1. (선택 사항) **[!UICONTROL Creative optimisation]** 탭을 열어 [순환 및 예약을 사용자 지정](experience-optimization-scheduling-targeting.md)합니다.

1. 대화 상자에서 **[!UICONTROL Save]**&#x200B;을(를) 클릭하여 작업 트리를 업데이트합니다.

1. (선택 사항) [추적 URL을 사용자 지정](experience-tracking-urls-targeting.md#ai-editor)합니다.

1. 변경 내용을 유지하려면 트리 헤더에서 [환경을 저장](#save)하세요.

## 수동 편집기 사용 {#manual-editor}

[수동 편집기를 엽니다](experience-edit-targeting.md#experience-open).

1. 다음 중 하나를 수행합니다.

   * (크리에이티브가 없는 최종 노드) 노드 아래에서 **[!UICONTROL Assign Bundles]**&#x200B;을(를) 클릭합니다.

   * (기존 크리에이티브가 있는 노드) 대상 노드 아래의 크리에이티브 번들 상자 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Edit Bundles]**&#x200B;을(를) 클릭합니다.

1. 각 번들 옆의 확인란을 선택하여 대상 노드에 할당하고, 할당을 취소할 각 번들 옆의 확인란을 선택 취소합니다.

   경험에 대한 관련 번들 유형의 번들(표준 또는 동적)만 나열됩니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 할당된 번들에 대해 [크리에이티브 최적화 및 일정을 사용자 지정](experience-optimization-scheduling-targeting.md)합니다.

1. (선택 사항) [할당된 번들의 광고 추적 URL을 사용자 지정](experience-tracking-urls-targeting.md)합니다.

## 경험 저장 {#save}

다음 단계는 두 편집기에 모두 적용됩니다. 번들 대화 상자만 저장해도 경험이 저장되거나 게시되지 않습니다.

{{$include /help/_includes/experience-save.md}}

>[!MORELIKETHIS]
>
>* [최종 수준에 대상 노드 추가](experience-target-node-add-final.md)
>* [노드 사이에 대상 노드 삽입](experience-target-node-add-inner.md)
>* [노드 사이에 형제 대상 노드 추가](experience-target-node-add-sibling.md)
>* [하위 노드 및 크리에이티브를 같은 수준의 다른 노드에 복사](experience-target-node-copy.md)
>* [의사 결정 트리 타깃팅으로 경험 만들기](experience-create-targeting.md)
>* [의사 결정 트리 타깃팅으로 경험 편집](experience-edit-targeting.md)
>* [타깃팅된 경험 설정](experience-settings-targeting.md)
>* [라이브 경험에 대한 광고 경험 태그 내보내기 및 구현](experience-tag-export.md)
>* [경험에 대한 변경 로그 보기](/help/creative/experiences/experience-view-change-log.md)
