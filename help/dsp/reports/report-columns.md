---
title: 사용 가능한 보고서 열
description: 사용자 지정 보고서에서 사용 가능한 열에 대한 설명을 참조하십시오.
feature: DSP Custom Reports
exl-id: 6dc30603-8a45-4188-aca6-591f3422b74a
source-git-commit: 7b7e9687bf79fce564103606efbe8c5997d3c05c
workflow-type: tm+mt
source-wordcount: '2413'
ht-degree: 0%

---

# 사용 가능한 보고서 열

<!-- Add when added:

|[!UICONTROL Dimension]|[!UICONTROL Feed]|[!UICONTROL Deal List]|The name of a user-created deal list for which an ad was shown.|

-->

| 지표 유형 | 하위 유형 | 열 이름 | 설명 |
|-----------|-------|-----------|-----------|
| [!UICONTROL Dimension] | [!UICONTROL Ad] | [!UICONTROL Ad External ID] | 외부 광고 서버에서 할당한 광고 ID입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Ad] | [!UICONTROL Ad ID] | DSP의 광고에 대한 고유 식별자. |
| [!UICONTROL Dimension] | [!UICONTROL Ad] | [!UICONTROL Ad Name] | 사용자가 할당한 광고 이름. |
| [!UICONTROL Dimension] | [!UICONTROL Ad] | [!UICONTROL Ad Type] | 광고 형식입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Ad] | [!UICONTROL Status] | 사용자가 변경하거나 날짜 입력으로 표시한 광고 분류: *[!UICONTROL live]*, *[!UICONTROL scheduled]*, *[!UICONTROL completed]* 또는 *[!UICONTROL archived]*. |
| [!UICONTROL Dimension] | [!UICONTROL Advertiser] | [!UICONTROL Advertiser Name] | 광고주의 이름입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Campaign] | [!UICONTROL Budget] | 캠페인에 대해 사용자가 할당한 총 예산. |
| [!UICONTROL Dimension] | [!UICONTROL Campaign] | [!UICONTROL Campaign End Date] | 캠페인 종료일. |
| [!UICONTROL Dimension] | [!UICONTROL Campaign] | [!UICONTROL Campaign ID] | DSP의 Campaign 고유 식별자입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Campaign] | [!UICONTROL Campaign Name] | 사용자가 할당한 캠페인의 이름입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Campaign] | [!UICONTROL Campaign Start Date] | 캠페인의 첫 번째 날짜입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Content] | [!UICONTROL Title] | 콘텐츠/영화 제목. |
| [!UICONTROL Dimension] | [!UICONTROL Content] | [!UICONTROL Series] | 콘텐츠 시리즈. |
| [!UICONTROL Dimension] | [!UICONTROL Content] | [!UICONTROL Genre] | 콘텐츠 장르. |
| [!UICONTROL Dimension] | [!UICONTROL Content] | [!UICONTROL ProdQ] | [IAB 기술 연구소](https://github.com/InteractiveAdvertisingBureau/AdCOM/blob/main/AdCOM%20v1.0%20FINAL.md)에서 정의한 프로덕션 품질입니다. 값은 `Unknown`, `Professionally Produced`, `Prosumer` 또는 `User Generated`일 수 있습니다. |
| [!UICONTROL Dimension] | [!UICONTROL Content] | [!UICONTROL Context] | [IAB 기술 연구소](https://github.com/InteractiveAdvertisingBureau/AdCOM/blob/main/AdCOM%20v1.0%20FINAL.md)에서 정의한 콘텐츠 유형입니다. 값에는 `Video,` `Game`, `Music`, `Application`, `Text`, `Other` 또는 `Unknown`이(가) 포함될 수 있습니다. |
| [!UICONTROL Dimension] | [!UICONTROL Content] | [!UICONTROL Content Rating] | 콘텐츠 등급(예: PG 또는 R). |
| [!UICONTROL Dimension] | [!UICONTROL Content] | [!UICONTROL Livestream] | 광고가 실시간 스트림에 표시되었는지 여부: `Not Live` 또는 `Live`. |
| [!UICONTROL Dimension] | [!UICONTROL Content] | [!UICONTROL Content Length (in seconds)] | 콘텐츠의 길이(초)입니다. 일반적으로 비디오나 오디오에 사용됩니다. |
| [!UICONTROL Dimension] | [!UICONTROL Content] | [!UICONTROL Language (as per ISO 639)] | ISO-639-1-alpha-2를 사용하는 콘텐츠의 언어입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Date/Time] | [!UICONTROL Day (YYYY-MM-DD)] | 연도, 월, 일입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Date/Time] | [!UICONTROL of Week]일 | 특정 날짜(예: [!UICONTROL Monday] 또는 [!UICONTROL Tuesday]). |
| [!UICONTROL Dimension] | [!UICONTROL Date/Time] | [!UICONTROL Hour (YYYY-MM-DD HH)] | 연도, 월, 일 및 시간. |
| [!UICONTROL Dimension] | [!UICONTROL Date/Time] | [!UICONTROL Month (YYYY-MM)] | 월 및 연도. |
| [!UICONTROL Dimension] | [!UICONTROL Date/Time] | [!UICONTROL Time of Day] | 0-23 사이의 시간입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Date/Time] | [!UICONTROL Week (YYYY-MM-DD to YYYY-MM-DD)] | 해당 주의 날짜 범위(일요일부터 토요일까지). 예: 2021-02-18 ~ 2021-03-07. |
| [!UICONTROL Dimension] | [!UICONTROL Device] | [!UICONTROL Browser Vendor] | 광고가 표시된 브라우저의 공급업체(예: Google 또는 Mozilla). |
| [!UICONTROL Dimension] | [!UICONTROL Device] | [!UICONTROL Browser Version] | 광고가 표시된 브라우저의 버전입니다(예: [!UICONTROL Safari 4.3] 또는 [!UICONTROL Chrome 7.0]). |
| [!UICONTROL Dimension] | [!UICONTROL Device] | [!UICONTROL Browser] | 광고가 표시된 브라우저(예: [!UICONTROL Chrome] 또는 [!UICONTROL Firefox]). |
| [!UICONTROL Dimension] | [!UICONTROL Device] | [!UICONTROL Environment] | 광고가 *[!UICONTROL sites]*&#x200B;에 표시되었는지 아니면 *[!UICONTROL Apps]*&#x200B;에 표시되었는지 여부입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Device] | [!UICONTROL Hardware] | 광고가 표시된 디바이스 유형(예: [!UICONTROL Set Top Box] 또는 [!UICONTROL Mobile Phone]). |
| [!UICONTROL Dimension] | [!UICONTROL Device] | [!UICONTROL Manufacturer] | 광고가 표시된 장치의 제조업체(예: [!UICONTROL Samsung], [!UICONTROL Lenovo] 또는 [!UICONTROL Apple]). |
| [!UICONTROL Dimension] | [!UICONTROL Device] | [!UICONTROL Model] | 광고가 표시된 장치의 모델입니다(예: [!UICONTROL iPhone XS] 또는 [!UICONTROL Galaxy Note 7]). |
| [!UICONTROL Dimension] | [!UICONTROL Device] | [!UICONTROL Operating System Vendor] | 광고가 표시된 운영 체제의 공급업체(예: [!UICONTROL Microsoft] 또는 [!UICONTROL Apple]). |
| [!UICONTROL Dimension] | [!UICONTROL Device] | [!UICONTROL Operating System Version] | 광고가 표시된 운영 체제의 버전(예: [!UICONTROL Windows 10] 또는 [!UICONTROL iOS Mojave]) |
| [!UICONTROL Dimension] | [!UICONTROL Device] | [!UICONTROL Operating System] | 광고가 표시된 운영 체제(예: [!UICONTROL Apple iOS] 또는 [!UICONTROL Android]). |
| [!UICONTROL Dimension] | [!UICONTROL Feed] | [!UICONTROL Deal Name] | DSP에 입력된 거래에 대해 사용자가 할당한 이름. |
| [!UICONTROL Dimension] | [!UICONTROL Feed] | [!UICONTROL Deal Type] | 거래가 *[!UICONTROL Guaranteed]*&#x200B;인지 *[!UICONTROL Non-Guaranteed]*&#x200B;인지 여부. |
| [!UICONTROL Dimension] | [!UICONTROL Feed] | [!UICONTROL Inventory Type] | 인벤토리 분류: *[!UICONTROL Private],* *[!UICONTROL On Demand],* 또는 *[!UICONTROL Public]*. |
| [!UICONTROL Dimension] | [!UICONTROL Feed] | [!UICONTROL Private Deal ID] | 외부 공급 파트너를 통해 비공개 거래에 할당된 고유 식별자. |
| [!UICONTROL Dimension] | [!UICONTROL Feed] | [!UICONTROL Publisher] | 재고를 제공하는 공급측 파트너. 이는 일반적으로 게시자이지만 SSP일 수도 있습니다. |
| [!UICONTROL Dimension] | [!UICONTROL Feed] | [!UICONTROL SSP] | 미디어가 속하는 SSP(공급측 파트너)입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Frequency] | [!UICONTROL Frequency] | 장치가 고유 쿠키 또는 장치 ID를 기반으로 한 광고를 받은 횟수입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Geos] | [!UICONTROL City] | 보고된 데이터가 속하는 도시입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Geos] | [!UICONTROL Country] | 보고된 데이터가 속하는 국가입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Geos] | [!UICONTROL DMA] | 보고된 데이터가 속하는 DMA(Designated Market Area). |
| [!UICONTROL Dimension] | [!UICONTROL Geos] | [!UICONTROL State] | 보고된 데이터가 속하는 상태입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Household] | [!UICONTROL Audience] | 청중. 이 보고서는 최대 10개의 고유한 대상을 지원합니다. |
| [!UICONTROL Dimension] | [!UICONTROL Household] | [!UICONTROL Campaign] | 캠페인. |
| [!UICONTROL Dimension] | [!UICONTROL Household] | [!UICONTROL Creative Length] | 크리에이티브의 길이. 이 보고서는 최대 10개의 고유한 크리에이티브 길이를 지원합니다. |
| [!UICONTROL Dimension] | [!UICONTROL Household] | [!UICONTROL Device] | 디바이스. 이 보고서는 최대 10개의 고유 장치를 지원합니다. |
| [!UICONTROL Dimension] | [!UICONTROL Household] | [!UICONTROL Feed Type] | 피드 유형. 보고서는 최대 10개의 고유한 피드 유형을 지원합니다. |
| [!UICONTROL Dimension] | [!UICONTROL Household] | [!UICONTROL Media Type] | 미디어 유형. 이 보고서는 최대 10개의 고유한 미디어 유형을 지원합니다. |
| [!UICONTROL Dimension] | [!UICONTROL Household] | [!UICONTROL Publisher] | 게시자입니다. 이 보고서는 최대 10개의 고유한 게시자를 지원합니다. |
| [!UICONTROL Dimension] | [!UICONTROL Household] | [!UICONTROL Package] | 패키지. <!-- Note: The Package dimensions include another dimension called Package Name. --> |
| [!UICONTROL Dimension] | [!UICONTROL Household] | [!UICONTROL Placement] | 배치입니다.<!-- Note: The Placement dimensions include another dimension called Placement Name --> |
| [!UICONTROL Dimension] | [!UICONTROL Household] | [!UICONTROL Site/Apps] | 광고 노출이 제공된 사이트 또는 앱입니다. 이 보고서는 최대 10개의 고유한 사이트 또는 앱을 지원합니다. |
| [!UICONTROL Dimension] | [!UICONTROL Household] | [!UICONTROL Tags] | 배치에 대한 사용자 지정 식별자로 사용되는 배치 태그입니다. 이 보고서는 최대 10개의 고유한 배치 태그를 지원합니다. <!-- Note: The Placement dimensions include another dimension called Placement Tags. --> |
| [!UICONTROL Dimension] | [!UICONTROL Household Conversions] | [!UICONTROL Audience] | 청중. |
| [!UICONTROL Dimension] | [!UICONTROL Household Conversions] | [!UICONTROL Campaign] | 캠페인. |
| [!UICONTROL Dimension] | [!UICONTROL Household Conversions] | [!UICONTROL Creative Length] | 크리에이티브의 길이. |
| [!UICONTROL Dimension] | [!UICONTROL Household Conversions] | [!UICONTROL Device] | 디바이스. (CTV, 데스크탑 등) |
| [!UICONTROL Dimension] | [!UICONTROL Household Conversions] | [!UICONTROL Media Type] | 미디어 유형. (디스플레이, 오디오 등) |
| [!UICONTROL Dimension] | [!UICONTROL Household Conversions] | [!UICONTROL Publisher] | 게시자입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Household Conversions] | [!UICONTROL Placement] | 배치. |
| [!UICONTROL Dimension] | [!UICONTROL Packages] | [!UICONTROL Package End Date] | 패키지의 종료 날짜입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Packages] | [!UICONTROL Package Goal Type] | 패키지의 게재 간격 목표 양입니다. 이 금액은 지출 또는 노출 횟수입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Packages] | [!UICONTROL Package ID] | DSP 패키지의 고유 식별자입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Packages] | [!UICONTROL Package Name] | 패키지 이름 |
| [!UICONTROL Dimension] | [!UICONTROL Packages] | [!UICONTROL Package Start Date] | 패키지 시작 날짜입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Packages] | [!UICONTROL Placement End Date] | 배치 종료 일자. |
| [!UICONTROL Dimension] | [!UICONTROL Pixel] | [!UICONTROL Conversion ID] | (사용하지 않음) DSP에서 레거시 [!DNL TubeMogul] 전환 이벤트에 할당한 전환 ID입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Pixel] | [!UICONTROL Conversion Name] | (사용하지 않음) 레거시 [!DNL TubeMogul] 전환 이벤트에 할당된 전환 이름입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Placement] | [!UICONTROL Placement ID] | DSP 배치에 대한 고유 식별자. |
| [!UICONTROL Dimension] | [!UICONTROL Placement] | [!UICONTROL Placement Name] | 사용자가 지정한 배치의 이름입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Placement] | [!UICONTROL Budget] | 배치 예산. |
| [!UICONTROL Dimension] | [!UICONTROL Placement] | [!UICONTROL Max Bid] | 배치에 대한 최대 입찰가. |
| [!UICONTROL Dimension] | [!UICONTROL Placement] | [!UICONTROL Device Environment] | 배치가 타겟팅하는 장치 환경: (*[!UICONTROL Desktop]*, *[!UICONTROL Mobile]* 및/또는 *[!UICONTROL Connected TV])*. |
| [!UICONTROL Dimension] | [!UICONTROL Placement] | [!UICONTROL Placement End Date] | 배치 종료 일자. |
| [!UICONTROL Dimension] | [!UICONTROL Placement] | [!UICONTROL Placement Start Date] | 배치 시작 일자. |
| [!UICONTROL Dimension] | [!UICONTROL Placement] | [!UICONTROL Placement Tags] | 배치에 대한 사용자 지정 식별자로 사용되는 배치 태그입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Segment] | [!UICONTROL Billing Segment Description] | 청구 가능 세그먼트와 연관된 설명입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Segment] | [!UICONTROL Billing Segment Key] | 청구 가능 세그먼트와 연계된 고유 키. |
| [!UICONTROL Dimension] | [!UICONTROL Segment] | [!UICONTROL Billing Segment Name] | 청구 가능한 세그먼트의 이름입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Segment] | [!UICONTROL Segment Membership Description] | 데이터 공급자가 제공하는 세그먼트와 연계된 설명. |
| [!UICONTROL Dimension] | [!UICONTROL Segment] | [!UICONTROL Segment Membership Key] | 세그먼트와 연결된 고유 키. |
| [!UICONTROL Dimension] | [!UICONTROL Segment] | [!UICONTROL Segment Membership Name] | 세그먼트 이름입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Segment] | [!UICONTROL Segment Membership Provider Name] | 세그먼트와 연계된 데이터 공급자의 이름입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Site] | [!UICONTROL Site ID] | DSP 사이트 또는 앱의 고유 식별자입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Site] | [!UICONTROL Site Name] | 사이트의 이름입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Video] | [!UICONTROL Video Duration] | 업로드 후 처리되는 비디오 길이입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Video] | [!UICONTROL Video ID] | DSP의 비디오 크리에이티브에 대한 고유 식별자입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Video] | [!UICONTROL Video Name] | 사용자가 할당한 크리에이티브의 이름. |
| [!UICONTROL Metrics] | [!UICONTROL Frequency] | [!UICONTROL % Distinct Uniques] | [!UICONTROL App/Site Distinct Uniques]을(를) [!UICONTROL App/Site Uniques]&#x200B;(으)로 나눈 값입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Frequency] | [!UICONTROL App/Site Distinct Uniques] | 이 앱에서만 도달한 총 장치 수입니다. 여러 게시자에서 광고에 노출되는 뷰어는 이 값에 포함되지 않습니다. |
| [!UICONTROL Metrics] | [!UICONTROL Frequency] | [!UICONTROL Cost per Distinct Unique] | [!UICONTROL Total Spend]을(를) [!UICONTROL App/Site Distinct Uniques]&#x200B;(으)로 나눈 값입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Frequency] | [!UICONTROL Cost per Unique] | [!UICONTROL Total Spend]을(를) [!UICONTROL App/Site Uniques]&#x200B;(으)로 나눈 값입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Frequency] | [!UICONTROL Estimated % Reached] | 노출을 받은 타겟팅된 가정 우주의 예상 백분율입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Frequency] | [!UICONTROL Estimated Average Frequency] | 고유 항목에 표시된 평균 노출 횟수입니다. 일부 인벤토리의 경우 게시자는 장치 식별자를 전달하지 않으며 그러한 노출 횟수는 이 값에 포함되지 않습니다. [!UICONTROL Frequency (by App/Site)] 보고서에 유사한 지표가 있지만 해당 지표는 예상되지 않습니다. |
| [!UICONTROL Metrics] | [!UICONTROL Frequency] | [!UICONTROL Estimated Impressions (Device/Browser)] | ([!UICONTROL Frequency (by Impression)] 보고서에 포함됨) 특정 빈도 분류에 대한 예상 노출 횟수입니다. DSP 예상 값은 노출 횟수의 샘플을 기반으로 합니다. 일부 인벤토리의 경우 게시자는 장치 식별자를 전달하지 않으며 그러한 노출 횟수는 이 값에 포함되지 않습니다. [!UICONTROL Frequency (by App/Site)] 보고서에 유사한 지표가 있지만 해당 지표는 예상되지 않습니다. |
| [!UICONTROL Metrics] | [!UICONTROL Frequency] | [!UICONTROL Estimated Uniques (Device/Browser)] | ([!UICONTROL Frequency (by Impression)] 보고서에 포함됨) 특정 빈도에 대해 기록된 고유한 브라우저 또는 장치의 수입니다. DSP 예상 값은 노출 횟수의 샘플을 기반으로 합니다. 일부 인벤토리의 경우 장치 식별자를 전달하지 마십시오. 해당 노출은 이 값에 포함되지 않습니다. [!UICONTROL Frequency (by App/Site)] 보고서에 유사한 지표가 있지만 해당 지표는 예상되지 않습니다. |
| [!UICONTROL Metrics] | [!UICONTROL Frequency] | [!UICONTROL Estimated Universe] | DSP(경매)가 날짜 범위 내에서 본 고유 가구의 합계입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Frequency] | [!UICONTROL Extended Impressions] | 사용자 기반, 크로스 디바이스 타깃팅에 디바이스 그래프를 사용한 결과로 제공된 총 노출 횟수입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Household] | [!UICONTROL Frequency] | 가구당 노출 빈도. |
| [!UICONTROL Metrics] | [!UICONTROL Household] | [!UICONTROL Frequency Overlap] | 차원에 대한 최대 3개 값의 교차를 포함하여 보고된 차원으로만 가구에 도달하는 빈도입니다. 예를 들어 [!UICONTROL Placement] 차원을 사용하는 경우 개별 배치에서 도달하는 빈도, 두 배치의 조합에서 도달한 빈도, 세 배치의 조합에서 도달한 빈도를 볼 수 있습니다. |
| [!UICONTROL Metrics] | [!UICONTROL Household] | [!UICONTROL Incremental Household Reached] | 보고된 차원에서만 도달한 가구 수(보고된 차원에서만 도달한 <code>[IP 주소] - [다른 차원에서 도달한 IP 주소]로 계산)</code>. |
| [!UICONTROL Metrics] | [!UICONTROL Household] | [!UICONTROL % Incremental Household Reached] | 보고된 차원에서만 도달한 가구의 백분율을 <code>[차원에 도달한 IP 주소의 백분율] - [다른 차원에 도달한 IP 주소의 백분율]로 계산합니다.</code>. |
| [!UICONTROL Metrics] | [!UICONTROL Household] | [!UICONTROL Impressions] | 제공된 총 광고 노출 횟수. |
| [!UICONTROL Metrics] | [!UICONTROL Household] | [!UICONTROL Measurable Impressions] | 조회 수를 측정할 수 있는 제공된 총 노출 횟수. |
| [!UICONTROL Metrics] | [!UICONTROL Household] | [!UICONTROL Measurable Impressions (Overlap)] | 차원에 대해 최대 3개 값의 교차를 포함하여 보고된 차원에서만 제공되는 측정 가능한 총 노출 횟수입니다. 예를 들어 [!UICONTROL Placement] 차원을 사용하는 경우 개별 배치로 인한 측정 가능한 노출, 두 배치의 조합으로 인한 측정 가능한 노출 및 세 배치의 조합으로 인한 측정 가능한 노출 수를 볼 수 있습니다. |
| [!UICONTROL Metrics] | [!UICONTROL Household] | [!UICONTROL Total Media Spend] | 총 지출입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Household] | [!UICONTROL Unique Household Reached] | 총 고유 가구(고유 IP 주소)에 도달했습니다. |
| [!UICONTROL Metrics] | [!UICONTROL Household] | [!UICONTROL Unique Household (Overlap)] | 차원에 대해 최대 3개의 값 교차를 포함하여 보고된 차원에서만 도달한 총 고유 세대(개별 IP 주소)입니다. 예를 들어 [!UICONTROL Placement] 차원을 사용하는 경우 개별 배치에 의해 도달된 고유한 가구, 두 배치의 조합에 의해 도달된 일반적인 가구 및 세 배치의 조합에 의해 도달된 일반적인 가구를 볼 수 있습니다. |
| [!UICONTROL Metrics] | [!UICONTROL Household Conversions] | [!UICONTROL Cost per Incremental HH] | 증분 가구로 나눈 총 지출이 도달했습니다. |
| [!UICONTROL Metrics] | [!UICONTROL Household Conversions] | [!UICONTROL Cost per Unique HH] | 고유 가구로 나눈 총 지출 금액이 도달했습니다. |
| [!UICONTROL Metrics] | [!UICONTROL Household Conversions] | [!UICONTROL Frequency] | 가구당 노출 빈도. |
| [!UICONTROL Metrics] | [!UICONTROL Household Conversions] | [!UICONTROL Incremental Household Reached] | 보고된 차원에서만 도달한 가구 수는 보고된 차원에서만 도달한 [IP 주소] - 다른 차원에서 도달한 [IP 주소]로 계산됩니다. |
| [!UICONTROL Metrics] | [!UICONTROL Household Conversions] | [!UICONTROL % Incremental Household Reached] | 보고된 차원에서만 도달한 가구의 백분율은 [차원이 도달한 IP 주소의 백분율] - [다른 차원이 도달한 IP 주소의 백분율]로 계산됩니다. |
| [!UICONTROL Metrics] | [!UICONTROL Household Conversions] | [!UICONTROL Impressions] | 제공된 총 광고 노출 횟수. |
| [!UICONTROL Metrics] | [!UICONTROL Household Conversions] | [!UICONTROL Measurable Impressions] | 조회 수를 측정할 수 있는 제공된 총 노출 횟수. |
| [!UICONTROL Metrics] | [!UICONTROL Household Conversions] | [!UICONTROL Total Media Spend] | 총 지출입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Household Conversions] | [!UICONTROL Unique Household Reached] | 총 고유 가구(고유 IP 주소)에 도달했습니다. |
| [!UICONTROL Metrics] | [!UICONTROL Identifier] | [!UICONTROL Identifier Type] | 타겟팅된 ID의 유형입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Performance] | [!UICONTROL % bid at Max CPM] | 최대 CPM에서 입찰한 총 입찰의 백분율입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Performance] | [!UICONTROL Gross CPA] | <code>[!UICONTROL Gross Spend]/[!UICONTROL Custom Goal]에 의해 계산된 획득당 평균 총 비용</code>. |
| [!UICONTROL Metrics] | [!UICONTROL Performance] | [!UICONTROL Gross CPC] | 광고 클릭당 평균 총 비용입니다(<code>[!UICONTROL Gross Spend]/[!UICONTROL Total Ad Clicks]).</code>. |
| [!UICONTROL Metrics] | [!UICONTROL Performance] | [!UICONTROL Gross CPCV] | 완료된 비디오 보기당 평균 비용입니다(<code>[!UICONTROL Gross Spend]/[!UICONTROL 100% Completions]).</code>. |
| [!UICONTROL Metrics] | [!UICONTROL Performance] | [!UICONTROL Gross CPE] | 광고 참여당 평균 총 비용입니다(<code>[!UICONTROL Gross Spend]/[!UICONTROL Total Ad Engagements]).</code>. |
| [!UICONTROL Metrics] | [!UICONTROL Performance] | [!UICONTROL Gross CPI] | 광고 노출당 평균 총 비용입니다(<code>[!UICONTROL Gross Spend]/[!UICONTROL Total Ad Impressions]).</code>. |
| [!UICONTROL Metrics] | [!UICONTROL Performance] | [!UICONTROL Gross CPM] | <code>[!UICONTROL Gross Spend] / [!UICONTROL Impressions] x 1000으로 계산된 1000회 노출당 평균 비용</code>. |
| [!UICONTROL Metrics] | [!UICONTROL Performance] | [!UICONTROL Gross CPV] | <code>[!UICONTROL Gross Spend]/[!UICONTROL Views]에 의해 계산된 비디오 보기당 평균 비용입니다.</code>. |
| [!UICONTROL Metrics] | [!UICONTROL Performance] | [!UICONTROL Gross vCPM] | <code>[!UICONTROL Gross Spend] / [!UICONTROL Viewable Impressions] x 1000으로 계산된 조회 가능한 노출 횟수 1000건당 평균 비용</code>. |
| [!UICONTROL Metrics] | [!UICONTROL Performance] | [!UICONTROL Net CPC] | 광고 클릭당 평균 순 비용입니다. <code>[!UICONTROL Net Spend]/[!UICONTROL Total Ad Clicks]&#x200B;(으)로 계산됨</code>. |
| [!UICONTROL Metrics] | [!UICONTROL Performance] | [!UICONTROL Net CPCV] | <code>[!UICONTROL Net Spend]/[!UICONTROL 100% Completions]에 의해 계산된 완료된 비디오 보기당 평균 순 비용</code>. |
| [!UICONTROL Metrics] | [!UICONTROL Performance] | [!UICONTROL Net CPI] | 광고 노출당 평균 순 비용입니다(<code>[!UICONTROL Net Spend]/[!UICONTROL Total Ad Impressions]).</code>. |
| [!UICONTROL Metrics] | [!UICONTROL Performance] | [!UICONTROL Net CPM] | <code>[!UICONTROL Net Spend] / [!UICONTROL Impressions] x 1000으로 계산된 1000회 노출당 평균 순 비용</code>. |
| [!UICONTROL Metrics] | [!UICONTROL Performance] | [!UICONTROL Net CPV] | <code>[!UICONTROL Net Spend]/[!UICONTROL Views]에 의해 계산된 비디오 보기당 평균 순 비용</code>. |
| [!UICONTROL Metrics] | [!UICONTROL Performance] | [!UICONTROL Net vCPM] | <code>[!UICONTROL Net Spend] / [!UICONTROL Viewable Impressions] x 1000으로 계산된 조회 가능한 노출 횟수 1000건당 평균 순 비용</code>. |
| [!UICONTROL Metrics] | [!UICONTROL Performance] | [!UICONTROL Unique Users Bid On] | DSP이 배치를 위해 입찰한 고유한 사용자 수입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Agency Fee] | 대행 서비스 요금. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Billable Creative Spend] | Adobe Creative에서 제공하는 광고에 대한 총 지출입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Billable Data Spend] | DSP을 통해 청구된 대상 세그먼트 데이터 요금의 총 순 비용입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Billable Media Spend] | 기술 비용을 포함하여 청구 가능한 미디어의 총 순 비용으로, DSP을 통해 청구됩니다. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Billable Other Spend] | DSP을 통해 청구된 기타 서비스 요금(타사 인증 파트너, 광고 서비스 제공 등)의 총 비용입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Estimated Tax on Creative] | Adobe Creative에서 제공하는 광고에 대한 예상 세금입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Estimated Tax on Data] | 서드파티 대상 세그먼트 및 데이터 서비스에 대한 예상 세금입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Estimated Tax on Media] | DSP의 미디어 비용 재청구 및 기술 비용 서비스에 적용되는 세금을 포함하는 미디어에 대한 예상 세금입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Estimated Tax on Other] | DSP을 통해 청구된 기타 서비스 수수료(타사 확인 파트너, 주제 타겟팅 등 포함)에 대한 예상 세금입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Gross Spend] | 총 지출액. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Margin %] | (여백 관리가 활성화된 경우) <code>([!UICONTROL Gross Spend] - [!UICONTROL Net Spend]) / [!UICONTROL Gross Spend]&#x200B;(으)로 계산되는 여백 비율입니다.</code>. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Media Cost] | 기술 수수료 없이 청구 불가능한 미디어 비용과 청구 가능한 미디어 비용의 합계입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Net vCPM] | <code>[!UICONTROL Net Spend] / [!UICONTROL Viewable Impressions] x 1000으로 계산된 조회 가능한 노출 횟수 1000건당 평균 순 비용</code>. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Non Billable Creative Spend] | Adobe Creative을 통해 청구되지 않은 광고에 대한 총 지출입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Non-Billable Data Spend] | DSP을 통해 청구되지 않은 대상 세그먼트 데이터 요금의 총 순 비용입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Non-Billable Media Spend] | DSP을 통해 청구되지 않는 기술 비용을 포함하여 청구 불가능한 미디어의 총 순 비용. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Non-Billable Other Net Spend] | DSP을 통해 청구되지 않은 기타 서비스 요금(타사 인증 파트너 및 서비스 제공 등)의 총 비용. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Profit] | [!UICONTROL Gross Spend] - [!UICONTROL Net Spend] |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Total Billable Spend] | [!UICONTROL Billable Spend (Media)], [!UICONTROL Billable Spend (Data)] 및 [!UICONTROL Billable Spend (Other)]의 합계입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Total Creative CPM] | Adobe Creative에서 제공하는 광고의 1000개 노출당 평균 순 미디어 비용입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Total Creative Spend] | Adobe Creative에서 제공하는 광고에 대한 총 청구 가능 및 청구 불가능 지출. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Total Data eCPM] | <code>[!UICONTROL Net Spend (Data)] / [!UICONTROL Impressions] x 1000으로 계산된 1000회 노출당 평균 순 데이터 비용입니다.</code>. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Total Data Spend] | 대상 세그먼트 데이터 요금의 총 순 비용입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Total Media CPM] | <code>[!UICONTROL Net Spend (Media)] / [!UICONTROL Impressions] x 1000으로 계산된 1000회 노출당 평균 순 미디어 비용</code>. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Total Media Spend] | 기술 비용을 포함한 미디어의 총 순 비용. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Total Net Spend] | [!UICONTROL Net Spend (Media)], [!UICONTROL Net Spend (Data)] 및 [!UICONTROL Net Spend (Other)]의 합계입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Total Non-Billable Net Spend] | [!UICONTROL Non-billable Spend (Media)], [!UICONTROL Non-billable Spend (Data)] 및 [!UICONTROL Non-billable Spend (Other)]의 합계입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Total Other eCPM] | 기타 수수료에 대한 1000회 노출당 평균 순 비용, <code>[!UICONTROL Net Spend (Other)]/[!UICONTROL Impressions] x 1000으로 계산됨</code>. |
| [!UICONTROL Metrics] | [!UICONTROL Spend] | [!UICONTROL Total Other Spend] | 기타 서비스 요금(타사 인증 파트너, 광고 서비스 등)의 총 순 비용. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL 100% Completion Rate] | 광고 전체를 시청한 보기 횟수의 비율입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL 100% Completions] | 광고 전체를 시청한 보기 수입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL 100% Viewable Completion (%)] | 광고 전체를 시청한 볼 수 있는 노출 횟수의 백분율입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL 25% Completion Rate] | 최소 1개 이상의 광고 분위를 시청한 보기 비율입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL 25% Completions] | 최소 1개 이상의 광고 사분위를 시청한 보기 수입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL 50% Completion Rate] | 광고의 최소 2개 사분위를 시청한 보기 비율입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL 50% Completions] | 광고의 최소 2개 사분위를 시청한 보기 수입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL 50% Viewable Completion (%)] | 최소 2개 이상의 광고 사분위를 시청한 볼 수 있는 노출 횟수입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL 75% Completion Rate] | 광고의 최소 3개 사분위를 시청한 보기 비율입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL 75% Completions] | 광고의 최소 3개 사분위를 시청한 보기 수입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL Avg Percent Viewed] | 광고가 완료되기 위해 시청한 평균 백분율로, 모든 보기를 차지합니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL Banner and Overlay Clicks] | 광고 오버레이 및 배너의 클릭 수입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL Click Through Rate] | 광고 노출 횟수로 나눈 클릭 수의 백분율입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL Clicks Per View Rate] | 클릭수를 비디오 보기로 나눈 비율입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL Companion Clicks] | 컴패니언 배너 클릭 수입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL Companion CTR] | 클릭 수를 컴패니언 배너 노출 횟수로 나눈 비율입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL Companion Impressions] | 컴패니언 배너 노출 횟수. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL Connection] | 광고를 보는 데 사용된 인터넷 연결 유형(예: Wifi 또는 4g LTE). |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL Engagements] | 제공된 광고의 상호 작용 수입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL Impressions] | 총 광고 노출 횟수. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL Play Rate] | 비디오 보기에 도달한 제공된 노출 횟수의 비율입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL Playtime per View] | 비디오 보기의 평균 기간(초 단위)입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL Total Ad Clicks] | 광고의 모든 클릭 수 합계입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL Viewed Minutes] | 비디오 광고를 본 총 시간(분)입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL Views] | 총 비디오 광고 보기 횟수. |
| [!UICONTROL Metrics] | [!UICONTROL Viewability] | [!UICONTROL Avg. Player Width x Height] | 평균 플레이어 너비 및 높이입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Viewability] | [!UICONTROL Measurable Impressions] | 조회 수를 측정할 수 있는 제공된 총 노출 횟수. |
| [!UICONTROL Metrics] | [!UICONTROL Viewability] | [!UICONTROL Measurable Rate (%)] | 조회 수를 측정할 수 있었던 제공된 노출 횟수의 백분율로, <code>[!UICONTROL Measurable Impressions] x 1000 / [!UICONTROL Impressions]로 계산됩니다.</code>. |
| [!UICONTROL Metrics] | [!UICONTROL Viewability] | [!UICONTROL Unmeasurable - iFrame (%)] | 호환되지 않는 iFrame으로 인해 보기에 측정할 수 없는 노출 비율입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Viewability] | [!UICONTROL Unmeasurable - Not Supported (%)] | 광고 단위에서 지원되지 않는 조회 추적으로 인해 보기에 측정할 수 없는 노출 횟수입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Viewability] | [!UICONTROL Unmeasurable - Other (%)] | 다른 이유로 인해 조회가 불가능한 노출 비율입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Viewability] | [!UICONTROL Unmeasurable Impressions] | 조회에 측정할 수 없는 광고 노출 횟수입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Viewability] | [!UICONTROL Unmeasurable Rate (%)] | 조회에 측정할 수 없는 광고 노출 비율입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Viewability] | [!UICONTROL Unmeasurable rate (Not supported)] | 이 광고 단위에서 지원되지 않는 조회 추적으로 인해 조회에 측정할 수 없는 노출 비율입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Viewability] | [!UICONTROL Viewability Rate (%)] | 측정 가능한 모든 노출 중 볼 수 있는 노출 횟수의 백분율로, <code>[!UICONTROL Viewable Impressions] / [!UICONTROL Measurable Impressions]&#x200B;(으)로 계산됩니다.</code>. |
| [!UICONTROL Metrics] | [!UICONTROL Viewability] | [!UICONTROL Viewable Impressions] | 조회 가능한 것으로 간주된 광고 노출 횟수. |
| [!UICONTROL Conversion Metrics] | [보고서 설정에서 광고주별로 그룹화됨] | [광고주별 전환] | 지정된 광고주별 전환 지표 또는 Adobe Analytics 이벤트에 대한 합계입니다. |
| [!UICONTROL Custom Goals] | [보고서 설정에서 광고주별로 그룹화됨] | [광고주별 사용자 지정 목표] | 지정된 [사용자 지정 목표](/help/dsp/optimization/custom-goal.md)에 포함된 모든 전환의 가중 합계입니다. |

{style="table-layout:auto"}

<!-- |Omitted|[!UICONTROL Performance]|Custom Goal CPA|The average cost per acquisition, calculated by <code>Gross Spend / Custom Goal</code> | -->
<!-- |Omitted|[!UICONTROL Performance]|Custom Goal ROAS|The average return on ad spend, calculated by <code>Custom goal / Gross spend</code> |-->

>[!MORELIKETHIS]
>
>* [사용자 지정 보고서 정보](/help/dsp/reports/report-about.md)
>* [사용자 지정 보고서 만들기](/help/dsp/reports/report-create.md)
>* [사용자 지정 보고서 복제](/help/dsp/reports/report-copy.md)
>* [사용자 지정 보고서 편집](/help/dsp/reports/report-edit.md)
>* [사용자 지정 보고서 설정](/help/dsp/reports/report-settings.md)
