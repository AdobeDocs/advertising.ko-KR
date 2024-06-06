---
title: 와 DSP 통합 사용 [!DNL Adobe] [!DNL Real-time CDP]
description: DSP을 활성화하여 다음을 수집하는 방법 알아보기 [!DNL Adobe] [!DNL Real-time CDP] 자사 세그먼트.
feature: DSP Audiences
exl-id: cb1da95b-0d19-4450-8770-6c383248ddae
source-git-commit: 0a1555875fd18b326297475bc19fcfd6f28ea0c5
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# 다음에서 사용자 ID 변환 [!DNL Adobe Real-Time CDP] 범용 ID로

*Beta 기능*

과 DSP 통합 사용 [다음 [!DNL Adobe Real-Time Customer Data Platform (CDP)]](https://experienceleague.adobe.com/docs/experience-platform/rtcdp/overview.html): Adobe Experience Platform의 일부로, 해시된 이메일 주소를 타겟팅된 광고를 위한 범용 ID로 변환합니다.

1. (이메일 주소를 (으)로 변환 [!DNL RampIDs]<!-- or [!DNL ID5] IDs -->; 광고주 [[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md)) 추적 설정 [!DNL Analytics] 측정:

   1. (아직 완료하지 않은 경우) 모두 완료 [구현을 위한 사전 요구 사항 [!DNL Analytics for Advertising]](/help/integrations/analytics/prerequisites.md) 및 [추적 URL의 AMO ID 및 EF ID](/help/integrations/analytics/ids.md).

   1. 범용 ID 파트너에 등록하고 웹 페이지에 범용 ID 관련 코드를 배포하여 데스크탑 및 모바일 웹 브라우저(모바일 앱은 아님)의 ID에서 뷰스루로의 전환을 일치시킵니다.

      * **대상 [!DNL RampIDs]:** 뷰스루를 위해 데스크탑 및 모바일 웹 브라우저(모바일 앱은 아님)의 ID에서 변환된 내용을 일치시키려면 웹 페이지에 추가 JavaScript 태그를 배포해야 합니다. Adobe 계정 팀에 문의하여 다음에 대한 등록 지침을 제공합니다. [!DNL LiveRamp] [!DNL LaunchPad] 태그 위치: [!DNL LiveRamp] 인증 트래픽 솔루션. 등록은 무료이지만 계약서에 서명하셔야 합니다 등록하면 Adobe 계정 팀이 웹 페이지에서 구현할 조직의 고유 태그를 생성하고 제공합니다.

1. [대상자 소스 만들기](source-manage.md) DSP 계정 또는 광고주 계정으로 대상자를 가져오려면 다음을 수행하십시오. 사용자 식별자를 다음 중 하나로 변환하도록 선택할 수 있습니다 [사용 가능한 범용 ID 형식](source-about.md).

   소스 설정에는 다음 단계에서 사용할 자동 생성 소스 키가 포함됩니다.

1. Adobe Experience Platform에서 다음을 사용하여 Advertising DSP 대상 연결을 구성합니다. [!UICONTROL Source Key] DSP 소스 설정에서 생성되었습니다.

   DSP 대상 연결을 활성화하고, 세그먼트를 선택하고, 제어 권한에 액세스하는 방법에 대한 지침은 &quot;[Adobe Advertising Cloud DSP 연결](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/advertising/adobe-advertising-cloud-connection.html).&quot;

   소스 이메일 주소는 SHA-256 알고리즘을 사용하여 해시해야 합니다.

1. 모든 단계를 완료하고에서 대상을 만들거나 편집할 때 사용할 수 있는 대상 라이브러리에서 확인합니다 [!UICONTROL Audiences] > [!UICONTROL All Audiences] 또는 배치 설정 내에서) 세그먼트가 24시간 내에 채워집니다. 범용 ID 수를 해시된 원본 이메일 주소 수와 비교합니다.

   범용 ID에 대한 해시된 이메일 주소의 번역률은 90%보다 커야 합니다. 예를 들어 고객 데이터 플랫폼에서 100개의 해시된 이메일 주소를 전송하는 경우 90개 이상의 범용 ID로 변환되어야 합니다. 90% 이하의 번역률이 문제입니다. 세그먼트 카운트가 달라질 수 있는 방법에 대한 자세한 내용은 &quot;[이메일 ID와 범용 ID 간의 데이터 분산 원인](#universal-ids-data-variances).&quot;

   문제 해결 지원은 Adobe 계정 팀에 문의하거나 `adcloud-support@adobe.com`.

세그먼트는 24시간마다 새로 고쳐집니다. 그러나 개인 정보 보호를 위해 세그먼트에 포함하면 30일 후에 만료되므로 30일 이내에서 Real-Time CDP에서 다시 푸시하여 대상자를 새로 고치십시오.

>[!MORELIKETHIS]
>
>* [범용 ID 대상을 활성화하기 위한 대상 소스 관리](source-manage.md)
>* [Adobe Advertising DSP 연결](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/advertising/adobe-advertising-cloud-connection.html)
>* Adobe Experience Platform [대상 카탈로그 개요](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/overview.html)
>* [에서 인증된 세그먼트 수동으로 가져오기 [!DNL LiveRamp]](/help/dsp/audiences/sources/source-import-liveramp-segments.md)
>* [다음에서 사용자 ID 변환 [!DNL Tealium] 범용 ID로](/help/dsp/audiences/sources/source-tealium.md)
>* [대상자 관리 기본 정보](/help/dsp/audiences/audience-about.md)

<!--
>* [Convert User IDs from [!DNL Optimizely] to Universal IDs](/help/dsp/audiences/sources/source-optimizely.md)
-->
