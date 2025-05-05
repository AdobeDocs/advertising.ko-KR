---
title: 피드에서 생성된 데이터 상태
description: 인벤토리 데이터 피드에서 생성된 데이터의 상태에 대해 알아봅니다.
exl-id: 45c93fb2-0ed2-4336-9883-e150c292a7a5
feature: Search Inventory Feeds
source-git-commit: 67fe8581832dc0762d62908d01672e53cc95b847
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# 피드에서 생성된 데이터 상태

*[!DNL Google Ads], [!DNL Microsoft Advertising], [!DNL Yahoo! Japan Ads] (삭제 작업만) 및 [!DNL Yandex] 계정만*

각 구성 요소는 다음 상태 중 하나를 가질 수 있습니다.

* *[!UICONTROL New]:* 구성 요소가 광고 네트워크에 없으며 광고 네트워크에 게시되지 않았습니다. 필요한 경우 구성 요소 이름을 클릭하여 설정을 편집할 수 있습니다. 데이터를 게시할 준비가 되면 **[!UICONTROL Post to SE]**&#x200B;을(를) 클릭하고 제출할 데이터를 지정하십시오.

* *[!UICONTROL Posted]:*(캠페인 및 광고 그룹만 해당) 캠페인 또는 광고 그룹이 광고 네트워크에 부분적으로 게시되었지만 일부 구성 요소는 오류로 인해 게시되지 않았습니다. 각 키워드 및 광고의 유효성 검사 상태는 수정해야 하는 정보를 보여줍니다. 필요한 경우 구성 요소 이름을 클릭하여 구성 요소의 설정을 편집할 수 있습니다.

* *[!UICONTROL Active]:* 구성 요소가 이미 광고 네트워크에서 활성화되어 있으므로 여기에서 해당 설정을 편집할 수 없습니다. 활성 구성 요소에는 데이터가 올바른 경우 게시할 수 있는 하위 구성 요소 [!UICONTROL New]이(가) 포함될 수 있습니다.

* *[!UICONTROL Paused]:* 구성 요소가 광고 네트워크에서 이미 일시 중지되었으므로 여기에서 해당 설정을 편집할 수 없습니다. 일시 중지된 구성 요소에는 데이터가 올바른 경우 게시할 수 있는 [!UICONTROL New]인 하위 구성 요소가 포함될 수 있습니다.

* *[!UICONTROL Deleted]:* 구성 요소가 광고 네트워크에서 이미 삭제되었으므로 여기에서 해당 설정을 편집할 수 없습니다. 삭제된 구성 요소에는 데이터가 올바른 경우 게시할 수 있는 하위 구성 요소 [!UICONTROL New]이(가) 포함될 수 있습니다.

>[!MORELIKETHIS]
>
>* [인벤토리 피드 정보](inventory-feeds-about.md)
>* [피드에서 생성된 데이터 보기](propagated-data-view.md)
>* [피드에서 생성된 데이터 편집](propagated-data-edit.md)
>* [피드에서 생성된 캠페인 데이터를 광고 네트워크에 게시](propagated-data-post.md)
>* [인벤토리 피드 데이터에 대한 게시 작업 중지](stop-job.md)
