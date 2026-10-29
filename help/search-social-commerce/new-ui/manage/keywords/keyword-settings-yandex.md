---
title: '[!DNL Yandex] 키워드 설정'
description: '[!DNL Yandex] 키워드에 대한 설정을 참조합니다.'
feature: Search Campaign Management
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: 76ac9ff6-5d89-5acb-bc0b-875761bb3320
    internal-label: Search Campaign Management
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
    internal-label: Optimization
source-git-commit: 3bb565d689b65ae66d6ea2094abccdff3c9e891d
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%
---
# [!DNL Yandex] 키워드 설정

[!DNL Yandex] 키워드는 검색 및 표시(콘텐츠) 네트워크 모두에 사용됩니다.

## [!UICONTROL Basic Settings]

*새 키워드만*

**[!UICONTROL Network]:** 광고 네트워크입니다.

**[!UICONTROL Account]:** 광고 네트워크 계정입니다.

**[!UICONTROL Campaign]:** 캠페인입니다.

**[!UICONTROL Ad Group]:** 광고 그룹입니다.

## [!UICONTROL Keyword Details]

**[!UICONTROL Keywords]:** 키워드에 대한 [[!DNL Yandex] 일치 유형 구문](https://yandex.com/support/direct/keywords/symbols-and-operators.html)을 포함하는 키워드 구문입니다. 각 키워드는 정지어를 제외하고 최대 7개의 단어를 사용할 수 있습니다.

최대 2000개의 키워드를 입력하거나 붙여넣을 수 있습니다. 여러 키워드를 쉼표로 구분하거나 별도의 줄에 입력합니다.

>[!NOTE]
>
>* [!DNL Yandex] 키워드 또는 일치 유형을 변경하면 기존 키워드가 삭제되고 새 키워드가 만들어집니다.
>* 각 [!DNL Yandex] 광고 그룹에는 최대 200개의 키워드를 포함할 수 있습니다.

**[!UICONTROL Status]:** 키워드의 표시 상태: *[!UICONTROL Active]* 또는 *[!UICONTROL Paused]*. 새 키워드의 기본값은 *[!UICONTROL Active]*&#x200B;입니다.

## [!UICONTROL Bids]

{{$include /help/_includes/bid-keyword.md}}

## [!UICONTROL Placeholders]

>[!NOTE]
>
>특수 문자는 UTF-8로 자동 인코딩됩니다. 예를 들어 연결된 광고의 기본 URL이 `http://www.example.com/{param1}`이고 키워드 수준 값이 `{param1}`인 경우 광고는 `http://www.example.com/shoes%2Fflats.html`(으)로 이어집니다.`shoes/flats.html`

**[!UICONTROL Param1]:** 광고를 표시하는 데 키워드를 사용할 때 기본 URL에 광고 및 사이트 링크에 대한 `{param1}` 동적 대체 문자열이 포함된 경우 대체 값으로 사용할 문자열입니다. 최대 길이는 255바이트입니다.

**[!UICONTROL Param2]:** 광고를 표시하는 데 키워드를 사용할 때 기본 URL에 광고 및 사이트 링크에 대한 `{param2}` 동적 대체 문자열이 포함된 경우 대체 값으로 사용할 문자열입니다. 최대 길이는 255바이트입니다.

>[!MORELIKETHIS]
>
>* [키워드 관리](keyword-manage.md)
