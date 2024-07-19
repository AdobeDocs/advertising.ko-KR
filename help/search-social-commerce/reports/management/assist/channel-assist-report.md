---
title: '[!UICONTROL Channel Assist Report]'
description: '[!UICONTROL Channel Assist Report]에 대해 알아봅니다.'
exl-id: 67bce347-2776-4585-adb4-e1a4d76fbadc
feature: Search Reports, Search Assist Reports
source-git-commit: e16bc62127a708de8f4deb1eddfa53a14405cbc2
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 0%

---

# [!UICONTROL Channel Assist Report]

*검색, 소셜 및 Commerce 클릭 추적 및 Adobe Advertising, Adobe Analytics([!DNL Analytics] 통합 포함)의 전환 추적 또는 토큰(`ef_id`)만 사용하여 피드로 제공되는 광고주*

[!UICONTROL Channel Assist Report]은(는) 다양한 마케팅 채널(검색, 소셜 및 Commerce의 검색 또는 소셜, Advertising DSP의 디스플레이 또는 비디오)이 전환 프로세스를 어떻게 지원했는지 나타냅니다. 이 보고서는 하나 이상의 전환으로 이어진 각 이벤트 유형 패턴이 전체 전환에 어떻게 기여했는지 보여 줍니다. 예를 들어, 사용자가 디스플레이 광고 노출을 처음 본 다음 검색 광고를 클릭한 다음 클릭했을 때 발생한 전환 수를 볼 수 있습니다
주문하거나, 사용자가 10개 이상의 광고와 상호 작용한 후 발생한 전환 수를 볼 수 있습니다. 이벤트 유형에는 검색 클릭, 디스플레이 노출 횟수 및 클릭 수, 비디오 노출 횟수 및 클릭 수, 기타 노출 횟수 및 기타 클릭 수가 포함됩니다. <!-- [DSP metrics may show up as "Other Path Length (<length>)" or empty; we're supposed to fill in more values for DSP at some point.] -->

보고서 결과에는 광고주의 [전환 확인 기간](/help/search-social-commerce/glossary.md#c-d) 및 [노출 전환 확인 기간](/help/search-social-commerce/glossary.md#i-j) 내에서 발생한 전환 경로의 각 이벤트 유형(최대 N개의 가장 이른 이벤트 유형)에 대한 집계된 데이터가 포함됩니다. 예를 들어, 경로 크기 5를 선택하는 경우 보고서에는 추적된 이벤트 유형의 각 패턴에 대해 하나의 행이 있는, 가장 이른 이벤트 5개까지 포함된 전환 경로가 포함됩니다(예: &quot;검색 클릭&quot;, &quot;노출 표시&quot;). 각 행에는 경로의 첫 번째 이벤트와 전환을 초래한 마지막 이벤트를 포함한 한 가지 이벤트 패턴이 표시됩니다(마지막 이벤트가 지정된 경로 크기를 벗어난 경우에도). 기본적으로 행은 경로에 있는 이벤트 수만큼 오름차순으로 정렬됩니다.

선택적으로 각 행에 대한 집계 전환 데이터를 포함할 수 있습니다. 보고서에 전환/매출 열을 포함할 때 각 전환 유형은 4개의 열로 표시되어 a) 총 전환 수, b) 해당 이벤트 패턴에 기여한 전체 전환의 백분율, c) 첫 번째 이벤트부터 전환까지의 평균 지연 시간, d) 마지막 이벤트부터 전환까지의 평균 지연 시간(일)을 보여 줍니다. 전환 경로에 지정된 경로 크기보다 많은 이벤트가 포함된 경우 보고서에는 더 많은 이벤트 수(예: 6개의 이벤트 유형을 포함한 모든 패턴)로 인한 전환을 위한 데이터를 집계하는 추가 행이 포함됩니다.

이전 18개월의 데이터를 볼 수 있습니다.

## 사용 가능한 열

다음은 각 보고서에 사용할 수 있는 열입니다. 기본 열은 기본적으로 자동으로 포함됩니다. 보고서 설정의 열 섹션에서 사용 가능한 사용자 정의 열을 추가할 수 있습니다.

| 열 | 기본? | 설명 |
| ---- | ---- | ---- |
| [!UICONTROL 1st Event] - [!UICONTROL 5th Event] | 기본값 | 광고주의 [전환 확인 기간](/help/search-social-commerce/glossary.md#c-d) 및 [노출 확인 기간](/help/search-social-commerce/glossary.md#i-j) 내에서 발생한 전환 경로의 가장 빠른 이벤트 유형 5개. |
| [!UICONTROL Path Size] | 기본값 | 광고주의 [전환 확인 기간](/help/search-social-commerce/glossary.md#c-d) 및 [노출 확인 기간](/help/search-social-commerce/glossary.md#i-j) 내에서 발생한 전환 경로의 이벤트 유형 수입니다. |
| [!UICONTROL First Event Type] | 기본값 | 전환 경로의 첫 번째(가장 이른) 이벤트의 이벤트 유형입니다. |
| [!UICONTROL Last Event Type] | 기본값 | 전환을 초래한 마지막 이벤트의 이벤트 유형(마지막 이벤트가 지정된 경로 크기를 벗어난 경우에도). |
| \[광고주별 사용자 지정(파생) 지표\] | 사용자 정의 | 만든 사용자 지정 지표의 값은 기존 지표에서 계산됩니다. |
| \[광고주별 전환 지표\] | 사용자 정의 | 지정된 전환 지표 또는 사이트 참여 지표에 대한 전환 수입니다. |
| [!UICONTROL % of Total] \[전환 지표\] | 자동 | (보고서 설정에서 사용할 수 없지만 포함된 각 전환 지표에 대해 보고서 출력에 자동으로 포함됨) 이벤트 패턴에 귀속된 포트폴리오 간 전체 전환의 비율입니다. |
| [!UICONTROL 6th Event] - [!UICONTROL 30th Event] | 사용자 정의 | 광고주의 [전환 확인 기간](/help/search-social-commerce/glossary.md#c-d) 및 [노출 전환 확인 기간](/help/search-social-commerce/glossary.md#i-j) 내에서 발생한 전환 경로의 여섯 번째에서 30번째 이벤트 유형입니다. |
| [!UICONTROL Avg. Conv. Latency (First Channel To Conversion)] \[전환 지표\] | 자동 | (보고서 설정에서 사용할 수 없지만 포함된 각 전환 지표에 대해 보고서 출력에 자동으로 포함됨) 첫 번째 이벤트에서 전환까지의 평균 지연 시간(일 수)입니다. |
| [!UICONTROL Avg. Conv. Latency (Last Channel To Conversion)] \[전환 지표\] | 자동 | (보고서 설정에서 사용할 수 없지만 보고서 출력에 자동으로 포함됨) 마지막 이벤트부터 전환까지의 평균 대기 시간(일)입니다. |
| [!UICONTROL Path Frequency] | 사용자 정의 | 이 행의 경로가 전환되기 전에 발생한 횟수입니다. |

>[!MORELIKETHIS]
>
>* [지원 보고서 정보](assist-report-about.md)
>* [[!UICONTROL Campaign Assist Report]](campaign-assist-report.md)
>* [[!UICONTROL Keyword Assist Report]](keyword-assist-report.md)
>* [보고서 설정 지원](assist-report-settings.md)
>* [지원 보고서 생성](assist-report-generate.md)
