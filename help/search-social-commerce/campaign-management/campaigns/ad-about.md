---
title: 광고 관리
description: 사용 가능한 광고 유형을 포함하여 검색, 소셜 및 Commerce의 광고에 대해 알아봅니다.
exl-id: 01bd211d-fe6b-4329-90e1-0e54d626c125
feature: Search Campaign Management
source-git-commit: 7e4d2aa502f26b480a5fd76d68411586c24f68b2
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---

# 광고 정보

*[!DNL Google Ads], [!DNL Microsoft Advertising], [!DNL Yahoo! Japan Ads], [!DNL Yandex] 및 기존 [!DNL Baidu] 계정만*

광고는 대상 웹 사이트(콘텐츠 또는 배치 대상 캠페인), 사용자가 광고 그룹(검색 캠페인) 또는 웹 사이트의 콘텐츠([!DNL Google Ads] 검색 전용 캠페인의 동적 검색 광고)에서 키워드 중 하나를 검색하는 경우 또는 사용자가 [!DNL Google Merchant Center] 또는 [!DNL Microsoft Merchant Center] 제품 피드의 항목 중 하나와 관련된 검색을 수행하는 경우([!DNL Google Ads]의 쇼핑 광고 또는 [!DNL Microsoft Advertising] 캠페인의 제품 광고)에 표시될 수 있습니다.

## 사용 가능한 광고 유형

동기화된 광고 네트워크 계정 내에서 광고 그룹에 대해 지원되는 광고 유형을 만들고 관리할 수 있습니다.

* 검색 네트워크를 대상으로 하는 캠페인의 광고 그룹에 대한 **텍스트 광고 또는 확장된 텍스트 광고**. 텍스트 광고에는 광고 그룹 또는 캠페인 수준 매개 변수를 오버라이드하는 선택적 추적 매개 변수가 포함될 수 있습니다. 광고 네트워크에 따라 확장/확장 텍스트 광고 또는 표준 텍스트 광고를 만들 수 있습니다.

* [!DNL Microsoft Audience Network]의 [!DNL Microsoft Advertising] 캠페인에 대한 교차 장치, 기본 **대상 광고**. 캠페인 설정에 따라 대상 광고에 대한 두 가지 옵션이 있습니다.

   * 캠페인이 판매자 센터 상점에 연결된 경우 광고 네트워크에서 상점의 제품 정보를 사용하여 캠페인에 대한 광고 피드 기반 광고를 자동으로 생성하도록 합니다. 캠페인에 대한 피드 기반 광고를 만들 필요는 없지만 사용자 타겟팅을 사용하여 광고 그룹을 만들어야 합니다.

   * 캠페인이 판매자 센터 계정에 연결되어 있지 않은 경우, 여러 텍스트 및 이미지 에셋이 포함된 반응형 광고 형식을 사용하여 이미지 기반 대상 광고를 만드십시오. 광고 네트워크는 가장 효과적인 광고 요소 조합을 사용하여 광고를 조합하고 [!DNL MSN], [!DNL Outlook.com] 및 [!DNL Microsoft Edge]과(와) 같은 사이트에 표시합니다.

* 검색 네트워크에서 [!DNL Google Ads] 캠페인에 대한 **통화 전용 광고**. 호출 전용 광고는 전화 번호를 포함하는 텍스트 광고입니다. 필요에 따라 고급 호출 보고를 위해 [!DNL Google Ads]이(가) 할당한 전달 번호를 사용할 수 있습니다.

* 검색 캠페인의 [!DNL Google Ads] 및 [!DNL Microsoft Advertising]개 동적 검색 광고 그룹에 대해 **확장된 동적 검색 광고**(이제 광고 네트워크에서 &quot;동적 검색 광고&quot;라고 함). 동적 검색 광고는 키워드 대신 웹 사이트의 콘텐츠를 사용하여 광고를 표시할 시기를 결정합니다. 광고 네트워크는 동적으로 헤드라인을 생성하고, 랜딩 페이지 URL과 디스플레이 URL을 선택하며, 최종 URL을 자동으로 생성합니다.

  광고 그룹에 대한 특정 동적 검색 대상을 설정하여 콘텐츠가 동적 검색 광고를 타깃팅하는 데 사용되는 웹 사이트의 페이지를 정의할 수 있습니다. [!DNL Google Ads]의 경우 검색, 소셜 및 Commerce에서 동적 검색 대상을 만들 수 있습니다. [!DNL Microsoft Advertising]의 경우 [!DNL Microsoft Advertising] 내에 동적 검색 대상을 만들어야 합니다. [!DNL Google Ads] 캠페인에서는 동적 검색 대상을 만드는 대신 또는 동적 검색 대상을 만드는 것에 추가하여 캠페인의 &quot;[!DNL DSA Options]&quot; 섹션에 웹 사이트 도메인과 언어를 선택적으로 지정할 수 있습니다.

  사용자의 검색어가 키워드 기반 캠페인 중 하나의 키워드와 정확히 일치하는 경우 동적 검색 광고 대신 키워드 기반 캠페인의 광고가 표시됩니다. 사용자의 검색어가 키워드 중 하나와 광범위하게 일치하거나 구문이 일치하고 동적 검색 광고의 광고 등급이 더 높은 경우 광고 네트워크에 키워드 타깃팅된 광고 대신 동적 검색 광고가 표시됩니다.

  동적 검색 광고에 대한 자세한 내용은 [[!DNL Google Ads] 설명서](https://support.google.com/google-ads/answer/2471185) 및 [[!DNL Microsoft Advertising] 설명서](https://help.ads.microsoft.com/#apex/ads/en/56794)를 참조하세요.

* [!DNL Microsoft Advertising] 검색 캠페인에 대한 **멀티미디어 광고**. 멀티미디어 광고는 눈에 띄는 메인 라인과 사이드바 위치에 표시되는 대형 이미지 광고이며, 페이지당 하나의 멀티미디어 광고만 표시됩니다. 여기에는 반응형 광고와 같은 여러 텍스트 및 이미지 자산이 포함될 수 있으며 광고 네트워크는 광고 요소의 가장 효과적인 조합을 사용하여 광고를 어셈블합니다. 멀티미디어 광고는 텍스트 광고 배치를 대체하지 않습니다.

* 쇼핑 네트워크의 **[!DNL Microsoft Advertising]개 제품(쇼핑) 광고**&#x200B;에 대한 프로모션 라인입니다. 쇼핑 광고는 키워드 대신 기존 [!DNL Microsoft Merchant Center] 제품 피드의 제품을 사용하여 광고를 표시할 방법과 위치를 결정합니다. 광고 복사 및 랜딩 페이지 URL은 피드의 제품 정보에서 자동으로 생성되지만 선택적으로 광고 그룹에 포함할 프로모션 라인을 설정할 수 있습니다.

  [!UICONTROL Campaigns] > [!UICONTROL Campaigns] > [!UICONTROL Product Groups] 보기에서 광고 그룹에 대해 별도의 제품 그룹을 설정하여 [!DNL Microsoft Advertising] 쇼핑 광고와 함께 표시되는 제품을 제어할 수 있습니다.

  제품/쇼핑 광고 워크플로에 대한 자세한 내용은 &quot;[쇼핑 캠페인 구현 [!DNL Microsoft Advertising] 2&rbrace;&quot;을 참조하십시오.  ](/help/search-social-commerce/campaign-management/special-workflows/microsoft-shopping-campaigns.md)  제품 광고에 대한 자세한 내용은 [Microsoft Advertising 설명서](https://help.ads.microsoft.com/#apex/3/en/51082)를 참조하세요.

* 검색 네트워크에서 [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 캠페인에 대한 반응형 검색 광고. 광고 네트워크는 광고 제목 및 설명 세트에서 텍스트 기반 반응형 검색 광고를 동적으로 어셈블하며, 함께 잘 작동하는 조합을 선호합니다. 이 광고에는 최대 3개의 헤드라인, 2개의 설명 및 기본 URL과 선택적 경로1 및 경로2 필드의 사용자 지정 가능한 URL이 포함되어 있습니다. 광고 제목과 설명을 특정 위치에 선택적으로 고정할 수 있습니다.

>[!NOTE]
>
>[!DNL Google Ads]은(는) 광고로 표시된 텍스트 조합에 대한 데이터를 기본 편집기 외부에 제공하지 않습니다. 각 텍스트 조합에 대한 보고에 대한 자세한 내용은 [Google 광고 설명서](https://support.google.com/google-ads/answer/7684791)를 참조하세요.

## [!UICONTROL Ads] 보기

[!UICONTROL Campaigns] > [!UICONTROL Campaigns] > [!UICONTROL Ads] 보기에서 광고를 만들고 편집하고 상태를 변경할 수 있습니다.

## 광고 수준 성능 데이터

광고 수준 데이터는 대부분의 광고 유형에 사용할 수 있습니다.

그러나 [!DNL Google Ads] 동적 검색 광고(DSA), 성능 최대, 스마트 쇼핑 및 [!DNL YouTube] 캠페인에는 사용할 수 없습니다. 캠페인에 대한 총 광고 수준 데이터와 캠페인에 대한 총 데이터 간의 불일치를 예상합니다.

| 광고 네트워크/캠페인/광고 유형 | 데이터 가용성 |
|---|---|
| [!DNL Google Ads] 동적 검색 광고(DSA) | 캠페인, 광고 그룹 |
| 최대 [!DNL Google Ads] 성능 | 캠페인 |
| [!DNL Google Ads] 쇼핑, 스마트 쇼핑 | 캠페인, 광고 그룹 |
| [!DNL Google Ads] [!DNL YouTube] | 캠페인, 광고 그룹 |

>[!MORELIKETHIS]
>
>* [광고 관리](ad-manage.md)
