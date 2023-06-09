---
title: EF ID 피드를 사용한 전환 추적
description: 전환 추적 데이터에 EF ID 피드를 사용하는 방법에 대해 알아봅니다.
source-git-commit: 46e918418bf2e5c412efa8825dda22bc1953e439
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# EF ID 피드를 사용한 전환 추적

이 메서드에서 Advertising Cloud은 `ef_id` 사용자가 및 광고를 클릭하여 랜딩 페이지에 도달하고 광고주가 `ef_id` 값을 전환 데이터와 함께 지정하고 데이터 피드에 전송합니다.

## 구현 개요

*에이전시 계정 관리자, [!DNL Adobe] 계정 관리자 및 관리자 역할만*

1. 계정 또는 캠페인 추적 옵션 사용[!UICONTROL EF Redirect],&quot; 의 리디렉션 유형[!UICONTROL Token]및 &quot;[!UICONTROL Auto Upload]계정이나 캠페인의 각 키워드(키워드 수준 추적용) 또는 광고(광고 수준 추적용)에 대해 Adobe Advertising 토큰(ef_id)을 사용하여 대상 URL 또는 최종 URL을 자동으로 생성합니다.

   >[!NOTE]
   >* 이 메서드는 광고주가 Adobe Advertising 전환 추적 태그를 사용할 필요가 없습니다.
   >* 기존 계정 또는 캠페인에 대한 리디렉션 유형을에서 전환하는 경우 [!UICONTROL Standard] 끝 [!UICONTROL Token]또는 그 반대로 적용 가능한 모든 추적 URL을 다시 생성해야 합니다.

   ef_id는 최종 사용자가 광고를 클릭하여 Adobe Advertising 서버로 리디렉션될 때 채워져 랜딩 페이지 URL에 추가됩니다. 그런 다음 ef_id가 광고 또는 키워드의 대상 URL 또는 최종 URL에서 광고주에게 전달됩니다. 다음은 리디렉션 중에 광고주에게 전달되는 대상 URL의 예입니다.

   `http://pixel.everesttech.net/1180/cq?ev_sid=3&ev_ln={keyword}&ev_crx={creative}&ev_mt={matchtype}&ev_n={network}&ev_ltx=&ev_pl={placement}&url=http%3A//www.example.com&ef_id=D59Nu0u@BD0AAM1q:20110630172936:s`

1. 광고주는 리디렉션에서 ef_id를 추출하여 관련 전환 데이터와 함께 피드 파일에 포함합니다. ef_id를 변경하거나 대/소문자를 변경하지 마십시오.

1. (선택 사항이지만 권장됨) 광고주는 피드 파일에 포함할 각 트랜잭션에 대해 고유한 트랜잭션 ID를 만들 수 있습니다.

1. 광고주가 [필수 전환 데이터](/help/search-social-commerce/tracking/feed-ef-id-data-requirements.md) 지정된 서버 위치로 이동합니다.

1. 기술 서비스는 업로드된 파일의 변환 데이터를 구문 분석한 다음 데이터를 Adobe Advertising으로 업로드합니다. 그런 다음 Adobe Advertising은 개별 키워드, 광고 및 배치에 대해 데이터를 추적하고 각각에 대한 매출 예측을 만듭니다.

1. 기술 서비스는 피드 데이터에 대해 처리된 데이터의 유효성을 검사하고 [고립 트랜잭션](/help/search-social-commerce/glossary.md#o-p).

>[!MORELIKETHIS]
>
>* [변환 피드 파일에 대한 파일 요구 사항](feed-file-requirements.md)
>* [EF ID를 사용한 데이터 피드에 대한 데이터 요구 사항](/help/search-social-commerce/tracking/feed-ef-id-data-requirements.md)


