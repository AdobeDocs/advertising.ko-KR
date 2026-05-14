---
title: 사용자 지정 시뮬레이션 실행 또는 재실행
description: 포트폴리오에 대한 사용자 지정 시뮬레이션을 실행하거나 다시 실행하는 방법을 알아봅니다.
feature: Search Optimization, Search Portfolios, Search Simulations
hide: true
exl-id: 0ee62d04-fdc4-445c-90fb-71d5a40a9ed0
TQID: https://experienceleague.adobe.com/DlSJEcKXOxVz6UXVpAjQqaiwDTakgJ4SS6rsQUxkQIE
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c2296997-5d79-4905-b32e-99b5aa892429
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
source-git-commit: 2504e6a4eebeab74352606a89a5012ab96c89c47
workflow-type: tm+mt
source-wordcount: 505
ht-degree: 0%

---

# 사용자 지정 시뮬레이션 실행 또는 재실행

*Beta 기능*

[최적화 또는 활성](/help/search-social-commerce/new-ui/manage/portfolios/portfolio-about.md) 포트폴리오에 대한 사용자 지정 시뮬레이션을 생성할 수 있습니다. 기존 시뮬레이션의 매개변수를 변경하고 시뮬레이션을 재생성하거나 기존 매개변수를 사용하여 기존 시뮬레이션을 재실행할 수도 있습니다.

<!-- You can't run sims for portfolios with legacy keyword-level optimization when they include smart bidding campaigns. Clarify all exceptions so users don't find out via error messages. -->

[!UICONTROL Admin] 및 [!UICONTROL Account Manager] 사용자는 다른 사용자가 만든 시뮬레이션을 볼 수 있습니다. 다른 모든 사용자는 자신이 만든 사용자 지정 시뮬레이션만 볼 수 있습니다.

## 새 시뮬레이션 만들기

1. 다음 중 하나를 수행합니다.

* [!UICONTROL Simulations] 보기에서:

   1. 메인 메뉴에서 **[!UICONTROL Plan]>[!UICONTROL Simulations]**&#x200B;을(를) 클릭합니다.

   1. 데이터 테이블 위에서 **[!UICONTROL Run Simulation]**&#x200B;을(를) 클릭합니다.

   1. 포트폴리오 선택:

      1. **[!UICONTROL Select Portfolio]**&#x200B;을(를) 클릭합니다.

      1. 포트폴리오를 선택합니다.

         특정 텍스트 문자열을 포함하는 포트폴리오를 검색하려면 검색 필드 내에 텍스트 문자열 입력을 시작합니다. 값은 대/소문자를 구분하지 않습니다.

      1. **[!UICONTROL Proceed]**&#x200B;을(를) 클릭합니다.

* [!UICONTROL Portfolios] 보기에서:

   1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Portfolios]**&#x200B;을(를) 클릭합니다.

   1. 포트폴리오 행 위에 커서를 놓습니다. 포트폴리오 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Run Simulation]**&#x200B;을(를) 클릭합니다.

1. [사용자 지정 시뮬레이션 설정 지정](#custom-simulation-settings):

   1. (선택 사항) 시뮬레이션에 사용되는 포트폴리오를 변경하려면 포트폴리오 이름 옆에 있는 **[!UICONTROL Change Portfolio]**&#x200B;을(를) 클릭하고 포트폴리오를 선택한 다음 **[!UICONTROL Proceed]**&#x200B;을(를) 클릭합니다.

   1. [!UICONTROL Basic Settings] 탭에서:

      1. 고유한 **[!UICONTROL Simulation Name]**&#x200B;을(를) 입력하십시오.

      1. (선택 사항) 시뮬레이션의 기본 매개 변수를 변경합니다.

   1. (선택 사항) [!UICONTROL Advanced Settings] 탭에서 시뮬레이션의 고급 매개 변수를 변경합니다.

   선택한 포트폴리오의 기존 매개 변수는 기본적으로 지정됩니다. 값을 변경하면 포트폴리오의 기존 매개 변수를 변경하지 않고 다른 매개 변수가 생성하는 결과가 표시됩니다.

1. **[!UICONTROL Next]**&#x200B;을(를) 클릭합니다.

1. 설정을 검토하고 필요에 따라 설정을 편집합니다.

1. **[!UICONTROL Submit & Run]**&#x200B;을(를) 클릭합니다.

시뮬레이션 보고서를 사용할 수 있으면 귀하와 지정된 다른 이메일 수신자는 하나의 통합 문서(XLSX 파일)가 포함된 ZIP 파일에서 데이터를 다운로드할 수 있는 링크가 포함된 알림을 받게 됩니다.

<!-- Still true:  When the results for any report type include more than 60,000 rows, the workbook includes multiple worksheets. -->

## 기존 시뮬레이션에 대한 설정을 편집하고 다시 실행하십시오.

1. 메인 메뉴에서 **[!UICONTROL Plan]>[!UICONTROL Simulations]**&#x200B;을(를) 클릭합니다.

1. 재생성할 시뮬레이션 옆에 있는 확인란을 선택합니다.

1. 데이터 테이블 위에서 **[!UICONTROL Run Simulation]**&#x200B;을(를) 클릭합니다.

1. [사용자 지정 시뮬레이션 설정 지정](#custom-simulation-settings):

   1. (선택 사항) 시뮬레이션에 사용되는 포트폴리오를 변경하려면 포트폴리오 이름 옆에 있는 **[!UICONTROL Change Portfolio]**&#x200B;을(를) 클릭하고 포트폴리오를 선택한 다음 **[!UICONTROL Proceed]**&#x200B;을(를) 클릭합니다.

   1. [!UICONTROL Basic Settings] 탭에서:

      1. 고유한 **[!UICONTROL Simulation Name]**&#x200B;을(를) 입력하십시오.

      1. (선택 사항) 시뮬레이션의 기본 매개 변수를 변경합니다.

   1. (선택 사항) [!UICONTROL Advanced Settings] 탭에서 시뮬레이션의 고급 매개 변수를 변경합니다.

   선택한 포트폴리오의 기존 매개 변수는 기본적으로 지정됩니다. 값을 변경하면 포트폴리오의 기존 매개 변수를 변경하지 않고 다른 매개 변수가 생성하는 결과가 표시됩니다.

1. **[!UICONTROL Next]**&#x200B;을(를) 클릭합니다.

1. 설정을 검토하고 필요에 따라 설정을 편집합니다.

1. **[!UICONTROL Submit & Run]**&#x200B;을(를) 클릭합니다.

시뮬레이션 보고서를 사용할 수 있으면 귀하와 지정된 다른 이메일 수신자는 하나의 통합 문서(XLSX 파일)가 포함된 ZIP 파일에서 데이터를 다운로드할 수 있는 링크가 포함된 알림을 받게 됩니다.

<!-- Still true:  When the results for any report type include more than 60,000 rows, the workbook includes multiple worksheets. -->

## 기존 설정으로 시뮬레이션 다시 실행

현재 큐에 있지 않은 시뮬레이션을 다시 실행할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Plan]>[!UICONTROL Simulations]**&#x200B;을(를) 클릭합니다.

1. 다시 실행할 시뮬레이션 옆의 확인란을 선택합니다.

1. 데이터 테이블 위의 도구 모음에서 ![다시 실행](/help/search-social-commerce/assets/rerun.png "다시 실행")을 클릭합니다.

## 사용자 정의 시뮬레이션 설정 {#custom-simulation-settings}

사용자 지정 시뮬레이션 설정에 대한 자세한 내용은 Search, Social 및 Commerce 내에서 사용할 수 있는 최적화 안내서를 참조하십시오.

>[!MORELIKETHIS]
>
>* [시뮬레이션 정보](simulation-about.md)
>* [시뮬레이션 세부 정보 보기](simulation-view.md)
>* [시뮬레이션 다운로드](simulation-download.md)
