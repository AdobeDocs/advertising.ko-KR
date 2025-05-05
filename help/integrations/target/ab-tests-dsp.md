---
title: Adobe Target에서 Adobe Advertising DSP 광고에 대한 A/B 테스트 구성
description: ' [!DNL Target] 에서 DSP 광고를 위해 A/B 테스트를 설정하는 방법에 대해 알아봅니다.'
exl-id: 5092e06b-eef0-43f3-ba81-6dbe7164158c
source-git-commit: a69bef9d249514f5c494cff8d706b9df792eaf23
workflow-type: tm+mt
source-wordcount: '1413'
ht-degree: 0%

---

# Advertising DSP 광고용 Adobe Target에서 A/B 테스트 구성

*Advertising DSP만 있는 광고주*

Adobe Advertising 및 Adobe Target을 사용하면 마케터가 유료 미디어 및 온사이트 메시징 간에 개인화되고 연결된 경험을 보다 쉽게 제공할 수 있습니다. 제품 간 신호를 공유하여 다음과 같은 작업을 수행할 수 있습니다.

* DSP 캠페인의 고객 광고 노출을 사이트 내 경험에 연결하여 사이트 폴스루 비율을 낮춥니다.

* Adobe Audience Manager 노출 데이터 및 클릭투피드 대상 [!DNL Target]명을 사용하여 광고 메시징으로 온사이트 경험을 미러링하여 A/B 테스트를 설정하십시오.

* [!DNL Target]에 대한 Adobe Analytics의 간단한 시각화를 통해 통합 메시징이 온사이트 목표 상승도에 미치는 영향을 측정합니다.

클릭스루 및 뷰스루 추적을 설정하고, DSP과 [!DNL Target] 간의 신호 공유를 구현하고, A/B 테스트 활동을 설정하고, 테스트 데이터를 볼 수 있도록 [!DNL Analytics] Analysis Workspace을 설정하는 지침 및 사전 요구 사항에 대해서는 다음 섹션을 참조하십시오.

추가 질문이 있는 경우 adcloud_support@adobe.com으로 문의하십시오.

## 사전 요구 사항

이 사용 사례에는 다음 제품 및 통합이 필요합니다.

* [!DNL Target]

* [[!DNL Analytics] Advertising용](/help/integrations/analytics/overview.md) 통합<!-- necessary for testing view-throughs, which most advertisers want to do -->

* [[!DNL Analytics] for [!DNL Target]](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4t.html?lang=ko) 통합

* Audience Manager(뷰스루 테스트에만 필요)

## 1단계: 클릭스루 프레임워크 설정 {#click-through-framework}

![클릭스루 프레임워크](/help/integrations/assets/target-ct-framework.png)

클릭스루 URL(사용자가 광고를 클릭하여 랜딩 페이지에 도달할 때 표시되는 URL)에 DSP 매크로를 추가하면 DSP은 클릭스루 URL에 `${TM_PLACEMENT_ID}`을(를) 포함하여 배치 키를 자동으로 캡처합니다. 이 매크로는 숫자 배치 ID가 아닌 영숫자 배치 키를 캡처합니다.

![랜딩 페이지 URL에 추가된 클릭스루 URL](/help/integrations/assets/target-ct-url.jpg)

### (DSP만 해당) 클릭스루 URL에 DSP 매크로 추가

<!-- If we ever write instructions for ads on other ad servers (such as Sizmek ads in DCO), then work that into the following section. -->

[!DNL Flashtalking] 또는 Google Campaign Manager 360 내에서 각 광고의 클릭스루 URL을 수동으로 업데이트하여 AMO ID 변수를 캡처하는 데 필요한 매크로를 포함합니다. AMO ID 변수는 클릭 데이터를 Adobe Analytics으로 전송하고 A/B 테스트를 위한 배치 키를 공유하는 데 사용됩니다. 지침은 다음 페이지를 참조하십시오.

* [추가 [!DNL Analytics for Advertising] 매크로를  [!DNL Flashtalking] 광고 태그](/help/integrations/analytics/macros-flashtalking.md)에 추가합니다. **참고:** 조직에서 [!DNL Flashtalking]과(와) 직접 파트너 관계를 맺고 데이터 전달 매크로를 사용하여 [https://support.flashtalking.com/hc/en-us/articles/4409808166419-Accessing-Data-Pass-Macros](https://support.flashtalking.com/hc/en-us/articles/4409808166419-Accessing-Data-Pass-Macros)에 있는 [!DNL Flashtalking] 지원 설명서별로 `s_kwcid` 및 `ef_id` 추적 매개 변수를 추적하는 경우에는 이 절차가 필요하지 않습니다.

* [ [!DNL Google Campaign Manager 360] 광고 태그에  [!DNL Analytics for Advertising] 매크로 추가](/help/integrations/analytics/macros-google-campaign-manager.md)

Adobe 계정 팀 및 Advertising 솔루션 그룹(aac-advertising-solutions-group@adobe.com)에 문의하여 필요한 배치 키를 검색하고 설정을 완료하고 각 클릭스루 URL에 배치 키가 채워져 있는지 확인합니다.

## 2단계: Audience Manager을 사용하여 뷰스루 프레임워크 설정 {#view-through-framework}

![뷰스루 프레임워크](/help/integrations/assets/targetr-vt-framework.png)

광고 태그 및 배치 설정에서 Audience Manager 노출 이벤트 픽셀을 추가하여 추가 뷰스루 테스트 기회를 위한 테스트 세그먼트를 만들 수 있습니다.

1. 광고 태그 및 DSP 배치 설정에서 Audience Manager 노출 이벤트 픽셀을 구현합니다.

   지침은 &quot;[Advertising DSP 캠페인에서 미디어 노출 데이터 수집](/help/integrations/audience-manager/media-data-integration/collect.md)&quot;을 참조하십시오.

   숫자 배치 ID에 대한 `${TM_PLACEMENT_ID_NUM}`을(를) 포함하여 노출 이벤트 픽셀에서 다시 전달할 모든 데이터를 캡처하려면 [DSP 매크로](/help/dsp/campaign-management/macros.md)를 추가해야 합니다.

   >[!NOTE]
   >
   >클릭 추적 URL에는 숫자 배치 ID의 `${TM_PLACEMENT_ID_NUM}` 대신 영숫자 배치 키의 `${TM_PLACEMENT_ID}` 매크로가 포함됩니다.

1. DSP 노출 데이터에서 Audience Manager 세그먼트를 구성합니다.

   1. 세그먼트 데이터를 사용할 수 있는지 확인합니다.

      1. 세그먼트 사용자를 그룹화할 수준을 결정하는 [키-값 쌍](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/data-explorer/signals-search/data-explorer-search-pairs.html?lang=ko)에 대한 신호를 [검색](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/data-explorer/signals-search/data-explorer-signals-search.html?lang=ko)합니다.

         Audience Manager 노출 이벤트 픽셀에 추가한 매크로에 해당하는 값으로 [지원되는 키](https://experienceleague.adobe.com/docs/audience-manager/user-guide/implementation-integration-guides/media-data-integration/impression-data-pixels.html?lang=ko)을(를) 사용합니다.

         예를 들어 특정 배치에 대해 사용자를 그룹화하려면 `d_placement` 키를 사용하십시오. 값에 대해 DSP 매크로 `${TM_PLACEMENT_ID_NUM}`에서 캡처한 실제 숫자 배치 ID(예: 2501853)를 사용합니다. <!-- Explain where to find the placement ID, other than in a custom report. -->

         검색 결과에 픽셀이 올바르게 배치되었고 데이터가 흐르고 있음을 나타내는 키-값 쌍에 대한 사용자 수가 표시되면 다음 단계를 계속 진행합니다.

   1. Audience Manager에서 세그먼트를 만들 [규칙 기반 특성을 만듭니다](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/traits/trait-builder/create-onboarded-rule-based-traits.html?lang=ko).

      * 테스트 활동 내에서 쉽게 식별할 수 있도록 트레이트 이름을 지정합니다. 원하는 폴더에 트레이트를 저장합니다.

      * `Ad Cloud`을(를) **[!UICONTROL Data Source]**(으)로 선택합니다.

      * 트레이트 식의 경우 `d_event`을(를) **[!UICONTROL Key]**(으)로 사용하고 `imp`을(를) **[!UICONTROL Value]**(으)로 사용합니다.

   1. [Audience Manager에서 새 트레이트에 대한 테스트 세그먼트를 설정](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/segments/segment-builder.html?lang=ko)하고 `Ad Cloud`을(를) **[!UICONTROL Data Source]**(으)로 선택합니다.

      Audience Manager은 세그먼트를 표준 랜딩 페이지 경험을 받는 컨트롤 그룹과 개인화된 온사이트 경험을 받는 테스트 그룹으로 자동으로 분할합니다.

## 3단계: DSP용 [!DNL Target]에서 A/B 테스트 활동 설정

다음 지침은 DSP 사용 사례와 관련된 정보를 강조 표시합니다.

1. [Adobe Target에 로그인](https://experienceleague.adobe.com/docs/target/using/introduction/target-access-from-mac.html?lang=ko).

1. [A/B 테스트 만들기](https://experienceleague.adobe.com/docs/target/using/activities/abtest/create/test-create-ab.html?lang=ko):

   1. **[!UICONTROL Enter Activity URL]** 필드에 테스트용 랜딩 페이지 URL을 입력합니다.

      >[!NOTE]
      >
      >여러 URL을 사용하여 뷰스루 사이트 항목을 테스트할 수 있습니다. 자세한 내용은 &quot;[다중 페이지 활동](https://experienceleague.adobe.com/docs/target/using/experiences/vec/multipage-activity.html?lang=ko)&quot;을 참조하세요. Analytics에서 [사이트 시작 보고서](https://experienceleague.adobe.com/ko/docs/analytics-learn/tutorials/integrations/adobe-advertising-dsp/create-advertising-cloud-site-entry-reports)를 만들어 페이지 URL별로 상위 항목을 쉽게 식별할 수 있습니다.

   1. **[!UICONTROL Goal]** 필드에 테스트에 대한 성공 지표를 입력합니다.

      >[!NOTE]
      >
      >[!DNL Analytics]이(가) [!DNL Target] 내에서 데이터 원본으로 사용되고 올바른 보고서 세트가 선택되었는지 확인하십시오.

   1. 테스트 세그먼트의 사용자가 잘못된 온사이트 경험을 받을 때 충돌을 방지하려면 **[!UICONTROL Priority]**&#x200B;을(를) `High` 또는 `999`(으)로 설정하십시오.

   1. **[!UICONTROL Reporting Settings]** 내에서 DSP 계정에 연결된 **[!UICONTROL Company Name]** 및 **[!UICONTROL Report Suite]**&#x200B;을(를) 선택하십시오.

      추가 보고 팁은 &quot;[보고 모범 사례 및 문제 해결](https://experienceleague.adobe.com/docs/analytics/analyze/reports-analytics/report-troubleshooting.html?lang=ko)&quot;을 참조하십시오.

   1. **[!UICONTROL Date Range]** 필드에 테스트에 대한 적절한 시작 날짜와 종료 날짜를 입력합니다.

   1. 활동에 대상 추가:

      1. 이전에 Audience Manager에서 만든 [세그먼트를 선택하여 뷰스루 대상](#view-through-framework)을 테스트하십시오.

      1. **[!UICONTROL Site Pages]** > **[!UICONTROL Landing Page]** > **[!UICONTROL Query]**&#x200B;을(를) 선택하고 **[!UICONTROL Value]** 필드에 DSP 배치 키를 입력하여 클릭스루 대상에 대해 Target 쿼리 문자열 매개 변수를 사용합니다.

   1. **[!UICONTROL Traffic Allocation Method]**&#x200B;에 대해 **[!UICONTROL Manual (Default)]**&#x200B;을(를) 선택하고 대상을 50/50으로 분할합니다.

   1. 활동을 저장합니다.

1. [Target 시각적 경험 작성기](https://experienceleague.adobe.com/docs/target/using/activities/abtest/create/test-create-ab.html?lang=ko)를 사용하여 A/B 테스트 랜딩 페이지 템플릿에 대한 디자인을 변경합니다.

   * 경험 A: 개인화가 없는 기본/제어 랜딩 페이지 경험이므로 편집하지 마십시오.

   * 경험 B: [!DNL Target] 사용자 인터페이스를 사용하여 테스트에 포함된 자산(예: 헤드라인, 사본, 단추 배치 및 크리에이티브)을 기반으로 랜딩 페이지 템플릿을 사용자 지정합니다.

   >[!NOTE]
   >
   >크리에이티브 테스트 사용 사례의 경우 Adobe 계정 팀에 문의하십시오.

## 4단계: [!DNL Analytics]에서 [!DNL Analytics for Target] Analysis Workspace 설정

<!-- [If separate page, add "Adobe" before first-use of product names.] -->

[!DNL Analytics for Target]&#x200B;(A4T)은(는) 광고주가 [!DNL Analytics] 전환 지표 및 대상 세그먼트를 기반으로 [!DNL Target] 활동을 만든 다음 [!DNL Analytics]을(를) 보고 소스로 사용하여 결과를 측정할 수 있는 솔루션 간 통합입니다. 해당 활동에 대한 모든 보고 및 세분화는 [!DNL Analytics] 데이터 수집을 기반으로 합니다.

구현 지침에 대한 링크를 포함하여 [!DNL Analytics for Target]에 대한 자세한 내용은 &quot;[Adobe Target용 보고 소스로서의 Adobe Analytics(A4T)](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4t.html?lang=ko)&quot;을(를) 참조하십시오.

### [!DNL Analytics for Target] 패널 설정

Analysis Workspace에서 [!DNL Target] 활동 및 경험을 분석하도록 [!DNL Analytics for Target panel]을(를) 구성합니다. 보고서에 대한 다음과 같은 중요한 지침과 정보를 숙지하십시오.

#### 지표

* 테스트가 실행된 Adobe Advertising 캠페인, 패키지 또는 배치와 관련된 작업 영역 내 패널을 만듭니다. 요약 시각화를 사용하여 [!DNL Target] 테스트 성능과 동일한 보고서에 Adobe Advertising 지표를 표시합니다.

* 성과를 측정하기 위해 온사이트 지표(예: 방문 및 전환)를 사용하는 우선 순위를 지정합니다.

* Adobe Advertising의 집계된 미디어 지표(예: 노출 횟수, 클릭 수 및 비용)를 [!DNL Target] 지표와 일치시킬 수 없음을 이해합니다.

#### 치수

다음 차원은 [!DNL Analytics for Target]과(와) 관련이 있습니다.

* **[!UICONTROL Target Activities]**: A/B 테스트의 이름

* **[!UICONTROL Target Experiences]**: 활동 내에서 사용된 랜딩 페이지 경험의 이름

* **[!UICONTROL Target Activity]** > **[!UICONTROL Experience]**: 같은 행의 활동 이름과 경험 이름

### [!DNL Target] 데이터에 대한 Analytics 문제 해결

Analysis Workspace 내에서 활동 및 경험 데이터가 최소화되거나 채워지지 않는 것을 발견하면 다음을 수행하십시오.

* [!DNL Target]과(와) [!DNL Analytics]에 모두 동일한 [!UICONTROL Supplemental Data ID]&#x200B;(SDID)가 사용되는지 확인하십시오. 캠페인이 사용자를 유도하는 랜딩 페이지에서 [Adobe Experience Cloud Debugger](https://experienceleague.adobe.com/docs/target-learn/tutorials/troubleshooting/troubleshoot-with-the-experience-cloud-debugger.html?lang=ko)를 사용하여 SDID 값을 확인할 수 있습니다.

[Adobe Debugger의 SDID(Supplemental Data ID) 값](/help/integrations/assets/target-troubleshooting-sdid.png)

* 같은 랜딩 페이지에서 a) [!UICONTROL Solutions] > [!UICONTROL Target] 아래의 Adobe Debugger에 표시된 [!UICONTROL Hostname]이(가) b) 활동에 대한 [!DNL Target] ([!UICONTROL Goals & Settings] > [!UICONTROL Reporting Settings] 아래)에 표시된 [!UICONTROL Tracking Server]과(와) 일치하는지 확인하십시오.

  [!DNL Analytics For Target]을(를) 사용하려면 [!DNL Target]에서 Analytics용 [!DNL Modstats] 데이터 수집 서버로 호출하는 동안 [!DNL Analytics] 추적 서버를 보내야 합니다.<!-- just "to Analytics?"-->

[Adobe Debugger의 호스트 이름 값](/help/integrations/assets/target-troubleshooting-hostname.png)

[Target의 추적 서버 값](/help/integrations/assets/target-troubleshooting-tracking-server.png)

## 추가 읽기

* [Analytics와 Target 통합](https://experienceleague.adobe.com/docs/target-learn/tutorials/integrations/3.2-target-analytics.html?lang=ko) - Analysis Workspace에서 [!DNL Target] 보고를 설정하는 방법에 대해 설명합니다.
* [A/B 테스트 개요](https://experienceleague.adobe.com/docs/target/using/activities/abtest/test-ab.html?lang=ko) - DSP 광고에 사용할 수 있는 A/B 테스트 활동에 대해 설명합니다.
* [경험 및 오퍼](https://experienceleague.adobe.com/docs/target/using/experiences/experiences.html?lang=ko) - DSP 테스트 사용자가 노출되는 사이트 콘텐츠를 결정하는 [!DNL Target] 도구에 대해 설명합니다.
* [신호, 트레이트 및 세그먼트](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reference/signal-trait-segment.html?lang=ko) - DSP 뷰스루 테스트에 도움이 되는 일부 Audience Manager 도구를 정의합니다.
* [Advertising용 Analytics 개요](/help/integrations/analytics/overview.md) - Analytics 인스턴스에서 클릭스루 및 뷰스루 사이트 상호 작용을 추적할 수 있는 Advertising용 Analytics를 소개합니다.

>[!MORELIKETHIS]
>
>* [Adobe Target에서 Advertising 검색, 소셜 및 Commerce 광고에 대한 A/B 테스트 구성](ab-tests-search.md)
