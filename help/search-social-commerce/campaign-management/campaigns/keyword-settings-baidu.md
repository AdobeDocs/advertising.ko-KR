---
title: '[!DNL Baidu] 키워드 설정'
description: ' [!DNL Baidu] 키워드에 대한 설정을 참조합니다.'
exl-id: 3b3a578b-06f1-486f-9ade-9104e0a1dd5f
feature: Search Campaign Management
source-git-commit: e16bc62127a708de8f4deb1eddfa53a14405cbc2
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 0%

---

# [!DNL Baidu] 키워드 설정

## [!UICONTROL Keyword Details]

**[!UICONTROL Keywords]:** 키워드입니다. 키워드당 최대 길이는 30개의 싱글바이트 또는 15개의 더블바이트 문자입니다

최대 2000개의 키워드를 입력하거나 붙여넣을 수 있습니다. 여러 키워드를 쉼표로 구분하거나 별도의 줄에 입력합니다. 다음 구문을 사용합니다.

* 광범위한 일치의 `keyword`
* 구 일치에 대한 `"keyword"`
* 정확히 일치할 경우 `[keyword]`

>[!NOTE]
>
>* [!DNL Baidu]에서는 광고 그룹당 키워드당 일치 유형을 하나만 사용할 수 있습니다. 예를 들어 광고 그룹 1은 `"keyword"`과(와) `[keyword]`을(를) 모두 포함할 수 없습니다.
>* [!UICONTROL Keywords] > [!UICONTROL Negatives] 보기, 광고 그룹 및 캠페인 설정에서 부정적인 키워드를 만들 수 있습니다.
>* [!DNL Baidu] 키워드를 변경하면 기존 키워드가 삭제되고 새 키워드 ID로 새 키워드가 만들어집니다. 그러나 일치 유형을 변경해도 기존 키워드는 삭제되지 않습니다.

**[!UICONTROL Status]:** 키워드의 표시 상태: *활성* 또는 *일시 중지됨*. 새 키워드의 기본값은 *Active*&#x200B;입니다.

## [!UICONTROL Bids]

<!-- **[!UICONTROL Bid]:** -->

{{$include /help/_includes/bid-keyword.md}}

## URL 옵션

**[!UICONTROL Base URL]:**(키워드 수준의 추적만 사용하는 캠페인; 선택 사항) 사용자가 광고를 클릭할 때 사용하는 랜딩 페이지 URL입니다. 다음을 포함할 수 있습니다.
타사 리디렉션 및 추적 코드. 값을 입력하면 광고의 기본 URL이 무시됩니다.

레코드를 저장하면 기본 URL에 캠페인이나 계정에 대해 구성된 추가 매개 변수가 포함됩니다.

Adobe Advertising 전환 추적 서비스를 사용하고 캠페인 설정에 [!UICONTROL EF Redirect] 사용 및 키워드 수준에서 추적 추가가 포함된 경우 검색, 소셜 및 Commerce에서 자동으로 자체 클릭 추적 코드를 추가합니다.

>[!MORELIKETHIS]
>
>* [키워드 관리](/help/search-social-commerce/campaign-management/campaigns/keyword-manage.md)
