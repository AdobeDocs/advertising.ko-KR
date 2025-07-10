---
title: 의사 결정 트리 타겟팅으로 경험 만들기
description: 의사 결정 트리를 사용하여 타깃팅된 광고 경험을 만드는 방법을 알아봅니다.
feature: Creative Experiences
exl-id: 825fd9af-ca7a-4b44-8e4b-1a6f34edac9e
source-git-commit: 45b2dad83aa626ea30e7553df7caaf5e7f53b3e1
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 0%

---

# 의사 결정 트리 타겟팅으로 경험 만들기

*베타가 닫힘*

의사 결정 트리를 사용하여 타깃팅된 광고 경험을 만듭니다. 각 경험은 단일 크리에이티브 라이브러리의 광고를 사용합니다.

>[!NOTE]
>
>* 타겟팅된 경험을 만들면 나중에 다른 워크플로우를 사용하는 타겟팅되지 않은 경험으로 변경할 수 없습니다.
>* 광고 경험에 구현할 캠페인과 호환되는 타겟팅이 포함되어 있는지 확인하십시오. 계층 타겟팅 동작은 DSP에 따라 다를 수 있습니다. 광고 경험 태그를 Advertising DSP에 업로드하고 배치에 첨부하면 광고 수준 타깃팅이 배치 수준 타깃팅 (대신 적용되지 않음) 위에 적용됩니다. 예를 들어 배치가 오스트레일리아의 사용자를 타겟팅하고 광고가 일본의 사용자를 타겟팅하는 경우 광고는 &quot;기타 사용자&quot; 분기를 타겟팅합니다.

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Experiences]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Create New Experience]**&#x200B;을(를) 클릭합니다.

1. [일반 환경 설정](experience-settings-targeting.md)을 입력하세요.

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

1. 결정 트리에서 다음을 수행합니다.

   1. (선택 사항) 의사 결정 트리에 대한 보기 설정을 변경합니다.

      로그아웃할 때까지 설정이 저장됩니다.

      * 슬라이더를 이동하여 확대 또는 축소합니다.

      * ![세로 트리로 보기](/help/creative/assets/tree-vertical.png "세로 트리로 보기") 또는 ![가로 트리로 보기](/help/creative/assets/tree-horizontal.png "가로 트리로 보기")을(를) 클릭하여 세로 목록과 가로 목록 보기 간을 각각 전환합니다.

   1. (선택 사항) 다음 방법 중 하나로 광고 타겟 및 해당 광고 타겟을 설정합니다.

      * 대상:

         * [대상 노드를 최종 수준에 추가](experience-target-node-add-final.md).

         * [노드 사이에 대상 노드를 삽입합니다](experience-target-node-add-inner.md).

         * [노드 사이에 형제 대상 노드를 추가](experience-target-node-add-sibling.md)합니다.

         * [하위 노드 및 크리에이티브를 같은 수준의 다른 노드에 복사](experience-target-node-copy.md).

      * Creative 번들:

         * [최종 노드에 대한 크리에이티브 할당 및 할당 해제](experience-assign-creative-bundles.md).

           각 최종 노드에 하나 이상의 번들을 할당하지 않는 경우 경험을 저장할 때 할당되지 않은 각 노드에 대한 기본 크리에이티브를 사용하도록 선택할 수 있습니다. 경험을 게시하려면 번들을 할당하거나 각 최종 노드에 대한 기본 크리에이티브를 사용해야 합니다.

         * [할당된 번들의 광고 추적 URL을 사용자 지정](experience-tracking-urls-targeting.md)합니다.

         * 할당된 번들에 대해 [크리에이티브 최적화 및 예약을 사용자 지정](experience-optimization-scheduling-targeting.md)합니다.

1. (선택 사항) 의사 결정 트리와 일반 설정 간에 전환합니다.

   * 결정 트리에서 일반 설정을 열려면 오른쪽 상단의 **[!UICONTROL Experience Form]**&#x200B;을(를) 클릭합니다.

   * 일반 설정에서 결정 트리를 열려면 오른쪽 상단의 **[!UICONTROL Decision Tree]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭하고 다음을 수행합니다.

   * (맨 아래 수준의 각 노드에 하나 이상의 Creative 번들이 포함된 경우) **[!UICONTROL OK]**&#x200B;을(를) 클릭합니다.

   * (맨 아래 수준의 각 노드에 크리에이티브 번들이 하나 이상 포함되지 않은 경우) 다음 중 하나를 수행하십시오.

      * 필요한 모든 Creative 번들 없이 환경을 저장하려면 **[!UICONTROL Save as Draft]**&#x200B;을(를) 클릭합니다.

        [초안](experience-about.md#experience-statuses) 경험에 대한 광고 태그를 만들 수 없습니다.

      * 아직 Creative 번들이 할당되지 않은 각 대상에 기본 Creative를 할당하려면 **[!UICONTROL Assign Default Creatives]**&#x200B;을(를) 클릭합니다. 기본 크리에이티브가 할당된 업데이트된 트리를 검토한 후 **[!UICONTROL Save]** 및 **[!UICONTROL OK]**&#x200B;을(를) 클릭합니다.

      * 결정 트리 편집을 계속하려면 **[!UICONTROL Continue Edit]**&#x200B;을(를) 클릭합니다.

경험이 라이브되면 [!DNL Creative]에서 적용 가능한 각 광고 크기에 대한 광고 태그를 자동으로 만듭니다. 그런 다음 [광고 태그를 내보내고 DSP에서 구현](/help/creative/experiences/experience-tag-export.md)할 수 있습니다.

비디오 광고 경험의 경우 비디오 크리에이티브가 DSP as VAST 2.0 태그로 자동으로 코드 변환되므로 미리 볼 수 있습니다. 원할 경우 [게시자별 코드 변환](experience-tag-video-transcoding.md)을 모든 비디오 광고 경험 태그에 적용할 수 있습니다.

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
>* [의사 결정 트리 타깃팅으로 경험 편집](experience-edit-targeting.md)
