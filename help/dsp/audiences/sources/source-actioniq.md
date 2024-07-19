---
title: "사용자 ID를  [!DNL ActionIQ] 에서 범용 ID로 변환"
description: "DSP에서  [!DNL ActionIQ] 자사 세그먼트를 수집할 수 있도록 하는 방법을 알아봅니다."
feature: DSP Audiences
source-git-commit: 91b08bf54f067666c9c27949ff740639738887d0
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# 사용자 ID를 [!DNL ActionIQ]에서 유니버설 ID로 변환

*Beta 기능*

[!DNL ActionIQ] 고객 데이터 플랫폼과 DSP 통합을 사용하여 해시된 이메일 주소를 타깃팅된 광고를 위한 범용 ID로 변환합니다.

[!DNL ActionIQ]의 데이터를 DSP과 공유하는 단계는 <!-- NN -->개입니다.

1. [DSP에서 대상 소스를 만듭니다](#source-create).

1. ?

## 1단계: DSP에서 대상 소스 만들기 {#source-create}

1. [대상 소스를 만들어](source-manage.md) 대상을 DSP 계정 또는 광고주 계정으로 가져오고, 사용자 식별자를 변환할 [범용 ID 형식](source-about.md)을(를) 지정합니다.

1. 대상 소스를 만든 후 [!DNL ActionIQ] 사용자와 소스 코드 키를 공유합니다.

## 2단계:

## 3단계:

1. 대상 라이브러리([!UICONTROL Audiences] > [!UICONTROL All Audiences]에서 대상을 만들거나 편집할 때 또는 배치 설정 내에서 사용 가능)에서 세그먼트가 채워지고 있는지 확인하고 범용 ID 수를 원래 해시된 이메일 주소 수와 비교합니다.

   세그먼트는 24시간 이내에 DSP에서 사용할 수 있어야 합니다. DSP이 세그먼트 데이터를 받은 후 대상자 카운트는 9시간 이내에 표시됩니다. 허용되는 ID 변환 속도와 세그먼트 수가 달라질 수 있는 이유에 대한 자세한 내용은 &quot;[이메일 ID와 범용 ID 간의 데이터 분산](#universal-ids-data-variances)&quot;을 참조하십시오.

세그먼트는 24시간마다 새로 고쳐집니다.

## 문제 해결

번역 속도 및 사용자 수 문제를 해결하려면 &quot;[범용 ID 활성화 지원](/help/dsp/audiences/universal-ids.md)&quot;을 참조하십시오.

전환 프로시저의 문제를 해결하려면 Adobe 계정 팀이나 `adcloud-support@adobe.com`에 문의하십시오.

>[!MORELIKETHIS]
>
>* [자사 대상 소스 정보](/help/dsp/audiences/sources/source-about.md)
>* [범용 ID 대상을 활성화하기 위한 대상 소스 관리](source-manage.md)
>* [사용자 ID를  [!DNL Adobe Real-Time CDP] 에서 범용 ID로 변환](/help/dsp/audiences/sources/source-adobe-rtcdp.md)
>* [사용자 ID를  [!DNL Tealium] 에서 범용 ID로 변환](/help/dsp/audiences/sources/source-tealium.md)
>* [대상자 관리 정보](/help/dsp/audiences/audience-about.md)
