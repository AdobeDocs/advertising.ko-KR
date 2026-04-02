---
title: ' [!DNL Naver]에 대한 클릭 추적 형식'
description: ' [!DNL Naver] 계정의 클릭 추적 형식에 대해 알아봅니다.'
exl-id: b438652e-6e98-4223-8169-2bfb37500670
feature: Search Tracking
TQID: https://experienceleague.adobe.com/c1zAy1aKgr4MRpyiitdmO4VxP7kfKfFWHzYk88lvX2w
product_v2: id: a829a185-511f-4bf8-8dcf-9e684f8011cf
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 527ca2bb74de388c13ba1ce5bde3f8be1cead8d0
workflow-type: tm+mt
source-wordcount: 90
ht-degree: 0%

---

# [!DNL Naver]에서 후원 광고에 대한 클릭 추적 형식

다음 기본 대상 UR 형식은 스폰서 광고에 적용됩니다.

`http://pixel.everesttech.net/<advertiser_ID>/cq?ev_sid=87&ev_cl={ef_uniqueid}&url=<the landing page>`

예:

`http://pixel.everesttech.net/1234/cq?ev_sid=87&ev_cl=258e27dcec70156a667f2229020e488&url=http%3A//www.example.com`

>[!NOTE]
>
>* `<advertiser_ID>`은(는) Adobe Advertising 내의 광고주 고유 ID에 대한 변수입니다.
>
>* 이 형식은 캠페인에 대해 토큰 전달이 활성화되었음을 나타냅니다(기본값). 토큰 전달이 비활성화된 경우 `cq?` 뒤의 `<advertiser_ID>`을(를) `c?`(으)로 바꾸십시오.
>
* `<the landing page>`은(는) 최종 사용자가 이동되는 사이트의 URL을 나타내는 변수입니다.

>[!MORELIKETHIS]
>
>* [Adobe Advertising 전환 추적 서비스에 대한 클릭 추적 URL 형식 정보](formats-click-tracking-about.md)
>* [AMO ID 형식](https://experienceleague.adobe.com/en/docs/analytics/components/dimensions/amo-id#dimension-items)
