---
title: 재사용 가능한 대상 편집
description: 재사용 가능한 대상을 편집하는 방법을 알아봅니다.
feature: DSP Audiences
exl-id: 4de6b9a4-2907-474d-92bf-83686a1f0b31
source-git-commit: 0afe1d9985c1451c28943aaa17c7d6f8a73a95ef
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# 재사용 가능한 대상 편집

배치나 기타 재사용 가능한 대상에 사용되는 대상을 편집하면 해당 배치 및 대상에 변경 사항이 즉시 적용됩니다.<!-- verify -->

>[!NOTE]
>
>(DSP에서 해시된 이메일 ID를 LiveRamp RampID 세그먼트로 변환하는 광고주) 활성, 예약됨 또는 일시 중지된 배치에 첨부되지 않은 자사 RampID 세그먼트는 일시 중지됩니다. 세그먼트는 세그먼트 목록에 &quot;자동 일시 중지됨&quot;으로 표시됩니다.

1. 메인 메뉴에서 **[!UICONTROL Audiences]** > **[!UICONTROL All audiences]**&#x200B;을(를) 클릭합니다.

1. 대상자 행 위에 커서를 놓고 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. 다음 방법 중 하나로 대상자 설정을 편집합니다.

   >[!NOTE]
   >
   >대상 세그먼트 논리를 편집하면 자세한 [대상 크기 데이터](audience-about.md)가 오른쪽 패널에서 업데이트됩니다.

   * (선택 사항) **[!UICONTROL Audience Name]**&#x200B;을(를) 편집하려면 대상 이름 옆에 있는 ![편집](/help/dsp/assets/edit.png)을(를) 클릭하고 고유한 대상 이름을 입력한 다음 **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

   * (선택 사항) [[!UICONTROL Third Party Segments], [!UICONTROL First Party Segments], [!UICONTROL Adobe Segments], [!UICONTROL Custom Segments] 및 [!UICONTROL Saved Audiences] 탭](audience-settings.md)에서 사용할 수 있는 세그먼트를 사용하여 세그먼트 논리를 수동으로 편집하려면 다음을 수행하십시오.

      * 기존 세그먼트 그룹에 세그먼트를 추가하려면 다음 작업을 수행하십시오.

      1. 오른쪽 패널에서 세그먼트 그룹을 클릭합니다.

      1. (선택 사항) 필요에 따라 그룹 논리를 *[!UICONTROL Include Any]*, *[!UICONTROL Include All]* 또는 *[!UICONTROL Exclude All]*(으)로 변경합니다.

         *[!UICONTROL Exclude All]*&#x200B;은(는) 첫 번째 세그먼트 그룹에서 사용할 수 없습니다. 제외만 포함하는 대상의 경우 이 대상을 *[!UICONTROL Include Any]*(으)로 만든 다음 배치 내에서 제외된 대상 메뉴에서 해당 대상을 선택합니다.

      1. 왼쪽 패널에서 새 세그먼트를 찾은 다음 세그먼트 이름 옆에 있는 확인란을 선택합니다.

         세그먼트 그룹이 새 세그먼트로 자동으로 업데이트됩니다.

   * 새 세그먼트 그룹을 추가하려면:

      1. 오른쪽 패널에서 **[!UICONTROL + New Group]**&#x200B;을(를) 클릭합니다.

      1. (선택 사항) 필요에 따라 이전 그룹과 새 그룹 간의 논리를 *[!UICONTROL And]* 또는 *[!UICONTROL Or]*(으)로 변경합니다.

      1. 왼쪽 패널에서 새 그룹의 세그먼트를 찾은 다음 세그먼트 이름 옆에 있는 확인란을 선택합니다.

      1. (선택 사항) 필요에 따라 그룹 논리를 *[!UICONTROL Include Any]*, *[!UICONTROL Include All]* 또는 *[!UICONTROL Exclude All]*(으)로 변경합니다.

   * 기존 대상의 세그먼트 논리를 사용하려면 다음을 수행합니다.

      1. 다음 방법 중 하나로 기존 대상에서 세그먼트 논리를 복사합니다.

         * 모든 대상 보기에서 대상 행 위에 커서를 놓고 **[!UICONTROL More]** > **[!UICONTROL Copy to Clipboard]**&#x200B;을(를) 클릭합니다.

         * 기존 대상에 대한 설정에서 세그먼트 논리 패널의 맨 위에서 **[!UICONTROL More]** > **[!UICONTROL Copy to Clipboard]**&#x200B;을(를) 클릭합니다.

         * 텍스트 편집기에서 영숫자 세그먼트 ID와 [부울 구문](audience-segment-logic-syntax.md)을 사용하여 세그먼트 논리를 수동으로 만든 다음 클립보드에 복사합니다.

      1. **[!UICONTROL paste in an audience rule to begin building]**&#x200B;을(를) 클릭하고 기존 세그먼트 논리를 입력 필드에 붙여 넣은 다음 **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

         >[!NOTE]
         >
         >대상에 이미 세그먼트 논리가 포함되어 있는 경우 새 세그먼트 논리에 붙여넣으면 기존 논리를 덮어씁니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Continue]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [대상자 관리 정보](audience-about.md)
>* [재사용 가능한 대상 만들기](reusable-audience-create.md)
>* [재사용 가능한 대상 복제](reusable-audience-duplicate.md)
>* [재사용 가능한 대상에 대한 세부 정보 보기](reusable-audience-view-details.md)
>* [재사용 가능한 대상 공유](reusable-audience-share.md)
>* [재사용 가능한 대상 내보내기](reusable-audience-export.md)
>* [재사용 가능한 대상의 세그먼트 키를 클립보드에 복사](reusable-audience-clipboard.md)
>* [재사용 가능한 대상 삭제](reusable-audience-delete.md)
>* [대상 설정](audience-settings.md)
>* [대상 세그먼트 논리에 대한 구문](audience-segment-logic-syntax.md)
>* [사용 가능한 타사 데이터 공급자](third-party-data-providers.md)
