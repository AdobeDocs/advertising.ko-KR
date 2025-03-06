---
title: 의사 결정 트리 타겟팅으로 경험 편집
description: 의사 결정 트리를 사용하여 타깃팅된 광고 경험에 대한 설정을 편집하는 방법을 알아봅니다.
feature: Creative Experiences
exl-id: 8c5e8f9b-c405-41b2-98a9-da7c5debd3e1
source-git-commit: 115b769c2880936c422747b44f43b4be7281916d
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# 의사 결정 트리 타겟팅으로 경험 편집

*베타가 닫힘*

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Experiences]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 특정 경험을 포함하도록 [보기를 사용자 지정](/help/creative/introduction/customize-data-views.md)합니다.

1. 다음 중 하나를 수행합니다.

   * 카드 보기에서 경험 이름 옆의 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

   * 테이블 보기에서 행 위에 커서를 놓고 **[!UICONTROL More]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. [일반 환경 설정](experience-settings-targeting.md)을(를) 편집합니다.

1. (선택 사항) 결정 트리를 편집하려면 오른쪽 상단의 **[!UICONTROL Decision Tree]**&#x200B;을(를) 클릭하고 다음 중 하나를 수행합니다.

   * ([처리](experience-about.md#experience-statuses) 경험) 다음 중 하나를 수행합니다.

      * Live Experience에 게시되지 않은 기존 변경 내용을 취소하려면 **[!UICONTROL Discard and start again]**&#x200B;을(를) 클릭합니다.

      * 게시되지 않은 기존 변경 내용을 유지하려면 **[!UICONTROL Continue editing draft]**&#x200B;을(를) 클릭합니다.

      * 경험 세부 정보를 편집하려면 **[!UICONTROL Edit Experience Details]**&#x200B;을(를) 클릭하십시오.

   * (선택 사항) 의사 결정 트리에 대한 보기 설정을 변경합니다.

     로그아웃할 때까지 설정이 저장됩니다.

   * 슬라이더를 이동하여 확대 또는 축소합니다.

   * ![세로 트리로 보기](/help/creative/assets/tree-vertical.png "세로 트리로 보기") 또는 ![가로 트리로 보기](/help/creative/assets/tree-horizontal.png "가로 트리로 보기")을(를) 클릭하여 세로 목록과 가로 목록 보기 간을 각각 전환합니다.

   * (선택 사항) 다음 방법 중 하나로 광고 타겟 및 해당 크리에이티브를 변경합니다.

      * 대상:

        *[경험의 최종 수준에 대상 노드를 추가](experience-target-node-add-final.md)합니다.

         * [노드 사이에 대상 노드를 삽입합니다](experience-target-node-add-inner.md).

         * [노드 사이에 형제 대상 노드를 추가](experience-target-node-add-sibling.md)합니다.

         * [하위 노드 및 크리에이티브를 같은 수준의 다른 노드에 복사](experience-target-node-copy.md).

      * Creative 번들:

         * [최종 노드에 대한 크리에이티브 할당 및 할당 해제](experience-assign-creative-bundles.md).

           각 최종 노드에 하나 이상의 번들을 할당하지 않는 경우 경험을 저장할 때 할당되지 않은 각 노드에 대한 기본 크리에이티브를 사용하도록 선택할 수 있습니다. 경험을 게시하려면 번들을 할당하거나 각 최종 노드에 대한 기본 크리에이티브를 사용해야 합니다.

         * [할당된 번들의 광고 추적 URL을 사용자 지정](experience-tracking-urls-targeting.md)합니다.

         * 할당된 번들에 대해 [크리에이티브 최적화 및 예약을 사용자 지정](experience-optimization-scheduling-targeting.md)합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭하고 다음을 수행합니다.

   * (맨 아래 수준의 각 노드에 하나 이상의 Creative 번들이 포함된 경우) **[!UICONTROL OK]**&#x200B;을(를) 클릭합니다.

   * (맨 아래 수준의 각 노드에 크리에이티브 번들이 하나 이상 포함되지 않은 경우) 다음 중 하나를 수행하십시오.

      * 필요한 모든 Creative 번들 없이 경험을 저장하려면 **[!UICONTROL Save as Draft]**&#x200B;을(를) 클릭합니다.

        [초안](experience-about.md#experience-statuses) 경험에 대한 광고 태그를 만들 수 없습니다.

      * 아직 Creative 번들이 할당되지 않은 각 대상에 기본 Creative를 할당하려면 **[!UICONTROL Assign Default Creatives]**&#x200B;을(를) 클릭합니다. 기본 크리에이티브가 할당된 업데이트된 트리를 검토한 후 **[!UICONTROL Save]** 및 **[!UICONTROL OK]**&#x200B;을(를) 클릭합니다.

      * 결정 트리 편집을 계속하려면 **[!UICONTROL Continue Edit]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [타깃팅된 경험 설정](experience-settings-targeting.md)
>* [최종 수준에 대상 노드 추가](experience-target-node-add-final.md)
>* [노드 사이에 대상 노드 삽입](experience-target-node-add-inner.md)
>* [노드 사이에 형제 대상 노드 추가](experience-target-node-add-sibling.md)
>* [하위 노드 및 크리에이티브를 같은 수준의 다른 노드에 복사](experience-target-node-copy.md)
>* [최종 노드에 광고 할당](experience-assign-creative-bundles.md)
>* [할당된 번들에서 크리에이티브에 대한 추적 URL을 사용자 지정](experience-tracking-urls-targeting.md)
>* [크리에이티브 최적화 및 일정 사용자 지정](experience-optimization-scheduling-targeting.md)
>* [라이브 경험에 대한 광고 경험 태그 내보내기 및 구현](/help/creative/experiences/experience-tag-export.md)
>* [의사 결정 트리 타깃팅으로 경험 만들기](experience-create-targeting.md)
