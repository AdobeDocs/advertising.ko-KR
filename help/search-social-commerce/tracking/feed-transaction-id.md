---
title: 거래 ID 피드를 사용한 전환 추적
description: 전환 추적 데이터에 거래 ID 피드를 사용하는 방법에 대해 알아봅니다.
exl-id: 3341ac20-d435-4387-99da-7b874e53c2e7
feature: Search Tracking
TQID: https://experienceleague.adobe.com/wGlR5tUF7ajbnQLUnW0c-U84BskLzr63Wet-e-x823M
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 527ca2bb74de388c13ba1ce5bde3f8be1cead8d0
workflow-type: tm+mt
source-wordcount: 293
ht-degree: 0%

---

# 거래 ID 피드를 사용한 전환 추적

광고주가 온라인 및 오프라인 트랜잭션을 모두 보유한 경우, Adobe Advertising은 Adobe Advertising 전환 추적 픽셀을 통해 온라인 트랜잭션을 추적할 수 있으며, 광고주는 트랜잭션 ID를 사용하여 오프라인 트랜잭션을 추적하고 피드를 통해 이를 전달할 수 있습니다.

* 온라인 트랜잭션의 경우 Adobe Advertising은 광고 클릭 수와 웹 사이트의 결과 트랜잭션을 추적합니다.

* 광고주는 오프라인 전환을 추적하고 트랜잭션 수준 피드 파일을 Adobe Advertising에 보내야 합니다.

## 구현 개요

*에이전시 계정 관리자, [!DNL Adobe] 계정 관리자 및 관리자 역할만*

1. 계정 또는 캠페인 추적 옵션 &quot;[!UICONTROL EF Redirect]&quot; 및 &quot;[!UICONTROL Auto Upload]&quot;을(를) 사용하여 계정 또는 캠페인의 각 키워드(키워드 수준 추적용) 또는 광고(광고 수준 추적용)에 대한 대상 URL 또는 최종 URL을 자동으로 생성합니다.

1. 온라인 전환에 대한 Adobe Advertising 전환 추적을 설정합니다. 이 프로세스는 Adobe Advertising 픽셀 기반 전환 추적을 사용하는 광고주와 동일합니다. 고유한 거래 ID(`ev_transid=<transid>`)에 대한 매개 변수를 포함하는 전환 태그를 생성하는 것이 중요합니다.

1. 각 트랜잭션의 오프라인 부분에 대해 광고주는 피드 파일에 포함할 트랜잭션의 온라인 부분에 사용된 동일한 트랜잭션 ID를 생성합니다.

1. 광고주가 [필요한 변환 데이터](/help/search-social-commerce/tracking/feed-transaction-id-data-requirements.md)가 포함된 파일을 지정된 서버 위치에 업로드합니다.

1. 기술 서비스는 업로드된 파일의 변환 데이터를 구문 분석한 다음 데이터를 Adobe Advertising에 업로드합니다. 그런 다음 Adobe Advertising은 개별 키워드, 광고 및 배치에 대해 데이터를 추적하고 각각에 대한 매출 예측을 만듭니다.

1. 기술 서비스는 피드 데이터에 대해 처리된 데이터의 유효성을 검사하고 [고립 트랜잭션](/help/search-social-commerce/glossary.md#o-p)을(를) 확인합니다.

>[!MORELIKETHIS]
>
>* [변환 피드 파일에 대한 파일 요구 사항](feed-file-requirements.md)
>* [거래 ID를 사용하는 데이터 피드에 대한 데이터 요구 사항](/help/search-social-commerce/tracking/feed-transaction-id-data-requirements.md)
