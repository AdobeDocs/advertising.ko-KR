---
title: 다음에서 사용자 ID 변환 [!DNL Optimizely] 범용 ID로
description: DSP을 활성화하여 다음을 수집하는 방법 알아보기 [!DNL Optimizely] 자사 세그먼트.
feature: DSP Audiences
source-git-commit: 9b784b99051e33330ee7fbc736a9edbdf22066ca
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 0%

---

# 다음에서 사용자 ID 변환 [!DNL Optimizely] 범용 ID로

와 DSP 통합 사용 [!DNL Optimizely] 고객 데이터 플랫폼 : 조직의 자사 해시된 이메일 주소를 타겟팅된 광고를 위한 범용 ID로 변환합니다.

1. (이메일 주소를 (으)로 변환 [!DNL RampIDs]<!-- or [!DNL ID5] IDs -->; 광고주 [[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md)) [활성화하려면 추적 설정 [!DNL Analytics] 측정](#analytics-tracking).

1. [DSP에서 대상 소스 만들기](#source-create).

1. [세그먼트 데이터 준비 및 푸시](#push-data).

1. [범용 ID 수를 해시된 이메일 주소 수와 비교](#compare-id-count).

## 1단계: 추적 설정 [!DNL Analytics] 측정 {#analytics-tracking}

*를 사용하는 광고주 [[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md))*

이메일 주소를 다음으로 변환하려면 [!DNL RampIDs] 또는 [!DNL ID5] ID, 다음을 수행해야 합니다.

1. (아직 완료하지 않은 경우) 모두 완료 [구현을 위한 사전 요구 사항 [!DNL Analytics for Advertising]](/help/integrations/analytics/prerequisites.md) 및 다음을 확인합니다. [AMO ID 및 EF ID](/help/integrations/analytics/ids.md) 가 추적 URL에서 채워집니다.

1. 범용 ID 파트너에 등록하고 웹 페이지에 범용 ID 관련 코드를 배포하여 데스크탑 및 모바일 웹 브라우저(모바일 앱은 아님)의 ID에서 뷰스루로의 전환을 일치시킵니다.

   * **대상 [!DNL RampIDs]:** 뷰스루를 위해 데스크탑 및 모바일 웹 브라우저(모바일 앱은 아님)의 ID에서 변환된 내용을 일치시키려면 웹 페이지에 추가 JavaScript 태그를 배포해야 합니다. Adobe 계정 팀에 문의하여 다음에 대한 등록 지침을 제공합니다. [!DNL LiveRamp] [!DNL LaunchPad] 태그 위치: [!DNL LiveRamp] 인증 트래픽 솔루션. 등록은 무료이지만 계약서에 서명하셔야 합니다 등록하면 Adobe 계정 팀이 웹 페이지에서 구현할 조직의 고유 태그를 생성하고 제공합니다.

## 2단계: DSP에서 대상 소스 만들기 {#source-create}

1. [대상자 소스 만들기](source-manage.md) DSP 계정 또는 광고주 계정으로 대상자를 가져오려면 다음을 수행하십시오. 사용자 식별자를 다음 중 하나로 변환하도록 선택할 수 있습니다 [사용 가능한 범용 ID 형식](source-about.md).

   소스 설정에는 세그먼트 데이터를 푸시하는 데 사용할 자동 생성 소스 키가 포함됩니다.

1. 대상 소스를 만든 후 소스 코드 키를 [!DNL Optimizely] 사용자.

## 3단계: 세그먼트 데이터 준비 및 푸시 {#push-data}

광고주는 자신의 도움을 받아 데이터를 준비하고 푸시해야 합니다 [!DNL Optimizely] 담당자.

1. 다음 범위 내 [!DNL Optimizely Data Platform]는 SHA-256 알고리즘을 사용하여 광고주의 대상자에 대한 이메일 ID를 해시합니다.

1. 광고주 연락처 [!DNL Optimizely] DSP에 세그먼트 푸시하기 지침 담당자 세그먼트를 푸시할 때 다음 정보를 포함합니다.

   * **소스 키:** 다음에서 생성된 소스 키입니다. [2단계](#source-create).

   * **계정 코드:** 영숫자 DSP 계정 코드이며 DSP 내에서 찾을 수 있습니다. [!UICONTROL Settings] > [!UICONTROL Account].

세그먼트는 24시간 이내에 DSP에서 사용할 수 있어야 하며 광고주에 대해 구성된 대로 새로 고쳐집니다. 세그먼트의 새로 고침 빈도에 관계없이 세그먼트에 포함된 항목은 30일 후에 만료되어 개인 정보 준수를 보장하므로 다음에서 대상을 다시 푸시하여 새로 고칩니다. [!DNL Optimizely] 30일 이내입니다.

<!--
Are they using the Data Platform web services, another type of API, or a UI? Add a link to instructions, including how to designate DSP as the destination. And where will they input the DSP-specific fields?]
-->

## 4단계: 범용 ID 수를 해시된 이메일 주소 수와 비교 {#compare-id-count}

모든 단계를 완료하고에서 대상을 만들거나 편집할 때 사용할 수 있는 대상 라이브러리에서 확인합니다 [!UICONTROL Audiences] > [!UICONTROL All Audiences] 또는 배치 설정 내에서) 세그먼트를 사용할 수 있으며 24시간 이내에 채울 수 있습니다. 범용 ID 수를 해시된 원본 이메일 주소 수와 비교합니다.

범용 ID에 대한 해시된 이메일 주소의 번역률은 90%보다 커야 합니다. 예를 들어 고객 데이터 플랫폼에서 100개의 해시된 이메일 주소를 전송하는 경우 90개 이상의 범용 ID로 변환되어야 합니다. 90% 이하의 번역률이 문제입니다. 세그먼트 카운트가 달라질 수 있는 방법에 대한 자세한 내용은 &quot;[이메일 ID와 범용 ID 간의 데이터 분산 원인](#universal-ids-data-variances).&quot;

문제 해결 지원은 Adobe 계정 팀에 문의하거나 `adcloud-support@adobe.com`.

>[!MORELIKETHIS]
>
>* [자사 대상 소스 정보](/help/dsp/audiences/sources/source-about.md)
>* [범용 ID 대상을 활성화하기 위한 대상 소스 관리](source-manage.md)
>* [범용 ID 활성화 지원](/help/dsp/audiences/universal-ids.md)
>* [대상자 관리 기본 정보](/help/dsp/audiences/audience-about.md)