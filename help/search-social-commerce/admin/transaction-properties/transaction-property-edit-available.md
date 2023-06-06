---
title: 관리 보기 및 보고서에서 사용할 수 있는 거래 속성 변경
description: 관리 보기 및 보고서에서 거래 속성을 사용할 수 있도록 하는 방법을 알아봅니다.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# 관리 보기 및 보고서에서 사용할 수 있는 거래 속성 변경

Adobe 광고가 다음을 추적할 때 [거래 속성](/help/search-social-commerce/glossary.md#s-t) 광고주의 경우 처음에는 포트폴리오 목표, 보고서 및 관리 보기에서 제외됩니다. 속성을 표시하려면 속성을 명시적으로 사용할 수 있도록 설정한 다음 선택적으로 표시되는 이름인 기본 표시 이름을 변경해야 합니다. 유일한 예외는 전환을에서 추적한다는 것입니다. [!DNL Google Ads], [!DNL Google Analytics], 및 [!DNL Microsoft® Advertising] 범용 이벤트 추적 태그는 자동으로 사용할 수 있고 표시됩니다.

마찬가지로 포트폴리오 목표, 보고서 및 관리 보기에서 속성을 숨길 수 있습니다. 이전에 표시된 속성을 숨기면 속성이 포함된 파생 지표에서 제거됩니다.

사용 가능한 속성 목록에서 광고주의 데이터에 액세스할 수 있는 각 사용자는 특정 속성을 선택하거나 생략하는 등 관리 보기 및 보고서에 대해 표시되는 속성을 사용자 지정할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Admin] >[!UICONTROL Transaction Properties]**.

   광고주를 위해 수집된 모든 트랜잭션 속성과 표시를 위해 지정된 다른 모든 이름이 나열됩니다.

1. (선택 사항) 목록을 필터링합니다.

   * 특정 등록 정보 이름 또는 표시 이름을 검색하려면 ![검색](/help/search-social-commerce/assets/search.png "검색")를 클릭하고 입력 필드에 단어 또는 문자열을 입력한 다음 **[!DNL Enter]** 키.

      첫 번째 글자 또는 마지막 세 글자와 같이 구문 내 어디에나 나타나는 문자열을 검색할 수 있지만 검색어는 검색되지 않습니다 [대/소문자 구분](/help/search-social-commerce/glossary.md#c-d).

   * 관리 보기 및 보고서에서 사용 가능으로 속성을 검색하려면 ![필터](/help/search-social-commerce/assets/filter.png "필터")을 클릭하고 필터를 선택합니다 **[!UICONTROL Show in UI and Reports]**. 다음 중 하나를 선택합니다. **[!UICONTROL Show]** (보고서 및 관리 보기에 포함할 수 있는 속성을 보려면) 또는 **[!UICONTROL Hide]** (보고서 및 관리 보기에서 사용할 수 없는 속성을 보려면).

1. 관리 보기 및 보고서에 사용할 수 있는 속성을 변경합니다.

   * 단일 속성을 표시하거나 숨기려면 **[!UICONTROL Show in UI and Reports]** 열 을 입력하여 설정을 변경할 수 있습니다.

   * 여러 속성을 표시하거나 숨기려면 다음을 수행합니다.

      1. 각 속성 옆에 있는 확인란을 선택합니다.

         여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md).&quot;

      1. 데이터 테이블 위의 도구 모음에서 ![표시](/help/search-social-commerce/assets/show.png "표시") 속성을 표시하거나 ![숨기기](/help/search-social-commerce/assets/hide.png "숨기기") 속성을 숨깁니다.

      1. (속성을 숨기려면) 확인 메시지에서 **[!UICONTROL Yes]** 속성을 포함하는 파생 지표에서 속성을 제거하는 등 속성을 숨깁니다.

1. (선택 사항) [열 머리글에 나타나는 이름 변경](transaction-property-edit-display-name.md) 모든 속성입니다.

   표시되는 각 속성의 기본 표시 이름은 검색된 데이터의 맞춤법에 따른 속성 이름입니다.

>[!NOTE]
>
>Adobe 광고에서 새 속성에 대한 데이터를 수집하는 경우 새 속성 — 다음에서 추적한 전환을 제외 [!DNL Google Ads], [!DNL Google Analytics], 및 [!DNL Microsoft® Advertising] 범용 이벤트 추적 태그 — 를 포함할 때까지 관리 보기 및 보고서에서 자동으로 제외됩니다. 추적한 새 전환 [!DNL Google Ads], [!DNL Google Analytics], 및 [!DNL Microsoft® Advertising] 범용 이벤트 추적 태그는 항상 자동으로 사용할 수 있습니다.

>[!MORELIKETHIS]
* [광고주의 거래 속성 관리 정보](transaction-property-about.md)
* [광고주에 대해 추적된 트랜잭션 속성 보기](transaction-property-view-tracked.md)
* [거래 속성에 대한 표시 이름 변경](transaction-property-edit-display-name.md)

