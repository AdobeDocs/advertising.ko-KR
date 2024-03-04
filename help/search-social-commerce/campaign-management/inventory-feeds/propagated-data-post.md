---
title: 피드에서 생성된 캠페인 데이터를 광고 네트워크에 게시
description: 인벤토리 데이터 피드에서 생성된 데이터를 광고 네트워크에 게시하는 방법을 알아봅니다.
exl-id: 7d66c52b-f761-4be2-a1d9-2c63887d7cb7
feature: Search Inventory Feeds
source-git-commit: c27665b979ad8e37fd4f92385bb7339af4354d5f
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 0%

---

# 피드에서 생성된 캠페인 데이터를 광고 네트워크에 게시

*[!DNL Google Ads], [!DNL Microsoft® Advertising], [!DNL Yahoo! Japan Ads] (작업만 삭제) 및 [!DNL Yandex] 계정만*

피드에서 생성된 캠페인 데이터를 관련 템플릿을 통해 전파할 때 또는 별도의 프로세스로 게시할 수 있습니다. 데이터를 게시하면 기존의 전파된 데이터가 [!UICONTROL Campaigns], [!UICONTROL Ad Groups], [!UICONTROL Keywords], 및 [!UICONTROL Ads] 목록을 표시합니다.

게시가 성공하려면 모든 광고 그룹을 캠페인에 할당하고, 모든 키워드와 광고를 광고 그룹에 할당하며, 길이 위반 없이 모든 필수 정보를 포함해야 합니다.

* 옵션을 사용하여 &quot;[!UICONTROL Propagate and Preview],&quot; 그런 다음 [생성된 일괄 시트 파일 게시](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-post.md) (이름이 &quot;`<feed file name>_<template name>`&quot;)을(를) 통해 가져왔습니다. [!UICONTROL Bulksheets] 보기.

  이전에 하지 않았다면 [랜딩 페이지 유효성 검사](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-validate-landing-pages.md)그런 다음 파일을 게시하기 전에 이 작업을 수행할 수 있습니다.

* 옵션을 사용하여 &quot;[!UICONTROL Propagate only],&quot; 그런 다음 구성 요소에 대해 생성된 데이터를 [[!UICONTROL New] 상태](propagated-data-status.md) 에서 캠페인 계층 구조 보기 내 [!UICONTROL Templates] 탭.

  >[!NOTE]
  >
  >활성 또는 삭제된 구성 요소에는 새로운 하위 구성 요소가 포함될 수 있으며 데이터가 유효한 경우 하위 구성 요소를 게시할 수 있습니다.

  >[!TIP]
  >
  >이전에 랜딩 페이지의 유효성을 검사하지 않았으며 확인하고자 하는 경우, [데이터 전파 및 미리보기](feed-data-propagate.md) 다음에서 [!UICONTROL Bulksheets] 광고 네트워크에 게시하지 않고 봅니다. 그런 다음 [url의 유효성 검사](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-validate-landing-pages.md) 파일을 광고 네트워크에 수동으로 게시하기 전에.

   1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Advanced (ACM)]**: 다음에 열립니다. [!UICONTROL Templates] 탭.

   1. 템플릿 옆에 있는 확인란을 선택합니다.

   1. 도구 모음에서 를 클릭합니다 **[!UICONTROL Post]**.

   1. 게시 설정에서 필드에 정보를 입력하거나 선택한 다음 을 클릭합니다. **[!UICONTROL Post]**.

      * **[!UICONTROL Selection]:** 게시되는 계정 구성 요소

      * **[!UICONTROL Scheduling]:** 파일 게시 시기:

         * *[!UICONTROL Post to search engine now]* (기본값): 전파된 피드 데이터에서 일괄 시트 파일을 생성하고 즉시 게시하기 시작합니다.

         * *[!UICONTROL Post to search engine on these start/end times (in America/Los_Angeles time)]:* 일괄 시트 파일을 만들고 나중에 게시합니다. 다음을 지정합니다.

            * **[!UICONTROL Start Time]:** 일괄 시트 파일을 광고 네트워크에 게시해야 하는 향후 날짜 및 시간입니다. 기본적으로 파일은 다음 날 00:00(오전 12:00)에 전송됩니다. **참고:** 더 긴 처리가 필요한 큰 파일의 경우, 게시된 데이터는 캠페인 관리 보기 또는 네트워크의 광고 관리자 내에서 즉시 사용할 수 없습니다.

            * **[!UICONTROL End Time]:** 게시한 광고를 다음에 따라 일시 중지 또는 삭제할 수 있는 향후 날짜 및 시간 [피드 데이터 설정](feed-settings-manage.md#feed-data-settings) 의 경우[!UICONTROL When the Scheduled End Date is reached].&quot; 기본적으로 종료 시간은 오늘부터 30일 후인 00:00(오전 12:00)입니다. 선택 **[!UICONTROL None]** 데이터를 무기한 활성 상태로 유지하거나(또는 템플릿에 대한 새 데이터를 전파할 때까지) 날짜 및 시간을 지정합니다.

              날짜를 지정하려면 DD/MM/YYYY 또는 D/M/YYYY 형식을 사용하거나 ![캘린더](/help/search-social-commerce/assets/calendar.png "캘린더") 캘린더를 열고 [날짜 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/calendar.md). 시간을 변경하려면 시간을 24시간 형식 HH/MM 또는 H/M으로 입력하거나 목록에서 시간(30분 간격)을 선택합니다.

         * **[!UICONTROL Preview in Bulksheet Management Area only, post later]:** 에서 사용할 수 있는 벌크 시트 파일을 만듭니다. [!UICONTROL Search] > [!UICONTROL Bulksheets] 보기. 선택적으로 여기에서 파일을 게시할 수 있습니다.

           결과 일괄 시트 파일이 2MB를 초과하는 경우 파일은 ZIP 형식입니다. 파일을 게시하기 위해 압축 해제할 필요가 없습니다.

      * **[!UICONTROL Generate Tracking URLs]:** 일괄 시트 파일에 키워드 및 광고 변형에 대한 추적 URL을 포함할지 여부: *[!UICONTROL Yes]* (기본값) 또는 *[!UICONTROL No]*.

        다음을 선택하는 경우 *[!UICONTROL Yes]*&#x200B;에 따라 키워드 및 광고의 기본 URL에서 URL이 생성됩니다 [!UICONTROL Tracking Methods] 의 매개 변수 [계정 설정](/help/search-social-commerce/campaign-management/accounts/ad-network-account-manage.md) 또는 기존 캠페인에 데이터를 매핑하는 경우 [!UICONTROL Tracking Methods] 기존 의 매개 변수 [캠페인 설정](/help/search-social-commerce/campaign-management/campaigns/campaign-manage.md).

        관련 항목에 대한 추적 URL이 있는 경우 새 URL이 필요하지 않으면 다시 생성되지 않습니다(예: 키워드 일치 유형, 크리에이티브 텍스트 또는 계정의 추적 매개 변수가 변경된 경우).

      * **[!UICONTROL Bulksheet Name]:** 전파된 피드 데이터에서 생성할 일괄 시트 파일의 이름입니다. 기본적으로 파일 이름은 로 지정됩니다 `<feed file name_file extension>_<feed template name>_<creation date in the format YYYYMMDDHHMMSS>.txt`. 원하는 대로 파일 이름을 바꿀 수 있지만 파일 확장명은 다음 중 하나로 끝나야 합니다. `.tsv` (탭으로 구분된 값의 경우), `.txt` (ASCII 텍스트의 경우), `.csv` (쉼표로 구분된 값의 경우) 또는 `.zip` (압축된 TSV 파일의 경우). 국제 문자가 포함된 데이터의 경우 TSV 또는 TXT 형식을 사용하십시오.

        게시된 파일은에서 사용할 수 있습니다. [!UICONTROL Bulksheets] 광고 네트워크에 게시할지 여부에 관계없이 30일 동안 봅니다.

&quot;[!UICONTROL Last Prop. Status]&quot;열에 적용 가능한 템플릿의 작업 상태가 표시됩니다.

일괄 시트가 만들어지면 다음 목록에 나열됩니다. [!UICONTROL Bulksheets] 보기. 파일이 게시되면 파일에 대한 링크가 포함된 이메일 알림이 전송됩니다. 그러나 데이터의 전부 또는 일부를 게시할 수 없으면 오류 파일이 [!UICONTROL Bulksheets] 을 확인하면 오류 파일에 대한 링크와 함께 이메일 알림이 전송됩니다.

>[!NOTE]
>
>* 선택한 예약 옵션에 관계없이 지정된 데이터는 [!UICONTROL Campaigns], [!UICONTROL Ad Groups], [!UICONTROL Keywords], 및 [!UICONTROL Ads] 목록을 표시합니다.
>* 많은 양의 데이터를 처리하는 데 시간이 더 오래 걸립니다. 프로세스 중에 파일의 진행 상황을 따를 수 있습니다.
>* 게시된 모든 데이터는 네트워크의 편집 절차에 따릅니다.
>* 일괄 시트 파일을 게시하기 전에 다음을 수행할 수 있습니다 [게시 취소](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-stop-job.md).

>[!MORELIKETHIS]
>
>* [인벤토리 피드 기본 정보](inventory-feeds-about.md)
>* [피드에서 생성된 데이터 보기](propagated-data-view.md)
>* [피드에서 생성된 데이터 편집](propagated-data-edit.md)
>* [재고 피드 데이터에 대한 게시 작업 중지](stop-job.md)
>* [피드에서 생성된 데이터 상태](propagated-data-status.md)
