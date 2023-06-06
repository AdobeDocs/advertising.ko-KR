---
title: 동기화 기본 정보 [!DNL Google Analytics] 전환 지표
description: 동기화에 대해 알아보기 [!DNL Google Analytics] 최적화 및 보고를 위한 전환 지표.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 0%

---

# 동기화 기본 정보 [!DNL Google Analytics] 전환 지표

Search, Social 및 Commerce는 특정 항목에 대한 전환 지표를 동기화할 수 있습니다. [!DNL Google Analytics] 최적화 및 보고를 위한 계정, 속성 및 보기 조합. [페이지 보기 수](https://ga-dev-tools.google/dimensions-metrics-explorer/#view=detail&amp;group=page_tracking&amp;jump=ga_pageviews), [세션](https://ga-dev-tools.google/dimensions-metrics-explorer/#view=detail&amp;group=session&amp;jump=ga_sessions), [바운스 비율](https://ga-dev-tools.google/dimensions-metrics-explorer/#view=detail&amp;group=session&amp;jump=ga_bouncerate) (바운스/세션으로 계산됨) 및 [세션 기간](https://ga-dev-tools.google/dimensions-metrics-explorer/#view=detail&amp;group=session&amp;jump=ga_sessionduration) 자동으로 포함됩니다. 데이터 소스당 최대 16개의 추가 지표를 포함할 수 있습니다.

>[!NOTE]
>
>Advertising DSP 사용자는 전환 지표를 사용자 지정 목표 및 보고서로 사용할 수 있습니다.

데이터 전송을 위한 모든 API 사용은 적용 가능한 프로젝트에 평가됩니다 [!DNL Google Analytics] 계정입니다. 다음에서 이 프로젝트에 대한 할당량을 볼 수 있습니다. [다음 [!DNL Google API Console]](https://console.developers.google.com/apis/api/analytics-json.googleapis.com/quotas). 다음을 참조하십시오 [!DNL Google Analytics] 에 대한 자세한 내용은 설명서 를 참조하십시오. [보고 API 요청에 대한 할당량 및 호출 제한](https://developers.google.com/analytics/devguides/reporting/core/v4/limits-quotas).

다음 절차에서는 변환 데이터를 동기화하는 프로세스에 대해 간략히 설명합니다 [!DNL Google Analytics].

1. [전제 조건 작업 수행](data-source-prerequisites.md)

   * Adobe 광고 토큰 구현(`ef_id` 쿼리 문자열 매개 변수)를 사용하십시오.

   * Adobe 광고 토큰(`ef_id` 쿼리 문자열 매개 변수) [!DNL Custom Dimension] 위치: [!DNL Google Analytics].

1. (에이전시 계정 관리자, 에이전시 계정 관리자, [!DNL Adobe] 계정 관리자 및 관리자 전용) [당 하나의 데이터 소스 만들기 [!DNL Google Analytics] 계정, 속성 및 보기 조합](data-source-configure.md).

   단일 속성에 대해 여러 속성 또는 여러 보기의 지표를 통합하려면 각각에 대해 별도의 데이터 소스를 설정합니다.

   데이터 소스가 구성되면 검색, 소셜 및 상거래는 광고주의 시간대에서 05:00부터 시작하여 매일 데이터를 가져옵니다. 지표를 사용할 수 있게 되면 캠페인 및 포트폴리오 관리 보기와 보고서에 지표를 포함할 수 있으며, 필요에 따라 최적화 목표에 사용할 수 있습니다.

>[!MORELIKETHIS]
>
>* [구성 사전 요구 사항 [!DNL Google Analytics] 데이터 소스](data-source-prerequisites.md)
>* [구성 [!DNL Google Analytics] 데이터 소스로 보기](data-source-configure.md)
>* [편집 [!DNL Google Analytics] 데이터 소스](data-source-edit.md)
>* [데이터 소스 동기화 일시 중지](data-source-pause.md)
>* [재인증 [!DNL Google Analytics] 데이터 소스](data-source-reauthenticate.md)
>* [[!DNL Google Analytics] 데이터 소스 설정](data-source-settings.md)
>* [부록 - 사용 가능 [!DNL Google Analytics] 지표](data-source-ga-metrics.md)

