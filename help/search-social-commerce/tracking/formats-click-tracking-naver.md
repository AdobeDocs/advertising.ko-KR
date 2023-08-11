---
title: 클릭 추적 형식 [!DNL Naver]
description: 의 클릭 추적 형식에 대해 알아봅니다. [!DNL Naver] 계정.
exl-id: ff243eb5-d768-4e5c-b5b3-015fe22c9d5a
feature: Search Tracking
source-git-commit: 05b9a55e19c9f76060eedb35c41cdd2e11753c24
workflow-type: tm+mt
source-wordcount: '89'
ht-degree: 0%

---

# 스폰서 광고에 대한 클릭 추적 형식 [!DNL Naver]

다음 기본 대상 UR 형식은 스폰서 광고에 적용됩니다.

`http://pixel.everesttech.net/<advertiser_ID>/cq?ev_sid=87&ev_cl={ef_uniqueid}&url=<the landing page>`

예:

`http://pixel.everesttech.net/1234/cq?ev_sid=87&ev_cl=258e27dcec70156a667f2229020e488&url=http%3A//www.example.com`

>[!NOTE]
>
>* `<advertiser_ID>` 는 Adobe Advertising 내 광고주의 고유 ID에 대한 변수입니다.
>
>* 이 형식은 캠페인에 대해 토큰 전달이 활성화되었음을 나타냅니다(기본값). 토큰 전달이 비활성화된 경우 을(를) 대체합니다. `cq?` 이후 `<advertiser_ID>` 포함 `c?`.
>
* `<the landing page>` 는 최종 사용자가 안내하는 사이트의 URL을 나타내는 변수입니다.

>[!MORELIKETHIS]
>
>* [Adobe Advertising 전환 추적 서비스에 대한 클릭 추적 URL 형식 정보](formats-click-tracking-about.md)
>* [AMO ID 형식](/help/integrations/analytics/ids.md#amo-id-formats)
