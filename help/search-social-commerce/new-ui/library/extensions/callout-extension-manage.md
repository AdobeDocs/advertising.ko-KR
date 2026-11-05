---
title: Google 광고 공유 설명선 확장 관리
description: Google Ads 공유 콜아웃 확장을 만들고, 편집하고, 삭제하는 방법을 알아봅니다.
feature: Search Campaign Management
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: aed5e38a-3e62-42fa-8d16-cd080729b2a0
    internal-label: Search, Social, & Commerce
  - id: 76ac9ff6-5d89-5acb-bc0b-875761bb3320
    internal-label: Search Campaign Management
subfeature_v2:
  - id: f3d33161-c519-436e-bbbd-730ba428736b
    internal-label: Campaign management
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 10d7adc3b3ced812ee1281139a23a573df2beeef
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 0%
---
# [!DNL Google Ads] 공유 콜아웃 확장 관리

*[!DNL Google Ads]개의 계정만*

설명선 확장은 사이트에서 제공하는 제품, 서비스 또는 프로모션에 대한 정보 텍스트로서, 텍스트 광고와 함께 표시됩니다. 광고 네트워크에는 광고가 포함된 2~4개의 콜아웃이 표시될 수 있습니다.

[동기화된 Google 광고 계정](/help/search-social-commerce/new-ui/manage/accounts/api-accounts/api-account-manage.md)에 대해 계정 수준에서 공유 콜아웃 텍스트 및 설정을 만듭니다. 라이브러리의 설명선은 검색 네트워크에서 지원되는 캠페인이나 광고 그룹에 연결할 때까지 광고와 함께 사용되지 않습니다.

광고를 콜아웃과 함께 표시할 수 있도록 하려면 캠페인 또는 광고 그룹당 최소 두 개의 콜아웃을 할당하십시오. 광고 그룹 수준의 콜아웃은 캠페인 수준의 콜아웃을 재정의합니다.

## [!UICONTROL Callouts] 및 [!UICONTROL Associations] 보기 정보 {#callout-view-about}

**[!UICONTROL Library]>[!UICONTROL Extensions]**&#x200B;에서 **[!UICONTROL Callouts]** 탭에 계정 수준 공유 설명선이 나열됩니다. **[!UICONTROL Associations]** 탭에는 확장과 계정 엔터티 간의 연결이 나열됩니다.

이 탭을 보려면 [!UICONTROL View Extensions] 권한이 필요합니다. 설명선을 만들고, 편집하고, 삭제하고, 연결을 만들거나 삭제하려면 [!UICONTROL Edit Extensions] 권한이 필요합니다.

계정당 최대 확장 수는 [계정 제한에 대한 Google 광고 설명서](https://support.google.com/google-ads/answer/6372658)를 참조하세요.

### 사용 가능한 작업

* [공유 설명선 만들기](#callout-create)

* [공유 설명선 설정 편집](#callout-edit)

* [공유 설명선 삭제](#callout-delete)

* [공유 콜아웃을 캠페인 및 광고 그룹과 연결](ad-extension-association-manage.md#callout-associate)

* [확장 연결 삭제](ad-extension-association-manage.md#association-delete)

* [선택한 행의 모든 데이터를 클립보드에 복사](#copy-to-clipboard)

## 공유 설명선 만들기 {#callout-create}

1. 주 메뉴에서 **[!UICONTROL Library]>[!UICONTROL Extensions]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Callouts]** 탭을 클릭합니다.

1. **[!UICONTROL Create Callout]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Basic Settings]**&#x200B;에서 [!DNL Google Ads] 및 계정을 선택합니다.

1. [공유 설명선 설정](#shared-callout-settings)을 입력하십시오.

1. **[!UICONTROL Review and Save]**&#x200B;을(를) 클릭합니다.

1. 설정을 검토합니다. 설정을 변경하려면 해당 섹션에서 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

콜아웃을 만든 후 [캠페인 또는 광고 그룹에 연결](ad-extension-association-manage.md#callout-associate)합니다.

## 공유 설명선 설정 편집 {#callout-edit}

한 번에 하나의 공유 콜아웃을 편집할 수 있습니다. 만든 후에는 시작 날짜를 변경할 수 없습니다.

1. 주 메뉴에서 **[!UICONTROL Library]>[!UICONTROL Extensions]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Callouts]** 탭을 클릭합니다.

1. 설명선 옆에 있는 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. [공유 설명선 설정](#shared-callout-settings)을(를) 편집합니다.

1. **[!UICONTROL Review and Save]**&#x200B;을(를) 클릭하고 설정을 검토한 다음 **[!UICONTROL Update]**&#x200B;을(를) 클릭합니다.

## 공유 설명선 삭제 {#callout-delete}

1. 주 메뉴에서 **[!UICONTROL Library]>[!UICONTROL Extensions]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Callouts]** 탭을 클릭합니다.

1. 삭제할 각 공유 설명선 옆의 확인란을 선택합니다.

   여러 행 선택에 대한 자세한 내용은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)&quot;을 참조하십시오.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

라이브러리에서 공유 콜아웃을 삭제하지 않고 연결을 제거하려면 [연결을 삭제](ad-extension-association-manage.md#association-delete)하십시오.

## 선택한 행의 모든 데이터를 클립보드에 복사 {#copy-to-clipboard}

보기에 표시되는 적용된 필터 및 열에 따라 선택한 행에 표시되는 정보를 복사합니다. 정보는 탭으로 구분된 값(TSV)으로 저장됩니다.

1. 데이터를 복사할 각 행 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Copy]**&#x200B;을(를) 클릭합니다.

## 공유 설명선 설정 {#shared-callout-settings}

추가 정책 및 설명선 승인 거절의 이유에 대해서는 [Google 광고 설명선 요구 사항](https://support.google.com/adspolicy/answer/1054212)을 참조하십시오.

**[!UICONTROL Callout Text]:** 표시할 텍스트입니다. 최대 25개의 1바이트 문자 또는 12개의 2바이트 문자를 포함할 수 있습니다. 텍스트 앞부분에 느낌표나 구두점을 포함할 수 없습니다.

**[!UICONTROL Start Date]:**(선택 사항, 만들기만) 콜아웃이 표시될 수 있는 첫 번째 날짜입니다. 기본값은 현재 날짜입니다. 미래 날짜를 지정하려면 MM/DD/YYYY 형식으로 입력하거나 날짜 선택기를 사용합니다. 기존 콜아웃에 대해 시작 날짜가 읽기 전용입니다.

**[!UICONTROL End Date]:**(선택 사항) 콜아웃을 표시할 마지막 날짜입니다. 기본적으로 설명선은 무기한 표시될 수 있습니다. 종료 날짜를 지정하려면 MM/DD/YYYY 형식으로 입력하거나 날짜 선택기를 사용합니다.

**[!UICONTROL Mobile Preference]:**(선택 사항) [!DNL Google Ads]에서 데스크톱 또는 태블릿 사용자가 아닌 모바일 장치 사용자에게 확장을 표시할 수 있도록 합니다. 그렇지 않으면 모든 디바이스 유형에 확장이 나타날 수 있습니다. [!DNL Google Ads]은(는) 기본 장치 유형에서 확장을 표시할지 보장하지 않습니다.

## 콜아웃에 대한 성능 데이터 {#callout-performance}

Search, Social 및 Commerce은 광고 확장에 대한 클릭 수와 결과 전환을 확장이 표시되는 광고와 연결된 키워드로 매핑합니다. 검색, 소셜 및 Commerce에서는 확장 수준 비용 및 클릭 데이터를 사용할 수 없습니다.

확장 수준 비용을 보고 [!DNL Google Ads] 인터페이스에서 데이터를 클릭할 수 있습니다.

>[!MORELIKETHIS]
>
>* [공유 사이트 링크 확장 관리](sitelink-extension-manage.md)
>* [광고 확장 연결 관리](ad-extension-association-manage.md)
