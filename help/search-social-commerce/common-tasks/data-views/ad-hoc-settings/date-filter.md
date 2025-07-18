---
title: 날짜 범위별로 데이터 필터링
description: 글로벌 날짜 범위 필터를 사용하는 방법을 알아봅니다.
exl-id: 35c0f63f-84ae-4e8e-8a48-acae7ff24498
feature: Search Common Tasks, Search Custom Data Views
source-git-commit: a438e0c24f9ff83941710f890c55c94b74d4d0f3
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---

# 날짜 범위별로 데이터 필터링

<!-- The same in new UI and legacy CM views -->

특정 날짜 범위를 저장한 기본 및 사용자 지정 보기를 제외하고 모든 광고주에 걸쳐 있는 대부분의 데이터 보기에 동일한 전역 날짜 범위 필터가 적용됩니다. 캠페인 관리 보기에 대한 시스템 기본 날짜 범위는 &quot;어제&quot;입니다.

날짜 범위 설정은 브라우저별 쿠키에 저장되므로, 필터를 변경하거나 쿠키를 삭제할 때까지 동일한 브라우저 애플리케이션을 사용하여 로그인할 때마다 날짜 범위 필터에 대한 모든 변경 사항이 모든 광고주에 대해 사용됩니다. 사용하는 각 브라우저 애플리케이션은 날짜 범위 필터 설정을 다른 쿠키에 저장합니다.

기본 보기 또는 사용자 지정 보기에 대해 특정 날짜 범위를 저장하면 사용 중인 브라우저 응용 프로그램에 관계없이 보기를 적용할 때마다 해당 범위가 적용됩니다.

>[!NOTE]
>
>* 이전 13개월의 데이터를 볼 수 있지만 기존의 모든 사용자 지정 보기에는 이전 180일까지의 데이터만 포함할 수 있습니다.
>* 이전 데이터를 보려면 [[!UICONTROL Reports] 보기](/help/search-social-commerce/reports/management/basic-advanced/basic-advanced-report-about.md)(으)로 이동하여 기본 보고서를 실행하십시오.
>* [기본 보기 또는 사용자 지정 보기](/help/search-social-commerce/common-tasks/data-views/custom-default-views-manage.md)에 대한 날짜 범위를 저장할 수도 있습니다.

## 캠페인 보기에서 전역 날짜 필터 변경

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
