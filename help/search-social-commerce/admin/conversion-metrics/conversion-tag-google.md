---
title: ' [!DNL Google Ads]에 대한 변환 태그 만들기'
description: ' [!DNL Google Ads] 전환 태그를 만드는 방법을 알아봅니다.'
feature: Conversions
exl-id: 214611f0-bd38-499e-a7de-3a5878995fb5
source-git-commit: 2c20d2138ee797b6ed2f27d9baa9eda7d413da8d
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# [!DNL Google Ads]에 대한 변환 태그 만들기

관리자 계정 수준에서 추적되지 않고 개별 [!DNL Google Ads] 계정에 대해 추적할 새 전환에 대한 전환 태그를 만들 수 있습니다.

기존 전환에 대한 전환 태그를 생성하려면 광고 네트워크의 편집기를 사용하십시오.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Admin] >[!UICONTROL Conversions]**&#x200B;을(를) 클릭합니다. 그러면 **[!UICONTROL Summary]** 탭이 열립니다.

1. 데이터 테이블 위의 도구 모음에서 ![만들기](/help/search-social-commerce/assets/add.png "만들기")를 클릭합니다.

1. [변환 태그 설정](#conversion-tag-settings-google)을 지정하십시오.

   1. 계정을 선택한 다음 전환 유형을 선택합니다.

   1. **[!UICONTROL Next]**&#x200B;을(를) 클릭합니다.

   1. 변환 옵션을 지정합니다.

   1. **[!UICONTROL Generate]**&#x200B;을(를) 클릭합니다.

1. 전환 태그를 복사하여 전환 지표를 추적할 웹 사이트에 구현합니다.

   &quot;[2&quot;에 대한 [!DNL Google Ads] 도움말의 &quot;[!DNL Google] 태그 설치&quot;를 참조하십시오. Google 태그 ](https://support.google.com/google-ads/answer/12215519)을(를) 설정합니다.&quot;

1. **[!UICONTROL Done].** 클릭

태그를 웹 사이트에 추가하면 태그가 실행되기 시작하면 [!DNL Google Ads]에서 웹 사이트에 전환을 기록합니다. Search, Social 및 Commerce은 전환을 매일 동기화합니다. 동기화된 데이터에 대한 자세한 내용은 &quot;[[!DNL Google Ads] 검색, 소셜 및 Commerce의 전환 데이터](/help/search-social-commerce/campaign-management/introduction/google-conversion-data.md)를 참조하십시오.

## 전환 태그 설정 {#conversion-tag-settings-google}

**[!UICONTROL Select an Account]:** 적용 가능한 Google 광고 계정입니다.

**[!UICONTROL Type of Conversion]:** 추적 전환 유형: *[!UICONTROL Click on a webpage element]*, *[!UICONTROL Calls to a phone number on your website]* 또는 *[!UICONTROL Clicks to your number on your mobile website]*. **참고:** *[!UICONTROL Import conversion]*&#x200B;은(는) 다른 용도로 사용됩니다. &quot;[잠재 고객에 대한 전환 작업 만들기 [!DNL Google Ads] 향상된 전환](/help/search-social-commerce/admin/conversion-metrics/conversion-action-google.md)&quot;를 참조하세요.&quot;

**[!UICONTROL Conversion Name]:** 전환 지표에 대한 고유한 이름입니다.

**\[전환 범주\]:** 전환 범주입니다. 사용 가능한 카테고리는 전환 유형에 따라 다릅니다. *[!UICONTROL Calls to a phone number on your website]* 및 *[!UICONTROL Clicks to your number on your mobile website]*&#x200B;의 경우 기본적으로 &quot;[!UICONTROL Phone Call Lead]&quot;이(가) 선택됩니다.

**\[작업 유형\]:** 목표가 *[!UICONTROL Primary action used for bidding optimization]*&#x200B;인지 *[!UICONTROL Secondary action not used for bidding optimization]*&#x200B;인지 여부.

**[!UICONTROL Value]:** 각 전환의 [값을 측정하는 방법](https://support.google.com/google-ads/answer/3419241):

* 통화를 선택하고 각 전환에 대한 값을 입력해야 하는 *[!UICONTROL Use the same value for each conversion],*.

* 통화를 선택하고 각 전환에 대한 기본값을 입력해야 하는 *[!UICONTROL Use a different value for each conversion],*. 특정 웹 페이지에서 태그를 구현할 때 태그에서 기본값을 트랜잭션 특정 값으로 변경할 수 있습니다.

* *[!UICONTROL Don't use a value for this conversion action (Not recommended)]*

**[!UICONTROL Count]:** [클릭당 또는 상호 작용당 카운트할 전환 수](https://support.google.com/google-ads/answer/3438531): *[!UICONTROL Every (Recommended for every purchases because every purchase is valuable)]* 또는 *[!UICONTROL One (Recommended for leads, sign-ups and other conversions because only the first interaction is valuable)]*.

**[!UICONTROL Click Through Conversion Window]:** 전환이 기록된 광고 상호 작용 후 최대 일 수입니다. 검색, 표시 및 쇼핑 캠페인의 경우 기간은 1~90일 사이일 수 있습니다. 숫자를 선택하거나 **[!UICONTROL Custom]**&#x200B;을(를) 선택하고 숫자를 입력하세요.

**[!UICONTROL View Through Conversion Window]:** 사용자가 광고를 본 후 뷰스루 전환이 기록된 최대 일 수입니다. 검색, 표시 및 쇼핑 캠페인의 경우 기간은 1~90일 사이일 수 있습니다. 숫자를 선택하거나 **[!UICONTROL Custom]**&#x200B;을(를) 선택하고 숫자를 입력하세요.

**[!UICONTROL Attribution Model]:** [각 광고 상호 작용에 필요한 크레딧의 양](https://support.google.com/google-ads/answer/6259715?sjid=8211249329930775138): *[!UICONTROL Data driven]* 또는 *[!UICONTROL Last click]*. **참고:** 이전에 현재 지원되지 않는 *[!UICONTROL First click]*, *[!UICONTROL Linear]*, *[!UICONTROL Time decay]* 또는 *[!UICONTROL Position based]* 모델을 사용했던 전환 작업에서 이제 *[!UICONTROL Data driven]* 모델을 사용합니다.

>[!MORELIKETHIS]
>
>* [향상된 전환을 위해 오프라인 전환 데이터 업로드](/help/search-social-commerce/admin/conversion-metrics/upload-data-offline-conversions.md)
>* [[!DNL Google Ads] 검색, 소셜 및 Commerce의 전환 데이터](/help/search-social-commerce/campaign-management/introduction/google-conversion-data.md)
