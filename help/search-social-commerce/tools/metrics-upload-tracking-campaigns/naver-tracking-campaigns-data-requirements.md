---
title: 다음에 대한 트래픽 및 전환 지표에 대한 데이터 요구 사항 [!DNL Naver] 추적 전용 계정
description: 에 대한 데이터 업로드 요구 사항 참조 [!DNL Naver] 추적 전용 계정입니다.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 0%

---

# 다음에 대한 지표 데이터 요구 사항 [!DNL Naver] 추적 전용 계정

다음은 의 데이터 요구 사항입니다 [!DNL Naver] 추적 전용 계정에 대한 트래픽 및 전환 지표.

데이터 파일은 TSV, CSV 또는 TXT 형식이어야 합니다.

다음 헤더 필드는 필수이며 선택 사항입니다. 각 데이터 행에는 하나 이상의 지표 필드에 대해 일별로 집계된 값이 포함되어야 합니다.

| 헤더 필드/열 이름 | 유형 | 설명 |
| ---- | ---- | ---- |
| 기간 | DateTime | 데이터가 적용되는 날짜(형식) `YYYY.MM.DD.` (예: `2019.11.15.`, (하루 뒤에 마침표 포함). |
| 캠페인 | 대/소문자 문자열 | 캠페인 이름. |
| 광고 그룹(한 단어로) | 대/소문자 문자열 | 광고 그룹 이름입니다. |
| 키워드 | 대/소문자 문자열 | (키워드 광고) 광고를 생성한 키워드입니다. |
| [지표] | 정수 | (선택 사항) [지표가 측정하는 모든 항목].</br><br>표준 지표에는 노출 횟수, 비용 및 클릭 수가 포함됩니다. 광고 네트워크에서 원하는 추가 지표를 포함할 수 있습니다. 각 지표를 별도의 열에 포함합니다.<br><br><b>참고:</b><ul><li>비용의 열 머리글은 &quot;비용(KRW)&quot;이어야 합니다.</li><li>브랜드 광고에 비용(KRW)을 포함하려면 광고 그룹 수준에서 고정된 월별 비용을 일별로 수동으로 분할합니다.</li><li>표준 지표 값에서 모든 쉼표를 제거합니다. 예를 들어 1,000 대신 1000을 사용합니다.</li><li>null 값의 경우 0을 사용합니다.</li></ul> |

>[!MORELIKETHIS]
>
>* [구현 [!DNL Naver] 추적 전용 계정](/help/search-social-commerce/campaign-management/naver-tracking-only-account-implement.md)
>* [부록 - 필수 일괄 시트 데이터 [!DNL Naver] 계정](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-naver.md))
>* [트래픽 및 전환 지표 업로드 [!DNL Naver] 추적 전용 계정](/help/search-social-commerce/tools/metrics-upload-tracking-campaigns/naver-tracking-campaigns-upload-metrics.md)

