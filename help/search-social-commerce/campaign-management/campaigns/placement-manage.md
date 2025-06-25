---
title: ' [!DNL Google Ads] 배치 관리'
description: ' [!DNL Google Ads] 광고 그룹에 대해 추가할 수 있는 배치를 만들고 관리하는 방법을 알아봅니다.'
exl-id: 80cb6fc6-e778-4b19-9e52-e0b57bde0d73
feature: Search Campaign Management
source-git-commit: d0f1c413134a0868ddec79ded7672af316267edd
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# [!DNL Google Ads]개 배치 관리

*[!DNL Google Ads]개의 계정만*

[동기화된 광고 네트워크 계정](/help/search-social-commerce/campaign-management/accounts/ad-network-account-about.md) 내에서 디스플레이 네트워크를 대상으로 하는 [지원되는 캠페인 유형](/help/search-social-commerce/introduction/supported-inventory.md)에서 광고 그룹에 대한 배치를 만들고 편집할 수 있습니다.

## [!DNL Google Ads]개 배치 만들기

>[!TIP]
>
>한 번에 여러 배치를 만들려면 [캠페인 일괄 시트](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-about.md)를 사용하십시오.

1. 메인 메뉴에서 **[!UICONTROL Search, Social, & Commerce]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다. 하위 메뉴에서 **[!UICONTROL Live]> [!UICONTROL Placements] >[!UICONTROL Placements]**&#x200B;을(를) 클릭합니다.

1. 
   1. 데이터 테이블 위의 도구 모음에서 ![만들기](/help/search-social-commerce/assets/add.png "만들기")를 클릭합니다.

1. 광고 네트워크, 계정, 캠페인 및 광고 그룹을 선택한 다음 **[!UICONTROL Continue]**&#x200B;을(를) 클릭합니다.

1. [배치 설정](#placement-settings)을 구성하십시오.

1. **[!UICONTROL Post]**&#x200B;을(를) 클릭합니다.

## [!DNL Google Ads]개 배치 편집

>[!TIP]
>
>한 번에 여러 배치를 편집하려면 [캠페인 일괄 시트](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-about.md)를 사용하십시오.

1. 메인 메뉴에서 **[!UICONTROL Search, Social, & Commerce]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다. 하위 메뉴에서 **[!UICONTROL Live]> [!UICONTROL Keywords] >[!UICONTROL Keywords]**&#x200B;을(를) 클릭합니다.

1. 편집할 각 행 옆의 확인란을 선택합니다.

   여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)&quot;을 참조하십시오.

1. 데이터 테이블 위의 도구 모음에서 ![편집](/help/search-social-commerce/assets/edit.png "편집") 을 클릭합니다.

1. [배치 설정](#placement-settings)을(를) 편집합니다.

   여러 배치의 경우 변경 사항이 선택한 모든 배치에 적용됩니다. 일부 영숫자 필드의 경우 기존 값을 지정된 값으로 변경하거나, 기존 문자열을 지정된 문자열로 바꾸거나, 각 값의 시작 부분에 지정된 접두사를 추가하거나, 각 값의 끝에 접미사를 추가할 수 있습니다. 일부 통화 필드의 경우 기존 값을 지정된 값으로 변경하거나, 제한을 사용하여 지정된 백분율 또는 통화 금액만큼 금액을 늘리거나 줄일 수 있습니다.

1. 데이터를 저장합니다.

   * (단일 배치) **[!UICONTROL Post]**&#x200B;을(를) 클릭합니다.

   * (여러 배치) **[!UICONTROL Post Now]**&#x200B;을(를) 클릭합니다.

## 배치 설정 {#placement-settings}

### [!UICONTROL Placement Details]

광고가 표시될 수 있는 콘텐츠 네트워크의 사이트 **[!UICONTROL Placements]:**&#x200B;개. 올바른 URL(예: www.example.com, example.com 또는 www.example.com/shoes/kids)을 입력하십시오. 여러 문자열을 지정하려면 쉼표로 구분하거나 별도의 줄에 입력합니다. URL에 물음표(`?`)를 포함할 수 없습니다. **참고:** [!UICONTROL Placements] > [!UICONTROL Negatives] 보기, 광고 그룹 및 캠페인 설정에서 [웹 사이트 배치를 제외](placement-negative-create.md)할 수 있습니다.

**[!UICONTROL Status]:** 배치 표시 상태: *활성*(입찰 활성화, 기본값), *일시 중지됨*(입찰 비활성화) 또는 *삭제됨*(배치를 삭제, 기존 배치만 해당).

### [!UICONTROL Bids]

**[!UICONTROL Bid]:**(선택 사항) 캠페인 입찰 전략에 따라 배치 기반 광고의 클릭당 최대 비용(CPC) 또는 천 단위 조회 노출당 비용(vCPM)입니다. 이 값은 광고 그룹 수준의 입찰을 무시합니다.

<!-- If the placement is in a standard optimized portfolio, then the specified bid is applied for one day. Afterward, the optimization capability places bids according to its own calculations. -->

### [!UICONTROL Tracking URLs]

<!-- **[!UICONTROL Base URL]:** -->

{{$include /help/_includes/base-url-keyword-ad-sitelink.md}}

<!-- note -->

{{$include /help/_includes/base-url-google-note.md}}

<!-- **[!UICONTROL Tracking Template]:** -->

{{$include /help/_includes/tracking-template-google.md}}

>[!MORELIKETHIS]
>
>* [배치 정보](placement-about.md)
>* [음수 배치 만들기](placement-negative-create.md)
>* [배치 및 음수 배치 상태 변경](placement-status-edit.md)
