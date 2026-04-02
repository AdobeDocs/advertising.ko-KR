---
title: '[!UICONTROL CCPA Opt-out-of-Sale]개 세그먼트 및 보고서 정보'
description: CCPA 판매 중지 요청에서 ID를 추적하는 세그먼트를 만들고 ID의 보고서를 검색하는 방법에 대해 알아봅니다.
feature: CCPA, DSP Segments
exl-id: 28b5e00b-a695-46f1-abbf-7bbd78f05411
TQID: https://experienceleague.adobe.com/Bp8Fj0z7lqSXmHd-aJQa6ocQyj6FVQuydArNBucpJp4
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2:
  - id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
subfeature_v2:
  - id: c193c532-b70e-4556-bde7-857186cbe140
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 527ca2bb74de388c13ba1ce5bde3f8be1cead8d0
workflow-type: tm+mt
source-wordcount: 245
ht-degree: 0%

---

# [!UICONTROL CCPA Opt-out-of-Sale]개 세그먼트 및 보고서 정보

[CCPA 판매 중지 세그먼트를 만들고 구현](ccpa-opt-out-segment-create.md)하여 CCPA(California Consumer Privacy Act)에 따라 웹 사이트의 소비자 판매 중지 요청에서 사용자 ID를 추적할 수 있습니다. 사용자는 CCPA 판매 중지 세그먼트에 무기한 유지됩니다.

세그먼트 픽셀 태그가 구현되면 Adobe Advertising은 광고주를 대신하여 ID 풀을 수집하기 시작합니다.

## 소비자 판매 중지 보고서

Adobe Advertising은 고객이 계정에 대한 판매 중지 요청을 제출한 ID에 대한 월별 보고서를 생성합니다. 이 데이터는 DSP에서 생성된 CCPA 판매 중지 세그먼트를 사용하여 캡처된 요청과 Privacy Service API를 통해 제출된 모든 요청을 통합합니다.  보고서는 이전 달의 매월 1일에 생성됩니다. 예를 들어 6월의 월별 사용자 목록은 7월 1일에 제공됩니다.

각 보고서는 GZIP 형식으로 압축된 탭으로 구분된 텍스트 파일로 사용할 수 있습니다. CCPA 판매 중지 세그먼트에 캡처된 사용자 ID는 세그먼트 및 광고주별로 식별됩니다.

DSP 내에서 또는 DSP [을(를) 사용하여 이전 3개월 동안 만든 &#x200B;](ccpa-opt-out-segment-report-retrieve.md)월별 보고서에 대한 링크를 검색[!DNL Trafficking API]할 수 있습니다. 각 링크는 7일 동안 유효하지만 고객이 하나를 검색하려고 할 때마다 새로 고침됩니다.

>[!MORELIKETHIS]
>
>* [캘리포니아 소비자 개인 정보 보호법에 대한 Adobe Advertising 지원: 소비자 판매 거부 지원](/help/privacy/ccpa/ccpa-opt-out-of-sale.md)
>* [[!UICONTROL CCPA Opt-Out-of-Sale] 세그먼트 만들기 및 구현](ccpa-opt-out-segment-create.md)
>* [소비자 판매 중지 보고서 검색](ccpa-opt-out-segment-report-retrieve.md)
>* [대상자 관리 정보](audience-about.md)
