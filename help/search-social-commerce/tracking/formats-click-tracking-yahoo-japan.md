---
title: ' [!DNL Yahoo! Japan Ads]에 대한 클릭 추적 형식'
description: ' [!DNL Yahoo! Japan Ads] 계정의 클릭 추적 형식에 대해 알아봅니다.'
exl-id: 79e45205-5c72-4612-9b60-36538e3c48c4
feature: Search Tracking
source-git-commit: e16bc62127a708de8f4deb1eddfa53a14405cbc2
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---

# [!DNL Yahoo! Japan Ads]에서 후원 광고에 대한 클릭 추적 형식

스폰서 광고에는 다음과 같은 기본 추적 템플릿 형식이 적용됩니다.

`http://pixel.everesttech.net/<advertiser_ID>/cq?ev_sid=<ad network ID>&ev_ln={keyword}&ev_crx={creative}&ev_mt={matchtype}&ev_n={network}&ev_dvc={device}&url=!{unescapedlpurl}`

또는 [!DNL Yahoo! Japan Ads]의 계정에 대해 자동 태그 지정 옵션이 설정된 경우:

`http://pixel.everesttech.net/<advertiser_ID>/cq?ev_sid=<ad network ID>&ev_ln={keyword}&ev_crx={creative}&ev_mt={matchtype}&ev_n={network}&ev_dvc={device}&url=!{unescapedlpurl}/?yclid=<yclid>`

예:

`http://pixel.everesttech.net/1234/cq?ev_sid=94&ev_ln={keyword}&ev_crx={creative}&ev_mt={matchtype}&ev_n={network}&ev_dvc={device}&url=http%3A//www.example.com/?yclid=1234567890`

>[!NOTE]
>
>* `<advertiser_ID>`은(는) Adobe Advertising 내 광고주의 고유 ID에 대한 변수입니다.
>
>* 이 형식은 캠페인에 대해 토큰 전달이 활성화되었음을 나타냅니다(기본값). 토큰 전달이 비활성화된 경우 `<advertiser_ID>` 뒤의 `cq?`을(를) `c?`(으)로 바꾸십시오.
>
>* `<the landing page>`은(는) 최종 사용자가 이동되는 사이트의 URL을 나타내는 변수입니다.

>[!MORELIKETHIS]
>
>* [Adobe Advertising 전환 추적 서비스의 클릭 추적 URL 형식 정보](formats-click-tracking-about.md)
>* [AMO ID 형식](/help/integrations/analytics/ids.md#amo-id-formats)
