---
title: Adobe Advertising Creative 정보
description: ' [!DNL Creative]에 대해 알아봅니다.'
feature: Creative Introduction
source-git-commit: 8d88a46e82a17ce5d2debf93ea0652f35a734d7a
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# Adobe Advertising Creative 2.0 정보

*베타가 닫힘*

<!-- verify all and rewrite to include new stuff -->

Adobe Advertising의 일부인 Advertising Creative은 개인화된 실시간 광고 경험을 자동화하고 선택적으로 광고 요소 수준에서 광고를 최적화하는 셀프서비스 플랫폼입니다.

## 재사용 가능한 크리에이티브 사용자 정의 크리에이티브 라이브러리

Creative 라이브러리를 사용하면 광고 경험에서 사용할 크리에이티브를 관리할 수 있습니다. 개별 크리에이티브 및 크리에이티브 그룹이 포함된 라이브러리를 여러 개 만들 수 있습니다(*번들*). 광고 경험에 크리에이티브 번들을 추가합니다.

## 규칙 기반 경험

[!DNL Creative]을(를) 사용하면 규칙 기반 의사 결정 트리 모델을 사용하여 스토리를 작성할 수 있습니다. 즉, 대상자에 대해 알고 있는 내용에 따라 실시간으로 맞춤화되고 고객이 다른 웹 사이트로 이동할 때에도 고객을 따라 이동하는 안무된 광고 문자열을 펼칠 수 있습니다<!-- verify if that's true without Adobe CDP -->. 예를 들어 스토리는 고객 행동, 지역, 인구 통계, 재타겟팅, 고객 여정 내 위치 등에 따라 변경될 수 있습니다.

### 경험을 광고로 구현

경험을 만든 후에는 경험에 대한 JavaScript 또는 iframe 태그를 생성하고 Advertising DSP 또는 다른 DSP에서 타사 광고로 태그를 구현할 수 있습니다.<!-- Add any more info about integration with DSP? -->

<!-- Maybe add a subsection "Audience targeting options" with info about types of creative-level REtargeting and placement-level targeting within your DSP.  Need to clarify if any placement-level targeting might contradict/override creative-level targeting, or if they're completely different.

Advertiser should be able to target all segments which are available in DSP for targeting
-->

### 광고 요소 최적화

선택적으로 [!DNL Creative]이(가) Adobe Sensei에서 제공하는 최적화된 가중 광고 회전을 사용하여 특정 대상 타겟을 정의하는지 여부에 관계없이 성능에 따라 모든 경험에 대한 광고 요소를 최적화하도록 허용할 수 있습니다.

## 픽셀 재타겟팅

광고 경험 내에서 크리에이티브의 타겟으로 사용할 리타기팅 픽셀을 만들 수 있습니다. 타겟은 이전에 특정 웹 페이지를 방문한 지정된 특성을 가진 사용자에게만 광고를 표시합니다.

## 노출, 클릭 및 전환 추적

[!DNL Creative]은(는) 경험에서 제공된 광고에 대한 모든 노출 횟수 및 클릭 수를 자동으로 추적합니다. 또한 선택적으로 Creative 라이브러리의 크리에이티브에 서드파티 노출 추적 및 클릭 추적 URL과 경험의 사용자 지정 추적 URL을 추가할 수도 있습니다.

[!DNL Creative]은(는) 광고 경험에서 만들어진 제공된 광고의 전환도 추적합니다.<!-- Verify wording; anything important to add here? We do track them for all users, right? Or is it optoinal?  -->

<!--
 [Don't need to mention] When an ad is served, the DSP that buys the ad first tracks the impression, and then passes the impression information to [!DNL Creative]. [!DNL Creative] first tracks a click on an ad, and it then passes the click information
to the DSP.
-->

## 성능 보고

Creative > Experiences에서 경험 수준의 상세한 성과 보고서를 볼 수 있습니다.

보고서 > 사용자 지정 보고서에서 사용자 지정 Creative 보고서를 만들어 경험 전반의 경험 수준 성능을 모니터링할 수도 있습니다. [!DNL Creative] 경험을 DSP 캠페인 내에서 광고로 사용하는 경우 해당 광고의 성능 데이터는 다른 DSP 광고의 데이터와 마찬가지로 추가 사용자 지정 보고서에서 사용할 수 있습니다. <!-- Verify that [!DNL Creative] users have access to ALL other reports, and if I can completely duplicate the report help for both help sets. -->

선택적으로 사용자 지정 보고서를 지정된 [보고서 대상](/help/dsp/reports/report-destinations/report-destination-about.md)에 전달할 수 있습니다.

<!--
>* [Overview of implementing Adobe Advertising Creative](/help/creative/introduction/implementation-overview.md)
>* [How the user interface is organized](/help/creative/introduction/ui.md)
-->

>[!MORELIKETHIS]
>
>* [크리에이티브 라이브러리 정보](/help/creative/creative-libraries/creative-libraries-about.md)
>* [Advertising Creative의 경험 정보](/help/creative/experiences/experience-about.md)
