---
title: Customer Journey Analytics의 Adobe Advertising 지표 및 차원
description: Customer Journey Analytics에서 사용할 수 있는 Adobe Advertising 지표 및 차원을 참조하십시오.
feature: Integration with Adobe Customer Journey Analytics
source-git-commit: c3836d8af50061701434790b2bd9214df29e8a01
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# Customer Journey Analytics의 Adobe Advertising 지표 및 차원

*Adobe Advertising-Customer Journey Analytics 통합만 있는 광고주*

Adobe Advertising은 트래픽 지표 및 차원을 매일 [!DNL Customer Journey Analytics]에 전달합니다. [!DNL Web SDK]에서 Adobe Advertising 클릭스루 및 뷰스루를 실시간으로 캡처하여 Customer Journey Analytics에 전달합니다.

## Adobe Advertising 트래픽 지표

<!-- Verify column names -->

>[!NOTE]
>
>* &quot;XDM 필드 이름&quot;은 Adobe Experience Platform의 필드 이름입니다.
>* &quot;XDM 필드 표시 이름&quot;은 Customer Journey Analytics 내의 표시 이름을 나타냅니다.

| Adobe Advertising 필드 이름 | XDM 필드 이름 | XDM 필드 표시 이름 | Source |
|------------------------------|----------------|------------------------|--------|
| 날짜 | 날짜 | 모두 | |
| AMO ID | skwcid | ADOBE ADVERTISING ID | 모두 |
| AMO 노출 횟수 | adobe_advertising_impressions | Adobe Advertising 노출 횟수 | 모두 |
| AMO 클릭수 | adobe_advertising_clicks | Adobe Advertising 클릭 수 | 모두 |
| AMO 비용 | adobe_advertising_cost | Adobe Advertising 비용 | 모두 |
| 통화 코드 | 통화 | 통화 | 모두 |
| AMO 보기 | adobe_advertising_views | Adobe Advertising 보기 | Ad Cloud DSP |
| AMO 조회수: 25% 완료 | adobe_advertising_views_25_pct | Adobe Advertising 조회수 25% 완료 | Ad Cloud DSP |
| AMO 조회수: 50% 완료 | adobe_advertising_views_50_pct | Adobe Advertising 조회수 50% 완료 | Ad Cloud DSP |
| AMO 조회수: 75% 완료 | adobe_advertising_views_75_pct | Adobe Advertising 조회수 75% 완료 | Ad Cloud DSP |
| AMO 뷰 100% 완료 | adobe_advertising_views_100_pct | Adobe Advertising 보기 100% 완료 | Ad Cloud DSP |
| AMO 시간(분) 조회함 | adobe_advertising_minutes_viewed | Adobe Advertising 조회수(분) | Ad Cloud DSP |
| AMO 조회 가능 노출 횟수 | adobe_advertising_viewable_impressions | Adobe Advertising 조회 가능 노출 횟수 | Ad Cloud DSP |
| AMO 볼 수 없는 노출 횟수 | adobe_advertising_not_viewable_impressions | Adobe Advertising 조회 불가 노출 횟수 | Ad Cloud DSP |
| AMO 측정 가능한 노출 횟수 | adobe_advertising_measureable_impressions | Adobe Advertising 측정 가능한 노출 횟수 | Ad Cloud DSP |

<!--
| Adobe Advertising Landing Page Views | adobe_advertising_landing_page_views | Adobe Advertising Landing Page Views | Meta Only |
| Adobe Advertising App Events | adobe_advertising_app_events | Adobe Advertising App Events | Meta Only |
| Adobe Advertising Engagements | adobe_advertising_engagements | Adobe Advertising Engagements | Meta Only |
| Adobe Advertising Ad Platform Conversions | adobe_advertising_ad_platform_conversions | Adobe Advertising Ad Platform Conversions | Meta Only |
| Adobe Advertising App Installs | adobe_advertising_app_installs | Adobe Advertising App Installs | Meta Only |
| Adobe Advertising Ad Platform Conversion Value | adobe_advertising_ad_platform_conversion_value | Adobe Advertising Ad Platform Conversion Value | Meta Only |
| Adobe Advertising Ad Platform Leads | adobe_advertising_ad_platform_leads | Adobe Advertising Ad Platform Leads | Meta Only |
| Adobe Advertising Page Like | adobe_advertising_page_like | Adobe Advertising Page Like | Meta Only |
| Adobe Advertising Phone Calls | adobe_advertising_phone_calls | Adobe Advertising Phone Calls | Meta Only |
| Adobe Advertising Messages | adobe_advertising_messages | Adobe Advertising Messages | Meta Only |
-->

## Adobe Advertising 차원

>[!NOTE]
>
>* &quot;XDM 필드&quot;는 Adobe Experience Platform의 필드 이름입니다.
>* &quot;XDM 필드 표시 이름&quot;은 Customer Journey Analytics 내의 표시 이름을 나타냅니다.

| Adobe Advertising 필드 이름 | XDM 필드 이름 | XDM 필드 표시 이름 | Source |
|------------------------------|----------------|------------------------|--------|
| 키 | skwcid | ADOBE ADVERTISING ID |
| 광고 플랫폼 | adobe_advertising_ad_platform | Adobe Advertising 광고 플랫폼 |
| 계정 | adobe_advertising_account | Adobe Advertising 계정 |
| 캠페인 | adobe_advertising_campaign | Adobe Advertising 캠페인 |
| 광고 그룹 | adobe_advertising_ad_group | Adobe Advertising 광고 그룹 |
| 키워드 | adobe_advertising_키워드 | Adobe Advertising 키워드 |
| 광고 | adobe_advertising_ad | Adobe Advertising 광고 |
| 배치 | adobe_advertising_placement | Adobe Advertising 배치 |
| 일치 유형 | adobe_advertising_match_type | Adobe Advertising 일치 유형 |
| 광고 제목 | adobe_advertising_ad_title | Adobe Advertising 광고 제목 |
| 광고 설명 | adobe_advertising_ad_description | Adobe Advertising 광고 설명 |
| 광고 대상 URL | adobe_advertising_ad_destination_url | Adobe Advertising 광고 대상 URL |
| 광고 표시 URL | adobe_advertising_ad_display_url | Adobe Advertising 광고 표시 URL |
| 장치 | adobe_advertising_device | Adobe Advertising 장치 |
| 키워드 일치 유형 | adobe_advertising_keyword_matchtype | Adobe Advertising 키워드 일치 유형 |
| 네트워크 | adobe_advertising_network | Adobe Advertising 네트워크 |
| 광고 유형 | adobe_advertising_ad_type | Adobe Advertising 광고 유형 |
| 제품 타겟 | adobe_advertising_product_target | Adobe Advertising 제품 타겟 |
| 랜딩 유형 | adobe_advertising_landing_type | Adobe Advertising 랜딩 유형 |
| 최적화 | adobe_advertising_optimization | Adobe Advertising 최적화 |

>[!MORELIKETHIS]
>
>* [개요](overview.md)
>* [필수 구성 요소](prerequisites.md)
>* [사용한 Adobe Advertising ID [!DNL Customer Journey Analytics]](ids.md)
