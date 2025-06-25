---
title: 클릭 추적 URL 생성
description: 검색, 소셜 및 Commerce 클릭 추적 URL을 수동으로 생성하는 방법을 알아봅니다.
exl-id: 43a36869-146a-4c5f-b4f2-eddfb856480b
feature: Search Tools, Search Tracking
source-git-commit: d0f1c413134a0868ddec79ded7672af316267edd
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---

# 추적 URL 도구를 사용하여 검색, 소셜 및 Commerce 클릭 추적 URL 생성

*Adobe Advertising 전환 추적만 있는 광고주*

클릭 추적 URL을 수동으로 생성하고 구현해야 하는 시기에 대한 자세한 내용은 &quot;[클릭 추적 URL을 생성하는 시기와 방법](/help/search-social-commerce/tracking/click-tracking-ways-to-generate.md)&quot;을 참조하십시오.

>[!NOTE]
>
>이 기능은 관련 광고 계정에서 추적 템플릿 또는 대상 URL을 구현하지 않습니다.

1. 메인 메뉴에서 **[!UICONTROL Search, Social, & Commerce]> [!UICONTROL Tools] >[!UICONTROL Tracking URL]**&#x200B;을(를) 클릭합니다.

1. 목록에서 광고 네트워크 계정을 선택합니다.

   ([!DNL Google Ads]개의 키워드, 텍스트, 모바일 앱 설치 및 동적 검색 광고, 배치, 사이트링크 및 제품 그룹) 추적 템플릿 필드에 대한 추적 태그가 표시됩니다. 계정 수준 추가 매개 변수는 포함되지 않습니다. 4단계로 건너뜁니다.

   다른 모든 유형의 태그에 대해 태그를 생성하는 정보를 입력합니다.

1. (필요한 경우) 태그를 생성합니다.

   1. 다음 방법 중 하나로, 요청이 있는 경우 사이트링크 또는 제품 이름과 함께 랜딩 페이지를 지정합니다.

      * 전체 경로와 파일 이름을 입력하거나 **[!UICONTROL Browse]**&#x200B;을(를) 클릭하여 장치 또는 네트워크에서 파일을 찾아 정보가 포함된 파일을 지정하십시오. 파일은 다음 형식의 한 줄에 하나의 항목이 있는 탭으로 구분된 텍스트 파일이어야 합니다.

         * (광고 크리에이티브, 표준 광고) `**landing_page**`

           여기서 `landing_page`은(는) 올바른 랜딩 페이지 URL 또는 기본 URL입니다.

           예: http://www.example.com/travel.html

         * ([!DNL Microsoft Advertising]개의 사이트 링크) `sitelink <tab> ** <tab> landing_page`

           여기서 `sitelink`은(는) 사이트 링크 이름이고 `landing_page`은(는) 올바른 랜딩 페이지 URL 또는 기본 URL입니다.

           예: `Careers <tab> ** <tab> http://www.example.com/careers.html`

           파일에는 최대 10,000개의 줄이 포함될 수 있습니다.

         * ([!DNL Google Merchant Center]개 제품 그룹 및 [!DNL Microsoft Advertising]개 제품 광고) `product name <tab> ** <tab> landing_page`

           여기서 `product name`은(는) 제품 이름이고 `landing_page`은(는) 올바른 랜딩 페이지 URL 또는 기본 URL입니다.

           예: `Acme PR208 <tab> ** <tab> http://www.example.com/travel.html`

           파일에는 최대 10,000개의 줄이 포함될 수 있습니다.

      * 입력 필드에 다음 형식으로 한 줄에 하나의 항목을 입력합니다.

         * (광고 크리에이티브, 표준 광고) `landing_page`

           여기서 `landing_page`은(는) 올바른 랜딩 페이지 URL 또는 기본 URL입니다.

           예: http://www.example.com/travel.html

         * ([!DNL Microsoft Advertising]개의 사이트 링크) `sitelink**landing_page`

           여기서 `sitelink`은(는) 사이트 링크 이름이고 `landing_page`은(는) 올바른 랜딩 페이지 URL 또는 기본 URL입니다.

           예: `Careers**http://www.example.com/careers.html`

         * ([!DNL Google Merchant Center]개 제품 그룹 및 [!DNL Microsoft Advertising]개 제품 광고) `product name**landing_page`

           여기서 `product name`은(는) 제품 이름이고 `landing_page`은(는) 올바른 랜딩 페이지 URL 또는 기본 URL입니다.

           예: Acme PR208**http://www.example.com/travel.html

   1. **[!UICONTROL Generate Tracking URLs]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 화면 또는 출력 페이지에서 URL(&quot;http&quot; 또는 &quot;https&quot;로 시작)을 복사하여 검색 또는 소셜 계정에서 구현합니다.

대상 URL이 있는 계정의 경우 해당 [!UICONTROL Base URL] 필드에 값을 입력하십시오.

최종 URL이 있는 계정의 경우 해당 [!UICONTROL Tracking Template] 필드에 화면 값을 입력하십시오. `&url=` 매개 변수(예: `{lpurl}`) 뒤에 최종 URL에 대한 매개 변수를 추가해야 합니다. [!DNL Yahoo! Japan Ads] 계정의 경우 `{lpurl}` 매개 변수를 사용하십시오. 추적 템플릿의 최종 URL을 나타내는 [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 매개 변수 목록을 보려면 [[!DNL Google Ads] 설명서](https://support.google.com/google-ads/answer/6305348)&#x200B;(&quot;사용 가능한 [!DNL ValueTrack] 매개 변수&quot;에 대한 섹션에서 &quot;추적 템플릿 전용&quot; 매개 변수 참조) 및 [[!DNL Microsoft Advertising] 설명서](https://help.ads.microsoft.com/#apex/3/en/56799/2)를 참조하십시오.

>[!MORELIKETHIS]
>
>* [추적 태그를 만들고 디코딩하는 도구에 대한 정보](tracking-tools-about.md)
>* [클릭 추적 URL을 생성하는 시기와 방법](/help/search-social-commerce/tracking/click-tracking-ways-to-generate.md)
>* [검색, 소셜 및 Commerce 클릭 추적 URL 디코딩](click-tracking-url-decode.md)
