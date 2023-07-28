---
title: Adobe Advertising 전환 추적 태그 기본 정보
description: Adobe Advertising 전환 추적 태그 사용에 대해 알아봅니다.
exl-id: 07403d60-6db2-47e7-977b-4b59c8797c3d
feature: Search Tracking
source-git-commit: 052574217d7ddafb8895c74094da5997b5ff83db
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Adobe Advertising 전환 추적 태그 기본 정보

Adobe Advertising은 &quot;성공&quot; 페이지처럼 전환 이벤트가 발생할 때 열리는 웹 페이지에 삽입된 Adobe Advertising 전환 추적 태그를 사용하여 광고 클릭으로 인한 전환을 추적합니다. 태그에는 트랜잭션 데이터를 사용자의 Adobe Advertising 쿠키와 함께 추적 서버로 전송하기 위한 임베드된 정보가 포함되어 있습니다. 추적 서버에서 트랜잭션은 적절한 광고 클릭 또는 노출(광고주의 전환 속성 설정에 따라)로 크레딧됩니다.

>[!NOTE]
>
>사용자에게 유효한 쿠키가 없는 경우 Adobe Advertising은 전환을 보고하지 않습니다.

추적할 각 전환 지표 세트에 대해 별도의 전환 태그를 만들어야 합니다. 각 태그를 삽입할 웹 페이지 목록을 광고주 또는 에이전시에 제공합니다. 다음 유형의 전환 태그를 생성할 수 있습니다. 를 참조하십시오.[Adobe Advertising 변환 태그 생성](/help/search-social-commerce/tools/conversion-tag-generate.md)지침:

* (권장) 웹 페이지에 표시되지 않는 JavaScript 태그(버전 3 또는 버전 2)입니다.

* HTML 이미지 태그를 사용하여 최종 사용자가 볼 수 없는 1픽셀 x 1픽셀 투명 이미지(픽셀)를 웹 페이지에 표시합니다. 회사에 JavaScript 태그 사용에 대한 정책이 있는 경우에만 이미지 태그를 사용하십시오.

태그 유형 간의 차이에 대한 자세한 내용은 &quot;[Advertising Cloud 전환 추적 태그에 대한 FAQ](/help/search-social-commerce/tracking/faqs-conversion-page-view-tracking-tags.md).&quot;

>[!NOTE]
>
>* 이 기능은 광고주의 웹 페이지에 이미지 태그나 JavaScript 태그를 추가하지 않습니다. 태그는 웹 페이지를 업데이트하기 위한 광고주의 일반적인 절차에 따라 추가해야 합니다.
>* 태그를 구현하는 데 걸리는 시간을 고려해야 합니다. 회사의 정책에 따라 구현에는 몇 주 또는 심지어 몇 달이 걸릴 수 있습니다.

## Adobe Advertising 전환 추적 태그의 기능

Adobe Advertising은 전환 추적 픽셀을 통해 다음 작업을 수행할 수 있습니다.

* 검색 캠페인에 대한 키워드 수준에서 전환 데이터를 추적하고 보고합니다.

* 모든 마케팅 채널(유료 검색 및 디스플레이)에서 광고(크리에이티브) 수준에서 전환 데이터를 추적 및 보고하여 크리에이티브 테스트를 용이하게 할 수 있습니다.

* 모든 마케팅 채널에서 거래 수준에서 전환 데이터를 추적하고 보고합니다.

* 가장 효과적인 마케팅 채널을 확인할 수 있도록 전환이 배포되는 방식을 보여 줍니다.

* 서로 다른 속성 수준(예: 마지막 관련 이벤트에 대한 속성 전환 또는 모든 이벤트에 균등하게 가중치 적용)에서 보고하고 최적화합니다.

* 클릭 지원(전환 단계에 기여한 검색 키워드 또는 배치)과 채널 지원(전환 단계에 기여한 사용자 이벤트, 가능하면 여러 마케팅 채널에서)에 대한 가시성을 제공합니다.

* 사이트 트래픽 및 전환의 지리적 분포 및 참조 도메인에 대한 가시성을 제공하여 지리적 및 웹 사이트 타겟팅을 세분화할 수 있습니다.

* 전환율을 향상시키는 데 사용할 수 있는 요일 또는 당일 트렌드를 분석합니다.

>[!MORELIKETHIS]
>
>* [전환 추적 옵션](conversion-tracking-about.md)
>* [Adobe Advertising 변환 태그 생성](/help/search-social-commerce/tools/conversion-tag-generate.md)
>* [JavaScript 전환 추적 태그 버전 3의 형식](format-conversion-tag-jsv3.md)
>* [JavaScript 전환 추적 태그 버전 2의 형식](format-conversion-tag-jsv2.md)
>* [이미지 변환 추적 태그의 형식](format-conversion-tag-image.md)
>* [전환 및 페이지 보기 추적 태그에 대한 FAQ](faqs-conversion-page-view-tracking-tags.md)
>* [Adobe Advertising JavaScript 전환 매핑 태그](/help/search-social-commerce/tracking/itp-conversion-mapping-tag.md)
