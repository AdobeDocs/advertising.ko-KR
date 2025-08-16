---
title: 경험의 노드 사이에 타겟 노드 추가
description: 광고 경험에서 타겟 노드 사이에 타겟 노드를 추가하는 방법을 알아봅니다.
feature: Creative Experiences
exl-id: ac9211e5-c6ed-4185-bf9c-c2689f1b2775
source-git-commit: f7d5bf3193cb41ca2a0d4415998209e5a9b724ba
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 0%

---

# 경험의 노드 사이에 타겟 노드 추가

*의사 결정 트리가 타겟팅된 경험*

기존 레벨 사이에 대상 노드를 삽입하면 새 대상 노드는 기존의 모든 하위 대상 및 크리에이티브를 유지하고 새 노드를 처음에는 &quot;모두&quot;라고 합니다. 더 많은 특정 대상을 추가하지 않고 선택적으로 새 노드를 유지할 수 있습니다.

특정 대상을 정의하려면 동일한 수준에서 형제 대상 노드를 추가하고 새 대상을 지정한 다음 해당 대상에만 크리에이티브를 할당합니다. 동일 수준의 대상 노드를 추가하면 새 대상 노드가 만들어지고 이전에 &quot;모두&quot;에 할당되었던 모든 하위 대상 및 크리에이티브가 동일한 수준의 새 &quot;기타 모든 항목&quot; 노드로 이동합니다. 이렇게 하면 새 동위 멤버 노드에만 새 타기팅 정보가 포함되므로 새 대상을 추가해도 기존 하위 분기에는 영향을 주지 않습니다.

>[!NOTE]
>
>의사 결정 트리의 맨 아래 수준에 대상 노드를 추가하려면 &quot;[경험의 최종 수준에 대상 노드 추가](experience-target-node-add-final.md)&quot;를 참조하십시오.

<!-- 1. [ways to get to the decision tree] -->

1. 대상을 삽입할 노드 아래에서 ![추가](/help/creative/assets/add.png "추가")를 클릭한 다음 **[!UICONTROL Insert New Target]**&#x200B;을(를) 선택합니다.

1. 다음 중 하나를 수행합니다.

   * 동위 노드가 아직 없는 경우 다음을 수행합니다.

      1. 대상 유형을 선택한 다음 **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

         * 대상 대상에 대해 **[!UICONTROL Audience]**&#x200B;을(를) 선택합니다.

         * 지리적 대상의 경우 단일 지리적 범주(예: [!UICONTROL Geo: Country])를 선택하십시오.

         * 데이터 전달 대상의 경우 **[!UICONTROL Data Pass]**&#x200B;을(를) 선택합니다.

         * 픽셀 대상을 다시 타겟팅하려면 **[!UICONTROL RT Pixel]을(를) 선택합니다.

         * 장치 대상에 대해 단일 대상 범주(**[!UICONTROL Device: Type]**, **[!UICONTROL Device: OS]** 또는 **[!UICONTROL Device: Browser]**)를 선택하십시오.

   * 형제 노드가 이미 있는 경우 다음을 수행합니다.

      * 대상자 타겟의 경우 다음을 수행합니다.

         1. **[!UICONTROL Click to Browse]**&#x200B;을(를) 클릭하여 [!UICONTROL Audience Targeting] 옵션을 연 후 다음을 수행합니다.

            * 첫 번째 세그먼트를 추가하려면 왼쪽 패널에서 세그먼트를 찾은 다음 세그먼트 이름 옆에 있는 확인란을 선택합니다.

            * 기존 세그먼트 그룹에 세그먼트를 추가하려면 다음 작업을 수행하십시오.

               1. 오른쪽 패널에서 세그먼트 그룹을 클릭합니다.

               1. (선택 사항) 필요에 따라 그룹 논리를 *[!UICONTROL Include Any]*, *[!UICONTROL Include All]* 또는 *[!UICONTROL Exclude All]*(으)로 변경합니다.

                  *[!UICONTROL Exclude All]*&#x200B;은(는) 첫 번째 세그먼트 그룹에서 사용할 수 없습니다. 제외만 포함하는 대상의 경우 이 대상을 *[!UICONTROL Include Any]*(으)로 만든 다음 DSP 내의 배치에 추가할 때 해당 대상을 제외합니다.

               1. 왼쪽 패널에서 새 세그먼트를 찾은 다음 세그먼트 이름 옆에 있는 확인란을 선택합니다.

                  세그먼트 그룹이 새 세그먼트로 자동으로 업데이트됩니다.

            * 새 세그먼트 그룹을 추가하려면:

               1. 오른쪽 패널에서 **[!UICONTROL + New Group]**&#x200B;을(를) 클릭합니다.

               1. (선택 사항) 필요에 따라 이전 그룹과 새 그룹 간의 논리를 *[!UICONTROL And]* 또는 *[!UICONTROL Or]*(으)로 변경합니다.

               1. 왼쪽 패널에서 새 그룹의 세그먼트를 찾은 다음 세그먼트 이름 옆에 있는 확인란을 선택합니다.

               1. (선택 사항) 필요에 따라 그룹 논리를 *[!UICONTROL Include Any]*, *[!UICONTROL Include All]* 또는 *[!UICONTROL Exclude All]*(으)로 변경합니다.

         1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

         1. **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

      * 지리적 대상의 경우 다음을 수행합니다.

         1. **[!UICONTROL Click to Browse]**&#x200B;을(를) 클릭하여 [!UICONTROL Geo Targeting] 옵션을 열고 지리적 대상을 한 개 이상 지정한 다음 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

            우편 번호 대상에는 벌크 편집 옵션이 있습니다. 여러 우편번호를 붙여넣으려면 **[!UICONTROL Paste postal codes]** 탭을 클릭하고 국가를 선택하고 쉼표로 구분되거나 별도의 줄에 우편번호를 붙여 넣거나 입력한 다음 **[!UICONTROL Include All]**&#x200B;을(를) 클릭합니다. 포함된 우편번호 대상을 제거하려면 대상 위에 커서를 놓고 ![제거](/help/creative/assets/delete.png "제거") **[!UICONTROL Remove]**&#x200B;를 클릭합니다.

         1. (선택 사항) 지리적 대상을 여러 개 지정할 때 여러 대상 노드를 만들려면 **[!UICONTROL Split targets to create nodes]**&#x200B;을(를) 선택합니다.

            이 기능은 지정된 각 지리적 대상에 대해 별도의 대상 노드(별도의 크리에이티브 번들과 함께)를 만듭니다. 대상을 분할하지 않으면 사용자가 지정된 모든 위치([!DNL Boolean] `AND` 문)에 속해야 합니다.

         1. **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

      * 데이터 전달 대상의 경우 선택적으로 데이터 전달 키를 사용자 지정하고 단일 데이터 전달 값을 입력한 다음 **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

        키-값 쌍의 키에 대한 기본값이 **[!UICONTROL Data Pass]**&#x200B;경험 설정[!UICONTROL Advanced]의 [ 섹션에 있는 ](experience-settings-targeting.md) 필드에 이미 설정되어 있습니다. 선택적으로 키를 사용자 지정할 수 있습니다.

      * 재타겟팅 픽셀 타겟의 경우 사용할 단일 재타겟팅 픽셀과 크리에이티브를 표시하는 데 필요한 픽셀 특성 값을 선택한 다음 **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

        리타겟팅 픽셀에 대한 특성은 [리타겟팅 픽셀 설정](/help/creative/pixels/retargeting-pixel-manage.md)에 구성되어 있습니다.

      * 장치 대상의 경우 다음을 수행합니다.

         1. 대상을 선택합니다.

         1. (선택 사항) 지리적 대상을 여러 개 지정할 때 여러 대상 노드를 만들려면 **[!UICONTROL Split targets to create nodes]**&#x200B;을(를) 선택합니다.

            이 기능은 지정된 각 지리적 대상에 대해 별도의 대상 노드(별도의 크리에이티브 번들과 함께)를 만듭니다. 대상을 분할하지 않으면 사용자가 지정된 모든 위치([!DNL Boolean] `AND` 문)에 속해야 합니다.

         1. (선택 사항) 지리적 대상을 여러 개 지정할 때 여러 대상 노드를 만들려면 **[!UICONTROL Split targets to create nodes]**&#x200B;을(를) 선택합니다.

         1. **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 사용자 정의 분기의 사용자 지정 분기 이름을 지정합니다.

   기본적으로 사용자 정의 분기는 적용된 타겟으로 레이블이 지정됩니다.

   &quot;All&quot; 또는 &quot;Everyone Else&quot; 분기에 대한 사용자 지정 분기 이름을 만들 수 없습니다.

   1. 대상 노드 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Edit Name]**&#x200B;을(를) 클릭합니다.

   1. **[!UICONTROL Node Name]**&#x200B;을(를) 입력한 다음 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * (선택 사항) [새 대상 노드 및 &quot;기타 모든 항목&quot; 노드에 크리에이티브를 할당](experience-assign-creative-bundles.md)합니다.

   * (선택 사항) [지정한 대상 형식의 형제 대상 노드를 추가](experience-target-node-add-sibling.md)합니다.

   * (선택 사항) 경험을 저장하려면:

      1. **[!UICONTROL Save]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL OK]**&#x200B;을(를) 클릭합니다.

      1. (맨 아래 수준의 각 노드에 크리에이티브가 하나 이상 포함되지 않은 경우): 다음 중 하나를 수행합니다.

         * 필요한 모든 Creative 번들 없이 환경을 저장하려면 **[!UICONTROL Save as Draft]**&#x200B;을(를) 클릭합니다.

           초안 경험을 위한 광고 태그를 만들 수 없습니다.

         * 아직 Creative 번들이 할당되지 않은 각 대상에 기본 Creative를 할당하려면 **[!UICONTROL Assign Default Creatives]**&#x200B;을(를) 클릭합니다. 기본 크리에이티브가 할당된 업데이트된 트리를 검토한 후 **[!UICONTROL Save]** 및 **[!UICONTROL OK]**&#x200B;을(를) 클릭합니다.

         * 결정 트리 편집을 계속하려면 **[!UICONTROL Continue Edit]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [최종 수준에 대상 노드 추가](experience-target-node-add-final.md)
>* [노드 사이에 형제 대상 노드 추가](experience-target-node-add-sibling.md)
>* [하위 노드 및 크리에이티브를 같은 수준의 다른 노드에 복사](experience-target-node-copy.md)
>* [최종 노드에 광고 할당](experience-assign-creative-bundles.md)
>* [대상 노드 또는 크리에이티브 리프 노드 삭제](/help/creative/experiences/experience-target-node-delete.md)
>* [의사 결정 트리 타깃팅으로 경험 만들기](experience-create-targeting.md)
>* [의사 결정 트리 타깃팅으로 경험 편집](experience-edit-targeting.md)
>* [타깃팅된 경험 설정](experience-settings-targeting.md)
