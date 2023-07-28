---
title: 거래 ID를 사용하는 데이터 피드에 대한 데이터 요구 사항
description: 거래 ID를 사용하여 데이터 피드에 대한 데이터 요구 사항을 참조하십시오.
exl-id: 67e1cadd-b607-465c-9db6-ca76d8ca84c5
feature: Search Tracking
source-git-commit: 052574217d7ddafb8895c74094da5997b5ff83db
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---

# 거래 ID를 사용하는 데이터 피드에 대한 데이터 요구 사항

다음은 각 피드 파일 유형에 필요한 헤더 필드와 해당 데이터 필드입니다.

>[!NOTE]
>* 후속 행의 데이터가 동일한 순서를 따르는 한 헤더는 임의의 순서가 될 수 있습니다. 헤더를 포함하지 않는 경우 데이터 행의 순서는 각 피드 파일과 일치해야 합니다.
>* 피드 파일의 각 줄에는 한 트랜잭션에 대한 데이터가 포함되어야 하며, 트랜잭션은 트랜잭션 ID로 식별되어야 합니다.

| 헤더 필드/열 이름 | 유형 | 설명 |
| ---- | ---- | ---- |
| 거래 ID (ev_transid) | 대/소문자 문자열 | 거래와 연계된 광고주 생성 식별자. Adobe Advertising 전환 추적 태그는 트랜잭션의 온라인 부분에 사용되므로, 이 태그는 트랜잭션의 이전 부분에 대해 Adobe Advertising이 제공한 트랜잭션 ID(ev_transid)와 동일해야 합니다. 즉, 트랜잭션의 온라인 부분에 대한 전환 태그에 고유한 트랜잭션 ID에 대한 속성이 포함되어야 합니다.<br><br>**참고:** Adobe Advertising은 ID를 사용하여 이전 거래 데이터를 찾고 합의된 삽입 모드에 따라 업데이트합니다(예: 기존 데이터를 바꾸거나 새 데이터로 보강함). |
| 트랜잭션 날짜 | DateTime | 트랜잭션 날짜. 각 트랜잭션에 대해 형식이 일관되어야 합니다. |
| 클라이언트별 전환 | 문자열 | 추적 중인 전환(예: 거래 유형 또는 금액)입니다. 피드를 시작하기 전에 Adobe Advertising 구현 팀에 포함될 전환에 대해 논의합니다. |

## 예

다음 예제 파일에는 두 거래 속성(제품 및 매출)에 대한 데이터가 포함되어 있습니다.

```
Transaction ID,Transaction Date,Product,Revenue
12345,2010-02-17,Coffee,15.00
12346,2010-02-17,Tea,42.00
12347,2010-02-17,Coffee,22.00
```

>[!MORELIKETHIS]
>
>* [변환 피드 파일에 대한 파일 요구 사항](feed-file-requirements.md)
>* [거래 ID 피드를 사용한 전환 추적](/help/search-social-commerce/tracking/feed-transaction-id.md)
