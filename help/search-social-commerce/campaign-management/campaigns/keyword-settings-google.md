---
title: '[!DNL Google Ads] 키워드 설정'
description: ' [!DNL Google Ads] 키워드에 대한 설정을 참조합니다.'
exl-id: b2937d18-565a-43f0-ba33-d46d4c77ec07
feature: Search Campaign Management
source-git-commit: e16bc62127a708de8f4deb1eddfa53a14405cbc2
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---

# [!DNL Google Ads] 키워드 설정

검색 및 표시 네트워크를 사용하는 캠페인에 대한 키워드를 만들 수 있습니다.

[계정당 키워드 제한](https://support.google.com/google-ads/answer/6372658)에 대해서는 Google 광고 도움말을 참조하십시오.

## [!UICONTROL Keyword Details]

**[!UICONTROL Keywords]:** 키워드 및 자리 표시자에 대한 [!DNL Google Ads] 일치 구문을 포함하는 키워드입니다. [!DNL Google Ads] 계정에는 다음 특성을 가진 키워드가 필요합니다.

* 키워드당 최대 길이는 80자이며 10단어 이하여야 합니다.
* 키워드는 문자, 숫자 및 다음 특수 문자만 포함할 수 있습니다. 공백 `# $ & _ - " [] ' + . / :`

최대 2000개의 키워드를 입력하거나 붙여넣을 수 있습니다. 여러 키워드를 쉼표로 구분하거나 별도의 줄에 입력합니다.

>[!NOTE]
>
>* [!UICONTROL Keywords] > [!UICONTROL Negatives] 보기, 광고 그룹 및 캠페인 설정에서 부정적인 키워드를 만들 수 있습니다.
>* [!DNL Google Ads] 키워드 또는 일치 유형을 변경하면 기존 키워드가 삭제되고 새 키워드가 만들어집니다.

**[!UICONTROL Status]:** 키워드의 표시 상태: *활성* 또는 *일시 중지됨*. 새 키워드의 기본값은 *Active*&#x200B;입니다.

## [!UICONTROL Bids]

<!-- **[!UICONTROL Bid]:** -->

{{$include /help/_includes/bid-keyword.md}}

## 자리 표시자

**[!UICONTROL Param1]:** 기본 URL 또는 추적 템플릿에 [동적 대체 문자열 `{param1}`](https://support.google.com/google-ads/answer/6305348)이(가) 포함된 경우 대체 값으로 사용할 문자열입니다.

**[!UICONTROL Param2]:** 기본 URL 또는 추적 템플릿에 [동적 대체 문자열 `{param2}`](https://support.google.com/google-ads/answer/6305348)이(가) 포함된 경우 대체 값으로 사용할 문자열입니다.

## URL 옵션

<!-- **[!UICONTROL Base URl]:** -->

{{$include /help/_includes/base-url-keyword-ad-sitelink.md}}

<!-- **[note for Base URL field]:** -->

{{$include /help/_includes/base-url-google-note.md}}

<!-- **[!UICONTROL Tracking Template]:** -->

{{$include /help/_includes/tracking-template-google.md}}

>[!MORELIKETHIS]
>
>* [키워드 관리](/help/search-social-commerce/campaign-management/campaigns/keyword-manage.md)
