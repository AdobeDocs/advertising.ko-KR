---
title: 의사 결정 트리 타겟팅으로 경험 편집
description: AI 기반 또는 수동 의사 결정 트리 편집기를 사용하여 타깃팅된 광고 경험을 편집하는 방법을 알아봅니다.
feature: Creative Experiences
exl-id: 8c5e8f9b-c405-41b2-98a9-da7c5debd3e1
TQID: 'https://experienceleague.adobe.com/0mcPjfiET-DKrm2qaa1Odygv1GIgv4cR7lBRNmrYGBk'
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
source-wordcount: '655'
ht-degree: 0%
---
# 의사 결정 트리 타겟팅으로 경험 편집

AI 기반 편집기(Beta)는 타깃팅이 있는 경험에 대해 기본적으로 열립니다. AI 에이전트로 작업하거나 캔버스를 직접 편집하거나 기존 수동 편집기를 열 수 있습니다.

## 경험 열기 {#experience-open}

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Experiences]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 특정 경험을 포함하도록 [보기를 사용자 지정](/help/creative/introduction/customize-data-views.md)합니다.

1. 다음 중 하나를 수행합니다.

   * AI 기반 편집기를 열려면 다음을 수행하십시오.

     * 카드 보기에서 경험 이름 옆의 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

     * 테이블 보기에서 행 위에 커서를 놓고 **[!UICONTROL More]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

   * 수동 편집기를 열려면

     * 카드 보기에서 경험 이름 옆의 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Create Decision Tree Manually (Legacy)]**&#x200B;을(를) 클릭합니다.

     * 테이블 보기에서 행 위에 커서를 놓고 **[!UICONTROL More]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Create Decision Tree Manually (Legacy)]**&#x200B;을(를) 클릭합니다.

     * AI 기반 편집기 내에서

## AI 기반 편집기를 사용하여 편집(Beta) {#ai-editor}

1. [경험 열기](#experience-open).

1. 대화에서 원하는 타겟팅 변경 사항을 설명합니다. 영향을 받는 분기를 대상으로 식별하거나 캔버스에 표시되면 노드 ID를 사용하여 식별하십시오.

1. 업데이트된 트리를 검토하고 추가 변경 사항을 설명합니다. 캔버스와 상호 작용하기 전에 도우미가 처리를 완료할 때까지 기다립니다.

1. (선택 사항) 캔버스에서 직접 변경합니다.

   * [최종 수준 대상을 추가](experience-target-node-add-final.md#ai-editor), [대상 수준을 삽입](experience-target-node-add-inner.md#ai-editor) 또는 [형제 대상을 추가](experience-target-node-add-sibling.md#ai-editor)합니다.

   * 대상 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Edit]**&#x200B;을(를) 클릭하고 값을 변경한 다음 **[!UICONTROL Edit Node]**&#x200B;을(를) 클릭하여 대상의 기준을 편집합니다.

   * [하위 노드 및 광고 크리에이티브 복사](experience-target-node-copy.md#ai-editor) 또는 [노드 삭제](experience-target-node-delete.md#ai-editor).

   * [Creative 번들 할당 또는 할당 해제](experience-assign-creative-bundles.md#ai-editor).

   * [크리에이티브 최적화 및 일정 사용자 지정](experience-optimization-scheduling-targeting.md) 또는 [추적 URL](experience-tracking-urls-targeting.md#ai-editor).

1. [경험 저장](#save).

## 수동 편집기를 사용하여 편집 {#manual-editor}

1. [경험 열기](#experience-open).

1. (상태가 `[processing](experience-about.md#experience-statuses)`인 경험) 게시되지 않은 기존 초안에 대한 메시지가 표시되면 다음 중 하나를 수행하십시오.

   * 초안을 검토하고 계속 편집하려면 **[!UICONTROL Continue editing draft]**&#x200B;을(를) 클릭하십시오.

   * **[!UICONTROL Discard and start again]**&#x200B;을(를) 클릭하여 초안을 삭제하고 라이브 버전에서 시작하십시오.

   * 편집을 중지하려면 **[!UICONTROL Cancel this edit]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 확대/축소 슬라이더를 조정하거나 ![세로 트리로 보기](/help/creative/assets/tree-vertical.png "세로 트리로 보기") 또는 ![가로 트리로 보기](/help/creative/assets/tree-horizontal.png "가로 트리로 보기")을(를) 클릭하여 방향을 변경합니다.

   보기 설정은 로그아웃할 때까지 저장됩니다.

1. 필요에 따라 타겟 및 크리에이티브를 변경합니다.

   * [최종 수준 대상을 추가](experience-target-node-add-final.md#manual-editor), [노드 사이에 대상 삽입](experience-target-node-add-inner.md#manual-editor) 또는 [형제 대상을 추가](experience-target-node-add-sibling.md#manual-editor)합니다.

   * [하위 노드 및 광고 크리에이티브 복사](experience-target-node-copy.md#manual-editor) 또는 [노드 삭제](experience-target-node-delete.md#manual-editor).

   * [Creative 번들 할당 또는 할당 해제](experience-assign-creative-bundles.md#manual-editor).

   * [크리에이티브 최적화 및 일정 사용자 지정](experience-optimization-scheduling-targeting.md) 또는 [추적 URL](experience-tracking-urls-targeting.md#manual-editor).

1. [경험 저장](#save).

## 편집기 전환 또는 경험 설정 편집 {#switch-editors}

>[!IMPORTANT]
>
>AI 기반 편집기를 종료하기 전에 유지할 트리 변경 사항을 저장하십시오. 수동 편집기 또는 경험 양식으로 전환해도 저장되지 않은 변경 사항은 전송되지 않습니다.

* **수동 편집기에 대한 AI 기반 편집기:** **[!UICONTROL Manual Decision Tree]**&#x200B;을(를) 클릭합니다. 확인 대화 상자에서 **[!UICONTROL Yes]**&#x200B;을(를) 클릭하여 저장되지 않은 변경 내용을 삭제하고 수동 편집기를 열거나 **[!UICONTROL No]**&#x200B;을(를) 클릭하여 유지합니다.

* **일반 설정에 대한 AI 기반 편집기:** **[!UICONTROL Experience Form]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Yes]**&#x200B;을(를) 클릭하여 저장되지 않은 트리 변경 내용을 취소하고 양식을 엽니다. [일반 환경 설정](experience-settings-targeting.md)을 편집한 다음 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

* **일반 설정에 대한 수동 편집기:** 유지할 트리 변경 내용을 저장한 다음 **[!UICONTROL Experience Form]**&#x200B;을(를) 클릭합니다. [일반 환경 설정](experience-settings-targeting.md)을 편집한 다음 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

* **AI 기반 편집기에 대한 일반 설정:** **[!UICONTROL Decision Tree]**&#x200B;을(를) 클릭합니다. 타겟팅된 경험의 일반 설정에 대한 변경 사항을 저장하면 AI 기반 편집기도 열립니다.

* **AI 기반 편집기의 수동 편집기:** 트리 변경 내용을 저장하고 [!UICONTROL Experiences] 보기로 돌아간 다음 경험에 대해 **[!UICONTROL Edit]**&#x200B;을(를) 선택하십시오.

다른 편집기를 열지 않고 AI 기반 편집기를 종료하려면 **[!UICONTROL Cancel]**&#x200B;을(를) 클릭합니다. 저장하지 않은 트리 변경 내용을 취소하려면 **[!UICONTROL Yes]**&#x200B;을(를) 클릭하고 편집을 계속하려면 **[!UICONTROL No]**&#x200B;을(를) 클릭하십시오.

## 경험 저장 {#save}

다음 단계는 두 편집기에 모두 적용됩니다.

{{$include /help/_includes/experience-save.md}}

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
>* [경험에 대한 변경 로그 보기](/help/creative/experiences/experience-view-change-log.md)
