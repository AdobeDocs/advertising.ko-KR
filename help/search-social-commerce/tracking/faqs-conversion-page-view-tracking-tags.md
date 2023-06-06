---
title: Adobe 광고 전환 및 페이지 보기 추적 태그에 대한 FAQ
description: Adobe 광고 전환 및 페이지 보기 추적 태그의 비교를 참조하십시오.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---

# Adobe 광고 전환 및 페이지 보기 추적 태그에 대한 FAQ

다음은 Adobe 광고 전환 추적 태그 및 페이지 보기 추적 태그에 적용됩니다.

|  | ECID가 있는 JS 태그 | JS 버전 3 태그 | JS 버전 2 태그 | 이미지 태그 |
| ---- | ---- | ---- | ---- | ---- |
| 다른 JS 버전과 동일한 웹 페이지에서 사용할 수 있습니다. | — | — | — | 해당 사항 없음 |
| 동일한 웹 페이지에서 동일한 광고주 사용자 ID로 여러 태그를 사용할 수 있습니다. | 예 | 예 | 예 | — |
| 동일한 웹 페이지에서 서로 다른 광고주 사용자 ID가 있는 여러 태그를 사용할 수 있습니다. | 예 | 예 | 아니요 | 아니요 |
| Adobe Experience Platform용 Adobe 광고 확장에서 사용하며, Experience Platform을 사용하여 생성된 다른 태그와 호환됩니다 | 예 | 예 | — | — |
| 에서 생성되는 모든 전환 허용 [!DNL Apple Safari] 및 [!DNL Mozilla Firefox] Adobe Advertising JavaScript 전환 매핑 태그와 함께 사용할 때 추적됩니다 | 예 | 예 | 예 | — |

<!-- add link to page on conversion mapping tag above? -->

>[!NOTE]
>
>* 모든 새 구현은 JavaScript 버전 3을 사용합니다.
>* ECID가 있는 JavaScript 태그는 [Adobe Experience Cloud ID(ECID) 서비스](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html) 기존 ef_id 및 gsurferid를 사용하여 전환을 측정할 수 있습니다. 이 최신 태그는 다음을 생성합니다. [자사 Experience Cloud s_ecid 쿠키](https://experienceleague.adobe.com/docs/core-services/interface/administration/ec-cookies/cookies-first-party.html) 및 는 다른 Experience Cloud 제품과의 긴밀한 통합을 제공합니다.
>* JavaScript 버전 2 태그가 광고주의 웹 페이지에 이미 구현된 경우에만 해당 태그를 사용합니다.
>* 가장 좋은 방법은 사이트에 이미지 태그 사용에 대한 정책이 없는 경우 이미지 태그 대신 JavaScript 태그를 사용하는 것입니다.
>* JavaScript 태그는 Adobe Experience Cloud에서 만들었거나 Adobe Audience Manager에서 만들었거나 Audience Manager 또는 Adobe Analytics에서 Adobe Experience Cloud에 게시한 대상을 타깃팅하려는 광고주에게 필요합니다.


>[!MORELIKETHIS]
>
>* [Adobe 광고 전환 추적 태그 정보](/help/search-social-commerce/tracking/conversion-tracking-advertising.md)
>* [Adobe 광고 전환 태그 생성](/help/search-social-commerce/tools/conversion-tag-generate.md)
>* [JavaScript 전환 추적 태그 버전 3의 형식](/help/search-social-commerce/tracking/format-conversion-tag-jsv3.md)
>* [JavaScript 전환 추적 태그 버전 2의 형식](/help/search-social-commerce/tracking/format-conversion-tag-jsv2.md)
>* [이미지 변환 추적 태그의 형식](/help/search-social-commerce/tracking/format-conversion-tag-image.md)


<!-- add if I keep the file:  
>* The Adobe Advertising JavaScript conversion mapping tag
-->
