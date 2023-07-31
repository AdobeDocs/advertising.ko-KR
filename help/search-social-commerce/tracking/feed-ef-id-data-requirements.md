---
title: EF ID를 사용한 데이터 피드에 대한 데이터 요구 사항
description: EF ID를 사용하여 데이터 피드에 대한 데이터 요구 사항을 참조하십시오.
exl-id: 15e76f3a-c376-4e7b-b3c8-ca76fd427002
feature: Search Tracking
source-git-commit: f21283731d7a1830af585cec43805c54c81c72ff
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# EF ID를 사용한 데이터 피드에 대한 데이터 요구 사항

다음은 각 피드 파일 유형에 필요한 헤더 필드와 해당 데이터 필드입니다.

>[!NOTE]
>* 후속 행의 데이터가 동일한 순서를 따르는 한 헤더는 임의의 순서가 될 수 있습니다. 헤더를 포함하지 않는 경우 데이터 행의 순서는 각 피드 파일과 일치해야 합니다.
>* 피드 파일의 각 줄에는 한 트랜잭션에 대한 데이터가 포함되어야 하며, 트랜잭션은 Adobe Advertising이 생성한 ef_id(토큰)로 식별되어야 합니다.

| 헤더 필드/열 이름 | 유형 | 설명 |
| ---- | ---- | ---- |
| EF ID | 대/소문자 문자열 | 트랜잭션을 클릭할 때 캡처한 ef_id(토큰)로서, 서퍼 ID, 클릭 시간 및 네트워크 유형으로 구성됩니다. 값을 변경하지 마십시오. |
| 거래 ID | 대/소문자 문자열 | (선택 사항이지만 권장됨) 광고주가 생성한 트랜잭션 ID입니다. 가장 좋은 방법은 리디렉션 시 트랜잭션을 추적하는 데 ef_id가 사용되더라도 각 트랜잭션에 대해 이 매개 변수를 포함하는 것입니다. |
| 트랜잭션 날짜 | DateTime | 트랜잭션 날짜. 각 트랜잭션에 대해 형식이 일관되어야 합니다. |
| 클라이언트별 전환 | 문자열 | 추적 중인 전환(예: 거래 유형 또는 금액)입니다. 피드를 시작하기 전에 Adobe Advertising 구현 팀에 포함될 전환에 대해 논의합니다. |

## 예

다음 예제 파일에는 두 개의 전환 지표(제품 및 매출)에 대한 데이터가 포함되어 있습니다.

```
EF ID,Client Transaction ID, Transaction Date,Product,Revenue
TIl4VQqoEEQAAG8CU5EAAACY:20100217062449:s,04896325,2010-02-17,Coffee,15.00
SOl5PRKlPEILDG6CL3QYENOI:20100217065632:s,04896490,2010-02-17,Tea,42.00
TRl4BEtoTPMBEW4SU5ZUMEPIE:20100217065804:s,04896552,2010-02-17,Coffee,22.00
```

>[!MORELIKETHIS]
>
>* [변환 피드 파일에 대한 파일 요구 사항](feed-file-requirements.md)
>* [EF ID 피드를 사용한 전환 추적](/help/search-social-commerce/tracking/feed-efid.md)
