---
title: ' [!DNL Google Analytics] 데이터 원본을 구성하기 위한 필수 구성 요소'
description: ' [!DNL Google Analytics] 데이터 원본을 구성하기 전에 완료해야 하는 단계에 대해 알아봅니다.'
role: User, Admin
exl-id: 97b0c149-5f82-4a1e-a5d9-aeab43cbd88f
feature: Search Admin, Search Data Sources
source-git-commit: e16bc62127a708de8f4deb1eddfa53a14405cbc2
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# [!DNL Google Analytics] 데이터 원본을 구성하기 위한 필수 구성 요소

[!DNL Google Analytics] 데이터 소스를 설정하려면 먼저 Search, Social 및 Commerce 쿼리 문자열 매개 변수 &quot;ef_id&quot;를 기본 키로 설정하여 [!DNL Google Analytics]의 데이터를 Search, Social 및 Commerce에 전달해야 합니다. 데이터를 동기화할 각 [!DNL Google Analytics] 계정 및 속성 조합에 대한 기본 키를 설정합니다. 조직의 다른 사용자가 이러한 작업을 완료해야 할 수 있습니다. 자세한 내용은 아래를 참조하십시오.

광고 또는 키워드의 랜딩 페이지 URL에 검색, 소셜 및 Commerce 리디렉션이 포함되어 있지 않은 경우, 먼저 추가한 것입니다.

## 전제 조건 1: 적용 가능한 모든 광고 계정에 대해 랜딩 페이지 URL에서 검색, 소셜 및 Commerce 토큰(&quot;ef_id&quot; 쿼리 문자열 매개 변수)을 구현합니다

관련 캠페인에 대한 유료 검색 클릭마다 고유한 `ef_id`을(를) 생성하고 `https://www.adobe.com?someParam=123&ef_id=abcde:123456789:s`과(와) 같은 쿼리 문자열로 랜딩 페이지 URL에 추가해야 합니다. 여기서 `&ef_id=abcde:123456789:s`은(는) 추가 기호, `ef_id` 키 및 `ef_id` 값입니다. ef_id를 포함하려면 관련 광고 네트워크 계정 및 캠페인에 [!UICONTROL Tracking Type] &quot;[!UICONTROL EF Redirect]&quot; 및 [!UICONTROL Redirect Type] &quot;[!UICONTROL Token]&quot;이(가) 있어야 합니다.

기존 계정 및 캠페인의 경우 ef_id가 이미 구현되었을 수 있습니다.

ef_id가 포함되지 않은 경우 Adobe 계정 팀에 도움을 요청하십시오.

모든 필수 구성 요소가 완료되면 `ef_id`이(가) 기본 키로 사용되어 [!DNL Google Analytics]에서 Search, Social 및 Commerce으로 데이터를 전달합니다.

## 전제 조건 2: 관련된 각 [!DNL Google Analytics] 속성에 대해 사용자 지정 차원에서 검색, 소셜 및 Commerce 토큰(&quot;ef_id&quot; 쿼리 문자열 매개 변수)을 캡처합니다.

데이터를 동기화할 각 [!DNL Google Analytics] 계정 및 속성 조합에 대해 다음 작업을 반복합니다. 이러한 작업에 대한 도움말은 [[!DNL Google Analytics] 사용자 지정 차원 만들기 및 구현에 대한 설명서](https://support.google.com/analytics/answer/2709829?hl=en#zippy=%2Cin-this-article)를 참조하십시오.

1. [!DNL Google Analytics]에서 &quot;`ef_id`&quot;(이)라는 사용자 지정 차원을 만듭니다. 차원의 범위를 [!DNL User](으)로 설정하고 차원을 활성으로 설정합니다.

   >[!NOTE]
   >
   >이 전제 조건을 사용하려면 관련 속성에 대한 편집 권한이 필요합니다.

1. [!DNL Google Analytics] 추적 코드를 업데이트하여 ef_id 쿼리 문자열 매개 변수가 랜딩 페이지 URL에 있을 때 이 매개 변수의 값을 캡처하고 ef_id 사용자 지정 차원에 저장합니다.

   >[!NOTE]
   >
   >ef_id는 랜딩 페이지 URL에만 있어야 합니다.

   예를 들어 랜딩 페이지 URL이 `https://www.adobe.com?someParam=123&ef_id=abcde:123456789:s&anotherParam=asdf`이면 [!DNL Google Analytics]의 ef_id 차원 값은 `abcde:123456789:s`입니다.

   >[!NOTE]
   >
   >이 전제 조건은 자격을 갖춘 개발자가 완료해야 합니다.

>[!MORELIKETHIS]
>
>* [동기화 정보 [!DNL Google Analytics] 전환 지표](data-source-about.md)
>* [데이터 소스로  [!DNL Google Analytics] 보기 구성](data-source-configure.md)
>* [데이터 원본 편집 [!DNL Google Analytics] 2}](data-source-edit.md)
>* [데이터 원본 동기화 일시 중지](data-source-pause.md)
>* [데이터 원본 다시 인증 [!DNL Google Analytics] 2}](data-source-reauthenticate.md)
>* [[!DNL Google Analytics] 데이터 원본 설정](data-source-settings.md)
>* [부록 - 사용 가능 [!DNL Google Analytics] 지표](data-source-ga-metrics.md)
