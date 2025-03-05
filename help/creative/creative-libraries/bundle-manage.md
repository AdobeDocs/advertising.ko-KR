---
title: Creative 번들 관리
description: xxxx에 대해 알아보십시오.
feature: Creative Bundles
exl-id: a9ed4e8f-db93-46d5-9231-2b3bb0aa072a
source-git-commit: 8d88a46e82a17ce5d2debf93ea0652f35a734d7a
workflow-type: tm+mt
source-wordcount: '1118'
ht-degree: 0%

---

# Creative 번들 관리

*베타가 닫힘*

<!--
**I'll probably split this up into multiple pages since the creative-related topics are separate**
-->

번들은 한 경험에 한 단위로 추가할 수 있는 광고 그룹입니다. 번들 컨테이너를 만든 후 크리에이티브를 번들에 첨부할 수 있습니다. 표준 번들에는 표준 광고만 포함될 수 있고, 동적 번들에는 동적 광고만 포함될 수 있습니다. 기본 크리에이티브에 영향을 주지 않고 경험 결정 트리 내에서 경험에 할당된 번들 내의 모든 크리에이티브에 대한 랜딩 페이지, 노출 추적 태그 및 클릭 추적 태그를 재정의할 수 있습니다.

[!DNL Creative]은(는) 번들이 할당된 각 경험에 대해 지정된 대로 번들의 크리에이티브를 순환합니다. 선택적으로 [!DNL Creative]이(가) Adobe Sensei에서 제공하는 알고리즘 광고 순환을 사용하여 성능을 기반으로 모든 경험에 대한 광고 요소를 최적화하도록 허용할 수 있습니다.

광고 경험에서 번들 간 광고 요소의 최적화를 활성화하기 위해 각 번들에는 각 \[creative size + language\] 조합 중 하나만 포함될 수 있습니다. 예를 들어 번들에 기본 언어가 &quot;프랑스어&quot;인 250x250 작성자가 하나 포함되어 있으면 기본 언어가 &quot;프랑스어&quot;인 두 번째 250x250 작성자를 추가할 수 없습니다. 동일한 언어에서 동일한 크기의 크리에이티브가 여러 개 있는 경우 경험에 개별적으로 추가하십시오.

번들에 첨부된 크리에이티브는 여전히 개별 크리에이티브로 사용할 수 있습니다. 단일 크리에이티브를 여러 번들에 추가할 수 있습니다. 번들에 첨부된 크리에이티브에 대한 설정을 편집하는 경우 변경 사항이 번들에 전파됩니다. 그러나 경험 내의 크리에이티브에 대해 구성된 모든 사용자 지정 랜딩 페이지, 노출 추적 태그 및 클릭 추적 태그는 항상 경험에 사용됩니다.

<!-- multiselect only to duplicate and delete -->

## Creative Library용 번들 만들기

크리에이티브를 여러 번들에 첨부할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

1. 라이브러리 이름을 클릭합니다.

1. **[!UICONTROL Bundles]** 탭을 클릭합니다.

1. 오른쪽 상단에서 **[!UICONTROL Create]** > **[!UICONTROL Bundles]** > **[!UICONTROL Bundle]**&#x200B;을(를) 클릭합니다.

1. 고유 **[!UICONTROL Bundle Name]** 및 **[!UICONTROL Bundle Type]:** *표준*(표준 크리에이티브) 또는 *동적*(동적 크리에이티브)을 입력하십시오.

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

## 번들에 광고 나열

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 특정 라이브러리를 포함하도록 [보기를 사용자 지정](/help/creative/introduction/customize-data-views.md)합니다.

1. 라이브러리 이름을 클릭합니다.

1. **[!UICONTROL Bundles]** 탭을 클릭합니다.

1. 번들 카드 또는 행을 클릭하여 번들의 모든 크리에이티브를 표시합니다.

## 번들 복제

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 특정 라이브러리를 포함하도록 [보기를 사용자 지정](/help/creative/introduction/customize-data-views.md)합니다.

1. 라이브러리 이름을 클릭합니다.

1. **[!UICONTROL Bundles]** 탭을 클릭합니다.

1. 복제할 번들 선택:

   * 단일 번들을 복제하려면:

      * 카드 보기에서 번들 이름 옆의 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Duplicate]**&#x200B;을(를) 클릭합니다.

      * 테이블 보기에서 행 위에 커서를 놓고 **[!UICONTROL Duplicate]**&#x200B;을(를) 클릭합니다.

   * 하나 이상의 번들을 복제하려면 복제할 각 번들에 대한 확인란을 선택합니다. 일괄 작업 도구 모음에서 **[!UICONTROL Duplicate].**&#x200B;을(를) 클릭합니다

     모든 행을 선택하려면 왼쪽 상단의 글로벌 확인란을 선택합니다.

   새 번들의 이름은 `<original name> (copy) # 1`(또는 시퀀스의 다음 번호)입니다. 예를 들어 &quot;테스트 번들&quot;을 두 개 복제하는 경우 중복 이름은 &quot;Test bundle (copy) # 1&quot;과 &quot;Test bundle (copy) # 2&quot;로 지정됩니다.

## 번들 이름 편집

번들 이름에 대한 변경 사항은 연결된 모든 경험에 전파됩니다.

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

1. 라이브러리 이름을 클릭합니다.

1. **[!UICONTROL Bundles]** 탭을 클릭합니다.

1. 번들을 선택합니다.

   * 카드 보기에서 라이브러리 이름 옆의 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

   * 테이블 보기에서 행 위에 커서를 놓고 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Bundle Name]** 편집

   [!UICONTROL Bundle Name]은(는) 고유해야 합니다.

1. **[!UICONTROL Update]**.<!-- inconsistent with "Edit" for creative libraries and creatives --> 클릭

## 번들에 크리에이티브 첨부

표준 번들에 [기존 표준 크리에이티브](/help/creative/creative-libraries/creative-libraries-about.md)을(를) 연결하고 동적 번들에 기존 동적 크리에이티브<!-- [existing dynamic creatives](creative-dynamic-manage.md) -->을(를) 연결할 수 있습니다. 번들에 크리에이티브를 첨부하면 번들이 할당된 모든 경험에서 크리에이티브를 사용할 수 있습니다. 각 번들에는 각 \[creative size + language\] 조합 중 하나만 포함될 수 있습니다.

<!--
>[!NOTE]
>
>You can also [attach creatives to bundles from the Standard Ads and Dynamic Ads views](creative-attach-detach-bundles.md).
-->

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 특정 라이브러리를 포함하도록 [보기를 사용자 지정](/help/creative/introduction/customize-data-views.md)합니다.

1. 라이브러리 이름을 클릭합니다.

1. **[!UICONTROL Bundles]** 탭을 클릭합니다.

1. 번들을 선택합니다.

   * 카드 보기에서 번들 이름 옆의 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Attach Creatives]**&#x200B;을(를) 클릭합니다.

   * 테이블 보기에서 행 위에 커서를 놓고 **[!UICONTROL Attach Creatives]**&#x200B;을(를) 클릭합니다.

   번들 유형에 적합한 각 크리에이티브가 오른쪽 프레임에 나열됩니다. 번들에 이미 첨부된 크리에이티브는 나열되지만 선택할 수 없습니다.

1. 오른쪽 프레임에서 번들에 첨부할 각 광고 옆에 있는 확인란을 선택한 다음 **[!UICONTROL Attach Creative to Bundle]**&#x200B;을(를) 클릭합니다.

## 번들에서 크리에이티브 분리 {#bundle-detach-creatives}

번들에서 크리에이티브를 분리하면 둘 간의 연관성이 제거되므로 더 이상 해당 크리에이티브가 번들을 타깃팅하는 경험에 사용되지 않습니다.

번들에서 크리에이티브를 분리해도 크리에이티브 라이브러리의 크리에이티브 탭에서는 크리에이티브가 삭제되지 않습니다.

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 특정 라이브러리를 포함하도록 [보기를 사용자 지정](/help/creative/introduction/customize-data-views.md)합니다.

1. 라이브러리 이름을 클릭합니다.

1. **[!UICONTROL Bundles]** 탭을 클릭합니다.

1. 번들 카드 또는 행을 클릭하여 번들의 모든 크리에이티브를 표시합니다.

1. 번들에서 분리할 크리에이티브 선택:

   * 단일 크리에이티브를 분리하려면 다음을 수행합니다.

      * 카드 보기에서 Creative 이름 옆의 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Detach]**&#x200B;을(를) 클릭합니다.

      * 테이블 보기에서 행 위에 커서를 놓고 **[!UICONTROL Detach]**&#x200B;을(를) 클릭합니다.

   * 하나 이상의 크리에이티브를 분리하려면 분리하려는 각 크리에이티브에 대한 확인란을 선택합니다. 일괄 작업 도구 모음에서 **[!UICONTROL Detach]**&#x200B;을(를) 클릭합니다.

     모든 행을 선택하려면 왼쪽 상단의 글로벌 확인란을 선택합니다.

## 번들에서 크리에이티브 미리 보기

시청자가 보게 될 대로 하이퍼링크를 사용하여 크리에이티브를 미리 볼 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 특정 라이브러리를 포함하도록 [보기를 사용자 지정](/help/creative/introduction/customize-data-views.md)합니다.

1. 라이브러리 이름을 클릭합니다.

1. **[!UICONTROL Bundles]** 탭을 클릭합니다.

1. 번들 카드 또는 행을 클릭하여 번들의 모든 크리에이티브를 표시합니다.

1. 크리에이티브 선택:

   * 카드 보기에서 Creative 이름 옆의 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Preview]**&#x200B;을(를) 클릭합니다.

   * 테이블 보기에서 행 위에 커서를 놓고 **[!UICONTROL Preview]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 화면 내에서 이미지 크기를 조정하려면 **[!UICONTROL Zoom]** 목록에서 이미지 크기의 10%에서 100%까지 옵션을 선택합니다.

<!-- Not there as of 1/22/24:  1. (Flexible HTML5 creatives; optional) To show all frames for the creative, select **Show frames**. -->

1. (선택 사항) 크리에이티브를 다운로드하려면 ![다운로드](/help/creative/assets/download.png "다운로드")를 클릭합니다.

   브라우저의 일반적인 절차에 따라 파일이 다운로드됩니다.


<!-- Not there as of 1/22/25:

## Edit the landing page and tracking tags for the creatives in a standard creative bundle

*Standard creative bundles only*

[Verify and edit all this, including the command names and where they're available. This is supposed to be a single and bulk action from within the right frame when you've open bundle details for a single bundle -- not from the Bundles table view.]

This procedure customizes the landing page, impression-tracking tags, and click-tracking tags for the creatives only within the context of the bundle. It doesn't change the settings for the base creative in [!UICONTROL Creative Libraries].

The custom URL and tags are applied to a creative when the bundle is assigned to an experience and the creative is served for the experience.

1. In the main menu, click **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**.

1. (Optional) [Customize the view](/help/creative/introduction/customize-data-views.md) to include specific libraries.

1. Click the library name.

1. Click the **[!UICONTROL Bundles]** tab.

1. Click the bundle name.

1. In the right pane, XXXXXXXXXXXX.

1. 

1. Edit any of the following settings: **[!UICONTROL Landing Page]**, **[!UICONTROL Click Tags]**, **[!UICONTROL Impression Tags]**.[Verify, and is can you do this for only one creative or is multiselect available?]

1.

 -->

## 번들 삭제

[live](/help/creative/experiences/experience-about.md#experience-statuses-experience-statuses) 경험에 할당되지 않은 번들을 삭제할 수 있습니다. 번들이 라이브 경험에 할당된 경우 계속하기 전에 경험에 대한 [결정 트리에서 번들을 제거](/help/creative/experiences/experience-target-node-delete.md)하십시오.

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 특정 라이브러리를 포함하도록 [보기를 사용자 지정](/help/creative/introduction/customize-data-views.md)합니다.

1. 라이브러리 이름을 클릭합니다.

1. **[!UICONTROL Bundles]** 탭을 클릭합니다.

1. 삭제할 번들을 선택하십시오.

   * 단일 번들을 삭제하려면

      * 카드 보기에서 번들 이름 옆의 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

      * 테이블 보기에서 행 위에 커서를 놓고 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

   * 하나 이상의 번들을 삭제하려면 삭제할 각 번들에 대한 확인란을 선택합니다. 일괄 작업 도구 모음에서 **[!UICONTROL Delete].**&#x200B;을(를) 클릭합니다

     모든 행을 선택하려면 왼쪽 상단의 글로벌 확인란을 선택합니다.

1. 확인 메시지에서 **[!UICONTROL Delete].**&#x200B;을(를) 클릭합니다

<!--
>* [Overview of implementing Adobe Advertising Creative](/help/creative/introduction/implementation-overview.md)
>* [How the user interface is organized](/help/creative/introduction/ui.md)
-->

>[!MORELIKETHIS]
>
>* [경험의 최종 노드에 Creative 번들 할당 및 할당 해제](/help/creative/experiences/experience-assign-creative-bundles.md)
>* [Creative 라이브러리에 표준 크리에이티브 추가](/help/creative/creative-libraries/creative-add-standard.md)
>* [Creative 라이브러리 관리](/help/creative/creative-libraries/creative-library-manage.md)
>* [크리에이티브 라이브러리 정보](/help/creative/creative-libraries/creative-libraries-about.md)
