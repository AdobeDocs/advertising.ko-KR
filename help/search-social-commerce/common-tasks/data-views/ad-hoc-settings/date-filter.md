---
title: 날짜 범위별로 데이터 필터링
description: 글로벌 날짜 범위 필터를 사용하는 방법을 알아봅니다.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# 날짜 범위별로 데이터 필터링

특정 날짜 범위를 저장한 기본 및 사용자 지정 보기를 제외하고 모든 광고주에 걸쳐 있는 대부분의 캠페인 데이터 보기에 동일한 전역 날짜 범위 필터가 적용됩니다. 캠페인 관리 보기에 대한 시스템 기본 날짜 범위는 &quot;어제&quot;입니다.

날짜 범위 설정은 브라우저별 쿠키에 저장되므로, 필터를 변경하거나 쿠키를 삭제할 때까지 동일한 브라우저 애플리케이션을 사용하여 로그인할 때마다 날짜 범위 필터에 대한 모든 변경 사항이 모든 광고주에 대해 사용됩니다. 사용하는 각 브라우저 애플리케이션은 날짜 범위 필터 설정을 다른 쿠키에 저장합니다.

기본 보기 또는 사용자 지정 보기에 대해 특정 날짜 범위를 저장하면 사용 중인 브라우저 응용 프로그램에 관계없이 보기를 적용할 때마다 해당 범위가 적용됩니다.

>[!NOTE]
>
>* 이전 13개월의 데이터를 볼 수 있지만 기존의 모든 사용자 지정 보기에는 이전 180일까지의 데이터만 포함할 수 있습니다.
>* 이전 데이터를 보려면 [[!UICONTROL Reports] 보기](/help/search-social-commerce/reports/management/basic-advanced/basic-advanced-report-about.md) 기본 보고서를 실행합니다.
>* 날짜 범위를 저장할 수도 있습니다. [기본 보기 또는 사용자 지정 보기](/help/search-social-commerce/common-tasks/data-views/custom-default-views-manage.md).


## 캠페인 보기에서 전역 날짜 필터 변경

1. 검색 \> 캠페인 \> 캠페인의 데이터 테이블 위에서 현재 날짜 범위를 클릭합니다.

1. 다음에서 **[!UICONTROL Date Range]** 필드에서 범위를 지정합니다.

   * 사전 설정된 범위의 경우: 다음 범위의 공통 시간 증분 목록에서 선택합니다. *[!UICONTROL Today]* 끝 *[!UICONTROL Last 180 Days]*. 기본값은 입니다 *[!UICONTROL Yesterday]*.

   * 특정 범위의 경우 다음을 선택합니다 **[!UICONTROL Custom Date Range]** 를 클릭한 다음 시작 날짜와 종료 날짜를 지정합니다.

      날짜를 MM/DD/YYYY 또는 MM-DD-YYYY 형식으로 입력하거나 ![달력 아이콘](/help/search-social-commerce/assets/calendar.png "달력 아이콘") 각 필드 옆에 있는 을 클릭하여 달력을 열고 날짜를 선택합니다.

1. (선택 사항) 지정된 날짜 범위의 데이터를 두 번째 날짜 범위의 데이터와 비교합니다.

   1. 이동 **[!UICONTROL Comparison]** 슬라이더 *[!UICONTROL On]*.

      이 옵션을 선택하면 각 일반 데이터 열에 대해 두 개의 열이 더 추가됩니다. 예를 들어 &quot;에 대해 하나의 열만 포함하는 대신[!UICONTROL Impressions],&quot; 표에는 &quot;에 대한 열이 포함되어 있습니다.[!UICONTROL Impressions R1],&quot; &quot;[!UICONTROL Impressions R2]및 &quot;[!UICONTROL Impressions Diff].&quot;  데이터를 내보내면 동일한 열의 맞춤법이 다음과 같습니다[!UICONTROL Impressions Range 1],&quot; &quot;[!UICONTROL Impressions Range 2]및 &quot;[!UICONTROL Impressions Difference].&quot;

   1. 두 번째 날짜 범위를 지정합니다.

   1. &quot;\[&quot;에서 선택한 두 날짜 범위의 데이터 차이를 표시하는 방법 선택&#x200B;_데이터 필드_\] 차이&quot; 열:

      * *[!UICONTROL Variance]* (기본값): 차이를 숫자 값으로 표시합니다.

      * *[!UICONTROL % Change]:*  차이를 백분율로 표시합니다.

1. 클릭 **[!UICONTROL Apply]**.
