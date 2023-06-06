---
title: 구성 사전 요구 사항 [!DNL Google Analytics] 데이터 소스
description: 를 구성하기 전에 완료해야 하는 단계에 대해 알아봅니다. [!DNL Google Analytics] 데이터 소스.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---

# 구성 사전 요구 사항 [!DNL Google Analytics] 데이터 소스

을(를) 설정하기 전에 [!DNL Google Analytics] 데이터 소스에서는 데이터를 전달할 기본 키로 Search, Social, &amp; Commerce 쿼리 문자열 매개 변수 &quot;ef_id&quot;를 설정해야 합니다 [!DNL Google Analytics] 검색, 소셜 및 상거래에 사용됩니다. 각각에 대한 기본 키 설정 [!DNL Google Analytics] 데이터를 동기화할 계정 및 속성 조합입니다. 조직의 다른 사용자가 이러한 작업을 완료해야 할 수 있습니다. 자세한 내용은 아래를 참조하십시오.

광고 또는 키워드의 랜딩 페이지 URL에 검색, 소셜 및 상거래 리디렉션이 포함되어 있지 않은 경우, 먼저 추가한 것입니다.

## 전제 조건 1: 적용 가능한 모든 광고 계정에 대한 랜딩 페이지 URL에서 검색, 소셜 및 상거래 토큰(&quot;ef_id&quot; 쿼리 문자열 매개 변수)을 구현합니다

유료 검색 시마다 관련 캠페인에 대해 고유한 을 클릭합니다 `ef_id` 을 생성하고 쿼리 문자열로 랜딩 페이지 URL에 추가해야 합니다. 예: `https://www.adobe.com?someParam=123&ef_id=abcde:123456789:s`, 여기서 `&ef_id=abcde:123456789:s` 는 추가 기호, `ef_id` 키 및 `ef_id` 값. ef_id를 포함하려면 관련 광고 네트워크 계정 및 캠페인에 [!UICONTROL Tracking Type] &quot;[!UICONTROL EF Redirect]&quot; 및 [!UICONTROL Redirect Type] &quot;[!UICONTROL Token].&quot;

기존 계정 및 캠페인의 경우 ef_id가 이미 구현되었을 수 있습니다.

ef_id가 포함되지 않은 경우 Adobe 계정 팀에 도움을 요청하십시오.

모든 전제 조건이 완료되면 `ef_id` 는 데이터를 전달할 기본 키로 사용됩니다. [!DNL Google Analytics] 검색, 소셜 및 상거래에 사용됩니다.

## 사전 요구 사항 2: 각 관련 항목에 대한 사용자 지정 차원에서 검색, 소셜 및 상거래 토큰(&quot;ef_id&quot; 쿼리 문자열 매개 변수)을 캡처합니다. [!DNL Google Analytics] 속성

각각에 대해 다음 작업을 반복합니다 [!DNL Google Analytics] 데이터를 동기화할 계정 및 속성 조합입니다. 다음을 참조하십시오 [[!DNL Google Analytics] 사용자 지정 차원 생성 및 구현에 대한 설명서](https://support.google.com/analytics/answer/2709829?hl=en#zippy=%2Cin-this-article) 을 참조하십시오.

1. 위치 [!DNL Google Analytics], 이름이 인 사용자 지정 차원 만들기`ef_id`&quot;. 차원 범위를 다음으로 설정 [!DNL User]을 누르고 차원을 활성으로 설정합니다.

   >[!NOTE]
   >
   >이 전제 조건을 사용하려면 관련 속성에 대한 편집 권한이 필요합니다.

1. 업데이트 [!DNL Google Analytics] 추적 코드 : 랜딩 페이지 URL에 있는 ef_id 쿼리 문자열 매개 변수의 값을 캡처하여 ef_id 사용자 지정 차원에 저장합니다.

   >[!NOTE]
   >
   >ef_id는 랜딩 페이지 URL에만 있어야 합니다.

   예를 들어 랜딩 페이지 URL이 `https://www.adobe.com?someParam=123&ef_id=abcde:123456789:s&anotherParam=asdf`를 누르고 ef_id 차원의 값을 [!DNL Google Analytics] 은(는) `abcde:123456789:s`.

   >[!NOTE]
   >
   >이 전제 조건은 자격을 갖춘 개발자가 완료해야 합니다.

>[!MORELIKETHIS]
>
>* [동기화 기본 정보 [!DNL Google Analytics] 전환 지표](data-source-about.md)
>* [구성 [!DNL Google Analytics] 데이터 소스로 보기](data-source-configure.md)
>* [편집 [!DNL Google Analytics] 데이터 소스](data-source-edit.md)
>* [데이터 소스 동기화 일시 중지](data-source-pause.md)
>* [재인증 [!DNL Google Analytics] 데이터 소스](data-source-reauthenticate.md)
>* [[!DNL Google Analytics] 데이터 소스 설정](data-source-settings.md)
>* [부록 - 사용 가능 [!DNL Google Analytics] 지표](data-source-ga-metrics.md)

