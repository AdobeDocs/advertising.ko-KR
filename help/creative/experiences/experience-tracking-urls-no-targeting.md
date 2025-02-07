---
title: 타깃팅하지 않고 경험에 대한 추적 URL 사용자 지정
description: 의사 결정 트리 타깃팅 없이 경험에서 각 크리에이티브에 대한 추적 URL을 사용자 지정하는 방법을 알아봅니다.
feature: Creative Experiences
source-git-commit: fd925c641bef7953aea50813725252c3913757fa
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# 의사 결정 트리 타깃팅 없이 경험에 대한 추적 URL 사용자 지정

*베타가 닫힘*

의사 결정 트리 타깃팅이 없는 경험의 경우 [!UICONTROL Tag Manager] 내에서 광고 경험 태그에 사용되는 개별 크리에이티브에 대해 최대 5개의 사용자 지정 노출 추적 URL, 5개의 사용자 지정 클릭 추적 URL 및 1개의 사용자 지정 랜딩 페이지 URL을 만들 수 있습니다.

사용자 지정 URL은 광고 경험 태그에서 만들어진 광고에만 사용되며 [!UICONTROL Creative Libraries]의 기본 크리에이티브 설정에 저장되지 않습니다.

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Experiences]**&#x200B;을(를) 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * 카드 보기에서 경험 이름 옆의 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Tag Manager]**&#x200B;을(를) 클릭합니다.

   * 테이블 보기에서 행 위에 커서를 놓고 **[!UICONTROL More]**&#x200B;을 클릭한 다음 **[!UICONTROL Tag Manager]**&#x200B;을(를) 클릭합니다

1. (광고 크기에 대한 태그가 없는 경우) 적용 가능한 크리에이티브 크기에 대한 태그를 만듭니다.

   경험에 사용되는 각 크리에이티브 크기에 대해 하나 이상의 태그를 만들 수 있습니다.

   1. 오른쪽 상단에서 **[!UICONTROL Create Tag]**&#x200B;을(를) 클릭합니다.

   1. 고유한 **[!UICONTROL Tag name]**&#x200B;을(를) 입력하고 **[!UICONTROL Tag size]**&#x200B;을(를) 선택하십시오.

      사용 가능한 크기는 경험에 대한 기본 이미지 크리에이티브의 크기에 따라 결정됩니다.

   1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

1. 적용 가능한 광고 태그의 행 위에 커서를 놓고 ![추적 URL 편집](/help/creative/assets/edit-gray.png "추적 URL 편집") **[!UICONTROL Tracking URLs]**&#x200B;을(를) 클릭합니다. <!-- For targeted experiences, this is "EDIT Tracking URLs" -->&lt;!— 2/2부터 Tag Manager에는 목록 보기만 있고 카드 보기는 없습니다. >

   [!UICONTROL Click Tracking URLs], [!UICONTROL Impression Tracking URLs] 및 [!UICONTROL Landing URLs] 탭에는 할당된 번들에서 적용 가능한 크기의 모든 크리에이티브 이름이 나열됩니다. 적용 가능한 크기는 경험에 대한 기본 이미지 크리에이티브의 크기에 따라 결정됩니다.<!-- There's no distinct "Creative Sizes" setting. -->

1. **[!UICONTROL Click Tracking URLs]**, **[!UICONTROL Impression Tracking URLs]** 및 **[!UICONTROL Landing URLs]** 탭에서 필요에 따라 각 크리에이티브에 대해 다음을 수행합니다.

   1. 크리에이티브에 대한 행을 확장합니다.

   1. 다음 중 하나를 수행합니다.

      * 사용자 지정 URL을 추가하거나 편집하려면 입력 필드에 URL을 입력합니다.

      * 다른 사용자 지정 URL을 추가하려면 **[!UICONTROL +]**&#x200B;을(를) 클릭하고 입력 필드에 URL을 입력합니다.

      * 사용자 지정 URL을 제거하려면 Creative 행 위에 커서를 놓고 ![삭제](/help/creative/assets/delete.png "삭제")를 클릭합니다.

      최대 5개의 사용자 지정 노출 추적 URL, 5개의 사용자 지정 클릭 추적 URL 및 1개의 사용자 지정 랜딩 페이지 URL을 포함할 수 있습니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [타깃팅이 없는 경험에 대한 광고 태그에 크리에이티브를 할당](experience-tag-assign-creatives.md)
>* [의사 결정 트리 타깃팅을 사용하는 경험에 대한 추적 URL을 사용자 지정합니다](experience-tracking-urls-targeting.md)
