---
title: 기본 및 고급 보고서용 보고서 열
description: 기본 및 고급 보고서에 사용할 수 있는 데이터 열에 대해 알아봅니다.
exl-id: 649cdfa0-e6f2-4881-9f9d-8217e2547d99
feature: Search Reports, Search Basic Reports, Search Advanced Reports
source-git-commit: e517dd5f5fa283ff8a2f57728612937148889732
workflow-type: tm+mt
source-wordcount: '3747'
ht-degree: 0%

---

# 기본 및 고급 보고서용 보고서 열

| 열 | 설명 |
| ---- | ---- |
| \[광고주별 사용자 지정(파생) 지표\] | 에 대한 값 [생성한 사용자 정의 지표](/help/search-social-commerce/common-tasks/custom-metrics/custom-metric-about.md) 기존 지표에서 계산됩니다. |
| \[광고주별 레이블 분류\] | 엔티티 레벨에서 엔티티에 현재 적용된 모든 레이블 분류. 여러 레이블 분류는 쉼표(,)로 구분됩니다. |
| \[광고주별 전환 지표\] | 지정된 전환 지표 또는 사이트 참여 지표에 대한 전환 수입니다. |
| \[Google 추적 전환\] | &quot;GGL\*, GGL_CT\* 및 GGL_XD_CT\*&quot; 항목을 참조하십시오. |
| [!UICONTROL 7-Day Click Accuracy] | ([!UICONTROL Portfolio Report]) 현재 날짜를 포함하지 않고(보고서의 지정된 날짜 범위가 아님) 이전 7일 동안의 클릭 예측 평균 정확도로, 백분율로 표시됩니다. |
| [!UICONTROL 7-Day Cost Accuracy] | ([!UICONTROL Portfolio Report]) 현재 일자를 포함하지 않고(보고서의 지정된 일자 범위가 아님) 이전 7일에 대한 원가 예측의 평균 정확도는 백분율로 표시됩니다. |
| [!UICONTROL 7-Day Revenue Accuracy] | ([!UICONTROL Portfolio Report]) 현재 일자를 포함하지 않고(보고서의 지정된 일자 범위가 아님) 이전 7일 동안의 수익 예측의 평균 정확도는 백분율로 표시됩니다. |
| [!UICONTROL Account] | 계정 이름. |
| [!UICONTROL Account Status] | 검색, 소셜 및 Commerce 내 계정의 상태: <ul><li><i>[!UICONTROL Enabled]:</i> (기본값) 동기화된 광고 네트워크의 경우 검색, 소셜 및 Commerce은 광고 네트워크 계정에 로그인하여 캠페인 데이터를 검색할 수 있으며 최적화 및 추적 생성과 같은 기타 적용 가능한 기능이 활성화됩니다.<br><br>동기화되지 않은 광고 네트워크의 경우 최적화 및/또는 추적 생성과 같은 적용 가능한 기능을 사용할 수 있습니다.</li><li><i>[!UICONTROL Disabled]:</i> 동기화된 광고 네트워크의 경우 검색, 소셜 및 Commerce은 광고 네트워크 계정에 로그인하지 않으므로 캠페인 데이터를 검색하지 않으며 최적화 및 추적 생성과 같은 기타 적용 가능한 기능이 비활성화됩니다. 계정이 활성화된 동안 수집된 데이터는 여전히 저장되지만 나중에 만드는 모든 캠페인 관리 보기 및 모든 보고서에는 계정이 비활성화된 기간에 대한 데이터가 포함되지 않습니다.<br><br>동기화되지 않은 광고 네트워크의 경우 최적화 및/또는 추적 생성과 같은 적용 가능한 기능을 사용할 수 없습니다.</li></ul> |
| [!UICONTROL Active Ad Groups] | 활성 광고 그룹 수입니다. |
| [!UICONTROL Active Ads/Creatives] | 활성 광고/광고 크리에이티브 수. |
| [!UICONTROL Active Campaigns] | 활성 캠페인 수. |
| [!UICONTROL Active Keywords] | 활성 키워드의 수입니다. |
| [!UICONTROL Ad Group] | 광고 그룹. |
| [!UICONTROL Ad Group ID] | Search, Social 및 Commerce이 광고 그룹에 할당하는 숫자 ID입니다. |
| [!UICONTROL Ad Group Status] | 광고 그룹 상태: <i>[!UICONTROL Active]</i>, <i>[!UICONTROL Paused]</i>, 또는 <i>[!UICONTROL Deleted]</i>. |
| [!UICONTROL Ad Group Type] | 다음과 같은 광고 그룹 유형 <i>[!UICONTROL Audience]</i> (대상자 캠페인의 경우), <i>[!UICONTROL Discovery]</i> (검색 캠페인의 경우에만), <i>[!UICONTROL Display]</i> (디스플레이 캠페인만 해당), <i>[!UICONTROL Search Dynamic]</i> (동적 검색 광고만 해당), <i>[!UICONTROL Search Standard]</i> (반응형 검색 광고 및 기존 확장 텍스트 광고만 해당), <i>[!UICONTROL Shopping Showcase]</i>, <i>[!UICONTROL Shopping Product]</i> (표준 쇼핑 캠페인만 해당) 또는 <i>[!UICONTROL Shopping Smart]</i> (스마트 쇼핑 캠페인의 경우). 일부 캠페인 유형의 경우, 단일 캠페인에 여러 광고 유형이 포함될 수 있습니다. |
| [!UICONTROL Ad Groups] | 레이블 값이 할당된 광고 그룹 수입니다. |
| [!UICONTROL AD Name] | 광고 그룹 이름, 와 동일한 값 [!UICONTROL Ad Group]. |
| [!UICONTROL Ad Recall Lift] | ([!DNL Meta] 캠페인 전용) 2일 이내에 광고를 기억하는 예상 사람 수입니다. |
| [!UICONTROL Ad Recall Rate] | ([!DNL Meta] 캠페인 전용) 2일 이내에 광고를 기억하는 예상 사람 수를 도달된 사람 수로 나눈 백분율(%)입니다. |
| [!UICONTROL Ad Size] | 광고 차원. |
| [!UICONTROL AD Strength] | ([!DNL Google Ads] 반응형 검색 광고) 광고의 효과: <i>[!UICONTROL average]</i>, <i>[!UICONTROL excellent]</i>, <i>[!UICONTROL good]</i>, <i>[!UICONTROL no_ads]</i>, <i>[!UICONTROL pending]</i>, <i>[!UICONTROL poor]</i>, <i>[!UICONTROL unknown]</i>, 또는 <i>[!UICONTROL unspecified]</i>. |
| [!UICONTROL Adgroup MBA] | ([!DNL Google Ads], [!DNL Microsoft Advertising], 및 [!DNL Yahoo! Japan Ads] 캠페인) 광고가 모바일 장치에 표시될 때 입찰이 조정되는 방법을 결정하는 현재 광고 그룹 수준의 모바일 입찰 조정입니다. |
| [!UICONTROL Advertiser] | 광고주 이름. |
| [!UICONTROL Advertiser ID] | 광고주의 검색, 소셜 및 Commerce 계정에 대한 숫자 ID입니다. |
| [!UICONTROL Avg Position] | 지정된 날짜 범위 동안의 평균 광고 위치입니다.<br><br>대상 [!DNL Google Ads] 및 [!DNL Yahoo! Japan Ads] 캠페인, 이 데이터는 2019년 9월까지만 사용할 수 있습니다. 대상 [!DNL Microsoft Advertising], 이 데이터는 2021년 1월 22일까지만 사용할 수 있습니다. |
| [!UICONTROL Base URL] | 캠페인이나 계정에 대해 구성된 추가 매개 변수를 포함한 키워드의 기본 URL입니다. 여기에는 검색, 소셜 및 Commerce 리디렉션 및 추적 코드가 포함되지 않습니다. |
| [!UICONTROL Bid Strategy] | (대부분의 광고 네트워크) 캠페인 또는 캠페인 구성 요소의 경우 이것이 캠페인의 입찰 전략입니다. 관리자 계정에 연결된 광고 네트워크 계정의 경우 계정 간 입찰 전략입니다. 사용 가능한 값은 광고 네트워크에 따라 다릅니다. |
| [!UICONTROL Business Name] | ([!DNL Microsoft Advertising] 반응형 광고) 비즈니스 이름입니다. |
| [!UICONTROL Call to Action] | ([!DNL Microsoft Advertising] 반응형 및 멀티미디어 광고) 광고에 포함된 클릭 유도 문안. |
| [!UICONTROL Campaign] | 캠페인. |
| [!UICONTROL Campaign Budget] | 캠페인 예산. |
| [!UICONTROL Campaign MBA] | ([!DNL Google Ads], [!DNL Microsoft Advertising], 및 [!DNL Yahoo! Japan Ads] 캠페인) 광고가 모바일 장치에 표시될 때 입찰이 조정되는 방법을 결정하는 현재 캠페인 수준의 모바일 입찰 조정입니다. |
| [!UICONTROL Campaign Product Scope Filter] | (쇼핑 네트워크만 사용하는 캠페인) 판매자 계정의 제품으로서, 캠페인에 대한 제품 광고를 만들 수 있습니다. |
| [!UICONTROL Campaign Start Date] | 캠페인에 대한 입찰이 수행된/배치된 첫 번째 날입니다. |
| [!UICONTROL Campaign Status] | 캠페인 상태: <i>[!UICONTROL Active]</i>, <i>[!UICONTROL Paused]</i>, <i>[!UICONTROL Ended]</i>, 또는 <i>[!UICONTROL Deleted]</i>. |
| [!UICONTROL Campaign Type] | 캠페인 유형(예: ) <i>[!UICONTROL Audience (Ctv Video)]</i><i>[!UICONTROL Audience (Feed)]</i>, <i>[!UICONTROL Audience (Image)]</i>, <i>[!UICONTROL Audience (Video)]</i>, <i>[!UICONTROL Brand Shopping]</i>, <i>[!UICONTROL Discovery]</i>, <i>[!UICONTROL Search and Display]</i>, <i>[!UICONTROL Standard Display]</i>, <i>[!UICONTROL Standard Performance Max]</i>, <i>[!UICONTROL Standard Search]</i>, <i>[!UICONTROL Standard Shopping]</i>, <i>[!UICONTROL Store Ad]</i>, <i>[!UICONTROL Video]</i>, 또는 <i>[!UICONTROL Others]</i>. |
| [!UICONTROL Channel Type] | 마케팅 채널 유형: <i>[!UICONTROL Search]</i> 또는 <i>[!UICONTROL Content]</i>. 이 열은 보고서에 포함되지 않습니다. [!UICONTROL Search/Content] 보고서 설정의 설정은 &quot;[!UICONTROL Combined].&quot; |
| [!UICONTROL City] | ([!UICONTROL Geo Distribution Report], [!UICONTROL Transaction Report]) 클릭 수가 시작된 도시입니다. 사용자의 IP 주소에서 결정됩니다. |
| [!UICONTROL Click Match Type] | 클릭한 광고에 대한 키워드 일치 유형입니다. 이는 과(와) 동일합니다 [!UICONTROL Listing Match Type] 를 제외하고 [!DNL Microsoft Advertising] 여러 일치 유형이 있는 키워드. 대상 [!DNL Microsoft Advertising] 키워드: 실제로 클릭한 일치 유형입니다. |
| [!UICONTROL Click Value] | ([!UICONTROL Portfolio Report]) 포트폴리오의 목표에 지정된 클릭 값입니다. |
| [!UICONTROL Click/Impression Time] | ([!UICONTROL Transaction Report]) 전환의 원인이 된 클릭 또는 노출이 발생한 시간입니다. |
| [!UICONTROL Clicks] | 지정된 날짜 범위 동안 광고를 클릭한 횟수입니다. |
| [!UICONTROL Client ID1], [!UICONTROL Client Id 1] | ([!UICONTROL Keyword Report], [!UICONTROL Ad Variation Report], 및 [!UICONTROL Transaction Report]; 피드 기반 추적 구현) 피드 파일에서 전송된 키워드 또는 광고에 대한 클라이언트별 추적 ID입니다. |
| [!UICONTROL Client Id 2] | ([!UICONTROL Keyword Report] 및 [!UICONTROL Transaction Report]; 피드 기반 추적 구현) 피드 파일에서 전송된 키워드 또는 광고에 대한 클라이언트별 추적 ID입니다. |
| [!UICONTROL Client Transaction ID] | ([!UICONTROL Transaction Report]) 고유한 거래 ID입니다. |
| [!UICONTROL Constraint End Date] | ([!UICONTROL Constraint Report]) 제한이 활성화된 마지막 날입니다. |
| [!UICONTROL Constraint Name] | ([!UICONTROL Constraint Report]) 제약 조건 이름입니다. |
| [!UICONTROL Constraint Start Date] | ([!UICONTROL Constraint Report]) 제약조건이 활성화된 첫 번째 날입니다. |
| [!UICONTROL Constraint Status] | ([!UICONTROL Constraint Report]) 제약조건의 상태:  <i>[!UICONTROL Active]</i> 또는 <i>[!UICONTROL Paused]</i>. |
| [!UICONTROL Constraint Type] | ([!UICONTROL Constraint Report]) 제한 유형:  <i>[!UICONTROL Bid/Pos Constraint]</i>, <i>[!UICONTROL Bid Shift]</i>, <i>[!UICONTROL Campaign Budget]</i>, <i>[!UICONTROL Context Sensitive Bid]</i>, <i>[!UICONTROL Incremental Bidding]</i>, <i>[!UICONTROL Max CPA]</i>, <i>[!UICONTROL Min Margin]</i>, <i>[!UICONTROL Variable Bid Position]</i>, <i>[!UICONTROL Search Engine Min Bid]</i>, 또는 <i>[!UICONTROL Variable Position]</i>. |
| [!UICONTROL Constraints] | 엔티티에 적용 가능한 모든 제약 조건의 이름으로, 쉼표로 구분됩니다. |
| [!UICONTROL Content IS] | 디스플레이/대상 네트워크의 광고에 대해 받은 노출 횟수를 수신 자격이 있는 예상 노출 횟수로 나눈 값입니다. 위치 [!DNL Microsoft Advertising], 이를 &quot;라고 합니다.[!UICONTROL Audience IS].&quot; |
| [!UICONTROL Content IS Lost (budget)] | 일별 또는 월별 예산이 너무 적어 디스플레이/대상자 네트워크의 광고가 받지 못한 예상 노출 비율입니다. 위치 [!DNL Microsoft Advertising], 이를 &quot;라고 합니다.[!UICONTROL Audience lost IS (budget)].&quot; |
| [!UICONTROL Content IS Lost (rank)] | 광고 등급이 낮아 디스플레이/대상자 네트워크의 광고가 표시되지 않은 예상 노출 비율입니다. 위치 [!DNL Microsoft Advertising], 이를 &quot;라고 합니다.[!UICONTROL Audience lost IS (rank)].&quot; |
| [!UICONTROL Conversion Type] | ([!UICONTROL Transaction Report]) 전환 이전의 작업입니다.<ul><li><i>[!UICONTROL Click:]</i> 전환 전에 최소 한 번의 유료 클릭이 발생했습니다.</li><li><i>[!UICONTROL Impression:]</i> 전환 전에 유료 클릭이 발생하지 않았으므로 전환은 뷰스루(유료 클릭이 없는 노출 횟수)에서 비롯되었습니다.</li></ul> |
| [!UICONTROL Cost] | 지정된 날짜 범위 동안의 광고에 대한 총 비용입니다. |
| [!UICONTROL Country] | ([!UICONTROL Geo Distribution Report], [!UICONTROL Keyword Report]) 클릭이 시작된 국가입니다. 사용자의 IP 주소에서 결정됩니다. |
| [!UICONTROL CPC] | 지정된 날짜 범위 동안의 광고에 대한 클릭당 비용(CPC). |
| [!UICONTROL Creative Base URL] | 캠페인이나 계정에 대해 구성된 추가 매개 변수를 포함한 광고의 기본 URL입니다. 여기에는 검색, 소셜 및 Commerce 리디렉션 및 추적 코드가 포함되지 않습니다. |
| [!UICONTROL Creative Destination URL] | 광고의 최종 URL 또는 대상 URL(추적 매개 변수 포함)입니다. |
| [!UICONTROL Creative Name] | ([!DNL Yahoo! Japan] 만 해당) 광고 이미지 이름입니다. |
| [!UICONTROL Creative Title], [!UICONTROL Creative Title2] - [!UICONTROL Creative Title3] | 광고의 제목 또는 헤드라인입니다. 각 크리에이티브 유형에는 필수 및 선택적 제목 줄 수가 다릅니다. 보려면 [!UICONTROL Creative Title4] 및 의 상위 열 [!DNL Microsoft Advertising] 반응형 광고 또는 멀티미디어 광고, 다음을 포함: &quot;[!UICONTROL Creative Titles]보고서 설정의 &quot;열. |
| [!UICONTROL Creative Titles] | (멀티미디어 및 반응형 검색 광고만 해당) 광고의 짧은 각 헤드라인에 대한 열을 추가합니다(&quot;[!UICONTROL Creative Title]&quot;~&quot;[!UICONTROL Creative Title15]&quot;). 이 열을 포함할 때 다른 열은 포함할 필요가 없습니다 [!UICONTROL Creative Title] 열이지만 [!UICONTROL Order Results/Limit Rows By] 정렬 기준 섹션 [!UICONTROL Creative Titles] 대신 [!UICONTROL Creative Title]. |
| [!UICONTROL Creative Type] | 광고 포맷. 가능한 값은 다음과 같습니다. <i>[!UICONTROL App Install Ad]</i>, <i>[!UICONTROL Call Only Ad]</i>, <i>[!UICONTROL Discovery Ad (single-image ads)]</i>, <i>[!UICONTROL Discovery Carousel Ad]</i> (다중 이미지 회전 광고), <i>[!UICONTROL Display Ad]</i>, <i>[!UICONTROL Dynamic Search Ad]</i>, <i>[!UICONTROL Expanded Dynamic Search Ad]</i>, <i>[!UICONTROL Expanded Text Ad]</i>, <i>[!UICONTROL Legacy Text Ad]</i>, <i>[!UICONTROL Multimedia Ad]</i>, <i>[!UICONTROL Product Ad]</i>, <i>[!UICONTROL Responsive Ad]</i>, <i>[!UICONTROL Responsive Search Ad]</i>, 또는 <i>[!UICONTROL Text Ad]</i>. |
| [!UICONTROL CTR] | 클릭스루 비율(클릭 수를 포함된 광고에 대한 노출 횟수로 나눈 값) |
| [!UICONTROL Currency] | 해당 통화 유형(예: &quot;USD&quot; 또는 &quot;GBP&quot;).<br><br><b>참고:</b> 보고서에 통화가 다른 계정에 대한 데이터가 포함되어 있으면[!UICONTROL Total]&quot;통화 가치는 통화에 관계없이 열에 있는 모든 숫자의 합계입니다. |
| [!UICONTROL Current Bid] | 대상의 현재 입찰입니다. |
| [!UICONTROL Current First Page Bid] | ([!DNL Google Ads] 캠페인만 해당) 광고가 다음 경우에 검색 결과의 첫 페이지에 배치되는 데 현재 필요한 예상 CPC(클릭당 비용) 입찰 [!DNL Google] 검색 쿼리가 키워드와 일치합니다.<br><br>단일 키워드 및 일치 유형 조합의 경우 이 값은 해당 조합에 현재 필요한 첫 번째 페이지 입찰입니다. 동일한 키워드 및 일치 유형 조합이 여러 캠페인에서 사용되는 경우 이 값은 모든 인스턴스에서 현재 필요한 최소 첫 페이지 입찰가입니다. |
| [!UICONTROL Current Quality Score] | ([!DNL Google Ads] 및 [!DNL Microsoft Advertising] 캠페인 전용) 광고 네트워크에서 지정한 키워드 또는 입찰 단위의 현재 품질 점수입니다. 범위는 1(낮음)부터 10(완벽)까지입니다. 단일 키워드 및 일치 유형 조합의 경우 이 값은 해당 조합의 현재 점수입니다. 여러 캠페인에서 동일한 키워드 및 일치 유형 조합을 사용하는 경우 이 값은 모든 인스턴스 중 최대 현재 점수입니다.<br><br>광고 네트워크는 품질 점수를 사용하여 입찰 가격 및 광고 위치를 결정합니다. 관련 광고 및 사용자의 검색 쿼리와 랜딩 페이지의 품질 관련 등 여러 요인에 따라 계산됩니다. 의 키워드용 [!DNL Google Ads], 키워드의 클릭스루 비율 도 고려되며 의 키워드에 대해서도 [!DNL Microsoft Advertising], 랜딩 페이지에서 제공하는 사용자 경험도 고려됩니다. |
| [!UICONTROL Custom Bid Level] | (디스플레이 네트워크만 타겟팅하는 Google 캠페인) 입찰이 적용되는 수준에서: <i>[!UICONTROL Ad Group]</i>, <i>[!UICONTROL Age]</i>, <i>[!UICONTROL Gender]</i>, <i>[!UICONTROL Interest and List]</i>, <i>[!UICONTROL Keyword]</i>, <i>[!UICONTROL Placement]</i>, <i>[!UICONTROL Vertical]</i>, <i>[!UICONTROL None]</i>, 또는 <i>[!UICONTROL Unknown]</i>. |
| [!UICONTROL Description1] - [!UICONTROL Description4] | 광고 본문. 크리에이티브 유형마다 필수 및 선택적 설명 라인의 숫자가 다릅니다. 보려면 [!UICONTROL Description3] 및 [!UICONTROL Description4] 열 위치 [!DNL Microsoft Advertising] 반응형 광고 또는 멀티미디어 광고, 다음을 포함: &quot;[!UICONTROL Descriptions]보고서 설정의 &quot;열. |
| [!UICONTROL Descriptions] | ([!DNL Microsoft Advertising] 반응형 및 멀티미디어 광고) 각 광고의 설명 행에 대해 열을 추가합니다(&quot;[!UICONTROL Description1]&quot;~&quot;[!UICONTROL Description4]&quot;). 이 열을 포함할 때 다른 열은 포함할 필요가 없습니다 [!UICONTROL Description] 열. |
| [!UICONTROL Device] | ([!DNL Google Ads], [!DNL Microsoft Advertising], [!DNL Yahoo! Display Network], [!DNL Yahoo! Japan Ads], 및 [!DNL Yahoo Native] campaigns) 광고가 표시된 디바이스 유형: <i>[!UICONTROL Computers]</i>, <i>[!UICONTROL Mobile]</i>, <i>[!UICONTROL Tablets]</i>, <i>[!UICONTROL Other]</i>, 또는 <i>[!UICONTROL N/A]</i> (값 없음). 다른 광고 네트워크의 행에는 해당 사항 없음 값이 있습니다.<br><br>검색 캠페인에서 키워드, 광고 및/또는 광고 확장에 대한 추적 템플릿 또는 대상 URL에 디바이스별로 데이터를 추적하기 위한 매개 변수가 포함된 경우(`&ev_dvc={device}&ev_dvm={devicemodel}`) 광고를 클릭할 때 전환 데이터도 각 장치 유형의 행에 포함됩니다. 그렇지 않으면 전환 데이터가 디바이스 유형에 귀속될 수 없는 경우 &quot;가 있는 별도의 행에 집계됩니다.[!UICONTROL Device]&quot; 값 [!UICONTROL N/A]. |
| [!UICONTROL Display Path 1] | ([!DNL Google Ads] 확장 텍스트 광고만 해당) 광고의 기본 URL 뒤에 있는 첫 번째 표시 경로입니다. |
| [!UICONTROL Display Path 2] | ([!DNL Google Ads] 확장 텍스트 광고만 해당) 광고의 기본 URL 뒤에 있는 두 번째 표시 경로입니다. |
| [!UICONTROL Display Type] | 사용되지 않음 |
| [!UICONTROL Display URL] | 최종 사용자가 광고에서 보는 광고의 표시 URL입니다. |
| [!UICONTROL DMA] | ([!UICONTROL Geo Distribution Report], [!UICONTROL Keyword Report]) 클릭이 발생한 지정 시장 지역(예: Denver의 경우 751)입니다. 사용자의 IP 주소에서 결정됩니다. |
| [!UICONTROL Domain] | ([!UICONTROL Domain Referral Report], [!UICONTROL Keyword Report]) 클릭이 시작된 도메인 이름입니다. |
| [!UICONTROL eCPM] | 유효 CPM 또는 지정된 날짜 범위 동안 1000회 노출당 지급된 평균 비용입니다. eCPM 값은 CPM 또는 CPC 캠페인에 대해 계산됩니다. |
| [!UICONTROL EF Campaign ID] | Search, Social 및 Commerce이 캠페인에 할당하는 숫자 ID입니다. |
| [!UICONTROL EF ID] | ([!UICONTROL Transaction Report]) (Adobe Advertising 전환 추적 서비스 및 &quot;[!UICONTROL EF Redirect]&quot;토큰을 사용한 추적 메서드) 클릭 또는 전환을 위한 토큰입니다.<ul><li>대상 [!DNL Google Ads] 검색 광고, EF ID: `{gclid}:G:s`: Google 클릭 ID(GCLID) 및 네트워크 유형(&quot;s&quot; for search)이 포함됩니다.</li><li> 대상 [!DNL Microsoft Advertising] 검색 광고, EF ID: `{msclkid}:G:s`: Microsoft 클릭 ID(MSCLKID) 및 네트워크 유형(&quot;s&quot; for search)이 포함됩니다.</li><li>다른 광고 네트워크의 검색 광고의 경우 EF ID에는 서퍼 ID, 클릭 시간 및 네트워크 유형이 포함됩니다.</li><li>디스플레이 광고의 경우 EF ID에는 서퍼 ID, 클릭 또는 노출 시간 및 네트워크 유형이 포함됩니다.</li></ul> |
| [!UICONTROL EF Pixel Location ID] | ([!UICONTROL Geo Distribution Report]; 검색, 소셜 및 Commerce의 경우 만 사용) 데이터를 정규화하는 데 사용되는 지리적 위치에 대한 내부 ID입니다. |
| [!UICONTROL EF Portfolio Group ID] | 포트폴리오가 속한 포트폴리오 그룹의 숫자 ID입니다. |
| [!UICONTROL EF Search Engine ID] | Search, Social 및 Commerce이 광고 네트워크에 할당하는 숫자 ID입니다.  <i>[!UICONTROL 3]</i> 대상 [!DNL Google Ads], <i>[!UICONTROL 10]</i> 대상 [!DNL Microsoft Advertising], <i>[!UICONTROL 45]</i> 대상 [!DNL Meta], <i>[!UICONTROL 86]</i> 대상 [!DNL Yahoo! Display Network], <i>[!UICONTROL 87]</i> 대상 [!DNL Naver], <i>[!UICONTROL 88]</i> 대상 [!DNL Baidu], <i>[!UICONTROL 90]</i> 대상 [!DNL Yandex], <i>[!UICONTROL 94]</i> 대상 [!DNL Yahoo! Japan Ads], <i>[!UICONTROL 105]</i> 대상 [!DNL Yahoo Native] (더 이상 사용되지 않음) 또는 <i>[!UICONTROL 106]</i> 대상 [!DNL Pinterest] (사용하지 않음). |
| [!UICONTROL End Date] | 마지막으로 보고된 날짜입니다. |
| [!UICONTROL Engagement Rate] | (비디오 광고) 참여 수를 광고가 표시된 횟수로 나눈 값입니다. |
| [!UICONTROL Engagements] | (비디오 광고) 사용자가 광고를 10초 이상 시청한 횟수나, 10초 미만인 경우 전체 광고입니다. |
| [!UICONTROL Est. Clicks] | ([!UICONTROL Geo Distribution Report]; 검색 및 디스플레이 캠페인 전용) 광고 그룹/캠페인/포트폴리오 조합에 대한 예상 클릭 수입니다. 이 값은 광고 네트워크에서 제공한 값과 다를 수 있습니다. |
| [!UICONTROL Estimated Cost] | Search, Social 및 Commerce이 추적한 관련 광고의 총 예상 비용입니다. 이 값은 광고 네트워크에서 제공한 값과 다를 수 있습니다. |
| [!UICONTROL Estimated Impressions] | (캠페인만 표시) Search, Social 및 Commerce에서 추적한 예상 광고 노출 횟수입니다. 이 값은 의 값과 다를 수 있습니다. [!UICONTROL Impressions] 광고 네트워크에서 제공한 값을 표시하는 열(사용 가능한 경우). |
| [!UICONTROL Exclude (yes/no)] | 입찰이 제외되는지 여부(<i>[!UICONTROL Yes]</i>) 또는 입찰이 허용됩니다(<i>[!UICONTROL No]</i>)를 클릭하여 제품군에 맞는 광고를 제작할 수 있습니다. |
| [!UICONTROL First Page CPC] | (Google 캠페인만 해당) 지정된 날짜 범위 동안 검색 결과의 첫 페이지에 표시되는 광고의 클릭당 비용(CPC)입니다. |
| [!UICONTROL Frequency] | ([!DNL Meta] campaigns 전용) 누군가 내 광고를 본 평균 횟수입니다. |
| `GGL*`, `GGL_CT*`, 및 `GGL_XD_CT*` [[!DNL Google Ads]-tracked conversions] | ([!DNL Google Ads] 검색 및 쇼핑 네트워크의 캠페인) [!DNL Google Ads]-추적된 전환, 각 전환에 대해 최대 3개의 개별 지표 포함:<ul><li>`GGL*` — (추적할 때) &quot;GGL&quot; 접두사로 시작하는 키워드에 대한 전환 값(예: GGL 구매)입니다.</li><li>`GGL_CT*` — &quot;GGL_CT&quot; 접두사로 시작하는 전환 수(개수)(예: GGL_CT_Purchase)</li><li>`GGL_XD_CT*` — (전환 유형에 사용할 수 있는 경우, 추적할 때) 다음을 기준으로 측정한 교차 장치 전환 수(수)입니다. [!DNL Google Ads] &quot;GGL_XD_CT_&quot; 접두사로 시작(예: GGL_XD_CT_Purchase).</li></ul><br>각 전환은 입찰 단위와 클릭 날짜로 기록되며 이벤트 수준에서 사용할 수 없습니다. 에 대한 자세한 내용 [!DNL Google Ads]-추적된 전환, 참조 &quot;[[!DNL Google Ads] 검색, 소셜 및 상거래의 전환 데이터](/help/search-social-commerce/campaign-management/introduction/google-conversion-data.md).&quot; |
| [!UICONTROL Impr. (Abs. Top) %] | ([!DNL Google Ads] 전용) 유기 검색 결과 위에 첫 번째 광고로 표시되는 광고 노출 비율입니다. |
| [!UICONTROL Impr. (Top) %] | ([!DNL Google Ads] 전용) 유기 검색 결과 위에 표시되는 광고 노출 비율입니다. |
| [!UICONTROL Impressions] | 지정된 날짜 범위 동안의 광고 노출 횟수입니다. |
| [!UICONTROL Interaction Rate] | (비디오 광고) 상호 작용 수를 광고(비디오 및 썸네일 노출) 표시 횟수로 나눈 값입니다. |
| [!UICONTROL Interactions] | (비디오 광고) 사람들이 광고를 시청한 횟수입니다. |
| [!UICONTROL Is_Click_Objectives] | ([!UICONTROL Portfolio Report]) <i>true</i> 포트폴리오에 캠페인이 포함된 경우 [!UICONTROL Maximize Clicks] 입찰 전략 및 <i>false</i> 그렇지 않으면. |
| [!UICONTROL Keyword] | 키워드.<br><br><b>참고:</b> 보고서에 컨텐츠 사용 검색 캠페인의 광고 그룹 데이터가 포함된 경우 이 열에는 &quot;(광고 그룹 컨텐츠) 광고 그룹 이름&quot;과 같은 적용 가능한 광고 그룹 이름이 포함됩니다. 검색 캠페인의 사이트 타겟팅 배치의 경우 이 열에는 값이 없습니다. |
| [!UICONTROL Keyword ID] | Search, Social 및 Commerce이 키워드에 할당하는 숫자 ID입니다. |
| [!UICONTROL Keyword Status] | 검색어가 일치하는 키워드의 상태: <i>[!UICONTROL Active]</i>, <i>[!UICONTROL Paused]</i>, <i>[!UICONTROL Deleted]</i>, 또는 <i>[!UICONTROL Disapproved]</i>. |
| [!UICONTROL Label Classification] | ([!UICONTROL Label Classification Report] 및 [!UICONTROL Label Value Report]) 레이블 분류입니다. |
| [!UICONTROL Label Value] | ([!UICONTROL Label Classification Report] 및 [!UICONTROL Label Value Report]) 레이블 분류에 대한 값입니다. |
| [!UICONTROL Language] | (캠페인 표시) 타겟 대상 언어입니다. |
| [!UICONTROL Link Type] | ([!UICONTROL Keyword Report]; [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 캠페인 전용, 보고서에 지정된 속성 규칙이 &quot;마지막 이벤트&quot;인 경우에만 데이터를 사용할 수 있습니다. 행이 광고 확장(광고 자체가 아님) 또는 제품/쇼핑 광고를 클릭했기 때문에 발생한 전환을 보고할 때 이 열에는 클릭한 링크의 유형 및 제목이 표시됩니다.<ul><li>`pla:*` — 제품 광고가 다음으로 나열됩니다. `pla:<product ID>`, 예: &quot;pla:8525822&quot;</li><li>`sl:*` — 사이트링크가 다음으로 나열됩니다. `sl:<Sitelink text>`( 예: &quot;sl:See Current Offers&quot;)</li></ul> |
| [!UICONTROL Listing Match Type] | 광고 목록에 대한 키워드 일치 유형, <i>[!UICONTROL Content]</i> 콘텐츠 타겟팅 캠페인의 광고용 또는 <i>[!UICONTROL Sitecpc]</i> 를 참조하십시오. 대상 [!DNL Microsoft Advertising] 키워드, 여기에는 여러 일치 유형(예: &quot;[!UICONTROL Broad],[!UICONTROL Exact]&quot;). |
| [!UICONTROL Location] | (캠페인 표시) 타겟 대상자 위치입니다. |
| [!UICONTROL Long Creative Title1] - [!UICONTROL Long Creative Title5] | (다음에 대한 완료된 보고서 행에서) [!DNL Microsoft Advertising] 반응형 및 멀티미디어 광고) 광고의 긴 헤드라인. 이러한 열을 보려면 다음을 포함하십시오. &quot;[!UICONTROL Long Creative Titles]보고서 설정의 &quot;열. |
| [!UICONTROL Long Creative Titles] | (대상 [!DNL Microsoft Advertising] 반응형 및 멀티미디어 광고) 각 광고의 긴 제목(&quot;)에 대해 열을 추가합니다.[!UICONTROL Long Creative Title1]&quot;~&quot;[!UICONTROL Long Creative Title5]&quot;). |
| [!UICONTROL Market Type] | 시장 유형:  <i>[!UICONTROL search]</i> 또는 <i>[!UICONTROL social]</i> |
| [!UICONTROL Max Spend % Target] | (포트폴리오의 캠페인 [!UICONTROL ROI], [!UICONTROL CPT], 또는 [!UICONTROL Marginal Cost per Transaction] 지출 전략) 포트폴리오의 최대 일일 예산 목표입니다. |
| [!UICONTROL Max Spend (%)] | ([!UICONTROL Network Constraint Report]) 광고 네트워크에 대해 구성된 포트폴리오의 최대 지출 비율입니다. 제한 유형 을 사용하는 포트폴리오의 경우 &quot;[!UICONTROL Min-Max],&quot; 이는 [!UICONTROL Max %] 값. 제한 유형 을 사용하는 포트폴리오의 경우 &quot;[!UICONTROL Target Spend],&quot; 이는 [!UICONTROL Target Spend] 값. |
| [!UICONTROL Method ID] | ([!UICONTROL Portfolio Report]) |
| [!UICONTROL Metro Code] | ([!UICONTROL Geo Distribution Report], [!UICONTROL Keyword Report]) 노출 횟수 또는 클릭이 발생한 숫자 메트로 코드(예: Denver의 경우 us-751)입니다. 검색 사용자의 IP 주소에서 결정됩니다. |
| [!UICONTROL Min Spend (%)] | ([!UICONTROL Network Constraint Report]) 광고 네트워크에 대해 구성된 포트폴리오 비용의 최소 비율입니다. 제한 유형 을 사용하는 포트폴리오의 경우 &quot;[!UICONTROL Min-Max],&quot; 이는 [!UICONTROL Min %] 값, 인 경우 [!UICONTROL Min %] 이(가) 구성되었습니다. 제한 유형 을 사용하는 포트폴리오의 경우 &quot;[!UICONTROL Target Spend],&quot; 이는 [!UICONTROL Target Spend] 값. |
| [!UICONTROL Network Account ID] | 네트워크에서 할당한 계정 ID입니다. |
| [!UICONTROL Network Ad Group ID] | 네트워크에서 할당한 광고 그룹 ID입니다. |
| [!UICONTROL Network Campaign ID] | 네트워크에서 할당한 캠페인 ID. |
| [!UICONTROL Network Campaign Objective] | ([!DNL Meta] 캠페인 전용) 캠페인에 대한 목표입니다. |
| [!UICONTROL Objective Name] | 포트폴리오의 목표입니다. |
| [!UICONTROL Objective Value] | 포트폴리오의 현재 목표에 따라 계산된 총 가중 전환입니다. |
| [!UICONTROL Objective Value Calculation] | 목표 값을 도출하는 데 사용되는 계산입니다. |
| [!UICONTROL Outbound Clicks] | ([!DNL Meta] 캠페인 전용) 광고 내에서 사람들을 떼어내는 링크의 클릭 수 [!DNL Meta]소유하는 속성입니다. |
| [!UICONTROL Parent Product Groupings] | 상위 제품 그룹의 전체 계층 구조 `>>` 계층 간(예: `All Products>>CategoryL1=Animals`), 해당되는 경우. |
| [!UICONTROL Partition Type] | 제품 그룹 유형: <i>[!UICONTROL Sub-Division]</i> (상위 제품 그룹) 또는 <i>[!UICONTROL Unit]</i> (입찰이 있는 하위 제품 그룹의 가장 낮은 수준). |
| [!UICONTROL Path Position] | ([!UICONTROL Transaction Report]) 전환 경로 내의 이벤트 위치입니다. |
| [!UICONTROL Path Total] | ([!UICONTROL Transaction Report]) 경로 위치에 대한 총 이벤트 수입니다. |
| [!UICONTROL Portfolio] | 포트폴리오입니다. |
| [!UICONTROL Portfolio Count] | ([!UICONTROL Portfolio Report]) 목표와 연결된 포트폴리오 수입니다. <!-- This count is different than what I see within the Objectives view. --> |
| [!UICONTROL Portfolio Group Name] | 포트폴리오가 속한 포트폴리오 그룹의 이름입니다. |
| [!UICONTROL Portfolio ID] | 숫자 포트폴리오 ID입니다. |
| [!UICONTROL Portfolio Spend Strategy] | ([!UICONTROL Portfolio Report]) 포트폴리오에 대한 지출 전략: <i>[!UICONTROL Daily]</i>, <i>[!UICONTROL Weekly]</i>, <i>[!UICONTROL Monthly]</i>, <i>[!UICONTROL ROI]</i>, <i>[!UICONTROL Day of week]</i>, <i>[!UICONTROL Day of month]</i>, <i>[!UICONTROL CPT]</i>, <i>[!UICONTROL Marginal CPT]</i>, <i>[!UICONTROL Google Target CPA]</i>, 또는 <i>[!UICONTROL Google Target ROAS]</i>. |
| [!UICONTROL Portfolio Status] | 포트폴리오 상태:<ul><li><i>[!UICONTROL Optimize]:</i> 최적화 기능은 관련 캠페인에 대한 클릭 및 매출 데이터를 수집하고, 데이터를 모델링하여 입찰을 최적화하며, 입찰 및/또는 캠페인 예산(최적화 유형 및 캠페인 입찰 전략에 따라)을 최적화하는 것입니다.</li><li><i>[!UICONTROL Active]:</i> 최적화 기능은 관련 캠페인에 대한 클릭 및 매출 데이터를 수집하고 데이터를 모델링하지만 입찰이나 캠페인 예산을 최적화하지 않습니다.</li><li><i>[!UICONTROL Inactive]:</i> 최적화 기능은 보고 목적으로 관련 캠페인에 대한 클릭 데이터를 수집하는 것이지만, 데이터를 모델링하거나 입찰 또는 캠페인 예산을 최적화하지 않습니다.</li></ul> |
| [!UICONTROL Portfolio Target] | ([!UICONTROL Portfolio Report]) 포트폴리오의 비용 전략에 대한 일별 대상입니다. 일별/월별 및 요일/월 전략의 경우 현재 날짜의 대상이 표시됩니다. |
| [!UICONTROL Preferred Devices] | ([!DNL Google Ads], [!DNL Microsoft Advertising], 및 [!DNL Yahoo! Japan Ads] 캠페인) 광고 설정에서 환경 설정을 <i>[!UICONTROL Mobile ads]</i> 또는 종료 <i>[!UICONTROL All ads]</i>. |
| [!UICONTROL Product Group ID] | 광고 네트워크가 제품 그룹에 할당하는 숫자 ID입니다. |
| [!UICONTROL Product Group Name] | 제품 그룹의 이름입니다. |
| [!UICONTROL Product Group Status] | 제품 그룹의 상태입니다. |
| [!UICONTROL Product Groupings] | 상위 제품 그룹. |
| [!UICONTROL Product ID] | ([!UICONTROL Keyword Report]; [!DNL Google Ads] 제품 목록 광고) 광고에 표시된 제품의 제품 ID입니다.<br><br><b>참고:</b> ID는 제품 목록에 추적 매개 변수가 포함된 경우에만 캡처됩니다 `ev_plx=<GMC product ID>`: 내에 추가해야 합니다. [!DNL Google Merchant Center]. |
| [!UICONTROL Raw Transaction Data] | ([!UICONTROL Transaction Report]) 전환 지표 매출(예: 한 개 등록의 경우 1, 12 USD 주문의 경우 12)입니다. 여러 입찰 단위에 동일한 거래 ID가 있는 경우 추적 ID의 매출은 지정된 클릭 날짜(클릭 데이터를 사용할 수 있을 때)의 클릭 수에 따라 분할됩니다. |
| [!UICONTROL Reach] | ([!DNL Meta] 캠페인 전용) 광고를 한 번 이상 본 사람 수입니다. 참고: [!DNL Meta] 중복 제거는 매일 사용자 프로필에 도달하므로 다음에서 보고하는 숫자에 해당합니다. [!DNL Meta] 그리고 검색별로 소셜 및 Commerce이 다를 수 있습니다. |
| [!UICONTROL Region] | ([!UICONTROL Geo Distribution Report], [!UICONTROL Keyword Report]) 노출 또는 클릭이 시작된 지역 또는 미국/캐나다 주입니다. 사용자의 IP 주소에서 결정됩니다. |
| [!UICONTROL SE Creative ID] | 네트워크에서 할당한 광고 ID입니다. |
| [!UICONTROL Search (Abs. Top) IS] | ([!DNL Google Ads] 및 [!DNL Microsoft Advertising]) 절대 상단 위치(유기 검색 결과 위의 첫 번째 광고)에서 받은 노출 횟수를 상단 위치에서 받을 수 있는 예상 노출 횟수로 나눈 값입니다. 10% 미만의 백분율은 &quot;로 표시됩니다.`<10%`&quot; 또는 &quot;`0.0999`.&quot; |
| [!UICONTROL Search (Top) IS] | ([!DNL Google Ads] 및 [!DNL Microsoft Advertising]) 상위 위치(유기 검색 결과 위)에서 받은 노출 횟수를 상위 위치에서 받을 수 있는 예상 노출 횟수로 나눈 값입니다. 10% 미만의 백분율은 &quot;로 표시됩니다.`<10%`&quot; 또는 &quot;`0.0999`.&quot; |
| [!UICONTROL Search Engine] | 광고 네트워크입니다. |
| [!UICONTROL Search exact match IS] | 키워드와 정확히 일치하는 검색에 대해 받은 노출 수를 수신 자격이 있는 예상 정확한 일치 노출 수로 나눈 값입니다. 이 수치가 낮으면 입찰가가 너무 낮거나 광고 품질이나 관련성이 낮기 때문일 수 있습니다. |
| [!UICONTROL Search impr. share] | ([!DNL Google Ads] 만 해당) 받은 노출 수를 받을 수 있는 예상 노출 수로 나눈 값입니다. 10% 미만의 백분율은 &quot;&lt;10%&quot;로 표시되며, 90% 이상의 백분율은 &quot;로 표시됩니다.`>90%`.&quot; |
| [!UICONTROL Search lost abs. top IS (budget)] | ([!DNL Google Ads] 및 [!DNL Microsoft Advertising]) 일별 또는 월별 예산이 너무 낮기 때문에 광고가 유기 검색 결과보다 첫 번째 광고가 아닌 시간의 백분율입니다. Google 광고 캠페인의 경우 90%가 넘는 백분율이 &quot;`>90%`&quot; 또는 &quot;`0.9001`.&quot; |
| [!UICONTROL Search lost abs. top IS (rank)] | ([!DNL Google Ads] 및 [!DNL Microsoft Advertising]) 광고 등급이 낮기 때문에 광고가 유기 검색 결과보다 높은 첫 번째 광고가 아닌 시간의 백분율입니다. Google 광고 캠페인의 경우 90%가 넘는 백분율이 &quot;`>90%`&quot; 또는 &quot;`0.9001`.&quot; |
| [!UICONTROL Search lost IS (budget)] | ([!DNL Google Ads] 만 해당) 일별 또는 월별 예산이 너무 낮아서 광고가 표시되지 않은 시간의 백분율입니다. 이 지표는 캠페인 수준에서만 사용할 수 있습니다. 90%가 넘는 백분율은 &quot;로 표시됩니다.`>90%`&quot; 또는 &quot;`0.9001`.&quot; |
| [!UICONTROL Search lost IS (rank)] | ([!DNL Google Ads] 전용) 광고 등급이 낮아 광고가 표시되지 않은 시간의 백분율입니다. 90%가 넘는 백분율은 &quot;로 표시됩니다.`>90%`&quot; 또는 &quot;`0.9001`.&quot; |
| [!UICONTROL Search lost top IS (budget)] | ([!DNL Google Ads] 및 [!DNL Microsoft Advertising]) 일별 또는 월별 예산이 너무 낮아서 광고가 유기 검색 결과 위에 표시되지 않은 시간의 백분율입니다. 대상 [!DNL Google Ads] 캠페인, 90% 이상의 백분율이 &quot;로 표시됩니다.`>90%`&quot; 또는 &quot;`0.9001`.&quot; |
| [!UICONTROL Search lost top IS (rank)] | ([!DNL Google Ads] 및 [!DNL [!DNL Microsoft Advertising]]) 광고 순위가 낮기 때문에 광고가 유기 검색 결과 위에 표시되지 않은 시간의 백분율입니다. Google 광고 캠페인의 경우 90%가 넘는 백분율이 &quot;`>90%`&quot; 또는 &quot;`0.9001`.&quot; |
| [!UICONTROL Search Term] | ([!UICONTROL Transaction Report]) 사용자가 쿼리하는 검색어입니다. |
| [!UICONTROL SETrackingOnly] | 계정을 추적하지만 입찰은 하지 않는지 여부: <i>[!UICONTROL TRUE]</i> 또는 <i>[!UICONTROL FALSE]</i>. |
| [!UICONTROL Site] | (도메인 조회 보고서 및 [!UICONTROL Keyword Report]; 사이트 타겟 배치) 클릭이 시작된 사이트입니다. |
| [!UICONTROL Start Date] | 보고된 첫 번째 날. |
| [!UICONTROL State] | (지역 배포 보고서, [!UICONTROL Keyword Report]) 트랜잭션이 시작된 상태입니다. 사용자의 IP 주소에서 결정됩니다. |
| [!UICONTROL Surfer ID] | ([!UICONTROL Transaction Report]) 트랜잭션을 완료한 사용자의 ID입니다. |
| [!UICONTROL Thru Plays] | ([!DNL Meta] 캠페인 전용) 광고 전체를 시청한 보기 수입니다. |
| [!UICONTROL Top of Page CPC] | (Google 캠페인만 해당) 지정된 날짜 범위 동안 검색 결과 페이지의 맨 위에 표시되는 광고의 클릭당 비용(CPC)입니다. |
| [!UICONTROL Tracking URL] | (검색 대상 키워드만 해당) 추적 템플릿 또는 검색, 소셜 및 Commerce 추적 코드에 포함된 대상 URL(해당되는 경우)입니다. |
| [!UICONTROL Transaction Property Name] | ([!UICONTROL Transaction Report]) 트랜잭션이 크레딧되는 광고주별 전환 지표입니다. |
| [!UICONTROL Transaction Time] | ([!UICONTROL Transaction Report]) 지정된 전환 지표가 차감된 시간입니다. |
| [!UICONTROL Two Second Continuous Video Plays] | ([!DNL Meta] 캠페인 전용) 비디오가 2초 이상 연속으로 재생된 횟수입니다. |
| [!UICONTROL User Account Type] | 사용되지 않음 |
| [!UICONTROL User SE Account ID] | Search, Social 및 Commerce이 광고 네트워크에 할당하는 숫자 ID입니다. |
| [!UICONTROL Video Average Play Time] | ([!DNL Meta] 캠페인 전용) 단일 노출에 대해 비디오가 재생된 평균 시간(비디오 재생 시간 포함). |
| [!UICONTROL Video Plays] | ([!DNL Meta] 캠페인만 해당) 비디오가 재생되기 시작하는 횟수입니다. 재생 횟수는 제외됩니다. |
| [!UICONTROL Video Played at 25 Percent Count], [!UICONTROL Video Played at 50 Percent Count], [!UICONTROL Video Played at 75 Percent Count], 및 [!UICONTROL Video Played at 100 Percent Count] | (비디오 광고) 끝까지 재생되는 비디오의 횟수는 25%, 50%, 75% 또는 100%입니다. |
| [!UICONTROL VideoQuartile25Rate], [!UICONTROL VideoQuartile50Rate], [!UICONTROL VideoQuartile75Rate], 및 [!UICONTROL VideoQuartile100Rate] | (비디오 광고) 끝까지 재생되는 비디오의 25%, 50%, 75% 또는 100%의 비율입니다. |
| [!UICONTROL View Rate] | (비디오 광고) 보기 또는 참여 수를 광고(비디오 및 썸네일 노출) 표시 횟수로 나눈 값입니다. |
| [!UICONTROL Views] | (비디오 광고) 사람들이 광고를 시청하거나 광고에 참여한 횟수입니다. |
| [!UICONTROL ViewThroughConversions] | (대상 네트워크의 광고) 하나 이상의 노출로 인한 전환 횟수지만 클릭은 없습니다. |

<!-- HOW IS MARKET TYPE DIFFERENT FROM CHANNEL TYPE? And what are all possible values for each? -->

>[!MORELIKETHIS]
>
>* [기본 및 고급 보고서 정보](/help/search-social-commerce/reports/management/basic-advanced/basic-advanced-report-about.md)
>* [기본 또는 고급 보고서 생성](/help/search-social-commerce/reports/management/basic-advanced/basic-advanced-report-generate.md)
>* [기본 및 고급 보고서 설정](/help/search-social-commerce/reports/management/basic-advanced/basic-advanced-report-settings.md)
