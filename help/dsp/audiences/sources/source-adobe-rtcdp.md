---
title: ' [!DNL Adobe] [!DNL Real-time CDP]과(와) DSP 통합 사용'
description: DSP에서  [!DNL Adobe] [!DNL Real-time CDP]개의 자사 세그먼트를 수집할 수 있도록 하는 방법을 알아봅니다.
feature: DSP Audiences
exl-id: cb1da95b-0d19-4450-8770-6c383248ddae
source-git-commit: 3a641db6b145e67e6e1f1daca271dd524973e075
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# 사용자 ID를 [!DNL Adobe Real-Time CDP]에서 유니버설 ID로 변환

*Beta 기능*

Adobe Experience Platform의 일부인 [the [!DNL Adobe Real-Time CDP]](https://experienceleague.adobe.com/docs/experience-platform/rtcdp/overview.html)과(와) DSP 통합을 사용하여 해시된 이메일 주소를 타깃팅된 광고를 위한 범용 ID로 변환합니다.

1. (전자 메일 주소를 [!DNL RampIDs]<!-- or [!DNL ID5] IDs -->(으)로 전환하려면, [[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md)을(를) 사용하는 광고주) [!DNL Analytics] 측정에 대한 추적을 설정합니다.

   1. 아직 완료하지 않은 경우) 추적 URL에서 [AMO ID 및 EF ID](/help/integrations/analytics/ids.md)와(과)  [!DNL Analytics for Advertising][&#128279;](/help/integrations/analytics/prerequisites.md)을(를) 구현하기 위한 필수 구성 요소를 모두 완료하십시오.

   1. 범용 ID 파트너에 등록하고 웹 페이지에 범용 ID 관련 코드를 배포하여 데스크탑 및 모바일 웹 브라우저(모바일 앱은 아님)의 ID에서 뷰스루로의 전환을 일치시킵니다.

      * **[!DNL RampIDs]의 경우:** 뷰스루에 대한 데스크톱 및 모바일 웹 브라우저(모바일 앱은 아님)의 ID 전환과 일치하려면 웹 페이지에 추가 JavaScript 태그를 배포해야 합니다. Adobe 계정 팀에 문의하여 [!DNL LiveRamp] 인증 트래픽 솔루션에서 [!DNL LiveRamp] [!DNL LaunchPad] 태그를 등록하는 방법에 대한 지침을 제공받으십시오. 등록은 무료이지만 계약서에 서명하셔야 합니다 등록하면 Adobe 계정 팀이 웹 페이지에서 구현할 조직의 고유 태그를 생성하고 제공합니다.

1. 대상을 DSP 계정 또는 광고주 계정으로 가져오려면 [대상 소스를 만듭니다](source-manage.md). 사용자 식별자를 [사용 가능한 범용 ID 형식](source-about.md) 중 하나로 변환하도록 선택할 수 있습니다.

   소스 설정에는 다음 단계에서 사용할 자동 생성 소스 키가 포함됩니다.

1. Adobe Experience Platform에서 DSP 소스 설정에서 생성된 [!UICONTROL Source Key]을(를) 사용하여 Advertising DSP 대상 연결을 구성합니다.

   DSP 대상 연결을 활성화하고, 세그먼트를 선택하고, 제어 권한에 액세스하는 방법에 대한 지침은 &quot;[Adobe Advertising Cloud DSP 연결](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/advertising/adobe-advertising-cloud-connection.html)&quot;을 참조하십시오.

   소스 이메일 주소는 SHA-256 알고리즘을 사용하여 해시해야 합니다.

1. 대상 라이브러리([!UICONTROL Audiences] > [!UICONTROL All Audiences]에서 대상을 만들거나 편집할 때 또는 배치 설정 내에서 사용 가능)에서 세그먼트가 채워지고 있는지 확인하고 범용 ID 수를 원래 해시된 이메일 주소 수와 비교합니다.

   세그먼트는 24시간 이내에 DSP에서 사용할 수 있어야 합니다. DSP이 세그먼트 데이터를 받은 후 대상자 카운트는 9시간 이내에 표시됩니다. 허용되는 ID 변환 속도와 세그먼트 수가 달라질 수 있는 이유에 대한 자세한 내용은 &quot;[이메일 ID와 범용 ID 간의 데이터 분산](#universal-ids-data-variances)&quot;을 참조하십시오.

세그먼트는 24시간마다 새로 고쳐집니다. 하지만 세그먼트에 포함되면 기본적으로 30일 이후 또는 고객이 지정한 만료 기간 이후에 만료됩니다. 만료 전에 Real-Time CDP에서 세그먼트를 다시 푸시하여 새로 고침합니다. 사용자 지정 세그먼트 만료를 요청하려면 Adobe 계정 팀에 문의하십시오.

## 문제 해결

번역 속도 및 사용자 수 문제를 해결하려면 &quot;[범용 ID 활성화 지원](/help/dsp/audiences/universal-ids.md)&quot;을 참조하십시오.

전환 프로시저의 문제를 해결하려면 Adobe 계정 팀이나 `adcloud-support@adobe.com`에 문의하십시오.

>[!MORELIKETHIS]
>
>* [자사 대상 소스 정보](/help/dsp/audiences/sources/source-about.md)
>* [범용 ID 대상을 활성화하기 위한 대상 소스 관리](source-manage.md)
>* [Adobe Advertising DSP 연결](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/advertising/adobe-advertising-cloud-connection.html)
>* Adobe Experience Platform [대상 카탈로그 개요](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/overview.html)
>* [범용 ID 활성화 지원](/help/dsp/audiences/universal-ids.md)
>* [대상자 관리 정보](/help/dsp/audiences/audience-about.md)
