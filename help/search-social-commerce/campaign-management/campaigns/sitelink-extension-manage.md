---
title: 공유 사이트 링크 관리
description: 공유 사이트링크 확장을 만들고 관리하는 방법을 알아봅니다.
exl-id: e510f53b-f48c-4129-887c-351a840b8398
feature: Search Campaign Management
source-git-commit: c3b8e387cfc38d195e77761791e689fd094d8f39
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# 공유 사이트 링크 관리

*[!DNL Google Ads]및 [!DNL Microsoft Advertising]만*

[!UICONTROL Extensions] > [!UICONTROL Sitelinks] 라이브러리에서 동기화된 [!DNL Google Ads] 또는 [!DNL Microsoft Advertising] 계정에 대한 계정 수준 공유 사이트링크를 만들고 관리합니다.

## 공유 사이트링크 만들기

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다. 하위 메뉴에서 **[!UICONTROL Live]> [!UICONTROL Extensions] >[!UICONTROL Sitelinks]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위의 도구 모음에서 ![만들기](/help/search-social-commerce/assets/add.png "만들기")를 클릭합니다.

1. 광고 네트워크 및 계정 이름을 선택한 다음 **[!UICONTROL Continue]**&#x200B;을(를) 클릭합니다.

1. [공유된 사이트 링크 설정](#shared-sitelink-settings)을 입력하십시오.

1. **[!UICONTROL Post]**&#x200B;을(를) 클릭합니다.

사이트 링크를 만들면 [계정, 캠페인 또는 광고 그룹에 할당](sitelink-extension-associate.md)할 수 있습니다.

## 공유 사이트 링크 설정 편집

공유 사이트링크를 한 번에 하나씩 편집할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다. 하위 메뉴에서 **[!UICONTROL Live]> [!UICONTROL Extensions] >[!UICONTROL Sitelinks]**&#x200B;을(를) 클릭합니다.

1. 편집할 사이트 링크 옆에 있는 확인란을 선택합니다.

1. 데이터 테이블 위의 도구 모음에서 ![편집](/help/search-social-commerce/assets/edit.png "편집")을 클릭합니다.

1. [공유 사이트 링크 설정](#shared-sitelink-settings)을(를) 편집합니다.

1. **[!UICONTROL Post]**&#x200B;을(를) 클릭합니다.

## 공유 사이트 링크 삭제

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다. 하위 메뉴에서 **[!UICONTROL Live]> [!UICONTROL Extensions] >[!UICONTROL Sitelinks]**&#x200B;을(를) 클릭합니다.

1. 삭제할 각 공유 사이트 링크 옆에 있는 확인란을 선택합니다.

   여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)&quot;을 참조하십시오.

1. 도구 모음에서 ![자세히](/help/search-social-commerce/assets/more.png "자세히")를 클릭하고 **[!UICONTROL Delete]**&#x200B;을(를) 선택합니다.

1. 확인 메시지에서 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

## 공유 사이트 링크 설정 {#shared-sitelink-settings}

추가 정책 및 sitelink 불승인 사유에 대해서는 [[!DNL Google Ads]](https://support.google.com/adspolicy/answer/1054210) 및 [[!DNL Microsoft Advertising]](https://help.ads.microsoft.com/#apex/ads/en/ext60206) sitelink 확장 요구 사항을 참조하십시오.

### [!UICONTROL Sitelink]

**[!UICONTROL Link Name]:** 링크에 표시할 텍스트입니다. 최대 25개의 1바이트 문자 또는 12개의 2바이트 문자를 포함할 수 있습니다. 링크 텍스트는 계정 또는 캠페인 내에서 고유해야 합니다.

>[!NOTE]
>
>([!DNL Google Ads]) 데스크톱 및 태블릿의 광고에 35자로 된 기존 텍스트가 표시되지만 모바일 장치에서는 표시되지 않습니다.

**[!UICONTROL Status]:** 사이트 링크의 표시 상태: *[!UICONTROL Active]* 또는 *[!UICONTROL Deleted]*(기존 사이트 링크만 해당). 새 사이트 링크의 기본값은 *[!UICONTROL Active]*&#x200B;입니다.

**[!UICONTROL Description Line 1], [!UICONTROL Description Line 2]:** 검색 엔진이 링크 텍스트 아래에 표시할 수 있는 추가 텍스트입니다. 설명을 포함하려면 두 설명 필드 모두에 대한 값을 입력합니다. 각 설명 필드에는 최대 35개의 1바이트 문자 또는 17개의 2바이트 문자가 포함될 수 있습니다.

**[!UICONTROL Start Date]:**(기존 사이트 링크가 있거나 사이트 링크만 없는 캠페인; 선택 사항) 캠페인에서 사이트 링크가 광고와 함께 표시될 수 있는 첫 번째 날짜입니다. 새 사이트 링크의 기본값은 현재 날짜입니다. 미래의 시작 날짜를 지정하려면 MM/DD/YYYY 또는 M/D/YYYY 형식으로 날짜를 입력하거나   날짜를 선택합니다.

**[!UICONTROL End Date]:**(선택 사항) 캠페인에서 사이트 링크가 광고와 함께 표시될 수 있는 마지막 날짜입니다. 기본적으로 사이트링크가 무기한으로 표시될 수 있습니다. 종료 날짜를 지정하려면 MM/DD/YYYY 또는 M/D/YYYY 형식으로 날짜를 입력하거나   날짜를 선택합니다.

**[!UICONTROL Mobile Preference]:**(선택 사항) 네트워크에서 데스크톱 또는 태블릿 사용자가 아닌 모바일 장치 사용자에게 광고 확장을 표시하려고 할 수 있습니다. 기본적으로 옵션은 활성화되어 있지 않고 광고 확장 기능은 장치 유형에 표시됩니다.

>[!NOTE]
>
>네트워크에서는 기본 장치 유형에 광고 확장을 표시할 수 없습니다.

### [!UICONTROL Tracking URLs]

**[!UICONTROL Base URL]** 검색 엔진 사용자가 광고를 클릭할 때 사용하는 랜딩 페이지 URL입니다. 페이지의 콘텐츠를 결정하는 매개 변수를 포함합니다. 값을 입력하면 광고의 기본 URL이 무시됩니다.

레코드를 저장하면 기본 URL에 캠페인이나 계정에 대해 구성된 추가 매개 변수가 포함됩니다.

>[!NOTE]
>
>* (최종 URL이 있는 계정) 기본 URL은 랜딩 페이지 도메인 또는 하위 도메인 내에 리디렉션을 포함할 수 있지만 랜딩 페이지 도메인 외부에는 리디렉션을 포함하지 않습니다. 광고 네트워크는 이 URL에서 도메인을 추출하고, 광고의 선택적 표시 경로를 추가하여 광고의 표시 URL을 만듭니다.
>* ([!DNL Google Ads]) 캠페인 또는 광고 그룹의 각 사이트 링크에는 고유한 랜딩 페이지가 있어야 하며 각 사이트 링크 랜딩 페이지의 콘텐츠에는 약 80%의 고유한 콘텐츠가 있어야 합니다. 예를 들어 동일한 페이지 내에서 여러 앵커에 대한 링크가 있는 사이트링크를 가질 수 없습니다.
>* ([!DNL Google Ads]) 병렬 추적을 활성화하는 소스의 클릭에 대체되지 않는 매크로를 사용하지 마십시오. 광고주가 매크로를 사용해야 하는 경우 Adobe 계정 팀은 고객 지원 팀 또는 구현 팀과 협력하여 매크로를 추가해야 합니다.

**[!UICONTROL Tracking Template]:**(선택 사항) 모든 랜딩 외부 도메인 리디렉션 및 추적 매개 변수를 지정하고 매개 변수에 최종/랜딩 페이지 URL을 임베드하는 추적 템플릿 또는 추적 URL입니다. 예: 리디렉션을 포함하는 `{lpurl}?source={network}&id=5` 또는 `http://www.trackingservice.example.com/?url={lpurl}?source={network}&id=5`.

* 캠페인 설정에 &quot;[!UICONTROL EF Redirect]&quot; 및 &quot;자동 업로드&quot;가 포함된 경우에 적용되는 Adobe Advertising 전환 추적의 경우 레코드를 저장할 때 Search, Social 및 Commerce에 자체 클릭 추적 코드가 자동으로 접두사로 추가됩니다.

* 최종 URL을 포함하는 지원되는 매개 변수에 대해서는 [[!DNL Google Ads] documentation](https://support.google.com/google-ads/answer/6305348)의 &quot;사용 가능한 [!DNL ValueTrack] 매개 변수&quot;에 대한 섹션에서 ([!DNL Microsoft Advertising]만 해당) [[!DNL Microsoft Advertising] documentation](https://help.ads.microsoft.com/#apex/3/en/56799) 또는 ([!DNL Google Ads]만 해당) &quot;추적 템플릿 전용&quot; 매개 변수를 참조하십시오.

* 필요에 따라 URL 매개 변수와 캠페인에 대해 정의된 사용자 지정 매개 변수를 앰퍼샌드(&amp;)로 구분하여 포함할 수 있습니다(예: `{lpurl}?matchtype={matchtype}&device={device}`).

* 원할 경우 서드파티 리디렉션 및 추적을 추가할 수 있습니다.

>[!NOTE]
>
>* 캠페인 설정에 &quot;[!UICONTROL EF Redirect]&quot; 및 &quot;[!UICONTROL Auto Upload]&quot;이(가) 포함된 경우 레코드를 저장할 때 Search, Social 및 Commerce에 자체 리디렉션 및 추적 코드 접두사가 자동으로 추가됩니다.
>* 가장 세분화된 수준의 추적 템플릿은 모든 상위 수준의 값을 재정의합니다. 예를 들어 계정 설정과 키워드 설정 모두에 값이 포함된 경우 키워드 값이 적용됩니다.
>* ([!DNL Google Ads]) 사이트 링크 또는 키워드 수준에서 추적 템플릿을 업데이트하면 관련 광고가 다시 제출되어 검토됩니다. 승인을 위해 광고를 다시 제출하지 않고도 계정, 캠페인 또는 광고 그룹 수준에서 추적 템플릿을 업데이트할 수 있습니다.
>* ([!DNL Microsoft Advertising]) 승인을 위해 광고를 다시 제출하지 않고 모든 수준에서 추적 템플릿을 업데이트할 수 있습니다.
>* [!DNL Google Ads]의 경우 병렬 추적을 활성화하는 소스의 클릭에 대체되지 않는 매크로를 사용하지 마십시오. 광고주가 매크로를 사용해야 하는 경우 Adobe 계정 팀은 고객 지원 팀 또는 구현 팀과 협력하여 매크로를 추가해야 합니다.

>[!MORELIKETHIS]
>
>* [사이트 링크 확장 정보](sitelink-extension-about.md)
>* [공유 사이트링크를 계정, 캠페인 및 광고 그룹과 연결](sitelink-extension-associate.md)
