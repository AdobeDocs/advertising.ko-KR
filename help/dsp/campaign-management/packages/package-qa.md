---
title: 일괄 시트를 사용하여 패키지 설정 검토 및 편집
description: 스프레드시트를 사용하여 주요 패키지 설정을 대량으로 검토하고 편집하는 방법에 대해 알아봅니다.
feature: DSP Packages
exl-id: bf52de27-db48-40e2-bb55-a2c27a1924ad
source-git-commit: fa4cee46135c85849daa7faa4059c77fc753c2c8
workflow-type: tm+mt
source-wordcount: '1184'
ht-degree: 0%

---

# 일괄 시트를 사용하여 패키지 설정 검토 및 편집

하나 이상의 패키지에 대한 설정을 검토를 위해 XLSX([!DNL Microsoft Excel] 스프레드시트) 형식으로 다운로드할 수 있습니다. 스프레드시트에는 비행 정보가 포함된 별도의 탭이 포함됩니다.

여러 설정을 한 번에 업데이트하려면 다음 중 하나를 수행할 수 있습니다.

* 필드를 선택하고, 파일을 저장하고, 편집된 일괄 시트 파일을 다시 DSP에 업로드하도록 변경합니다.

* 추가 패키지, 배치 또는 광고의 설정을 변경하려면 각 캠페인 구성 요소 유형에 대한 탭이 포함된 빈 일괄 시트 템플릿을 다운로드하고 새 설정이나 업데이트된 설정을 템플릿 파일에 입력하거나 붙여 넣은 다음 파일을 업로드하여 변경합니다. 지침은 &quot;[일괄 시트를 사용하여 캠페인 구성 요소 설정 검토 및 편집](/help/dsp/campaign-management/campaign-components-review-edit.md)&quot;을 참조하십시오.

편집 가능한 필드에는 일반적으로 편집할 수 있는 대부분의 설정이 포함됩니다.

>[!TIP]
>
>하나 이상의 패키지에 대해 더 많은 필드를 빠르게 편집하려면 &quot;[패키지 편집](/help/dsp/campaign-management/packages/package-edit.md)&quot;을 참조하세요.

## Campaign 있는 모든 패키지에 대한 다운로드 설정

캠페인의 모든 패키지에 대한 설정을 다운로드 할 때 스프레드 시트에는 패키지 설정 및 항공편 정보에 대한 별도의 탭이 포함됩니다. 패키지와 연결된 배치 및 광고에 대한 설정을 선택적으로 포함할 수 있습니다. 배치 및 광고 설정에 대한 추가 탭이 포함되어 있습니다.

1. 주 메뉴에서 을 클릭합니다 **[!UICONTROL Campaigns]**.

1. 캠페인 이름을 클릭합니다.

1. 오른쪽 상단에서 > **[!UICONTROL Download QA sheet]**&#x200B;을 클릭합니다 **[!UICONTROL ...]** .

1. [!UICONTROL QA Sheet Download] 대화 상자에서 다운로드한 파일에서 설정을 제외할 캠페인 구성 요소의 선택을 취소한 다음 **[!UICONTROL Download]**&#x200B;을(를) 클릭합니다.

기본적으로 패키지와 연결된 모든 배치 및 광고에 대한 설정이 선택됩니다.

알림 메시지는 파일을 다운로드할 수 있는 시기를 나타냅니다.

1. 파일을 다운로드하려면 다음 중 하나를 수행합니다.

   * 알림 메시지에서 을 클릭합니다 **[!UICONTROL Download].**

   * 상단 메뉴 표시줄의 오른쪽에서 작업을](/help/dsp/assets/downloads.png) 클릭합니다![. 작업 옆에 있는 **[!UICONTROL Download]**&#x200B;을(를) 클릭합니다.

     파일은 브라우저의 다운로드 폴더에 저장됩니다. 포함된 열의 목록은 &quot;[다운로드한/업로드한 스프레드시트의 배치 열](#qa-sheet-columns)&quot;을 참조하십시오.

>[!NOTE]
>
>캠페인 수준 QA 시트를 편집하고 다시 업로드할 수 없습니다. 이러한 파일의 캠페인 구성 요소 설정을 변경하려면 별도의 bulksheet 템플릿을 다운로드하고 QA 시트의 행을 bulksheet 템플릿에 입력하거나 붙여 넣은 다음 파일을 저장한 다음 채워진 bulksheet를 업로드하십시오. 지침은 &quot;[일괄 시트를 사용하여 캠페인 구성 요소 설정 검토 및 편집](/help/dsp/campaign-management/campaign-components-review-edit.md)&quot;을 참조하십시오.

## 하나 이상의 패키지에 대한 다운로드 설정

특정 패키지의 설정을 다운로드할 때 일괄 시트 파일에 패키지 설정 및 비행 정보에 대한 별도의 탭이 포함되어 있으며 파일을 편집할 수 있습니다.

1. 주 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 캠페인의 이름을 클릭합니다.

1. 하위 메뉴에서 **[!UICONTROL Packages]**&#x200B;을(를) 클릭합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL ...]** > **[!UICONTROL Download Bulksheet]**&#x200B;을(를) 클릭합니다.

   일괄 시트 파일을 다운로드할 수 있는 시기를 나타내는 알림 메시지가 표시됩니다.

1. 일괄 시트를 다운로드하려면 다음 중 하나를 수행하십시오.

   * 알림 메시지에서 **[!UICONTROL Download].**&#x200B;을(를) 클릭합니다

   * 상단 메뉴 모음 오른쪽에서 ![작업](/help/dsp/assets/downloads.png)을 클릭합니다. 작업 옆에 있는 **[!UICONTROL Download]**&#x200B;을(를) 클릭합니다.

     파일은 브라우저의 다운로드 폴더에 저장됩니다. 포함된 열의 목록은 &quot;[다운로드한/업로드한 스프레드시트의 배치 열](#qa-sheet-columns)&quot;을 참조하십시오.

<!-- I don't think I need this here

## Download a Bulksheet Template {#download-template}

You can optionally download a blank bulksheet template that includes tabs for each type of campaign component. You can later add rows to any tab on the template and [upload the edited file](##upload-bulksheet-package) to make changes. 

1. Click the name of the campaign.

1.  In the upper right, click **[!UICONTROL ...]** > **[!UICONTROL Download Bulksheet]**.

   The file is saved to the browser's Downloads folder. See "[Placement Columns in Downloaded/Uploaded Spreadsheets](#qa-sheet-columns)" for a list of the included columns.

-->

## 패키지 설정을 사용하여 일괄 시트 업로드 {#upload-bulksheet-package}

패키지와 연관된 배치 및 광고를 포함하여 패키지에 대한 설정을 일괄 시트 파일에 업로드할 수 있습니다.

1. 주 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 캠페인의 이름을 클릭합니다.

1. 오른쪽 상단에서 **[!UICONTROL ...]** > **[!UICONTROL Upload Bulksheet]**&#x200B;을(를) 클릭합니다.

1. [!UICONTROL Upload Bulksheet] 대화 상자에서:

   1. 파일을 상자로 끌어다 놓거나 상자 안을 클릭하여 장치나 네트워크에서 파일을 선택합니다.

   1. **[!UICONTROL Upload]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 업데이트가 처리되었는지 확인하려면 맨 위 메뉴 모음의 오른쪽에 있는 ![작업](/help/dsp/assets/downloads.png)을 클릭합니다.

## 다운로드/업로드된 스프레드시트의 패키지 설정 열{#qa-sheet-columns-packages}

>[!TIP]
>
> 다운로드한 스프레드시트에서 편집 가능한 모든 열이 파란색으로 강조 표시됩니다.

### [!UICONTROL Package] 탭

| 섹션 | 열 | 설명 | 편집 가능합니까? |
|---------|--------|-------------|-----------|
| [!UICONTROL Basic details] | [!UICONTROL Package ID] | 패키지의 숫자 ID입니다. | — |
| [!UICONTROL Basic details] | [!UICONTROL Package Name] | 패키지의 이름입니다. | 예 |
| [!UICONTROL Basic details] | [!UICONTROL Status] | 패키지 상태: *[!UICONTROL active]* 또는 *[!UICONTROL inactive]*. | 예 |
| [!UICONTROL Basic details] | [!UICONTROL Description] | 패키지에 대한 선택적 설명. | 예 |
| [!UICONTROL Basic details] | [!UICONTROL 3rd-party fees - CPM] | 1000회 노출당 청구 불가능한 비용으로 추적할 정적 타사 수수료 비율(해당하는 경우). | 예 |
| [!UICONTROL Basic details] | [!UICONTROL 3rd-party fees - description] | 서드파티 수수료율에 대한 선택적 설명(해당되는 경우). | 예 |
| [!UICONTROL Goals & Budget] | [!UICONTROL Package Start Date] | 패키지의 시작 날짜입니다. | 예 |
| [!UICONTROL Goals & Budget] | [!UICONTROL Package End Date] | 패키지의 종료 날짜입니다. | 예 |
| [!UICONTROL Goals & Budget] | [!UICONTROL Pacing Level] | 패키지에서 배치 간격 및 상한 수준: *[!UICONTROL Package]* 또는 *[!UICONTROL Placement]*. | — |
| [!UICONTROL Goals & Budget] | [!UICONTROL Budget] | 패키지 예산입니다. | 예 |
| [!UICONTROL Goals & Budget] | [!UICONTROL Budget Interval] | 예산 간격: &lt;i[!UICONTROL >Daily]*, *[!UICONTROL Weekly]*, *[!UICONTROL Monthly]*, 또는 *[!UICONTROL All Time]*. | 예 |
| [!UICONTROL Goals & Budget] | [!UICONTROL Interval Cap] | 선택적 예산 간격 한도입니다. | 예 |
| [!UICONTROL Goals & Budget] | [!UICONTROL Interval Cap Period] | 선택적 예산 간격 한도의 간격: &lt;i[!UICONTROL >Daily]*, *[!UICONTROL Weekly]*, *[!UICONTROL Monthly]* 또는 *[!UICONTROL All Time]*. | 예 |
| [!UICONTROL Goals & Budget] | [!UICONTROL Optimization Goal] | 패키지의 목적입니다. | 예 |
| [!UICONTROL Goals & Budget] | [!UICONTROL Optimization Target] | 목표의 타겟 값입니다. | 예 |
| [!UICONTROL Goals & Budget] | [!UICONTROL Custom Goal Name] | (최적화 목표가 &quot;[!UICONTROL Highest Return on Ad Spend]&quot; 및 &quot;[!UICONTROL Lowest Cost per Acquisition]&quot;인 패키지 전용)CPA 또는 ROAS 지표를 계산하는 데 사용되는 매출 또는 전환 이벤트가 포함된 [사용자 지정 목표](/help/dsp/optimization/custom-goal.md)입니다. | 예 |
| [!UICONTROL Goals & Budget] | [!UICONTROL Conversion Metric Name] | (선택 사항, &quot;[!UICONTROL Highest Return on Ad Spend]&quot; 및 &quot;[!UICONTROL Lowest Cost per Acquisition]&quot; 최적화 목표만 포함된 패키지) 광고 투자 수익률 또는 획득당 비용을 계산하는 데 사용할 최종 전환 이벤트 또는 매출 이벤트/매출 금액입니다. | 예 |
| [!UICONTROL Goals & Budget] | [!UICONTROL Package Goal Type] | (사용자 지정 최적화 목표가 있는 패키지만 해당) 패키지의 목적으로, 패키지를 최적화하는 방법을 결정하는 데 도움이 됩니다. *[!UICONTROL Prospecting]*, *[!UICONTROL Retargeting]* 또는 *[!UICONTROL Other]* . | 예 |
| [!UICONTROL Goals & Budget] | [!UICONTROL Linked Package id for learning carryover] | (사용자 지정 최적화 목표가 있는 패키지만 해당) 패키지 최적화를 위한 입력으로 내역 데이터가 사용되는 다른 패키지의 패키지 ID입니다. | 예 |
| [!UICONTROL Goals & Budget] | [!UICONTROL Linked Package Name for learning carryover] | (사용자 지정 최적화 목표가 있는 패키지만 해당) 패키지 최적화를 위한 입력으로 내역 데이터가 사용되는 다른 패키지. | — |
| [!UICONTROL Goals & Budget] | [!UICONTROL Pace on] | 패키지가 *[!UICONTROL budget]* 또는 *[!UICONTROL primary_goal]*(노출 횟수)을 향해 진행되는지 여부. | — |
| [!UICONTROL Goals & Budget] | [!UICONTROL Primary Goal Amount] | (노출 횟수에 따라 패키지 속도를 변경하는 경우) 지정된 시간 간격 동안의 타겟 노출 횟수입니다. | 예 |
| [!UICONTROL Goals & Budget] | [!UICONTROL Primary Goal Interval] | (노출 횟수에 따라 패키지 속도를 변경하는 경우) 타겟 노출 횟수에 대한 시간 간격입니다. | 예 |
| [!UICONTROL Goals & Budget] | [!UICONTROL Flight Pacing] | 패키지에 대한 플라이트 게재 간격 전략: *[!UICONTROL Even]*, *[!UICONTROL slightly ahead]*, *[!UICONTROL frontload]* 또는 *[!UICONTROL aggressive frontload]*. | 예 |
| [!UICONTROL Goals & Budget] | [!UICONTROL Intraday Pacing] | 패키지의 일일 게재 전략: *[!UICONTROL Even]* 또는 *[!UICONTROL ASAP]*. | 예 |
| [!UICONTROL Goals & Budget] | [!UICONTROL Frequency Cap] | 지정된 [!UICONTROL Frequency Cap Interval] 동안 패키지의 기본 빈도 상한입니다. | 예 |
| [!UICONTROL Goals & Budget] | [!UICONTROL Frequency Cap Interval] | 기본 빈도 제한 간격: *[!UICONTROL Day]*, *[!UICONTROL Week]* 또는 *[!UICONTROL Month]*. | 예 |
| [!UICONTROL Goals & Budget] | [!UICONTROL Frequency Cap Interval Value] | 기본 [!UICONTROL Frequency Cap]이(가) 적용되는 주, 일, 시간 또는 분 수입니다. 예를 들어 기본 상한이 한 달에 12회 노출이면 여기에 있는 값은 `12`입니다. | 예 |
| [!UICONTROL Goals & Budget] | [!UICONTROL Secondary Frequency Cap] | 지정된 [!UICONTROL Secondary Frequency Cap Interval] 동안 패키지의 보조 빈도 제한 | 예 |
| [!UICONTROL Goals & Budget] | [!UICONTROL Secondary Frequency Cap Interval] | 보조 빈도 제한 간격 유형: *[!UICONTROL Week]*, *[!UICONTROL Day]*, *[!UICONTROL Hour]* 또는 *[!UICONTROL Minute]*. 적용 가능한 주, 일, 시간 또는 분 수는 [!UICONTROL Secondary Frequency Cap Interval Value]에 표시됩니다. | 예 |
| [!UICONTROL Goals & Budget] | [!UICONTROL Secondary Frequency Cap Interval Value] | [!UICONTROL Secondary Frequency Cap]이(가) 적용되는 주, 일, 시간 또는 분 수입니다. 예를 들어 보조 캡이 6시간당 세 개의 노출 횟수이면 여기에 있는 값은 `6`입니다. | 예 |
| [!UICONTROL Custom Flights] | [!UICONTROL Activate Custom Flights] | 패키지의 비균등 간격 비행을 만들지 여부&#x200B;*T*(true) 또는 *F*(false). 사용자 정의 조명을 활성화하고 패키지를 저장하면 사용자 정의 조명을 비활성화하거나 패키지 시작 날짜를 편집할 수 없습니다. | — |
| [!UICONTROL Custom Flights] | [!UICONTROL Automatic Budget Rollover] | ([!UICONTROL Activate Custom Flighting] 옵션이 활성화된 경우에만 사용 가능) 다음 항공편의 기존 예산에 이전 항공편의 남은 예산을 자동으로 추가할지 여부: *T*(true) 또는 *F*(false). | 예 |
| [!UICONTROL Error] | [!UICONTROL Error] | 관련 오류. | — |

### [!UICONTROL Package_Flights] 탭 {#qa-sheet-columns-package-flights}

| 섹션 | 열 | 설명 | 편집 가능합니까? |
|---------|--------|-------------|-----------|
| [!UICONTROL Flight Details] | [!UICONTROL Package ID] | 패키지의 숫자 ID입니다. | — |
| [!UICONTROL Flight details] | [!UICONTROL Flight ID] | 항공편의 숫자 ID입니다. | — |
| [!UICONTROL Flight details] | [!UICONTROL Flight Start Date] | 플라이트의 첫 번째 날짜입니다. | 예 |
| [!UICONTROL Flight details] | [!UICONTROL Flight End Date] | 비행의 최종 날짜입니다. | 예 |
| [!UICONTROL Flight details] | [!UICONTROL Flight Budget] | 타겟이 비행에 대한 지출 목표입니다. | 예 |
| [!UICONTROL Flight details] | [!UICONTROL Rollover] | (&quot;[!UICONTROL Automatically rollover remaining flight budget to next flight]&quot; 옵션이 활성화되지 않은 기존 패키지) 다음 항공편에 추가할 지출되지 않을 수 있는 예산 금액입니다. | 예 |

>[!MORELIKETHIS]
>
>* [일괄 시트를 사용하여 Campaign 구성 요소 설정 검토 및 편집](/help/dsp/campaign-management/campaign-components-review-edit.md)
>* [패키지 편집](/help/dsp/campaign-management/packages/package-edit.md)
>* [패키지 설정](/help/dsp/campaign-management/packages/package-settings.md)
