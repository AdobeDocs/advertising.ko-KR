---
title: 클릭 추적 URL 생성
description: 검색, 소셜 및 상거래 클릭 추적 URL을 수동으로 생성하는 방법을 알아봅니다.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# 추적 URL 도구를 사용하여 검색, 소셜 및 상거래 클릭 추적 URL 생성

*Adobe 광고 전환 추적만 있는 광고주*

클릭 추적 URL을 수동으로 생성하고 구현해야 하는 시기에 대한 자세한 내용은 &quot;[클릭 추적 URL 생성 시기 및 방법](/help/search-social-commerce/tracking/click-tracking-ways-to-generate.md).&quot;

>[!NOTE]
>
>이 기능은 관련 광고 계정에서 추적 템플릿 또는 대상 URL을 구현하지 않습니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Tools] >[!UICONTROL Tracking URL]**.

1. 목록에서 광고 네트워크 계정을 선택합니다.

   ([!DNL Google Ads] 키워드, 텍스트, 모바일 앱 설치 및 동적 검색 광고, 배치, 사이트링크 및 제품 그룹) 추적 템플릿 필드에 대한 추적 태그가 표시됩니다. 계정 수준 추가 매개 변수는 포함되지 않습니다. 4단계로 건너뜁니다.

   다른 모든 유형의 태그에 대해 태그를 생성하는 정보를 입력합니다.

1. (필요한 경우) 태그를 생성합니다.

   1. 다음 방법 중 하나로, 요청이 있는 경우 사이트링크 또는 제품 이름과 함께 랜딩 페이지를 지정합니다.

      * 전체 경로와 파일 이름을 입력하거나 을 눌러 정보가 포함된 파일을 지정합니다. **[!UICONTROL Browse]** 장치 또는 네트워크에서 파일을 찾습니다. 파일은 다음 형식의 한 줄에 하나의 항목이 있는 탭으로 구분된 텍스트 파일이어야 합니다.

         * (크리에이티브, 표준 광고) `**landing_page**`

            위치 `landing_page` 는 유효한 랜딩 페이지 URL 또는 기본 URL입니다.

            예: http://www.example.com/travel.html

         * ([!DNL Microsoft® Advertising] sitelinks) `sitelink <tab> ** <tab> landing_page`

            위치 `sitelink` 는 사이트링크 이름이며, `landing_page` 는 유효한 랜딩 페이지 URL 또는 기본 URL입니다.

            예: `Careers <tab> ** <tab> http://www.example.com/careers.html`

            파일에는 최대 10,000개의 줄이 포함될 수 있습니다.

         * ([!DNL Google Merchant Center] 제품 그룹 및 [Microsoft® Advertising] 제품 광고) `product name <tab> ** <tab> landing_page`

            위치 `product name` 는 제품 이름이며 `landing_page` 는 유효한 랜딩 페이지 URL 또는 기본 URL입니다.

            예: `Acme PR208 <tab> ** <tab> http://www.example.com/travel.html`

            파일에는 최대 10,000개의 줄이 포함될 수 있습니다.
      * 입력 필드에 다음 형식으로 한 줄에 하나의 항목을 입력합니다.

         * (크리에이티브, 표준 광고) `landing_page`

            위치 `landing_page` 는 유효한 랜딩 페이지 URL 또는 기본 URL입니다.

            예: http://www.example.com/travel.html

         * ([!DNL Microsoft® Advertising] sitelinks) `sitelink**landing_page`

            위치 `sitelink` 는 사이트링크 이름이며, `landing_page` 는 유효한 랜딩 페이지 URL 또는 기본 URL입니다.

            예: `Careers**http://www.example.com/careers.html`

         * ([!DNL Google Merchant Center] 제품 그룹 및 [!DNL Microsoft® Advertising] 제품 광고) `product name**landing_page`

            위치 `product name` 는 제품 이름이며 `landing_page` 는 유효한 랜딩 페이지 URL 또는 기본 URL입니다.

            예: Acme PR208**http://www.example.com/travel.html
   1. 클릭 **[!UICONTROL Generate Tracking URLs]**.



1. (선택 사항) 화면 또는 출력 페이지에서 URL(&quot;http&quot; 또는 &quot;https&quot;로 시작)을 복사하여 검색 또는 소셜 계정에서 구현합니다.

대상 URL이 있는 계정의 경우 적절한 필드에 값을 입력합니다 [!UICONTROL Base URL] 필드.

최종 URL이 있는 계정의 경우 적절한 필드에 화면 값을 입력합니다 [!UICONTROL Tracking Template] 필드. 최종 URL 뒤에 매개 변수를 추가해야 합니다. `&url=` 매개 변수(예: `{lpurl}`). 대상 [!DNL Yahoo! Japan Ads] 계정, 매개 변수 사용 `{lpurl}`. 의 목록 [!DNL Google Ads] 및 [!DNL Microsoft® Advertising] 추적 템플릿에서 최종 URL을 나타내는 매개 변수는 [[!DNL Google Ads] 설명서](https://support.google.com/google-ads/answer/6305348) (&quot;사용 가능한 ValueTrack 매개 변수&quot;에 대한 섹션의 &quot;추적 템플릿만&quot; 매개 변수 참조) 및 [[!DNL Microsoft® Advertising] 설명서](https://help.ads.microsoft.com/#apex/3/en/56799/2).

>[!MORELIKETHIS]
>
>* [추적 태그를 만들고 디코딩하는 도구 정보](tracking-tools-about.md)
>* [클릭 추적 URL 생성 시기 및 방법](/help/search-social-commerce/tracking/click-tracking-ways-to-generate.md)
>* [검색, 소셜 및 상거래 클릭 추적 URL 디코딩](click-tracking-url-decode.md)

