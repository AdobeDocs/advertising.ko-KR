---
title: Adobe Advertising 전환 추적 서비스에 대한 클릭 추적 URL 형식 정보
description: 지원되는 광고 네트워크의 클릭 추적 형식에 대해 알아봅니다.
exl-id: b6f225d5-2268-4b2a-9927-063155ba0dc5
feature: Search Tracking
source-git-commit: e16bc62127a708de8f4deb1eddfa53a14405cbc2
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---

# Adobe Advertising 전환 추적 서비스에 대한 클릭 추적 URL 형식 정보

Adobe Advertising 전환 추적 서비스를 사용하는 광고 계정 및 캠페인에 대한 추적 템플릿, 랜딩 페이지 접미사(최종 URL 접미사) 및 대상 URL의 형식은 다음과 같습니다.

`http://pixel.everesttech.net/<advertiser_ID>/<token passing parameter>?ev_sid=<ad network ID>&<tracking ID>&url=<the landing page>`

여기서:

* `http://pixel.everesttech.net`에서 사용자를 Adobe Advertising 픽셀 서버로 리디렉션합니다.

* `<advertiser_ID>`은(는) Adobe Advertising 내 광고주에게 할당된 고유한 사용자 ID에 대한 변수입니다.

* `<token passing parameter>`은(는) 다음 중 하나의 변수입니다.

   * `cq?` 또는 `rq`은(는) 토큰 전달이 활성화되었음을 나타냅니다.

   * `c?` 또는 `r`은(는) 토큰 전달이 비활성화되었음을 나타냅니다.

* `<ad network ID>`은(는) 지정한 광고 네트워크의 숫자 ID에 대한 변수입니다. 예를 들어 [!DNL Google Ads]의 *3*, [!DNL Microsoft Advertising]의 *10*, [!DNL Meta]의 *45*, [!DNL Yahoo! Display Network]의 *86*, [!DNL Naver]의 *87*, [!DNL Baidu]의 *87*, [!DNL Yandex]의 *90*, [!DNL Yahoo! Japan Ads]의 *94*, [!DNL Yahoo Native]의 *105*(더 이상 사용되지 않음) 또는 *106962 [!DNL Pinterest]용&rbrace;(더 이상 사용되지 않음)*

* `<tracking ID>`은(는) 계정에서 고유한 키워드, 광고 또는 배치를 식별하는 시스템 생성 추적 ID 문자열의 변수입니다. 문자열은 광고 네트워크별로 다릅니다.

* `<the landing page>`은(는) 최종 사용자가 이동되는 사이트의 URL을 나타내는 변수입니다. 대상 URL이 있는 계정의 경우 이 값은 URL입니다. 추적 템플릿이 있는 계정의 경우 이 값은 최종 URL을 나타내는 매개 변수(예: `{lpurl}`)입니다.

[[!DNL Baidu] 형식](formats-click-tracking-baidu.md), [[!DNL Google Ads] 형식](formats-click-tracking-google.md), [[!DNL Microsoft Advertising] 형식](formats-click-tracking-microsoft.md), [[!DNL Naver] 형식](formats-click-tracking-naver.md), [[!DNL Yahoo! Display Network] 형식](formats-click-tracking-yahoo-display-network.md), [[!DNL Yahoo! Japan Ads] 형식](formats-click-tracking-yahoo-japan.md) 및 [[!DNL Yandex] 형식](formats-click-tracking-yandex.md)을 나타내는 개별 페이지를 참조하세요.

>[!MORELIKETHIS]
>
>* [스폰서 광고에 대한 클릭 추적 형식 [!DNL Baidu]](formats-click-tracking-baidu.md)
>*  [!DNL Google Ads][&#128279;](formats-click-tracking-google.md)에 대한 클릭 추적 형식
>*  [!DNL Microsoft Advertising][&#128279;](formats-click-tracking-microsoft.md)에 대한 클릭 추적 형식
>* [스폰서 광고에 대한 클릭 추적 형식 [!DNL Naver]](formats-click-tracking-naver.md)
>* [스폰서 광고에 대한 클릭 추적 형식 [!DNL Yahoo! Japan Ads]](formats-click-tracking-yahoo-japan.md)
>* [스폰서 광고에 대한 클릭 추적 형식 [!DNL Yahoo! Display Network]](formats-click-tracking-yahoo-display-network.md)
>* [스폰서 광고에 대한 클릭 추적 형식 [!DNL Yandex]](formats-click-tracking-yandex.md)
