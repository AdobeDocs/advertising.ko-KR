---
title: Adobe Advertising 전환 및 페이지 보기 추적 태그에 대한 FAQ
description: Adobe Advertising 전환 및 페이지 보기 추적 태그의 비교를 참조하십시오.
exl-id: 2e5ef792-e0f5-4409-bd37-87d9fab1265f
feature: Search Tracking
TQID: https://experienceleague.adobe.com/ckLRjqXGTShwM2TTyULRKjPwL5RYVWkiVVSkwMmvxE8
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 45b15880c20d516e4bab1ec664a45ebdf8ffbdcc
workflow-type: tm+mt
source-wordcount: 327
ht-degree: 0%

---

# Adobe Advertising 전환 및 페이지 보기 추적 태그에 대한 FAQ

다음은 Adobe Advertising 전환 추적 태그 및 페이지 보기 추적 태그에 적용됩니다.

| | ECID가 있는 JS 태그 | JS 버전 3 태그 | JS 버전 2 태그 | 이미지 태그 |
| ---- | ---- | ---- | ---- | ---- |
| 다른 JS 버전과 동일한 웹 페이지에서 사용할 수 있습니다. | — | — | — | 해당 사항 없음 |
| 동일한 웹 페이지에서 동일한 광고주 사용자 ID로 여러 태그를 사용할 수 있습니다. | 예 | 예 | 예 | — |
| 동일한 웹 페이지에서 서로 다른 광고주 사용자 ID가 있는 여러 태그를 사용할 수 있습니다. | 예 | 예 | — | — |
| Adobe Experience Platform용 Adobe Advertising 확장에서 사용하며, Experience Platform을 사용하여 생성된 다른 태그와 호환됩니다 | 예 | 예 | — | — |
| Adobe Advertising JavaScript 전환 매핑 태그와 함께 사용할 때 [!DNL Apple Safari] 및 [!DNL Mozilla Firefox]에서 시작된 모든 전환을 추적할 수 있습니다. | 예 | 예 | 예 | — |

<!-- add link to page on conversion mapping tag above? -->

>[!NOTE]
>
>* 모든 새로운 구현은 JavaScript 버전 3을 사용합니다.
>* ECID가 있는 JavaScript 태그는 [ECID(Adobe Experience Cloud ID) 서비스](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html?lang=ko)와 레거시 ef_id 및 gsurferid를 사용하여 전환을 측정합니다. 이 최신 태그는 [자사 CX Enterprise s_ecid 쿠키](https://experienceleague.adobe.com/docs/core-services/interface/administration/ec-cookies/cookies-first-party.html?lang=ko)를 만들고 다른 CX Enterprise 제품과의 긴밀한 통합을 제공합니다.
>* 광고주의 웹 페이지에 이미 태그가 구현된 경우에만 JavaScript 버전 2 태그를 사용합니다.
>* 가장 좋은 방법은 사이트에 이미지 태그 사용에 대한 정책이 없는 한 이미지 태그 대신 JavaScript 태그를 사용하는 것입니다.
>* JavaScript 태그는 Adobe CX Enterprise에서 만들거나, Adobe Audience Manager에서 만들거나, Audience Manager 또는 Adobe Analytics에서 Adobe CX Enterprise에 게시한 대상을 타깃팅하려는 광고주에게 필요합니다.

>[!MORELIKETHIS]
>
>* [Adobe Advertising 전환 추적 태그 정보](/help/search-social-commerce/tracking/conversion-tracking-advertising.md)
>* [Adobe Advertising 전환 태그 생성](/help/search-social-commerce/tools/conversion-tag-generate.md)
>* [JavaScript 전환 추적 태그 버전 3](/help/search-social-commerce/tracking/format-conversion-tag-jsv3.md)의 형식
>* [JavaScript 전환 추적 태그 버전 2](/help/search-social-commerce/tracking/format-conversion-tag-jsv2.md)의 형식
>* [이미지 변환 추적 태그의 형식](/help/search-social-commerce/tracking/format-conversion-tag-image.md)

<!--
 add if I keep the file:  
>* The Adobe Advertising JavaScript conversion mapping tag
-->
