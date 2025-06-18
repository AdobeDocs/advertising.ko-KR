---
title: 경험 미리보기
description: 광고 경험에서 크리에이티브를 미리 보는 방법을 알아봅니다.
feature: Creative Experiences
exl-id: 2ac8f580-7d3d-4de6-ba14-5d72b30188d7
source-git-commit: ae226015d1a8a3da4ea2a0db0db31858e750b9a7
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

# 경험 미리보기

*베타가 닫힘*

모든 하이퍼링크를 포함하여 타겟 뷰어가 경험에 대해 보게 될 특정 광고 크기로 크리에이티브를 미리 볼 수 있습니다. 의사 결정 트리 타겟팅이 있는 경험의 경우 단일 크리에이티브, 특정 분기(타겟 유형)에 대한 크리에이티브 또는 경험의 모든 크리에이티브를 미리 볼 수 있습니다. 의사 결정 트리 타깃팅이 없는 경험의 경우 단일 크리에이티브를 미리 볼 수 있습니다. <!-- verify -->

* 경험 또는 특정 분기에 대한 모든 크리에이티브를 미리 보면 적용 가능한 모든 크리에이티브가 표시됩니다.

* 기준에 맞는 단일 크리에이티브 및 다중 크리에이티브를 미리 볼 때 미리 보기를 새로 고칠 때마다 보는 크리에이티브는 경험에 대한 광고 순환 설정을 기반으로 합니다.

   * 알고리즘 광고 회전의 경우 최적화 목표를 기반으로 크리에이티브가 선택됩니다.

   * 가중 광고 회전의 경우, 매번 지정된 가중치(예: Creative A가 표시될 80% 확률 및 Creative B가 표시될 20% 확률)를 기반으로 크리에이티브가 선택됩니다.

   * 예약된 광고 순환의 경우 예약의 첫 번째 크리에이티브가 표시됩니다. 시퀀스를 계속하려면 미리 보기를 계속 새로 고칠 수 있습니다.<!-- Refresh isn't there as of 2/3 -->

## 의사 결정 트리 타겟팅을 사용하는 경험에서 크리에이티브 미리 보기

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Experiences]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 특정 경험을 포함하도록 [보기를 사용자 지정](/help/creative/introduction/customize-data-views.md)합니다.

1. 다음 중 하나를 수행합니다.

   * 카드 보기에서 경험 이름 옆의 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Preview]**&#x200B;을(를) 클릭합니다.

   * 테이블 보기에서 행 위에 커서를 놓고 **[!UICONTROL More]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Preview]**&#x200B;을(를) 클릭합니다.

1. 미리 볼 광고 선택:

   * 단일 크리에이티브를 미리 보려면

      1. **[!UICONTROL Creative]**&#x200B;을(를) 클릭합니다.

      1. 광고 크기를 선택합니다.

      1. [!UICONTROL Decision Tree Targeting] 섹션에서 크리에이티브 대상을 선택합니다.

   * 특정 분기에 대한 크리에이티브를 미리 보려면 다음과 같이 하십시오.

      1. **[!UICONTROL Particular branch]**&#x200B;을(를) 클릭합니다.

      1. 광고 크기를 선택합니다.

     <!-- I don't see this as of 2/3:
     1. Select whether to group the creatives by Rotation Type or Ad Size.
     -->

      1. 크리에이티브 대상을 선택합니다.

   * 경험의 모든 크리에이티브를 미리 보려면 **[!UICONTROL Entire Tree]**&#x200B;을(를) 클릭합니다.

     <!-- I don't see this as of 2/3:
     1. Click **[!UICONTROL Entire Tree]**.
     1. Select the ad size.
     1. Select whether to group the creatives by Rotation Type or Ad Size.
     -->

1. (선택 사항) 크리에이티브 이름, 크리에이티브 유형 및 크기, 랜딩 페이지 URL 또는 클릭 URL, 각 크리에이티브 아래에 유연한 특성을 포함하려면 **[!UICONTROL Display Creative Metadata]**&#x200B;을(를) 선택합니다.

1. **[!UICONTROL Preview]**&#x200B;을(를) 클릭합니다.

1. (크리에이티브별 미리 보기 전용, 선택 사항) 도구 모음에서 **[!UICONTROL Refresh]**&#x200B;을(를) 클릭하여 광고 순환 설정에 따라 표시될 수 있는 추가 크리에이티브를 미리 봅니다.<!-- I don't see this as of 2/3 -->

1. (선택 사항) [!DNL Creative]에 로그인하지 않고 다른 사용자와 공유할 경험의 데모 URL을 복사하려면 다음을 수행하십시오.

   1. 미리 보기의 오른쪽 상단에서 ![공유](/help/creative/assets/share.png "공유")를 클릭합니다.

   1. [!UICONTROL Share Demo URL] 대화 상자에서 **[!UICONTROL Copy]**&#x200B;을(를) 클릭하여 URL을 클립보드에 복사하여 다른 사람과 공유할 수 있도록 합니다.

## 의사 결정 트리 타깃팅 없이 경험에서 크리에이티브 미리 보기

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Experiences]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 특정 경험을 포함하도록 [보기를 사용자 지정](/help/creative/introduction/customize-data-views.md)합니다.

1. 다음 중 하나를 수행합니다.

   * 카드 보기에서 경험 이름 옆의 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Preview]**&#x200B;을(를) 클릭합니다.

   * 테이블 보기에서 행 위에 커서를 놓고 **[!UICONTROL More]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Preview]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 특정 크리에이티브 크기를 선택하여 크리에이티브 목록을 제한합니다.

   기본적으로 모든 크기의 크리에이티브가 나열됩니다.

1. 광고 태그 이름을 클릭하여 행을 확장하고 크리에이티브를 미리 봅니다.

1. (선택 사항) 크리에이티브의 랜딩 페이지로 이동하려면 크리에이티브를 클릭합니다.

   <!-- Verify:  Will the creative click be tracked like a regular ad click but not linked to a publisher and placement? Explain effect/consequences. -->

1. (선택 사항) [!DNL Creative]에 로그인하지 않고 다른 사용자와 공유할 경험의 데모 URL을 복사하려면 다음을 수행하십시오.

   1. 미리 보기의 오른쪽 상단에서 ![공유](/help/creative/assets/share.png "공유")를 클릭합니다.

   1. [!UICONTROL Share Demo URL] 대화 상자에서 **[!UICONTROL Copy]**&#x200B;을(를) 클릭하여 URL을 클립보드에 복사하여 다른 사람과 공유할 수 있도록 합니다.

>[!MORELIKETHIS]
>
>* [의사 결정 트리 타깃팅으로 경험 만들기](experience-create-targeting.md)
>* [의사 결정 트리 타깃팅 없이 경험 만들기](/help/creative/experiences/experience-create-no-targeting.md)
