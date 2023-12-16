---
title: Adobe Target에서 Adobe Advertising 검색, 소셜 및 상거래 광고에 대한 A/B 테스트 구성
description: "에서 A/B 테스트를 설정하는 방법 알아보기 [!DNL Target] 에 대한 [!DNL Google Ads] 및 [!DNL Microsoft® Advertising] 검색, 소셜 및 커머스의 광고."
source-git-commit: 3e8290d85aba379ece4b6d488c01e4ddda2b554e
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 0%

---

# 광고 검색, 소셜 및 상거래 광고를 위한 Adobe Target에서 A/B 테스트 구성

*Advertising Search, Social 및 Commerce만 있는 광고주*

*[!DNL Google Ads]및 [!DNL Microsoft® Advertising] 계정만*

Adobe Advertising 및 Adobe Target을 사용하면 디지털 광고 트래픽에 대한 랜딩 페이지 경험 A/B 테스트를 쉽게 설정할 수 있습니다 [!DNL Google Ads] 및 [!DNL Microsoft® Advertising] 끝:

* 전환율(CVR) 및 획득 효율성 측정(CPA, CPL 및 CAC 등)을 개선합니다.

* 광고와 관련된 보다 개인화된 랜딩 페이지 경험을 제공합니다(예: 이미지/비디오 크리에이티브, 복사, 키워드 또는 기타 광고 신호를 랜딩 페이지에 일치).

기본 항목을 결합할 수도 있습니다 [[!DNL Analytics] 광고용](/help/integrations/analytics/overview.md) 및 [[!DNL Analytics] 대상 [!DNL Target]](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4t.html) Adobe Analytics에 통합되어 다음으로 테스트 데이터를 측정하고 시각화하는 통합 보고 차원 [!DNL Analytics] 지표 및 성공 이벤트.

전제 조건, A/B 테스트 설정 지침에 대해서는 다음 섹션을 참조하십시오. [!DNL Target] 검색, 소셜 및 상거래의 광고에서 클릭스루 트래픽에 대한 정의에서 테스트를 측정하고 시각화하는 방법에 대한 팁 [!DNL Analytics].

## 전제 조건

### 필수 제품

* 검색, 소셜 및 상거래
* [!DNL Target]

### 권장 제품 및 통합

* [!DNL Analytics]

* [[!DNL Analytics] 광고용](/help/integrations/analytics/overview.md) 통합<!-- necessary for testing view-throughs, which most advertisers want to do -->

* [[!DNL Analytics] 대상 [!DNL Target]](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4t.html) 통합

## 1단계: A/B 테스트 활동 만들기 [!DNL Target] 검색, 소셜 및 상거래용

다음 지침은 검색, 소셜 및 상거래 사용 사례와 관련된 정보를 강조 표시합니다.

1. [Adobe Target에 로그인](https://experienceleague.adobe.com/docs/target/using/introduction/target-access-from-mac.html).

1. [A/B 테스트 만들기](https://experienceleague.adobe.com/docs/target/using/activities/abtest/create/test-create-ab.html):

   1. 다음에서 **[!UICONTROL Enter Activity URL]** 필드에 테스트용 랜딩 페이지 URL을 입력합니다.

   1. 다음에서 **[!UICONTROL Goal]** 필드에 테스트에 대한 성공 지표를 입력합니다.

      >[!NOTE]
      >
      >다음을 확인합니다. [!DNL Analytics] 내에서 데이터 소스로 활성화됨 [!DNL Target]을 클릭하여 올바른 보고서 세트를 선택합니다.

   1. 설정 **[!UICONTROL Priority]** 끝 `High` 또는 `999` 테스트 세그먼트의 사용자가 잘못된 온사이트 경험을 받을 때 충돌을 방지하기 위해 입니다.


   1. 다음 범위 내 **[!UICONTROL Reporting Settings]**&#x200B;를 선택하고 **[!UICONTROL Company Name]** 및 **[!UICONTROL Report Suite]** 을 검색, 소셜 및 상거래 계정에 연결했습니다.

      추가 보고 팁은 &quot;[보고 우수 사례 및 문제 해결](https://experienceleague.adobe.com/docs/analytics/analyze/reports-analytics/report-troubleshooting.html).&quot;

   1. 다음에서 **[!UICONTROL Date Range]** 필드에 테스트에 대한 적절한 시작 날짜와 종료 날짜를 입력합니다.

   1. 선택 **[!UICONTROL Site Pages]** > **[!UICONTROL Landing Page]** > **[!UICONTROL Query]**. 다음에서 **[!UICONTROL Value]** 필드에 [!UICONTROL Network Account ID], [!UICONTROL Network Campaign ID], [!UICONTROL Network Adgroup ID], 또는 [!UICONTROL Network Ad ID] Search, Social, Commerce의 관련 광고 네트워크 엔티티용. 이를 통해 다음을 사용할 수 있습니다. [!DNL Target] 엔티티의 클릭스루 대상에 대한 쿼리 문자열 매개 변수입니다.

      다음 방법으로 ID를 찾을 수 있습니다. [엔티티 보기에 관련 ID 열 추가](/help/search-social-commerce/common-tasks/data-views/custom-default-views-manage.md).

      ![[!UICONTROL Network Account ID] 열의 [!UICONTROL Accounts] 보기](/help/integrations/assets/target-search-id.png "[!UICONTROL Network Account ID] 열의 [!UICONTROL Accounts] 보기")

      지원이 필요한 경우 Adobe 계정 팀과 협력합니다.

   1. 의 경우 **[!UICONTROL Traffic Allocation Method]**, 선택 **[!UICONTROL Manual (Default)]** 대상자를 50/50으로 나눕니다.

   1. 활동을 저장합니다.

1. 사용 [Target 시각적 경험 작성기](https://experienceleague.adobe.com/docs/target/using/activities/abtest/create/test-create-ab.html) A/B 테스트 랜딩 페이지 템플릿에 대한 디자인을 변경합니다.

   * 경험 A: 개인화가 없는 기본/제어 랜딩 페이지 경험이므로 편집하지 마십시오.

   * 경험 B: [!DNL Target] 테스트에 포함된 에셋(예: 헤드라인, 복사, 버튼 배치 및 크리에이티브)을 기반으로 랜딩 페이지 템플릿을 사용자 정의하는 사용자 인터페이스.

   >[!NOTE]
   >
   >크리에이티브 테스트 사용 사례의 경우 Adobe 계정 팀에 문의하십시오.

## 2단계: 설정 [!DNL Analytics for Target] Analysis Workspace in [!DNL Analytics]

[!DNL Analytics for Target] (A4T)는 광고주가 만들 수 있는 교차 솔루션 통합입니다 [!DNL Target] 활동 기준 [!DNL Analytics] 전환 지표 및 대상 세그먼트를 클릭한 다음 를 사용하여 결과를 측정합니다. [!DNL Analytics] 를 보고 소스로 사용합니다. 해당 활동에 대한 모든 보고 및 세분화는 [!DNL Analytics] 데이터 수집입니다.

에 대한 자세한 내용 [!DNL Analytics for Target], 구현 지침에 대한 링크를 포함하면 &quot;[Adobe Target용 보고 소스로서의 Adobe Analytics (A4T)](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4t.html)&quot;.

### 다음을 설정합니다. [!DNL Analytics for Target] 패널

Analysis Workspace에서 다음을 구성합니다 [!DNL Analytics for Target panel] 을(를) 분석하려면 [!DNL Target] 활동 및 경험. 보고서에 대한 다음과 같은 중요한 지침과 정보를 숙지하십시오.

#### 지표

* 작업 영역 내에서 Adobe Advertising 계정, 캠페인 또는 광고 그룹과 관련된 패널을 만듭니다<!-- only applicable entities? --> 테스트가 실행된 경우입니다. 요약 시각화를 사용하여 Adobe Advertising 지표를 와 동일한 보고서에 표시 [!DNL Target] 성능을 테스트합니다.

* 성과를 측정하기 위해 온사이트 지표(예: 방문 및 전환)를 사용하는 우선 순위를 지정합니다.

* Adobe Advertising의 집계된 미디어 지표(예: 노출 횟수, 클릭 수 및 비용)를 일치시킬 수 없음을 이해합니다. [!DNL Target] 지표.

#### Dimension

다음 차원은 다음과 같습니다 [!DNL Analytics for Target]:

* **Target 활동**: A/B 테스트 이름

* **Target 경험**: 활동 내에 사용된 랜딩 페이지 경험의 이름

* **Target 활동** > **경험**: 동일한 행의 활동 이름 및 경험 이름

### Analytics 문제 해결 [!DNL Target] 데이터

Analysis Workspace 내에서 활동 및 경험 데이터가 최소화되거나 채워지지 않는 것을 발견하면 다음을 수행하십시오.

* 동일한 [!UICONTROL Supplemental Data ID] (SDID)는 두 가지 모두에 사용됩니다 [!DNL Target] 및 [!DNL Analytics]. 다음을 사용하여 SDID 값을 확인할 수 있습니다. [Adobe Experience Cloud 디버거](https://experienceleague.adobe.com/docs/target-learn/tutorials/troubleshooting/troubleshoot-with-the-experience-cloud-debugger.html) 사용자를 유도하는 캠페인의 랜딩 페이지에서.

[Adobe Debugger의 SDID(Supplemental Data ID) 값](/help/integrations/assets/target-troubleshooting-sdid.png)

* 동일한 랜딩 페이지에서 가) [!UICONTROL Hostname] 아래의 Adobe Debugger에 표시됨 [!UICONTROL Solutions] > [!UICONTROL Target] b) 와 일치합니다. [!UICONTROL Tracking Server] 표시 위치 [!DNL Target] 활동용(아래) [!UICONTROL Goals & Settings] > [!UICONTROL Reporting Settings]).

  [!DNL Analytics For Target] 을(를) 필요로 합니다. [!DNL Analytics] 호출 시 보낼 추적 서버 [!DNL Target] (으)로 [!DNL Modstats] analytics용 데이터 수집 서버.<!-- just "to Analytics?"-->

[Adobe Debugger의 호스트 이름 값](/help/integrations/assets/target-troubleshooting-hostname.png)

[Target의 추적 서버 값](/help/integrations/assets/target-troubleshooting-tracking-server.png)

## 추가 읽기

* [Analytics와 Target 통합](https://experienceleague.adobe.com/docs/target-learn/tutorials/integrations/3.2-target-analytics.html) - 설정 방법을 설명합니다. [!DNL Target] Analysis Workspace에서 보고.
* [A/B 테스트 개요](https://experienceleague.adobe.com/docs/target/using/activities/abtest/test-ab.html) - 검색, 소셜 및 상거래 광고와 함께 사용할 수 있는 A/B 테스트 활동에 대해 설명합니다.
* [Analytics for Advertising 개요](/help/integrations/analytics/overview.md) - Analytics 인스턴스에서 클릭스루 및 뷰스루 사이트 상호 작용을 추적할 수 있는 Analytics for Advertising을 소개합니다.

>[!MORELIKETHIS]
>
>* [Advertising DSP Ads용 Adobe Target에서 A/B 테스트 구성](ab-tests-dsp.md)
