---
title: 쇼핑 제품 그룹 관리
description: 쇼핑 제품 그룹을 생성, 편집 및 삭제하고, Google 광고 및 Microsoft Advertising에 대한 제품 그룹 설정을 참조하는 방법에 대해 알아봅니다.
feature: Search Campaign Management
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2:
  - id: aed5e38a-3e62-42fa-8d16-cd080729b2a0
subfeature_v2:
  - id: f3d33161-c519-436e-bbbd-730ba428736b
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: c074f430583e2d320eb4d47b4fc956c1822bd04a
workflow-type: tm+mt
source-wordcount: 2337
ht-degree: 0%

---


# 쇼핑 제품 그룹 관리

*[!DNL Google Ads]및 [!DNL Microsoft Advertising] 쇼핑 캠페인만*

[!UICONTROL Assets] > [!UICONTROL Shopping]의 [!UICONTROL Product Groups] 보기에서 제품 그룹을 만들고 관리할 수 있습니다.

[의 [!UICONTROL Product Group Report]](/help/search-social-commerce/new-ui/reports/management/basic-advanced/product-group-report.md)에서 제품 그룹에 대한 데이터를 볼 수 있습니다.

## 제품 그룹이란?

쇼핑 캠페인에서 키워드가 아닌 제품 그룹은 쇼핑 광고가 표시되는 머천트 센터 계정의 제품을 결정합니다. 각 제품 그룹은 단일 제품 속성(예: 카테고리, 제품 유형, 브랜드, 조건, 제품 ID 또는 사용자 정의 레이블)을 기반으로 하며 일치하는 모든 제품에 대해 동일한 입찰을 사용합니다. 각 그룹의 제품에 대한 입찰을 포함하거나 제외할 수 있습니다.

광고 그룹 수준에서 제품 그룹을 구성하여 머천트 센터 계정의 제품 중 광고 그룹의 쇼핑 광고에 나타나는 제품을 결정합니다. 광고 그룹에 광고 엔티티가 포함되지 않은 경우에도 광고 네트워크에는 여전히 제품에 대한 광고가 표시됩니다.

동일한 제품이 둘 이상의 캠페인에 포함된 경우 광고 네트워크는 먼저 캠페인 우선 순위를 사용하여 광고 경매에 적합한 캠페인(및 관련 입찰)을 결정합니다. 모든 캠페인이 동일한 우선 순위를 갖는 경우 입찰이 가장 높은 캠페인이 적격입니다.

[!DNL Google] 쇼핑 캠페인 및 광고에 대한 자세한 내용은 &quot;[&#128279;](/help/search-social-commerce/campaign-management/special-workflows/google-shopping-campaigns.md)쇼핑 캠페인 구현 [!DNL Google Ads] 3&rbrace;&quot; 및 [Google 광고 설명서](https://support.google.com/google-ads/answer/3455481?visit_id=638205553638977410-2592024034&rd=1)를 참조하십시오. &#x200B;[!DNL Microsoft] 쇼핑 캠페인에 대한 자세한 내용은 &quot;[&#128279;](/help/search-social-commerce/campaign-management/special-workflows/microsoft-shopping-campaigns.md)쇼핑 캠페인 구현 [!DNL Microsoft Advertising] 3&rbrace;&quot; 및 [[!DNL Microsoft Advertising] 설명서](https://help.bingads.microsoft.com/#apex/3/en/50903/1-500)를 참조하세요.

>[!NOTE]
>
>성과 최대 캠페인에 그룹을 나열하는 [!DNL Google Ads]에 대해서는 지원을 사용할 수 없습니다. 목록 그룹에 대한 데이터를 관리하고 보려면 [!DNL Google Ads] 편집기를 사용하십시오.

### 제품 그룹 계층

광고 그룹에 대한 특정 특성을 사용하여 제품 그룹을 만들려면 먼저 &quot;[!UICONTROL All Products]&quot;이라는 포괄적 제품 그룹을 만들어야 합니다. 이 상위 제품 그룹에서 제품 하위 집합에 대한 하위 제품 그룹을 생성할 수 있으며 하위 제품 그룹에서 손자를 생성할 수 있습니다. 광고 그룹에 대해 첫 번째 하위 제품 그룹을 만들면 기본 광고 그룹 입찰을 사용하여 &quot;[!UICONTROL Everything Else]&quot;이라는 다른 제품 그룹이 자동으로 만들어집니다. 제품 그룹을 더 추가하면 &quot;[!UICONTROL Everything Else]&quot; 그룹이 다른 제품 그룹에 없는 모든 제품을 구성하도록 적절하게 조정됩니다.

광고 그룹 내에서 입찰에서 포함하거나 제외할 제품 그룹을 최대 7개까지 만들 수 있습니다(&quot;[!UICONTROL All Products]&quot; 제외). 하나 이상의 제품 그룹은 각 수준에서 동일한 특성을 타깃팅합니다(예: 한 제품 그룹의 경우 [!UICONTROL Brand]=Acme, 같은 수준의 다른 제품 그룹의 경우 [!UICONTROL Brand]=AcmePlus). 상위 제품군을 세부분류라고 하며, 세부분류의 가장 낮은 수준을 단위라고 한다. 단위 수준에서 입찰 및 추적 템플릿을 설정하거나 입찰을 완전히 제외할 수 있습니다. 광고 그룹에 대한 전체 활성 제품 그룹 세트가 계층적으로 적용되어 적격 제품을 결정합니다. 예를 들어 [!UICONTROL All Products]을(를) [!UICONTROL Brand]=AcmeBasic 및 [!UICONTROL Brand]=AcmePlus로 세분한 다음 각 제품 그룹을 [!UICONTROL Condition]=New로 세분하고 입찰을 설정하면 AcmeBasic 및 AcmePlus 브랜드가 있는 새 제품만 광고하거나 광고에서 제외할 수 있습니다.

![제품 그룹 집합의 예](/help/search-social-commerce/assets/product-group-list-new.png "제품 그룹 집합의 예")

![제품 그룹 계층 구조 예](/help/search-social-commerce/assets/product-group-tree-new.png "제품 그룹 계층 구조 예")

### 제품 필터 {#product-filters}

<!-- I should be able to point to help in GGL and MS -->

[!DNL Google Ads] 도움말 &quot;[제품 그룹으로 쇼핑 캠페인 관리](https://support.google.com/google-ads/answer/6275317)&quot; 및 [!DNL Microsoft Advertising] 도움말 &quot;[제품 그룹 이해 및 사용](https://help.ads.microsoft.com/#apex/bae/en/56782)&quot;도 참조하세요.

| 쇼핑 네트워크 | 제품 Dimension | 속성 | 메모 |
|----|----|----|----|
| [!DNL Google Ads], [!DNL Microsoft Advertising] | [!DNL Google Ads]: [!UICONTROL Category=]<br><br>Microsoft: [!UICONTROL Category 1=] ~ [!UICONTROL Category 5=] | \[범주 ID\] | — |
| [!DNL Google Ads], [!DNL Microsoft Advertising] | [!UICONTROL Brand=] | \[브랜드\] | — |
| [!DNL Google Ads], [!DNL Microsoft Advertising] | [!UICONTROL Item ID=] | \[항목 ID\] | — |
| [!DNL Google Ads], [!DNL Microsoft Advertising] | [!UICONTROL Condition] | [!UICONTROL New], [!UICONTROL Used], [!UICONTROL Refurbished], [!UICONTROL Unknown] | — |
| [!DNL Google Ads], [!DNL Microsoft Advertising] | [!DNL Google Ads]: [!UICONTROL Product Type (1st level)=] - [!UICONTROL Product Type (5th level)=]<br><br>[!DNL Microsoft]: [!UICONTROL Product Type=] | \[제품 유형\] | — |
| [!DNL Google Ads], [!DNL Microsoft Advertising] | [!UICONTROL Custom Label 0=] - [!UICONTROL Custom Label 4=] | \[사용자 지정 레이블의 속성\] | — |
| [!DNL Google Ads] | 채널= | [!UICONTROL Local], [!UICONTROL Online] | 로컬 제품 또는 온라인 제품에 대한 광고만 표시하려면 <br><br><b>참고:</b> 로컬 제품에 대한 광고를 만들려면 &quot;로컬 인벤토리 광고&quot; 옵션을 사용하도록 설정해야 하며 [!DNL Google Merchant Center]을(를) 사용하여 로컬 쇼핑 프로그램에 참여해야 합니다. |
| [!DNL Google Ads] | [!UICONTROL ChannelExclusivity=] | [!UICONTROL SingleChannel], [!UICONTROL MultiChannel] | 단일 채널에만 사용 가능한(로컬에만 사용 또는 온라인에만 사용) 또는 여러 채널(로컬과 온라인 모두 사용)에 사용할 수 있는 제품에 대한 광고를 표시할지 여부. |

## [!UICONTROL Product Groups] 보기

[!UICONTROL Assets] > [!UICONTROL Shopping] 보기의 [!UICONTROL Product Groups] 보기에는 선택한 광고주 계정에 대해 필터링된 보기의 모든 제품 그룹이 나열됩니다. 제품 그룹을 만들고 관리할 수도 있습니다.

### 사용 가능한 작업 <!-- Go through all -->

* [&quot;[!UICONTROL All Products]&quot; 제품 그룹 만들기](#product-group-create-all-products)

* [기존 제품 그룹에 하위 제품 그룹 노드 만들기](#node-add)

* 제품 그룹 노드에 대한 설정을 편집합니다.

  * [모든 설정 편집](#node-edit)

  * [[!UICONTROL Tracking Template]만 편집](#node-edit-tracking-template)

  * [[!UICONTROL Max CPC]만 편집](#node-edit-maxcpc)

* [제품 그룹 노드 삭제](#node-delete)

* 제품 그룹에 [제약 조건 할당](#constraint-assign) 및 제품 그룹에서 [제약 조건 제거](#constraint-unassign)

* [제품 그룹에 레이블 분류를 할당](#classification-values-assign)하고 제품 그룹에서 [레이블 분류를 제거](#classification-values-remove)합니다.

>[!NOTE]
>
>[일괄 시트 파일](/help/search-social-commerce/new-ui/set-up/bulksheets/about.md)을 업로드하고 광고 네트워크에 게시하여 한 번에 많은 양의 제품 그룹 데이터(레이블 및 제한 할당 포함)를 만들고 편집할 수 있습니다.

## &quot;[!UICONTROL All Products]&quot; 제품 그룹 만들기 {#product-group-create-all-products}

특정 특성을 사용하여 제품 그룹을 만들려면 먼저 &quot;[!UICONTROL All Products]&quot;이라는 모든 포함 제품 그룹을 만들어야 합니다. 각 광고 그룹에는 하나의 &quot;[!UICONTROL All Products]&quot; 그룹만 있을 수 있습니다.

>[!TIP]
>
>한 번에 많은 계정 구성 요소를 만들려면 [캠페인 일괄 시트](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-about.md)를 사용하십시오.

1. 메인 메뉴에서 **[!UICONTROL Assets]>[!UICONTROL Shopping]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL Create Product Group]**&#x200B;을(를) 클릭합니다.

1. 광고 네트워크, 계정, 캠페인 및 광고 그룹을 선택한 다음 **[!UICONTROL Continue]**&#x200B;을(를) 클릭합니다.

1. [Google Ads 제품 그룹 설정](#google-ads-product-group-settings) 또는 [Microsoft Advertising 제품 그룹 설정](#microsoft-advertising-product-group-settings)을 지정하십시오.

1. **[!UICONTROL Review and Save]**&#x200B;을(를) 클릭합니다.

1. 필요한 경우 ![편집](/help/search-social-commerce/assets/edit-new.png "편집")을 클릭하고 [Google Ads 제품 그룹 설정](#google-ads-product-group-settings) 또는 [Microsoft Advertising 제품 그룹 설정](#microsoft-advertising-product-group-settings)을 변경합니다.

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

## 기존 제품 그룹에 하위 제품 그룹 노드 만들기 {#product-group-create-child}

광고 그룹에 대해 하나 이상의 모든 포함 &quot;[!UICONTROL All Products]&quot; 그룹을 만든 후에는 입찰에서 포함하거나 제외할 제품 하위 집합에 대한 하위 제품 그룹 노드를 만들 수 있습니다. 하나 이상의 제품 그룹은 각 수준에서 동일한 특성을 타깃팅합니다(예: 한 제품 그룹의 경우 [!UICONTROL Brand]=Acme, 같은 수준의 다른 제품 그룹의 경우 [!UICONTROL Brand]=AcmePlus). &quot;[!UICONTROL All Products]&quot;을(를) 포함하지 않고 최대 7개의 하위 제품 그룹 노드 수준을 만들 수 있습니다.

>[!NOTE]
>
>&quot;[!UICONTROL Everything Else]&quot; 제품 그룹에 대해 하위 제품 그룹을 만들 수 없습니다.

1. 메인 메뉴에서 **[!UICONTROL Assets]>[!UICONTROL Shopping]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 트리 보기에서 제품 그룹 및 하위 제품 그룹 노드를 보려면 커서를 제품 그룹 이름 위에 놓고 **[!UICONTROL ...]>[!UICONTROL Tree View]**&#x200B;을(를) 클릭합니다.

1. 제품 그룹 이름 위에 커서를 놓고 **[!UICONTROL ...]>[!UICONTROL + Add Node]**&#x200B;을(를) 클릭합니다.

1. [Google Ads 제품 그룹 설정](#google-ads-product-group-settings) 또는 [Microsoft Advertising 제품 그룹 설정](#microsoft-advertising-product-group-settings)을 지정하십시오.

1. **[!UICONTROL Center]**&#x200B;을(를) 클릭합니다.

## 제품 그룹 노드에 대한 설정 편집 {#node-edit}

광고 그룹에 포함된 단위 제품 그룹 노드(하위 제품 그룹 노드가 없는 제품 그룹)에 대한 입찰 및 추적 템플릿을 편집할 수 있습니다. 하위 제품 그룹 노드가 있는 제품 그룹인 제외된 단위 제품 그룹 또는 포함되거나 제외된 하위 분할 노드에 대한 정보는 편집할 수 없습니다.

1. 메인 메뉴에서 **[!UICONTROL Assets]>[!UICONTROL Shopping]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 트리 보기에서 제품 그룹 및 하위 제품 그룹 노드를 보려면 커서를 제품 그룹 이름 위에 놓고 **[!UICONTROL ...]>[!UICONTROL Tree View]**&#x200B;을(를) 클릭합니다.

1. 제품 그룹 이름 위에 커서를 놓고 **[!UICONTROL ...]>[!UICONTROL + Edit Node]**&#x200B;을(를) 클릭합니다.

1. [Google Ads 제품 그룹 설정](#google-ads-product-group-settings) 또는 [Microsoft Advertising 제품 그룹 설정](#microsoft-advertising-product-group-settings)을 편집합니다.

1. **[!UICONTROL Update]**&#x200B;을(를) 클릭합니다.

## 제품 그룹 노드의 [!UICONTROL Tracking Template]만 편집 {#node-edit-tracking-template}

1. 메인 메뉴에서 **[!UICONTROL Assets]>[!UICONTROL Shopping]**&#x200B;을(를) 클릭합니다.

1. 제품 그룹 이름 위에 커서를 놓고 **[!UICONTROL ...]>[!UICONTROL Tree View]**&#x200B;을(를) 클릭하여 트리 보기에서 제품 그룹과 해당 하위 제품 그룹 노드를 봅니다.

1. **[!UICONTROL Tracking Template]** 열에서 ![편집](/help/search-social-commerce/assets/edit-new.png "편집")을 클릭합니다.

1. **[!UICONTROL Tracking Template]** 값을 변경한 다음 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 제품 그룹 노드의 [!UICONTROL Max CPC]만 편집 {#node-edit-maxcpc}

1. 메인 메뉴에서 **[!UICONTROL Assets]>[!UICONTROL Shopping]**&#x200B;을(를) 클릭합니다.

1. 제품 그룹 이름 위에 커서를 놓고 **[!UICONTROL ...]>[!UICONTROL Tree View]**&#x200B;을(를) 클릭하여 트리 보기에서 제품 그룹과 해당 하위 제품 그룹 노드를 봅니다.

1. **[!UICONTROL Max CPC]** 열에서 ![편집](/help/search-social-commerce/assets/edit-new.png "편집")을 클릭합니다.

1. **[!UICONTROL Max CPC]** 값을 변경한 다음 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 제품 그룹 노드 삭제 {#node-delete}

같은 수준에 다른 제품 그룹이 있는 경우 &quot;기타 모든 제품&quot; 그룹을 제외한 모든 제품 그룹을 삭제할 수 있습니다. 이 그룹은 머천트 센터 계정의 제품 중 광고 그룹에 대한 쇼핑 광고에 포함되는 제품을 결정하는 데 사용됩니다. 제품 그룹을 삭제하면 모든 하위 제품 그룹이 삭제됩니다.

1. 메인 메뉴에서 **[!UICONTROL Assets]>[!UICONTROL Shopping]**&#x200B;을(를) 클릭합니다.

1. 제품 그룹 이름 위에 커서를 놓고 **[!UICONTROL ...]>[!UICONTROL Tree View]**&#x200B;을(를) 클릭하여 트리 보기에서 제품 그룹과 해당 하위 제품 그룹 노드를 봅니다.

1. **[!UICONTROL Status]** 열을 클릭하고 **[!UICONTROL Delete]**&#x200B;을(를) 선택합니다.

1. 확인 메시지에서 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

## 선택한 제품 그룹에 제한 할당 {#constraint-assign}

1. 메인 메뉴에서 **[!UICONTROL Assets]>[!UICONTROL Shopping]**&#x200B;을(를) 클릭합니다.

1. 단일 제약조건을 지정할 각 제품 그룹 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **+[!UICONTROL Assign]** > **[!UICONTROL Constraint]**&#x200B;을(를) 클릭합니다.

1. 제약조건을 선택합니다.

1. **[!UICONTROL Assign Now]**&#x200B;을(를) 클릭합니다.

## 선택한 제품 그룹에서 제한 제거 {#constraint-unassign}

1. 메인 메뉴에서 **[!UICONTROL Assets]>[!UICONTROL Shopping]**&#x200B;을(를) 클릭합니다.

1. 제한을 할당 해제할 각 제품 그룹 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **-[!UICONTROL Unassign]** > **[!UICONTROL Constraint]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

## 제품 그룹에 분류 값 할당 {#classification-values-assign}

>[!NOTE]
>
>레이블 값은 하위 엔티티에 의해 상속되므로 상속된 값을 재정의하지 않는 한 하위 엔티티에 대한 값을 입력하지 마십시오.

1. 메인 메뉴에서 **[!UICONTROL Assets]>[!UICONTROL Shopping]**&#x200B;을(를) 클릭합니다.

1. 레이블 값을 지정할 각 제품 그룹 옆의 확인란을 선택합니다.

   여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)&quot;을 참조하십시오.

1. 일괄 작업 도구 모음에서 **+[!UICONTROL Assign]** > **[!UICONTROL Label Classification]**&#x200B;을(를) 클릭합니다.

1. 적용 가능한 각 분류 값에 대해 다음을 수행합니다.

   1. **[!UICONTROL Classifications]** 열에서 분류를 지정합니다.

      * 기존 분류를 사용하려면 분류 이름을 클릭하여 확장합니다.

      * 분류를 만들려면 열 머리글에서 [!UICONTROL +]을(를) 클릭합니다. 입력 필드에 분류 이름을 입력한 다음 ![저장](/help/search-social-commerce/assets/save-checkmark.png "저장")을 클릭하여 분류를 즉시 저장합니다. 새 분류를 사용하려면 분류 이름을 클릭하여 확장합니다.

        이름은 [ASCII 문자 32-126](https://www.asciitable.com/)&#x200B;(으)로 구성되어야 하며 최대 길이는 27개의 싱글바이트 문자입니다.

   1. **[!UICONTROL Value Name]** 열에서 선택한 분류의 값을 지정하십시오.

      * 기존 값을 사용하려면 값을 선택합니다.

      * 값을 만들려면 열 머리글에서 [!UICONTROL +]을(를) 클릭합니다. 입력 필드에 값을 입력한 다음 ![저장](/help/search-social-commerce/assets/save-checkmark.png "저장")을 클릭하여 값을 즉시 저장하고 기본적으로 선택합니다.

        최대 길이는 100자이며 ASCII 및 비 ASCII 문자를 포함할 수 있습니다.

1. **+[!UICONTROL Assign Now]**&#x200B;을(를) 클릭합니다.

## 제품 그룹에서 레이블 분류 값 제거 {#classification-values-remove}

분류 값을 제거하면 계정 구성 요소 및 모든 하위 구성 요소와의 연결이 제거됩니다. 분류 값에 대한 보고서 데이터는 해당 구성 요소에서 더 이상 사용할 수 없습니다. 분류 값을 제거해도 값이나 계정 구성 요소는 삭제되지 않습니다.

1. 메인 메뉴에서 **[!UICONTROL Assets]>[!UICONTROL Shopping]**&#x200B;을(를) 클릭합니다.

1. 레이블 값을 제거할 각 제품 그룹 옆의 확인란을 선택합니다.

   여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)&quot;을 참조하십시오.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Unassign]** > **[!UICONTROL Label Classification]**&#x200B;을(를) 클릭합니다.

1. 선택한 엔티티에서 제거할 각 분류 값 옆의 확인란을 선택합니다.

   할당된 모든 값을 선택하려면 **[!UICONTROL Select All]**&#x200B;을(를) 클릭하십시오. 할당된 모든 값을 선택 해제하려면 **[!UICONTROL Deselect All]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Unassign Selected]**&#x200B;을(를) 클릭합니다.

## [!DNL Google Ads] 제품 그룹 설정 {#google-ads-product-group-settings}

### &quot;모든 제품&quot; 제품 그룹

**[!UICONTROL Network]:**(새 제품 그룹만 해당) 광고 네트워크입니다.

**[!UICONTROL Account]:**(새 제품 그룹만 해당) 광고 네트워크 계정 이름입니다.

**[!UICONTROL Campaign]:**(새 제품 그룹만 해당) 캠페인.

**[!UICONTROL Ad Group]:**(새 제품 그룹만 해당) 광고 그룹입니다.

**[!UICONTROL Condition]** 또는 **[!UICONTROL Condition Type]:**(읽기 전용) 모든 제품

**[!UICONTROL Condition Value]:**(기존 제품 그룹만 해당)  

**[!UICONTROL Bid]** 또는 **[!UICONTROL Max CPC]:**(제품 그룹만 포함) 광고 클릭에 대해 지불할 가장 높은 금액인 클릭당 최대 비용(CPC)입니다. 이 값은 하위 제품 그룹이 없는 단위에 대해서만 사용되며 광고 그룹 수준 값 대신 사용됩니다.

{{$include /help/_includes/tracking-template-google.md}}

이 템플릿은 상위 수준의 템플릿을 재정의하며 하위 제품 그룹이 없는 단위에 대해서만 사용됩니다. 계정이나 캠페인에 대해 지정된 추가 매개 변수는 포함되지 않습니다. 계정이나 캠페인에 대해 지정된 추가 매개 변수는 포함되지 않습니다.

### 기타 모든 제품 그룹

**[!UICONTROL Condition Type]** 및 **[!UICONTROL Condition Value]:**(기존 제품 그룹의 경우 읽기 전용) 대상으로 지정할 제품 차원입니다. 새 제품 그룹의 경우 제품을 타겟팅할 차원 및 선택한 정보 카테고리의 자격 속성(예: 브랜드별로 타겟팅하는 경우 &quot;Acme&quot; 또는 조건별로 타겟팅하는 경우 &quot;New&quot;)을 입력합니다.

특정 제품 차원(&quot;모든 제품&quot;이 아닌)에 대한 제품 그룹을 만들면 검색, 소셜 및 Commerce에서 자동으로 &quot;기타 모두&quot;에 대한 제품 그룹을 만듭니다.

사용 가능한 제품 차원 목록을 보려면 &quot;[제품 필터](#product-filters)&quot;을 참조하세요. 캠페인의 [!UICONTROL Inventory Filter] 설정에 따라 차원 목록이 제한될 수 있습니다.

**[!UICONTROL Excluded]:**(새 제품 그룹의 경우 선택 사항, 기존 제품 그룹의 경우 읽기 전용) 일치하는 제품의 광고에 대한 입찰을 제외합니다.

**[!UICONTROL Max CPC]:**(포함된 제품 그룹만 해당) 광고 클릭에 대해 지불할 가장 높은 금액인 클릭당 최대 비용(CPC)입니다. 이 값은 하위 제품 그룹이 없는 단위에 대해서만 사용되며 광고 그룹 수준 값 대신 사용됩니다.

<!--
 ExL can't handle the same include twice in the same file, so using a snippet for the second occurrence.

{{$include /help/_includes/tracking-template-google.md}}
-->

{{tracking-template-google}}

이 템플릿은 상위 수준의 템플릿을 재정의하며 하위 제품 그룹이 없는 단위에 대해서만 사용됩니다.

## [!DNL Microsoft Advertising] 제품 그룹 설정 {#microsoft-advertising-product-group-settings}

### &quot;모든 제품&quot; 제품 그룹

**[!UICONTROL Network]:**(새 제품 그룹만 해당) 광고 네트워크입니다.

**[!UICONTROL Account]:**(새 제품 그룹만 해당) 광고 네트워크 계정 이름입니다.

**[!UICONTROL Campaign]:**(새 제품 그룹만 해당) 캠페인.

**[!UICONTROL Ad Group]:**(새 제품 그룹만 해당) 광고 그룹입니다.

**[!UICONTROL Condition]** 또는 **[!UICONTROL Condition Type]:**(읽기 전용) 모든 제품

**[!UICONTROL Condition Value]:**(기존 제품 그룹만 해당)  

**[!UICONTROL Bid]** 또는 **[!UICONTROL Max CPC]:**(제품 그룹만 포함) 광고 클릭에 대해 지불할 가장 높은 금액인 클릭당 최대 비용(CPC)입니다. 이 값은 하위 제품 그룹이 없는 단위에 대해서만 사용되며 광고 그룹 수준 값 대신 사용됩니다.

**[!UICONTROL Base URL]:**(새 제품 그룹만) 사용되지 않음<!-- Not sure this is supposed to be there; it's not showing for an existing product group: {{$include /help/_includes/base-url-keyword-ad-sitelink.md}} -->

{{$include /help/_includes/tracking-template-microsoft.md}}

이 템플릿은 상위 수준의 템플릿을 재정의하며 하위 제품 그룹이 없는 단위에 대해서만 사용됩니다.

### 기타 모든 제품 그룹

**[!UICONTROL Condition Type]** 및 **[!UICONTROL Condition Value]:**(기존 제품 그룹의 경우 읽기 전용) 대상으로 지정할 제품 차원입니다. 새 제품 그룹의 경우 제품을 타겟팅할 차원과 선택한 정보 카테고리의 자격 속성(예: 브랜드별로 타겟팅하는 경우 &quot;Acme&quot; 또는 조건별로 타겟팅하는 경우 &quot;New&quot;)을 입력합니다.

특정 제품 차원(&quot;모든 제품&quot;이 아닌)에 대한 제품 그룹을 만들면 검색, 소셜 및 Commerce에서 자동으로 &quot;기타 모두&quot;에 대한 제품 그룹을 만듭니다.

사용 가능한 제품 차원 목록을 보려면 &quot;[제품 필터](#product-filters)&quot;을 참조하세요. 캠페인의 [!UICONTROL Inventory Filter] 설정에 따라 차원 목록이 제한될 수 있습니다.

**[!UICONTROL Excluded]:**(새 제품 그룹의 경우 선택 사항, 기존 제품 그룹의 경우 읽기 전용) 일치하는 제품의 광고에 대한 입찰을 제외합니다.

**[!UICONTROL Max CPC]:**(포함된 제품 그룹만 해당) 광고 클릭에 대해 지불할 가장 높은 금액인 클릭당 최대 비용(CPC)입니다. 이 값은 하위 제품 그룹이 없는 단위에 대해서만 사용되며 광고 그룹 수준 값 대신 사용됩니다.

<!--
 ExL can't handle the same include twice in the same file, so using a snippet for the second occurrence.

{{$include /help/_includes/tracking-template-microsoft.md}}
-->

{{tracking-template-microsoft}}

이 템플릿은 상위 수준의 템플릿을 재정의하며 하위 제품 그룹이 없는 단위에 대해서만 사용됩니다.

>[!MORELIKETHIS]
>
>* [쇼핑 캠페인 구현 [!DNL Google Ads] 2&rbrace;](/help/search-social-commerce/campaign-management/special-workflows/google-shopping-campaigns.md)
>* [쇼핑 캠페인 구현 [!DNL Microsoft Advertising] 2&rbrace;](/help/search-social-commerce/campaign-management/special-workflows/microsoft-shopping-campaigns.md)
>* [[!UICONTROL Product Group Report]](/help/search-social-commerce/new-ui/reports/management/basic-advanced/product-group-report.md)
