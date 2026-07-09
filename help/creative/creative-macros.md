---
title: 추적 URL에 사용 가능한 매크로
description: 랜딩 페이지 URL, 추적 URL 및 서드파티 크리에이티브에 추가할 수 있는 매크로를 참조합니다.
feature: Creative Experiences, Creative Experiences
exl-id: d0cbbb21-467d-4ed1-bc6e-ded1b045b98b
TQID: https://experienceleague.adobe.com/J5jfIECrL29NngVOulEgHKZBHYqBmoz4680HzEzhIng
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2:
  - id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 3c3bffe0c28bb24c0df9385f9cc91be1376a66d2
workflow-type: tm+mt
source-wordcount: 319
ht-degree: 0%

---

# 추적 URL에 사용 가능한 매크로

<!-- More feature metadata???  -->

서드파티 크리에이티브, 경험에 대한 서드파티 추적 URL 및 자체 사용을 위한 랜딩 페이지 URL에 다음 매크로를 포함할 수 있습니다.

사용 가능한 매크로 중 일부 또는 이와 동등한 매크로는 경험 태그에 자동으로 포함됩니다.

<!--
 Later: 

| Macro | Description | Automatically in experience tags for Advertising DSP? | Automatically in experience tags for [!DNL Google Campaign Manager 360]? |
| --- | --- | --- | --- |
| `${TM_CAMPAIGN_ID_NUM}` | Tracks and reports the campaign ID from the DSP | Yes | No, but tags include the equivalent [!DNL Google Campaign Manager 360] macro `%ebuy!` |
| `${TM_SITE_ID_NUM}` | Tracks and reports the site ID from the DSP | Yes | No, but tags include the equivalent [!DNL Google Campaign Manager 360] macro `%esid!` |
| `${TM_PLACEMENT_ID_NUM}` | Tracks and reports the placement ID from the DSP | Yes | No, but tags include the equivalent [!DNL Google Campaign Manager 360] macro `%epid!` |
| `${TM_AD_ID_NUM}` | Tracks and reports the ad ID from the DSP | Yes | No, but tags include the equivalent [!DNL Google Campaign Manager 360] macro `%eaid!` |
| `${TM_CREATIVE_ID_NUM}` | Tracks and reports the creative ID from the DSP | N/A | No, but tags include the equivalent [!DNL Google Campaign Manager 360] macro `%ecid!` |
| `${TM_SESSION_ID}` | Tracks and reports the impression ID from the DSP. If a value isn't returned, Advertising Creative generates one. | Yes | &mdash; |
| `${TM_ACC_EXPERIENCE_ID}` | Tracks and reports the Advertising Creative experience ID | &mdash; | &mdash; |
| `${TM_ACC_CREATIVE_ID}` | Tracks and reports the Advertising Creative creative ID | &mdash; | &mdash; |
| `${TM_RANDOM}` | A random number between 1 and 1000000 | &mdash; | &mdash; |
| `${TM_TIMESTAMP}` | The Unix Timestamp (in seconds) | &mdash; | &mdash; |
| `${TM_CLICK_URL_URLENC}` | (For third-party ads from vendors who require URL encoding) The encoded click redirect URL, which enables ad servers to track and count ad clicks. When the ad is served and the user clicks on it, the macro is activated, and the click is recorded and counted for reporting purposes. | Yes | &mdash; |
| `${TC_1}` | Custom tracking code 1. | &mdash; | &mdash; |
| `${TC_2}` | Custom tracking code 2. | &mdash; | &mdash; |
| `${TC_3}` | Custom tracking code 3. | &mdash; | &mdash; |
| `${TC_4}` | Custom tracking code 4. | &mdash; | &mdash; |
| `${TC_5}` | Custom tracking code 5. | &mdash; | &mdash; |
| `${GDPR_ENFORCED}` | Whether GDPR enforcement is required for the bid request. Values: **1** = GDPR should be enforced, **0** = GDPR should not be enforced. | &mdash; | &mdash; |
| `${GDPR_CONSENT}` | The GDPR consent value received from the supply partner in the bid request. Typically: **1** = consent provided, **0** = no consent provided. | &mdash; | &mdash; |
-->

| 매크로 | 설명 | Advertising DSP용 경험 태그에서 자동으로 사용하시겠습니까? |
| --- | --- | --- |
| `${TM_CAMPAIGN_ID_NUM}` | DSP에서 캠페인 ID를 추적하고 보고합니다. | 예 |
| `${TM_SITE_ID_NUM}` | DSP에서 사이트 ID를 추적하고 보고합니다. | 예 |
| `${TM_PLACEMENT_ID_NUM}` | DSP에서 배치 ID를 추적하고 보고합니다 | 예 |
| `${TM_AD_ID_NUM}` | DSP에서 광고 ID를 추적하고 보고합니다. | 예 |
| `${TM_CREATIVE_ID_NUM}` | DSP에서 크리에이티브 ID를 추적하고 보고합니다. | 해당 사항 없음 |
| `${TM_SESSION_ID}` | 광고 요청과 연결된 세션 ID를 추적하고 보고합니다. 값이 반환되지 않으면 Advertising Creative에서 값을 생성합니다. | 예 |
| `${TM_ACC_EXPERIENCE_ID}` | Advertising Creative 경험 ID를 추적하고 보고합니다. | — |
| `${TM_ACC_CREATIVE_ID}` | Advertising Creative Creative ID를 추적하고 보고합니다 | — |
| `${TM_RANDOM}` | 1에서 1,000,000 사이의 임의로 생성된 숫자. 일반적으로 캐시 무효화에 사용됩니다. | — |
| `${TM_TIMESTAMP}` | UNIX® 타임스탬프(초) | — |
| `${TM_CLICK_URL_URLENC}` | (URL 인코딩이 필요한 공급업체의 서드파티 광고) 광고 서버가 광고 클릭을 추적하고 계산할 수 있도록 인코딩된 클릭 리디렉션 URL입니다. 사용자가 광고를 클릭하면 매크로가 활성화되고 클릭이 기록 및 보고용으로 카운트됩니다. | 예 |
| `${TC_1}` | 사용자 지정 추적 코드 1. | — |
| `${TC_2}` | 사용자 지정 추적 코드 2. | — |
| `${TC_3}` | 사용자 지정 추적 코드 3. | — |
| `${TC_4}` | 사용자 지정 추적 코드 4. | — |
| `${TC_5}` | 사용자 지정 추적 코드 5. | — |
| `${GDPR_ENFORCED}` | 입찰 요청에 GDPR 시행이 필요한지 여부. 값: **1** = GDPR은 적용되어야 하며 **0** = GDPR은 적용되지 않아야 합니다. | — |
| `${GDPR_CONSENT}` | 입찰 요청에서 공급 파트너로부터 받은 GDPR 동의 값. 일반적으로: **1** = 제공된 동의, **0** = 제공된 동의 없음. | — |

>[!MORELIKETHIS]
>
>* [Creative 라이브러리에 표준 크리에이티브 추가](/help/creative/creative-libraries/creative-add-standard.md#creative-add-third-party)
>* [표준 크리에이티브 설정](/help/creative/creative-libraries/creative-settings-standard.md#creative-settings-third-party)
>* &lbrack;타깃팅된 경험 설정*[타깃팅되지 않은 경험 설정](/help/creative/experiences/experience-settings-no-targeting.md)
