---
title: ' [!DNL Analytics for Advertising] 개요'
description: ' [!DNL Analytics for Advertising] 개요'
feature: Integration with Adobe Analytics
exl-id: 94558478-ffa6-4b83-bc79-c7589fe0f14c
source-git-commit: 8911f6ea16878bede96151f004e6de2717484140
workflow-type: tm+mt
source-wordcount: '1223'
ht-degree: 0%

---

# [!DNL Analytics for Advertising] 개요

*Advertising DSP 및[!DNL Advertising Search, Social, & Commerce]*&#x200B;을(를) 사용하는 광고주

[!DNL Analytics for Advertising]은(는) Adobe Analytics과 Adobe Advertising을 통합하여 각 제품의 기능을 확장하고 향상합니다.

이 통합을 통해 광고주는 [!DNL Analytics] 인스턴스에서 클릭스루 및 뷰스루 사이트 상호 작용을 추적할 수 있으므로 브랜드는 광고 지출이 사이트 참여 및 중요한 비즈니스 목표로 이어지는 방식을 확인할 수 있습니다.

또한 Adobe Advertising은 [!DNL Analytics]이(가) 사이트에 이미 있는 [!DNL Analytics] 태그를 사용하여 수집하는 방대한 자사 데이터에 액세스할 수 있습니다. 이를 통해 보다 강력한 여정 관리, 자사 리마케팅 및 유료 미디어 사이트 보고를 수행할 수 있습니다. Adobe Advertising은 지출 및 입찰 최적화에 [!DNL Analytics] 데이터를 추가로 사용할 수 있습니다.

올바르게 작동하면 [!DNL Analytics for Advertising]은(는) 광고 여정 관리(광고를 통해 사용자를 사이트로 보내는 행위)와 웹 분석을 통해 해당 사이트 참여를 이해하는 것과 같은 두 가지 기존의 역할 사이의 선을 흐리게 합니다.

주요 이점:

* 자사 사이트 리마케팅을 위해 [!DNL Analytics] 세그먼트를 Adobe Advertising에 직접 보냅니다.
* 유료 미디어 광고를 최적화하기 위한 전환 신호로 [!DNL Analytics] 사용자 지정 및 표준 이벤트를 사용합니다.
* 사이트 시작 지점 및 방문 동작을 더 잘 이해하려면 [!DNL Analytics] Analysis Workspace을 활용하십시오.
* 웹 분석가와 유료 미디어 팀 간의 긴밀한 공동 작업을 활성화합니다.
* [!DNL Analytics] 내의 영구 Adobe Advertising 뷰스루 및 클릭스루 ID를 사용하여 사이트 참여를 이해합니다.
* 데이터나 픽셀을 광고 서버나 다른 DSP으로 내보낼 때 얻을 수 없는 사용자 지정 지표, 사용자 지정 차원 및 사이트 활동을 통해 Analysis Workspace의 기존 유료 미디어 보고서를 개선합니다.
* Adobe Advertising 내 추적 및 최적화를 위해 웹 사이트에 이미 있는 [!DNL Analytics] 코드를 활용하십시오.

>[!TIP]
>
> [비디오 소개 [!DNL Analytics for Advertising]](https://experienceleague.adobe.com/docs/advertising-learn/tutorials/analytics/intro-a4adc.html?lang=ko#analytics)를 시청하세요.

## 유료 미디어 보고를 위해 Analytics 사용

[!DNL Analytics for Advertising]은(는) 다음 작업을 수행하여 광고가 사이트 동작을 유도하는 방식에 대한 보고와 통찰력을 향상시킵니다.

* [!DNL Analytics] 내의 영구 Adobe Advertising 뷰스루 및 클릭스루 ID를 사용하여 사이트 참여를 이해합니다.
* Analysis Workspace을 활용하여 사이트 시작 지점 및 방문 동작을 보다 잘 이해할 수 있습니다. Adobe Advertising 캠페인 엔티티 이름(배치 및 광고까지) 및 관련 지표(예: 클릭, 노출 횟수 및 비용)가 포함된 유료 미디어 차원 및 이벤트 데이터에 액세스할 수 있습니다.

[!DNL Analytics]을(를) 유료 미디어 보고 도구로 사용하려면 조직에서 Analysis Workspace에 액세스할 수 있는 Experience Cloud 로그인이 필요합니다. Adobe Advertising 팀은 Adobe Advertising 데이터를 Analysis Workspace의 개별 보고서 세트에 매핑하는 데 도움이 됩니다. Adobe Advertising 데이터를 모든 보고서 세트에 보낼 수 있지만, Adobe Advertising에 매핑된 보고서 세트와 매핑되지 않은 보고서 세트를 알고 있어야 합니다. 보고서 세트에 따라, 보고된 데이터가 변경될 수 있습니다.

 [!DNL Analytics][&#128279;](ids.md) 내의 Adobe Advertising ID는 사용자 지정 영구 만료로 다른 [!DNL eVars]과(와) 동일하게 작동합니다. 기본적으로 Adobe Advertising 구현 중에 속성 전환 확인 기간은 60일로 설정됩니다. 이 설정을 변경하려면 Adobe 계정 팀과 작업하십시오.

Adobe Advertising 차원은 접미사 &quot;(AMO ID)&quot;(예: &quot;광고 유형(AMO ID)&quot;)와 함께 추가됩니다. 사용 가능한 차원 목록은 &quot;[Analysis Workspace의 Adobe Advertising 지표](advertising-metrics-in-analytics.md)&quot;을 참조하십시오.

>[!NOTE]
>
> [!DNL Analytics] 내에서 Adobe Advertising 데이터(또는 데이터 세트)를 볼 때는 지표와 보고서가 [!DNL Analytics] 내에 설정된 규칙을 기반으로 한다는 것을 알고 있어야 합니다. 데이터는 광고 서버 보고서, [!DNL DSP] 보고서 또는 검색 엔진 보고서와 같은 다른 보고 시스템 내에서 표시되는 데이터와 다를 수 있습니다. [!DNL Analytics]의 데이터 차이점을 이해하려면 [!DNL eVar] 데이터가 언제 만료되는지, 방문을 정의하는지, 마지막 터치 속성 대 총 지속 속성으로 간주되는 것과 기타 요인을 알아야 합니다. 자세한 내용은 [과(와) Adobe Advertising 사이의 예상 데이터 차이 [!DNL Analytics] 를 참조하십시오](data-variances.md).

## Analytics를 사용하여 Adobe Advertising 캠페인 및 Portfolio 강화

추가 픽셀 없이도 [!DNL Analytics for Advertising]은(는) 두 개의 기본 신호를 Adobe Advertising으로 전송하여 최적화를 향상시키고 대상 세그멘테이션을 보다 쉽게 할 수 있습니다.

* 입찰 신호로 사용할 전환 지표:
   * [!UICONTROL Revenue] 및 [!UICONTROL Cart Views]과(와) 같은 표준 지표.
   * 페이지 보기 및 방문 지표와 같은 사이트 참여 지표
   * 사용자 지정 매출 지표.
   * 예약된 매출 지표.
* [!DNL Analytics]에서 만들어 Experience Cloud에 게시한 세그먼트입니다.

  [!DNL DSP]의 자사 사이트 리타기팅 및 유료 검색 광고에 [!DNL Analytics]개의 세그먼트를 사용할 수 있습니다.

  ([!DNL Search, Social, & Commerce]만 해당) [!DNL Analytics]을(를) 갖지만 Audience Manager을 하지 않는 광고주는 Experience Cloud과 공유된 [!DNL Analytics] 세그먼트에서 Google 웹 사이트 태그 기반 대상(리마케팅 목록) 및 고객 일치 대상(고객 목록)을 만들 수도 있습니다.

### 입찰 신호로서의 사이트 전환 지표

[!DNL Analytics]의 표준 이벤트와 사용자 지정 이벤트를 사용하여 Adobe Advertising에서 가중 목표를 작성할 수 있습니다. 목표는 [!DNL DSP] 패키지 및 Search, Social, Commerce 포트폴리오에 대한 입찰 결정을 알려줍니다.

검색, 소셜 및 Commerce 하이브리드 포트폴리오의 [!DNL Google Ads] 및 [!DNL Google Microsoft Advertising] 캠페인의 경우 선택적으로 목표의 [!DNL Analytics] 이벤트를 포함한 목표를 광고 네트워크에 직접 업로드할 수 있습니다. 그러면 이 목표를 계정 수준 및 캠페인 수준 사용자 지정 전환 목표에 대한 전환 작업으로 사용할 수 있습니다.

>[!NOTE]
>
> [!DNL Analytics]의 계산된 지표를 Adobe Advertising에 매핑할 수 없습니다.

Adobe Advertising 팀이 유료 미디어 성능에 적용할 수 있는 이벤트를 식별하고 Adobe Advertising에 매핑하는 데 도움을 줍니다. [!UICONTROL Search] > [!UICONTROL Admin] > [!UICONTROL Conversions]에 나열되어 있습니다.

사용 가능한 지표 목록은 &quot;[Adobe Advertising의 Analytics 지표](analytics-data-in-advertising.md)&quot;을 참조하십시오.

### 사이트 재타겟팅을 위한 Analytics 세그먼트

Adobe Advertising은 [!DNL Analytics]과(와) Experience Cloud 간의 기본 Experience Cloud 대상 통합을 사용하여 Advertising DSP 및 [!DNL Search, Social, & Commerce] 광고에 대한 리마케팅 목적으로 [!DNL Analytics]개 세그먼트를 수집할 수 있습니다.

[!DNL Analytics] 세그먼트에 액세스하려면 광고주 계정이 [Experience Cloud ID 서비스](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=ko)를 사용하도록 설정해야 합니다. ID 서비스가 활성화되면 처리되는 즉시 모든 Experience Cloud 세그먼트([!DNL Analytics]에서 만들어지고 Experience Cloud에 게시된 세그먼트, Adobe Audience Manager에서 만들어진 세그먼트, [!DNL People core service]을(를) 사용하여 Experience Cloud에서 만들어진 세그먼트, Adobe Experience Platform에서 만들어지고 Audience Manager을 통해 Adobe Advertising으로 전송된 세그먼트 포함)를 Adobe Advertising 내에서 사용할 수 있습니다.

[!DNL Analytics] 세그먼트는 24시간 내에 사용할 수 있으며 매일 업데이트됩니다.

Experience Cloud 대상 서비스에 대한 자세한 내용은 [Experience Cloud 대상](https://experienceleague.adobe.com/docs/core-services/interface/audiences/audience-library.html?lang=ko)을 참조하세요.

## 통합 사용 방법의 예 {#integration-examples}

### Analysis Workspace에서 Adobe Advertising 데이터 사용

Adobe Advertising 데이터를 사용하여 Analysis Workspace에서 시각적 보고서를 만드는 방법에 대해 알아보려면 비디오 &quot;[Workspace 및 보고 소개](https://experienceleague.adobe.com/docs/advertising-learn/tutorials/analytics/analytics-analysis-workspace-a4adc.html?lang=ko)&quot;를 참조하십시오.

#### 보고서에서 연결된 TV 뷰스루 전환 사용

*Advertising DSP 사용자만*

CTV 장치의 광고 노출을 현장 전환과 연결하여 연결된 TV(CTV) 캠페인의 전체 단계 효과를 측정할 수 있습니다. 새 [!UICONTROL Landing Type] 필터 &quot;[!UICONTROL View-through (CTV)]&quot;은(는) 변환을 [!UICONTROL Click Through], [!UICONTROL View Through] 및 [!UICONTROL View Through (CTV)] 값에 대한 별도의 행으로 분할합니다.

CTV 뷰스루 전환 지표를 보려면 Analysis Workspace의 배치 보기 또는 마케팅 채널 보기를 사용하십시오.

배치 뷰를 사용하여 다음을 수행합니다.

1. 보고 보기에 CTV 지출 배치를 포함합니다.

1. &quot;노출 횟수&quot;, &quot;클릭 수&quot; 등과 같이 원하는 지표를 포함합니다.

1. 다음 필터를 적용합니다.

   광고 플랫폼: `Advertising Cloud DSP`

   랜딩 페이지: `View-Through (CTV)`

마케팅 채널 보기 사용:

1. `Marketing Channel` 차원을 포함합니다.

1. &quot;노출 횟수&quot;, &quot;클릭 수&quot; 등과 같이 원하는 지표를 포함합니다.

1. 다음 필터를 적용합니다.

   광고 플랫폼: `Advertising Cloud DSP`

   랜딩 페이지: `View-Through (CTV)`

### Adobe Advertising 대시보드 만들기

Analysis Workspace에서 목표에 대한 Adobe Advertising 데이터를 추적하는 방법에 대해 알아보려면 &quot;[Adobe Analytics을 사용하여 Adobe Advertising 대시보드 만들기](https://experienceleague.adobe.com/docs/advertising-learn/tutorials/analytics/analytics-dashboards-a4adc.html?lang=ko)&quot; 비디오를 참조하십시오.

### 사이트 시작 분석에 Adobe Advertising ID 사용

Adobe Advertising 사이트 시작 보고서를 만들어 요일, 시간, 브라우저 및 지리적 영향을 모니터링하는 방법은 비디오 &quot;[Adobe Advertising 사이트 시작 보고서 만들기](https://experienceleague.adobe.com/docs/advertising-learn/tutorials/analytics/analytics-site-entry-a4adc.html?lang=ko)&quot;를 참조하십시오.

## [!DNL Analytics for Advertising] 구현을 시작하는 방법

시작하는 데 필요한 초기 구성을 완료하고 조직의 요구 사항에 따라 구현 및 데이터 사용을 계획하는 데 도움이 되는 Adobe 계정 팀에 문의하십시오.

>[!MORELIKETHIS]
>
>* [비디오: 소개 [!DNL Analytics for Advertising]](https://experienceleague.adobe.com/docs/advertising-learn/tutorials/analytics/intro-a4adc.html?lang=ko)
>* [구현을 위한 필수 구성 요소 및 키 정보 [!DNL Analytics for Advertising]](prerequisites.md)
>* [Analytics에서 사용하는 Adobe Advertising ID](ids.md)
>* [Advertising용 Analytics용 JavaScript 코드](/help/integrations/analytics/javascript.md)
>* [과(와) Adobe Advertising  [!DNL Analytics]  사이의 예상 데이터 분산](data-variances.md)
>* Analysis Workspace의 [Adobe Advertising 지표](/help/integrations/analytics/advertising-metrics-in-analytics.md)
>* [[!DNL Analytics] Adobe Advertising의 데이터](/help/integrations/analytics/analytics-data-in-advertising.md)
