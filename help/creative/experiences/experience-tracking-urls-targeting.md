---
title: 경험에 대한 추적 URL 사용자 지정
description: 의사 결정 트리 타깃팅을 사용하는 경험에서 각 크리에이티브에 대한 추적 URL을 사용자 지정하는 방법을 알아봅니다.
feature: Creative Experiences
exl-id: ba3b15b4-116e-4caa-8ce1-4d2e488a6362
TQID: 'https://experienceleague.adobe.com/LjeF7eYU8V93W28VbV-D6NNWWwdKqywOP2BwzDwQAgo'
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
source-wordcount: '448'
ht-degree: 0%
---
# 의사 결정 트리 타겟팅이 있는 경험에서 크리에이티브에 대한 추적 URL 사용자 지정

*기존 크리에이티브만 있는 노드 타깃팅*

의사 결정 트리 타깃팅이 있는 경험의 경우 경험에 사용되는 각 개별 크리에이티브에 대해 최대 5개의 사용자 지정 노출 추적 URL과 5개의 사용자 지정 클릭 추적 URL을 만들 수 있습니다. 랜딩 페이지 재정의를 사용할 수 있는 경우, 사용자 지정 랜딩 페이지 URL을 한 개 지정할 수도 있습니다. 두 의사 결정 트리 편집기 내에서 추적 URL을 사용자 지정할 수 있습니다.

사용자 지정 URL은 경험에서 만든 광고에만 사용되며 [!UICONTROL Creative Libraries]의 기본 크리에이티브 설정에 저장되지 않습니다.

랜딩 페이지 재정의는 표준 경험 및 기본 크리에이티브를 사용하는 노드에 사용할 수 있습니다. 할당된 동적 번들의 경우 랜딩 페이지는 피드에 의해 결정되며 랜딩 페이지 탭은 표시되지 않습니다.

## AI 기반 편집기 사용(Beta) {#ai-editor}

경험을 [생성](experience-create-targeting.md#ai-editor) 또는 [편집](experience-edit-targeting.md#ai-editor)하는 동안 캔버스 컨트롤을 사용하십시오.

1. 대상 노드 아래의 Creative Leaf 노드에서 **[!UICONTROL ...]** > **[!UICONTROL Edit Tracking URLs]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Click Tracking URLs]**, **[!UICONTROL Impression Tracking URLs]** 또는 **[!UICONTROL Landing URL]** 탭을 선택합니다(가능한 경우).

   광고 팀은 번들로 그룹화됩니다. 경험에 대한 기본 크리에이티브 크기는 사용 가능한 크리에이티브 크기를 결정합니다.

1. 편집할 크리에이티브를 확장하고 다음 중 하나를 수행합니다.

   * 사용자 지정 URL을 추가하거나 편집하려면 입력 필드에 URL을 입력합니다.

   * 다른 사용자 지정 추적 URL을 추가하려면 **[!UICONTROL Add URL]**&#x200B;을(를) 클릭하고 입력 필드에 URL을 입력합니다.

   * 사용자 지정 URL을 제거하려면 **[!UICONTROL Delete URL]**&#x200B;을(를) 클릭합니다.

   편집된 필드 외부를 클릭하고 저장하기 전에 유효성 검사 오류를 수정합니다.

1. 대화 상자에서 **[!UICONTROL Save]**&#x200B;을(를) 클릭하여 작업 트리를 업데이트합니다.

1. 트리 헤더에서 [환경을 저장](#save)합니다.

## 수동 편집기 사용 {#manual-editor}

[수동 편집기를 엽니다](experience-edit-targeting.md#experience-open).

1. 대상 노드 아래의 Creative Leaf 노드에서 **[!UICONTROL ...]** > **[!UICONTROL Edit Tracking URLs]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Click Tracking URLs]**, **[!UICONTROL Impression Tracking URLs]** 또는 **[!UICONTROL Landing URLs]** 탭을 선택합니다(가능한 경우).

   탭에는 할당된 번들의 크리에이티브가 나열됩니다. 경험의 기본 크리에이티브 크기가 사용 가능한 크리에이티브 크기를 결정합니다.<!-- There's no distinct "Creative Sizes" setting. -->

1. 편집할 크리에이티브를 확장하고 다음 중 하나를 수행합니다.

   * 사용자 지정 URL을 추가하거나 편집하려면 입력 필드에 URL을 입력합니다.

   * 다른 사용자 지정 추적 URL을 추가하려면 **[!UICONTROL +]**&#x200B;을(를) 클릭하고 입력 필드에 URL을 입력합니다.

   * 사용자 지정 URL을 제거하려면 Creative 행 위에 커서를 놓고 ![삭제](/help/creative/assets/delete.png "삭제")를 클릭합니다.

1. 대화 상자에서 **[!UICONTROL Save]**&#x200B;을(를) 클릭하여 작업 트리를 업데이트합니다.

1. 트리 헤더에서 [환경을 저장](#save)합니다.

## 경험 저장 {#save}

다음 단계는 두 편집기에 모두 적용됩니다. 추적 URL 대화 상자만 저장해도 경험이 저장되거나 게시되지 않습니다.

{{$include /help/_includes/experience-save.md}}

>[!MORELIKETHIS]
>
>* [경험의 최종 노드에 Creative 번들 할당 및 할당 해제](/help/creative/experiences/experience-assign-creative-bundles.md)
>* [의사 결정 트리 타깃팅 없이 경험에 대한 추적 URL 사용자 지정](experience-tracking-urls-no-targeting.md)
