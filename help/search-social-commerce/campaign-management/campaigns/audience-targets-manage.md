---
title: 캠페인 및 광고 그룹에 대한 대상자 타겟 관리
description: 에 대한 대상 타겟을 구성 및 관리하는 방법을 알아봅니다. [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 캠페인 및 광고 그룹.
exl-id: 9a496d15-082d-44e1-a0a3-71356e24b932
feature: Search Campaign Management
source-git-commit: 67fe8581832dc0762d62908d01672e53cc95b847
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# 다음에 대한 대상자 타겟 관리 [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 캠페인 및 광고 그룹

*[!DNL Google Ads]및 [!DNL Microsoft Advertising] 전용*

[!DNL Google Ads] 캠페인 및 광고 그룹 및 [!DNL Microsoft Advertising] 광고 그룹은 동일한 광고 네트워크에서 특정 대상을 타깃팅할 수 있습니다. 광고 네트워크는 대상이 타겟팅되어야 하는 대상의 크기를 결정합니다.

>[!NOTE]
>
>제외는 항상 포함/대상을 재정의합니다.

대상자 타겟을 구성하고, 대상자 타겟에 대한 입찰 수정자를 편집하고, 대상자 타겟의 상태를 변경할 수 있습니다.

## 대상자 타겟 구성

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**. 하위 메뉴에서 **[!UICONTROL Live]> [!UICONTROL Audiences] >[!UICONTROL Targets]**.

1. 데이터 테이블 위의 도구 모음에서 ![만들기](/help/search-social-commerce/assets/add.png "만들기").

1. 광고 네트워크와 계정 이름을 선택한 다음 **[!UICONTROL Continue]**.

1. 특정 캠페인 및 광고 그룹에 대한 대상자 타겟을 구성합니다.

   1. 지정된 광고 네트워크에 적용할 대상을 선택합니다.

      필요한 경우 최소 3자의 특정 텍스트 문자열이 포함된 대상을 검색할 수 있습니다. 일치하는 대상을 보려면 다음을 클릭하십시오. **[!UICONTROL Include]** 을 눌러 선택합니다.

      [!DNL Google Ads] 고객 일치 대상은 검색 및 쇼핑 캠페인에만 사용할 수 있습니다.

   1. 대상을 지정합니다.

      1. (선택 사항) 캠페인을 확장하려면 하위 광고 그룹을 선택하고 캠페인 이름을 클릭합니다.

      1. (선택 사항) 캠페인 목록 또는 광고 그룹 목록을 이름에 포함된 텍스트 문자열로 필터링하려면 다음을 클릭하십시오. ![필터](/help/search-social-commerce/assets/filter.png "필터") 를 입력하거나 텍스트 문자열을 입력 필드에 붙여넣은 다음 **[!UICONTROL Enter]** 키.

      1. 파란색 확인 표시( )가 표시되도록 인접한 빈 원을 클릭하여 지정된 광고 네트워크에 대한 각 캠페인 및 광고 그룹 대상을 지정합니다.![선택](/help/search-social-commerce/assets/include.png "선택"))가 표시됩니다.

      상위 캠페인과 하위 광고 그룹(자동으로 타겟을 사용)에 대한 타겟을 모두 구성할 수는 없습니다.

1. 클릭 **[!UICONTROL Post]**.

1. (선택 사항) 다음 방법 중 하나로 타겟의 입찰 조정을 설정합니다. [!UICONTROL Targets] 보기:

   * 을(를) 클릭합니다. **[!UICONTROL Bid Adjustment]** 열을 만들고 값을 입력합니다.

   * 대상 행 옆에 있는 확인란을 선택합니다. 도구 모음에서 를 클릭합니다 ![편집](/help/search-social-commerce/assets/edit.png "편집")를 클릭하고 입찰 수정자를 입력한 다음 을 클릭합니다. **[!UICONTROL Post]**.

   값은 다음과 같습니다.

   * *0%:* 이 대상자의 광고 입찰을 조정하지 않습니다.

   * /[*-90% ~ 900%의 기타 값*/]: 이 대상자의 광고 입찰을 늘리거나 줄입니다. 예를 들어 키워드 수준의 입찰이 1 USD이고 특정 대상 타겟에 대한 입찰 조정이 50%인 경우 해당 대상에 대한 입찰은 1.50 USD로 증가합니다.

## 대상자 타겟에 대한 입찰 수정자 편집

마켓 내 대상을 제외한 모든 대상 유형에 대해 입찰 수정자 및 대상 타겟의 상태를 변경할 수 있습니다.

>[!NOTE]
>
>상위 캠페인이 CPC 입찰 전략을 사용하고 대상자 타겟에 대한 입찰 조정 값을 자동 최적화하도록 구성된 포트폴리오에 있는 경우 검색, 소셜 및 Commerce은 입찰 수정자를 자동으로 최적화합니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**. 하위 메뉴에서 **[!UICONTROL Live]> [!UICONTROL Audiences] >[!UICONTROL Targets]**.

1. 다음 중 하나를 수행합니다.

   * 하나의 대상에 대한 입찰 수정자를 편집하려면 **[!UICONTROL Bid Adjustment]** 입찰 조정을 열어서 편집합니다.

   * 한 개 이상의 대상에 대한 입찰 수정자를 편집하려면 다음을 수행합니다.

      1. 편집할 각 대상 옆의 확인란을 선택합니다.

         여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md).&quot;

      1. 데이터 테이블 위의 도구 모음에서 ![편집](/help/search-social-commerce/assets/edit.png "편집").

      1. 편집 **[!UICONTROL Bid Modifier]** 및/또는 **[!UICONTROL Status]** 필드.

         의 경우 [!UICONTROL Bid Modifier] 필드에는 기존 값을 지정된 값으로 변경하거나, 제한을 두고 지정된 백분율 또는 통화 금액만큼 금액을 늘리거나 줄이는 옵션이 있습니다.

         설정된 값의 경우 값은 다음을 포함할 수 있습니다.

         * *0%:* 이 대상자의 광고 입찰을 조정하지 않습니다.

         * /[*-90% ~ 900%의 기타 값*/]: 이 대상자의 광고 입찰을 늘리거나 줄입니다. 예를 들어 키워드 수준의 입찰이 1 USD이고 특정 대상 타겟에 대한 입찰 조정이 50%인 경우 해당 대상에 대한 입찰은 1.50 USD로 증가합니다.

         여러 타겟의 경우 변경 사항이 선택한 모든 타겟에 적용됩니다.

      1. (선택 사항) **[!UICONTROL Additional Details]** 프로젝트 이름과 설명을 입력합니다(선택적).

      1. 클릭 **[!UICONTROL Post]**.

## 대상자 타겟의 상태 변경

활성 대상 타겟을 일시 중지하여 입찰을 비활성화할 수 있습니다. 나중에 상태를 다시 활성으로 변경하여 입찰을 다시 시작할 수 있습니다.

활성 또는 일시 중지된 검색 대상자 타겟을 삭제할 수도 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**. 하위 메뉴에서 **[!UICONTROL Live]> [!UICONTROL Audiences] >[!UICONTROL Targets]**.

1. (선택 사항) 특정 대상 타겟을 포함하도록 목록을 필터링합니다.

1. 상태를 변경할 각 대상자 타겟 옆의 확인란을 선택합니다.

   여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md).&quot;

1. 도구 모음에서 상태 단추 를 클릭합니다.

   * 행을 활성화하려면 ![활성화](/help/search-social-commerce/assets/activate.png "활성화").

   * 행을 일시 중지하려면 ![일시 중지](/help/search-social-commerce/assets/pause.png "일시 중지").

   * 행을 삭제하려면 ![추가 작업](/help/search-social-commerce/assets/more.png "추가 작업") 및 선택 **[!UICONTROL Delete]**. 확인 메시지에서 다음을 클릭합니다. **[!UICONTROL Delete]**.

>[!MORELIKETHIS]
>
>* [대상자 기본 정보](audience-about.md)
>* [캠페인 및 광고 그룹에 대한 대상자 제외 관리](/help/search-social-commerce/campaign-management/campaigns/audience-exclusions-manage.md)
