---
title: 템플릿을 통해 인벤토리 피드 데이터 전파
description: 계정 구조를 관리하고 동적 광고를 게재하기 위해 인벤토리 피드에서 광고 템플릿을 통해 데이터를 전파하는 방법에 대해 알아봅니다.
exl-id: 9660af19-a517-4593-9a99-da600a0285a5
feature: Search Inventory Feeds
source-git-commit: 67fe8581832dc0762d62908d01672e53cc95b847
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---

# 템플릿을 통해 인벤토리 피드 데이터 전파

*[!DNL Google Ads], [!DNL Microsoft Advertising], [!DNL Yahoo! Japan Ads](삭제 작업만) 및 [!DNL Yandex] 계정만*

광고 네트워크별 피드 템플릿을 만들고 피드 파일 또는 [!DNL Google] 또는 [!DNL Microsoft] 판매자 센터 계정을 연결한 후 [피드 데이터 설정](feed-settings-manage.md)에 따라 템플릿을 통해 피드 데이터를 전파하여 광고를 동적으로 만들 수 있습니다. 전달 중에 템플릿의 열 이름은 피드의 데이터 값으로 대체되며, 템플릿에서 다르게 지정하지 않는 한 생성된 캠페인 및 해당 구성 요소의 기본 설정은 다음과 같습니다. 템플릿 옵션에 따라 검색, 소셜 및 Commerce은 광고에 대한 새 계정 구조(캠페인, 광고 그룹, 키워드)를 만들거나 광고를 기존 계정 구조에 매핑합니다.

새 피드 데이터에 항목에 대한 새 데이터 값이 포함되어 있거나 템플릿이 변경되면 기존 광고가 삭제되고 새 광고가 만들어집니다. [!DNL Google Ads] 매개 변수 1 및 매개 변수 2를 지정하는 경우에만 해당 값이 업데이트됩니다. 중복 광고(동일한 광고 사본 및 랜딩 페이지)는 생성되지 않습니다.

데이터를 전파할 때 선택적으로 캠페인 계층 보기 내에서 생성된 데이터를 미리 보거나, 검토를 위해 일괄 시트 파일을 생성하거나, 광고 네트워크에 즉시 게시하기 위해 일괄 시트 파일을 생성할 수 있습니다. 각 전달 작업이 완료되면 전달 탭에 전달 요약이 추가되어 전달을 기반으로 생성, 일시 중지 또는 삭제되었거나 생성될 각 엔티티 유형의 수를 나타냅니다. 데이터를 즉시 게시하지 않는 경우 미리 보고 나중에 게시할 수 있습니다.

## [!UICONTROL Templates] 탭에서 피드 파일 전파

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Advanced (ACM)]**&#x200B;을(를) 클릭합니다. 그러면 [!UICONTROL Templates] 탭이 열립니다.

1. 전파할 템플릿 옆에 있는 확인란을 선택합니다.

1. 도구 모음에서 **[!UICONTROL Propagate]**&#x200B;을(를) 클릭하고 다음 옵션 중 하나를 선택합니다.

   * **[!UICONTROL Propagate Only]:** [!UICONTROL Campaigns], [!UICONTROL Ad Groups], [!UICONTROL Keywords] 및 [!UICONTROL Ads] 탭에서 전파된 데이터를 표시합니다. 나중에 [!UICONTROL Templates] 탭에서 구성 요소 및 해당 하위 구성 요소에 대한 데이터를 게시할 수 있습니다.

   * **[!UICONTROL Propagate and Preview]:** 일괄 시트 파일(이름이 &quot;`<feed file name>_<template name>`&quot;임)을 만들려면 [!UICONTROL Bulksheets] 보기에서 검토할 수 있습니다([!UICONTROL Campaigns], [!UICONTROL Ad Groups], [!UICONTROL Keywords] 및 [!UICONTROL Ads] 탭에서는 사용할 수 없음). 나중에 [!UICONTROL Bulksheets] 보기에서 일괄 시트 파일을 게시할 수 있습니다.

     결과 일괄 시트 파일이 2MB를 초과하는 경우 파일은 ZIP 형식입니다. 파일을 게시하기 위해 압축 해제할 필요가 없습니다.

   * **[!UICONTROL Propagate and Post to SE]:** 광고 네트워크에 게시하기 위해 즉시 대기 중인 일괄 시트 파일(&quot;`<feed file name>_<template name>`&quot;)을 만들려면. 일괄 시트 파일은 [!UICONTROL Bulksheets] 보기에서 사용할 수 있지만 [!UICONTROL Campaigns], [!UICONTROL Ad Groups], [!UICONTROL Keywords] 및 [!UICONTROL Ads] 탭에서는 사용할 수 없습니다.

     결과 일괄 시트 파일이 2MB를 초과하는 경우 파일은 ZIP 형식입니다.

   &quot;마지막 Prop. 상태&quot; 열에는 해당 템플릿에 대한 작업 상태가 표시됩니다.

   각 전파 작업이 완료되면 [!UICONTROL Propagations] 탭에 전파 요약이 추가되어 전파를 기반으로 생성, 일시 중지 또는 삭제되었거나 생성되었을 각 엔터티 형식의 수를 나타냅니다. 예상 값에는 광고 네트워크의 자체 광고 편집기 내에서 수행한 변경 사항이 포함되지 않습니다.

## [!UICONTROL Feeds] 목록에서 피드 파일 전파

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Advanced (ACM)]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL Feeds]**&#x200B;을(를) 클릭합니다.

1. 피드 파일 옆에 있는 확인란을 선택합니다.

1. 데이터 테이블 위에서 **[!UICONTROL Propagate/Post Feed Data]**&#x200B;을(를) 클릭하고 다음 옵션 중 하나를 선택합니다.

   * **[!UICONTROL Propagate Only]:** [!UICONTROL Campaigns], [!UICONTROL Ad Groups], [!UICONTROL Keywords] 및 [!UICONTROL Ads] 탭에서 전파된 데이터를 표시합니다. 나중에 [!UICONTROL Templates] 탭에서 구성 요소 및 해당 하위 구성 요소에 대한 데이터를 게시할 수 있습니다.

   * **[!UICONTROL Propagate and Preview]:** 일괄 시트 파일(이름이 &quot;`<feed file name>_<template name>`&quot;임)을 만들려면 [!UICONTROL Bulksheets] 보기에서 검토할 수 있습니다([!UICONTROL Campaigns], [!UICONTROL Ad Groups], [!UICONTROL Keywords] 및 [!UICONTROL Ads] 탭에서는 사용할 수 없음). 나중에 [!UICONTROL Bulksheets] 보기에서 일괄 시트 파일을 게시할 수 있습니다.

     결과 일괄 시트 파일이 2MB를 초과하는 경우 파일은 ZIP 형식입니다. 파일을 게시하기 위해 압축 해제할 필요가 없습니다.

   * **[!UICONTROL Propagate and Post to SE]:** 광고 네트워크에 게시하기 위해 즉시 대기 중인 일괄 시트 파일(&quot;`<feed file name>_<template name>`&quot;)을 만들려면. 일괄 시트 파일은 [!UICONTROL Bulksheets] 보기에서 사용할 수 있지만 [!UICONTROL Campaigns], [!UICONTROL Ad Groups], [!UICONTROL Keywords] 및 [!UICONTROL Ads] 탭에서는 사용할 수 없습니다.

     결과 일괄 시트 파일이 2MB를 초과하는 경우 파일은 ZIP 형식입니다.

1. 팝업 창에서 피드 파일의 데이터를 전달할 각 템플릿 옆의 확인란을 선택한 다음 **[!UICONTROL Propagate Feed]**&#x200B;을(를) 클릭합니다.

   파일과 연관된 모든 템플릿이 나열됩니다.

[!UICONTROL Templates] 탭이 열리고 &quot;[!UICONTROL Last Prop. Status]&quot; 열에 적용 가능한 템플릿에 대한 작업 상태가 표시됩니다.

각 전파 작업이 완료되면 [!UICONTROL Propagations] 탭에 전파 요약이 추가되어 전파를 기반으로 생성, 일시 중지 또는 삭제되었거나 생성되었을 각 엔터티 형식의 수를 나타냅니다. 예상 값에는 광고 네트워크의 자체 광고 편집기 내에서 수행한 변경 사항이 포함되지 않습니다.

## 전달 요약 보기

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Advanced (ACM)]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Propagations]** 탭을 클릭합니다.

1. 템플릿 이름 옆에 있는 ![설정 보기/편집 아이콘](/help/search-social-commerce/assets/settings.png "설정 보기/편집 아이콘")을 클릭합니다.

## 전달 작업 중지

작업이 대기열에 있는 동안 재고 피드 데이터에 대한 전달 작업을 중지할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Advanced (ACM)]**&#x200B;을(를) 클릭합니다. 그러면 [!UICONTROL Templates] 탭이 열립니다.

1. 템플릿 이름 옆의 &quot;[!UICONTROL Last Prop. Status]&quot; 열에서 **[!UICONTROL Cancel]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [인벤토리 피드 정보](inventory-feeds-about.md)
>* [인벤토리 피드에 대한 광고 템플릿 관리](/help/search-social-commerce/campaign-management/inventory-feeds/ad-templates/ad-template-manage.md)
>* [피드에서 생성된 데이터 보기](propagated-data-view.md)
>* [피드에서 생성된 데이터 편집](propagated-data-edit.md)
>* [피드에서 생성된 캠페인 데이터를 광고 네트워크에 게시](propagated-data-post.md)
>* [인벤토리 피드 데이터에 대한 게시 작업 중지](stop-job.md)
>* [피드에서 생성된 데이터의 상태](propagated-data-status.md)
