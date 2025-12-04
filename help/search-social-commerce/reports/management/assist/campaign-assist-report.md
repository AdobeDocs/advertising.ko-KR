---
title: '[!UICONTROL Campaign Assist Report]'
description: '[!UICONTROL Campaign Assist Report]에 대해 알아봅니다.'
exl-id: c89b4c9f-16d5-4e1a-a73f-6cc99dd3f526
feature: Search Reports, Search Assist Reports
source-git-commit: 7a87d3c3827125adb97f50986823568c9aef8c24
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 1%

---

# [!UICONTROL Campaign Assist Report]

*검색, 소셜 및 Commerce 클릭 추적 및 Adobe Advertising, Adobe Analytics([!DNL Analytics] 통합 포함)의 전환 추적을 사용하거나 토큰(`ef_id`)만 사용하여 피드에 제공된 광고주*

[!UICONTROL Campaign Assist Report]은(는) 전환 프로세스를 지원한 캠페인을 나타냅니다. 하나 이상의 전환으로 이어지는 광고의 각 캠페인 패턴이 전체 전환에 기여한 방식을 보고합니다. 예를 들어 사용자가 캠페인 A에서 광고를 처음 본 다음 캠페인 B에서 광고를 클릭한 다음 주문했을 때 발생한 전환 수를 볼 수 있습니다. 마찬가지로 사용자가 10개 이상의 캠페인의 광고와 상호 작용한 후 발생한 전환 수를 확인할 수 있습니다.

보고서 결과에는 광고주의 [전환 확인 기간](/help/search-social-commerce/glossary.md#c-d) 및 [노출 전환 확인 기간](/help/search-social-commerce/glossary.md#i-j) 내에서 발생한 이벤트에 대해 전환 경로의 각 캠페인 패턴(최대 N개 초기 캠페인)에 대해 집계된 데이터가 포함됩니다. 예를 들어, 경로 크기 5를 선택하면 보고서에는 가장 이른 캠페인 5개까지 포함한 전환 경로가 포함되며, 이벤트가 추적된 캠페인 패턴마다 하나의 행이 있습니다. 각 행에는 경로의 첫 번째 캠페인과 전환을 초래한 마지막 캠페인을 포함하여 한 가지 캠페인 패턴이 표시됩니다(마지막 캠페인이 지정된 경로 크기를 벗어난 경우에도). 기본적으로 행은 경로에 있는 캠페인 수만큼 오름차순으로 정렬됩니다.

각 행에 대해 선택적으로 사용자 지정 지표를 포함한 집계 전환 데이터를 포함할 수 있습니다. 보고서에 전환/매출 열을 포함할 때 각 전환 유형은 4개의 열로 표시되어 a) 총 전환 수, b) 해당 캠페인 패턴에 기여한 전체 전환의 백분율, c) 첫 번째 이벤트(첫 번째 캠페인에서)에서 전환까지의 평균 지연 시간(일), d) 마지막 이벤트(마지막 캠페인에서)에서 전환까지의 평균 지연 시간(일)을 보여줍니다. 전환 경로에 지정된 경로 크기보다 많은 캠페인이 포함된 경우 보고서에는 캠페인 수가 많을수록 전환을 위한 데이터를 집계하는 추가 행(예: 6개 캠페인을 포함한 모든 패턴)이 포함됩니다.

캠페인 이름 뒤에 광고 네트워크 및/또는 이벤트 유형을 포함할 수도 있습니다(예: `<campaign name> (Google) click`).

이전 18개월의 데이터를 볼 수 있습니다.

>[!TIP]
>
>브랜드 키워드가 일반 키워드와 다른 캠페인에 있는 경우 보고서는 브랜드 키워드가 전환에 기여하는지 여부를 나타냅니다.

## 사용 가능한 열

다음은 각 보고서에 사용할 수 있는 열입니다. 기본 열은 기본적으로 자동으로 포함됩니다. 보고서 설정의 열 섹션에서 사용 가능한 사용자 정의 열을 추가할 수 있습니다.

| 열 | 기본? | 설명 |
| ---- | ---- | ---- |
| [!UICONTROL 1st Campaign] - [!UICONTROL 5th Campaign] | 기본값 | 광고주의 [전환 확인 기간](/help/search-social-commerce/glossary.md#c-d) 및 [노출 전환 확인 기간](/help/search-social-commerce/glossary.md#i-j) 내에서 발생한 전환 경로의 가장 빠른 캠페인 5개.<br><br>엔터티 이름 뒤에 광고 네트워크, 계정 이름 또는 이벤트 유형을 나타내는 보고서 옵션을 포함한 경우 해당 정보가 캠페인 이름 뒤에 포함됩니다(예: `"<"campaign name> [Google] [Account1] [impression]`&quot;). |
| [!UICONTROL Path Size] | 기본값 | 광고주의 [전환 확인 기간](/help/search-social-commerce/glossary.md#c-d) 및 [노출 확인 기간](/help/search-social-commerce/glossary.md#i-j) 내에서 발생한 전환 경로의 캠페인 수입니다. |
| [!UICONTROL First Campaign] | 기본값 | 전환 경로의 첫 번째 캠페인. |
| [!UICONTROL Last Campaign] | 기본값 | 전환을 초래한 마지막 캠페인(마지막 키워드가 지정된 경로 크기를 벗어난 경우에도).<br><br>엔터티 이름 뒤에 광고 네트워크, 계정 이름 또는 이벤트 유형을 나타내는 보고서 옵션을 포함한 경우 해당 정보가 캠페인 이름 뒤에 포함됩니다(예: `"<"campaign name> [Google] [Account1] [impression]`&quot;). |
| \[광고주별 사용자 지정(파생) 지표\] | 사용자 정의 | 생성한 사용자 지정 지표의 값은 기존 지표에서 계산됩니다. |
| \[광고주별 전환 지표\] | 사용자 정의 | 지정된 전환 지표 또는 사이트 참여 지표에 대한 전환 수입니다. |
| [!UICONTROL % of Total] \[전환 지표\] | 자동 | (보고서 설정에서 사용할 수 없지만 포함된 각 전환 지표에 대해 보고서 출력에 자동으로 포함됨) 캠페인 패턴에서 발생한 지정된 전환 지표에 대한 전환 수입니다. |
| [!UICONTROL 6th Campaign] - [!UICONTROL 20th Campaign] | 사용자 정의 | 광고주의 [전환 확인 기간](/help/search-social-commerce/glossary.md#c-d) 및 [노출 전환 확인 기간](/help/search-social-commerce/glossary.md#i-j) 내에서 발생한 전환 경로의 여섯 번째~20번째 캠페인입니다.<br><br>엔터티 이름 뒤에 광고 네트워크, 계정 이름 또는 이벤트 유형을 나타내는 보고서 옵션을 포함한 경우 해당 정보가 캠페인 이름 뒤에 포함됩니다(예: `"<"campaign name> [Baidu] [Account1] [click]`&quot;). |
| [!UICONTROL Avg. Conv. Latency (First Campaign To Conversion)] \[전환 지표\] | 자동 | (보고서 설정에서 사용할 수 없지만 포함된 각 전환 지표에 대해 보고서 출력에 자동으로 포함됨) 첫 번째 이벤트(첫 번째 캠페인)에서 전환까지의 평균 지연 시간(일)입니다. |
| [!UICONTROL Avg. Conv. Latency (Last Campaign To Conversion)] \[전환 지표\] | 자동 | (보고서 설정에서 사용할 수 없지만 보고서 출력에 자동으로 포함됨) 마지막 이벤트(마지막 캠페인)에서 전환까지의 평균 대기 시간(일)입니다. |
| [!UICONTROL EF Campaign ID] | 사용자 정의 | Search, Social 및 Commerce이 캠페인에 할당하는 숫자 ID입니다. |
| [!UICONTROL EF Portfolio Group ID] | 사용자 정의 | 포트폴리오가 속한 포트폴리오 그룹의 숫자 ID입니다. |
| [!UICONTROL EF Search Engine ID] | 사용자 정의 | Search, Social 및 Commerce이 광고 네트워크에 할당하는 숫자 ID입니다. <i>[!UICONTROL 3]</i>의 [!DNL Google Ads], <i>[!UICONTROL 10]</i>의 [!DNL Microsoft Advertising], <i>[!UICONTROL 45]</i>의 [!DNL Meta], <i>[!UICONTROL 86]</i>의 [!DNL Yahoo! Display Network], <i>[!UICONTROL 87]</i>의 [!DNL Naver], <i>[!UICONTROL 88]</i>의 [!DNL Baidu], <i>[!UICONTROL 90]</i>의 [!DNL Yandex], <i>[!UICONTROL 94]</i>의 [!DNL Yahoo! Japan Ads], <i>[!UICONTROL 105]</i>의 [!DNL Yahoo Native]&#x200B;(더 이상 사용되지 않음) 또는 <i>[!UICONTROL 106]</i>의 [!DNL Pinterest]&#x200B;(더 이상 사용되지 않음). |
| [!UICONTROL Portfolio ID] | 사용자 정의 | 숫자 포트폴리오 ID입니다. |
| [!UICONTROL User SE Account ID] | 사용자 정의 | Search, Social 및 Commerce이 광고 네트워크에 할당하는 숫자 ID입니다. |

>[!MORELIKETHIS]
>
>* [지원 보고서 정보](assist-report-about.md)
>* [[!UICONTROL Channel Assist Report]](channel-assist-report.md)
>* [[!UICONTROL Keyword Assist Report]](keyword-assist-report.md)
>* [보고서 설정 지원](assist-report-settings.md)
>* [지원 보고서 생성](assist-report-generate.md)
