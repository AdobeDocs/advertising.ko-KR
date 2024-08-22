---
title: 스프레드시트를 사용하여 패키지 설정 검토 및 편집
description: 스프레드시트를 사용하여 주요 패키지 설정을 검토하고 편집하는 방법에 대해 알아봅니다.
feature: DSP Packages
source-git-commit: ad00092c4ef5d44c364ab0593826220054f715c3
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 0%

---

# 스프레드시트를 사용하여 패키지 설정 검토 및 편집

하나 이상의 패키지에 대한 설정을 검토를 위해 XLSX([!DNL Microsoft Excel] 스프레드시트) 형식으로 다운로드할 수 있습니다. 스프레드시트에는 비행 정보가 포함된 별도의 탭이 포함됩니다. 그런 다음 두 탭에서 필드를 선택하도록 변경하고 데이터를 모두 한 번에 DSP에 다시 업로드할 수 있습니다. 편집 가능한 필드에는 일반적으로 편집할 수 있는 대부분의 설정이 포함됩니다.

>[!TIP]
>
>하나 이상의 패키지에 대해 더 많은 필드를 편집하려면 &quot;[패키지 편집](/help/dsp/campaign-management/packages/package-edit.md)&quot;을 참조하세요.

## 하나 이상의 패키지에 대한 다운로드 설정

1. 주 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 캠페인의 이름을 클릭합니다.

1. 하위 메뉴에서 **[!UICONTROL Packages]**&#x200B;을(를) 클릭합니다.

1. 설정을 다운로드할 각 패키지 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL ...]** > **[!UICONTROL Download Edit in Excel Sheet]**&#x200B;을(를) 클릭합니다.

파일은 브라우저의 다운로드 폴더에 자동으로 저장됩니다. 포함된 열의 목록은 &quot;[다운로드한/업로드한 스프레드시트의 패키지 열](#qa-sheet-columns-packages)&quot;을 참조하십시오.

## 하나 이상의 패키지에 대한 업로드 설정

1. 주 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 캠페인의 이름을 클릭합니다.

1. 하위 메뉴에서 **[!UICONTROL Packages]**&#x200B;을(를) 클릭합니다.

1. 설정을 업로드할 각 패키지 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL ...]** > **[!UICONTROL Upload Edit in Excel Sheet]**&#x200B;을(를) 클릭합니다.

1. [!UICONTROL Edit in Excel] 대화 상자에서:

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
| [!UICONTROL Goals & Budget] | [!UICONTROL Budget] | 패키지 예산. | 예 |
| [!UICONTROL Goals & Budget] | [!UICONTROL Budget Interval] | 예산 간격: &lt;i[!UICONTROL >Daily]*, *[!UICONTROL Weekly]*, *[!UICONTROL Monthly]* 또는 *[!UICONTROL All Time]*. | 예 |
| [!UICONTROL Goals & Budget] | [!UICONTROL Interval Cap] | 선택적 예산 간격 상한. | 예 |
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

### [!UICONTROL Package_Flights] 탭

| 섹션 | 열 | 설명 | 편집 가능합니까? |
|---------|--------|-------------|-----------|
| [!UICONTROL Flight Details] | [!UICONTROL Package ID] | 패키지의 숫자 ID입니다. | — |
| [!UICONTROL Flight details] | [!UICONTROL Flight ID] | 항공편의 숫자 ID입니다. | — |
| [!UICONTROL Flight details] | [!UICONTROL Flight Start Date] | 비행의 첫 번째 날짜. | 예 |
| [!UICONTROL Flight details] | [!UICONTROL Flight End Date] | 최종 비행 날짜. | 예 |
| [!UICONTROL Flight details] | [!UICONTROL Flight Budget] | 타겟이 비행에 대한 지출 목표입니다. | 예 |
| [!UICONTROL Flight details] | [!UICONTROL Rollover] | (&quot;[!UICONTROL Automatically rollover remaining flight budget to next flight]&quot; 옵션이 활성화되지 않은 기존 패키지) 다음 항공편에 추가할 지출되지 않을 수 있는 예산 금액입니다. | 예 |

>[!MORELIKETHIS]
>
>* [패키지 편집](/help/dsp/campaign-management/packages/package-edit.md)
>* [패키지 설정](/help/dsp/campaign-management/packages/package-settings.md)
