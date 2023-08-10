---
title: 클릭 추적 형식 [!DNL Baidu]
description: 의 클릭 추적 형식에 대해 알아봅니다. [!DNL Baidu] 계정.
exl-id: a57ff0cf-0bcf-4d55-9a86-7551db8a08e7
feature: Search Tracking
source-git-commit: f80d05aa40fd4114e9585220fe747ca7d36a19bb
workflow-type: tm+mt
source-wordcount: '101'
ht-degree: 0%

---

# 스폰서 광고에 대한 클릭 추적 형식 [!DNL Baidu]

다음 기본 대상 UR 형식은 스폰서 광고에 적용됩니다.

`http://pixel.everesttech.net/<advertiser_ID>/cq?ev_sid=<ad network ID>&ev_cmpid=<campaignID>&&ev_lx={keywordid}&ev_crx={creative}&ev_pl={placement}&url=<the landing page>`

예:

`http://pixel.everesttech.net/1234/cq?ev_sid=88&ev_cmpid=800577124&&ev_lx={keywordid}&ev_crx={creative}&ev_pl={placement}&url=http%3A//www.example.com`

>[!NOTE]
>
>* `<advertiser_ID>` 는 Adobe Advertising 내 광고주의 고유 ID에 대한 변수입니다.
>
>* 이 형식은 캠페인에 대해 토큰 전달이 활성화되었음을 나타냅니다(기본값). 토큰 전달이 비활성화된 경우 을(를) 대체합니다. `cq?` 이후 `<advertiser_ID>` 포함 `c?`.
>
>* `<campaignID>` 는 숫자 캠페인 ID에 대한 변수입니다.
>
>* `<the landing page>` 는 최종 사용자가 안내하는 사이트의 URL을 나타내는 변수입니다.

>[!MORELIKETHIS]
>
>* [Adobe Advertising 전환 추적 서비스에 대한 클릭 추적 URL 형식 정보](formats-click-tracking-about.md)
>* [AMO ID 추적 코드 형식](skwcid-tracking-parameter.md)
