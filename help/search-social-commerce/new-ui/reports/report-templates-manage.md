---
title: (새 UI) 보고서 템플릿 관리
description: 예약 및 온디맨드 보고서에 대한 재사용 가능한 보고서 템플릿을 만들고, 보고, 편집하고, 삭제하는 방법을 알아봅니다.
feature: Search Reports
source-git-commit: bfca434eacf52ec7236804c54b7740442aa12961
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# (새 UI) 보고서 템플릿 관리

보고서 템플릿은 대부분의 보고서를 생성할 때 재사용할 수 있는 사전 정의된 보고서 레이아웃입니다. 템플릿을 사용하면 기본값이 아닌 매개 변수를 사용하거나 동일한 보고서의 변형을 실행하려는 경우 또는 정기적인 일정에 따라 동일한 보고서를 실행하려는 경우 시간을 절약할 수 있습니다. 저장된 보고서 템플릿은 보고서 페이지의 보고서 템플릿 섹션에서 사용할 수 있습니다.

한 번에 최대 100개의 템플릿을 유지 관리할 수 있습니다.

## 사용 가능한 작업

* [보고서 템플릿을 처음부터 만들거나 기존 템플릿을 기반으로 ](#template-create)합니다.

* [지정된 서식 파일에 대해 요청 시 보고서를 실행합니다](#template-run).

* [보고서 템플릿을 삭제](#template-delete)합니다.

## 보고서 템플릿 만들기 {#template-create}

<!-- Add xrefs to report procedures and settings once available -->

1. 메인 메뉴에서 **[!UICONTROL Reports]>[!UICONTROL Scheduled Reports]**&#x200B;을(를) 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * [!UICONTROL Latest Reports] 탭이나 [!UICONTROL Templates] 탭에서 템플릿을 처음부터 만들려면 보고서를 만들어 **[!UICONTROL Save as Template]** 설정을 사용하도록 설정하십시오.

   * 기존 템플릿을 기반으로 템플릿을 만들려면 다음 작업을 수행하십시오.

      1. **[!UICONTROL Templates]** 탭을 클릭합니다.

      1. 다음 중 하나를 수행합니다.

         * 템플릿 행 위에 커서를 놓고 **..** > **[!UICONTROL Duplicate]**&#x200B;을(를) 클릭합니다.

         * 기존 템플릿 옆에 있는 확인란을 선택합니다. 일괄 작업 도구 모음에서 [복제](/help/search-social-commerce/assets/duplicate.png)를 클릭합니다.

      1. (선택 사항) 템플릿 이름을 변경하고 필요한 경우 보고서 설정을 편집합니다.

         설정 섹션 사이를 이동하려면 **[!UICONTROL Next]**&#x200B;을(를) 클릭하십시오.

1. **[!UICONTROL Save as Template]** 설정을 사용하도록 설정합니다.

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

<!--

Not available to anyone as of 5/21. EDIT ALL IF WE ADD THIS FCT:

## Edit a report template {#template-edit}

You can change the settings for any report template you created. The new settings are applied to any reports using the template that are generated in the future.

1. In the main menu, click **[!UICONTROL Search, Social, & Commerce] > [!UICONTROL Insights & Reports] > [!UICONTROL Reports]**.

1. Click the **[!UICONTROL Templates]** tab.

1. Click the template name.

1. Change the report settings.

   >[!NOTE]
   >
   > When you edit the settings, you don't need to select the check box next to "[!UICONTROL Save as template]" in the [!UICONTROL Scheduling and Delivery] section. Doing so prompts you to create a new template with a different name.

1. Click **[!UICONTROL Update Template]**.

-->

<!--

Not available to anyone as of 5/21. EDIT ALL IF WE ADD THIS FCT:

## View a report template {#template-view}

>[!NOTE]
>
>Adobe account manager and administrator users can view templates created by client and agency roles.

1. In the main menu, click **[!UICONTROL Search, Social, & Commerce] > [!UICONTROL Insights & Reports] > [!UICONTROL Reports]**.

1. Click the **[!UICONTROL Templates]** tab.

1. Click the template name.

-->

## 지정된 템플릿에 대해 요청 시 보고서 실행 {#template-run}

언제든지 하나 이상의 템플릿에 대해 보고서를 실행할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Reports]>[!UICONTROL Scheduled Reports]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Templates]** 탭을 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * (단일 템플릿을 실행하려면):

      1. 템플릿 행 위에 커서를 놓고 **..** > **[!UICONTROL Run]**&#x200B;을(를) 클릭합니다.

      1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

   * (하나 이상의 템플릿을 실행하려면):

      1. 실행할 각 템플릿 옆의 확인란을 선택합니다.

      1. 일괄 작업 도구 모음에서 [실행](/help/search-social-commerce/assets/run-new.png "실행")을 클릭합니다.

      1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

## 보고서 템플릿 삭제 {#template-delete}

사용 가능한 보고서 템플릿을 삭제할 수 있습니다. 일정이 포함된 템플릿을 삭제하면 향후 해당 보고서가 생성되지 않습니다.

1. 메인 메뉴에서 **[!UICONTROL Reports]>[!UICONTROL Scheduled Reports]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Templates]** 탭을 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * 단일 템플릿을 삭제하려면 다음 작업을 수행하십시오.

      1. 템플릿 행 위에 커서를 놓고 **..** > **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

      1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

   * (하나 이상의 템플릿을 삭제하려면 다음을 수행하십시오.)

      1. 삭제할 각 템플릿 옆에 있는 확인란을 선택합니다.

      1. 일괄 작업 도구 모음에서 [삭제](/help/search-social-commerce/assets/delete-new.png)를 클릭합니다.

      1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.
