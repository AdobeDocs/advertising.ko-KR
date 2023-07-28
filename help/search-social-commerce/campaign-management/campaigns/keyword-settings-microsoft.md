---
title: '[!DNL Microsoft Advertising] 키워드 설정'
description: 다음에 대한 설정 참조 [!DNL Microsoft Advertising] 키워드.
exl-id: 248f45c7-8b8c-46fe-a65a-66c50c630044
feature: Search Campaign Management
source-git-commit: 052574217d7ddafb8895c74094da5997b5ff83db
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# [!DNL Microsoft Advertising] 키워드 설정

검색 및 표시 네트워크를 사용하는 캠페인에 대한 키워드를 만들 수 있습니다.

## [!UICONTROL Keyword Details]

**[!UICONTROL Keywords]:** 키워드(모두 포함) [!DNL Microsoft Advertising] 구문 및 자리 표시자를 일치시킵니다. 키워드당 최대 길이는 100자입니다.

최대 2000개의 키워드를 입력하거나 붙여넣을 수 있습니다. 여러 키워드를 쉼표로 구분하거나 별도의 줄에 입력합니다.

>[!NOTE]
>
>* 에서 부정적인 키워드를 만들 수 있습니다. [!UICONTROL Keywords] > [!UICONTROL Negatives] 광고 그룹 및 캠페인 설정에서 및 를 봅니다.
>* 변경 [!DNL Microsoft Advertising] 키워드는 기존 키워드를 삭제하고 새 키워드 ID로 새 키워드를 만듭니다. 그러나 일치 유형을 변경해도 기존 키워드는 삭제되지 않습니다.

**[!UICONTROL Status]:** 키워드의 표시 상태: *활성* 또는 *일시 중지됨*. 새 키워드의 기본값은 입니다 *활성*.

## [!UICONTROL Bids]

<!-- **[!UICONTROL Bid]:** -->

{{$include /help/_includes/bid-keyword.md}}

## 자리 표시자

**[!UICONTROL Param2]:** 키워드의 기본 URL 또는 광고의 제목, 설명 또는 기본 URL에 다음이 포함된 경우 대체 값으로 사용할 문자열 [다음 `{Param2}` 동적 대체 문자열](https://help.bingads.microsoft.com/#apex/3/en/53079/0). 최대 길이는 70자이지만 이 길이를 사용하는 광고 요소의 최대 길이에 유의하십시오(예: 제목 1과 제목 2를 합한 길이는 최대 76자일 수 있음).

**[!UICONTROL Param3]:** 키워드의 기본 URL 또는 광고의 제목, 설명 또는 기본 URL에 다음이 포함된 경우 대체 값으로 사용할 문자열 [다음 `{Param3}` 동적 대체 문자열](https://help.bingads.microsoft.com/#apex/3/en/53079/0). 최대 길이는 70자이지만 이 길이를 사용하는 광고 요소의 최대 길이에 유의하십시오(예: 제목 1과 제목 2를 합한 길이는 최대 76자일 수 있음).

## URL 옵션

<!-- **[!UICONTROL Base URl]:** -->

{{$include /help/_includes/base-url-keyword-ad-sitelink.md}}

이 필드에는 다음 항목이 선택적으로 포함될 수 있습니다. `{Param2}` 및 `{Param3}` 동적 대체 변수입니다.

<!-- **[!UICONTROL Tracking Template]:** -->

{{$include /help/_includes/tracking-template-microsoft.md}}

>[!MORELIKETHIS]
>
>* [키워드 관리](/help/search-social-commerce/campaign-management/campaigns/keyword-manage.md)
