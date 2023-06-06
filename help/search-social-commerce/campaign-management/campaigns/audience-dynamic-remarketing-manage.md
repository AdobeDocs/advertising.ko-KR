---
title: 관리 [!DNL Microsoft Advertising] 동적 리마케팅 대상
description: 생성 및 관리 방법 알아보기 [!DNL Microsoft Advertising] 동적 리마케팅 대상자입니다.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---

# 관리 [!DNL Microsoft Advertising] 동적 리마케팅 대상

*[!DNL Microsoft Advertising]계정만*

다음을 만들 수 있습니다. [!DNL Microsoft Advertising] 웹 페이지에서 검색 엔진의 JavaScript 전환 및 대상 추적 태그를 사용할 때의 동적 리마케팅 대상. 각 대상자는 사용자가 대상자를 구성할 웹 페이지에 포함된 지정된 태그를 사용하여 만들어집니다. 동일한 추적 태그를 사용하여 여러 대상을 만들 수 있습니다. 기존 대상자에 대한 이름 및 데이터 소스를 변경하거나 기존 대상자를 삭제할 수도 있습니다.

동적 리마케팅 대상에는 대상 유형 이 있습니다.[!UICONTROL Dynamic Remarketing] \&lt;visitor type=&quot;&quot;>&quot; (예: &quot;동적 리마케팅 과거 구매자&quot;).

동적 리마케팅 및 필요한 JavaScript 태그를 구현하는 방법에 대한 자세한 내용은 [[!DNL Microsoft Advertising] 동적 리마케팅에 대한 설명서](https://help.ads.microsoft.com/#apex/ads/en/56910).

## 동적 리마케팅 대상자 만들기

>[!NOTE]
>
>대상 [!DNL Microsoft Advertising] 계정, JavaScript 태그에는 [제품 ID 및 페이지 유형 매개 변수](https://help.ads.microsoft.com/#apex/ads/en/56910/1/#exp85).

1. 의 이름 식별 [!DNL Microsoft Advertising] 대상을 만들 웹 페이지에 포함된 UET(범용 이벤트 추적) 태그입니다.

   이후 단계에서 태그 이름이 필요합니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**. 하위 메뉴에서 **[!UICONTROL Live]> [!UICONTROL Audiences] >[!UICONTROL Library]**.

1. 데이터 테이블 위의 도구 모음에서 ![만들기](/help/search-social-commerce/assets/add.png "만들기").

1. 광고 네트워크와 계정 이름을 선택한 다음 **[!UICONTROL Continue]**.

1. 대상 정보를 지정합니다.

   1. 다음에서 **[!UICONTROL Data Source]** 메뉴, 선택 **[!UICONTROL Dynamic Remarketing List]**.

   1. 다음을 입력합니다. **[!UICONTROL Audience Name]**.

   1. 검색 엔진 계정에 대해 사용 가능한 모든 태그 목록에서 [!DNL Microsoft Advertising] 사용자가 대상을 구성할 웹 페이지에 포함된 UET 태그입니다.

   1. 관련 웹 페이지의 방문자 작업을 기반으로 하는 대상에 대한 방문자 유형을 선택합니다. *[!UICONTROL General Visitors]*, *[!UICONTROL Product Searchers]*, *[!UICONTROL Product Viewers]*, *[!UICONTROL Past Buyers]*, 또는 *[!UICONTROL Shopping Cart Abandoners]*.

   1. 의 수를 지정합니다. **[!UICONTROL Membership Days]**: 사용자 쿠키가 대상에 있는 일 수입니다. 값의 범위는 1~180입니다.

      광고가 사용자와 관련이 있을 것으로 예상되는 시간을 사용합니다.

1. 클릭 **[!UICONTROL Post]**.

>[!NOTE]
>
>사용자 [!DNL Microsoft Advertising] 동적 리마케팅 목록에 최소 300명의 사용자가 포함되면 타겟팅할 수 있습니다.

## 동적 리마케팅 대상자 편집

의 이름과 데이터 소스를 변경할 수 있습니다. [!DNL Microsoft Advertising] 동적 리마케팅 대상자입니다. 의 값은 편집할 수 없습니다. [!UICONTROL Membership Days] 설정.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**. 하위 메뉴에서 **[!UICONTROL Live]> [!UICONTROL Audiences] >[!UICONTROL Library]**.

1. 편집할 대상 옆에 있는 확인란을 선택합니다.

1. 데이터 테이블 위의 도구 모음에서 ![편집](/help/search-social-commerce/assets/edit.png "편집").

1. 대상자 정보 편집:

   1. 다음에서 **[!UICONTROL Data Source]** 섹션, 클릭 ![편집](/help/search-social-commerce/assets/edit.png "편집").

   1. (선택 사항) **[!UICONTROL Audience Name]**.

   1. (선택 사항) 광고 네트워크 계정에 사용할 수 있는 모든 태그 목록에서 의 이름을 변경합니다. [!DNL Microsoft Advertising] 사용자가 대상을 구성할 웹 페이지에 포함된 UET 태그입니다.

   1. (선택 사항) 관련 웹 페이지에 대한 방문자 작업을 기반으로 하는 대상의 방문자 유형을 변경합니다. *[!UICONTROL General Visitors]*, *[!UICONTROL Product Searchers]*, *[!UICONTROL Product Viewers]*, *[!UICONTROL Past Buyers]*, 또는 *[!UICONTROL Shopping Cart Abandoners]*.

   1. 클릭 **[!UICONTROL Post]**.

## 동적 리마케팅 대상자 삭제

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**. 하위 메뉴에서 **[!UICONTROL Live]> [!UICONTROL Audiences] >[!UICONTROL Library]**.

1. (선택 사항) 특정 대상을 포함하도록 목록을 필터링합니다.

1. 삭제할 각 대상 옆에 있는 확인란을 선택합니다.

   여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md).&quot;

1. 확인 메시지에서 다음을 클릭합니다. **[!UICONTROL Delete]**.

>[!MORELIKETHIS]
>
>* [대상자 기본 정보](audience-about.md)
>* [만들기 [!DNL Google Ads] 의 고객 일치 대상 [!DNL Adobe] 대상](google-audience-from-adobe-audience.md)
>* [만들기 [!DNL Google Ads] Adobe Campaign 이메일 목록의 고객 일치 대상](google-audience-from-campaign-email-list.md)
>* [고객 데이터 목록을 사용하여 고객 일치 대상 관리](audience-from-customer-data-list.md)

