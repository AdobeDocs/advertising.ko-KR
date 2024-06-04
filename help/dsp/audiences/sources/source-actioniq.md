---
title: "다음에서 사용자 ID 변환: [!DNL ActionIQ] 범용 ID로"
description: "DSP에서 다음을 수집할 수 있도록 하는 방법 알아보기 [!DNL ActionIQ] 자사 세그먼트."
feature: DSP Audiences
source-git-commit: bd0586516c2457e4dfcd1a23046707e8bf652e3b
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# 다음에서 사용자 ID 변환 [!DNL ActionIQ] 범용 ID로

*Beta 기능*

와 DSP 통합 사용 [!DNL ActionIQ] 타깃팅된 광고를 위해 해시된 이메일 주소를 범용 ID로 변환하는 고객 데이터 플랫폼입니다.

다음 항목이 있습니다. <!-- NN --> 데이터 공유 단계 [!DNL ActionIQ] DSP 사용:

1. [DSP에서 대상 소스 만들기](#source-create).

1. ?

## 1단계: DSP에서 대상 소스 만들기 {#source-create}

1. [대상자 소스 만들기](source-create.md) DSP 계정 또는 광고주 계정으로 대상자를 가져오려면 [범용 ID 형식](source-about.md) 사용자 식별자를 변환할 대상.

1. 대상 소스를 만든 후 소스 코드 키를 [!DNL ActionIQ] 사용자.

1. 모든 단계를 완료하고에서 대상을 만들거나 편집할 때 사용할 수 있는 대상 라이브러리에서 확인합니다 [!UICONTROL Audiences] > [!UICONTROL All Audiences] 또는 배치 설정 내에서) 세그먼트가 24시간 내에 채워집니다. 범용 ID 수를 해시된 원본 이메일 주소 수와 비교합니다.

   범용 ID에 대한 해시된 이메일 주소의 번역률은 90%보다 커야 합니다. 예를 들어 고객 데이터 플랫폼에서 100개의 해시된 이메일 주소를 전송하는 경우 90개 이상의 범용 ID로 변환되어야 합니다. 90% 이하의 번역률이 문제입니다. 세그먼트 카운트가 달라질 수 있는 방법에 대한 자세한 내용은 &quot;[이메일 ID와 범용 ID 간의 데이터 분산 원인](#universal-ids-data-variances).&quot;

   문제 해결 지원은 Adobe 계정 팀에 문의하거나 `adcloud-support@adobe.com`.

세그먼트는 24시간마다 새로 고쳐집니다.

## 2단계:

>[!MORELIKETHIS]
>
>* [자사 대상 소스 정보](/help/dsp/audiences/sources/source-about.md)
>* [범용 ID 대상을 활성화하는 대상 소스 만들기](source-create.md)
>* [대상 소스 설정](source-settings.md)
>* [다음에서 사용자 ID 변환 [!DNL Adobe Real-Time CDP] 범용 ID로](/help/dsp/audiences/sources/source-adobe-rtcdp.md)
>* [다음에서 사용자 ID 변환 [!DNL Tealium] 범용 ID로](/help/dsp/audiences/sources/source-tealium.md)
>* [대상자 관리 기본 정보](/help/dsp/audiences/audience-about.md)

<!--
>* [Convert User IDs from [!DNL Optimizely] to Universal IDs](/help/dsp/audiences/sources/source-optimizely.md)
-->
