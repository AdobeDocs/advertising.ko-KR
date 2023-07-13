---
title: 개요 [!DNL Analytics for Advertising]
description: 개요 [!DNL Analytics for Advertising]
feature: Integration with Adobe Analytics
exl-id: 94558478-ffa6-4b83-bc79-c7589fe0f14c
source-git-commit: d4306553d4ad7379672be5bff1bc5cc6f74f70bf
workflow-type: tm+mt
source-wordcount: '1185'
ht-degree: 0%

---

# 개요 [!DNL Analytics for Advertising]

*Advertising DSP 및[!DNL Advertising Search, Social, & Commerce]*

[!DNL Analytics for Advertising] Adobe Analytics과 Adobe Advertising을 통합하여 각 제품의 기능을 확장하고 향상합니다.

이 통합을 통해 광고주는 자신의 클릭스루 및 뷰스루 사이트 상호 작용을 추적할 수 있습니다 [!DNL Analytics] 인스턴스: 브랜드가 광고 지출이 사이트 참여 및 중요한 비즈니스 목표로 이어지는 방식을 확인할 수 있습니다.

또한 Adobe Advertising은 다음과 같은 방대한 자사 데이터에 액세스할 수 있습니다 [!DNL Analytics] 다음을 사용하여 수집 [!DNL Analytics] 태그가 사이트에 이미 있습니다. 이를 통해 보다 강력한 여정 관리, 자사 리마케팅 및 유료 미디어 사이트 보고를 수행할 수 있습니다. Adobe Advertising은 [!DNL Analytics] 지출 및 입찰 최적화를 위한 데이터.

제대로 채용되면, [!DNL Analytics for Advertising] 는 광고 여정 관리(광고를 통해 사용자를 사이트로 보내는 행위)와 웹 분석을 통한 사이트 참여 이해와 같은 두 가지 기존 역할 사이의 선을 흐리게 합니다.

주요 이점:

* 보내기 [!DNL Analytics] 자사 사이트 리마케팅을 위해 Adobe Advertising에 직접 세그먼트화할 수 있습니다.
* 사용 [!DNL Analytics] 유료 미디어 광고를 최적화하기 위한 전환 신호로서 사용자 지정 및 표준 이벤트.
* 활용 [!DNL Analytics] Analysis Workspace을 통해 사이트 시작 지점 및 방문 동작을 보다 잘 이해할 수 있습니다.
* 웹 분석가와 유료 미디어 팀 간의 긴밀한 공동 작업을 활성화합니다.
* 내에서 영구 Adobe 광고 뷰스루 및 클릭스루 ID 사용 [!DNL Analytics] 사이트 참여를 이해할 수 있습니다.
* 데이터나 픽셀을 광고 서버나 다른 DSP으로 내보낼 때 얻을 수 없는 사용자 지정 지표, 사용자 지정 차원 및 사이트 활동을 통해 Analysis Workspace의 기존 유료 미디어 보고서를 개선합니다.
* 활용 [!DNL Analytics] 코드는 Adobe Advertising 내에서 추적 및 최적화를 위해 웹 사이트에 이미 있습니다.

>[!TIP]
>
> 시청 [비디오 소개 [!DNL Analytics for Advertising]](https://experienceleague.adobe.com/docs/advertising-learn/tutorials/analytics/intro-a4adc.html#analytics).

## 유료 미디어 보고를 위해 Analytics 사용

[!DNL Analytics for Advertising] 에서는 다음 작업을 수행하여 광고가 사이트 동작을 유도하는 방식에 대한 보고 및 통찰력을 향상시킵니다.

* 내에서 영구 Adobe 광고 뷰스루 및 클릭스루 ID 사용 [!DNL Analytics] 사이트 참여를 이해할 수 있습니다.
* Analysis Workspace을 활용하여 사이트 시작 지점 및 방문 동작을 보다 잘 이해할 수 있습니다. Adobe Advertising 캠페인 엔티티 이름(배치 및 광고까지) 및 관련 지표(예: 클릭, 노출 횟수 및 비용)가 포함된 유료 미디어 차원 및 이벤트 데이터에 액세스할 수 있습니다.

사용 [!DNL Analytics] 조직에 유료 미디어 보고 도구로 Analysis Workspace에 대한 액세스 권한이 있는 Experience Cloud 로그인이 필요합니다. Adobe Advertising 팀은 Adobe Advertising 데이터를 Analysis Workspace의 개별 보고서 세트에 매핑하는 데 도움이 됩니다. Adobe Advertising 데이터를 모든 보고서 세트에 보낼 수 있지만, Adobe Advertising에 매핑된 보고서 세트와 매핑되지 않은 보고서 세트를 알고 있어야 합니다. 보고서 세트에 따라, 보고된 데이터가 변경될 수 있습니다.

[내 Adobe Advertising ID [!DNL Analytics]](ids.md) 사용자 지정 영구 만료 기능을 사용하는 다른 eVar와 마찬가지로 작동합니다. 기본적으로 Adobe 광고 구현 중에 속성 전환 확인 기간은 60일로 설정됩니다. 이 설정을 변경하려면 Adobe 계정 팀과 작업하십시오.

Adobe Advertising 차원은 접미사 &quot;(AMO ID)&quot;(예: &quot;광고 유형(AMO ID)&quot;)와 함께 추가됩니다. 를 참조하십시오.[Analysis Workspace에서 광고 지표 Adobe](advertising-metrics-in-analytics.md)사용 가능한 차원 목록에 대해 설명합니다.

>[!NOTE]
>
> 내에서 Adobe Advertising 데이터(또는 데이터 세트)를 보는 경우 [!DNL Analytics], 지표 및 보고서는 내에 설정된 규칙을 기반으로 합니다 [!DNL Analytics]. 데이터는 광고 서버 보고서와 같은 다른 보고 시스템 내에서 표시되는 데이터와 다를 수 있습니다. [!DNL DSP] 보고서 또는 검색 엔진 보고서. 의 데이터 차이점을 이해하려면 [!DNL Analytics], eVar 데이터가 만료되는 시기, 방문을 정의하는 내용, 마지막 터치 속성 대 총 지속 속성으로 간주되는 내용 및 기타 요인을 알아야 합니다. 자세한 내용은 [다음 사이에 예상되는 데이터 분산: [!DNL Analytics] 및 Adobe Advertising](data-variances.md).

## Analytics를 사용하여 Adobe Advertising 캠페인 및 Portfolio 강화

추가 픽셀 필요 없이 [!DNL Analytics for Advertising] 는 두 개의 기본 신호를 Adobe Advertising으로 전송하여 최적화를 향상시키고 대상 세그멘테이션을 보다 쉽게 수행할 수 있도록 합니다.

* 입찰 신호로 사용할 전환 지표:
   * 표준 지표(예: ) [!UICONTROL Revenue] 및 [!UICONTROL Cart Views].
   * 페이지 보기 및 방문 지표와 같은 사이트 참여 지표
   * 사용자 지정 매출 지표.
   * 예약된 매출 지표.
* 다음에서 생성된 세그먼트 [!DNL Analytics] Experience Cloud에 게시됩니다.

  다음을 사용할 수 있습니다. [!DNL Analytics] 에서 자사 사이트 재타겟팅용 세그먼트 [!DNL DSP] 유료 검색 광고.

  ([!DNL Search, Social, & Commerce] 만 해당) [!DNL Analytics] 그러나 Audience Manager은에서 Google 웹 사이트 태그 기반 대상(리마케팅 목록) 및 고객 일치 대상(고객 목록)을 만들 수도 없습니다. [!DNL Analytics] Experience Cloud과 공유되는 세그먼트입니다.

### 입찰 신호로서의 사이트 전환 지표

에서 표준 이벤트와 사용자 지정 이벤트를 사용할 수 있습니다. [!DNL Analytics] Adobe Advertising에서 가중 목표를 수립합니다. 목표에 입찰 결정을 알립니다. [!DNL DSP] 패키지 및 검색 포트폴리오.

>[!NOTE]
>
> 다음에서 계산된 지표를 매핑할 수 없음: [!DNL Analytics] Adobe Advertising.

Adobe Advertising 팀은 유료 미디어 성능에 적용할 수 있는 이벤트를 식별하고 Adobe Advertising에 매핑하는 데 도움이 됩니다. 해당 이벤트는에 표시됩니다. [!UICONTROL Search] > [!UICONTROL Admin] > [!UICONTROL Transaction Properties].

를 참조하십시오.[Adobe Advertising의 Analytics 지표](analytics-data-in-advertising.md)사용 가능한 지표 목록.

### 사이트 재타겟팅을 위한 Analytics 세그먼트

Adobe Advertising 수집 가능 [!DNL Analytics] Advertising DSP 및 용 리마케팅 목적의 세그먼트 [!DNL Search, Social, & Commerce] 광고 사이에 기본 Experience Cloud 대상 통합을 사용하는 광고 [!DNL Analytics] Experience Cloud.

에 액세스하려면 [!DNL Analytics] 세그먼트, 광고주 계정에는 [Experience Cloud ID 서비스](https://experienceleague.adobe.com/docs/id-service/using/home.html) 활성화되었습니다. ID 서비스가 활성화되면 모든 Experience Cloud 세그먼트 (에서 만든 세그먼트 포함) [!DNL Analytics] 및 을(를) Experience Cloud에 게시하고, Adobe Audience Manager에서 만든 세그먼트, 를 사용하여 Experience Cloud에서 만든 세그먼트 [!DNL People core service], Adobe Experience Platform에서 만들어져 Audience Manager을 통해 Adobe Advertising으로 전송된 세그먼트 등은 처리되는 즉시 Adobe Advertising 내에서 사용할 수 있습니다.

[!DNL Analytics] 세그먼트는 24시간 이내에 사용할 수 있으며 매일 업데이트됩니다.

Experience Cloud 대상 서비스에 대한 자세한 내용은 [Experience Cloud 대상](https://experienceleague.adobe.com/docs/core-services/interface/audiences/audience-library.html).

## 통합 사용 방법의 예 {#integration-examples}

### Analysis Workspace에서 Adobe 광고 데이터 사용

Adobe Advertising 데이터를 사용하여 Analysis Workspace에서 시각적 보고서를 만드는 방법에 대해 알아보려면 비디오 를 참조하십시오.[작업 영역 및 보고 소개](https://experienceleague.adobe.com/docs/advertising-learn/tutorials/analytics/analytics-analysis-workspace-a4adc.html).&quot;

#### 보고서에서 연결된 TV 뷰스루 전환 사용

*Advertising DSP 사용자만*

CTV 장치의 광고 노출을 현장 전환과 연결하여 연결된 TV(CTV) 캠페인의 전체 단계 효과를 측정할 수 있습니다. CTV 뷰스루 전환 지표를 보려면 Analysis Workspace의 배치 보기 또는 마케팅 채널 보기를 사용하십시오.

배치 뷰를 사용하여 다음을 수행합니다.

1. 보고 보기에 CTV 지출 배치를 포함합니다.

1. &quot;노출 횟수&quot;, &quot;클릭 수&quot; 등과 같이 원하는 지표를 포함합니다.

1. 다음 필터를 적용합니다.

   광고 플랫폼: `Advertising Cloud DSP`

   랜딩 페이지: `View-Through (CTV)`

마케팅 채널 보기 사용:

1. 차원 포함 `Marketing Channel`.

1. &quot;노출 횟수&quot;, &quot;클릭 수&quot; 등과 같이 원하는 지표를 포함합니다.

1. 다음 필터를 적용합니다.

   광고 플랫폼: `Advertising Cloud DSP`

   랜딩 페이지: `View-Through (CTV)`

### Adobe Advertising 대시보드 만들기

Analysis Workspace에서 목표에 따라 Adobe Advertising 데이터를 추적하는 방법에 대해 알아보려면 비디오 를 참조하십시오.[Adobe Analytics을 사용하여 Adobe Advertising 대시보드 만들기](https://experienceleague.adobe.com/docs/advertising-learn/tutorials/analytics/analytics-dashboards-a4adc.html).&quot;

### 사이트 시작 분석에 Adobe Advertising ID 사용

Adobe Advertising 사이트 시작 보고서를 만들어 요일, 시간, 브라우저 및 지리적 영향을 모니터링하는 방법을 보려면 비디오 를 참조하십시오.[Adobe Advertising 사이트 시작 보고서 만들기](https://experienceleague.adobe.com/docs/advertising-learn/tutorials/analytics/analytics-site-entry-a4adc.html).&quot;

>[!MORELIKETHIS]
>
>* [비디오: 소개 [!DNL Analytics for Advertising]](https://experienceleague.adobe.com/docs/advertising-learn/tutorials/analytics/intro-a4adc.html)
>* [구현을 위한 사전 요구 사항 및 주요 정보 [!DNL Analytics for Advertising]](prerequisites.md)
>* [Analytics에서 사용하는 Adobe Advertising ID](ids.md)
>* [Advertising용 Analytics에 대한 JavaScript 코드](/help/integrations/analytics/javascript.md)
>* [다음 사이에 예상되는 데이터 분산: [!DNL Analytics] 및 Adobe Advertising](data-variances.md)
>* [Analysis Workspace에서 광고 지표 Adobe](/help/integrations/analytics/advertising-metrics-in-analytics.md)
>* [[!DNL Analytics] Adobe 광고의 데이터](/help/integrations/analytics/analytics-data-in-advertising.md)
