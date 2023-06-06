---
title: 클릭 추적 형식 [!DNL Yandex]
description: 의 클릭 추적 형식에 대해 알아봅니다. [!DNL Yandex] 계정.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---

# 스폰서 광고에 대한 클릭 추적 형식 [!DNL Yandex]

다음 기본 대상 UR 형식은 스폰서 광고에 적용됩니다.

`http://pixel.everesttech.net/<advertiser_ID>/cq?ev_sid=90&ev_lx={phrase_id}&ev_crx={ad_id}&ev_ln={keyword}&ev_mt={source_type}&ev_ltx=&ev_src={source}&ev_pos={position}&ev_pt={position_type}&url=<the landing page>`

예:

`http://pixel.everesttech.net/1234/cq?ev_sid=90&ev_lx={phrase_id}&amp;ev_crx={ad_id}&amp;ev_ln={keyword}&amp;ev_mt={source_type}&amp;ev_ltx=&amp;ev_src={source}&amp;ev_pos={position}&amp;ev_pt={position_type}&url=http%3A//www.example.com`

>[!NOTE]
>
>* `<advertiser_ID>` 는 Adobe 광고 내의 광고주의 고유 ID에 대한 변수입니다.
>
>* 이 형식은 캠페인에 대해 토큰 전달이 활성화되었음을 나타냅니다(기본값). 토큰 전달이 비활성화된 경우 을(를) 대체합니다. `cq?` 이후 `<advertiser_ID>` 포함 `c?`.
>
>* `<the landing page>` 는 최종 사용자가 안내하는 사이트의 URL을 나타내는 변수입니다.
>
>* `source_type`  는 일치 유형입니다.
>
>* `source` 광고가 검색 또는 콘텐츠 기반 사이트에 표시되었는지 여부입니다.
>
>* `position` 는 블록의 광고 위치 번호입니다. 비검색 트래픽의 경우 값은 &quot;0&quot;입니다.
>
>* `position_type` 광고가 표시된 블록입니다 [!DNL Yandex]. 가능한 값은 &quot;premium&quot;(상단 블록), &quot;other&quot;(오른쪽 블록) 또는 &quot;none&quot;(비검색 트래픽)입니다.


>[!MORELIKETHIS]
>
>* [Adobe 광고 전환 추적 서비스에 대한 클릭 추적 URL 형식 정보](formats-click-tracking-about.md)
>* [s\_kwcid 추적 코드 형식](skwcid-tracking-parameter.md)

