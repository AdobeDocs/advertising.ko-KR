---
title: 키워드 관리
description: 바인딩 가능한 및 부정적인 키워드를 만들고 관리하고 키워드에 제약 조건을 할당하는 방법을 알아봅니다.
feature: Search Optimization, Search Campaign Management
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: aed5e38a-3e62-42fa-8d16-cd080729b2a0
    internal-label: Search, Social, & Commerce
  - id: ae57d55f-b168-5358-b114-c3974b1b3d77
    internal-label: Search Optimization
  - id: 76ac9ff6-5d89-5acb-bc0b-875761bb3320
    internal-label: Search Campaign Management
subfeature_v2:
  - id: f3d33161-c519-436e-bbbd-730ba428736b
    internal-label: Campaign management
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: d3e38179ae119f35c184bee398edaaf456fab563
workflow-type: tm+mt
source-wordcount: '1282'
ht-degree: 0%
---
# 키워드 관리

*Beta 기능*

*[!DNL Google Ads], [!DNL LY Ads], [!DNL Microsoft Advertising], [!DNL Yandex] 및 기존 [!DNL Baidu] 계정만*

키워드는 광고와 연관된 단어 또는 구입니다. 키워드 설정에는 키워드 일치 유형, 키워드에 의해 광고가 트리거될 때 사용할 최대 입찰 및 선택적 추적 매개 변수(일부 광고 네트워크의 경우)가 포함됩니다. 키워드 수준 설정은 광고 그룹 또는 캠페인 설정을 재정의합니다. 음수 키워드는 일치하는 검색에 대한 광고가 표시되지 않도록 합니다.

[API 연결을 통해 광고 네트워크 계정에 액세스할 수 있도록 설정](/help/search-social-commerce/new-ui/manage/accounts/api-accounts/api-account-manage.md) 및 검색, 소셜 및 Commerce이 계정 데이터를 광고 네트워크와 동기화하면 [지원되는 캠페인 유형](/help/search-social-commerce/introduction/supported-inventory.md)에서 검색 광고 그룹에 대한 키워드를 만들 수 있습니다. 또한 키워드의 상태를 편집 및 변경하고 부정적인 키워드를 만들고 삭제할 수 있습니다.

각 광고 네트워크에서 사용할 수 있는 기능에 대한 자세한 내용은 &quot;[지원되는 인벤토리](/help/search-social-commerce/introduction/supported-inventory.md)&quot;를 참조하십시오.

## [!UICONTROL Keywords] 보기 정보 {#keyword-view-about}

[!UICONTROL Manage] > [!UICONTROL Keywords] 보기에는 선택한 광고주 계정에 대한 두 개의 탭이 있습니다.

* [!UICONTROL Keywords] 탭에는 필터링된 보기에 있는 모든 바인딩 가능한 키워드가 나열됩니다.

* [!UICONTROL Negatives] 탭에는 필터링된 보기의 모든 부정적인 키워드가 나열됩니다.

### 사용 가능한 작업

* [키워드 만들기](#keyword-create)

* [부정적인 키워드 만들기](#keyword-negative-create)

* [키워드 설정 편집](#keyword-edit)

* [키워드 및 부정적 키워드의 상태 변경 또는 삭제](#keyword-status)

* [선택한 행의 모든 데이터를 클립보드에 복사](#copy-to-clipboard)

* [키워드에 제한 할당 및 키워드에서 제한 할당 해제](#keyword-constraints)

* 키워드에 [레이블 분류 할당](/help/search-social-commerce/new-ui/set-up/label-classifications-manage.md)

## 키워드 만들기 {#keyword-create}

>[!TIP]
>
>한 번에 수많은 키워드를 만들려면 [캠페인 일괄 시트](/help/search-social-commerce/new-ui/set-up/bulksheets/about.md)를 사용하십시오.

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Keywords]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Keywords]** 탭에서 **[!UICONTROL Create Keywords]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Basic Settings]** 단계에서 네트워크, 계정, 캠페인 및 광고 그룹을 선택합니다.

1. [[!DNL Baidu] 키워드 설정](keyword-settings-baidu.md), [[!DNL Google Ads] 키워드 설정](keyword-settings-google.md), [[!DNL LY Ads] 키워드 설정](keyword-settings-yahoo-japan.md), [[!DNL Microsoft Advertising] 키워드 설정](keyword-settings-microsoft.md) 또는 [[!DNL Yandex] 키워드 설정](keyword-settings-yandex.md)을 입력하십시오.

   한 번의 작업으로 최대 2000개의 키워드를 입력하거나 붙여넣을 수 있습니다. 여러 키워드를 쉼표로 구분하거나 별도의 줄에 입력합니다.

   >[!NOTE]
   >
   >계정 또는 캠페인 설정에서 광고 수준에서만 추적을 지정하는 경우 검색, 소셜 및 Commerce은 키워드에 대한 추적을 생성하지 않습니다.

1. **[!UICONTROL Review and Save]**&#x200B;을(를) 클릭합니다.

1. 설정을 검토합니다. 설정을 변경하려면 해당 섹션에서 ![편집](/help/search-social-commerce/assets/edit-new.png "편집") **[!UICONTROL Edit]**&#x200B;을(를) 클릭하고 설정을 변경합니다.

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

## 키워드 설정 편집 {#keyword-edit}

키워드 텍스트나 일치 유형을 변경하면 광고 네트워크에 따라 기존 키워드를 삭제하고 새 키워드를 만들 수 있습니다. 자세한 내용은 광고 네트워크에 대한 키워드 설정을 참조하십시오.

>[!TIP]
>
>다른 광고 네트워크의 키워드를 포함하여 많은 양의 키워드 데이터를 한 번에 편집하려면 [캠페인 일괄 시트](/help/search-social-commerce/new-ui/set-up/bulksheets/about.md)를 사용하십시오.

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Keywords]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Keywords]** 탭에서 편집할 각 키워드 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. [[!DNL Baidu] 키워드 설정](keyword-settings-baidu.md), [[!DNL Google Ads] 키워드 설정](keyword-settings-google.md), [[!DNL LY Ads] 키워드 설정](keyword-settings-yahoo-japan.md), [[!DNL Microsoft Advertising] 키워드 설정](keyword-settings-microsoft.md) 또는 [[!DNL Yandex] 키워드 설정](keyword-settings-yandex.md)을 편집합니다.

   여러 키워드의 경우 선택한 모든 키워드에 공통되는 필드만 편집할 수 있으며 변경 사항은 선택한 모든 키워드에 적용됩니다. 일부 영숫자 필드의 경우 기존 값을 지정된 값으로 변경하거나, 기존 문자열을 지정된 문자열로 바꾸거나, 접두어를 추가하거나, 접미어를 추가할 수 있습니다. 일부 통화 필드의 경우 기존 값을 지정된 값으로 변경하거나, 제한을 두고 지정된 백분율이나 통화 금액만큼 금액을 늘리거나 줄일 수 있습니다.

1. **[!UICONTROL Review and Save]**&#x200B;을(를) 클릭합니다.

1. 설정을 검토합니다. 설정을 변경하려면 해당 섹션에서 ![편집](/help/search-social-commerce/assets/edit-new.png "편집") **[!UICONTROL Edit]**&#x200B;을(를) 클릭하고 설정을 변경합니다.

1. **[!UICONTROL Update]**&#x200B;을(를) 클릭합니다.

## 부정적인 키워드 만들기 {#keyword-negative-create}

*[!DNL Google Ads], [!DNL LY Ads], [!DNL Microsoft Advertising] 및 기존 [!DNL Baidu] 계정만*

검색 또는 디스플레이/기본 네트워크를 대상으로 하는 검색 광고 그룹 또는 캠페인에 대해 부정적인 키워드를 만들 수 있습니다.

>[!NOTE]
>
>[광고 그룹 설정](/help/search-social-commerce/new-ui/manage/ad-groups/ad-group-manage.md) 및 [캠페인 설정](/help/search-social-commerce/new-ui/manage/campaigns/campaign-manage.md)에서 부정적인 키워드를 만들고 편집할 수도 있습니다.

>[!TIP]
>
>한 번에 많은 수의 네거티브 키워드를 만들려면 [캠페인 일괄 시트](/help/search-social-commerce/new-ui/set-up/bulksheets/about.md)를 사용하십시오.

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Keywords]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Negatives]** 탭에서 **[!UICONTROL Create Negatives]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Campaign Negative Keyword]** 또는 **[!UICONTROL Ad Group Negative Keyword]**&#x200B;을(를) 클릭합니다.

1. 네트워크, 계정, 캠페인 및 광고 그룹을 선택합니다(광고 그룹 수준의 부정적 키워드의 경우).

1. 음의 키워드를 입력합니다. 빼기 기호(`-`) 없이 다음 구문을 사용하십시오.

   * 음수 브로드 일치: `keyword`([!DNL Microsoft Advertising]에서 지원되지 않음)

   * 음수 구 일치: `"keyword"`

   * 정확히 일치하는 음수: `[keyword]`

   여러 값을 쉼표로 구분하거나 별도의 라인에 입력합니다. 한 번의 작업으로 최대 2000개의 부정적인 키워드를 입력하거나 붙여넣을 수 있습니다. 다음 요구 사항 및 제한 사항이 적용됩니다.

   * 최대 문자 길이: [!DNL Baidu]: 1바이트 또는 15 2바이트; [!DNL Microsoft Advertising]: 100 1바이트 또는 50 2바이트; [!DNL Google Ads] 및 [!DNL LY Ads]: 80 1바이트 또는 40 2바이트.

   * [!DNL Baidu]에서는 광고 그룹당 키워드당 일치 유형을 하나만 사용할 수 있습니다. 예를 들어 광고 그룹 1은 `"keyword"`과(와) `[keyword]`을(를) 모두 포함할 수 없습니다.

   * [!DNL Google Ads]: 각 키워드는 10단어 이하로 구성될 수 있으며 문자, 숫자 및 다음 특수 문자만 포함할 수 있습니다. 공백 `# $ & _ - " [ ] ' + . / :`

1. **[!UICONTROL Review and Save]**&#x200B;을(를) 클릭합니다.

1. 설정을 검토합니다. 설정을 변경하려면 해당 섹션에서 ![편집](/help/search-social-commerce/assets/edit-new.png "편집") **[!UICONTROL Edit]**&#x200B;을(를) 클릭하고 설정을 변경합니다.

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

## 키워드 및 부정적 키워드의 상태 변경 {#keyword-status}

입찰 가능한 활성 검색 키워드를 일시 중지하여 입찰을 비활성화할 수 있습니다. 나중에 상태를 다시 활성으로 변경하여 입찰을 다시 시작할 수 있습니다.

활성 또는 일시 중지된 검색 키워드나 부정적 키워드를 삭제할 수도 있습니다. 삭제된 키워드는 광고 네트워크에서 삭제됩니다. 이러한 데이터는 데이터 필터에 포함할 때 계속 표시되지만 변경할 수는 없습니다.

### 키워드 활성화 또는 일시 중지

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Keywords]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Keywords]** 탭에서 선택적으로 목록을 필터링한 다음 상태를 변경할 각 키워드 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 상태를 변경합니다.

   * 일시 중지된 키워드를 활성화하려면 **[!UICONTROL Activate]**&#x200B;을(를) 클릭합니다.

   * 활성 키워드를 일시 중지하려면 **[!UICONTROL Pause]**&#x200B;을(를) 클릭합니다.

### 키워드 또는 부정적 키워드 삭제

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Keywords]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Keywords]** 또는 **[!UICONTROL Negatives]** 탭에서 선택적으로 목록을 필터링한 다음 삭제할 각 키워드 또는 음수 키워드 옆에 있는 확인란을 선택하십시오.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

## 선택한 행의 모든 데이터를 클립보드에 복사 {#copy-to-clipboard}

보기에 표시되는 적용된 필터 및 열에 따라 선택한 행에 표시되는 정보를 복사합니다. 정보는 탭으로 구분된 값(TSV)으로 저장됩니다.

1. 데이터를 복사할 각 행 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Copy]**&#x200B;을(를) 클릭합니다.

## 키워드에 대한 제한 할당 관리 {#keyword-constraints}

캠페인, 광고 그룹, 키워드, 배치, 단위 수준 제품 그룹 및 동적 검색 타겟에 대한 입찰 제한을 할당 및 제거할 수 있습니다. 각 엔티티에는 하나의 제약조건만 있을 수 있습니다.

구속은 하위 엔티티에 의해 상속되므로 상속된 값을 재정의하지 않는 한 하위 엔티티에 대한 구속을 할당할 필요가 없습니다.

제약 조건을 할당 해제하면 계정 구성 요소 및 모든 하위 구성 요소와의 연결이 제거되며 해당 구성 요소에 대해 제약 조건에 대한 보고서 데이터를 더 이상 사용할 수 없습니다. 제한 지정을 취소해도 제한 또는 계정 구성 요소 자체는 삭제되지 않습니다.

>[!NOTE]
>
>* 나중에 변경할 수 없는 광고에 대한 키워드 또는 광고 사본을 편집하여 새 키워드 또는 광고를 만드는 경우 새 엔티티에 제약 조건이 할당되지 않습니다.
>* 활성 제한은 최적화된 레거시 키워드 수준 포트폴리오에서 할당된 입찰 단위에 대해서만 입찰을 제한합니다. 활성 포트폴리오에 있거나, 하이브리드 포트폴리오에 있거나, 포트폴리오에 없는 입찰 단위에 대해서는 무시됩니다.

### 키워드에 제한 할당 {#keyword-constraint-assign}

하나 이상의 키워드에 단일 제약 조건을 지정할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Keywords]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Keywords]** 탭에서 단일 제약 조건을 할당할 각 키워드 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **+[!UICONTROL Assign]** > **[!UICONTROL Constraint]**&#x200B;을(를) 클릭합니다.

1. 제약조건을 선택합니다.

1. **[!UICONTROL Assign Now]**&#x200B;을(를) 클릭합니다.

### 키워드에서 제한 할당 해제 {#keyword-constraint-unassign}

제한 지정을 취소해도 삭제되지 않습니다. 제한을 삭제하여 나중에 사용할 수 없게 하려면 검색, 소셜 및 Commerce 내에서 사용할 수 있는 &quot;입찰 제한&quot;에 대한 최적화 안내서 장의 &quot;검색 입찰 단위에 대한 제한 삭제&quot;를 참조하십시오.

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Keywords]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Keywords]** 탭에서 제약 조건 할당을 취소할 각 키워드 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **-[!UICONTROL Unassign]** > **[!UICONTROL Constraint]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [[!DNL Baidu] 키워드 설정](keyword-settings-baidu.md)
>* [[!DNL Google Ads] 키워드 설정](keyword-settings-google.md)
>* [[!DNL LY Ads] 키워드 설정](keyword-settings-yahoo-japan.md)
>* [[!DNL Microsoft Advertising] 키워드 설정](keyword-settings-microsoft.md)
>* [[!DNL Yandex] 키워드 설정](keyword-settings-yandex.md)
>* [검색 입찰 단위에 대한 제약 조건 관리](/help/search-social-commerce/new-ui/goals/constraints-manage.md)
>* [레이블 분류 관리](/help/search-social-commerce/new-ui/set-up/label-classifications-manage.md)
