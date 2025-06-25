---
title: 부정적인 배치 만들기
description: ' [!DNL Google Ads] 캠페인 및 광고 그룹에 대해 부정적인 배치를 만드는 방법을 알아봅니다.'
exl-id: 9cc2dd8d-5563-4e02-af8f-6181165494d8
feature: Search Campaign Management
source-git-commit: d0f1c413134a0868ddec79ded7672af316267edd
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 0%

---

# [!DNL Google Ads]개의 부정적 배치에 대해 만들기

*[!DNL Google Ads]개의 계정만*

디스플레이 네트워크를 대상으로 하는 캠페인에서 [!DNL Google Ads] 광고 그룹에 대해 부정적인 배치를 만들 수 있습니다. 네거티브 배치는 디스플레이 네트워크에서 광고를 트리거하지 않는 사이트입니다.

>[!NOTE]
>[광고 그룹 설정](/help/search-social-commerce/campaign-management/campaigns/ad-group-manage.md) 및 [캠페인 설정](/help/search-social-commerce/campaign-management/campaigns/campaign-manage.md)에서 부정적인 배치를 만들고 편집할 수도 있습니다.

>[!TIP]
>한 번에 여러 개의 부정적인 배치를 만들려면 [캠페인 일괄 시트](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-about.md)를 사용하십시오.

1. 메인 메뉴에서 **[!UICONTROL Search, Social, & Commerce]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다. 하위 메뉴에서 **[!UICONTROL Live]> [!UICONTROL Placements] >[!UICONTROL Negatives]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위의 도구 모음에서 ![만들기](/help/search-social-commerce/assets/add.png "만들기")를 클릭한 다음 **[!UICONTROL Campaign]**&#x200B;을 클릭하여 캠페인 수준의 부정적인 배치를 만들거나 **[!UICONTROL Ad Group]**&#x200B;을 클릭하여 광고 그룹 수준의 부정적인 배치를 만듭니다.

1. 광고 네트워크, 계정, 캠페인 및 (해당되는 경우) 광고 그룹을 선택한 다음 **[!UICONTROL Continue]**&#x200B;을(를) 클릭합니다.

1. 음수 웹 사이트 URL을 입력합니다.

   여러 문자열을 지정하려면 쉼표로 구분하거나 별도의 줄에 입력합니다. 유효한 형식은 다음과 같습니다.

   * 웹 사이트: 유효한 URL(예: www.example.com)을 입력합니다. https://support.google.com/google-ads/answer/2454012의 &quot;제외 URL 추가 방법&quot;에서 허용되는 형식을 참조하십시오.

   * 주제, 카테고리 또는 문서 세로 [[!DNL Google Ads] 지침](https://support.google.com/google-ads/editor/answer/30517) 및 [모든 수직 항목의 목록](https://developers.google.com/adwords/api/docs/appendix/verticals)을 참조하세요. 예: `category::Industries > Energy & Utilities > Oil & Gas`

1. **[!UICONTROL Post]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [배치 정보](placement-about.md)
>* [바인딩 가능한 배치 관리](placement-manage.md)
>* [배치 및 음수 배치 상태 변경](placement-status-edit.md)
