---
title: "[!DNL Yandex] 키워드 설정"
description: 다음에 대한 설정 참조 [!DNL Yandex] 키워드.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---

# [!DNL Yandex] 키워드 설정

Yandex 키워드는 검색 및 표시(콘텐츠) 네트워크 모두에 사용됩니다.

<!-- Note to self: Yandex doesn't have separate website placements for display; users use keywords for the sites/parts of the content network on which they want to advertise. -->

## [!UICONTROL Keyword Details]

**[!UICONTROL Keywords]:** 모든 키워드 구문 포함 [Yandex 일치 유형 구문](https://yandex.com/support/direct/keywords/symbols-and-operators.html) 키워드. 각 키워드는 정지어를 제외하고 최대 7개의 단어를 사용할 수 있습니다.

최대 2000개의 키워드를 입력하거나 붙여넣을 수 있습니다. 여러 키워드를 쉼표로 구분하거나 별도의 줄에 입력합니다.

>[!NOTE]
>
>* 변경 [!DNL Yandex] 키워드 또는 일치 유형은 기존 키워드를 삭제하고 새 키워드를 만듭니다.
>* 각 Yandex 광고 그룹에는 최대 200개의 키워드가 포함될 수 있습니다.


**[!UICONTROL Status]:** 키워드의 표시 상태: *활성* 또는 *일시 중지됨*. 새 키워드의 기본값은 입니다 *활성*.

## [!UICONTROL Bids]

<!-- **[!UICONTROL Bid]:** -->

{{$include /help/_includes/bid-keyword.md}}

## 자리 표시자

**[!UICONTROL Param1]** **[!UICONTROL Param2]:** 값 `{param1}` 및 `{param2}` 키워드를 사용하여 광고를 표시할 때 광고 및 사이트링크의 기본 URL에서 {param1} 및 {param2}의 인스턴스를 대체하는 대체 변수입니다. 최대 길이는 255바이트입니다.

특수 문자는 UTF-8로 자동 인코딩됩니다. 예를 들어 연결된 광고에 기본 URL이 &quot;http://www.example.com/{param1}이고 키워드 수준의 값이 {param1}인 경우 광고는 &quot;shoes/flats.html http://www.example.com/shoes%2Fflats.html&quot;으로 이어집니다.

>[!MORELIKETHIS]
>
>* [키워드 관리](/help/search-social-commerce/campaign-management/campaigns/keyword-manage.md)

