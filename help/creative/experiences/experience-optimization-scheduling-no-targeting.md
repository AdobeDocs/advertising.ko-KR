---
title: 경험을 위한 크리에이티브 최적화 및 일정 사용자 정의
description: 방법 알아보기
feature: Creative Experiences
exl-id: 9398df69-6a48-4b72-8c5c-a79341bf3b8a
source-git-commit: a271589a2cb51ec50c37a52254fd8d1b535f279a
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 0%

---

# 의사 결정 트리 타깃팅 없이 경험에 대한 크리에이티브 최적화 및 예약 사용자 지정

기존 크리에이티브만 있는 *경험*

기본적으로 광고 경험 태그에 대한 크리에이티브 순환은 전체 클릭스루 속도를 최적화하도록 알고리즘적으로 결정되며 크리에이티브 최적화 설정은 할당된 모든 크리에이티브에 적용됩니다. 상대적 가중치에 따라 크리에이티브를 수동으로 실행하거나 지정된 Advertising DSP 사용자 지정 목표에 맞게 알고리즘적으로 최적화하도록 크리에이티브 회전을 사용자 지정할 수 있습니다. 또한 특정 크리에이티브가 지정된 순차적 기간 동안 실행되도록 예약하고 각 예약에 대해 사용자 정의 크리에이티브 순환 설정을 적용할 수 있습니다.

## 예약 없이 크리에이티브 최적화 구성

크리에이티브 일정이 비활성화되면 크리에이티브 최적화 설정이 할당된 모든 크리에이티브에 적용됩니다.

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Experiences]**&#x200B;을(를) 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * 카드 보기에서 경험 이름 옆의 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Tag Manager]**&#x200B;을(를) 클릭합니다.

   * 테이블 보기에서 행 위에 커서를 놓고 **[!UICONTROL More]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Tag Manager]**&#x200B;을(를) 클릭합니다.

1. 적용 가능한 광고 태그의 행 위에 커서를 놓고 ![광고 일정](/help/creative/assets/edit-gray.png "추적 URL 편집") **[!UICONTROL Creative Optimization]**&#x200B;을 클릭합니다.&lt;!— 2/2부터 Tag Manager에는 목록 보기만 있고 카드 보기는 없습니다. >

1. **[!UICONTROL Schedule]**&#x200B;을(를) 사용하지 않도록 설정합니다.

1. 크리에이티브 순환 유형을 선택합니다.

   * *[!UICONTROL Weighted]:* 상대 가중치에 따라 크리에이티브를 수동으로 회전합니다. 각 크리에이티브에 대한 가중치를 백분율로 입력합니다. 선택한 모든 크리에이티브에 대한 가중치는 최대 100개여야 합니다.

   * *[!UICONTROL Algorithmic]:* 지정한 최적화 목표에 따라 창의력을 알고리즘적으로 회전합니다.

      * **[!UICONTROL Optimization Goal]**&#x200B;에 대해 *[!UICONTROL Click Through Rate]*, (표준 비디오 광고 경험) *[!UICONTROL Completion Rate]* 또는 *[!UICONTROL Custom Objective]*&#x200B;을(를) 선택하십시오.  *[!UICONTROL Custom Objective]*&#x200B;을(를) 선택한 다음 기존 [Advertising DSP 사용자 지정 목표](/help/dsp/optimization/custom-goal.md)를 선택합니다.<!-- Verify -->

   * *[!UICONTROL Sequencing]:* 연결된 크리에이티브 번들을 지정된 순서로 회전합니다(첫 번째로 제공된 번들 1, 두 번째로 제공된 번들 2 등). 이때 각 번들 시퀀스에 대해 지정된 총 노출 횟수는 동일합니다. 제공되는 광고 크기는 사용 가능한 인벤토리에 의해 결정됩니다. a\) 무기한으로 표시되거나(기본값) b\) 다시 첫 번째 번들로 루프백되도록 시퀀스의 마지막 번들을 구성할 수 있습니다. 예를 들어, 3개의 (3) 노출에 대해 1번에서 모든 크리에이티브를 표시한 다음, 1개의 (1) 노출에 대해 2번에서 모든 크리에이티브를 표시한 다음, 2개의 (2) 노출에 대해 3번에서 모든 크리에이티브를 표시한 다음 루프를 다시 시작할 수 있습니다. 또는 번들 3의 크리에이티브가 표시되면 루프를 만드는 것이 아니라 계속 번들 3의 크리에이티브를 무한정 표시할 수 있습니다. 순번 지정 사용 시:

      1. 할당된 번들을 원하는 순서로 끌어다 놓습니다.

     할당된 번들은 기본적으로 경험에 추가된 순서대로 순서가 지정됩니다.

      1. 각 시퀀스에 대한 노출 횟수를 입력합니다.

      1. 마지막 시퀀스의 경우, a\) 시퀀스에 최종 번들을 무기한으로 표시할지(*[!UICONTROL Infinite]*(기본값) 또는 b\) 최종 번들이 표시된 후 첫 번째 번들로 다시 루프할지(*[!UICONTROL Keep in Loop]*) 변경합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## Creative Scheduling을 통해 크리에이티브 최적화 구성

광고 경험 태그에 사용된 특정 크리에이티브를 경험 시작일과 종료일 사이의 지정된 순차적 기간 동안 실행하도록 선택적으로 예약하고, 각 예약에 대해 사용자 지정 크리에이티브 순환 설정을 적용할 수 있습니다. 예를 들어 Creative 1이 클릭스루 속도에 최적화되도록 첫 2주 동안 실행되도록 예약하고 Creative 2가 지정된 사용자 지정 목표에 최적화되도록 다음 2주 동안 실행되도록 예약할 수 있습니다.

예약을 사용할 때는 경험 기간 동안 크리에이티브를 예약해야 합니다.

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Experiences]**&#x200B;을(를) 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * 카드 보기에서 경험 이름 옆의 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Tag Manager]**&#x200B;을(를) 클릭합니다.

   * 테이블 보기에서 행 위에 커서를 놓고 **[!UICONTROL More]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Tag Manager]**&#x200B;을(를) 클릭합니다.

1. 적용 가능한 광고 태그의 행 위에 커서를 놓고 ![광고 일정](/help/creative/assets/edit-gray.png "추적 URL 편집") **[!UICONTROL Creative Optimization]**&#x200B;을 클릭합니다. <!-- For targeted experiences, this is "Edit Schedules" -->&lt;!— 2/2부터 Tag Manager에는 목록 보기만 있고 카드 보기는 없습니다. >

1. **[!UICONTROL Schedule]** 사용

1. 첫 번째 예약의 경우:

   1. 왼쪽 열에서 첫 번째 예약에 추가할 각 크리에이티브 옆의 확인란을 선택합니다.

   1. 일정의 시작 및 종료 날짜를 지정합니다.

   1. 크리에이티브 순환 유형을 선택합니다.

      * *[!UICONTROL Weighted]:* 상대 가중치에 따라 크리에이티브를 수동으로 회전합니다. 각 크리에이티브에 대한 가중치를 백분율로 입력합니다. 선택한 모든 크리에이티브에 대한 가중치는 최대 100개여야 합니다.

      * *[!UICONTROL Algorithmic]:* 지정한 최적화 목표에 따라 창의력을 알고리즘적으로 회전합니다.

         * **[!UICONTROL Optimization Goal]**&#x200B;에 대해 *[!UICONTROL Click Through Rate]*, (표준 비디오 광고 경험) *[!UICONTROL Completion Rate]* 또는 *[!UICONTROL Custom Objective]*&#x200B;을(를) 선택하십시오.  *[!UICONTROL Custom Objective]*&#x200B;을(를) 선택한 다음 기존 [Advertising DSP 사용자 지정 목표](/help/dsp/optimization/custom-goal.md)를 선택합니다.<!-- Verify -->

      * *[!UICONTROL Sequencing]:* 연결된 크리에이티브 번들을 지정된 순서로 회전합니다(첫 번째로 제공된 번들 1, 두 번째로 제공된 번들 2 등). 이때 각 번들 시퀀스에 대해 지정된 총 노출 횟수는 동일합니다. 제공되는 광고 크기는 사용 가능한 인벤토리에 의해 결정됩니다. a\) 무기한으로 표시되거나(기본값) b\) 다시 첫 번째 번들로 루프백되도록 시퀀스의 마지막 번들을 구성할 수 있습니다. 예를 들어, 3개의 (3) 노출에 대해 1번에서 모든 크리에이티브를 표시한 다음, 1개의 (1) 노출에 대해 2번에서 모든 크리에이티브를 표시한 다음, 2개의 (2) 노출에 대해 3번에서 모든 크리에이티브를 표시한 다음 루프를 다시 시작할 수 있습니다. 또는 번들 3의 크리에이티브가 표시되면 루프를 만드는 것이 아니라 계속 번들 3의 크리에이티브를 무한정 표시할 수 있습니다. 순번 지정 사용 시:

         1. 할당된 번들을 원하는 순서로 끌어다 놓습니다.

            할당된 번들은 기본적으로 경험에 추가된 순서대로 순서가 지정됩니다.

         1. 각 시퀀스에 대한 노출 횟수를 입력합니다.

         1. 마지막 시퀀스의 경우, a\) 시퀀스에 최종 번들을 무기한으로 표시할지(*[!UICONTROL Infinite]*(기본값) 또는 b\) 최종 번들이 표시된 후 첫 번째 번들로 다시 루프할지(*[!UICONTROL Keep in Loop]*) 변경합니다.

1. 각 추가 일정에 대해:

   1. **[!UICONTROL + Add Schedule]**&#x200B;을(를) 클릭합니다.

   1. 왼쪽 열에서 첫 번째 예약에 추가할 각 크리에이티브 옆의 확인란을 선택합니다.

   1. 일정의 시작 및 종료 날짜를 지정합니다.

   1. 크리에이티브 순환 유형을 선택합니다.

      * *[!UICONTROL Weighted]:* 상대 가중치에 따라 크리에이티브를 수동으로 회전합니다. 각 크리에이티브에 대한 가중치를 백분율로 입력합니다. 선택한 모든 크리에이티브에 대한 가중치는 최대 100개여야 합니다.

      * *[!UICONTROL Algorithmic]:* 지정한 최적화 목표에 따라 창의력을 알고리즘적으로 회전합니다.

         * **[!UICONTROL Optimization Goal]**&#x200B;에 대해 *[!UICONTROL Click Through Rate]* 또는 *[!UICONTROL Custom Objective]*&#x200B;을(를) 선택하십시오.  *[!UICONTROL Custom Objective]*&#x200B;을(를) 선택한 다음 기존 [Advertising DSP 사용자 지정 목표](/help/dsp/optimization/custom-goal.md)를 선택합니다.<!-- Verify -->

      * *[!UICONTROL Sequencing]:* 각 번들 시퀀스에 대해 지정된 총 노출 횟수로 연결된 Creative 번들을 지정된 순서로 회전합니다. 순번 지정 사용 시:

         1. 할당된 번들을 원하는 순서로 끌어다 놓습니다.

            할당된 번들은 기본적으로 경험에 추가된 순서대로 순서가 지정됩니다.

         1. 각 시퀀스에 대한 노출 횟수를 입력합니다.

         1. 마지막 시퀀스의 경우, a\) 시퀀스에 최종 번들을 무기한으로 표시할지(*[!UICONTROL Infinite]*(기본값) 또는 b\) 최종 번들이 표시된 후 첫 번째 번들로 다시 루프할지(*[!UICONTROL Keep in Loop]*) 변경합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [적용 가능한 광고 크기에 대한 광고 태그를 수동으로 만듭니다](/help/creative/experiences/experience-tag-create-manually.md)
>* [타깃팅이 없는 경험에 대한 광고 태그에 크리에이티브를 할당](experience-tag-assign-creatives.md)
>* [의사 결정 트리 타깃팅 없이 경험에 대한 추적 URL 사용자 지정](experience-tracking-urls-no-targeting.md)
