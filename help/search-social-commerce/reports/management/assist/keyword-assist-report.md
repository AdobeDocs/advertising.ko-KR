---
title: '[!UICONTROL Keyword Assist Report]'
description: 에 대해 알아보기 [!UICONTROL Keyword Assist Report].
exl-id: 07de2880-111b-498f-9f7f-ec15f89230ae
feature: Search Reports, Search Assist Reports
source-git-commit: f21283731d7a1830af585cec43805c54c81c72ff
workflow-type: tm+mt
source-wordcount: '778'
ht-degree: 0%

---

# 다음 [!UICONTROL Keyword Assist Report]

*검색, 소셜 및 상거래 클릭 추적이 있고 Adobe Advertising, Adobe Analytics에서 전환 추적이 있는 광고주(및 [!DNL Analytics] 통합) 또는 토큰을 사용하여 피드에 제공(`ef_id`) 전용*

다음 [!UICONTROL Keyword Assist Report] 클릭을 유도하는 키워드 또는 배치를 나타냅니다. 이 보고서는 전환 경로에서 클릭을 받은 유료 검색 키워드 또는 배치의 각 패턴을 보여주며 해당 패턴이 전체 전환에 어떻게 기여했는지 보여 줍니다. 예를 들어, 사용자가 처음에 &quot;가죽 신발&quot;에 대한 키워드 검색으로 생성된 광고를 클릭한 다음, &quot;스웨이드 신발&quot;에 대한 키워드 검색 후 광고를 클릭한 다음 주문했을 때 발생한 전환 수를 확인하거나, 사용자가 10개 이상의 키워드로 생성된 광고를 클릭한 후 발생한 전환 수를 확인할 수 있습니다.

보고서 결과에는 광고주의 클릭 전환 확인 및 노출 전환 확인 기간 내에서 발생한 전환 경로의 최대 N개의 초기 유료 검색 키워드 또는 배치 클릭에 대한 집계된 데이터가 포함됩니다. 예를 들어 경로 크기 5개(5)를 선택하는 경우 보고서는 클릭을 받은 최대 5개의 초기 키워드 또는 배치를 포함하는 전환 경로로 구성되며, 추적된 클릭 패턴마다 한 개의 행이 있습니다. 각 행에는 경로에 첫 번째 키워드 또는 배치와 마지막 키워드가 지정된 경로 크기를 벗어난 경우에도 전환을 초래한 마지막 키워드 또는 배치가 포함됩니다. 기본적으로 행은 경로에 있는 이벤트 수만큼 오름차순으로 정렬됩니다.

>[!NOTE]
>
>키워드가 포함되지 않은 콘텐츠 활성화 검색 캠페인의 배치가 보고서에 포함된 경우 [!UICONTROL Keyword] 열에는 &quot;(광고 그룹 컨텐츠) 내 광고 그룹 이름&quot;과 같이 적용 가능한 광고 그룹 이름이 표시됩니다.

선택적으로 각 행에 대한 집계 전환 데이터를 포함할 수 있습니다. 보고서에 전환/매출 열을 포함할 때 각 전환 유형은 4개의 열로 표시되어 a) 총 전환 수, b) 해당 키워드 패턴에 귀속된 전체 전환의 백분율, c) 첫 번째 이벤트(첫 번째 키워드에 대한)에서 전환까지의 평균 지연 시간(일), d) 마지막 이벤트(마지막 키워드에 대한)에서 전환까지의 평균 지연 시간(일)을 보여 줍니다. 전환 경로에 지정된 경로 크기보다 더 많은 키워드가 포함된 경우 보고서에는 더 많은 수의 키워드(예: 6개의 키워드에 대한 클릭을 포함한 모든 패턴)로 인해 전환된 데이터를 집계하는 추가 행이 포함됩니다.

이전 18개월의 데이터를 볼 수 있습니다.

## 사용 가능한 열

다음은 각 보고서에 사용할 수 있는 열입니다. 기본 열은 기본적으로 자동으로 포함됩니다. 보고서 설정의 열 섹션에서 사용 가능한 사용자 정의 열을 추가할 수 있습니다.

| 열 | 기본? | 설명 |
| ---- | ---- | ---- |
| [!UICONTROL 1st Keyword] 끝 [!UICONTROL 5th Keyword] | 기본값 | 광고주 내에서 발생한 전환 경로에서 가장 빠른 5개의 유료 검색 키워드 또는 배치 클릭 [전환 확인 기간 클릭](/help/search-social-commerce/glossary.md#c-d) 및 [노출 전환 확인 기간](/help/search-social-commerce/glossary.md#i-j).<br><br><b>참고:</b> 키워드가 포함되지 않은 콘텐츠 활성화 검색 캠페인의 배치가 보고서에 포함된 경우 이 열에는 대신 &quot;(광고 그룹 콘텐츠) 광고 그룹 이름&quot;과 같은 적용 가능한 광고 그룹 이름이 표시됩니다. |
| [!UICONTROL Path Size] | 기본값 | 광고주 내에서 발생한 전환 경로의 키워드 및/또는 배치 수 [전환 확인 기간 클릭](/help/search-social-commerce/glossary.md#c-d) 및 [노출 전환 확인 기간](/help/search-social-commerce/glossary.md#i-j). |
| [!UICONTROL First Keyword] | 기본값 | 전환 경로의 첫 번째 키워드 또는 배치입니다. |
| [!UICONTROL Last Keyword] | 기본값 | 전환을 초래한 마지막 키워드 또는 배치입니다(마지막 키워드가 지정된 경로 크기를 벗어난 경우에도). |
| \[광고주별 사용자 지정(파생) 지표\] | 사용자 정의 | 만든 사용자 지정 지표의 값은 기존 지표에서 계산됩니다. |
| \[광고주별 전환 지표\] | 사용자 정의 | 지정된 전환 지표 또는 사이트 참여 지표에 대한 전환 수입니다. |
| [!UICONTROL % of Total] \[전환 지표\] | 자동 | (보고서 설정에서 사용할 수 없지만 포함된 각 전환 지표에 대해 보고서 출력에 자동으로 포함됨) 키워드 및/또는 배치 패턴에 귀속된 포트폴리오에서 전체 전환의 비율입니다. |
| [!UICONTROL 6th Keyword] 끝 [!UICONTROL 10th Keyword] | 사용자 정의 | 광고주 내에서 발생한 전환 경로에서 여섯 번째부터 열 번째까지의 유료 검색 키워드 또는 배치 클릭 수 [전환 확인 기간 클릭](/help/search-social-commerce/glossary.md#c-d) 및 [노출 전환 확인 기간](/help/search-social-commerce/glossary.md#i-j).<br><br><b>참고:</b> 키워드가 포함되지 않은 콘텐츠 활성화 검색 캠페인의 배치가 보고서에 포함된 경우 이 열에는 대신 &quot;(광고 그룹 콘텐츠) 광고 그룹 이름&quot;과 같은 적용 가능한 광고 그룹 이름이 표시됩니다. |
| [!UICONTROL Avg. Conv. Latency (First Channel To Conversion)] \[전환 지표\] | 자동 | (보고서 설정에서 사용할 수 없지만 포함된 각 전환 지표에 대해 보고서 출력에 자동으로 포함됨) 첫 번째 이벤트(첫 번째 키워드 또는 배치)에서 전환까지의 평균 대기 시간(일)입니다. |
| [!UICONTROL Avg. Conv. Latency (Last Channel To Conversion)] \[전환 지표\] | 자동 | (보고서 설정에서 사용할 수 없지만 보고서 출력에 자동으로 포함됨) 마지막 이벤트(마지막 키워드 또는 배치)에서 전환까지의 평균 대기 시간(일)입니다. |
| [!UICONTROL Path Frequency] | 사용자 정의 | 이 행의 경로가 전환되기 전에 발생한 횟수입니다. |

>[!MORELIKETHIS]
>
>* [지원 보고서 정보](assist-report-about.md)
>* [다음 [!UICONTROL Campaign Assist Report]](campaign-assist-report.md)
>* [다음 [!UICONTROL Channel Assist Report]](channel-assist-report.md)
>* [보고서 설정 지원](assist-report-settings.md)
>* [지원 보고서 생성](assist-report-generate.md)
