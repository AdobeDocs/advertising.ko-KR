---
title: Adobe Advertising Creative 정보
description: ' [!DNL Creative]에 대해 알아봅니다.'
feature: Creative Introduction
exl-id: 2cc12119-5924-4fcd-a54b-30f7887ae6a7
source-git-commit: de2a2a097802cc4a7b5ac63bee2eb326895e70f1
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# Adobe Advertising Creative 2.0 정보

<!-- verify all and rewrite to include new stuff -->

Adobe Advertising의 일부인 Advertising Creative은 개인화된 실시간 광고 경험을 자동화하고 선택적으로 광고 요소 수준에서 광고를 최적화하는 셀프서비스 플랫폼입니다.<!-- Verify --> Adobe Advertising DSP을 비롯한 모든 DSP에서 광고 경험을 광고로 구현할 수 있습니다.

## 재사용 가능한 크리에이티브 사용자 정의 크리에이티브 라이브러리

Creative 라이브러리를 사용하면 광고 경험에서 사용할 크리에이티브를 관리할 수 있습니다. 개별 크리에이티브 및 크리에이티브 그룹이 포함된 여러 라이브러리를 만들 수 있습니다(*번들*(경험에 첨부됨).

### [!DNL Adobe] 자산 통합

[!DNL Creative]은(는) Adobe Experience Manager과 직접 통합되어 있으므로 디자인 팀이 표준 이미지 광고에 대해 만들고 승인하는 [!DNL Adobe] 이미지 에셋을 쉽게 업로드할 수 있습니다.

## 규칙 기반 및 타깃팅되지 않은 경험 모두

* **타깃팅된 규칙 기반 경험:** 규칙 기반 의사 결정 트리 모델을 사용하여 스토리를 빌드합니다. 대상에 대해 알고 있는 내용에 따라 실시간으로 사용자 지정된 광고 안무 문자열을 펼칩니다. 예를 들어 스토리는 고객 행동, 지역, 인구 통계, 재타겟팅, 고객 여정 내 위치 등에 따라 변경될 수 있습니다.

* **타깃팅되지 않은 경험:** 대상을 좁히지 않고 광고 요소를 예약하고 최적화합니다.

### [!DNL Adobe] 데이터 통합

Adobe Audience Manager 및 Adobe Analytics의 자사 대상 세그먼트뿐만 아니라 Advertising DSP에서 만드는 사용자 지정 대상 세그먼트와 [!DNL Creative]을(를) 사용하여 만드는 픽셀을 광고 경험의 특정 크리에이티브를 위한 타겟으로 사용할 수 있습니다. <!-- Advertiser should be able to target all segments that are available in DSP for targeting -->

### 경험을 광고로 구현

경험을 만든 후에는 경험에 대한 JavaScript 또는 iframe 태그를 생성하고 Advertising DSP 캠페인 또는 다른 DSP에서 타사 광고로 태그를 구현할 수 있습니다.

### 광고 요소 최적화

[!DNL Creative]에서 제공하는 최적화된 가중치 광고 순환을 사용하여 선택적으로 [!DNL Adobe AI]에서 특정 대상 대상을 정의하는지 여부에 관계없이 성능에 따라 모든 경험에 대한 광고 요소를 최적화하도록 허용할 수 있습니다.

<!--
[!DNL Creative] serves first-party ads and triggers third-party ads for the experience based on the specified targeting (when applicable), scheduling, ad rotation, and optimization goal options 
-->

## 픽셀 재타겟팅

광고 경험 내에서 크리에이티브의 타겟으로 사용할 리타기팅 픽셀을 만들 수 있습니다. 타겟은 이전에 특정 웹 페이지를 방문한 지정된 특성을 가진 사용자에게만 광고를 표시합니다.

## 노출, 클릭 및 전환 추적

[!DNL Creative]은(는) 경험에서 제공된 광고에 대한 모든 노출 횟수 및 클릭 수를 자동으로 추적합니다. 또한 선택적으로 Creative 라이브러리의 크리에이티브에 서드파티 노출 추적 및 클릭 추적 URL과 경험의 사용자 지정 추적 URL을 추가할 수도 있습니다.

[!DNL Creative]은(는) 광고 경험에서 만들어진 제공된 광고의 전환도 추적합니다.<!-- Verify wording; anything important to add here? We do track them for all users, right? Or is it optional?  -->

<!--
 [Don't need to mention] When an ad is served, the DSP that buys the ad first tracks the impression, and then passes the impression information to [!DNL Creative]. [!DNL Creative] first tracks a click on an ad, and it then passes the click information
to the DSP.
-->

## 성능 보고

Creative > Experiences에서 경험 수준의 상세한 성과 보고서를 볼 수 있습니다.

보고서 > 사용자 지정 보고서에서 사용자 지정 Creative 보고서를 만들어 경험 전반의 경험 수준 성능을 모니터링할 수도 있습니다. [!DNL Creative] 경험을 DSP 캠페인 내에서 광고로 사용하는 경우 해당 광고의 성능 데이터는 다른 DSP 광고의 데이터와 마찬가지로 추가 사용자 지정 보고서에서 사용할 수 있습니다. <!-- Verify that [!DNL Creative] users have access to ALL other reports. -->

선택적으로 사용자 지정 보고서를 지정된 [보고서 대상](/help/dsp/reports/report-destinations/report-destination-about.md)에 전달할 수 있습니다.

<!--
>* [Overview of implementing Adobe Advertising Creative](/help/creative/introduction/implementation-overview.md)
>* [How the user interface is organized](/help/creative/introduction/ui.md)
-->

>[!MORELIKETHIS]
>
>* [크리에이티브 라이브러리 정보](/help/creative/creative-libraries/creative-libraries-about.md)
>* [Advertising Creative의 경험 정보](/help/creative/experiences/experience-about.md)
