---
title: 재사용 가능한 대상 만들기
description: 대상 세그먼트 및 기타 저장된 대상으로 구성된 재사용 가능한 대상을 만드는 방법을 알아봅니다.
feature: DSP Audiences
exl-id: 5f4a0abb-c285-4452-a6c3-a91d5281df9b
source-git-commit: e517dd5f5fa283ff8a2f57728612937148889732
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# 재사용 가능한 대상 만들기

<!-- "Saved audience" is used in UI (where?), but "saved" is a state, not a type. "Reusable audience" sounds better in a description. "Audience template" isn't right, either, since it implies you can edit it on the fly to create a new, different audience. Some other term? -->

대상 세그먼트 및 여러 배치에 대한 타겟 또는 제외로 사용할 수 있는 기타 저장된 대상의 그룹인 재사용 가능한 대상을 저장하고 관리할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Audiences]** > **[!UICONTROL All Audiences]**.

1. 데이터 테이블 위에서 **[!UICONTROL Create]**.

1. 고유 항목 입력 **[!UICONTROL Audience Name]**.

1. (선택 사항) 다음 옵션을 선택 취소합니다. **[!UICONTROL Share with all advertisers in my account]**.

   대상을 공유하면 해당 대상은 계정 내의 모든 광고주에게 타겟 또는 제외로 사용할 수 있습니다. 그러나 대상자의 개별 세그먼트는 세그먼트가 공유된 사용자만 사용할 수 있습니다. 예를 들어 동일한 대상에 매핑되지 않은 광고주와 Adobe Analytics 세그먼트가 포함된 대상을 공유하는 경우 [!DNL Analytics] 그러면 해당 광고주의 해당 대상에서 세그먼트가 미리보기되지 않습니다. 해당 광고주가 사용할 수 있는 세그먼트만 대상에서 미리 봅니다.

1. 클릭 **[!UICONTROL Save]**.

1. 대상자 작성:

   >[!NOTE]
   >
   >대상을 구축할 때 자세히 [대상 크기 데이터](audience-about.md) 오른쪽 패널에서 업데이트됨

   * 에서 사용할 수 있는 세그먼트를 사용하여 세그먼트 논리를 수동으로 만들려면 [[!UICONTROL Third Party Segments], [!UICONTROL First Party Segments], [!UICONTROL Adobe Segments], [!UICONTROL Custom Segments], 및 [!UICONTROL Saved Audiences] 탭](audience-settings.md)를 사용하여 다음을 수행합니다.

      * 첫 번째 세그먼트를 추가하려면 왼쪽 패널에서 세그먼트를 찾은 다음 세그먼트 이름 옆에 있는 확인란을 선택합니다.

      * 기존 세그먼트 그룹에 세그먼트를 추가하려면 다음 작업을 수행하십시오.

         1. 오른쪽 패널에서 세그먼트 그룹을 클릭합니다.

         1. (선택 사항) 그룹 논리를 다음으로 변경 *[!UICONTROL Include Any]*, *[!UICONTROL Include All]*, 또는 *[!UICONTROL Exclude All]*, 필요한 경우.

            *[!UICONTROL Exclude All]* 은(는) 첫 번째 세그먼트 그룹에서 사용할 수 없습니다. 제외만 포함하는 대상의 경우 다음과 같이 이 대상을 작성합니다. *[!UICONTROL Include Any]* 그런 다음 배치 내에서 제외된 대상 메뉴에서 해당 대상을 선택합니다.

         1. 왼쪽 패널에서 새 세그먼트를 찾은 다음 세그먼트 이름 옆에 있는 확인란을 선택합니다.

            세그먼트 그룹이 새 세그먼트로 자동으로 업데이트됩니다.

      * 새 세그먼트 그룹을 추가하려면:

         1. 클릭 **[!UICONTROL + New Group]** 오른쪽 패널에서

         1. (선택 사항) 이전 그룹과 새 그룹 간의 논리를 다음으로 변경 *[!UICONTROL And]* 또는 *[!UICONTROL Or]*, 필요한 경우.

         1. 왼쪽 패널에서 새 그룹의 세그먼트를 찾은 다음 세그먼트 이름 옆에 있는 확인란을 선택합니다.

         1. (선택 사항) 그룹 논리를 다음으로 변경 *[!UICONTROL Include Any]*, *[!UICONTROL Include All]*, 또는 *[!UICONTROL Exclude All]*, 필요한 경우.

   * 기존 대상의 세그먼트 논리를 사용하려면 다음을 수행합니다.

      1. 다음 방법 중 하나로 기존 대상에서 세그먼트 논리를 복사합니다.

         * 모든 대상 보기에서 대상 행 위에 커서를 놓고 을 클릭합니다 **[!UICONTROL More]** > **[!UICONTROL Copy to Clipboard]**.

         * 기존 대상에 대한 설정에서 세그먼트 논리 패널의 맨 위에 있는 **[!UICONTROL More]** > **[!UICONTROL Copy to Clipboard]**.

         * 텍스트 편집기에서 영숫자 세그먼트 ID 및 [부울 구문](audience-segment-logic-syntax.md)을 클릭하고 클립보드에 복사합니다.

      1. 클릭 **[!UICONTROL paste in an audience rule to begin building]**&#x200B;를 클릭하고 기존 세그먼트 논리를 입력 필드에 붙여 넣은 다음 을 클릭합니다 **[!UICONTROL Apply]**.

         >[!NOTE]
         >
         >대상에 이미 세그먼트 논리가 포함되어 있는 경우 새 세그먼트 논리에 붙여넣으면 기존 논리를 덮어씁니다.

1. 클릭 **[!UICONTROL Create]**.

>[!MORELIKETHIS]
>
>* [대상자 관리 기본 정보](audience-about.md)
>* [대상자 설정](audience-settings.md)
>* [대상 세그먼트 논리 구문](audience-segment-logic-syntax.md)
>* [사용 가능한 타사 데이터 공급자](third-party-data-providers.md)
>* [사용자 지정 세그먼트 만들기 및 구현](custom-segment-create.md)
>* [만들기 및 구현 [!UICONTROL CCPA Opt-Out-of-Sale] 세그먼트](ccpa-opt-out-segment-create.md)
>* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)
