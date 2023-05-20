---
title: 지속 ID 파트너의 인증된 세그먼트 활성화
description: 지속적인 ID 솔루션을 통해 인증된 대상을 활성화하는 방법에 대해 알아봅니다.
feature: DSP Audiences
exl-id: c56a54c7-5300-4cda-96d0-82d86e76ee39
source-git-commit: 9ca42d078c0d0b6a08d521c8465eca69c2affce5
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# 지속 ID 파트너의 인증된 세그먼트 활성화

*Beta 기능*

Advertising DSP 내의 지속적인 ID 솔루션을 통해 인증된 대상을 활성화하려면 세그먼트를 로 변환해야 합니다 [!DNL RampIDs]: 바인딩할 수 있는 환경에서 인식할 수 있습니다. 다음 중 하나를 통해 이를 수행할 수 있습니다.

* 과의 DSP 통합 활용 [!DNL Adobe Real-Time Customer Data Profile (CDP)] 및 [!DNL Adobe-LiveRamp Retrieval API].

* 에서 수동으로 DSP에 인증된 세그먼트 보내기 [!DNL LiveRamp] [!DNL Connect] 대시보드입니다.

## Tasks

1. 두 옵션 중 하나는 `adcloud-support@adobe.com` DSP에서 다음 설정을 활성화하여 DSP 캠페인에서 인증된 세그먼트를 한 번 타깃팅할 수 있습니다. [활성화 워크플로의 모든 단계가 완료되었습니다.](source-about.md#workflow-sources):

   1. [!DNL LiveRamp] [!DNL RampID] 세그먼트 공유 전 캠페인 구성 [!DNL Real-Time CDP].

   1. 계정 수준 &quot;[!UICONTROL LiveRamp segments]&quot; 옵션.

1. (사용자가에서 인증된 세그먼트를 수동으로 공유) [!DNL LiveRamp])에서 다음 단계를 완료합니다 [!DNL LiveRamp] [!DNL Connect] 대시보드:

   1. 대상 타일 활성화 **[!DNL AAC API 1P Onboarding]**.

   1. 설정 [!DNL Identifier Settings] 끝 **[!DNL Ramp ID]** 만 해당.

      ![식별자 설정](/help/dsp/assets/liveramp-tile-settings.png)

   1. (선택 사항) 쿠키 기반 식별자를 계속 수신하려면 두 번째 식별자를 만듭니다 [!DNL AAC API 1P Onboarding] 대상 타일(&quot;&quot;)[!DNL Cookies],&quot; &quot;[!DNL IDFA],&quot; 및 &quot;[!DNL AAID]&quot;선택됨.

## 테스트 및 데이터 유효성 검사에 대한 우수 사례

* **Target [!DNL RampID]- 세그먼트 및 쿠키 기반 세그먼트를 별도의 캠페인에 포함**

   * Campaign 설정을 사용하면 하나의 식별자만 우선 순위를 지정할 수 있습니다.

   * 현재, [!DNL RampIDs] 온사이트 이벤트 중에는 검색할 수 없습니다. 즉, 가장 낮은 CPA 및 ROAS와 같은 특정 사용자 지정 목표는 인증된 세그먼트를 사용할 때 사용할 수 없습니다. 제한적인 성과 KPI가 있는 경우에만 쿠키 기반 세그먼트를 사용하십시오.

* **두 위치 모두에서 하나의 배치를 만듭니다. [!DNL RampID] 쿠키 기반 캠페인.**

   * 공유 대상 세그먼트 Target [!DNL LiveRamp] 표준 세그먼트 활성화 프로세스 사용.

   * Adobe 광고 지원 팀과 협력하여 적절한 데이터 배포를 확인합니다.

과 DSP 통합에 대해 자세히 알아보려면 [!DNL LiveRamp], 연락처 `adcloud-support@adobe.com`.

>[!MORELIKETHIS]
>
>* [대상 소스에서 인증된 세그먼트 활성화 정보](source-about.md)
>* [자사 대상을 활성화할 대상 소스 만들기](source-create.md)
>* [대상 소스 설정](source-settings.md)
>* [Adobe Advertising DSP 연결](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/advertising/adobe-advertising-cloud-connection.html)
>* [대상자 관리 기본 정보](/help/dsp/audiences/audience-about.md)

