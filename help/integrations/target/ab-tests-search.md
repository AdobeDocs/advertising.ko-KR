---
title: Adobe Target에서 Adobe Advertising 검색, 소셜 및 Commerce 광고에 대한 A/B 테스트 구성
description: 검색, 소셜 및 Commerce에서  [!DNL Target] 및 [!DNL Google Ads] 광고에 대한 [!DNL Microsoft Advertising] 에서 A/B 테스트를 설정하는 방법에 대해 알아봅니다.
exl-id: 564c7d61-beec-40cf-ac68-83d1e87e3008
source-git-commit: 67fe8581832dc0762d62908d01672e53cc95b847
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 0%

---

# Advertising 검색, 소셜 및 Commerce 광고를 위해 Adobe Target에서 A/B 테스트 구성

*Advertising 검색, 소셜 및 Commerce을 사용하는 광고주*

*[!DNL Google Ads]및 [!DNL Microsoft Advertising] 계정만*

Adobe Advertising 및 Adobe Target을 사용하면 디지털 광고 트래픽 [!DNL Google Ads] 및 [!DNL Microsoft Advertising]에 대한 랜딩 페이지 경험 A/B 테스트를 쉽게 설정하여 다음을 수행할 수 있습니다.

* 전환율(CVR) 및 획득 효율성 측정(CPA, CPL 및 CAC 등)을 개선합니다.

* 광고와 관련된 보다 개인화된 랜딩 페이지 경험을 제공합니다(예: 이미지/비디오 크리에이티브, 복사, 키워드 또는 기타 광고 신호를 랜딩 페이지에 일치).

또한 Adobe Analytics에 통합된 기본 [[!DNL Analytics] for Advertising](/help/integrations/analytics/overview.md) 및 [[!DNL Analytics] for [!DNL Target]](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4t.html) 통합 보고 차원을 결합하여 [!DNL Analytics]개의 지표 및 성공 이벤트를 사용하여 테스트 데이터를 측정하고 시각화할 수 있습니다.

필수 구성 요소, 검색, 소셜 및 Commerce의 광고에서 클릭스루 트래픽에 대한 [!DNL Target]의 A/B 테스트 설정 지침 및 [!DNL Analytics]에서 테스트를 측정하고 시각화하는 방법에 대한 팁을 다음 섹션에서 확인하십시오.

## 전제 조건

### 필수 제품

* 검색, 소셜 및 Commerce
* [!DNL Target]

### 권장 제품 및 통합

* [!DNL Analytics]

* [[!DNL Analytics] Advertising용](/help/integrations/analytics/overview.md) 통합<!-- necessary for testing view-throughs, which most advertisers want to do -->

* [[!DNL Analytics] for [!DNL Target]](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4t.html) 통합

## 1단계: [!DNL Target]에서 검색, 소셜 및 Commerce을 위한 A/B 테스트 활동 만들기

다음 지침은 검색, 소셜 및 Commerce 사용 사례와 관련된 정보를 강조 표시합니다.

1. [Adobe Target에 로그인](https://experienceleague.adobe.com/docs/target/using/introduction/target-access-from-mac.html).

1. [A/B 테스트 만들기](https://experienceleague.adobe.com/docs/target/using/activities/abtest/create/test-create-ab.html):

   1. **[!UICONTROL Enter Activity URL]** 필드에 테스트용 랜딩 페이지 URL을 입력합니다.

   1. **[!UICONTROL Goal]** 필드에 테스트에 대한 성공 지표를 입력합니다.

      >[!NOTE]
      >
      >[!DNL Analytics]이(가) [!DNL Target] 내에서 데이터 원본으로 사용되고 올바른 보고서 세트가 선택되었는지 확인하십시오.

   1. 테스트 세그먼트의 사용자가 잘못된 온사이트 경험을 받을 때 충돌을 방지하려면 **[!UICONTROL Priority]**&#x200B;을(를) `High` 또는 `999`(으)로 설정하십시오.


   1. **[!UICONTROL Reporting Settings]** 내에서 Search, Social 및 Commerce 계정에 연결된 **[!UICONTROL Company Name]** 및 **[!UICONTROL Report Suite]**&#x200B;을(를) 선택하십시오.

      추가 보고 팁은 &quot;[보고 모범 사례 및 문제 해결](https://experienceleague.adobe.com/docs/analytics/analyze/reports-analytics/report-troubleshooting.html)&quot;을 참조하십시오.

   1. **[!UICONTROL Date Range]** 필드에 테스트에 대한 적절한 시작 날짜와 종료 날짜를 입력합니다.

   1. **[!UICONTROL Site Pages]** > **[!UICONTROL Landing Page]** > **[!UICONTROL Query]**&#x200B;을(를) 선택합니다. **[!UICONTROL Value]** 필드에 Search, Social 및 Commerce의 관련 광고 네트워크 엔터티에 대한 [!UICONTROL Network Account ID], [!UICONTROL Network Campaign ID], [!UICONTROL Network Adgroup ID] 또는 [!UICONTROL Network Ad ID]을(를) 입력합니다. 이를 통해 엔터티의 클릭스루 대상에 대해 [!DNL Target] 쿼리 문자열 매개 변수를 사용할 수 있습니다.

      [관련 ID 열을 엔터티 보기에 추가](/help/search-social-commerce/common-tasks/data-views/custom-default-views-manage.md)하여 ID를 찾을 수 있습니다.

      [!UICONTROL Accounts] 보기의 [!UICONTROL Accounts] 보기](/help/integrations/assets/target-search-id.png "[!UICONTROL Network Account ID] 열에 있는 ![[!UICONTROL Network Account ID] 열")

      지원이 필요한 경우 Adobe 계정 팀과 협력합니다.

   1. **[!UICONTROL Traffic Allocation Method]**&#x200B;에 대해 **[!UICONTROL Manual (Default)]**&#x200B;을(를) 선택하고 대상을 50/50으로 분할합니다.

   1. 활동을 저장합니다.

1. [Target 시각적 경험 작성기](https://experienceleague.adobe.com/docs/target/using/activities/abtest/create/test-create-ab.html)를 사용하여 A/B 테스트 랜딩 페이지 템플릿에 대한 디자인을 변경합니다.

   * 경험 A: 개인화가 없는 기본/제어 랜딩 페이지 경험이므로 편집하지 마십시오.

   * 경험 B: [!DNL Target] 사용자 인터페이스를 사용하여 테스트에 포함된 자산(예: 헤드라인, 사본, 단추 배치 및 크리에이티브)을 기반으로 랜딩 페이지 템플릿을 사용자 지정합니다.

   >[!NOTE]
   >
   >크리에이티브 테스트 사용 사례의 경우 Adobe 계정 팀에 문의하십시오.

## 2단계: [!DNL Analytics]에서 [!DNL Analytics for Target] Analysis Workspace 설정

[!DNL Analytics for Target](A4T)은(는) 광고주가 [!DNL Analytics] 전환 지표 및 대상 세그먼트를 기반으로 [!DNL Target] 활동을 만든 다음 [!DNL Analytics]을(를) 보고 소스로 사용하여 결과를 측정할 수 있는 솔루션 간 통합입니다. 해당 활동에 대한 모든 보고 및 세분화는 [!DNL Analytics] 데이터 수집을 기반으로 합니다.

구현 지침에 대한 링크를 포함하여 [!DNL Analytics for Target]에 대한 자세한 내용은 &quot;[Adobe Target용 보고 소스로서의 Adobe Analytics(A4T)](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4t.html)&quot;을(를) 참조하십시오.

### [!DNL Analytics for Target] 패널 설정

Analysis Workspace에서 [!DNL Target] 활동 및 경험을 분석하도록 [!DNL Analytics for Target panel]을(를) 구성합니다. 보고서에 대한 다음과 같은 중요한 지침과 정보를 숙지하십시오.

#### 지표

* 테스트가 실행된 Adobe Advertising 계정, 캠페인 또는 광고 그룹 <!-- only applicable entities? -->과(와) 관련된 작업 영역 내에 패널을 만듭니다. 요약 시각화를 사용하여 [!DNL Target] 테스트 성능과 동일한 보고서에 Adobe Advertising 지표를 표시합니다.

* 성과를 측정하기 위해 온사이트 지표(예: 방문 및 전환)를 사용하는 우선 순위를 지정합니다.

* Adobe Advertising의 집계된 미디어 지표(예: 노출 횟수, 클릭 수 및 비용)를 [!DNL Target] 지표와 일치시킬 수 없음을 이해합니다.

#### Dimension

다음 차원은 [!DNL Analytics for Target]과(와) 관련이 있습니다.

* **대상 활동**: A/B 테스트의 이름

* **타겟 경험**: 활동 내에 사용된 랜딩 페이지 경험의 이름

* **Target 활동** > **경험**: 같은 행에 있는 활동 이름과 경험 이름

### [!DNL Target] 데이터에 대한 Analytics 문제 해결

Analysis Workspace 내에서 활동 및 경험 데이터가 최소화되거나 채워지지 않는 것을 발견하면 다음을 수행하십시오.

* [!DNL Target]과(와) [!DNL Analytics]에 모두 동일한 [!UICONTROL Supplemental Data ID](SDID)가 사용되는지 확인하십시오. 캠페인이 사용자를 유도하는 랜딩 페이지에서 [Adobe Experience Cloud Debugger](https://experienceleague.adobe.com/docs/target-learn/tutorials/troubleshooting/troubleshoot-with-the-experience-cloud-debugger.html)를 사용하여 SDID 값을 확인할 수 있습니다.

[Adobe Debugger의 SDID(Supplemental Data ID) 값](/help/integrations/assets/target-troubleshooting-sdid.png)

* 같은 랜딩 페이지에서 a) [!UICONTROL Solutions] > [!UICONTROL Target] 아래의 Adobe Debugger에 표시된 [!UICONTROL Hostname]이(가) b) 활동의 [!DNL Target] ([!UICONTROL Goals & Settings] > [!UICONTROL Reporting Settings] 아래)에 표시된 [!UICONTROL Tracking Server]과(와) 일치하는지 확인하십시오.

  [!DNL Analytics For Target]을(를) 사용하려면 [!DNL Target]에서 Analytics용 [!DNL Modstats] 데이터 수집 서버로 호출하는 동안 [!DNL Analytics] 추적 서버를 보내야 합니다.<!-- just "to Analytics?"-->

[Adobe Debugger의 호스트 이름 값](/help/integrations/assets/target-troubleshooting-hostname.png)

[Target의 추적 서버 값](/help/integrations/assets/target-troubleshooting-tracking-server.png)

## 추가 읽기

* [Analytics와 Target 통합](https://experienceleague.adobe.com/docs/target-learn/tutorials/integrations/3.2-target-analytics.html) - Analysis Workspace에서 [!DNL Target] 보고를 설정하는 방법에 대해 설명합니다.
* [A/B 테스트 개요](https://experienceleague.adobe.com/docs/target/using/activities/abtest/test-ab.html) - 검색, 소셜 및 Commerce 광고에 사용할 수 있는 A/B 테스트 활동에 대해 설명합니다.
* [Advertising용 Analytics 개요](/help/integrations/analytics/overview.md) - Analytics 인스턴스에서 클릭스루 및 뷰스루 사이트 상호 작용을 추적할 수 있는 Advertising용 Analytics를 소개합니다.

>[!MORELIKETHIS]
>
>* [Advertising DSP 광고용 Adobe Target에서 A/B 테스트 구성](ab-tests-dsp.md)
