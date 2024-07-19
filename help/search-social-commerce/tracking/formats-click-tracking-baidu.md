---
title: ' [!DNL Baidu]에 대한 클릭 추적 형식'
description: ' [!DNL Baidu] 계정의 클릭 추적 형식에 대해 알아봅니다.'
exl-id: 4f4ed518-aa25-4a29-b263-c01f78b69b92
feature: Search Tracking
source-git-commit: e16bc62127a708de8f4deb1eddfa53a14405cbc2
workflow-type: tm+mt
source-wordcount: '97'
ht-degree: 0%

---

# [!DNL Baidu]에서 후원 광고에 대한 클릭 추적 형식

다음 기본 대상 UR 형식은 스폰서 광고에 적용됩니다.

`http://pixel.everesttech.net/<advertiser_ID>/cq?ev_sid=<ad network ID>&ev_cmpid=<campaignID>&&ev_lx={keywordid}&ev_crx={creative}&ev_pl={placement}&url=<the landing page>`

예:

`http://pixel.everesttech.net/1234/cq?ev_sid=88&ev_cmpid=800577124&&ev_lx={keywordid}&ev_crx={creative}&ev_pl={placement}&url=http%3A//www.example.com`

>[!NOTE]
>
>* `<advertiser_ID>`은(는) Adobe Advertising 내 광고주의 고유 ID에 대한 변수입니다.
>
>* 이 형식은 캠페인에 대해 토큰 전달이 활성화되었음을 나타냅니다(기본값). 토큰 전달이 비활성화된 경우 `<advertiser_ID>` 뒤의 `cq?`을(를) `c?`(으)로 바꾸십시오.
>
>* `<campaignID>`은(는) 숫자 캠페인 ID의 변수입니다.
>
>* `<the landing page>`은(는) 최종 사용자가 이동되는 사이트의 URL을 나타내는 변수입니다.

>[!MORELIKETHIS]
>
>* [Adobe Advertising 전환 추적 서비스의 클릭 추적 URL 형식 정보](formats-click-tracking-about.md)
>* [AMO ID 형식](/help/integrations/analytics/ids.md#amo-id-formats)
