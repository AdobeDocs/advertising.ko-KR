---
title: 피드에서 생성된 캠페인 데이터를 광고 네트워크에 게시
description: 인벤토리 데이터 피드에서 생성된 데이터를 광고 네트워크에 게시하는 방법을 알아봅니다.
exl-id: 7d66c52b-f761-4be2-a1d9-2c63887d7cb7
feature: Search Inventory Feeds
source-git-commit: 2cf15dbab3dc00ec88a41e4f7d8b5b3646b843e8
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 0%

---

# 피드에서 생성된 캠페인 데이터를 광고 네트워크에 게시

*[!DNL Google Ads], [!DNL Microsoft Advertising], [!DNL Yahoo! Japan Ads] (삭제 작업만) 및 [!DNL Yandex] 계정만*

피드에서 생성된 캠페인 데이터를 관련 템플릿을 통해 전파할 때 또는 별도의 프로세스로 게시할 수 있습니다. 데이터를 게시하면 기존의 전파된 데이터가 [!UICONTROL Campaigns], [!UICONTROL Ad Groups], [!UICONTROL Keywords] 및 [!UICONTROL Ads] 목록에서 제거됩니다.

게시가 성공하려면 모든 광고 그룹을 캠페인에 할당하고, 모든 키워드와 광고를 광고 그룹에 할당하며, 길이 위반 없이 모든 필수 정보를 포함해야 합니다.

* 옵션을 &quot;[!UICONTROL Propagate and Preview]&quot;에 사용한 경우 [!UICONTROL Bulksheets] 보기에서 [생성된 일괄 시트 파일](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-post.md)(&quot;`<feed file name>_<template name>`&quot;)을 게시합니다.

  이전에 [랜딩 페이지의 유효성 검사](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-validate-landing-pages.md)를 하지 않았다면 파일을 게시하기 전에 확인할 수 있습니다.

* 옵션을 &quot;[!UICONTROL Propagate only]&quot;에 사용한 경우 [!UICONTROL Templates] 탭에서 캠페인 계층 구조 보기 내에 [[!UICONTROL New] 상태가 ](propagated-data-status.md)인 구성 요소에 대해 생성된 데이터를 게시할 수 있습니다.

  >[!NOTE]
  >
  >활성 또는 삭제된 구성 요소에는 새로운 하위 구성 요소가 포함될 수 있으며 데이터가 유효한 경우 하위 구성 요소를 게시할 수 있습니다.

  >[!TIP]
  >
  >이전에 랜딩 페이지의 유효성을 검사하지 않았으며 그렇게 하려면 광고 네트워크에 게시하지 않고 [데이터를 전파하고 [!UICONTROL Bulksheets] 보기에서 미리 보기](feed-data-propagate.md)합니다. 그런 다음 파일을 광고 네트워크에 수동으로 게시하기 전에 [URL의 유효성을 확인](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-validate-landing-pages.md)할 수 있습니다.

   1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Advanced (ACM)]**&#x200B;을(를) 클릭합니다. 그러면 [!UICONTROL Templates] 탭이 열립니다.

   1. 템플릿 옆에 있는 확인란을 선택합니다.

   1. 도구 모음에서 **[!UICONTROL Post]**&#x200B;을(를) 클릭합니다.

   1. 게시 설정에서 필드에 정보를 입력하거나 선택한 다음 **[!UICONTROL Post]**&#x200B;을(를) 클릭합니다.

      * **[!UICONTROL Selection]:** 게시된 계정 구성 요소입니다.

      * **[!UICONTROL Scheduling]:** 파일을 게시할 시기:

         * *[!UICONTROL Post to search engine now]*(기본값): 전파된 피드 데이터에서 일괄 시트 파일을 만들고 즉시 게시하기 시작합니다.

         * *[!UICONTROL Post to search engine on these start/end times (in America/Los_Angeles time)]:* 일괄 시트 파일을 만들고 나중에 게시합니다. 다음을 지정합니다.

            * **[!UICONTROL Start Time]:** 일괄 시트 파일을 광고 네트워크에 게시해야 하는 미래 날짜 및 시간입니다. 기본적으로 파일은 다음 날 00:00(오전 12:00)에 전송됩니다. **참고:** 더 오래 처리해야 하는 대용량 파일의 경우 캠페인 관리 보기 또는 네트워크의 광고 관리자 내에서 게시된 데이터를 즉시 사용할 수 없습니다.

            * **[!UICONTROL End Time]:** &quot;[!UICONTROL When the Scheduled End Date is reached]&quot;에 대한 [피드 데이터 설정](feed-settings-manage.md#feed-data-settings)을(를) 기반으로 게시된 광고를 일시 중지하거나 삭제할 수 있는 향후 날짜 및 시간입니다. 기본적으로 종료 시간은 오늘부터 30일 후인 00:00(오전 12:00)입니다. **[!UICONTROL None]**&#x200B;을(를) 선택하여 무기한으로(또는 템플릿에 대한 새 데이터를 전파할 때까지) 데이터를 활성 상태로 유지하거나 날짜 및 시간을 지정하십시오.

              날짜를 지정하려면 DD/MM/YYYY 또는 D/M/YYYY 형식을 사용하거나 ![달력](/help/search-social-commerce/assets/calendar.png "달력")을 클릭하여 달력을 열고 [날짜를 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/calendar.md)합니다. 시간을 변경하려면 시간을 24시간 형식 HH/MM 또는 H/M으로 입력하거나 목록에서 시간(30분 간격)을 선택합니다.

         * **[!UICONTROL Preview in Bulksheet Management Area only, post later]:** [!UICONTROL Search] > [!UICONTROL Bulksheets] 보기에서 사용할 수 있는 일괄 시트 파일을 만듭니다. 선택적으로 여기에서 파일을 게시할 수 있습니다.

           결과 일괄 시트 파일이 2MB를 초과하는 경우 파일은 ZIP 형식입니다. 파일을 게시하기 위해 압축 해제할 필요가 없습니다.

      * **[!UICONTROL Generate Tracking URLs]:** 일괄 시트 파일에 키워드 및 광고 변형에 대한 추적 URL을 포함할지 여부: *[!UICONTROL Yes]*(기본값) 또는 *[!UICONTROL No]*.

        *[!UICONTROL Yes]*&#x200B;을(를) 선택하면 [계정 설정](/help/search-social-commerce/campaign-management/accounts/ad-network-account-manage.md)의 [!UICONTROL Tracking Methods] 매개 변수에 따라 키워드 및 광고의 기본 URL에서 URL이 생성되거나 기존 캠페인에 데이터를 매핑하는 경우 기존 [캠페인 설정](/help/search-social-commerce/campaign-management/campaigns/campaign-manage.md)의 [!UICONTROL Tracking Methods] 매개 변수에 URL이 생성됩니다.

        관련 항목에 대한 추적 URL이 있는 경우 새 URL이 필요하지 않으면 다시 생성되지 않습니다(예: 키워드 일치 유형, 크리에이티브 텍스트 또는 계정의 추적 매개 변수가 변경된 경우).

      * **[!UICONTROL Bulksheet Name]:** 전파된 피드 데이터에서 만들 일괄 시트 파일의 이름입니다. 기본적으로 파일 이름은 `<feed file name_file extension>_<feed template name>_<creation date in the format YYYYMMDDHHMMSS>.txt`입니다. 파일의 이름은 원하는 대로 바꿀 수 있지만 `.tsv`(탭으로 구분된 값), `.txt`(ASCII 텍스트), `.csv`(쉼표로 구분된 값) 또는 `.zip`(압축된 TSV 파일) 중 하나로 끝나야 합니다. 국제 문자가 포함된 데이터의 경우 TSV 또는 TXT 형식을 사용하십시오.

        게시한 파일은 광고 네트워크에 게시했는지 여부에 관계없이 [!UICONTROL Bulksheets] 보기에서 30일 동안 사용할 수 있습니다.

&quot;[!UICONTROL Last Prop. Status]&quot; 열은 적용 가능한 템플릿에 대한 작업 상태를 표시합니다.

일괄 시트가 만들어지면 [!UICONTROL Bulksheets] 보기에 표시됩니다. 파일이 게시되면 파일에 대한 링크가 포함된 이메일 알림이 전송됩니다. 그러나 일부 데이터를 게시할 수 없는 경우에는 오류 파일이 [!UICONTROL Bulksheets] 보기에 나열되며 오류 파일에 대한 링크와 함께 전자 메일 알림이 전송됩니다.

>[!NOTE]
>
>* 선택한 예약 옵션에 관계없이 [!UICONTROL Campaigns], [!UICONTROL Ad Groups], [!UICONTROL Keywords] 및 [!UICONTROL Ads] 목록에서 지정된 데이터가 제거됩니다.
>* 많은 양의 데이터를 처리하는 데 시간이 더 오래 걸립니다. 프로세스 중에 파일의 진행 상황을 따를 수 있습니다.
>* 게시된 모든 데이터는 네트워크의 편집 절차에 따릅니다.
>* 일괄 시트 파일을 게시하기 전에 [게시를 취소](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-stop-job.md)할 수 있습니다.

>[!MORELIKETHIS]
>
>* [인벤토리 피드 정보](inventory-feeds-about.md)
>* [피드에서 생성된 데이터 보기](propagated-data-view.md)
>* [피드에서 생성된 데이터 편집](propagated-data-edit.md)
>* [인벤토리 피드 데이터에 대한 게시 작업 중지](stop-job.md)
>* [피드에서 생성된 데이터의 상태](propagated-data-status.md)
