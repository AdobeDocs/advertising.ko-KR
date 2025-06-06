---
title: 경험의 노드 사이에 동일 수준의 타겟 노드 추가
description: 대상이 있거나 대상이 있는 노드와 동일한 수준에 있는 모든 노드에 형제 노드를 추가하는 방법을 알아봅니다.
feature: Creative Experiences
exl-id: 915fd399-1c55-49af-94ed-cf49a4154a53
source-git-commit: 05bcaa63779856cfea2f9cd3a0ab5d5e9d3d472a
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---

# 경험의 노드 사이에 동일 수준의 타겟 노드 추가

*의사 결정 트리가 타겟팅된 경험*
*Beta 완료*

대상이 있거나 대상이 있는 노드와 동일한 레벨에 있는 모든 노드에 동위 노드를 추가할 수 있습니다.

<!-- 1. Open the decision tree:


In a new experience


In an existing experience,
 -->

1. 형제 노드를 추가하려는 노드 위에서 ![추가](/help/creative/assets/add.png "추가")를 클릭한 다음 **[!UICONTROL Insert Sibling Target]**&#x200B;을(를) 선택합니다.

1. 대상을 지정합니다.

   * Adobe 대상 타겟의 경우 다음을 수행합니다.

      1. **[!UICONTROL Click to Browse]**&#x200B;을(를) 클릭하여 [!UICONTROL Audience Targeting] 옵션을 열고 **[!UICONTROL Adobe Segments]** 탭을 열고 광고주의 [!DNL Adobe] 대상 대상을 한 개 이상 지정한 다음 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

      1. (선택 사항) 여러 대상을 지정할 때 여러 대상 노드를 만들려면 **[!UICONTROL Split targets to create nodes]**&#x200B;을(를) 선택합니다.

         이 기능은 지정된 각 대상에 대해 별도의 대상 노드(별도의 크리에이티브 번들을 포함)를 만듭니다. 대상을 분할하지 않으면 사용자가 지정된 모든 대상([!DNL Boolean] `AND` 문)에 속해야 합니다.

      1. **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

   * 지리적 대상의 경우 다음을 수행합니다.

      1. **[!UICONTROL Click to Browse]**&#x200B;을(를) 클릭하여 [!UICONTROL Geo Targeting] 옵션을 열고 지리적 대상을 한 개 이상 지정한 다음 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

         우편 번호 대상에는 벌크 편집 옵션이 있습니다. 여러 우편번호를 붙여넣으려면 **[!UICONTROL Paste postal codes]** 탭을 클릭하고 국가를 선택하고 쉼표로 구분되거나 별도의 줄에 우편번호를 붙여 넣거나 입력한 다음 **[!UICONTROL Include All]**&#x200B;을(를) 클릭합니다. 포함된 우편번호 대상을 제거하려면 대상 위에 커서를 놓고 ![제거](/help/creative/assets/delete.png "제거") **[!UICONTROL Remove]**&#x200B;를 클릭합니다.

      1. (선택 사항) 지리적 대상을 여러 개 지정할 때 여러 대상 노드를 만들려면 **[!UICONTROL Split targets to create nodes]**&#x200B;을(를) 선택합니다.

         이 기능은 지정된 각 지리적 대상에 대해 별도의 대상 노드(별도의 크리에이티브 번들과 함께)를 만듭니다. 대상을 분할하지 않으면 사용자가 지정된 모든 위치([!DNL Boolean] `AND` 문)에 속해야 합니다.

      1. **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

   * 데이터 전달 대상의 경우 선택적으로 데이터 전달 키를 사용자 지정하고 단일 데이터 전달 값을 입력한 다음 **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

     키-값 쌍의 키에 대한 기본값이 [경험 설정](experience-settings-targeting.md)의 [!UICONTROL Advanced] 섹션에 있는 **[!UICONTROL Data Pass]** 필드에 이미 설정되어 있습니다. 선택적으로 키를 사용자 지정할 수 있습니다.

   * 픽셀 대상을 재타겟팅하려면 사용할 재타겟팅 픽셀과 크리에이티브를 표시하기 위해 존재해야 하는 픽셀 속성에 대한 필수 값을 선택합니다. **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

     리타겟팅 픽셀에 대한 특성은 [리타겟팅 픽셀 설정](/help/creative/pixels/retargeting-pixel-manage.md)에 구성되어 있습니다.

   * 장치 대상의 경우 다음을 수행합니다.

      1. 대상을 선택합니다.

      1. (선택 사항) 지리적 대상을 여러 개 지정할 때 여러 대상 노드를 만들려면 **[!UICONTROL Split targets to create nodes]**&#x200B;을(를) 선택합니다.

         이 기능은 지정된 각 지리적 대상에 대해 별도의 대상 노드(별도의 크리에이티브 번들과 함께)를 만듭니다. 대상을 분할하지 않으면 사용자가 지정된 모든 위치([!DNL Boolean] `AND` 문)에 속해야 합니다.

      1. **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * (선택 사항) [새 대상 노드에 크리에이티브를 할당](experience-assign-creative-bundles.md)합니다.

   * (선택 사항) 경험을 저장하려면:

      1. **[!UICONTROL Save]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL OK]**&#x200B;을(를) 클릭합니다.

      1. (맨 아래 수준의 각 노드에 크리에이티브가 하나 이상 포함되지 않은 경우): 다음 중 하나를 수행합니다.

         * 필요한 모든 Creative 번들 없이 경험을 저장하려면 **[!UICONTROL Save as Draft]**&#x200B;을(를) 클릭합니다.

           초안 경험을 위한 광고 태그를 만들 수 없습니다.

         * 아직 Creative 번들이 할당되지 않은 각 대상에 기본 Creative를 할당하려면 **[!UICONTROL Assign Default Creatives]**&#x200B;을(를) 클릭합니다. 기본 크리에이티브가 할당된 업데이트된 트리를 검토한 후 **[!UICONTROL Save]** 및 **[!UICONTROL OK]**&#x200B;을(를) 클릭합니다.

         * 결정 트리 편집을 계속하려면 **[!UICONTROL Continue Edit]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [최종 수준에 대상 노드 추가](experience-target-node-add-final.md)
>* [노드 사이에 대상 노드 삽입](experience-target-node-add-inner.md)
>* [하위 노드 및 크리에이티브를 같은 수준의 다른 노드에 복사](experience-target-node-copy.md)
>* [최종 노드에 광고 할당](experience-assign-creative-bundles.md)
>* [대상 노드 또는 크리에이티브 리프 노드 삭제](/help/creative/experiences/experience-target-node-delete.md)
>* [의사 결정 트리 타깃팅으로 경험 만들기](experience-create-targeting.md)
>* [의사 결정 트리 타깃팅으로 경험 편집](experience-edit-targeting.md)
>* [타깃팅된 경험 설정](experience-settings-targeting.md)
