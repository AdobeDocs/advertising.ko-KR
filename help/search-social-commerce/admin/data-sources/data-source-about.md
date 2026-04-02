---
title: ' [!DNL Google Analytics] 전환 지표 동기화 정보'
description: 최적화 및 보고를 위한  [!DNL Google Analytics] 전환 지표 동기화에 대해 알아봅니다.
role: User, Admin
exl-id: 32d0ba22-5c27-4f50-9886-1c09d2da952c
feature: Search Admin, Search Data Sources
TQID: https://experienceleague.adobe.com/dN7AVijGEiKM1o2iu3Fcb2D61pFkTguFOOu0qIe-mZk
product_v2: id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2: id: e55292b5-d4a1-4c98-9c20-2a2c5bea07fbid: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
subfeature_v2: id: e778848d-90fa-4520-b80f-e8dd7dfdcffc
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
source-git-commit: 527ca2bb74de388c13ba1ce5bde3f8be1cead8d0
workflow-type: tm+mt
source-wordcount: 289
ht-degree: 0%

---

# [!DNL Google Analytics] 전환 지표 동기화 정보

Search, Social 및 Commerce은 최적화 및 보고를 위해 특정 [!DNL Google Analytics] 계정, 속성 및 보기 조합에 대한 전환 지표를 동기화할 수 있습니다. [페이지 보기 수](https://ga-dev-tools.google/dimensions-metrics-explorer/#view=detail&group=page_tracking&jump=ga_pageviews), [세션 수](https://ga-dev-tools.google/dimensions-metrics-explorer/#view=detail&group=session&jump=ga_sessions), [바운스 비율](https://ga-dev-tools.google/dimensions-metrics-explorer/#view=detail&group=session&jump=ga_bouncerate)&#x200B;(바운스 수/세션으로 계산됨) 및 [세션 기간](https://ga-dev-tools.google/dimensions-metrics-explorer/#view=detail&group=session&jump=ga_sessionduration)이 자동으로 포함됩니다. 데이터 소스당 최대 16개의 추가 지표를 포함할 수 있습니다.

>[!NOTE]
>
>Advertising DSP 사용자는 전환 지표를 사용자 지정 목표 및 보고서로 사용할 수 있습니다.

데이터 전송에 대한 모든 API 사용은 적용 가능한 [!DNL Google Analytics] 계정의 프로젝트에 평가됩니다. [다음 [!DNL Google API Console]](https://console.developers.google.com/apis/api/analytics-json.googleapis.com/quotas)에서 이 프로젝트에 대한 할당량을 볼 수 있습니다. [!DNL Google Analytics]보고 API 요청에 대한 할당량 및 호출 제한에 대한 자세한 내용은 [ 설명서를 참조하십시오](https://developers.google.com/analytics/devguides/reporting/core/v4/limits-quotas).

다음 단계에서는 [!DNL Google Analytics]에서 변환 데이터를 동기화하는 프로세스에 대해 간략히 설명합니다.

1. [전제 조건 작업 수행](data-source-prerequisites.md)

   * 적용 가능한 모든 광고 계정에 대해 랜딩 페이지 URL에서 Adobe Advertising 토큰(`ef_id` 쿼리 문자열 매개 변수)을 구현합니다.

   * `ef_id`의 [!DNL Custom Dimension]에서 Adobe Advertising 토큰([!DNL Google Analytics] 쿼리 문자열 매개 변수)을 캡처합니다.

1. (에이전시 계정 관리자, 에이전시 계정 관리자, [!DNL Adobe] 계정 관리자 및 관리자 사용자만 해당) [계정, 속성 및 보기 조합당 하나의 데이터 소스를 만듭니다 [!DNL Google Analytics] .](data-source-configure.md)

   단일 속성에 대해 여러 속성 또는 여러 보기의 지표를 통합하려면 각각에 대해 별도의 데이터 소스를 설정합니다.

   데이터 소스가 구성되면 검색, 소셜 및 Commerce은 광고주의 시간대의 05:00부터 매일 데이터를 가져옵니다. 지표를 사용할 수 있게 되면 캠페인 및 포트폴리오 관리 보기와 보고서에 지표를 포함할 수 있으며, 필요에 따라 최적화 목표에 사용할 수 있습니다.

>[!MORELIKETHIS]
>
>* [데이터 원본 [!DNL Google Analytics] 구성을 위한 필수 구성 요소](data-source-prerequisites.md)
>* [데이터 소스로  [!DNL Google Analytics] 보기 구성](data-source-configure.md)
>* [데이터 원본 편집 [!DNL Google Analytics] 2}](data-source-edit.md)
>* [데이터 원본 동기화 일시 중지](data-source-pause.md)
>* [데이터 원본 다시 인증 [!DNL Google Analytics] 2}](data-source-reauthenticate.md)
>* [[!DNL Google Analytics] 데이터 원본 설정](data-source-settings.md)
>* [부록 - 사용 가능 [!DNL Google Analytics] 지표](data-source-ga-metrics.md)
