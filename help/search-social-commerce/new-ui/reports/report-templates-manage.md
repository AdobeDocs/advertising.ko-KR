---
title: (새 UI) 보고서 템플릿 관리
description: 예약 및 온디맨드 보고서에 대한 재사용 가능한 보고서 템플릿을 만들고, 보고, 편집하고, 삭제하는 방법을 알아봅니다.
feature: Search Reports
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: 9166e3e1-13c1-5edf-bc2a-c6e22231df68
    internal-label: Search Reports
source-git-commit: eb12699872b7c89240f5340cd3b0a251c9c08366
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 0%
---
# (새 UI) 보고서 템플릿 관리

보고서 템플릿은 대부분의 보고서를 생성할 때 재사용할 수 있는 사전 정의된 보고서 레이아웃입니다. 템플릿을 사용하면 기본값이 아닌 매개 변수를 사용하거나, 동일한 보고서의 변형을 실행하거나, 정기적인 일정에 따라 동일한 보고서를 실행하려는 경우 시간을 절약할 수 있습니다. 저장된 템플릿은 **[!UICONTROL Reports]>[!UICONTROL Reports]**&#x200B;의 **[!UICONTROL Templates]** 탭에서 사용할 수 있습니다.

한 번에 최대 100개의 템플릿을 유지 관리할 수 있습니다.

데이터를 보려면 [!UICONTROL View Scheduled Reports] 권한이 필요합니다. 행 데이터를 복사할 뿐 아니라 템플릿을 만들고, 복제하고, 편집하고, 실행하고, 삭제하려면 [!UICONTROL Edit Scheduled Reports] 권한이 필요합니다. 생성한 템플릿만 편집할 수 있습니다.

## 사용 가능한 작업

* [보고서 템플릿을 새 템플릿으로 만들거나](#template-create) 기존 템플릿을 기반으로 합니다.

* [원본을 변경하지 않고 보고서 서식 파일의 설정을 봅니다](#template-view).

* 일정을 포함하여 [보고서 템플릿을 편집](#template-edit)합니다.

* [지정된 서식 파일에 대해 요청 시 보고서를 실행합니다](#template-run).

* [보고서 템플릿을 삭제](#template-delete)합니다.

* [선택한 행의 모든 데이터를 클립보드에 복사](#copy-to-clipboard).

## 보고서 템플릿 만들기 {#template-create}

1. 메인 메뉴에서 **[!UICONTROL Reports]>[!UICONTROL Reports]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Templates]** 탭을 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * 새 템플릿을 만들려면 **[!UICONTROL Create Template]**&#x200B;을(를) 클릭합니다. **[!UICONTROL Create a New Template]** 패널에서 보고서 범주와 보고서 유형을 선택한 다음 **[!UICONTROL Proceed]**&#x200B;을(를) 클릭합니다.

   * 기존 템플릿을 기반으로 템플릿을 만들려면 템플릿 행 위에 커서를 놓고 ![템플릿 설정](/help/search-social-commerce/assets/settings-new.png "템플릿 설정") **[!UICONTROL Template Settings]** 또는 **[!UICONTROL ...]>[!UICONTROL Duplicate]**&#x200B;을(를) 클릭합니다.

1. 템플릿에 대해 고유한 **[!UICONTROL Report Name]**&#x200B;을(를) 입력하고 **[!UICONTROL Save as Template]**&#x200B;이(가) 활성화되어 있는지 확인하십시오.

   이 설정은 **[!UICONTROL Create Template]**(으)로 시작할 때 기본적으로 사용됩니다. 사용하지 않도록 설정하면 최종 작업이 **[!UICONTROL Run Report]**(으)로 변경되어 템플릿을 저장하는 대신 보고서가 생성됩니다.

1. [기본 및 고급 보고서](/help/search-social-commerce/new-ui/reports/management/basic-advanced/basic-advanced-report-settings.md), [지원 보고서](/help/search-social-commerce/new-ui/reports/management/assist/assist-report-settings.md), [모델 정확도 보고서](/help/search-social-commerce/new-ui/reports/management/model-accuracy/model-accuracy-report-settings.md) 또는 [전문 보고서](/help/search-social-commerce/new-ui/reports/management/specialty/specialty-report-settings.md)에 대한 보고서 설정을 구성하십시오.

   설정 섹션 사이를 이동하려면 **[!UICONTROL Next]**&#x200B;을(를) 클릭하십시오.

1. (선택 사항) 보고서를 자동으로 생성하려면 **[!UICONTROL Scheduling]**&#x200B;에서 **[!UICONTROL Frequency]** 및 게재 설정을 구성하십시오.

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

보고서 설정을 제출하기 전에 **[!UICONTROL Save as Template]**&#x200B;을(를) 활성화하여 [최신 보고서 탭에서 보고서를 생성](/help/search-social-commerce/new-ui/reports/management/report-manage.md)하는 동안 템플릿을 저장할 수도 있습니다.

## 보고서 템플릿의 설정 보기 {#template-view}

원본 템플릿을 변경하지 않고 설정을 검사하려면 복제본을 엽니다. 이를 위해서는 [!UICONTROL Edit Scheduled Reports] 권한이 필요합니다. 중복을 열어도 새 템플릿이 저장되지 않습니다.

1. 메인 메뉴에서 **[!UICONTROL Reports]>[!UICONTROL Reports]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Templates]** 탭을 클릭합니다.

1. 템플릿 행 위에 커서를 놓고 ![템플릿 설정](/help/search-social-commerce/assets/settings-new.png "템플릿 설정") **[!UICONTROL Template Settings]**&#x200B;을 클릭합니다.

1. 보고서 설정을 검토합니다.

1. 완료되면 **[!UICONTROL Cancel]**&#x200B;을(를) 클릭합니다. 설치를 취소하라는 메시지가 표시되면 **[!UICONTROL Discard]**&#x200B;을(를) 클릭합니다.

대신 복사본을 저장하려면 [템플릿 만들기 절차](#template-create)를 따르십시오.

## 보고서 템플릿 편집 {#template-edit}

만든 템플릿의 설정과 일정을 변경할 수 있습니다. 변경 사항은 나중에 템플릿에서 생성된 보고서에 적용됩니다.

1. 메인 메뉴에서 **[!UICONTROL Reports]>[!UICONTROL Reports]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Templates]** 탭을 클릭합니다.

1. 생성한 템플릿 옆에 있는 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

   여러 템플릿을 선택하거나 다른 사용자가 선택한 템플릿을 만든 경우에는 [!UICONTROL Edit]을(를) 사용할 수 없습니다.

1. 보고서 설정을 변경합니다. 일정을 추가, 변경 또는 제거하려면 **[!UICONTROL Scheduling]**&#x200B;에서 **[!UICONTROL Frequency]**&#x200B;을(를) 편집하세요.

   예약된 보고서의 일별, 주별 또는 월별 빈도를 선택합니다. 되풀이 일정을 제거하려면 **[!UICONTROL Now]**&#x200B;을(를) 선택하십시오.

   기존 템플릿을 편집할 때 **[!UICONTROL Save as Template]** 및 **[!UICONTROL Type]**&#x200B;은(는) 읽기 전용입니다. [!UICONTROL Save as Template]을(를) 다시 사용하도록 설정할 필요가 없습니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 지정된 템플릿에 대해 요청 시 보고서 실행 {#template-run}

언제든지 하나 이상의 템플릿에 대해 보고서를 실행할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Reports]>[!UICONTROL Reports]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Templates]** 탭을 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * (단일 템플릿을 실행하려면):

     1. 템플릿 행의 메뉴를 열고 **[!UICONTROL Run]**&#x200B;을(를) 선택합니다.

     1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

   * (하나 이상의 템플릿을 실행하려면):

     1. 실행할 각 템플릿 옆의 확인란을 선택합니다.

     1. 일괄 작업 도구 모음에서 **[!UICONTROL Run]**&#x200B;을(를) 클릭합니다.

     1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

템플릿을 편집하는 동안 **[!UICONTROL Run Report]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭하여 템플릿을 실행할 수도 있습니다. 먼저 변경 사항을 저장합니다. 이 작업은 저장된 템플릿을 실행합니다.

## 보고서 템플릿 삭제 {#template-delete}

사용 가능한 보고서 템플릿을 삭제할 수 있습니다. 일정이 포함된 템플릿을 삭제하면 향후 해당 보고서가 생성되지 않습니다.

1. 메인 메뉴에서 **[!UICONTROL Reports]>[!UICONTROL Reports]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Templates]** 탭을 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * 단일 템플릿을 삭제하려면 다음 작업을 수행하십시오.

     1. 템플릿 행의 메뉴를 열고 **[!UICONTROL Delete]**&#x200B;을(를) 선택합니다.

     1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

   * (하나 이상의 템플릿을 삭제하려면 다음을 수행하십시오.)

     1. 삭제할 각 템플릿 옆에 있는 확인란을 선택합니다.

     1. 일괄 작업 도구 모음에서 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

     1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

## 선택한 행의 모든 데이터를 클립보드에 복사 {#copy-to-clipboard}

보기에 표시되는 적용된 필터 및 열에 따라 선택한 행에 표시되는 정보를 복사합니다. 정보는 탭으로 구분된 값(TSV)으로 저장됩니다.

1. 데이터를 복사할 각 행 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Copy]**&#x200B;을(를) 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.
