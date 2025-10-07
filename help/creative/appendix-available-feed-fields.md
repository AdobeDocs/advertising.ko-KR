---
title: 동적 광고 피드 파일에 사용 가능한 필드
description: 동적 광고를 만드는 데 사용하는 피드 파일에 포함할 수 있는 필드에 대해 알아봅니다.
feature: Creative Dynamic Creatives
source-git-commit: 67ee38860ac5cb7e9340f8e9d4667353e509b1ec
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# 부록: 동적 광고 피드 파일에 사용 가능한 필드

Advertising Creative 백엔드에서 다음 피드 필드를 사용할 수 있습니다. 조직별 필드 이름을 사용하는 [피드 파일](/help/creative/feeds/asset-manage.md)을 업로드할 수 있습니다. 그러나 피드 파일에서 [카탈로그](/help/creative/feeds/catalog-manage.md)를 만들려면 먼저 피드 파일의 각 필드를 카탈로그를 만드는 데 사용할 [피드 템플릿](/help/creative/feeds/feed-template-manage.md)의 다음 필드 중 하나에 매핑해야 합니다.

피드 파일에 동등한 항목이 있어야 하는 유일한 필드는 `PART_NUM`입니다.

<!-- Questions:

What are these?
Rank
PROFILE_FILTER fields



Do geo fields need be populated as follows:
Country: 2 Letter country code (example: US)
State: state code_2 letter country code (example: CA_US)
City: City name_State code_2 letter country code (example: San Jose_CA_US)
DMA: DMA _2 letter country code (example: 201_US)
Zipcode: Zip code_2 letter country code (example: 94086_US)


TRUE?   GEO fields(Country/State/City/DMA/Zip), UT fields (UT1/UT2/UT3/UT4/UT5) [do we have an equivalent now?], Filtering fields(F1/F2/F3/F4/F5) can have comma separated values. We can have upto 2K characters.

TRUE FOR CSV AND TSV? character encoding on text format files should be UTF-8 -- If yes, then add that with feed file requirements.

-->

| 필드 이름 | 데이터 유형 | 필수? |
|------------|-----------|-----------|
| PART_NUM | varchar(64) | 예 |
| PRODUCT_이름 | 텍스트 | 아니요 |
| PRODUCT_URL | 텍스트 | 아니요 |
| 가격 | 십진수(10,2) | 아니요 |
| DISCOUNT_PRICE | 십진수(10,2) | 아니요 |
| 이미지 | varchar(1024) | 아니요 |
| IMAGE_높이 | int | 아니요 |
| IMAGE_너비 | int | 아니요 |
| 이미지_1 | varchar(1024) | 아니요 |
| 이미지 2 | varchar(1024) | 아니요 |
| 이미지_3 | varchar(1024) | 아니요 |
| 이미지_4 | varchar(1024) | 아니요 |
| 이미지_5 | varchar(1024) | 아니요 |
| 이미지_6 | varchar(1024) | 아니요 |
| 이미지_7 | varchar(1024) | 아니요 |
| 이미지_8 | varchar(1024) | 아니요 |
| IMAGE_9 | varchar(1024) | 아니요 |
| 이미지_10 | varchar(1024) | 아니요 |
| TEXT_1 | 텍스트 | 아니요 |
| TEXT_2 | 텍스트 | 아니요 |
| TEXT_3 | 텍스트 | 아니요 |
| TEXT_4 | 텍스트 | 아니요 |
| TEXT_5 | 텍스트 | 아니요 |
| TEXT_6 | 텍스트 | 아니요 |
| TEXT_7 | 텍스트 | 아니요 |
| TEXT_8 | 텍스트 | 아니요 |
| TEXT_9 | 텍스트 | 아니요 |
| TEXT_10 | 텍스트 | 아니요 |
| TEXT_11 | 텍스트 | 아니요 |
| TEXT_12 | 텍스트 | 아니요 |
| TEXT_13 | 텍스트 | 아니요 |
| TEXT_14 | 텍스트 | 아니요 |
| TEXT_15 | 텍스트 | 아니요 |
| ADDITIONAL_PRICE_1 | 십진수(10,2) | 아니요 |
| ADDITIONAL_PRICE_2 | 십진수(10,2) | 아니요 |
| ADDITIONAL_PRICE_3 | 십진수(10,2) | 아니요 |
| AD_SIZE | varchar(32) | 아니요 |
| 순위 | int | 아니요 |
| 국가 | 텍스트 | 아니요 |
| 시/도 | 텍스트 | 아니요 |
| 도시 | 텍스트 | 아니요 |
| ZIP | 텍스트 | 아니요 |
| DMA | 텍스트 | 아니요 |
| PROFILE_FILTER_1 | 텍스트 | 아니요 |
| PROFILE_FILTER_2 | 텍스트 | 아니요 |
| PROFILE_FILTER_3 | 텍스트 | 아니요 |
| PROFILE_FILTER_4 | 텍스트 | 아니요 |
| PROFILE_필터_5 | 텍스트 | 아니요 |
| DATAPASS_FILTER_1 | 텍스트 | 아니요 |
| DATAPASS_FILTER_2 | 텍스트 | 아니요 |
| DATAPASS_FILTER_3 | 텍스트 | 아니요 |
| DATAPASS_FILTER_4 | 텍스트 | 아니요 |
| DATAPASS_FILTER_5 | 텍스트 | 아니요 |
| AUDIENCE_SEGMENT | 텍스트 | 아니요 |
| 언어 | 텍스트 | 아니요 |
| CREATIVE_ATTRIBUTE_1 | varchar(256) | 아니요 |
| CREATIVE_ATTRIBUTE_2 | varchar(256) | 아니요 |
| CREATIVE_ATTRIBUTE_3 | varchar(256) | 아니요 |
| CREATIVE_ATTRIBUTE_4 | varchar(256) | 아니요 |
| CREATIVE_ATTRIBUTE_5 | varchar(256) | 아니요 |
| CREATIVE_ATTRIBUTE_6 | varchar(256) | 아니요 |
| CREATIVE_ATTRIBUTE_7 | varchar(256) | 아니요 |
| CREATIVE_ATTRIBUTE_8 | varchar(256) | 아니요 |
| CREATIVE_ATTRIBUTE_9 | varchar(256) | 아니요 |
| CREATIVE_ATTRIBUTE_10 | varchar(256) | 아니요 |
| IS_DEFAULT | enum | 아니요 |

>[!MORELIKETHIS]
>
>* [동적 광고용 워크플로](/help/creative/introduction/workflow-dynamic-ads.md)
>* [자산 파일 관리](/help/creative/feeds/asset-manage.md)
>* [피드 템플릿 관리](/help/creative/feeds/feed-template-manage.md)
>* [카탈로그 관리](/help/creative/feeds/catalog-manage.md)
