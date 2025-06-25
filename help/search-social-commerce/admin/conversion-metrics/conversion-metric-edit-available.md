---
title: 관리 보기 및 보고서에서 사용할 수 있는 전환 지표 변경
description: 관리 보기 및 보고서에서 사용 가능한 전환 지표를 만드는 방법을 알아봅니다.
feature: Conversions
exl-id: de3d288a-5fec-4479-92cf-7754390e21bb
source-git-commit: d0f1c413134a0868ddec79ded7672af316267edd
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 0%

---

# 관리 보기 및 보고서에서 사용할 수 있는 전환 지표 변경

Adobe Advertising이 광고주에 대한 [전환](/help/search-social-commerce/glossary.md#c-d) 지표를 추적하는 경우 처음에는 포트폴리오 목표, 보고서 및 관리 보기에서 제외됩니다. 전환 지표가 표시되도록 하려면 전환 지표를 명시적으로 사용할 수 있도록 한 다음 선택적으로 표시되는 이름인 기본 표시 이름을 변경해야 합니다. 유일한 예외는 [!DNL Google Ads], [!DNL Google Analytics] 및 [!DNL Microsoft Advertising] 유니버설 이벤트 추적 태그가 추적한 전환을 자동으로 사용할 수 있고 표시할 수 있다는 것입니다.

마찬가지로 포트폴리오 목표, 보고서 및 관리 보기에서 전환 지표를 숨길 수 있습니다. 이전에 표시되었던 전환 지표를 숨기면 전환 지표가 포함된 파생 지표에서 제거됩니다.

사용 가능한 전환 지표 목록에서 광고주의 데이터에 액세스할 수 있는 각 사용자는 특정 지표를 선택하거나 생략하는 등 관리 보기 및 보고서에 대해 표시되는 지표를 사용자 지정할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Search, Social, & Commerce]> [!UICONTROL Admin] >[!UICONTROL Conversions]**&#x200B;을(를) 클릭합니다.

   광고주를 위해 수집된 모든 전환 지표와 표시를 위해 지정된 다른 이름이 나열됩니다.

1. (선택 사항) 목록을 필터링합니다.

   * 특정 지표 이름이나 표시 이름을 검색하려면 ![검색](/help/search-social-commerce/assets/search.png "검색")을 클릭하고 입력 필드에 단어 또는 문자열을 입력한 다음 **[!DNL Enter]** 키를 누릅니다.

     구문 내의 어디에나 나타나는 문자열(예: 첫 번째 문자 또는 마지막 세 문자)을 검색할 수 있으며 검색어는 [대/소문자를 구분하지 않습니다](/help/search-social-commerce/glossary.md#c-d).

   * 관리 보기 및 보고서에서 가용성별로 전환 지표를 검색하려면 ![필터](/help/search-social-commerce/assets/filter.png "필터")를 클릭하고 필터 **[!UICONTROL Show in UI and Reports]**&#x200B;을(를) 선택하십시오. 그런 다음 **[!UICONTROL Show]**(보고서 및 관리 보기에 포함할 수 있는 전환 지표를 보려면) 또는 **[!UICONTROL Hide]**(보고서 및 관리 보기에 사용할 수 없는 전환 지표를 보려면)을 선택합니다.

1. 관리 보기 및 보고서에 사용할 수 있는 전환 지표를 변경합니다.

   * 단일 지표를 표시하거나 숨기려면 **[!UICONTROL Show in UI and Reports]** 열에서 스위치를 클릭하여 설정을 변경합니다.

   * 여러 지표를 표시하거나 숨기려면 다음을 수행합니다.

      1. 각 전환 지표 옆에 있는 확인란을 선택합니다.

         여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)&quot;을 참조하십시오.

      1. 데이터 테이블 위의 도구 모음에서 ![표시](/help/search-social-commerce/assets/show.png "표시")를 클릭하여 지표를 표시하거나 ![숨기기](/help/search-social-commerce/assets/hide.png "숨기기")을(를) 클릭하여 지표를 숨깁니다.

      1. (지표를 숨기려면) 확인 메시지에서 **[!UICONTROL Yes]**&#x200B;을(를) 클릭하여 지표가 포함된 파생 지표에서 지표를 제거하는 등 지표를 숨깁니다.

1. (선택 사항) [전환 지표에 대해 열 머리글에 나타나는 이름을 변경](conversion-metric-edit-display-name.md)합니다.

   표시되는 각 전환 지표의 기본 표시 이름은 검색된 데이터의 맞춤법에 따른 지표 이름입니다.

>[!NOTE]
>
>Adobe Advertising에서 새 전환 지표에 대한 데이터를 수집하는 경우 [!DNL Google Ads], [!DNL Google Analytics] 및 [!DNL Microsoft Advertising] 유니버설 이벤트 추적 태그에 의해 추적된 전환을 제외한 새 지표는 사용자가 포함할 때까지 관리 보기 및 보고서에서 자동으로 제외됩니다. [!DNL Google Ads], [!DNL Google Analytics] 및 [!DNL Microsoft Advertising] 유니버설 이벤트 추적 태그가 추적하는 새 전환은 항상 자동으로 사용할 수 있습니다.

>[!MORELIKETHIS]
>
>* [광고주의 전환 지표 관리 정보](conversion-metric-about.md)
>* [광고주에 대해 추적된 전환 지표를 봅니다](conversion-metric-view-tracked.md)
>* [전환 지표에 대한 표시 이름 변경](conversion-metric-edit-display-name.md)
