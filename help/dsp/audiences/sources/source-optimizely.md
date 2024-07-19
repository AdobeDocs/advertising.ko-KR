---
title: 사용자 ID를  [!DNL Optimizely] 에서 범용 ID로 변환
description: DSP에서  [!DNL Optimizely] 자사 세그먼트를 수집할 수 있도록 하는 방법을 알아봅니다.
feature: DSP Audiences
exl-id: 2c48a874-132a-4e5c-ba24-0e7ab80ac2d4
source-git-commit: 91b08bf54f067666c9c27949ff740639738887d0
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# 사용자 ID를 [!DNL Optimizely]에서 유니버설 ID로 변환

*Beta 기능*

[!DNL Optimizely] 고객 데이터 플랫폼과 DSP 통합을 사용하여 조직의 자사 해시된 이메일 주소를 타깃팅된 광고를 위한 범용 ID로 변환합니다.

1. (전자 메일 주소를 [!DNL RampIDs]<!-- or [!DNL ID5] IDs -->; [[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md)을(를) 사용하는 광고주로 변환하려면) [추적을 사용하도록 설정 [!DNL Analytics] 측정](#analytics-tracking)합니다.

1. [DSP에서 대상 소스를 만듭니다](#source-create).

1. [세그먼트 데이터를 준비하고 푸시합니다](#push-data).

1. [범용 ID 수를 해시된 이메일 주소 수와 비교](#compare-id-count).

## 1단계: [!DNL Analytics] 측정에 대한 추적 설정 {#analytics-tracking}

*[[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md)을(를) 사용하는 광고주*

전자 메일 주소를 [!DNL RampIDs] 또는 [!DNL ID5] ID로 변환하려면 다음을 수행해야 합니다.

1. 아직 완료하지 않았다면 [구현을 위한 필수 구성 요소 [!DNL Analytics for Advertising]](/help/integrations/analytics/prerequisites.md)를 모두 완료하고 [AMO ID 및 EF ID](/help/integrations/analytics/ids.md)이(가) 추적 URL에 채워져 있는지 확인하십시오.

1. 범용 ID 파트너에 등록하고 웹 페이지에 범용 ID 관련 코드를 배포하여 데스크탑 및 모바일 웹 브라우저(모바일 앱은 아님)의 ID에서 뷰스루로의 전환을 일치시킵니다.

   * **[!DNL RampIDs]의 경우:** 뷰스루에 대한 데스크톱 및 모바일 웹 브라우저(모바일 앱은 아님)의 ID 전환과 일치하려면 웹 페이지에 추가 JavaScript 태그를 배포해야 합니다. Adobe 계정 팀에 문의하여 [!DNL LiveRamp] 인증 트래픽 솔루션에서 [!DNL LiveRamp] [!DNL LaunchPad] 태그를 등록하는 방법에 대한 지침을 제공받으십시오. 등록은 무료이지만 계약서에 서명하셔야 합니다 등록하면 Adobe 계정 팀이 웹 페이지에서 구현할 조직의 고유 태그를 생성하고 제공합니다.

## 2단계: DSP에서 대상 소스 만들기 {#source-create}

1. 대상을 DSP 계정 또는 광고주 계정으로 가져오려면 [대상 소스를 만듭니다](source-manage.md). 사용자 식별자를 [사용 가능한 범용 ID 형식](source-about.md) 중 하나로 변환하도록 선택할 수 있습니다.

   소스 설정에는 세그먼트 데이터를 푸시하는 데 사용할 자동 생성 소스 키가 포함됩니다.

1. 대상 소스를 만든 후 [!DNL Optimizely] 사용자와 소스 코드 키를 공유합니다.

## 3단계: 세그먼트 데이터 준비 및 푸시 {#push-data}

광고주는 [!DNL Optimizely Data Platform]을(를) 사용하여 데이터를 준비하고 푸시해야 합니다. 프로세스에 대한 질문이 있으면 [!DNL Optimizely] 담당자에게 문의하십시오.

1. [!DNL Optimizely Data Platform] 내에서 SHA-256 알고리즘을 사용하여 대상자에 대한 전자 메일 ID를 해시합니다.

1. [[!DNL Optimizely's] 의 지침에 따라 세그먼트를 DSP에 푸시합니다](https://support.optimizely.com/hc/en-us/articles/27974930963981-Integrate-Adobe-Ads). 통합을 사용하려면 다음 정보를 포함하십시오.

   * **Source 키:** [단계 2](#source-create)에서 만든 소스 키입니다.

   * **계정 코드:** 영숫자 DSP 계정 코드입니다. [!UICONTROL Settings] > [!UICONTROL Account]에서 DSP 내에서 찾을 수 있습니다.

광고주에 대해 구성된 대로 세그먼트가 새로 고쳐집니다. 세그먼트의 새로 고침 빈도에 관계없이 세그먼트에 포함된 항목은 기본적으로 30일 후나 고객이 지정한 만료 기간 후에 만료됩니다. 만료 전에 [!DNL Optimizely]에서 세그먼트를 다시 푸시하여 세그먼트를 새로 고치십시오. 사용자 지정 세그먼트 만료를 요청하려면 Adobe 계정 팀에 문의하십시오.

## 4단계: 범용 ID 수를 해시된 이메일 주소 수와 비교 {#compare-id-count}

세그먼트는 24시간 이내에 DSP에서 사용할 수 있어야 합니다. DSP이 세그먼트 데이터를 받은 후 대상자 카운트는 9시간 이내에 표시됩니다.

대상 라이브러리([!UICONTROL Audiences] > [!UICONTROL All Audiences]에서 대상을 만들거나 편집할 때 또는 배치 설정 내에서 사용 가능)에서 세그먼트가 사용 가능하고 채워지고 있는지 확인하고 범용 ID 수를 원래 해시된 이메일 주소 수와 비교합니다. 허용되는 ID 변환 속도와 세그먼트 수가 달라질 수 있는 이유에 대한 자세한 내용은 &quot;[이메일 ID와 범용 ID 간의 데이터 분산](#universal-ids-data-variances)&quot;을 참조하십시오.

## 문제 해결

번역 속도 및 사용자 수 문제를 해결하려면 &quot;[범용 ID 활성화 지원](/help/dsp/audiences/universal-ids.md)&quot;을 참조하십시오.

전환 프로시저의 문제를 해결하려면 Adobe 계정 팀이나 `adcloud-support@adobe.com`에 문의하십시오.

>[!MORELIKETHIS]
>
>* [자사 대상 소스 정보](/help/dsp/audiences/sources/source-about.md)
>* [범용 ID 대상을 활성화하기 위한 대상 소스 관리](source-manage.md)
>* [범용 ID 활성화 지원](/help/dsp/audiences/universal-ids.md)
>* [대상자 관리 정보](/help/dsp/audiences/audience-about.md)
