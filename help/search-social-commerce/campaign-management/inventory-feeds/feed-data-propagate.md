---
title: 템플릿을 통해 인벤토리 피드 데이터 전파
description: 계정 구조를 관리하고 동적 광고를 게재하기 위해 인벤토리 피드에서 광고 템플릿을 통해 데이터를 전파하는 방법에 대해 알아봅니다.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '874'
ht-degree: 0%

---

# 템플릿을 통해 인벤토리 피드 데이터 전파

*[!DNL Google Ads], [!DNL Microsoft® Advertising], [!DNL Yahoo! Japan Ads] (작업만 삭제) 및 [!DNL Yandex] 계정만*

광고 네트워크별 피드 템플릿을 만들고 피드 파일 또는 [!DNL Google] 또는 [!DNL Microsoft®] 머천트 센터 계정 을 사용하면 다음에 따라 템플릿을 통해 피드 데이터를 전파하여 광고를 동적으로 만들 수 있습니다. [피드 데이터 설정](feed-settings-manage.md). 전달 중에 템플릿의 열 이름은 피드의 데이터 값으로 대체되며, 템플릿에서 다르게 지정하지 않는 한 생성된 캠페인 및 해당 구성 요소의 기본 설정은 다음과 같습니다. 템플릿 옵션에 따라 검색, 소셜 및 상거래는 광고에 대한 새 계정 구조(캠페인, 광고 그룹, 키워드)를 생성하거나 광고를 기존 계정 구조에 매핑합니다.

새 피드 데이터에 항목에 대한 새 데이터 값이 포함되어 있거나 템플릿이 변경되면 기존 광고가 삭제되고 새 광고가 만들어집니다. 변경 사항이 다음의 지정인 경우 [!DNL Google Ads] 매개 변수 1 및 매개 변수 2를 사용하면 해당 값만 업데이트됩니다. 중복 광고(동일한 광고 사본 및 랜딩 페이지)는 생성되지 않습니다.

데이터를 전파할 때 선택적으로 캠페인 계층 보기 내에서 생성된 데이터를 미리 보거나, 검토를 위해 일괄 시트 파일을 생성하거나, 광고 네트워크에 즉시 게시하기 위해 일괄 시트 파일을 생성할 수 있습니다. 각 전달 작업이 완료되면 전달 탭에 전달 요약이 추가되어 전달을 기반으로 생성, 일시 중지 또는 삭제되었거나 생성될 각 엔티티 유형의 수를 나타냅니다. 데이터를 즉시 게시하지 않는 경우 미리 보고 나중에 게시할 수 있습니다.

## 에서 피드 파일 전파 [!UICONTROL Templates] 탭

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Advanced (ACM)]**: 다음에 열립니다. [!UICONTROL Templates] 탭.

1. 전파할 템플릿 옆에 있는 확인란을 선택합니다.

1. 도구 모음에서 를 클릭합니다 **[!UICONTROL Propagate]**&#x200B;을 클릭하고 다음 옵션 중 하나를 선택합니다.

   * **[!UICONTROL Propagate Only]:** 에 전파된 데이터를 표시하려면 [!UICONTROL Campaigns], [!UICONTROL Ad Groups], [!UICONTROL Keywords], 및 [!UICONTROL Ads] 탭. 구성 요소 및 하위 구성 요소에 대한 데이터는 나중에 [!UICONTROL Templates] 탭.

   * **[!UICONTROL Propagate and Preview]:** 일괄 시트 파일(&quot;`<feed file name>_<template name>`&quot;): [!UICONTROL Bulksheets] 검토를 위해 보기(하지만 에는 없음) [!UICONTROL Campaigns], [!UICONTROL Ad Groups], [!UICONTROL Keywords], 및 [!UICONTROL Ads] 탭). 나중에 일괄 시트 파일을 [!UICONTROL Bulksheets] 보기.

      결과 일괄 시트 파일이 2MB를 초과하는 경우 파일은 ZIP 형식입니다. 파일을 게시하기 위해 압축 해제할 필요가 없습니다.

   * **[!UICONTROL Propagate and Post to SE]:** 일괄 시트 파일(&quot;`<feed file name>_<template name>`광고 네트워크에 게시하기 위해 즉시 대기열에 추가되는 &quot;) 일괄 시트 파일은 다음에서 사용할 수 있습니다. [!UICONTROL Bulksheets] 보기는 하지만 [!UICONTROL Campaigns], [!UICONTROL Ad Groups], [!UICONTROL Keywords], 및 [!UICONTROL Ads] 탭.

      결과 일괄 시트 파일이 2MB를 초과하는 경우 파일은 ZIP 형식입니다.
   &quot;마지막 Prop. 상태&quot; 열에는 해당 템플릿에 대한 작업 상태가 표시됩니다.

   각 전달 작업이 완료되면 전달 요약이 [!UICONTROL Propagations] 전달을 기반으로 생성, 일시 중지 또는 삭제되었거나 삭제될 각 엔티티 유형의 수를 나타내는 탭입니다. 예상 값에는 광고 네트워크의 자체 광고 편집기 내에서 수행한 변경 사항이 포함되지 않습니다.

## 에서 피드 파일 전파 [!UICONTROL Feeds] 목록

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Advanced (ACM)]**.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL Feeds]**.

1. 피드 파일 옆에 있는 확인란을 선택합니다.

1. 데이터 테이블 위에서 **[!UICONTROL Propagate/Post Feed Data]**&#x200B;을 클릭하고 다음 옵션 중 하나를 선택합니다.

   * **[!UICONTROL Propagate Only]:** 에 전파된 데이터를 표시하려면 [!UICONTROL Campaigns], [!UICONTROL Ad Groups], [!UICONTROL Keywords], 및 [!UICONTROL Ads] 탭. 구성 요소 및 하위 구성 요소에 대한 데이터는 나중에 [!UICONTROL Templates] 탭.

   * **[!UICONTROL Propagate and Preview]:** 일괄 시트 파일(&quot;`<feed file name>_<template name>`&quot;): [!UICONTROL Bulksheets] 검토를 위해 보기(하지만 에는 없음) [!UICONTROL Campaigns], [!UICONTROL Ad Groups], [!UICONTROL Keywords], 및 [!UICONTROL Ads] 탭). 나중에 일괄 시트 파일을 [!UICONTROL Bulksheets] 보기.

      결과 일괄 시트 파일이 2MB를 초과하는 경우 파일은 ZIP 형식입니다. 파일을 게시하기 위해 압축 해제할 필요가 없습니다.

   * **[!UICONTROL Propagate and Post to SE]:** 일괄 시트 파일(&quot;`<feed file name>_<template name>`광고 네트워크에 게시하기 위해 즉시 대기열에 추가되는 &quot;) 일괄 시트 파일은 다음에서 사용할 수 있습니다. [!UICONTROL Bulksheets] 보기는 하지만 [!UICONTROL Campaigns], [!UICONTROL Ad Groups], [!UICONTROL Keywords], 및 [!UICONTROL Ads] 탭.

      결과 일괄 시트 파일이 2MB를 초과하는 경우 파일은 ZIP 형식입니다.

1. 팝업 창에서 피드 파일의 데이터를 전달할 각 템플릿 옆의 확인란을 선택한 다음 을 클릭합니다 **[!UICONTROL Propagate Feed]**.

   파일과 연관된 모든 템플릿이 나열됩니다.

다음 [!UICONTROL Templates] 탭이 열리고, &quot;[!UICONTROL Last Prop. Status]&quot;열에 적용 가능한 템플릿의 작업 상태가 표시됩니다.

각 전달 작업이 완료되면 전달 요약이 [!UICONTROL Propagations] 전달을 기반으로 생성, 일시 중지 또는 삭제되었거나 삭제될 각 엔티티 유형의 수를 나타내는 탭입니다. 예상 값에는 광고 네트워크의 자체 광고 편집기 내에서 수행한 변경 사항이 포함되지 않습니다.

## 전달 요약 보기

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Advanced (ACM)]**.

1. 다음을 클릭합니다. **[!UICONTROL Propagations]** 탭.

1. 템플릿 이름 옆에 있는 ![설정 보기/편집 아이콘](/help/search-social-commerce/assets/settings.png "설정 보기/편집 아이콘") .

## 전달 작업 중지

작업이 대기열에 있는 동안 재고 피드 데이터에 대한 전달 작업을 중지할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Advanced (ACM)]**: 다음에 열립니다. [!UICONTROL Templates] 탭.

1. 의 &quot;[!UICONTROL Last Prop. Status]템플릿 이름 옆에 있는 &quot; 열에서 **[!UICONTROL Cancel]**.

>[!MORELIKETHIS]
>
>* [인벤토리 피드 기본 정보](inventory-feeds-about.md)
>* [인벤토리 피드에 대한 광고 템플릿 관리](/help/search-social-commerce/campaign-management/inventory-feeds/ad-templates/ad-template-manage.md)
>* [피드에서 생성된 데이터 보기](propagated-data-view.md)
>* [피드에서 생성된 데이터 편집](propagated-data-edit.md)
>* [피드에서 생성된 캠페인 데이터를 광고 네트워크에 게시](propagated-data-post.md)
>* [재고 피드 데이터에 대한 게시 작업 중지](stop-job.md)
>* [피드에서 생성된 데이터 상태](propagated-data-status.md)

