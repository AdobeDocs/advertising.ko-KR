---
title: '[!DNL Google Ads] 통화 전용 광고 설정'
description: ' [!DNL Google Ads] 통화 전용 광고에 대한 설정을 참조합니다.'
exl-id: 10672771-53fd-4ce9-9d67-6b1f8f5a41b8
feature: Search Campaign Management
source-git-commit: e16bc62127a708de8f4deb1eddfa53a14405cbc2
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 0%

---

# [!DNL Google Ads] 통화 전용 광고 설정

검색 네트워크를 사용하는 캠페인에 대한 호출 전용 텍스트 광고를 만들 수 있습니다.

Search, Social 및 Commerce은 계정 수준 랜딩 페이지 접미사와 추적 템플릿을 사용하여 호출 전용 광고를 추적하지만, 선택적으로 [!DNL Google Ads] Manager 내의 광고 수준에서 계정 수준 추적을 무시할 수 있습니다.

[계정당 광고 제한](https://support.google.com/google-ads/answer/6372658?hl=en)에 대한 [!DNL Google Ads] 도움말을 참조하십시오.

<!-- ## Call-only Ad -->

<!-- hiding section header since there's only one section -->

**[!UICONTROL Business Name]:** 비즈니스 이름입니다. 최대 길이는 25자 또는 12개의 더블바이트 문자입니다.

**[!UICONTROL Country]:**(선택 사항) 비즈니스가 있는 국가입니다.

**[!UICONTROL Phone Number]:** 회사 전화번호. 예: (124) 123-4567, 12345678901, +441234567890.

**[!UICONTROL Description 1], [!UICONTROL Description 2]:** 광고 본문의 첫 번째 줄과 두 번째 줄입니다. 각 행의 최대 길이는 35자 또는 17개의 더블바이트 문자입니다.

키워드 대체 구문은 최대 길이에 포함되지 않습니다. 예를 들어 &quot;`{Description1: Free Account Analysis!}`&quot;은(는) 22자로 처리됩니다(&quot;무료 계정 분석\!&quot; 부분만).

>[!NOTE]
>
>설명 필드에는 전화 번호가 포함될 수 없습니다.

**[!UICONTROL Display URL]:** 광고에 표시되는 URL입니다. 표시 URL은 귀사의 비즈니스와 연결된 도메인과 일치해야 하지만 광고는 사람들을 랜딩 페이지로 보내지 않습니다.

최대 길이는 싱글바이트 35자 또는 더블바이트 17자입니다. 키워드 대체 구문은 최대 길이에 포함되지 않습니다. 예를들어, &quot;`{DisplayURL: example.com}`&quot;은(는) 11자로 처리됩니다(&quot;example.com&quot; 부분만).

**[!UICONTROL Verification URL]:**(선택 사항) [!DNL Google Ads]에서 전화 번호가 유효한지 확인할 수 있도록 광고의 전화 번호가 텍스트로 표시되는 웹 페이지입니다. 광고 표시 URL과 동일한 도메인이 있어야 합니다.

**[!UICONTROL Is Tracked]:** 호출 추적 및 호출 전용 전환을 사용합니다.

**[!UICONTROL Count calls as phone call conversions]:**(&quot;[!UICONTROL Is Tracked]&quot;을(를) 선택한 경우, 선택 사항) 하나를 지정한 경우 광고에서 특정 유형의 전화 통화 전환으로 인해 발생하는 모든 호출의 특성을 지정합니다. 그렇지 않으면 [!DNL Google Ads]이(가) 전달 번호에서 하나 이상의 변환을 기록한 다음 특성 호출을 기록하면 기본 변환 작업 &quot;[!UICONTROL Calls from ads]&quot;을(를) 만듭니다.

**[!UICONTROL Count Action]:**(&quot;[!UICONTROL Count calls as phone call conversions]&quot;을(를) 선택한 경우; 선택 사항) 호출이 속하는 기존 전환 작업입니다.

[!DNL Google Ads] 내에서 전환 작업을 만들고 관리할 수 있습니다.

<!-- **[!UICONTROL Status]:** -->

{{$include /help/_includes/status-ad.md}}

>[!MORELIKETHIS]
>
>* [광고 정보](ad-about.md)
>* [광고 관리](ad-manage.md)
>* [[!DNL Google Ads] 확장된 동적 검색 광고 설정](ad-settings-google-dsa.md)
>* [[!DNL Google Ads] 반응형 검색 광고 설정](ad-settings-google-rsa.md)
