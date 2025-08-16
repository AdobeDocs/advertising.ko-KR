---
title: 경험의 최종 노드에 크리에이티브 번들 지정 및 지정 취소
description: 광고 경험의 각 타겟에 크리에이티브를 할당하는 방법을 알아봅니다.
feature: Creative Experiences
exl-id: 5449a760-6ade-41c0-9cab-bd92026b150b
source-git-commit: f7d5bf3193cb41ca2a0d4415998209e5a9b724ba
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---

# 경험의 최종 노드에 크리에이티브 번들 지정 및 지정 취소

*의사 결정 트리가 타겟팅된 경험*

경험 의사 결정 트리의 맨 아래 레벨에 있는 대상 노드에 크리에이티브 번들을 할당할 수 있습니다. 타겟을 구성하지 않은 경험의 경우 가장 아래 레벨이 &quot;모두&quot; 아래에 있습니다.

표준 광고 경험의 경우 표준 크리에이티브 번들만 할당할 수 있습니다. 동적 광고 경험의 경우 동적 크리에이티브 번들만 할당할 수 있습니다.

>[!NOTE]
>
>각 최종 노드에 하나 이상의 Creative 번들을 할당하지 않는 경우 [경험을 저장](experience-create-targeting.md)할 때 할당되지 않은 각 노드에 대해 기본 Creative를 사용하도록 선택할 수 있습니다. 경험을 게시하려면 번들을 할당하거나 각 최종 노드에 대한 기본 크리에이티브를 사용해야 합니다.

<!-- 1. [ways to get to the decision tree] -->

1. 다음 중 하나를 수행합니다.

   * (최종 노드(광고 크리에이티브 없음) 노드 아래에서 ![추가](/help/creative/assets/add.png "추가")를 클릭한 다음 **[!UICONTROL Assign Bundles]**&#x200B;을(를) 선택합니다.

   * (기존 크리에이티브가 있는 노드) 대상 노드 <!-- wording???? --> 아래의 크리에이티브 번들 상자 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Edit Bundles]**&#x200B;을(를) 클릭합니다.

1. 각 번들 옆의 확인란을 선택하여 대상 노드에 할당하고, 할당을 취소할 각 번들 옆의 확인란을 선택 취소합니다.

   경험에 대한 관련 번들 유형의 번들(표준 또는 동적)만 나열됩니다.

1. **[!UICONTROL Attach to Bundles]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) [할당된 번들의 광고 추적 URL을 사용자 지정](experience-tracking-urls-targeting.md)합니다.

1. (선택 사항) 할당된 번들에 대해 [크리에이티브 최적화 및 일정을 사용자 지정](experience-optimization-scheduling-targeting.md)합니다.

<!--
1. (Optional) To save the experience, click **[!UICONTROL Save]**, and then do the following.
...

These formatted steps are inserted automatically from text in the following file in the _includes folder, which reused in multiple places.
-->

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
