---
title: 경험을 위한 크리에이티브 최적화 및 일정 사용자 정의
description: 방법 알아보기
feature: Creative Experiences
source-git-commit: fd925c641bef7953aea50813725252c3913757fa
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 0%

---

# 의사 결정 트리 타겟팅을 사용하는 경험에 대한 크리에이티브 최적화 및 예약 사용자 지정

*기존 크리에이티브만 있는 노드 타깃팅*
*Beta 완료*

기본적으로 경험에 대한 크리에이티브 순환은 전체 클릭스루 속도를 최적화하기 위해 알고리즘적으로 결정되며 크리에이티브 최적화 설정은 할당된 모든 번들에 적용됩니다. 상대적 가중치에 따라 각 번들에서 크리에이티브를 수동으로 실행하거나 지정된 Advertising DSP 사용자 지정 목표에 대해 알고리즘적으로 최적화하도록 크리에이티브 순환을 사용자 지정할 수 있습니다. <!-- verify --> 또한 특정 크리에이티브 번들이 지정된 순차적 기간 동안 실행되도록 예약하고 각 예약에 대해 사용자 지정 크리에이티브 순환 설정을 적용할 수 있습니다.

>[!NOTE]
>
>할당된 크리에이티브 대신 기본 이미지 크리에이티브를 사용하는 노드에는 이러한 기능을 사용할 수 없습니다.

## 예약 없이 크리에이티브 최적화 구성

크리에이티브 일정이 비활성화되면 크리에이티브 최적화 설정이 할당된 모든 크리에이티브에 적용됩니다.

1. 대상 노드 아래의 크리에이티브 리프 노드 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Edit Schedules]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Schedule]**&#x200B;을(를) 사용하지 않도록 설정합니다.

1. 크리에이티브 순환 유형을 선택합니다.

   * ** *Weighted* ** — 상대 가중치에 따라 각 번들의 크리에이티브를 수동으로 회전합니다. 각 번들의 가중치를 백분율로 입력합니다. 모든 번들의 무게는 최대 100까지 더해야 합니다.

   * ** *알고리즘* ** — 지정된 최적화 목표에 따라 각 번들의 크리에이티브를 알고리즘 방식으로 회전합니다.

   * **[!UICONTROL Optimization Goal]**&#x200B;에 대해 *[!UICONTROL Click Through Rate]* 또는 *[!UICONTROL Custom Objective]*&#x200B;을(를) 선택하십시오.  *[!UICONTROL Custom Objective]*&#x200B;을(를) 선택한 다음 기존 [Advertising DSP 사용자 지정 목표](/help/dsp/optimization/custom-goal.md)를 선택합니다.<!-- Verify -->

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## Creative Scheduling을 통해 크리에이티브 최적화 구성

선택적으로 경험 시작일과 종료일 사이의 지정된 순차적 기간 동안 특정 크리에이티브 번들이 실행되도록 예약하고, 각 예약에 대해 사용자 정의 크리에이티브 순환 설정을 적용할 수 있습니다. 예를 들어 번들 1이 첫 2주 동안 실행되어 클릭스루 비율에 최적화되고 번들 2가 다음 2주 동안 실행되어 지정된 사용자 지정 목표에 최적화되도록 예약할 수 있습니다.

예약을 사용할 때는 경험 기간 동안 번들을 예약해야 합니다.

1. 대상 노드 아래의 크리에이티브 리프 노드 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Edit Schedules]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Schedule]** 사용

1. 첫 번째 예약의 경우:

   1. 왼쪽 열에서 첫 번째 예약에 추가할 각 Creative 번들 옆의 확인란을 선택합니다.

   1. 일정의 시작 및 종료 날짜를 지정합니다.

   1. 크리에이티브 순환 유형을 선택합니다.

      * ** *Weighted* ** — 상대 가중치에 따라 각 번들의 크리에이티브를 수동으로 회전합니다. 각 번들의 가중치를 백분율로 입력합니다. 선택한 모든 번들에 대한 가중치는 최대 100까지 추가해야 합니다.

      * ** *알고리즘* ** — 지정된 최적화 목표에 따라 각 번들의 크리에이티브를 알고리즘 방식으로 회전합니다.

      * **[!UICONTROL Optimization Goal]**&#x200B;에 대해 *[!UICONTROL Click Through Rate]* 또는 *[!UICONTROL Custom Objective]*&#x200B;을(를) 선택하십시오.  *[!UICONTROL Custom Objective]*&#x200B;을(를) 선택한 다음 기존 [Advertising DSP 사용자 지정 목표](/help/dsp/optimization/custom-goal.md)를 선택합니다.<!-- Verify -->

1. 각 추가 일정에 대해:

   1. **[!UICONTROL + Add Schedule]**&#x200B;을(를) 클릭합니다.

   1. 왼쪽 열에서 첫 번째 예약에 추가할 각 Creative 번들 옆의 확인란을 선택합니다.

   1. 일정의 시작 및 종료 날짜를 지정합니다.

   1. 크리에이티브 순환 유형을 선택합니다.

      * ** *Weighted* ** — 상대 가중치에 따라 각 번들의 크리에이티브를 수동으로 회전합니다. 각 번들의 가중치를 백분율로 입력합니다. 선택한 모든 번들에 대한 가중치는 최대 100까지 추가해야 합니다.

      * ** *알고리즘* ** — 지정된 최적화 목표에 따라 각 번들의 크리에이티브를 알고리즘 방식으로 회전합니다.

      * **[!UICONTROL Optimization Goal]**&#x200B;에 대해 *[!UICONTROL Click Through Rate]* 또는 *[!UICONTROL Custom Objective]*&#x200B;을(를) 선택하십시오.  *[!UICONTROL Custom Objective]*&#x200B;을(를) 선택한 다음 기존 [Advertising DSP 사용자 지정 목표](/help/dsp/optimization/custom-goal.md)를 선택합니다.<!-- Verify -->

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [경험의 최종 노드에 Creative 번들 할당 및 할당 해제](/help/creative/experiences/experience-assign-creative-bundles.md)
>* [광고 추적 URL 사용자 지정](/help/creative/experiences/experience-tracking-urls-targeting.md)
