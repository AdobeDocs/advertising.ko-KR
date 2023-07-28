---
title: Adobe Analytics 전환 추적
description: Adobe Advertising 캠페인에 Adobe Analytics 전환 추적을 사용하는 방법에 대해 알아봅니다.
exl-id: 0ed1d059-829a-4090-950d-41cbcc27b3ac
feature: Search Tracking
source-git-commit: 052574217d7ddafb8895c74094da5997b5ff83db
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# Adobe Analytics 전환 추적

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

Adobe Advertising-Adobe Analytics 통합을 사용하는 광고주의 경우 Advertising Cloud은 광고 클릭수 및 노출수를 이 추적한 사이트 참여 및 전환 지표와 연결할 수 있습니다. [!DNL Analytics] 토큰 ( )과 함께 리디렉션을 사용하는 경우`ef_id` 매개 변수)를 사용하십시오. [입찰 단위](/help/search-social-commerce/glossary.md#a-b). 다음 [!DNL Analytics] 데이터는 일별 피드 파일을 통해 Advertising Cloud으로 자동으로 전송됩니다.

를 참조하십시오.[개요 [!DNL Analytics for Advertising]](https://experienceleague.adobe.com/docs/advertising-cloud/dsp/integrations/analytics/overview.html){target="_blank"}통합에 대한 자세한 내용은 &quot;.

>[!PREREQUISITES]
>
> 검색, 소셜 및 상거래 광고주 계정의 시간대, [!DNL Analytics] 보고서 세트와 광고 네트워크 계정이 일치해야 합니다. 일치하지 않으면 데이터 분산이 시스템 간에 존재합니다.

## 구현 개요

1. 위치 [!DNL Analytics], 검색, 소셜 및 상거래 구현 팀이 각 보고서 세트에 대해 다음 구성 설정을 수정합니다.

   * 에 대한 만료 `ef_id` eVar이 Adobe Advertising에 대한 광고주의 클릭 전환 확인 기간과 일치하도록 변경되었습니다.

   * Adobe Advertising 사용자 ID입니다.

   * 최적화에 사용할 표준 및 사용자 지정 이벤트입니다.

1. 검색, 소셜 및 상거래에서 구현 팀은

   1. 기존 광고 네트워크 계정 계층을 검색, 소셜 및 상거래에 동기화합니다.

   1. &quot;&quot;로 리디렉션 추가`ef_id`&quot;토큰이 추적 URL로 전달되고 광고 네트워크에 게시됩니다.

   이 단계에서는 Adobe Advertising 추적 서버로 리디렉션을 추가합니다( [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 병렬 추적을 지원하고 광고 클릭 시 동적으로 채워진 &quot;ef_id&quot; 매개 변수를 URL에 추가하는 브라우저의 광고. 병렬 추적이 적용되면 최종 사용자가 광고에서 최종 URL로 직접 전송되고 추적 템플릿 URL(클릭 측정 포함)이 백그라운드로 로드됩니다.

통합이 완료되면 검색, 소셜 및 상거래에 추적된 모든 페이지 내 이벤트 데이터가 자동으로 수신됩니다. [!DNL Analytics] 구성된 보고서 세트용.

>[!MORELIKETHIS]
>
>* [전환 추적 옵션](conversion-tracking-about.md)
