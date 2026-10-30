---
title: 의사 결정 트리 타겟팅으로 경험 만들기
description: AI 기반 또는 수동 의사 결정 트리 편집기를 사용하여 타깃팅된 광고 경험을 만드는 방법을 알아봅니다.
feature: Creative Experiences
exl-id: 825fd9af-ca7a-4b44-8e4b-1a6f34edac9e
TQID: 'https://experienceleague.adobe.com/nxegtoNEqfAk7LUyb-3qD6YJYaGfx3M3QdrLx-q5y14'
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
    internal-label: Demand Side Platform
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
source-wordcount: '715'
ht-degree: 0%
---
# 의사 결정 트리 타겟팅으로 경험 만들기

의사 결정 트리를 사용하여 타깃팅된 광고 경험을 만듭니다. 각 경험은 단일 크리에이티브 라이브러리의 광고를 사용합니다.

기본적으로 AI 기반 편집기(Beta)가 열립니다. AI 에이전트를 통해 트리를 구성하거나 해당 캔버스를 직접 편집할 수 있습니다. 기존 수동 편집기로 전환할 수도 있습니다.

>[!NOTE]
>
>* 타겟팅된 경험을 만들면 나중에 다른 워크플로우를 사용하는 타겟팅되지 않은 경험으로 변경할 수 없습니다.
>* 광고 경험에 구현할 캠페인과 호환되는 타겟팅이 포함되어 있는지 확인하십시오. 계층 타겟팅 동작은 DSP에 따라 다를 수 있습니다. 광고 경험 태그를 Advertising DSP에 업로드하고 배치에 첨부하면 광고 수준 타깃팅이 배치 수준 타깃팅 (대신 적용되지 않음) 위에 적용됩니다. 예를 들어 배치가 오스트레일리아의 사용자를 타겟팅하고 광고가 일본의 사용자를 타겟팅하는 경우 광고는 &quot;기타 사용자&quot; 분기를 타겟팅합니다.

## 경험 만들기

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Experiences]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Create New Experience]**&#x200B;을(를) 클릭합니다.

1. [일반 경험 설정](experience-settings-targeting.md)을(를) 입력하십시오. **[!UICONTROL Targeting]**&#x200B;은(는) 활성화되어 있습니다.

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

   새 경험을 위한 AI 기반 의사 결정 트리 편집기가 열립니다.

1. 다음 절차 중 하나를 사용하여 트리를 구성합니다.

## AI 기반 편집기(Beta)를 사용하여 트리 구성 {#ai-editor}

1. 대화에서 각 분기의 기준과 지정된 대상과 일치하지 않는 뷰어를 처리하는 방법을 포함하여 원하는 타깃팅 구조를 설명합니다.

1. 캔버스에서 트리를 검토합니다. 변경을 요청하려면 대화에 설명을 입력합니다. 캔버스와 상호 작용하기 전에 도우미가 처리를 완료할 때까지 기다립니다.

1. (선택 사항) 캔버스에서 직접 트리를 세분화합니다.

   * [최종 수준 대상을 추가](experience-target-node-add-final.md#ai-editor), [대상 수준을 삽입](experience-target-node-add-inner.md#ai-editor) 또는 [형제 대상을 추가](experience-target-node-add-sibling.md#ai-editor)합니다.

   * [하위 노드 및 광고 크리에이티브 복사](experience-target-node-copy.md#ai-editor) 또는 [노드 삭제](experience-target-node-delete.md#ai-editor).

1. [크리에이티브 번들을 최종 노드에 할당](experience-assign-creative-bundles.md#ai-editor), 선택적으로 [크리에이티브 최적화 및 일정 사용자 지정](experience-optimization-scheduling-targeting.md) 및 [추적 URL](experience-tracking-urls-targeting.md#ai-editor)합니다.

   경험을 게시하려면 각 최종 노드에 번들을 할당하거나 경험의 기본 크리에이티브를 사용해야 합니다. 저장할 때 할당되지 않은 노드에 기본값을 할당할 수 있습니다.

1. (선택 사항) 일반 경험 설정을 편집합니다.

   1. 유지할 트리 변경 내용을 저장하려면 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

   1. **[!UICONTROL Experience Form]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Yes]**&#x200B;을(를) 클릭하여 저장되지 않은 트리 변경 내용을 취소하고 양식을 엽니다.

   1. [일반 환경 설정](experience-settings-targeting.md)을 편집한 다음 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

      AI 기반 편집기가 열립니다.

1. [경험 저장](#save).

## 수동 편집기를 사용하여 트리 구성 {#manual-editor}

1. AI 기반 편집기에서 **[!UICONTROL Manual Decision Tree]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Yes]**&#x200B;을(를) 클릭하여 AI 기반 편집기에서 나갑니다.

   전환하기 전에 유지할 AI 편집기 변경 사항을 모두 저장합니다. 스위치를 확인하면 저장되지 않은 트리 변경 내용이 삭제됩니다.

1. (선택 사항) 보기 설정을 변경합니다.

   * 슬라이더를 이동하여 확대 또는 축소합니다.

   * ![세로 트리로 보기](/help/creative/assets/tree-vertical.png "세로 트리로 보기") 또는 ![가로 트리로 보기](/help/creative/assets/tree-horizontal.png "가로 트리로 보기")을 클릭하여 세로 보기와 가로 보기 사이를 전환합니다.

   보기 설정은 로그아웃할 때까지 저장됩니다.

1. 광고 대상 및 해당 광고 크리에이티브를 구성합니다.

   * [최종 수준 대상을 추가](experience-target-node-add-final.md#manual-editor), [노드 사이에 대상 삽입](experience-target-node-add-inner.md#manual-editor) 또는 [형제 대상을 추가](experience-target-node-add-sibling.md#manual-editor)합니다.

   * [하위 노드 및 광고 크리에이티브 복사](experience-target-node-copy.md#manual-editor) 또는 [노드 삭제](experience-target-node-delete.md#manual-editor).

   * [크리에이티브 번들을 할당](experience-assign-creative-bundles.md#manual-editor)하고 선택적으로 [크리에이티브 최적화 및 일정 사용자 지정](experience-optimization-scheduling-targeting.md) 및 [추적 URL](experience-tracking-urls-targeting.md#manual-editor)합니다.

1. (선택 사항) 일반 경험 설정을 편집하려면 **[!UICONTROL Experience Form]**&#x200B;을(를) 클릭하고 [일반 경험 설정](experience-settings-targeting.md)을(를) 편집하십시오.

1. [경험 저장](#save).

## 경험 저장 {#save}

다음 단계는 두 편집기에 모두 적용됩니다.

{{$include /help/_includes/experience-save.md}}

## 저장된 경험을 위한 광고 태그 및 비디오 트랜스코딩

경험이 라이브되면 [!DNL Creative]은(는) 각 적용 가능한 광고 크기 또는 비디오 지속 시간에 대해 하나의 광고 태그를 자동으로 만듭니다. 그런 다음 [광고 태그를 내보내고 DSP에서 구현](/help/creative/experiences/experience-tag-export.md)할 수 있습니다.

비디오 광고 경험의 경우 비디오 크리에이티브가 Adobe Advertising DSP as VAST 2.0 태그로 자동으로 코드 변환되므로 미리 볼 수 있습니다. 원할 경우 [다른 DSP에 대한 코드 변환 적용을](experience-tag-video-transcoding.md)할 수 있습니다.

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
>* [경험에 대한 변경 로그 보기](/help/creative/experiences/experience-view-change-log.md)
