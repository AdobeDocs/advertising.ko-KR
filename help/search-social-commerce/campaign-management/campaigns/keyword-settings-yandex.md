---
title: '[!DNL Yandex] 키워드 설정'
description: ' [!DNL Yandex] 키워드에 대한 설정을 참조합니다.'
exl-id: 973be0df-9b3c-4f33-b48b-ef1db4ab35da
feature: Search Campaign Management
TQID: https://experienceleague.adobe.com/-PRiQ9myH0XNYF8pc2OVBuLOK-8BpxzqruOP2hzPW0I
product_v2: id: a829a185-511f-4bf8-8dcf-9e684f8011cf
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
source-git-commit: 527ca2bb74de388c13ba1ce5bde3f8be1cead8d0
workflow-type: tm+mt
source-wordcount: 181
ht-degree: 0%

---

# [!DNL Yandex] 키워드 설정

Yandex 키워드는 검색 및 표시(콘텐츠) 네트워크 모두에 사용됩니다.

<!-- Note to self: Yandex doesn't have separate website placements for display; users use keywords for the sites/parts of the content network on which they want to advertise. -->

## [!UICONTROL Keyword Details]

**[!UICONTROL Keywords]:** 키워드에 대한 [Yandex 일치 유형 구문](https://yandex.com/support/direct/keywords/symbols-and-operators.html)을(를) 포함하는 키워드 구문입니다. 각 키워드는 정지어를 제외하고 최대 7개의 단어를 사용할 수 있습니다.

최대 2000개의 키워드를 입력하거나 붙여넣을 수 있습니다. 여러 키워드를 쉼표로 구분하거나 별도의 줄에 입력합니다.

>[!NOTE]
>
>* [!DNL Yandex] 키워드 또는 일치 유형을 변경하면 기존 키워드가 삭제되고 새 키워드가 만들어집니다.
>* 각 Yandex 광고 그룹에는 최대 200개의 키워드가 포함될 수 있습니다.

**[!UICONTROL Status]:** 키워드의 표시 상태: *활성* 또는 *일시 중지됨*. 새 키워드의 기본값은 *Active*&#x200B;입니다.

## [!UICONTROL Bids]

<!-- **[!UICONTROL Bid]:** -->

{{$include /help/_includes/bid-keyword.md}}

## 자리 표시자

**[!UICONTROL Param1]** **[!UICONTROL Param2]:** 키워드를 사용하여 광고를 표시할 때 광고 및 사이트 링크의 기본 URL에서 `{param1}` 및 `{param2}` 인스턴스에 대해 대체되는 {param1} 및 {param2} 대체 변수의 값입니다. 최대 길이는 255바이트입니다.

특수 문자는 UTF-8로 자동 인코딩됩니다. 예를 들어 연결된 광고에 기본 URL이 &quot;http://www.example.com/{param1}이고 키워드 수준 값이 {param1}인 경우 광고는 &quot;shoes/flats.html http://www.example.com/shoes%2Fflats.html&quot;으로 이어집니다.

>[!MORELIKETHIS]
>
>* [키워드 관리](/help/search-social-commerce/campaign-management/campaigns/keyword-manage.md)
