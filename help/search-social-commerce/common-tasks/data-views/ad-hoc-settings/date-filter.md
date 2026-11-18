---
title: 날짜 범위별로 데이터 필터링
description: 글로벌 날짜 범위 필터를 사용하는 방법을 알아봅니다.
exl-id: 35c0f63f-84ae-4e8e-8a48-acae7ff24498
feature: Search Common Tasks, Search Custom Data Views
TQID: 'https://experienceleague.adobe.com/1zB1NSise7wN1B68fUTq6ef824eiJx3zEglI0iUzwKQ'
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: bcc57258-3285-5d02-a731-d86f57a58c47
    internal-label: Search Common Tasks
  - id: d6e2ef48-fac7-5a4a-96ff-9ac0264dc826
    internal-label: Search Custom Data Views
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
source-git-commit: b5d2d666af6062eb3bf07ae041992819a4cc6780
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 0%
---
# 날짜 범위별로 데이터 필터링

날짜 범위 필터를 사용하여 성능 데이터를 표시할 기간을 지정합니다. 날짜 비교를 지원하는 보기에서 두 기간에 대한 성능을 비교할 수도 있습니다.

## (새 UI) 날짜 범위 변경 {#date-filter-new-ui}

1. 페이지 헤더에서 달력 아이콘을 사용하여 날짜 범위 컨트롤을 클릭합니다.

1. 날짜 범위 지정:

   * 사전 설정된 범위를 사용하려면 첫 번째 달력 위의 메뉴에서 옵션을 선택합니다(예: **[!UICONTROL Yesterday]** 또는 **[!UICONTROL Last 7 Days]**).

   * 사용자 지정 범위를 사용하려면 **[!UICONTROL Custom Date Range]**&#x200B;을(를) 선택하고 달력에서 시작 날짜와 종료 날짜를 선택하십시오. 달력 화살표를 사용하여 월 사이를 탐색합니다.

1. **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

## (새 UI) 두 기간의 데이터 비교 {#compare-periods-new-ui}

*날짜 비교만 지원하는 보기*

1. 페이지 헤더에서 달력 아이콘을 사용하여 날짜 범위 컨트롤을 클릭합니다.

1. **[!UICONTROL Compare Periods]**&#x200B;을(를) 켭니다.

   두 개의 달력 패널이 나란히 표시됩니다. 제1 기간은 청록색 표지를 갖고, 비교기간은 자주색 표지를 갖는다.

1. 첫 번째 패널에서 날짜 범위를 지정합니다.

   * 사전 설정된 범위를 사용하려면 첫 번째 달력 위의 메뉴에서 옵션을 선택합니다(예: **[!UICONTROL Yesterday]** 또는 **[!UICONTROL Last 7 Days]**).

   * 사용자 지정 범위를 사용하려면 **[!UICONTROL Custom Date Range]**&#x200B;을(를) 선택하고 달력에서 시작 날짜와 종료 날짜를 선택하십시오. 달력 화살표를 사용하여 월 사이를 탐색합니다.

1. 두 번째 패널에서 비교 사전 설정을 선택하거나 달력에서 시작 날짜를 클릭합니다.

   비교 기간은 첫 번째 기간과 일 수가 동일합니다. 두 캘린더 위의 전체 날짜 범위를 검토하십시오.

1. **[!UICONTROL Comparison Format]**&#x200B;에서 차이점을 표시하는 방법을 선택하십시오.

   * **[!UICONTROL As percentage]:** 차이를 백분율로 표시합니다.

   * **[!UICONTROL As variance]:** 차이를 숫자 값으로 표시합니다.

1. **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

   날짜 범위 컨트롤은 기간 레이블과 색상 마커가 있는 전체 날짜 범위를 모두 표시합니다. 비교 가능한 각 지표는 두 개의 기간 열과 **[!UICONTROL Change]** 열로 그룹화됩니다. 비교할 수 없는 필드는 단일 열로 유지됩니다. 열 머리글의 기간 마커는 해당 날짜 범위를 식별합니다.

기간 비교를 중지하려면 날짜 범위 컨트롤을 열고 **[!UICONTROL Compare Periods]**&#x200B;을(를) 끄고 **[!UICONTROL Apply]**&#x200B;을(를) 클릭하십시오. 비교를 해제하면 비교 데이터를 기반으로 필터가 지워집니다.

### 열 메뉴에서 비교 형식 변경

1. 날짜 비교가 활성화된 상태에서 **[!UICONTROL Change]** 열에 대한 열 머리글 메뉴를 열거나 비교 가능한 지표에 대한 기간 열을 엽니다.

1. **[!UICONTROL As percentage]** 또는 **[!UICONTROL As variance]**&#x200B;을(를) 선택하십시오.

   이 선택 사항은 선택한 열뿐만 아니라 그리드의 모든 비교 지표에 적용됩니다. 날짜 범위 컨트롤은 선택 항목과 동기화되며, 저장된 날짜 범위가 있는 보기를 포함하여 현재 광고주의 적용 가능한 페이지에서 형식이 공유됩니다.

   그리드가 성공적으로 새로 고침되면 확인 메시지가 나타납니다. 선택한 형식으로 그리드를 새로 고칠 수 없는 경우 대신 오류 메시지가 나타납니다. 형식을 다시 선택하십시오.

정렬 및 필터링 옵션은 지원되는 경우 열 메뉴에서 계속 사용할 수 있습니다.

## (기존 UI) 날짜 범위 설정

특정 날짜 범위를 저장한 기본 및 사용자 지정 보기를 제외하고 모든 광고주에 걸쳐 있는 대부분의 데이터 보기에 동일한 전역 날짜 범위 필터가 적용됩니다. 캠페인 관리 보기에 대한 시스템 기본 날짜 범위는 &quot;어제&quot;입니다.

날짜 범위 설정은 브라우저별 쿠키에 저장되므로, 필터를 변경하거나 쿠키를 삭제할 때까지 동일한 브라우저 애플리케이션을 사용하여 로그인할 때마다 날짜 범위 필터에 대한 모든 변경 사항이 모든 광고주에 대해 사용됩니다. 사용하는 각 브라우저 애플리케이션은 날짜 범위 필터 설정을 다른 쿠키에 저장합니다.

기본 보기 또는 사용자 지정 보기에 대해 특정 날짜 범위를 저장하면 사용 중인 브라우저 응용 프로그램에 관계없이 보기를 적용할 때마다 해당 범위가 적용됩니다.

>[!NOTE]
>
>* 이전 13개월의 데이터를 볼 수 있지만 기존의 모든 사용자 지정 보기에는 이전 180일까지의 데이터만 포함할 수 있습니다.
>* 이전 데이터를 보려면 [[!UICONTROL Reports] 보기](/help/search-social-commerce/reports/management/basic-advanced/basic-advanced-report-about.md)(으)로 이동하여 기본 보고서를 실행하십시오.
>* [기본 보기 또는 사용자 지정 보기](/help/search-social-commerce/common-tasks/data-views/custom-default-views-manage.md)에 대한 날짜 범위를 저장할 수도 있습니다.

## (기존 UI) 캠페인 보기에서 전역 날짜 필터를 변경합니다

1. 검색 \> 캠페인 \> 캠페인의 데이터 테이블 위에서 현재 날짜 범위를 클릭합니다.

1. **[!UICONTROL Date Range]** 필드에서 범위를 지정합니다.

   * 사전 설정된 범위의 경우: *[!UICONTROL Today]*&#x200B;에서 *[!UICONTROL Last 180 Days]* 사이의 공통 시간 증분 목록에서 선택합니다. 기본값은 *[!UICONTROL Yesterday]*&#x200B;입니다.

   * 특정 범위의 경우: **[!UICONTROL Custom Date Range]** 을(를) 선택한 다음 시작 날짜와 종료 날짜를 지정합니다.

     날짜를 MM/DD/YYYY 또는 MM-DD-YYYY 형식으로 입력하거나 각 필드 옆에 있는 ![달력 아이콘](/help/search-social-commerce/assets/calendar.png "달력 아이콘")을 클릭하여 달력을 열고 날짜를 선택합니다.

1. (선택 사항) 지정된 날짜 범위의 데이터를 두 번째 날짜 범위의 데이터와 비교합니다.

   1. **[!UICONTROL Comparison]** 슬라이더를 &quot;켜짐&quot; 위치로 이동합니다.

      이 옵션을 선택하면 각 일반 데이터 열에 대해 두 개의 열이 더 추가됩니다. 예를 들어 테이블에 &quot;[!UICONTROL Impressions]&quot;에 대한 열을 하나만 포함하는 대신 &quot;[!UICONTROL Impressions R1]&quot;, &quot;[!UICONTROL Impressions R2]&quot; 및 &quot;[!UICONTROL Impressions Diff]&quot;에 대한 열이 포함됩니다.  데이터를 내보내면 동일한 열의 철자가 &quot;[!UICONTROL Impressions Range 1]&quot;, &quot;[!UICONTROL Impressions Range 2]&quot; 및 &quot;[!UICONTROL Impressions Difference]&quot;로 지정됩니다.

   1. 두 번째 날짜 범위를 지정합니다.

   1. &quot;\[_데이터 필드_\] 차이&quot; 열에서 선택한 두 날짜 범위의 데이터 차이를 표시하는 방법을 선택하십시오.

      * *[!UICONTROL Variance]*(기본값): 차이를 숫자 값으로 표시합니다.

      * *[!UICONTROL % Change]:* 차이를 백분율로 표시합니다.

1. **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.
