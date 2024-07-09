---
title: "다음에서 사용자 ID 변환: [!DNL ActionIQ] 범용 ID로"
description: "DSP에서 다음을 수집할 수 있도록 하는 방법 알아보기 [!DNL ActionIQ] 자사 세그먼트."
feature: DSP Audiences
source-git-commit: 91b08bf54f067666c9c27949ff740639738887d0
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# 다음에서 사용자 ID 변환 [!DNL ActionIQ] 범용 ID로

*Beta 기능*

와 DSP 통합 사용 [!DNL ActionIQ] 타깃팅된 광고를 위해 해시된 이메일 주소를 범용 ID로 변환하는 고객 데이터 플랫폼입니다.

다음 항목이 있습니다. <!-- NN --> 데이터 공유 단계 [!DNL ActionIQ] DSP 사용:

1. [DSP에서 대상 소스 만들기](#source-create).

1. ?

## 1단계: DSP에서 대상 소스 만들기 {#source-create}

1. [대상자 소스 만들기](source-manage.md) DSP 계정 또는 광고주 계정으로 대상자를 가져오려면 [범용 ID 형식](source-about.md) 사용자 식별자를 변환할 대상.

1. 대상 소스를 만든 후 소스 코드 키를 [!DNL ActionIQ] 사용자.

## 2단계:

## 3단계:

1. 대상 라이브러리에서 확인합니다(에서 대상을 만들거나 편집할 때 사용 가능). [!UICONTROL Audiences] > [!UICONTROL All Audiences] 또는 배치 설정 내에서) 세그먼트가 채워지고 있고 범용 ID 수를 원래 해시된 이메일 주소 수와 비교합니다.

   세그먼트는 24시간 이내에 DSP에서 사용할 수 있어야 합니다. DSP이 세그먼트 데이터를 받은 후 대상자 카운트는 9시간 이내에 표시됩니다. 허용되는 ID 번역률과 세그먼트 수가 달라질 수 있는 이유에 대한 자세한 내용은 &quot;[이메일 ID와 범용 ID 간의 데이터 분산](#universal-ids-data-variances).&quot;

세그먼트는 24시간마다 새로 고쳐집니다.

## 문제 해결

번역 속도 및 사용자 수 문제를 해결하려면 다음을 참조하십시오.[범용 ID 활성화 지원](/help/dsp/audiences/universal-ids.md).&quot;

전환 절차와 관련된 문제를 해결하려면 Adobe 계정 팀에 문의하거나 `adcloud-support@adobe.com`.

>[!MORELIKETHIS]
>
>* [자사 대상 소스 정보](/help/dsp/audiences/sources/source-about.md)
>* [범용 ID 대상을 활성화하기 위한 대상 소스 관리](source-manage.md)
>* [다음에서 사용자 ID 변환 [!DNL Adobe Real-Time CDP] 범용 ID로](/help/dsp/audiences/sources/source-adobe-rtcdp.md)
>* [다음에서 사용자 ID 변환 [!DNL Tealium] 범용 ID로](/help/dsp/audiences/sources/source-tealium.md)
>* [대상자 관리 기본 정보](/help/dsp/audiences/audience-about.md)
