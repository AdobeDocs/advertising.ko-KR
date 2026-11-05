---
title: 공유 사이트링크 확장 관리
description: 공유 사이트링크 확장을 만들고, 편집하고, 삭제하는 방법을 알아봅니다.
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
source-wordcount: '1127'
ht-degree: 0%
---
# 공유 사이트링크 확장 관리

*[!DNL Google Ads]및 [!DNL Microsoft Advertising] 계정만*

사이트링크는 텍스트 광고 목록에 있는 추가 텍스트 링크입니다. 사이트링크를 사용하여 사용자를 사이트의 특정 페이지로 직접 이동합니다. 광고 네트워크는 광고와의 관련성을 기반으로 표시할 사이트링크를 결정합니다.

각 사이트 링크에 대한 설명 텍스트를 선택적으로 포함할 수 있습니다. 또한 광고 네트워크는 사이트 링크와 관련성이 높을 때 계정에 있는 기존 광고의 사본을 표시할 수 있습니다. [!DNL Google Ads]은(는) 데스크톱 광고에 2~6개의 사이트링크를 표시할 수 있으며 모바일 광고에 최대 4개의 사이트링크를 표시할 수 있습니다. [!DNL Microsoft Advertising]은(는) 설명이 있는 사이트링크를 두 개, 네 개 또는 여섯 개 표시하거나 설명이 없는 사이트링크를 4-6개 표시할 수 있습니다.

[동기화된 광고 네트워크 계정](/help/search-social-commerce/new-ui/manage/accounts/api-accounts/api-account-manage.md)에 대해 계정 수준에서 공유 사이트 링크 텍스트 및 설정을 만듭니다. 라이브러리의 사이트 링크는 계정 엔티티에 연결할 때까지 광고와 함께 사용되지 않습니다.

## [!UICONTROL Sitelinks] 및 [!UICONTROL Associations] 보기 정보 {#sitelink-view-about}

**[!UICONTROL Library]>[!UICONTROL Extensions]**&#x200B;에서 **[!UICONTROL Sitelinks]** 탭에 계정 수준 공유 사이트 링크가 나열됩니다. **[!UICONTROL Associations]** 탭에는 확장과 계정 엔터티 간의 연결이 나열됩니다.

이 탭을 보려면 [!UICONTROL View Extensions] 권한이 필요합니다. 사이트 링크를 만들고, 편집하고, 삭제하고, 연결을 만들거나 삭제하려면 [!UICONTROL Edit Extensions] 권한이 필요합니다.

[Google 광고 계정](https://support.google.com/google-ads/answer/6372658) 및 [Microsoft Advertising 계정](https://help.ads.microsoft.com/#apex/3/en/52001)당 최대 확장 수에 대한 자세한 내용은 광고 네트워크 도움말을 참조하십시오.

### 사용 가능한 작업

* [공유 사이트링크 만들기](#sitelink-create)

* [공유 사이트 링크 설정 편집](#sitelink-edit)

* [공유 사이트 링크 삭제](#sitelink-delete)

* [공유 사이트링크를 계정, 캠페인 및 광고 그룹과 연결](ad-extension-association-manage.md#sitelink-associate)

* [확장 연결 삭제](ad-extension-association-manage.md#association-delete)

* [선택한 행의 모든 데이터를 클립보드에 복사](#copy-to-clipboard)

## 공유 사이트링크 만들기 {#sitelink-create}

1. 주 메뉴에서 **[!UICONTROL Library]>[!UICONTROL Extensions]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Sitelinks]** 탭을 클릭합니다.

1. **[!UICONTROL Create Sitelink]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Basic Settings]**&#x200B;에서 광고 네트워크 및 계정을 선택합니다.

1. [공유된 사이트 링크 설정](#shared-sitelink-settings)을 입력하십시오.

1. **[!UICONTROL Review and Save]**&#x200B;을(를) 클릭합니다.

1. 설정을 검토합니다. 설정을 변경하려면 해당 섹션에서 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

사이트 링크를 만든 후 [계정, 캠페인 또는 광고 그룹과 연결](ad-extension-association-manage.md#sitelink-associate)하세요.

## 공유 사이트 링크 설정 편집 {#sitelink-edit}

공유 사이트링크를 한 번에 하나씩 편집할 수 있습니다. 만든 후에는 시작 날짜를 변경할 수 없습니다.

1. 주 메뉴에서 **[!UICONTROL Library]>[!UICONTROL Extensions]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Sitelinks]** 탭을 클릭합니다.

1. 하나의 사이트링크 옆에 있는 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. [공유 사이트 링크 설정](#shared-sitelink-settings)을(를) 편집합니다.

1. **[!UICONTROL Review and Save]**&#x200B;을(를) 클릭하고 설정을 검토한 다음 **[!UICONTROL Update]**&#x200B;을(를) 클릭합니다.

사이트 링크의 값을 클릭하여 데이터 테이블에서 사이트 링크의 **[!UICONTROL Base URL]** 또는 **[!UICONTROL Tracking Template]**&#x200B;을(를) 직접 편집할 수도 있습니다.

## 공유 사이트 링크 삭제 {#sitelink-delete}

1. 주 메뉴에서 **[!UICONTROL Library]>[!UICONTROL Extensions]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Sitelinks]** 탭을 클릭합니다.

1. 삭제할 각 공유 사이트 링크 옆에 있는 확인란을 선택합니다.

   여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)&quot;을 참조하십시오.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

라이브러리에서 공유 사이트 링크를 삭제하지 않고 연결을 제거하려면 [연결을 삭제](ad-extension-association-manage.md#association-delete)하십시오.

## 선택한 행의 모든 데이터를 클립보드에 복사 {#copy-to-clipboard}

보기에 표시되는 적용된 필터 및 열에 따라 선택한 행에 표시되는 정보를 복사합니다. 정보는 탭으로 구분된 값(TSV)으로 저장됩니다.

1. 데이터를 복사할 각 행 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Copy]**&#x200B;을(를) 클릭합니다.

## 공유 사이트 링크 설정 {#shared-sitelink-settings}

추가 정책 및 sitelink 불승인 사유에 대해서는 [Google Ads sitelink 요구 사항](https://support.google.com/adspolicy/answer/1054210) 및 [Microsoft Advertising sitelink 요구 사항](https://help.ads.microsoft.com/#apex/ads/en/ext60206)을 참조하십시오.

### [!UICONTROL Sitelink]

**[!UICONTROL Link Name]:** 링크에 표시할 텍스트입니다. 최대 25개의 1바이트 문자 또는 12개의 2바이트 문자를 포함할 수 있습니다. 링크 텍스트는 계정 또는 캠페인 내에서 고유해야 합니다.

>[!NOTE]
>
>([!DNL Google Ads]) 데스크톱 및 태블릿의 광고에 35자로 된 기존 텍스트가 표시되지만 모바일 장치에서는 표시되지 않습니다.

**[!UICONTROL Status]:** 사이트 링크의 표시 상태: **[!UICONTROL Active]** 또는 기존 사이트 링크의 **[!UICONTROL Deleted]**. 기본적으로 새 사이트링크가 활성화됩니다.

**[!UICONTROL Description Line 1], [!UICONTROL Description Line 2]:** 광고 네트워크에서 링크 텍스트 아래에 표시할 수 있는 추가 텍스트입니다. 설명을 포함하려면 두 필드를 모두 입력합니다. 각 문자에는 최대 35개의 1바이트 문자 또는 17개의 2바이트 문자가 포함될 수 있습니다.

**[!UICONTROL Start Date]:**(선택 사항이며, 만들기만 해당) 사이트링크가 표시될 수 있는 첫 번째 날짜입니다. 기본값은 현재 날짜입니다. 미래 날짜를 지정하려면 MM/DD/YYYY 형식으로 입력하거나 날짜 선택기를 사용합니다. 기존 사이트링크에 대한 시작 날짜는 읽기 전용입니다.

**[!UICONTROL End Date]:**(선택 사항) 사이트 링크가 표시될 수 있는 마지막 날짜입니다. 기본적으로 사이트링크가 무기한으로 표시될 수 있습니다. 종료 날짜를 지정하려면 MM/DD/YYYY 형식으로 입력하거나 날짜 선택기를 사용합니다.

**[!UICONTROL Mobile Preference]:**(선택 사항) 네트워크에서 데스크톱 또는 태블릿 사용자가 아닌 모바일 장치 사용자에게 확장을 표시하려고 할 수 있습니다. 기본적으로 이 옵션은 활성화되어 있지 않으며, 확장은 모든 장치 유형에 표시될 수 있습니다. 네트워크는 기본 장치 유형에서 확장을 표시한다고 보장하지 않습니다.

### [!UICONTROL URL Options]

{{$include /help/_includes/base-url-keyword-ad-sitelink.md}}

**[!UICONTROL Tracking Template]:**(선택 사항) 랜딩 페이지 리디렉션 및 추적 매개 변수를 포함한 추적 URL과 매개 변수에 포함된 최종 랜딩 페이지 URL입니다. 예: `https://www.trackingservice.example.com/?url={lpurl}&source={network}&id=5`.

이 보기에서 [!UICONTROL Base URL] 및 [!UICONTROL Tracking Template]에 입력한 값은 `http://` 또는 `https://`(으)로 시작해야 하며 공백을 포함할 수 없습니다.

* 캠페인 설정에 **[!UICONTROL EF Redirect]** 및 **[!UICONTROL Auto Upload]**&#x200B;이(가) 포함된 경우 레코드를 저장할 때 검색, 소셜 및 Commerce에서 자동으로 리디렉션 및 추적 코드 접두사를 추가합니다.

* 최종 URL을 포함하는 매개 변수의 경우 [Microsoft Advertising 설명서](https://help.ads.microsoft.com/#apex/3/en/56799) 또는 [Google Ads ValueTrack 설명서](https://support.google.com/google-ads/answer/6305348)의 &quot;추적 템플릿만&quot; 매개 변수를 참조하십시오.

* 앰퍼샌드(`&`)로 구분된 URL 매개 변수 및 캠페인 수준 사용자 지정 매개 변수와 서드파티 리디렉션 및 추적을 포함할 수 있습니다.

* 가장 세분화된 수준의 추적 템플릿은 상위 수준의 템플릿을 무시합니다.

>[!NOTE]
>
>* 최종 URL이 있는 계정의 경우, 기본 URL은 랜딩 페이지 도메인 또는 하위 도메인 내에 리디렉션을 포함할 수 있지만, 랜딩 페이지 도메인 외부에는 포함될 수 없습니다. 광고 네트워크는 도메인을 추출하여 디스플레이 URL을 만듭니다.
>* ([!DNL Google Ads]) 캠페인 또는 광고 그룹의 각 사이트 링크에는 약 80%의 고유 콘텐츠가 있는 고유한 랜딩 페이지가 있어야 합니다. 동일한 페이지의 여러 앵커에 대한 링크를 별도의 사이트링크 랜딩 페이지로 사용하지 마십시오.
>* ([!DNL Google Ads]) 사이트 링크 또는 키워드 수준에서 추적 템플릿을 업데이트하면 관련 광고가 다시 제출되어 검토됩니다. 계정, 캠페인 또는 광고 그룹 수준에서 업데이트하면 광고가 다시 제출되지 않습니다.
>* ([!DNL Microsoft Advertising]) 승인을 위해 광고를 다시 제출하지 않고 모든 수준에서 추적 템플릿을 업데이트할 수 있습니다.
>* ([!DNL Google Ads]) 병렬 추적을 사용하는 소스의 클릭으로 대체되지 않는 매크로를 사용하지 마십시오. 매크로가 필요한 경우 Adobe 계정 팀은 고객 지원 센터 또는 구현 팀과 협력하여 매크로를 추가합니다.

## 사이트링크에 대한 성능 데이터 {#sitelink-performance}

Search, Social 및 Commerce은 광고 확장에 대한 클릭 수와 결과 전환을 확장이 표시되는 광고와 연결된 키워드로 매핑합니다. 검색, 소셜 및 Commerce에서는 확장 수준 비용 및 클릭 데이터를 사용할 수 없습니다.

[!UICONTROL Transaction Report]에서 `sl:See Current Offers`과(와) 같은 `sl:<Sitelink text>`의 [!UICONTROL Link Type] 값은 광고 자체가 아닌 사이트 링크에서 트랜잭션을 식별합니다. &quot;[거래 보고서](/help/search-social-commerce/new-ui/reports/management/basic-advanced/transaction-report.md)&quot;을(를) 참조하십시오.

광고 네트워크의 인터페이스에서 확장 수준 비용을 보고 데이터를 클릭할 수 있습니다.

>[!MORELIKETHIS]
>
>* [Google 광고 공유 콜아웃 확장 관리](callout-extension-manage.md)
>* [광고 확장 연결 관리](ad-extension-association-manage.md)
