---
title: 예약된 보고서 관리
description: 예약된 보고서를 관리하는 방법을 알아봅니다.
feature: Search Reports, Search Basic Reports, Search Advanced Reports, Search Assist Reports, Search Model Accuracy Reports, Search Specialty Reports
source-git-commit: bfca434eacf52ec7236804c54b7740442aa12961
workflow-type: tm+mt
source-wordcount: '1571'
ht-degree: 0%

---

# 예약된 보고서 관리

성능 보고서를 사용하면 포트폴리오, 광고 네트워크 및 광고 네트워크 계정 엔터티의 성능을 원하는 수준으로 추적하고 관리할 수 있습니다. 대부분의 보고서는 각 마케팅 채널의 광고가 전체 전환율에 어떻게 기여하는지에 대한 완전한 가시성을 제공합니다.

보고서의 데이터는 보고서를 실행할 때마다 동적으로 컴파일됩니다. 선택적으로 기존 보고서에서 새 보고서를 생성할 수 있습니다. 사용 가능한 보고서 매개 변수는 보고서 유형에 따라 다릅니다. 대부분의 보고서에서는 전체 보고서를 생성하는 대신 처음 50개 줄을 미리 볼 수 있는 옵션이 제공됩니다. 보고서를 생성할 때 보고서가 완료되면 하나 이상의 이메일 주소에 대한 다운로드 링크가 있는 알림을 보낼 수 있으며 받는 사람은 [[!UICONTROL Notification Center]](/help/search-social-commerce/notifications/notification-about.md)에서 알림을 관리할 수 있습니다.

완료된 보고서는 모두 [!UICONTROL Reports] 보기의 [!UICONTROL Latest Reports] 섹션에서 사용할 수 있으며 브라우저 창에서 표 형식으로 보거나 열거나 파일로 다운로드할 수 있습니다.

## 사용 가능한 보고서 카테고리

[!UICONTROL Reports] 보기에서 다음 보고서 범주를 사용할 수 있습니다. 모든 보고서에 대한 액세스 권한이 없을 수도 있습니다. 사용 가능한 보고서 및 보고서에서 생성하는 데이터는 사용자의 역할과 고객 계정이 구성되는 방식에 따라 결정됩니다.

| 보고서 범주 | 설명 |
| ----| ---- |
| [!UICONTROL Basic Reports] | 모든 사용자가 사용할 수 있는 [기본 보고서](/help/search-social-commerce/new-ui/reports/management/basic-advanced/basic-advanced-report-about.md)에는 포트폴리오, 광고 네트워크 계정, 특정 광고 네트워크 계정, 캠페인, 광고 그룹, 광고, 키워드, 제품 그룹, 레이블 분류 및 레이블 값, 입찰 단위 제한, 네트워크 제한에 대한 실제 비용과 클릭 데이터가 표시됩니다. 해당 광고 네트워크에서 청구한 클릭을 기반으로 하며 선택적으로 전환 데이터 또는 사용자가 만든 다른 지표를 포함할 수 있습니다. |
| [!UICONTROL Advanced Reports] | [고급 보고서](/help/search-social-commerce/new-ui/reports/management/basic-advanced/basic-advanced-report-about.md)는 광고 구성에 추가 insight을 제공하므로 지리적 타깃팅 또는 네트워크 설정을 변경하여 이점을 얻을 수 있는 위치를 파악할 수 있습니다. 또한 광고주의 내부 전환 추적 데이터에 대해 캠페인 및 포트폴리오 관리 보기와 보고서에서 전환 데이터의 유효성을 검사하는 데 도움이 될 수 있습니다. |
| [!UICONTROL Assist Reports] | [지원 보고서](/help/search-social-commerce/new-ui/reports/management/assist/assist-report-about.md)는 광고주의 모든 키워드 및 광고에 대한 전환 경로에 대한 통찰력을 제공합니다. Adobe Advertising 전환 추적 서비스를 통해 캡처한 데이터를 사용하며 해당 서비스를 사용하는 광고주에게만 생성될 수 있습니다. |
| [!UICONTROL Specialty Reports] | [특성 보고서](/help/search-social-commerce/new-ui/reports/management/specialty/specialty-report-about.md)는 Adobe Advertising 추적이 아니라 광고 네트워크에서 수집한 데이터로 구성됩니다. |
| [!UICONTROL Model Accuracy Reports] | [모델 정확도 보고서](/help/search-social-commerce/new-ui/reports/management/model-accuracy/model-accuracy-report-about.md)는 포트폴리오의 입찰, 캠페인 예산 및 입찰 전략 목표를 최적화하는 데 사용되는 비용 및 수익 모델의 정확도를 나타냅니다. |

## 보고서 자동화

다음 방법 중 하나 또는 둘 다로 사용자 지정된 보고서가 자동으로 생성되도록 예약합니다.

* [보고서 템플릿](/help/search-social-commerce/reports/automation/templates/template-about.md)을 사용하여 매일 또는 특정 요일 또는 달에 보고서를 자동으로 생성합니다.

  템플릿을 사용하는 [기본 및 고급 보고서의 FTP 배달](/help/search-social-commerce/new-ui/reports/ftp-reports.md)을 선택적으로 설정할 수 있습니다.

* [스프레드시트 피드](/help/search-social-commerce/new-ui/reports/spreadsheet-feeds-manage.md)를 사용하여 일일 성능 데이터로 사용자 지정된 스프레드시트 템플릿을 계속 새로 고칩니다.

## [!UICONTROL Scheduled Reports] 보기

[!UICONTROL Reports] > [!UICONTROL Scheduled Reports] 보기를 통해 보고서 및 보고서 템플릿을 만들고 관리할 수 있습니다.

* **[!UICONTROL Latest Reports]** 탭에는 수동으로 삭제된 보고서를 제외한 사용 가능한 모든 보고서가 나열되며, 기본적으로 가장 최근 보고서가 맨 위에 있습니다.<!-- Doesn't seem to be true: that were requested in the last seven days --> 각 보고서에 대해 표시되는 정보에는 보고서 실행 일정(해당되는 경우), 데이터가 생성되었거나 생성될 시작 및 종료 날짜, 보고서를 만든 사람, 보고서 상태(*[!UICONTROL Finished]*, *[!UICONTROL In Progress]* 또는 *[!UICONTROL Error]*)가 포함됩니다.

  각 보고서 옆에 있는 링크를 사용하면 보고서를 [!DNL Microsoft Excel] 통합 문서(XLS), 탭으로 구분된 값(TSV) 파일 또는 쉼표로 구분된 값(CSV) 파일로 열거나 저장할 수 있습니다. 일부 보고서 유형은 적용 가능한 각 캠페인에 대해 별도의 워크시트가 있는 [!UICONTROL Excel] 통합 문서로도 저장할 수 있습니다.

  이 탭에서는 새 보고서(선택적으로 템플릿으로 사용 가능)를 만들고, 기존 보고서의 설정을 기반으로 하거나 보고서 템플릿을 사용하여 새 보고서를 만들고, 진행 중인 보고서를 삭제하여 사용할 수 있으며, 완료된 보고서를 삭제할 수도 있습니다.

* **[!UICONTROL Templates]** 탭에는 연결된 일정에 대한 정보를 포함하여 저장된 모든 기본 및 고급 보고서 템플릿이 나열됩니다. 가장 최근 템플릿은 기본적으로 맨 위에 있습니다.

  이 탭에서 새 템플릿을 만들고, 만든 템플릿을 편집하고(일정 추가, 변경 또는 제거 포함), 템플릿에서 보고서를 생성하고, 사용 가능한 템플릿을 삭제합니다.

## 보고서 사용 방법

| 목적 | 보고서 |
| ---- | ---- |
| 성능 모니터링 | <ul><li>[[!UICONTROL Portfolio Report]](/help/search-social-commerce/new-ui/reports/management/basic-advanced/portfolio-report.md)</li><li>[[!UICONTROL Search Engine Report]](/help/search-social-commerce/new-ui/reports/management/basic-advanced/search-engine-report.md)</li><li>[[!UICONTROL Search Engine Account Report]](/help/search-social-commerce/new-ui/reports/management/basic-advanced/search-engine-account-report.md)</li><li>[[!UICONTROL Campaign Report]](/help/search-social-commerce/new-ui/reports/management/basic-advanced/campaign-report.md)</li><li>[[!UICONTROL Ad Group Report]](/help/search-social-commerce/new-ui/reports/management/basic-advanced/ad-group-report.md)</li><li>[[!UICONTROL Forecast Accuracy Report]](/help/search-social-commerce/new-ui/reports/management/model-accuracy/forecast-accuracy-report.md)</li></ul> |
| 성능 문제 해결 및 추세 분석 | <ul><li>[[!UICONTROL Keyword Report]](/help/search-social-commerce/new-ui/reports/management/basic-advanced/keyword-report.md)</li><li>[[!UICONTROL Ad Variation Report]](/help/search-social-commerce/new-ui/reports/management/basic-advanced/ad-variation-report.md)</li><li>[[!UICONTROL Transaction Report]](/help/search-social-commerce/new-ui/reports/management/basic-advanced/transaction-report.md)</li><li>[[!UICONTROL RSA Asset Report]](/help/search-social-commerce/new-ui/reports/management/specialty/rsa-asset-report.md)</li><li>[[!UICONTROL Keyword Daily Impression Share Report]](/help/search-social-commerce/new-ui/reports/management/specialty/keyword-daily-impression-share-report.md) 및 [[!UICONTROL Campaign Daily Impression Share Report]](/help/search-social-commerce/new-ui/reports/management/specialty/campaign-daily-impression-share-report.md)</li><li>&quot;[!UICONTROL Compare with]&quot; 기능을 사용하여 두 시간 창을 비교하는 모든 기본 보고서</li></ul> |
| 비즈니스 성장 기회 파악 | <ul><li>(Adobe Advertising 전환 추적 전용 광고주) [다음 [!UICONTROL Geo Distribution Report]](/help/search-social-commerce/new-ui/reports/management/basic-advanced/geo-distribution-report.md)</li><li>(Adobe Advertising 전환 추적 전용 광고주) [다음 [!UICONTROL Domain Referral Report]](/help/search-social-commerce/new-ui/reports/management/basic-advanced/domain-referral-report.md)</li><li>(광고주: [Adobe [!DNL Analytics for Advertising]](https://experienceleague.adobe.com/docs/advertising/integrations/analytics/overview.html?lang=ko)) Adobe Analytics Analysis Workspace 내에서 사용자 지정된 보고서</li></ul> |
| 분석 | <ul><li>(Adobe Advertising 전환 추적 전용 광고주) [다음 [!UICONTROL Channel Assist Report]](/help/search-social-commerce/new-ui/reports/management/assist/channel-assist-report.md)</li><li>(광고주: [Adobe [!DNL Analytics for Advertising]](https://experienceleague.adobe.com/docs/advertising/integrations/analytics/overview.html?lang=ko)) Adobe Analytics Analysis Workspace 내에서 사용자 지정된 보고서</li></ul> |

## 보고서 생성

### 새 보고서 생성

1. 메인 메뉴에서 **[!UICONTROL Reports]>[!UICONTROL Scheduled Reports]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Create Report]**&#x200B;을(를) 클릭하고 왼쪽 패널에서 보고서 범주를 클릭한 다음 보고서 유형을 선택합니다.<!-- Add link to list of report categories and report types --> **[!UICONTROL Proceed]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) [!UICONTROL Create Report] 창에서 [기본 및 고급 보고서](/help/search-social-commerce/new-ui/reports/management/basic-advanced/basic-advanced-report-settings.md), [지원 보고서](/help/search-social-commerce/new-ui/reports/management/assist/assist-report-settings.md), [모델 정확도 보고서](/help/search-social-commerce/new-ui/reports/management/model-accuracy/model-accuracy-report-settings.md) 및 [특성 보고서](/help/search-social-commerce/new-ui/reports/management/specialty/specialty-report-settings.md)에 대한 기본 보고서 설정을 변경합니다.

   1. (선택 사항) 보고서 및 템플릿에 대한 사용자 지정 이름을 입력합니다(보고서를 템플릿으로 저장하는 경우).

   1. (선택 사항) 보고서 설정을 템플릿으로 저장하려면 **[!UICONTROL Save as template]** 설정을 사용하도록 설정합니다.

   1. (선택 사항) 동일한 보고서 범주 내에서 다른 보고서 **[!UICONTROL Type]**&#x200B;을(를) 선택합니다.

   1. (선택 사항) **[!UICONTROL Basic Settings]** 탭에서 사용할 기존 보고서 템플릿을 선택하거나 보고서의 기본 기본 기본 설정을 변경합니다.

   1. (선택 사항) **[!UICONTROL Columns]** 탭을 클릭하고 열 순서를 포함하여 보고서의 기본 열을 변경합니다.

      기본적으로 보고서의 모든 통화 데이터는 미국 달러(예: 1,000.00) 형식으로 표시됩니다. 값을 올바른 통화 형식으로 표시하려면(CSV 및 TSV 형식의 통화 기호는 제외) &quot;[!UICONTROL Currency]&quot; 열을 보고서에 추가하십시오. 보고서에 통화가 다른 계정에 대한 데이터가 포함되어 있으면 통화에 관계없이 &quot;[!UICONTROL Total]&quot; 통화 값이 열에 있는 모든 숫자의 합계입니다.

   1. (일부 보고서 유형, 선택 사항) **[!UICONTROL Filters & Attribution]** 또는 **[!UICONTROL Filters]** 탭을 클릭하고 데이터 필터를 추가합니다. (일부 보고서 유형) 보고서 결과를 특정 레이블 분류만 포함하도록 제한하고 기본 속성 규칙 및 전환 속성 설정을 변경합니다.

   1. (선택 사항) **[!UICONTROL Scheduling]** 탭을 클릭하고 기본 예약 및 배달 옵션을 변경합니다.

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

보고서 일정을 지정하지 않은 경우 보고서가 즉시 실행됩니다. 그렇지 않으면 지정된 일정에 따라 실행됩니다. 보고서 이름이 [[!UICONTROL Latest Reports] 보기](/help/search-social-commerce/reports/report-about.md)에 추가됩니다. 보고서를 템플릿으로 저장하면 [[!UICONTROL Templates] 보기](/help/search-social-commerce/reports/report-about.md)에도 추가됩니다. 보고서가 완료되면 파일을 열거나 저장할 수 있습니다. 템플릿은 즉시 사용할 수 있습니다.

알림을 위해 이메일 주소를 입력한 경우, 보고서에 대한 사용자의 [구성된 알림 설정](/help/search-social-commerce/notifications/notification-edit.md)을 기반으로 보고서 작업이 완료되거나 실패하면 각 수신자는 알림을 받습니다.

### 기존 보고서에서 보고서 생성

1. 메인 메뉴에서 **[!UICONTROL Reports]>[!UICONTROL Scheduled Reports]**&#x200B;을(를) 클릭합니다. 그러면 **[!UICONTROL Latest Reports]** 탭이 열립니다.

1. 다음 중 하나를 수행합니다.

   * 커서를 보고서 행 위에 놓고 **..** > **[!UICONTROL Duplicate]**&#x200B;을(를) 클릭합니다.

   * 보고서 옆에 있는 확인란을 선택합니다. 일괄 작업 도구 모음에서 [복제](/help/search-social-commerce/assets/duplicate.png "복제")를 클릭합니다.

1. 필요한 경우 보고서 설정을 편집합니다.

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

### 기존 템플릿에서 보고서 생성

1. 메인 메뉴에서 **[!UICONTROL Reports]>[!UICONTROL Scheduled Reports]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Templates]** 탭을 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * 템플릿 행 위에 커서를 놓고 **..** > **[!UICONTROL Duplicate]**&#x200B;을(를) 클릭합니다.

   * 기존 템플릿 옆에 있는 확인란을 선택합니다. 일괄 작업 도구 모음에서 [복제](/help/search-social-commerce/assets/duplicate.png) **[!UICONTROL Duplicate]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 템플릿 이름을 변경하고 필요한 경우 보고서 설정을 편집합니다.

   설정 섹션 사이를 이동하려면 **[!UICONTROL Next]**&#x200B;을(를) 클릭하십시오.

1. **[!UICONTROL Save as Template]** 설정을 사용하도록 설정합니다.

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

## 보고서 미리 보기 또는 저장

웹 브라우저에서 보고서를 미리 보거나 보고서 데이터를 [!DNL Microsoft Excel] 통합 문서, 탭으로 구분된 값(TSV) 파일, 쉼표로 구분된 값(CSV) 파일 또는 [!DNL Microsoft Excel] 탭으로 표시된 통합 문서(일부 보고서 유형)로 열거나 저장할 수 있습니다.

>[!NOTE]
>
>Adobe 계정 팀원과 일부 관리자 사용자는 광고주와 에이전시 사용자가 만든 보고서를 볼 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Reports]>[!UICONTROL Scheduled Reports]**&#x200B;을(를) 클릭합니다. 그러면 **[!UICONTROL Latest Reports]** 탭이 열립니다.

1. 다음 중 하나를 수행합니다.

   * (웹 브라우저에서 보고서를 보려면) 다음 중 하나를 수행하십시오.

      * 템플릿 행 위에 커서를 놓고 **..** > **[!UICONTROL Preview]**&#x200B;을(를) 클릭합니다.

      * 기존 템플릿 옆에 있는 확인란을 선택합니다. 일괄 작업 도구 모음에서 **[!UICONTROL Preview]**&#x200B;을(를) 클릭합니다.

   * (보고서 데이터를 열거나 파일에 저장하려면) 보고서 이름 옆에 있는 [!UICONTROL Export] 열에서 형식 이름을 클릭한 다음 브라우저의 일반적인 절차에 따라 파일을 열거나 저장합니다.

      * **[!UICONTROL XLS]:** 단일 워크시트(XLSX 형식)가 있는 [!DNL Excel] 통합 문서의 경우. 이 보고서에는 매개 변수와 함께 맨 위에 레이블이 지정된 한 개의 워크시트가 포함되며, 구성 요소에 대한 데이터를 사용할 수 있을 때 각 구성 요소에 대해 하나의 행이 보고됩니다. 데이터가 없는 행은 생략됩니다.

        기본 보고서에는 각 숫자 열에 대한 합계가 포함됩니다.

      * TSV 파일용 **[!UICONTROL TSV]:**. 이 보고서에는 보고되는 각 구성 요소에 대한 매개 변수와 하나의 행이 포함됩니다.

      * CSV 파일용 **[!UICONTROL CSV]:**. 이 보고서에는 보고되는 각 구성 요소에 대한 매개 변수와 하나의 행이 포함됩니다.

## 보고서 삭제

1. 메인 메뉴에서 **[!UICONTROL Reports]>[!UICONTROL Scheduled Reports]**&#x200B;을(를) 클릭합니다. 그러면 **[!UICONTROL Latest Reports]** 탭이 열립니다.

1. 다음 중 하나를 수행합니다.

   * (단일 보고서를 삭제하려면):

      1. 커서를 보고서 행 위에 놓고 **..** > **[!UICONTROL Run]**&#x200B;을(를) 클릭합니다.

      1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

   * (하나 이상의 보고서를 삭제하려면 다음을 수행하십시오.)

      1. 삭제할 각 보고서 옆에 있는 확인란을 선택합니다.

      1. 일괄 작업 도구 모음에서 [삭제](/help/search-social-commerce/assets/delete-new.png "삭제") **[!UICONTROL Delete]**&#x200B;를 클릭합니다.

      1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

<!--

>[!MORELIKETHIS]
>
>* [About basic and advanced reports](/help/search-social-commerce/new-ui/reports/management/basic-advanced/basic-advanced-report-about.md)
>* [Basic and advanced report settings](/help/search-social-commerce/new-ui/reports/management/basic-advanced/basic-advanced-report-settings.md)
>* [Report columns for basic and advanced reports](/help/search-social-commerce/new-ui/reports/management/basic-advanced/basic-advanced-report-columns.md)

-->
