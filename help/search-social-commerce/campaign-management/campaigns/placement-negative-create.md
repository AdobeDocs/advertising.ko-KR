---
title: 부정적인 배치 만들기
description: 에 대한 부정적인 배치를 만드는 방법 알아보기 [!DNL Google Ads] 캠페인 및 광고 그룹.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 0%

---

# 다음에 대해 만들기 [!DNL Google Ads] 부정적 배치

*[!DNL Google Ads]계정만*

에 대해 부정적인 배치를 만들 수 있습니다. [!DNL Google Ads] 디스플레이 네트워크를 타깃팅하는 캠페인의 광고 그룹. 네거티브 배치는 디스플레이 네트워크에서 광고를 트리거하지 않는 사이트입니다.

>[!NOTE]
>에서 부정적인 배치를 만들고 편집할 수도 있습니다. [광고 그룹 설정](/help/search-social-commerce/campaign-management/campaigns/ad-group-manage.md) 및 [캠페인 설정](/help/search-social-commerce/campaign-management/campaigns/campaign-manage.md).

>[!TIP]
>한 번에 여러 개의 부정적인 배치를 만들려면 [캠페인 일괄 시트](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-about.md).

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**. 하위 메뉴에서 **[!UICONTROL Live]> [!UICONTROL Placements] >[!UICONTROL Negatives]**.

1. 데이터 테이블 위의 도구 모음에서 ![만들기](/help/search-social-commerce/assets/add.png "만들기")을 클릭한 다음 을 클릭합니다 **[!UICONTROL Campaign]** 캠페인 수준의 부정적인 배치 또는 **[!UICONTROL Ad Group]** 광고 그룹 수준의 부정적인 배치를 만듭니다.

1. 광고 네트워크, 계정, 캠페인 및 (해당되는 경우) 광고 그룹을 선택한 다음 를 클릭합니다. **[!UICONTROL Continue]**.

1. 음수 웹 사이트 URL을 입력합니다.

   여러 문자열을 지정하려면 쉼표로 구분하거나 별도의 줄에 입력합니다. 유효한 형식은 다음과 같습니다.

   * 웹 사이트: 유효한 URL(예: www.example.com)을 입력합니다. https://support.google.com/google-ads/answer/2454012의 &quot;제외 URL 추가 방법&quot;에서 허용되는 형식을 참조하십시오.

   * 주제, 카테고리 또는 문서 세로 다음을 참조하십시오 [[!DNL Google Ads] 지침](https://support.google.com/google-ads/editor/answer/30517) 및 a [모든 수직 분야 목록](https://developers.google.com/adwords/api/docs/appendix/verticals). 예: `category::Industries > Energy & Utilities > Oil & Gas`.

1. 클릭 **[!UICONTROL Post]**.

>[!MORELIKETHIS]
>
>* [배치 기본 정보](placement-about.md)
>* [바인딩 가능한 배치 관리](placement-manage.md)
>* [배치 및 음수 배치 상태 변경](placement-status-edit.md)

