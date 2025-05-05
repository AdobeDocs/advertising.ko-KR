---
title: ' [!DNL Microsoft Advertising] 동적 리마케팅 대상자 관리'
description: ' [!DNL Microsoft Advertising] 동적 리마케팅 대상자를 만들고 관리하는 방법을 알아봅니다.'
exl-id: 52faab75-e723-4e59-aac6-b4d0c4c1cf60
feature: Search Campaign Management
source-git-commit: e517dd5f5fa283ff8a2f57728612937148889732
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# [!DNL Microsoft Advertising]개의 동적 리마케팅 대상자 관리

*[!DNL Microsoft Advertising]개의 계정만*

웹 페이지에서 검색 엔진의 JavaScript 전환 및 대상 추적 태그를 사용할 때 [!DNL Microsoft Advertising] 동적 리마케팅 대상을 만들 수 있습니다. 각 대상자는 사용자가 대상자를 구성하는 웹 페이지에 포함된 지정된 태그를 사용하여 만들어집니다. 동일한 추적 태그를 사용하여 여러 대상을 만들 수 있습니다. 기존 대상자에 대한 이름 및 데이터 소스를 변경하거나 기존 대상자를 삭제할 수도 있습니다.

동적 리마케팅 대상에는 대상 유형이 &quot;[!UICONTROL Dynamic Remarketing] \&lt;방문자 유형\>&quot;입니다(예: &quot;동적 리마케팅 과거 구매자&quot;).

동적 리마케팅 및 필요한 JavaScript 태그를 구현하는 방법에 대한 자세한 내용은 [[!DNL Microsoft Advertising] 동적 리마케팅에 대한 설명서](https://help.ads.microsoft.com/#apex/ads/en/56910)를 참조하십시오.

## 동적 리마케팅 대상자 만들기

>[!NOTE]
>
>[!DNL Microsoft Advertising] 계정의 경우 JavaScript 태그에 [제품 ID 및 페이지 유형 매개 변수](https://help.ads.microsoft.com/#apex/ads/en/56910/1/#exp85)가 포함되어야 합니다.

1. 대상자를 만들 웹 페이지에 포함된 [!DNL Microsoft Advertising] UET(범용 이벤트 추적) 태그의 이름을 식별합니다.

   이후 단계에서 태그 이름이 필요합니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다. 하위 메뉴에서 **[!UICONTROL Live]> [!UICONTROL Audiences] >[!UICONTROL Library]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위의 도구 모음에서 ![만들기](/help/search-social-commerce/assets/add.png "만들기")를 클릭합니다.

1. 광고 네트워크 및 계정 이름을 선택한 다음 **[!UICONTROL Continue]**&#x200B;을(를) 클릭합니다.

1. 대상 정보를 지정합니다.

   1. **[!UICONTROL Data Source]** 메뉴에서 **[!UICONTROL Dynamic Remarketing List]**&#x200B;을(를) 선택합니다.

   1. **[!UICONTROL Audience Name]** 입력.

   1. 검색 엔진 계정에 대해 사용 가능한 모든 태그 목록에서 사용자가 대상자를 구성하는 웹 페이지에 포함된 [!DNL Microsoft Advertising] UET 태그의 이름을 선택합니다.

   1. 관련 웹 페이지의 방문자 작업을 기반으로 하는 대상의 방문자 유형을 선택하십시오. *[!UICONTROL General Visitors]*, *[!UICONTROL Product Searchers]*, *[!UICONTROL Product Viewers]*, *[!UICONTROL Past Buyers]* 또는 *[!UICONTROL Shopping Cart Abandoners]*.

   1. 사용자 쿠키가 대상에 있는 일 수인 **[!UICONTROL Membership Days]**&#x200B;을(를) 지정합니다. 값의 범위는 1~180입니다.

      광고가 사용자와 관련이 있을 것으로 예상되는 시간을 사용합니다.

1. **[!UICONTROL Post]**&#x200B;을(를) 클릭합니다.

>[!NOTE]
>
>[!DNL Microsoft Advertising] 동적 리마케팅 목록에 사용자가 300명 이상 포함되면 타깃팅할 수 있습니다.

## 동적 리마케팅 대상자 편집

[!DNL Microsoft Advertising] 동적 리마케팅 대상자의 이름과 데이터 원본을 변경할 수 있습니다. [!UICONTROL Membership Days] 설정의 값을 편집할 수 없습니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다. 하위 메뉴에서 **[!UICONTROL Live]> [!UICONTROL Audiences] >[!UICONTROL Library]**&#x200B;을(를) 클릭합니다.

1. 편집할 대상 옆에 있는 확인란을 선택합니다.

1. 데이터 테이블 위의 도구 모음에서 ![편집](/help/search-social-commerce/assets/edit.png "편집")을 클릭합니다.

1. 대상자 정보 편집:

   1. **[!UICONTROL Data Source]** 섹션에서 ![편집](/help/search-social-commerce/assets/edit.png "편집")을 클릭합니다.

   1. (선택 사항) **[!UICONTROL Audience Name]**&#x200B;을(를) 변경합니다.

   1. (선택 사항) 광고 네트워크 계정에 대해 사용 가능한 모든 태그 목록에서 사용자가 대상자를 구성하는 웹 페이지에 포함된 [!DNL Microsoft Advertising] UET 태그의 이름을 변경합니다.

   1. (선택 사항) 관련 웹 페이지의 방문자 작업을 기반으로 하는 대상의 방문자 유형을 변경합니다. *[!UICONTROL General Visitors]*, *[!UICONTROL Product Searchers]*, *[!UICONTROL Product Viewers]*, *[!UICONTROL Past Buyers]* 또는 *[!UICONTROL Shopping Cart Abandoners]*.

   1. **[!UICONTROL Post]**&#x200B;을(를) 클릭합니다.

## 동적 리마케팅 대상자 삭제

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다. 하위 메뉴에서 **[!UICONTROL Live]> [!UICONTROL Audiences] >[!UICONTROL Library]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 특정 대상을 포함하도록 목록을 필터링합니다.

1. 삭제할 각 대상 옆에 있는 확인란을 선택합니다.

   여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)&quot;을 참조하십시오.

1. 확인 메시지에서 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [대상자 정보](audience-about.md)
>* [고객 일치 대상자 만들기 [!DNL Google Ads] 출처 [!DNL Adobe] 대상자](google-audience-from-adobe-audience.md)
>* [Adobe Campaign 전자 메일 목록에서 고객 일치 대상 만들기 [!DNL Google Ads] 2&rbrace;](google-audience-from-campaign-email-list.md)
>* [고객 데이터 목록을 사용하여 고객 일치 대상 관리](audience-from-customer-data-list.md)
