---
title: 부정적인 키워드 만들기
description: 검색 캠페인 및 광고 그룹에 대한 부정적인 키워드를 만드는 방법을 알아봅니다.
exl-id: afe786bf-eda8-4590-b471-3fb696c420de
feature: Search Campaign Management
source-git-commit: d0f1c413134a0868ddec79ded7672af316267edd
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# 부정적인 키워드 만들기

*[!DNL Google Ads], [!DNL Microsoft Advertising], [!DNL Yahoo! Japan Ads] 및 기존 [!DNL Baidu] 계정만*

검색 또는 디스플레이/기본 네트워크를 대상으로 하는 검색 광고 그룹 또는 캠페인에 대해 부정적인 키워드를 만들 수 있습니다. 부정적인 키워드는 광고를 트리거하지 않습니다.

>[!NOTE]
>[광고 그룹 설정](/help/search-social-commerce/campaign-management/campaigns/ad-group-manage.md) 및 [캠페인 설정](/help/search-social-commerce/campaign-management/campaigns/campaign-manage.md)에서 부정적인 키워드를 만들고 편집할 수도 있습니다.

>[!TIP]
>한 번에 여러 개의 부정적인 키워드를 만들려면 [캠페인 일괄 시트](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-about.md)를 사용하십시오.

1. 메인 메뉴에서 **[!UICONTROL Search, Social, & Commerce]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다. 하위 메뉴에서 **[!UICONTROL Live]> [!UICONTROL Keywords] >[!UICONTROL Negatives]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위의 도구 모음에서 ![만들기](/help/search-social-commerce/assets/add.png "만들기")를 클릭한 다음 **[!UICONTROL Campaign]**&#x200B;을(를) 클릭하여 캠페인 수준의 부정적인 키워드를 만들거나 **[!UICONTROL Ad Group]**&#x200B;을(를) 클릭하여 광고 그룹 수준의 부정적인 키워드를 만듭니다.

1. 광고 네트워크, 계정, 캠페인 및 (해당되는 경우) 광고 그룹을 선택한 다음 **[!UICONTROL Continue]**&#x200B;을(를) 클릭합니다.

1. 음의 키워드를 입력합니다. 빼기 기호(`-`) 없이 다음 구문을 사용하십시오.

   * 음수 브로드 일치: `keyword`([!DNL Microsoft Advertising]에서 지원되지 않음)

   * 음수 구 일치: `"keyword"`

   * 정확히 일치하는 음수: `[keyword]`

   여러 값을 쉼표로 구분하거나 별도의 라인에 입력합니다. 한 번의 작업으로 최대 2000개의 부정적인 키워드를 입력하거나 붙여넣을 수 있습니다. 다음 요구 사항 및 제한 사항을 참조하십시오.

   * 최대 문자 길이: [!DNL Baidu]: 1바이트 또는 15 2바이트; [!DNL Microsoft Advertising]: 100 1바이트 또는 50 2바이트; [!DNL Google Ads] 및 [!DNL Yahoo! Japan Ads]: 80 1바이트 또는 40 2바이트.

   * [!DNL Baidu]에서는 광고 그룹당 키워드당 일치 유형을 하나만 사용할 수 있습니다. 예를 들어 광고 그룹 1은 `"keyword"`과(와) `[keyword]`을(를) 모두 포함할 수 없습니다.

   * [!DNL Google Ads]: 각 키워드는 10단어 이하로 구성될 수 있으며 문자, 숫자 및 다음 특수 문자만 포함할 수 있습니다. 공백 `# $ & _ - " [ ] ' + . / :`

   * [!DNL Yandex]: 각 키워드는 정지어를 제외하고 최대 7개의 단어를 사용할 수 있습니다. 각 [!DNL Yandex ad group]에는 최대 200개의 키워드가 포함될 수 있습니다.

1. **[!UICONTROL Post]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [키워드 정보](keyword-about.md)
>* [바인딩 가능한 키워드 관리](keyword-manage.md)
>* [키워드 및 부정적 키워드의 상태를 변경합니다](keyword-status-edit.md)
