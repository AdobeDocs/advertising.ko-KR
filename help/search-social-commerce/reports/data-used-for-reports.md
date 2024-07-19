---
title: 보고서에 사용된 데이터
description: 데이터 보기 및 사용자 지정 보고서에서 사용할 수 있는 다양한 유형의 데이터에 대해 알아봅니다.
exl-id: ba808b21-4421-4de5-9293-a20ec67cc81c
feature: Search Reports
source-git-commit: 840c7f6295b73a784725c301a78ae89c827fd45e
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---

# 보고서에 사용된 데이터

검색, 소셜 및 Commerce에는 클릭 및 전환 데이터를 기반으로 하는 포괄적인 성능 보고서 세트가 포함되어 있습니다. [!UICONTROL Portfolios] 및 [!UICONTROL Campaigns] 보기에서 포트폴리오 또는 광고 계정의 다양한 구성 요소에 대한 기본 성과 데이터를 볼 수 있을 뿐만 아니라 다양한 기본 및 고급 보고서를 생성할 수도 있습니다.

또한 Adobe Advertising 전환 추적 서비스를 사용하는 광고주는 참조 웹 사이트의 지리적 위치 또는 도메인 이름에 대한 클릭 수, 각 채널의 광고 및 전환으로 이어지는 다양한 이벤트가 전체 전환율에 기여하는 방법, 마케팅 채널별 단일 [전환 지표](/help/search-social-commerce/admin/conversion-metrics/conversion-metric-about.md)에 대한 전환 분포를 식별할 수 있습니다. 사용 가능한 보고서는 사용자 계정 유형에 따라 다릅니다. Adobe 계정 팀은 모든 보고서에 액세스할 수 있습니다.

대부분의 보고서는 보려는 정보만 표시하도록 사용자 지정할 수 있습니다. 다음 표준 지표는 대부분의 보고서에서 사용할 수 있으며 광고 수준에서 계산됩니다.

* **표준 성능 지표:**

   * **[!UICONTROL Impressions]:** 광고가 배치된 총 횟수입니다.

   * **[!UICONTROL Clicks]:** 광고에서 링크를 클릭한 총 횟수입니다.

   * **[!UICONTROL Cost]:** 광고의 총 비용입니다. PPC(Pay-per-Click) 광고 비용은 항상 클릭 수에 클릭당 비용을 곱한 것입니다.

   * **[!UICONTROL Cost per Click]:** 광고에 대한 한 번의 클릭에 대한 평균 비용입니다. 광고의 비용을 광고의 총 클릭 수로 나눈 값입니다. 예를 들어 광고 노출에 100USD를 사용하고 광고가 10번의 클릭을 생성하는 경우 클릭당 비용은 100USD/10=10USD입니다.

   * **[!UICONTROL Average Position]:**(해당되는 경우) 노출 횟수로 가중치가 적용된 광고의 평균 위치입니다.

   * **[!UICONTROL Estimated Clicks]:**(Adobe Advertising 전환 추적 서비스를 사용하는 광고주를 위한 고급 보고서에만 포함됨) 참조 웹 사이트의 도시 또는 도메인 이름에 대한 총 예상 클릭 수입니다. 여기에는 광고주가 광고 계정을 가지고 있지 않은 광고 네트워크에 대한 데이터가 포함될 수 있습니다.

* **전환 지표:** 광고주의 각 전환 지표 또는 전환 지표에 대해 추적된 트랜잭션 데이터에 대한 총 전환 수입니다. 여기에는 전환 및 사이트 참여 지표가 포함될 수 있지만 Adobe Analytics에서 동기화되는 계산된 지표 및 고급 계산된 지표는 포함되지 않습니다.

  광고주 계정에 대해 동기화된 [[!DNL Google Ads]개의 추적 전환](/help/search-social-commerce/campaign-management/introduction/google-conversion-data.md) 및 [[!DNL Google Analytics]개의 추적 전환](/help/search-social-commerce/admin/data-sources/data-source-about.md)도 여기에 포함될 수 있습니다.

* **사용자 지정 지표:** 기존 지표(예: 주문당 비용)를 기반으로 수식을 만들어 파생되는 고유한 지표입니다.

## 데이터 가용성

보고서를 생성할 때 전환으로 이어지는 일련의 이벤트에서 전환 데이터를 속성 지정하는 방법을 선택할 수 있습니다. 예를 들어 전체 전환을 마지막 이벤트에 기여하거나 마지막 이벤트의 가중치를 다른 이벤트보다 더 높게 지정할 수 있습니다. 기본적으로 전환은 마지막 이벤트에 기여합니다.

보고서에 대해 지정하는 속성 규칙에 따라 다음 날짜에 각 보고서 유형의 데이터를 사용할 수 있습니다.

| 보고서 그룹 | 보고서 | 데이터를 사용할 수 있는 날짜 |
|---|---|---|
| [!UICONTROL Basic Reports] | [!UICONTROL Campaign Hourly Report] | 2021년 5월 15일부터 시작.<br><br><b>예외:</b> 강조 지표 데이터는 2022년 9월 8일부터 사용할 수 있습니다. |
| | 다른 모든 [!UICONTROL Basic Reports] | 지난 36개월.<br><br><b>예외:</b> 강조 지표 데이터는 2022년 9월 8일부터 사용할 수 있습니다. |
| [!UICONTROL Advanced Reports] | [!UICONTROL Transaction Report] | 이전 45일. |
| | [!UICONTROL Domain Referral Report], [!UICONTROL Geo Distribution Report] | 이전 두 달(2)과 현재 달의 더하기. |
| [!UICONTROL Assist Reports] | 모두 | 지난 18개월. |
| [!UICONTROL Specialty Reports] | [!UICONTROL AdWords Audience Target Report] | 이전 연도. |
| | [!UICONTROL RSA Assets Report] | 2022년 8월 10일부터 시작. |
| | [!UICONTROL MSA Ad Extension by Ad Report], [!UICONTROL MSA Ad Extension by Keyword Report], [!UICONTROL MSA Ad Extension Detail Report], [!UICONTROL MSA Network Impression Share Report], [!UICONTROL MSA Network Performance Report] | 지난 180일. |
| | 다른 모든 [!UICONTROL Specialty Reports] | 이전 2개월. |
| [!UICONTROL Model Accuracy Reports] | [!UICONTROL Forecast Accuracy Report] | 지난 18개월. |
| [!UICONTROL Change History Report] | — | 이전 31일. |

>[!MORELIKETHIS]
>
>* [보고서 정보](report-about.md)
>* [보고서에 대한 초기 설정 작업](initial-setup.md)
