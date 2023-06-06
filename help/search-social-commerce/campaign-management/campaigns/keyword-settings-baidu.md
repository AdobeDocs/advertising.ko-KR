---
title: "[!DNL Baidu] 키워드 설정"
description: 다음에 대한 설정 참조 [!DNL Baidu] 키워드.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---

# [!DNL Baidu] 키워드 설정

## [!UICONTROL Keyword Details]

**[!UICONTROL Keywords]:** 키워드. 키워드당 최대 길이는 30개의 싱글바이트 또는 15개의 더블바이트 문자입니다

최대 2000개의 키워드를 입력하거나 붙여넣을 수 있습니다. 여러 키워드를 쉼표로 구분하거나 별도의 줄에 입력합니다. 다음 구문을 사용합니다.

* `keyword` 광범위한 일치용
* `"keyword"` 구문 일치
* `[keyword]` 정확한 일치

>[!NOTE]
>
>* [!DNL Baidu] 광고 그룹당 키워드당 하나의 일치 유형만 허용합니다. 예를 들어 광고 그룹 1은 두 가지를 모두 포함할 수 없습니다 `"keyword"` 및 `[keyword]`.
>* 에서 부정적인 키워드를 만들 수 있습니다. [!UICONTROL Keywords] > [!UICONTROL Negatives] 광고 그룹 및 캠페인 설정에서 및 를 봅니다.
>* 변경 [!DNL Baidu] 키워드는 기존 키워드를 삭제하고 새 키워드 ID로 새 키워드를 만듭니다. 그러나 일치 유형을 변경해도 기존 키워드는 삭제되지 않습니다.


**[!UICONTROL Status]:** 키워드의 표시 상태: *활성* 또는 *일시 중지됨*. 새 키워드의 기본값은 입니다 *활성*.

## [!UICONTROL Bids]

<!-- **[!UICONTROL Bid]:** -->

{{$include /help/_includes/bid-keyword.md}}

## URL 옵션

**[!UICONTROL Base URL]:** (키워드 수준 추적만 사용하는 캠페인; 선택 사항) 사용자가 광고를 클릭할 때 사용하는 랜딩 페이지 URL입니다. 여기에는 서드파티 리디렉션 및 추적 코드가 포함될 수 있습니다. 값을 입력하면 광고의 기본 URL이 무시됩니다.

레코드를 저장하면 기본 URL에 캠페인이나 계정에 대해 구성된 추가 매개 변수가 포함됩니다.

Adobe 광고 전환 추적 서비스를 사용하는 경우 캠페인 설정에 다음을 사용하는 것이 포함됩니다. [!UICONTROL EF Redirect] 키워드 수준에서 추적을 추가하면 검색, 소셜 및 상거래가 자동으로 자체 클릭 추적 코드를 추가합니다.

>[!MORELIKETHIS]
>
>* [키워드 관리](/help/search-social-commerce/campaign-management/campaigns/keyword-manage.md)

