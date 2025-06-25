---
title: 복사 및 붙여넣기를 사용하여 캠페인 데이터 일괄 생성 및 편집
description: 복사 및 붙여넣기 기능을 사용하여 캠페인 데이터를 대량으로 관리하는 방법을 알아봅니다.
exl-id: 2ae1b02f-46ac-4ea8-aa9f-9e26ccaf63d0
feature: Search Campaign Management
source-git-commit: d0f1c413134a0868ddec79ded7672af316267edd
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# 복사 및 붙여넣기를 사용하여 캠페인 데이터 일괄 생성 및 편집

*[!DNL Google Ads], [!DNL Microsoft Advertising], [!DNL Yahoo! Japan Ads], [!DNL Yandex] 및 기존 [!DNL Baidu] 계정만*

*[!UICONTROL Campaigns], [!UICONTROL Ad Groups], [!UICONTROL Keywords] 및 [!UICONTROL Ads] 보기*

[!UICONTROL Campaigns], [!UICONTROL Ad Groups], [!UICONTROL Keywords] 및 [!UICONTROL Ads] 보기에서 최대 10,000개의 행을 복사하여 [!DNL Microsoft Excel] 또는 다른 편집기에 붙여 넣어 ID가 아닌 필드를 편집할 수 있습니다. 그런 다음 [!DNL Excel] 행을 복사하고 탭으로 구분된 데이터로 다시 뷰에 붙여넣어 변경할 수 있습니다. 이 기능은 컴퓨터의 클립보드를 사용합니다.

이 기능을 사용하여 기존 캠페인 개체(ID 필드 포함)를 편집하고 ID 필드 없이 새 캠페인 개체를 만들 수 있습니다.

## 데이터 행 복사

1. 메인 메뉴에서 **[!UICONTROL Search, Social, & Commerce]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다. 하위 메뉴에서 **[!UICONTROL Live]> \[[!UICONTROL Campaigns] \| 을 클릭합니다 [!UICONTROL Ad Groups] \| [!UICONTROL Keywords] \| [!UICONTROL Ads]\]**.

1. 복사할 각 행 옆의 확인란을 선택합니다.

   최대 10,000개의 행을 복사할 수 있습니다.

1. 데이터 테이블 위의 도구 모음에서 ![자세히](/help/search-social-commerce/assets/more.png "자세히")를 클릭한 다음 **[!UICONTROL Copy]**&#x200B;을(를) 클릭합니다.

   또는 운영 체제의 &quot;copy&quot; 키보드 명령(예: [!DNL Microsoft Windows]의 경우 **[!DNL Ctrl+C]**, [!DNL Apple Mac]의 경우 **[!DNL Command-C]**)을 사용할 수 있습니다.

1. [!UICONTROL Copy to Clipboard] 대화 상자에서 **[!UICONTROL Continue]**&#x200B;을(를) 클릭합니다. 데이터를 복사할 준비가 되면 **[!UICONTROL Copy]**&#x200B;을(를) 클릭합니다.

1. [!DNL Excel] 또는 다른 편집기에 행을 붙여 넣습니다.

## 데이터 행 편집 및 만들기

1. 다음 요구 사항에 따라 데이터를 편집합니다.

   * 붙여넣은 데이터에는 머리글 행과 필요한 캠페인 개체 값이 포함되어야 합니다. [Baidu](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-baidu.md), [Google 광고](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-google.md), [Microsoft Advertising](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-microsoft.md), [Naver](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-naver.md), [Yahoo!에 필요한 일괄 시트 열을 참조하십시오. 네트워크 표시](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-yahoo-display-network.md), [Yahoo! 일본](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-yahoo-japan.md) 및 [Yandex](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-yandex.md). 열 순서는 중요하지 않습니다.

      * 편집할 기존 객체의 경우 관련 ID 열, 엔티티 이름 및 편집할 속성을 모두 포함해야 합니다. 개체의 숫자 ID는 편집하지 마십시오.

      * 새 캠페인 객체의 경우 모든 관련 엔티티 이름과 속성을 포함하지만 자동으로 생성되는 객체 ID는 포함하지 마십시오. 예를 들어 새 광고를 만드는 경우 [!UICONTROL Ad ID] 필드를 비워 둡니다. 개체를 게시하면 광고 네트워크에서 ID를 자동으로 만듭니다.

   * 필요하지 않은 열의 값은 null(비어 있음)일 수 있지만 각 행에는 탭으로 구분된 동일한 수의 값이 있어야 합니다.

1. 데이터를 탭으로 구분된 값으로 저장합니다.

## 캠페인 관리 보기에 데이터 행 붙여넣기

>[!NOTE]
>
>붙여넣은 행에 기존 엔티티의 데이터와 동일한 데이터가 포함되어 있거나 기존 엔티티를 복제하는 경우 중복 데이터는 무시됩니다.

1. [!DNL Excel] 또는 다른 편집기에서 관련 탭으로 구분된 행을 복사합니다.

1. 검색, 소셜 및 Commerce 주 메뉴에서 **[!UICONTROL Search, Social, & Commerce]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다. 데이터를 붙여넣을 보기를 엽니다(**[!UICONTROL Live]> \[[!UICONTROL Campaigns] \|) [!UICONTROL Ad Groups] \| [!UICONTROL Keywords] \| [!UICONTROL Ads]\]**).

1. 데이터 테이블 위의 도구 모음에서 ![자세히](/help/search-social-commerce/assets/more.png "자세히")를 클릭한 다음 **[!UICONTROL Paste]**&#x200B;을(를) 클릭합니다.

   또는 운영 체제의 &quot;붙여넣기&quot; 키보드 명령(예: [!DNL Microsoft Windows]의 경우 **[!DNL Ctrl+V]**, [!DNL Apple Mac]의 경우 **[!DNL Command-V]**)을 사용할 수 있습니다.

1. 입력 상자에 데이터를 붙여 넣은 다음 **[!UICONTROL Process]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 추가 세부 정보를 입력합니다.

   * (**[!UICONTROL Additional Details]**&#x200B;이(가) 압축된 경우) ![열기](/help/search-social-commerce/assets/chevron-up.png "열기")를 클릭하여 세부 정보를 확장합니다.

   * 선택적 **[!UICONTROL Job Name]** 및/또는 선택적 **[!UICONTROL Job Description]**&#x200B;을(를) 입력하십시오.

1. **[!UICONTROL Post Now]**&#x200B;을(를) 클릭합니다.


>[!MORELIKETHIS]
>
>* [일괄 시트를 사용하여 캠페인 데이터 관리 정보](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-about.md)
>* [행 내에서 직접 설정 편집](/help/search-social-commerce/common-tasks/settings-edit-within-row.md)
>* [캠페인 관리](/help/search-social-commerce/campaign-management/campaigns/campaign-manage.md)
>* [광고 그룹 관리](/help/search-social-commerce/campaign-management/campaigns/ad-group-manage.md)
>* [키워드 관리](/help/search-social-commerce/campaign-management/campaigns/keyword-manage.md)
>* [광고 관리](/help/search-social-commerce/campaign-management/campaigns/ad-manage.md)
