---
title: Adobe Target에서 Adobe Advertising 광고에 대한 A/B 테스트 구성
description: 에서 A/B 테스트를 설정하는 방법 알아보기 [!DNL Target] DSP 광고용.
exl-id: 5092e06b-eef0-43f3-ba81-6dbe7164158c
source-git-commit: 48f755b6f3ac00a69086fe4c7ce69d320946635b
workflow-type: tm+mt
source-wordcount: '1427'
ht-degree: 0%

---

# Advertising DSP Ads용 Adobe Target에서 A/B 테스트 구성

<!-- In title and Heading1:  DSP and [!DNL Advertising Search, Social, & Commerce] Ads -->

<!-- Add [!UICONTROL and [!DNL tags throughout as needed. -->

<!-- Break into sub-files, or just leave as one? -->

*Advertising DSP만 있는 광고주*

Adobe Advertising과 Adobe Target을 사용하면 마케터가 유료 미디어와 온사이트 메시징 간에 개인화되고 연결된 경험을 보다 쉽게 제공할 수 있습니다. 제품 간 신호를 공유하여 다음과 같은 작업을 수행할 수 있습니다.

* DSP 캠페인의 고객 광고 노출을 현장 경험과 연결하여 사이트 폴스루 비율을 낮춥니다.

* Adobe Audience Manager 노출 데이터 및 클릭투피드 Target 대상을 사용하여 광고 메시지로 온사이트 경험을 미러링하여 A/B 테스트를 설정합니다.

* Adobe Analytics 의 간단한 시각화를 통해 통합 메시징이 온사이트 목표 상승도에 미치는 영향을 측정합니다. [!DNL Target].

사전 요구 사항과 클릭스루 및 뷰스루 추적을 설정하는 지침은 DSP 및 간의 신호 공유를 구현하여 다음 섹션을 참조하십시오. [!DNL Target] A/B 테스트 활동 설정 및 설정 [!DNL Analytics] Analysis Workspace을 사용하여 테스트 데이터를 볼 수 있습니다.

추가 질문이 있는 경우 adcloud_support@adobe.com으로 문의하십시오.

## 전제 조건

이 사용 사례에는 다음 제품 및 통합이 필요합니다.

* [!DNL Target]

* [[!DNL Analytics] 광고용](/help/integrations/analytics/overview.md) 통합<!-- necessary for testing view-throughs, which most advertisers want to do -->

* [[!DNL Analytics] 대상 [!DNL Target]](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4t.html) 통합

* Audience Manager(뷰스루 테스트에만 필요)

## 1단계: 클릭스루 프레임워크 설정 {#click-through-framework}

<!-- [If separate page, add "Adobe" before first-use of product names.] -->

![클릭스루 프레임워크](/help/integrations/assets/target-ct-framework.png)

클릭스루 URL(사용자가 광고를 클릭하여 랜딩 페이지에 도달할 때 표시되는 URL)에 DSP 매크로를 추가하면 DSP은 다음을 포함하여 배치 키를 자동으로 캡처합니다 `${TM_PLACEMENT_ID}` 를 클릭합니다. 이 매크로는 숫자 배치 ID가 아닌 영숫자 배치 키를 캡처합니다.

![랜딩 페이지 URL에 추가된 클릭스루 URL](/help/integrations/assets/target-ct-url.jpg)

### (DSP 전용) 클릭스루 URL에 DSP 매크로 추가

<!-- If we ever write instructions for ads on other ad servers (such as Sizmek ads in DCO), then work that into the following section. -->

Flash 대화 또는 Google Campaign Manager 360 내에서 AMO ID 변수를 캡처하는 데 필요한 매크로를 포함하도록 각 광고의 클릭스루 URL을 수동으로 업데이트합니다. AMO ID 변수는 클릭 데이터를 Adobe Analytics으로 전송하고 A/B 테스트를 위한 배치 키를 공유하는 데 사용됩니다. 지침은 다음 페이지를 참조하십시오.

* [추가 [!DNL Analytics for Advertising] 매크로 위치 [!DNL Flashtalking] 광고 태그](/help/integrations/analytics/macros-flashtalking.md)

* [추가 [!DNL Analytics for Advertising] 매크로 위치 [!DNL Google Campaign Manager 360] 광고 태그](/help/integrations/analytics/macros-google-campaign-manager.md)

Adobe 계정 팀 및 Advertising Solutions 그룹(aac-advertising-solutions-group@adobe.com)에 문의하여 필요한 배치 키를 검색하고 설정을 완료하고 각 클릭스루 URL에 배치 키가 채워져 있는지 확인합니다.

## 2단계: Audience Manager을 사용하여 뷰스루 프레임워크 설정 {#view-through-framework}

<!-- [If separate page, add "Adobe" before first-use of product names.] -->

![뷰스루 프레임워크](/help/integrations/assets/targetr-vt-framework.png)

Audience Manager 태그 및 배치 설정에서 광고 노출 이벤트 픽셀을 추가하여 추가 뷰스루 테스트 기회를 위한 테스트 세그먼트를 만들 수 있습니다.

1. 광고 태그 및 DSP 배치 설정에서 Audience Manager 노출 이벤트 픽셀을 구현합니다.

   자세한 내용은 &quot;[Advertising DSP 캠페인에서 미디어 노출 데이터 수집](/help/integrations/audience-manager/media-data-integration/collect.md).&quot;

   다음을 추가했는지 확인 [DSP 매크로](/help/dsp/campaign-management/macros.md) 다음을 포함하여 노출 이벤트 픽셀이 다시 전달하려는 모든 데이터를 캡처합니다. `${TM_PLACEMENT_ID_NUM}` 숫자 배치 ID용.

   >[!NOTE]
   >
   >클릭 추적 URL에는 `${TM_PLACEMENT_ID}` 영숫자 배치 키 대신 매크로 `${TM_PLACEMENT_ID_NUM}` 숫자 배치 ID용.

1. DSP 노출 데이터에서 Audience Manager 세그먼트를 구성합니다.

   1. 세그먼트 데이터를 사용할 수 있는지 확인합니다.

      1. [신호 검색](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/data-explorer/signals-search/data-explorer-signals-search.html) 대상: [키-값 쌍](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/data-explorer/signals-search/data-explorer-search-pairs.html) 세그먼트 사용자를 그룹화하는 수준을 결정합니다.

         사용 [지원되는 키](https://experienceleague.adobe.com/docs/audience-manager/user-guide/implementation-integration-guides/media-data-integration/impression-data-pixels.html) Audience Manager 노출 이벤트 픽셀에 추가한 매크로에 해당하는 값을 사용합니다.

         예를 들어 특정 배치에 대한 사용자를 그룹화하려면 `d_placement` 키. 값의 경우 DSP 매크로에서 캡처한 실제 숫자 배치 ID(예: 2501853)를 사용합니다 `${TM_PLACEMENT_ID_NUM}`. <!-- Explain where to find the placement ID, other than in a custom report. -->

         검색 결과에 픽셀이 올바르게 배치되었고 데이터가 흐르고 있음을 나타내는 키-값 쌍에 대한 사용자 수가 표시되면 다음 단계를 계속 진행합니다.

   1. [규칙 기반 트레이트 만들기](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/traits/trait-builder/create-onboarded-rule-based-traits.html) Audience Manager에서 세그먼트를 만들 때 사용합니다.

      * 테스트 활동 내에서 쉽게 식별할 수 있도록 트레이트 이름을 지정합니다. 원하는 폴더에 트레이트를 저장합니다.

      * 선택 `Ad Cloud` (으)로 **데이터 소스**.

      * 트레이트 표현식의 경우 다음을 사용하십시오 `d_event` (으)로 **키** 및 `imp` (으)로 **값**.

   1. [테스트 세그먼트 설정](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/segments/segment-builder.html) Audience Manager의 새 트레이트에 대해 `Ad Cloud` (으)로 **데이터 소스**.

      Audience Manager은 세그먼트를 표준 랜딩 페이지 경험을 받는 컨트롤 그룹과 개인화된 온사이트 경험을 받는 테스트 그룹으로 자동으로 분할합니다.

## 3단계: Target에서 &quot;A/B 테스트&quot; 활동 설정

<!-- [If separate page, add "Adobe" before first-use of product names.] -->

다음 지침은 DSP 사용 사례와 관련된 정보를 강조 표시합니다. 자세한 내용은 &quot;&quot;을(를) 참조하십시오.

1. [Adobe Target에 로그인](https://experienceleague.adobe.com/docs/target/using/introduction/target-access-from-mac.html).

1. [A/B 테스트 만들기](https://experienceleague.adobe.com/docs/target/using/activities/abtest/create/test-create-ab.html):

   1. 다음에서 **활동 URL 입력** 필드에 테스트용 랜딩 페이지 URL을 입력합니다.

      >[!NOTE]
      >
      >여러 URL을 사용하여 뷰스루 사이트 항목을 테스트할 수 있습니다. 자세한 내용은 &quot;[다중 페이지 활동](https://experienceleague.adobe.com/docs/target/using/experiences/vec/multipage-activity.html).&quot; 를 만들어 페이지 URL별로 상위 항목을 쉽게 식별할 수 있습니다. [사이트 시작 보고서](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/integrations/ad-cloud/create-advertising-cloud-site-entry-reports.html) Analytics에서.

   1. 다음에서 **목표** 필드에 테스트에 대한 성공 지표를 입력합니다.

      >[!NOTE]
      >
      >다음을 확인합니다. [!DNL Analytics] 내에서 데이터 소스로 활성화됨 [!DNL Target]을 클릭하여 올바른 보고서 세트를 선택합니다.

   1. 설정 **우선 순위** 끝 `High` 또는 `999` 테스트 세그먼트의 사용자가 잘못된 온사이트 경험을 받을 때 충돌을 방지하기 위해 입니다.

   1. 다음 범위 내 **보고 설정**&#x200B;를 선택하고 **회사 이름** 및 **보고서 세트** DSP 계정에 연결되었습니다.

      추가 보고 팁은 &quot;[보고 우수 사례 및 문제 해결](https://experienceleague.adobe.com/docs/analytics/analyze/reports-analytics/report-troubleshooting.html).&quot;

   1. 다음에서 **날짜 범위** 필드에 테스트에 대한 적절한 시작 날짜와 종료 날짜를 입력합니다.

   1. 활동에 대상 추가:

      1. 다음을 선택합니다. [뷰스루 대상을 테스트하기 위해 Audience Manager에서 이전에 만든 세그먼트](#view-through-framework).

      1. 선택 **사이트 페이지** > **랜딩 페이지** > **쿼리**&#x200B;을 누르고 다음에 DSP 배치 키를 입력합니다. **값** 클릭스루 대상에 대한 Target 쿼리 문자열 매개 변수를 사용할 필드입니다.

   1. 의 경우 **트래픽 할당 방법**, 선택 **수동(기본값)** 대상자를 50/50으로 나눕니다.

   1. 활동을 저장합니다.

1. 사용 [!DNL Target] [시각적 경험 작성기](https://experienceleague.adobe.com/docs/target/using/activities/abtest/create/test-create-ab.html) A/B 테스트 랜딩 페이지 템플릿에 대한 디자인을 변경합니다.

   * 경험 A: 개인화가 없는 기본/제어 랜딩 페이지 경험이므로 편집하지 마십시오.

   * 경험 B: [!DNL Target] 테스트에 포함된 에셋(예: 헤드라인, 복사, 버튼 배치 및 크리에이티브)을 기반으로 랜딩 페이지 템플릿을 사용자 정의하는 사용자 인터페이스.

   >[!NOTE]
   >
   >크리에이티브 테스트 사용 사례의 경우 Adobe 계정 팀에 문의하십시오.

## 4단계: 설정 [!DNL Analytics for Target] Analysis Workspace in [!DNL Analytics]

<!-- [If separate page, add "Adobe" before first-use of product names.] -->

[!DNL Analytics for Target] (A4T)는 광고주가 만들 수 있는 교차 솔루션 통합입니다 [!DNL Target] 활동 기준 [!DNL Analytics] 전환 지표 및 대상 세그먼트를 클릭한 다음 를 사용하여 결과를 측정합니다. [!DNL Analytics] 를 보고 소스로 사용합니다. 해당 활동에 대한 모든 보고 및 세분화는 [!DNL Analytics] 데이터 수집입니다.

에 대한 자세한 내용 [!DNL Analytics for Target], 구현 지침에 대한 링크를 포함하면 &quot;[Adobe Target용 보고 소스로서의 Adobe Analytics (A4T)](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4t.html)&quot;.

### 다음을 설정합니다. [!DNL Analytics for Target] 패널

Analysis Workspace에서 다음을 구성합니다 [!DNL Analytics for Target panel] 을(를) 분석하려면 [!DNL Target] 활동 및 경험. 보고서에 대한 다음과 같은 중요한 지침과 정보를 숙지하십시오.

#### 지표

* 테스트가 실행된 Adobe Advertising 캠페인, 패키지 또는 배치와 관련된 작업 영역 내 패널을 만듭니다. 요약 시각화를 사용하여 Target 테스트 성능과 동일한 보고서에 Adobe Advertising 지표를 표시합니다.

* 성과를 측정하기 위해 온사이트 지표(예: 방문 및 전환)를 사용하는 우선 순위를 지정합니다.

* Adobe Advertising의 집계된 미디어 지표(예: 노출 횟수, 클릭 수 및 비용)는 Target 지표와 일치할 수 없다는 것을 이해합니다.

#### Dimension

다음 차원은 다음과 같습니다 [!DNL Analytics for Target]:

* **Target 활동**: A/B 테스트 이름

* **Target 경험**: 활동 내에 사용된 랜딩 페이지 경험의 이름

* **Target 활동** > **경험**: 동일한 행의 활동 이름 및 경험 이름

### Analytics 문제 해결 [!DNL Target] 데이터

Analysis Workspace 내에서 활동 및 경험 데이터가 최소화되거나 채워지지 않는 것을 발견하면 다음을 수행하십시오.

* Target과 Analytics 모두에 동일한 SDID(Supplemental Data ID)가 사용되는지 확인하십시오. 다음을 사용하여 SDID 값을 확인할 수 있습니다. [Adobe Experience Cloud 디버거](https://experienceleague.adobe.com/docs/target-learn/tutorials/troubleshooting/troubleshoot-with-the-experience-cloud-debugger.html) 사용자를 유도하는 캠페인의 랜딩 페이지에서.

[Adobe Debugger의 SDID(Supplemental Data ID) 값](/help/integrations/assets/target-troubleshooting-sdid.png)

* 동일한 랜딩 페이지에서 a) 솔루션 > Target 아래의 Adobe Debugger에 표시된 호스트 이름이에 표시된 추적 서버와 일치하는지 확인합니다. [!DNL Target] ( 목표 및 설정 > 보고 설정에서) 활동.

  [!DNL Analytics For Target] 을(를) 필요로 합니다. [!DNL Analytics] 호출 시 보낼 추적 서버 [!DNL Target] (으)로 [!DNL Modstats] analytics용 데이터 수집 서버.<!-- just "to Analytics?"-->

[Adobe Debugger의 호스트 이름 값](/help/integrations/assets/target-troubleshooting-hostname.png)

[Target의 추적 서버 값](/help/integrations/assets/target-troubleshooting-tracking-server.png)

## 추가 읽기

* [Analytics와 Target 통합](https://experienceleague.adobe.com/docs/target-learn/tutorials/integrations/3.2-target-analytics.html)- Analysis Workspace에서 Target 보고를 설정하는 방법을 설명합니다.
* [A/B 테스트 개요](https://experienceleague.adobe.com/docs/target/using/activities/abtest/test-ab.html) - DSP 광고와 함께 사용할 수 있는 A/B 테스트 활동에 대해 설명합니다.
* [경험 및 오퍼](https://experienceleague.adobe.com/docs/target/using/experiences/experiences.html) - 설명 [!DNL Target] DSP 테스트 사용자가 노출되는 온사이트 콘텐츠를 판별하는 도구입니다.
* [신호, 트레이트 및 세그먼트](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reference/signal-trait-segment.html) - DSP 뷰스루 테스트에 도움이 되는 일부 Audience Manager 도구를 정의합니다.
* [Analytics for Advertising 개요](/help/integrations/analytics/overview.md) - Analytics 인스턴스에서 클릭스루 및 뷰스루 사이트 상호 작용을 추적할 수 있는 Analytics for Advertising을 소개합니다.

<!-- 
>[!MORELIKETHIS]
>
>* 
-->
