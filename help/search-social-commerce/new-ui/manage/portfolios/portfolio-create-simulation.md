---
title: '[!UICONTROL Portfolios] 보기에서 시뮬레이션 실행 및 다운로드'
description: 포트폴리오 보기에서 사용자 정의 시뮬레이션을 실행하고 주간 시뮬레이션을 다운로드하는 방법을 알아봅니다.
feature: Search Optimization, Search Portfolios, Search Simulations
hide: true
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: ae57d55f-b168-5358-b114-c3974b1b3d77
    internal-label: Search Optimization
  - id: 893a7eac-45bd-56c2-a120-18db6d297dcc
    internal-label: Search Portfolios
  - id: 1d0fea65-a874-543d-94c9-b4dbf9e0360a
    internal-label: Search Simulations
source-git-commit: cb2d71e240af5ea1278cb2c00046d80040c914ce
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%
---
# [!UICONTROL Portfolios] 보기에서 시뮬레이션 실행 및 다운로드

*Beta 기능*

하나의 [최적화 또는 활성](portfolio-about.md#portfolio-status) 포트폴리오에 대해 사용자 지정 시뮬레이션을 실행하고 [!UICONTROL Portfolios] 보기에서 최대 100개의 포트폴리오에 대한 자동화된 주간 시뮬레이션을 다운로드할 수 있습니다.

사용자 지정 시뮬레이션을 실행하려면 [!UICONTROL Create Simulation] 권한이 필요합니다. 주간 시뮬레이션을 다운로드하려면 [!UICONTROL View Simulation] 권한이 필요합니다.

>[!NOTE]
>
>[!UICONTROL Simulations] 보기에서 [사용자 지정 시뮬레이션을 만들거나 다시 실행할 수도 있습니다](/help/search-social-commerce/new-ui/plan/simulations/simulation-create.md).

## 사용자 지정 시뮬레이션 실행 {#run-simulation}

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Portfolios]**&#x200B;을(를) 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * 포트폴리오 행 위에 커서를 놓습니다. 포트폴리오 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Run Simulation]**&#x200B;을(를) 클릭합니다.

   * 포트폴리오 옆에 있는 확인란을 선택합니다. 일괄 작업 도구 모음에서 **[!UICONTROL More]>[!UICONTROL Run Simulation]**&#x200B;을(를) 클릭합니다.

1. [사용자 지정 시뮬레이션 설정 지정](/help/search-social-commerce/new-ui/plan/simulations/simulation-create.md#custom-simulation-settings):

   1. **[!UICONTROL Basic Settings]** 탭에서 고유한 **[!UICONTROL Simulation Name]**&#x200B;을(를) 입력하고 필요에 따라 기본 매개 변수를 변경합니다.

   1. (선택 사항) **[!UICONTROL Advanced Settings]** 탭에서 고급 매개 변수를 변경합니다.

   선택한 포트폴리오의 현재 설정이 기본값으로 사용됩니다. 시뮬레이션 설정을 변경해도 포트폴리오의 설정은 변경되지 않습니다.

1. **[!UICONTROL Next]**&#x200B;을(를) 클릭합니다.

1. 설정을 검토하고 필요에 따라 변경합니다.

1. **[!UICONTROL Submit & Run]**&#x200B;을(를) 클릭합니다.

요청이 제출되고 [!UICONTROL Simulations] 보기가 열립니다. 시뮬레이션이 성공적으로 완료되면 [다운로드](/help/search-social-commerce/new-ui/plan/simulations/simulation-download.md)할 수 있습니다.

## 주간 시뮬레이션 다운로드 {#download-simulations}

한 번에 한 번의 실행 날짜에 대한 주간 시뮬레이션을 [!DNL Microsoft Excel] 통합 문서(XLSX 파일)로 다운로드할 수 있습니다. 해당 날짜에 사용 가능한 시뮬레이션 보고서가 있는 활성 및 최적화된 포트폴리오만 포함됩니다.

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Portfolios]**&#x200B;을(를) 클릭합니다.

1. 주간 시뮬레이션을 다운로드할 각 포트폴리오 옆에 있는 확인란을 선택합니다. 최대 100개의 포트폴리오를 선택할 수 있습니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL More]>[!UICONTROL Download Simulation]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Weekly Simulation]**&#x200B;에서 실행 날짜를 선택하십시오.

   기본적으로 가장 최근 사용 가능한 날짜가 선택됩니다. 선택한 일부 포트폴리오에 대해 보고서를 사용할 수 없는 경우 대화 상자에 제외되는 포트폴리오의 수가 표시됩니다. 필요한 경우 다른 날짜를 선택합니다. 선택한 포트폴리오에 해당 날짜에 사용 가능한 시뮬레이션이 없으면 보고서를 다운로드할 수 없습니다.

1. 사용 가능한 보고서가 있는 포트폴리오 수를 레이블에 포함하는 다운로드 단추를 클릭합니다(예: **[!UICONTROL Download 2 portfolios]**).

   브라우저의 일반적인 절차에 따라 파일이 다운로드됩니다. 완료 메시지는 포함된 포트폴리오 수를 나타냅니다.

사용자 지정 시뮬레이션을 다운로드하거나 개별 주간 시뮬레이션을 선택하려면 [[!UICONTROL Simulations] 보기](/help/search-social-commerce/new-ui/plan/simulations/simulation-download.md)를 사용하십시오.

>[!MORELIKETHIS]
>
>* [(새 UI) 포트폴리오 성능 세부 정보 보기](portfolio-details.md)
>* [포트폴리오 정보](portfolio-about.md)
>* [사용자 지정 시뮬레이션 실행 또는 다시 실행](/help/search-social-commerce/new-ui/plan/simulations/simulation-create.md)
>* [시뮬레이션 다운로드](/help/search-social-commerce/new-ui/plan/simulations/simulation-download.md)
