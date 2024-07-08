---
title: 사용자 ID를 [!DNL Optimizely] 유니버설 ID로 변환
description: DSP 에서 자사 세그먼트를 수집하는 [!DNL Optimizely] 방법을 알아봅니다.
feature: DSP Audiences
exl-id: 2c48a874-132a-4e5c-ba24-0e7ab80ac2d4
source-git-commit: 2c42e8e4b7ca7e0cfaaf7895f067e4ccf7a2a40e
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 0%

---

# 사용자 ID를 [!DNL Optimizely] 유니버설 ID로 변환

*Beta 기능*

고객 데이터 플랫폼과 [!DNL Optimizely] DSP 통합을 사용하여 조직의 자사 해시 이메일 주소를 타겟팅 광고를 위한 범용 ID로 전환할 수 있습니다.

1. (이메일 주소를 전환하려면[!DNL RampIDs]<!-- or [!DNL ID5] IDs -->; )[를 사용하는 [[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md)광고주 측정](#analytics-tracking)을 활성화 [!DNL Analytics] 하려면 추적을 설정합니다.

1. [DSP](#source-create)에서 대상자 소스를 만들기.

1. [세그먼트 데이터를](#push-data) 준비하고 푸시합니다.

1. [범용 ID 수와 해시된 이메일 주소](#compare-id-count) 수를 비교합니다.

## 1단계: 측정을 위한 [!DNL Analytics] 추적 설정 {#analytics-tracking}

*)가 있는 [[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md)광고주*

이메일 주소를 또는 [!DNL ID5] ID로 [!DNL RampIDs] 전환하려면 다음을 수행해야 합니다.

1. (아직 수행하지 않은 경우) 구현 [!DNL Analytics for Advertising]](/help/integrations/analytics/prerequisites.md)을 위한 모든 [필수 구성 요소를 모든 앱하고 AMO ID 및 EF ID](/help/integrations/analytics/ids.md)가 추적 URL에 채워지고 있는지 확인합니다[.

1. 유니버설 ID 파트너에 등록하고 웹페이지에 유니버설 ID 관련 코드를 배포하여 데스크탑 및 모바일 웹브라우저(모바일 앱 제외)의 ID에서 조회연결 ID로의 전환을 일치시킵니다.

   * **의 경우 [!DNL RampIDs]:** 데스크탑 및 모바일 웹브라우저(모바일 앱 제외)의 ID에서 조회스루로 전환되는 결과를 일치시키려면 웹페이지에 추가 JavaScript 태그 배포해야 합니다. Authentication Traffic Solutions의 태그 [!DNL LiveRamp] 등록 [!DNL LiveRamp] [!DNL LaunchPad] 지침을 제공하는 Adobe Systems 계정 팀에 문의하십시오. 등록은 무료 이지만 계약서에 서명해야 합니다. 등록하면 Adobe Systems 계정 팀이 조직이 웹 페이지에서 구현할 수 있는 고유한 태그를 생성하고 제공합니다.

## 2단계: DSP에서 대상자 소스 만들기 {#source-create}

1. [대상자 소스를](source-manage.md) 만들기하여 대상을 DSP 계정 또는 광고주 계정로 가져옵니다. 사용자 식별자 [를 사용 가능한 범용 ID 형식으로 전환 할 수 있습니다](source-about.md).

   소스 설정에는 세그먼트 데이터를 푸시하는 데 사용할 자동 생성된 소스 키가 포함됩니다.

1. 대상자 소스를 만든 후 소스 코드 키를 사용자와 [!DNL Optimizely] 공유합니다.

## 3단계: 세그먼트 데이터 준비 및 푸시 {#push-data}

광고주 담당자의 도움을 [!DNL Optimizely] 받아 데이터를 준비하고 푸시해야 합니다.

1. 내에서 [!DNL Optimizely Data Platform]SHA-256 알고리즘을 사용하여 광고주 대상자의 이메일 ID를 해시.

1. 지침에 따라 [[!DNL Optimizely's] 세그먼트를 DSP](https://support.optimizely.com/hc/en-us/articles/27974930963981-Integrate-Adobe-Ads)로 푸시합니다. 통합을 활성화하려면 다음 정보를 포함하십시오.

   * **소스 키:** 2](#source-create)단계에서 만든 [소스 키입니다.

   * **계정 Code:** 영숫자 DSP 계정 Code로, >[!UICONTROL Account]에서 DSP [!UICONTROL Settings] 내에서 찾을 수 있습니다.

세그먼트는 24시간 이내에 DSP에서 사용할 수 있어야 하며 광고주에 대해 구성된 대로 새로 고쳐집니다. 세그먼트를 새로 고치는 빈도에 관계없이 세그먼트에 대한 포함은 기본적으로 30일 후 또는 고객이 지정한 만료 기간 후에 만료됩니다. 세그먼트를 만료 전에 다시 푸시 [!DNL Optimizely] 하여 새로 고침. 사용자 지정 세그먼트 만료를 요청하려면 Adobe Systems 계정 팀에 문의하십시오.

## 4단계: 유니버설 ID 수와 해시된 이메일 주소 수 비교 {#compare-id-count}

모든 단계를 완료한 후 대상 라이브러리(> [!UICONTROL All Audiences] 또는 배치 설정 내에서 대상자 [!UICONTROL Audiences] 만들거나 편집할 때 사용 가능)에서 세그먼트 사용할 수 있고 24시간 이내에 채워지는지 확인합니다. 범용 ID의 개수와 원래 해시된 이메일 주소의 개수를 비교합니다.

해시된 이메일 주소를 범용 ID로 변환하는 비율은 90% 이상이어야 합니다. 예를 들어 고객 데이터 플랫폼에서 100개의 해시된 이메일 주소를 보내는 경우 90개 이상의 범용 ID로 변환되어야 합니다. 변환율이 90% 이하이면 문제가 됩니다. 세그먼트 수가 달라질 수 있는 방법에 대한 자세한 내용은 &quot;[전자 메일 ID와 유니버설 ID](#universal-ids-data-variances) 간의 데이터 차이 원인&quot;을 참조하십시오.

문제 해결 지원이 필요한 경우 Adobe Systems 계정 팀 또는 `adcloud-support@adobe.com`에 문의하십시오.

>[!MORELIKETHIS]
>
>* [자사 대상 소스 정보](/help/dsp/audiences/sources/source-about.md)
>* [대상 소스를 관리하여 유니버설 ID Audiences 활성화](source-manage.md)
>* [범용 ID 활성화 지원](/help/dsp/audiences/universal-ids.md)
>* [고객 관리 정보](/help/dsp/audiences/audience-about.md)
