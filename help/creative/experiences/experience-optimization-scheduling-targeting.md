---
title: 경험을 위한 크리에이티브 최적화 및 일정 사용자 정의
description: 타겟팅된 경험에 대한 최적화 및 광고 예약을 구성하는 방법을 알아봅니다.
feature: Creative Experiences
exl-id: 47d1a249-decd-4c3b-ac88-260488d5bcd2
source-git-commit: 9c7f3d2aec0952b38d2fd3097d0b3499d33bf3b8
workflow-type: tm+mt
source-wordcount: '1085'
ht-degree: 0%

---

# 의사 결정 트리 타겟팅을 사용하는 경험에 대한 크리에이티브 최적화 및 예약 사용자 지정

*기존 크리에이티브만 있는 노드 타깃팅*

기본적으로 경험에 대한 크리에이티브 순환은 전체 클릭스루 속도를 최적화하기 위해 알고리즘적으로 결정되며 크리에이티브 최적화 설정은 할당된 모든 번들에 적용됩니다. 지정된 Advertising DSP 사용자 지정 목표에 대해 알고리즘을 통해 최적화하거나, 각 번들 시퀀스에 대해 지정된 노출 횟수로 지정된 번들 시퀀스에 따라 번들을 회전하거나, 상대 가중치에 따라 번들을 회전할 수 있습니다. 또한 특정 크리에이티브 번들이 지정된 순차적 기간 동안 실행되도록 예약하고 각 예약에 대해 사용자 정의 크리에이티브 순환 설정을 적용할 수 있습니다.

>[!NOTE]
>
>할당된 크리에이티브 대신 기본 크리에이티브를 사용하는 노드에는 이러한 기능을 사용할 수 없습니다.

## 예약 없이 크리에이티브 최적화 구성

크리에이티브 일정이 비활성화되면 크리에이티브 최적화 설정이 할당된 모든 크리에이티브에 적용됩니다.

1. 대상 노드 아래의 크리에이티브 리프 노드 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Creative Optimization]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Schedule]**&#x200B;을(를) 사용하지 않도록 설정합니다.

1. 연결된 번들의 광고 변형에 대한 크리에이티브 회전 유형을 선택합니다.

   * *[!UICONTROL Weighted]:* 상대 가중치에 따라 연결된 Creative 번들의 광고 변형을 표시합니다. 각 번들의 가중치를 백분율로 입력합니다. 선택한 모든 번들에 대한 가중치는 최대 100.<!-- For example, if Bundle 1 is 60 and Bundle 2 is 40, then Bundle 1 is shown 60% of the time, and Bundle 2 is shown 40% of the time. -->까지 추가해야 합니다.

   * *[!UICONTROL Algorithmic]:* 지정된 목표를 기반으로 가장 효과적인 광고 변형을 더 자주 표시합니다.

      * **[!UICONTROL Optimization Goal]**&#x200B;에 대해 *[!UICONTROL Click Through Rate]*, (표준 비디오 광고 경험) *[!UICONTROL Completion Rate]* 또는 *[!UICONTROL Custom Objective]*&#x200B;을(를) 선택하십시오.  *[!UICONTROL Custom Objective]*&#x200B;을(를) 선택한 다음 기존 [Advertising DSP 사용자 지정 목표](/help/dsp/optimization/custom-goal.md)를 선택합니다.

   * *[!UICONTROL Sequencing]:* 연결된 크리에이티브 번들을 지정된 순서로 표시합니다(첫 번째로 제공된 번들 1, 두 번째로 제공된 번들 2 등). 이때 각 번들 시퀀스에 대해 지정된 총 노출 수가 표시됩니다. 제공되는 광고 크기는 사용 가능한 인벤토리에 의해 결정됩니다. a\) 무기한으로 표시되거나(기본값) b\) 다시 첫 번째 번들로 루프백되도록 시퀀스의 마지막 번들을 구성할 수 있습니다. 예를 들어, 3개의 (3) 노출에 대해 번들 1에 광고 변형을 표시한 다음 하나의 (1) 노출에 대해 번들 2에 광고 변형을 표시한 다음 2개의 (2) 노출에 대해 번들 3에 광고 변형을 표시한 다음 루프를 다시 시작할 수 있습니다. 또는 번들 3의 광고 변형이 표시되면 루프를 만드는 대신 번들 3의 광고 변형을 계속 무기한으로 표시할 수 있습니다. 순번 지정 사용 시:

      1. 할당된 번들을 원하는 순서로 끌어다 놓습니다.

     할당된 번들은 기본적으로 경험에 추가된 순서대로 순서가 지정됩니다.

      1. 각 시퀀스에 대한 노출 횟수를 입력합니다.

      1. 마지막 시퀀스의 경우, a\) 시퀀스에 최종 번들을 무기한으로 표시할지(*[!UICONTROL Infinite]*(기본값) 또는 b\) 최종 번들이 표시된 후 첫 번째 번들로 다시 루프할지(*[!UICONTROL Keep in Loop]*) 변경합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## Creative Scheduling을 통해 크리에이티브 최적화 구성

선택적으로 경험 시작일과 종료일 사이의 지정된 순차적 기간 동안 특정 크리에이티브 번들이 실행되도록 예약하고, 각 예약에 대해 사용자 정의 크리에이티브 순환 설정을 적용할 수 있습니다. 예를 들어 번들 1이 첫 2주 동안 실행되어 클릭스루 비율에 최적화되고 번들 2가 다음 2주 동안 실행되어 지정된 사용자 지정 목표에 최적화되도록 예약할 수 있습니다.

예약을 사용할 때는 경험 기간 동안 번들을 예약해야 합니다.

1. 대상 노드 아래의 크리에이티브 리프 노드 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Creative Optimization]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Schedule]** 사용

1. 첫 번째 예약의 경우:

   1. 왼쪽 열에서 첫 번째 예약에 추가할 각 Creative 번들 옆의 확인란을 선택합니다.

   1. 일정의 시작 및 종료 날짜를 지정합니다.

   1. 크리에이티브 순환 유형을 선택합니다.

      * *[!UICONTROL Weighted]:* 각 번들의 크리에이티브를 상대 가중치에 따라 수동으로 회전합니다. 각 번들의 가중치를 백분율로 입력합니다. 선택한 모든 번들에 대한 가중치는 최대 100까지 추가해야 합니다.

      * *[!UICONTROL Algorithmic]:* 지정된 최적화 목표에 따라 각 번들의 크리에이티브를 알고리즘 방식으로 회전합니다.

         * **[!UICONTROL Optimization Goal]**&#x200B;에 대해 *[!UICONTROL Click Through Rate]*, (표준 비디오 광고 경험) *[!UICONTROL Completion Rate]* 또는 *[!UICONTROL Custom Objective]*&#x200B;을(를) 선택하십시오.  *[!UICONTROL Custom Objective]*&#x200B;을(를) 선택한 다음 기존 [Advertising DSP 사용자 지정 목표](/help/dsp/optimization/custom-goal.md)를 선택합니다.

      * *[!UICONTROL Sequencing]:* 연결된 크리에이티브 번들을 지정된 순서로 회전합니다(첫 번째로 제공된 번들 1, 두 번째로 제공된 번들 2 등). 이때 각 번들 시퀀스에 대해 지정된 총 노출 횟수는 동일합니다. 제공되는 광고 크기는 사용 가능한 인벤토리에 의해 결정됩니다. a\) 무기한으로 표시되거나(기본값) b\) 다시 첫 번째 번들로 루프백되도록 시퀀스의 마지막 번들을 구성할 수 있습니다. 예를 들어, 3개의 (3) 노출에 대해 1번에서 모든 크리에이티브를 표시한 다음, 1개의 (1) 노출에 대해 2번에서 모든 크리에이티브를 표시한 다음, 2개의 (2) 노출에 대해 3번에서 모든 크리에이티브를 표시한 다음 루프를 다시 시작할 수 있습니다. 또는 번들 3의 크리에이티브가 표시되면 루프를 만드는 것이 아니라 계속 번들 3의 크리에이티브를 무한정 표시할 수 있습니다. 순번 지정 사용 시:

         1. 할당된 번들을 원하는 순서로 끌어다 놓습니다.

            할당된 번들은 기본적으로 경험에 추가된 순서대로 순서가 지정됩니다.

         1. 각 시퀀스에 대한 노출 횟수를 입력합니다.

         1. 마지막 시퀀스의 경우, a\) 시퀀스에 최종 번들을 무기한으로 표시할지(*[!UICONTROL Infinite]*(기본값) 또는 b\) 최종 번들이 표시된 후 첫 번째 번들로 다시 루프할지(*[!UICONTROL Keep in Loop]*) 변경합니다.

1. 각 추가 일정에 대해:

   1. **[!UICONTROL + Add Schedule]**&#x200B;을(를) 클릭합니다.

   1. 왼쪽 열에서 첫 번째 예약에 추가할 각 Creative 번들 옆의 확인란을 선택합니다.

   1. 일정의 시작 및 종료 날짜를 지정합니다.

   1. 크리에이티브 순환 유형을 선택합니다.

      * *[!UICONTROL Weighted]:* 각 번들의 크리에이티브를 상대 가중치에 따라 수동으로 회전합니다. 각 번들의 가중치를 백분율로 입력합니다. 선택한 모든 번들에 대한 가중치는 최대 100까지 추가해야 합니다.

      * *[!UICONTROL Algorithmic]:* 지정된 최적화 목표에 따라 각 번들의 크리에이티브를 알고리즘 방식으로 회전합니다.

         * **[!UICONTROL Optimization Goal]**&#x200B;에 대해 *[!UICONTROL Click Through Rate]* 또는 *[!UICONTROL Custom Objective]*&#x200B;을(를) 선택하십시오.  *[!UICONTROL Custom Objective]*&#x200B;을(를) 선택한 다음 기존 [Advertising DSP 사용자 지정 목표](/help/dsp/optimization/custom-goal.md)를 선택합니다.

      * *[!UICONTROL Sequencing]:* 각 번들 시퀀스에 대해 지정된 총 노출 횟수로 연결된 Creative 번들을 지정된 순서로 회전합니다. 순번 지정 사용 시:

         1. 할당된 번들을 원하는 순서로 끌어다 놓습니다.

            할당된 번들은 기본적으로 경험에 추가된 순서대로 순서가 지정됩니다.

         1. 각 시퀀스에 대한 노출 횟수를 입력합니다.

         1. 마지막 시퀀스의 경우, a\) 시퀀스에 최종 번들을 무기한으로 표시할지(*[!UICONTROL Infinite]*(기본값) 또는 b\) 최종 번들이 표시된 후 첫 번째 번들로 다시 루프할지(*[!UICONTROL Keep in Loop]*) 변경합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [경험의 최종 노드에 Creative 번들 할당 및 할당 해제](/help/creative/experiences/experience-assign-creative-bundles.md)
>* [광고 추적 URL 사용자 지정](/help/creative/experiences/experience-tracking-urls-targeting.md)
