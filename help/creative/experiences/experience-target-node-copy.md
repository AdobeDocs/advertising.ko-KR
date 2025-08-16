---
title: 하위 노드를 동일한 수준의 다른 대상 노드에 복사
description: 상위 대상 노드의 모든 하위 노드를 동일한 수준의 다른 대상 노드로 복사하는 방법에 대해 알아봅니다
feature: Creative Experiences
exl-id: b3705689-57b6-41ce-9e00-2358bd195c93
source-git-commit: f7d5bf3193cb41ca2a0d4415998209e5a9b724ba
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# 하위 노드를 동일한 수준의 다른 대상 노드에 복사

*의사 결정 트리가 타겟팅된 경험*

상위 대상 노드의 모든 하위 노드(모든 하위 대상 및 해당 하위 노드에 할당된 크리에이티브 번들 포함)를 동일한 레벨의 다른 대상 노드에 복사할 수 있습니다. a) 복사한 노드를 기존 프레임워크에 추가하거나 b) 기존 프레임워크를 완전히 교체하여 노드를 복사할 수 있습니다. <!-- Give the main use case or an example to explain. -->

이 기능은 상위 노드에 대해 지정된 대상에는 영향을 주지 않으며 하위 노드에만 영향을 줍니다.

<!-- 1. [ways to get to the decision tree] -->

1. 복사하려는 하위 항목이 있는 상위 노드를 클릭하고 ![추가](/help/creative/assets/add.png "추가")를 클릭한 다음 a\) **[!UICONTROL Copy Children ctrl+c]**&#x200B;을(를) 선택하거나 b\) 키보드에 **[!UICONTROL Ctrl+C]**([!DNL Microsoft Windows]) 또는 **[!UICONTROL Command-C]**([!DNL Apple Macintosh])을(를) 입력하십시오.

1. 다음 중 하나를 수행합니다.

   * 노드에 대한 모든 자식 노드 및 크리에이티브를 바꾸려면 복사한 정보를 붙여넣을 노드를 클릭하고 **..**&#x200B;을(를) 클릭한 다음 a\) **[!UICONTROL Replace ctrl+shift+v]** 또는 b\)를 선택하고 키보드에 **[!UICONTROL Ctrl+Shift+V]**([!DNL Microsoft Windows]) 또는 **[!UICONTROL Command-Shift-V]**([!DNL Apple Macintosh])을(를) 입력합니다.

   * (여러 하위 대상이 있는 노드, &quot;모든&quot; 노드가 없고 크리에이티브만 없음) 노드에 모든 하위 노드 및 크리에이티브를 추가하려면 기존 하위 노드를 삭제하지 않고 복사한 정보를 붙여넣을 노드를 클릭하고 **..**&#x200B;을(를) 클릭한 다음 a\) **[!UICONTROL Add ctrl+v]** **&#x200B; 또는 b\)를 선택합니다. 키보드에 &#x200B;** [!UICONTROL Ctrl+V]&#x200B;**([!DNL Microsoft Windows]) 또는 &#x200B;** [!UICONTROL Command-V]**([!DNL Apple Macintosh])을(를) 입력합니다.

<!--
1. (Optional) To save the experience, click **[!UICONTROL Save]**, and then do the following.
...

These formatted steps are inserted automatically from text in the following file in the _includes folder, which reused in multiple places.
-->

{{$include /help/_includes/experience-save.md}}

>[!MORELIKETHIS]
>
>* [최종 수준에 대상 노드 추가](experience-target-node-add-final.md)
>* [노드 사이에 대상 노드 삽입](experience-target-node-add-inner.md)
>* [노드 사이에 형제 대상 노드 추가](experience-target-node-add-sibling.md)
>* [최종 노드에 광고 할당](experience-assign-creative-bundles.md)
>* [대상 노드 또는 크리에이티브 리프 노드 삭제](/help/creative/experiences/experience-target-node-delete.md)
>* [의사 결정 트리 타깃팅으로 경험 만들기](experience-create-targeting.md)
>* [의사 결정 트리 타깃팅으로 경험 편집](experience-edit-targeting.md)
>* [타깃팅된 경험 설정](experience-settings-targeting.md)
