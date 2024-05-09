---
title: 정보 [!UICONTROL CCPA Opt-out-of-Sale] 세그먼트 및 보고서
description: CCPA 판매 중지 요청에서 ID를 추적하는 세그먼트를 만들고 ID의 보고서를 검색하는 방법에 대해 알아봅니다.
feature: CCPA, DSP Segments
exl-id: 28b5e00b-a695-46f1-abbf-7bbd78f05411
source-git-commit: 4b9cc5956d573b346eacdf71a8ea490c162b4660
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# 정보 [!UICONTROL CCPA Opt-out-of-Sale] 세그먼트 및 보고서

캘리포니아 소비자 개인 정보 보호법(CCPA)에 따라 다음 방법으로 웹 사이트의 소비자 판매 중지 요청에서 사용자 ID를 추적할 수 있습니다. [ccpa 판매 중지 세그먼트 생성 및 구현](ccpa-opt-out-segment-create.md). 사용자는 CCPA 판매 중지 세그먼트에 무기한 유지됩니다.

세그먼트 픽셀 태그가 구현되면 Adobe Advertising은 광고주를 대신하여 ID 풀을 수집하기 시작합니다.

## 소비자 판매 중지 보고서

Adobe Advertising은 고객이 계정에 대한 판매 중지 요청을 제출한 ID에 대한 월별 보고서를 생성합니다. 이 데이터는 DSP에서 생성된 CCPA 판매 중지 세그먼트를 사용하여 캡처된 요청과 Privacy Service API를 통해 제출된 모든 요청을 통합합니다.  보고서는 이전 달의 매월 1일에 생성됩니다. 예를 들어 6월의 월별 사용자 목록은 7월 1일에 제공됩니다.

각 보고서는 GZIP 형식으로 압축된 탭으로 구분된 텍스트 파일로 사용할 수 있습니다. CCPA 판매 중지 세그먼트에 캡처된 사용자 ID는 세그먼트 및 광고주별로 식별됩니다.

다음을 수행할 수 있습니다. [월별 보고서에 대한 링크 검색](ccpa-opt-out-segment-report-retrieve.md) 지난 3개월 동안 DSP 내에서 또는 DSP을 사용하여 생성된 [!DNL Trafficking API]. 각 링크는 7일 동안 유효하지만 고객이 하나를 검색하려고 할 때마다 새로 고침됩니다.

>[!MORELIKETHIS]
>
>* [캘리포니아 소비자 개인 정보 보호법에 대한 Adobe Advertising 지원: 소비자 옵트아웃 지원](/help/privacy/ccpa/ccpa-opt-out-of-sale.md)
>* [만들기 및 구현 [!UICONTROL CCPA Opt-Out-of-Sale] 세그먼트](ccpa-opt-out-segment-create.md)
>* [소비자 판매 중지 보고서 검색](ccpa-opt-out-segment-report-retrieve.md)
>* [대상자 관리 기본 정보](audience-about.md)
