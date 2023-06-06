---
title: 피드에서 생성된 데이터 편집
description: 인벤토리 데이터 피드에서 생성된 데이터를 편집하는 방법을 알아봅니다.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 0%

---

# 피드에서 생성된 데이터 편집

*[!DNL Google Ads], [!DNL Microsoft® Advertising], [!DNL Yahoo! Japan Ads] (작업만 삭제) 및 [!DNL Yandex] 계정만*

피드 데이터를 광고 네트워크에 동시에 게시하지 않고 전파할 때 다음 방법 중 하나로 데이터를 편집할 수 있습니다. 나중에 필요에 따라 [게시물 데이터](propagated-data-post.md) 두 위치에서 관련 광고 네트워크로:

* 옵션을 사용하여 &quot;[!UICONTROL Propagate and Preview],&quot; 그런 다음 생성된 일괄 시트 파일(&quot;`<feed file name>_<template name>`&quot;) 을(를) 다운로드합니다. [!UICONTROL Bulksheets] 파일을 보고 편집한 다음 다시 업로드하십시오. 에 데이터가 포함되지 않음 [!UICONTROL Campaigns], [!UICONTROL Ad Groups], [!UICONTROL Keywords], 및 [!UICONTROL Ads] 탭.

* 옵션을 사용하여 &quot;[!UICONTROL Propagate only],&quot; 그런 다음 구성 요소에 대해 생성된 데이터를 [[!UICONTROL New] 상태](propagated-data-status.md) 에서 캠페인 계층 구조 보기 내 [!UICONTROL Campaigns], [!UICONTROL Ad Groups], [!UICONTROL Keywords], 및 [!UICONTROL Ads] 탭.

   캠페인 계층 구조 보기에는 기존 계정 구성 요소가 표시되지 않고 피드 파일에서 생성된 데이터만 표시됩니다. 구성 요소 및 모든 하위 구성 요소에 대한 데이터가 광고 네트워크에 게시되면 더 이상 캠페인 계층에 나열되지 않습니다.

   1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Advanced (ACM)]**: 다음에 열립니다. [!UICONTROL Templates] 탭.

   1. (선택 사항) 특정 템플릿에 대해 생성된 캠페인 구성 요소만 표시하려면 다음을 수행합니다.

      1. 템플릿 이름을 클릭합니다.

      1. 다음에서 [!UICONTROL Accounts] 왼쪽 탐색 창의 메뉴에서 광고 네트워크 노드 및 광고 네트워크 계정 노드를 확장한 다음 템플릿 이름 옆에 있는 확인란을 선택합니다.
   1. 다음을 클릭합니다. **[!UICONTROL Campaigns]**, **[!UICONTROL Ad Groups]**, **[!UICONTROL Keywords]**, 또는 **[!UICONTROL Ads]** 탭입니다. 보려는 구성 요소에 따라 다릅니다.

      >[!NOTE]
      >
      >* 특정 템플릿에 대한 데이터를 보지 않는 한 [!UICONTROL Ad Groups], [!UICONTROL Keywords], 및 [!UICONTROL Ads] 탭에는 모든 템플릿 및 피드 파일에서 만든 모든 광고 그룹, 키워드 및 광고가 나열됩니다. 에 사용된 제품 그룹 [!DNL Google Ads] 쇼핑 광고는 다음 목록에 있습니다. [!UICONTROL Keywords] 탭.
      >* 특정 캠페인의 하위 구성 요소만 보려면 [!UICONTROL Campaigns] 탭. 마찬가지로 특정 광고 그룹의 하위 구성 요소만 보려면 [!UICONTROL Ad Groups] 탭.


   1. (선택 사항, 광고 그룹, 키워드 또는 광고만 편집) 특정 캠페인 또는 광고 그룹의 하위 구성 요소만 포함하도록 목록을 필터링합니다.

      * 캠페인의 모든 광고 그룹을 나열하려면 캠페인 이름을 클릭합니다.

      * 광고 그룹의 모든 키워드를 나열하려면 광고 그룹 이름을 클릭합니다.

      * 광고 그룹의 모든 을(를) 나열하려면 광고 그룹 이름을 클릭한 다음 [!UICONTROL Ads] 탭.
   1. 클릭 [설정 보기/편집 아이콘](/help/search-social-commerce/assets/settings.png "설정 보기/편집 아이콘") 캠페인, 광고 그룹, 키워드 또는 광고 이름 옆에 있습니다.

   1. 설정을 편집한 다음 **[!UICONTROL Save]**.



>[!MORELIKETHIS]
>
>* [인벤토리 피드 기본 정보](inventory-feeds-about.md)
>* [피드에서 생성된 데이터 보기](propagated-data-view.md)
>* [피드에서 생성된 캠페인 데이터를 광고 네트워크에 게시](propagated-data-post.md)
>* [재고 피드 데이터에 대한 게시 작업 중지](stop-job.md)
>* [피드에서 생성된 데이터 상태](propagated-data-status.md)

