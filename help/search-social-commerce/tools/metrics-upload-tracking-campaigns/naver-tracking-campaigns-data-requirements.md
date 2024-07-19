---
title: ' [!DNL Naver] 추적 전용 계정의 트래픽 및 전환 지표에 대한 데이터 요구 사항'
description: ' [!DNL Naver] 추적 전용 계정에 대한 데이터 업로드 요구 사항을 참조하십시오.'
exl-id: cc8ee5de-2bf2-48fd-9fa7-28421aed673f
feature: Search Tools
source-git-commit: e16bc62127a708de8f4deb1eddfa53a14405cbc2
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---

# [!DNL Naver] 추적 전용 계정에 대한 지표 데이터 요구 사항

다음은 추적 전용 계정에 대한 [!DNL Naver] 트래픽 및 전환 지표에 대한 데이터 요구 사항입니다.

데이터 파일은 TSV, CSV 또는 TXT 형식이어야 합니다.

다음 헤더 필드는 필수이며 선택 사항입니다. 각 데이터 행에는 하나 이상의 지표 필드에 대해 일별로 집계된 값이 포함되어야 합니다.

| 헤더 필드/열 이름 | 유형 | 설명 |
| ---- | ---- | ---- |
| 기간 | DateTime | 데이터가 적용되는 날짜입니다. 형식은 `YYYY.MM.DD.`(예: `2019.11.15.`, 다음 날 이후 마침표 포함)입니다. |
| 캠페인 | 대/소문자 문자열 | 캠페인 이름. |
| 광고 그룹(한 단어로) | 대/소문자 문자열 | 광고 그룹 이름입니다. |
| 키워드 | 대/소문자 문자열 | (키워드 광고) 광고를 생성한 키워드입니다. |
| [지표] | 정수 | (선택 사항) 지표가 측정하는 [개 수]입니다.</br><br>표준 지표에는 노출 횟수, 비용 및 클릭 수가 포함됩니다. 광고 네트워크에서 원하는 추가 지표를 포함할 수 있습니다. 각 지표를 별도의 열에 포함합니다.<br><br><b>메모:</b><ul><li>비용의 열 머리글은 &quot;비용(KRW)&quot;이어야 합니다.</li><li>브랜드 광고에 비용(KRW)을 포함하려면 광고 그룹 수준에서 고정된 월별 비용을 일별로 수동으로 분할합니다.</li><li>표준 지표 값에서 모든 쉼표를 제거합니다. 예를 들어 1,000 대신 1000을 사용합니다.</li><li>null 값의 경우 0을 사용합니다.</li></ul> |

>[!MORELIKETHIS]
>
>* [추적 전용 계정 구현 [!DNL Naver] 2}](/help/search-social-commerce/campaign-management/naver-tracking-only-account-implement.md)
>* [부록 - [!DNL Naver] 계정](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-naver.md)에 대한 일괄 시트 데이터 필요)
>* [추적 전용 계정에 대한 트래픽 및 전환 지표 업로드 [!DNL Naver] 2}](/help/search-social-commerce/tools/metrics-upload-tracking-campaigns/naver-tracking-campaigns-upload-metrics.md)
