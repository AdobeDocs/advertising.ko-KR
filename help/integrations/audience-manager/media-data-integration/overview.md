---
title: Adobe Audience Manager에 DSP Media 노출 데이터 전송 개요
description: Audience Manager 이벤트 픽셀을 사용하여 Advertising DSP 캠페인에서 노출 수준 및 클릭 수준 데이터를 캡처하는 방법을 알아봅니다
feature: Integration with Adobe Audience Manager
exl-id: c299cdf0-a83e-4026-8b8b-22ce08af0cc4
source-git-commit: aec57b49e636d63fc6967af8764ed62f239f31bb
workflow-type: tm+mt
source-wordcount: '524'
ht-degree: 0%

---

# Adobe Audience Manager에 DSP Media 노출 데이터 전송 개요

*Advertising DSP만 있는 광고주*

*Adobe Advertising-Adobe Audience Manager 통합만 있는 광고주*

Adobe Audience Manager을 사용하는 Advertising DSP 고객은 Audience Manager 이벤트 픽셀을 사용하여 DSP 캠페인에서 노출 수준 데이터 및 클릭 수준 데이터를 캡처할 수 있습니다. 이벤트 픽셀은 데이터를 Audience Manager에 실행 가능한 신호로 보냅니다. 이러한 신호를 통해 고급 세분화, 빈도 관리, 마케팅 분석 및 보고 통찰력과 같은 다양한 DSP 사용 사례를 사용할 수 있습니다.

DSP에서는 이러한 신호를 Audience Manager으로 전송하도록 요구하지 않습니다. 그러나 Audience Manager 계약에 따라 서버 호출을 기준으로 표준 Audience Manager 수집 비용을 지불합니다. Audience Manager은 두 가지 서로 다른 방식으로 추적되는 중복 이벤트를 제거하여 각 이벤트가 한 번만 부과되도록 합니다.

>[!NOTE]
>
> Audience Manager은 광고 서버 로그 파일에서 데이터 캡처를 지원하므로 유연성이 떨어집니다. 이 프로세스는 이 설명서에서 다루지 않습니다.

## 주요 이점

* DSP campaign 데이터는 실시간으로 Audience Manager으로 유입되며, 이 데이터를 사용하여 세그먼트를 정의하는 데 사용하는 규칙 기반 트레이트를 구축할 수 있습니다.

* 세그먼트는 사용자 트레이트 및 세그먼트 선별 후 즉시 타깃팅에 사용할 수 있으므로 실시간 타깃팅 노력을 강화합니다.

* 크리에이티브 간 빈도 제한, 이전 캠페인에 노출된 사용자 재타겟팅, 다운스트림 사이트 행동 및 진입점 분석과 같은 사용 사례에 캠페인 데이터를 활용할 수 있습니다.

* 집계된 데이터는 캠페인 성능에 대한 통합 보기를 제공하고 사용자 지정 전환 경로를 식별하는 데 도움이 되며, Audience Manager을 통해 전환되는 이벤트의 시퀀스를 개선하는 데 사용할 수 있습니다 [!DNL Audience Optimization Reports] 또는 [[!DNL Audience Analytics] Adobe Analytics과 통합](/help/integrations/audience-manager/audience-analytics.md).

## 데이터 추적 방법

Audience Manager 노출 및 클릭 이벤트 픽셀은 쿠키를 기반으로 합니다. 픽셀은 모바일 앱과 같이 쿠키가 없는 환경에서 발생하는 이벤트를 캡처하지 않습니다.<!-- Verify if this is still correct. -->

### 노출 추적 픽셀

1xl-pixel 투명 이벤트 추적 픽셀을 광고에 첨부할 때 Audience Manager이 광고에 대한 노출 데이터를 추적합니다. 이벤트 픽셀은 광고가 사용자에게 제공될 때마다 로드되고 웹 브라우저에 의해 로드됩니다. 픽셀은 클라이언트별 의 하위 도메인에서 로드됩니다. [`demdex.net`](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reference/demdex-calls.html): Audience Manager의 레거시 도메인이며 키-값 쌍으로 매개변수를 포함합니다. 이벤트 호출은 노출 및 전환 데이터를 수집하여 Audience Manager 데이터 수집 서버로 전송합니다.

### 클릭 추적 픽셀

Audience Manager은 광고가 제공될 때마다 투명한 이벤트 픽셀을 로드하지 않는다는 점을 제외하고 노출과 유사하게 클릭을 추적합니다. 대신 클릭 데이터가 광고의 클릭스루 URL에서 추적됩니다. 광고는 의 클라이언트별 하위 도메인을 가리킵니다. [`demdex.net`](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reference/demdex-calls.html): Audience Manager 데이터 수집 서버에서 처리할 Audience Manager의 기존 도메인입니다. 그런 다음 서버는 사용자를 의도한 랜딩 페이지로 리디렉션합니다. URL에는 매개 변수가 키-값 쌍으로 포함되어 있습니다.

>[!NOTE]
>
>조직에서 를 사용하는 경우 [!DNL Analytics] 추적하면 Audience Manager 클릭 추적이 필요하지 않을 수 있습니다. Adobe Analytics은 클릭 신호를 캡처하여 다음을 통해 Audience Manager으로 보낼 수 있습니다. [서버측 전달](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/server-side-forwarding/ssf.html).

>[!MORELIKETHIS]
>
>* [Advertising DSP 캠페인에서 클릭 및 노출 데이터 수집](collect.md)
>* [사용 사례](use-cases.md)
