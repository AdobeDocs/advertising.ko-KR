---
title: 추적 URL에 사용 가능한 매크로
description: 랜딩 페이지 URL 추적 URL 및 서드파티 크리에이티브에 추가할 수 있는 매크로를 참조합니다.
feature: Creative Experiences, Creative Experiences
source-git-commit: fd925c641bef7953aea50813725252c3913757fa
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# 추적 URL에 사용 가능한 매크로

*베타가 닫힘*

<!-- More feature metadata??? -->

서드파티 크리에이티브, 경험에 대한 서드파티 추적 URL 및 자체 사용을 위한 랜딩 페이지 URL에 다음 매크로를 포함할 수 있습니다.

사용 가능한 매크로 중 일부 또는 이와 동등한 매크로는 경험 태그에 자동으로 포함됩니다.

<!-- Later: 

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

-->

| 매크로 | 설명 | Advertising DSP용 경험 태그에서 자동으로 사용하시겠습니까? |
| --- | --- | --- | --- |
| `${TM_CAMPAIGN_ID_NUM}` | DSP에서 캠페인 ID를 추적하고 보고합니다. | 예 |
| `${TM_SITE_ID_NUM}` | DSP에서 사이트 ID를 추적하고 보고합니다. | 예 |
| `${TM_PLACEMENT_ID_NUM}` | DSP에서 배치 ID를 추적하고 보고합니다. | 예 |
| `${TM_AD_ID_NUM}` | DSP에서 광고 ID를 추적하고 보고합니다. | 예 |
| `${TM_CREATIVE_ID_NUM}` | DSP에서 Creative ID를 추적하고 보고합니다. | 해당 사항 없음 |
| `${TM_SESSION_ID}` | DSP의 노출 ID를 추적하고 보고합니다. 값이 반환되지 않으면 Advertising Creative에서 값을 생성합니다. | 예 |
| `${TM_ACC_EXPERIENCE_ID}` | Advertising Creative 경험 ID를 추적하고 보고합니다. | — |
| `${TM_ACC_CREATIVE_ID}` | Advertising Creative 크리에이티브 ID를 추적하고 보고합니다. | — |
| `${TM_RANDOM}` | 1과 1000000 사이의 난수 | — |
| `${TM_TIMESTAMP}` | Unix 타임스탬프(초) | — |
| `${TM_CLICK_URL_URLENC}` | (URL 인코딩이 필요한 공급업체의 서드파티 광고) 광고 서버가 광고 클릭을 추적하고 계산할 수 있도록 인코딩된 클릭 리디렉션 URL입니다. 광고가 게재되고 사용자가 해당 광고를 클릭하면 매크로가 활성화되고 클릭이 보고용으로 기록 및 카운트됩니다. | 예 |

>[!MORELIKETHIS]
>
>* 
>* 
