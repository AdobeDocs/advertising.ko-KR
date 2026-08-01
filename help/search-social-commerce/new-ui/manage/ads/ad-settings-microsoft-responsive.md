---
title: '[!DNL Microsoft Advertising] 반응형 광고 설정'
description: ' [!DNL Microsoft Advertising] 반응형 광고 설정을 참조합니다.'
feature: Search Campaign Management
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 730b474b83ae4df47c18f93adfec62b1dc9b8a16
workflow-type: tm+mt
source-wordcount: 243
ht-degree: 0%

---

# [!DNL Microsoft Advertising] 반응형(대상) 광고 설정

반응형 광고 형식은 [!DNL Microsoft Audience Network]에서 이미지 기반, 비디오 기반 및 연결된 TV 비디오 기반 대상 광고에 사용할 수 있습니다. 광고 네트워크는 광고 요소의 가장 효과적인 조합을 사용하여 반응형 광고를 동적으로 조합합니다.

## [!UICONTROL Basic Settings]

*새 광고만*

**[!UICONTROL Network]:** 광고 네트워크입니다.

**[!UICONTROL Account]:** 광고 네트워크 계정입니다.

**[!UICONTROL Campaign]:** 캠페인입니다.

**[!UICONTROL Ad Group]:** 광고 그룹입니다.

## [!UICONTROL Audience CTV Video Ad Details]

<!-- I can't find a video ad -- this same header is used for image ads. Need to verify the video ad settings and when you'll get them -->

### 비디오 광고

**[!UICONTROL Videos]:** 비디오 광고 URL.

**[!UICONTROL Status]:** 광고 상태: *[!UICONTROL Active]* 또는 *[!UICONTROL Paused]*.

### 이미지 광고)

>[!NOTE]
>
>광고 네트워크는 매장의 제품 정보 및 광고 그룹 수준의 사용자 타겟팅을 사용하여 가맹점 센터 스토어에 연결된 대상자 캠페인용 광고를 자동으로 생성합니다. 광고를 수동으로 만들 필요가 없습니다.

**[!UICONTROL Images]:** 광고의 JPEG 또는 PNG 이미지를 최대 15개까지 사용할 수 있습니다. 종횡비가 1.91:1인 이미지를 하나 이상 포함하십시오. [대상 광고 이미지](https://help.ads.microsoft.com/#apex/ads/en/56912/0)에 대해 허용되는 종횡비 및 치수를 확인하십시오.

대상 광고의 경우 [!DNL Microsoft Advertising]은(는) 가능한 모든 종횡비에 대해 이 이미지를 자동으로 자릅니다.

<!-- Instructions -->

{{$include /help/_includes/images-ms-multimedia-responsive-ad.md}}

**[!UICONTROL Business Name]:** 비즈니스 이름으로, 최대 25자입니다. 호출 전용 광고 형식으로 사용할 수 있습니다.

**[!UICONTROL Short Headlines]:** 최소 3자, 최대 15자의 짧은 머리글에 한 단어 이상, 최대 30자까지 포함할 수 있습니다.

**[!UICONTROL Long Headlines]:** 최소 3자, 최대 5자의 긴 헤드라인(각각 최대 90자).

**[!UICONTROL Ad Text]:** 최소 두 개, 최대 네 개의 단어 하나와 최대 90자로 구성된 설명.

**[!UICONTROL Status]:** 광고 상태: *[!UICONTROL Active]* 또는 *[!UICONTROL Paused]*.

## [!UICONTROL Tracking URLs]

<!-- **[!UICONTROL Base URl]:** -->

{{$include /help/_includes/base-url-keyword-ad-sitelink.md}}

<!-- **[!UICONTROL Tracking Template]:** -->

{{$include /help/_includes/tracking-template-microsoft.md}}

>[!MORELIKETHIS]
>
>* [광고 관리](/help/search-social-commerce/new-ui/manage/ads/ad-manage.md)
