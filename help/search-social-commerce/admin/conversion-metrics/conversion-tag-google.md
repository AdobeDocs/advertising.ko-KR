---
title: 다음에 대한 변환 태그 만들기 [!DNL Google Ads]
description: 을(를) 만드는 방법 알아보기 [!DNL Google Ads] 변환 태그.
feature: Conversions
source-git-commit: 395421c69214c3b0370523909047a924af23ea55
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# 다음에 대한 변환 태그 만들기 [!DNL Google Ads]

개인에 대해 추적할 새 변환에 대한 변환 태그를 만들 수 있습니다 [!DNL Google Ads] 계정(관리자 계정 수준에서 추적되지 않음)

기존 전환에 대한 전환 태그를 생성하려면 광고 네트워크의 편집기를 사용하십시오.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Admin] >[!UICONTROL Conversions]**.

1. 데이터 테이블 위의 도구 모음에서 ![만들기](/help/search-social-commerce/assets/add.png "만들기").

1. 다음을 지정합니다. [전환 태그 설정](#conversion-tag-settings-google).

   1. 계정을 선택한 다음 전환 유형을 선택합니다.

   1. 클릭 **[!UICONTROL Next]**.

   1. 변환 옵션을 지정합니다.

   1. 클릭 **[!UICONTROL Generate]**.

1. 전환 태그를 복사하여 전환 지표를 추적할 웹 사이트에 구현합니다.

   참조: &quot;설치 [!DNL Google] 태그 내&quot; [!DNL Google Ads] &quot; 도움말[2. Google 태그 설정](https://support.google.com/google-ads/answer/12215519).&quot;

1. 클릭 **[!UICONTROL Done].**

웹 사이트에 태그를 추가하고 태그가 실행되면 [!DNL Google Ads] 는 웹 사이트에서 전환을 기록합니다. Search, Social 및 Commerce는 전환을 매일 동기화합니다. 동기화된 데이터에 대한 자세한 내용은 &quot;[[!DNL Google Ads] 검색, 소셜 및 상거래의 전환 데이터](/help/search-social-commerce/campaign-management/introduction/google-conversion-data.md).

## 전환 태그 설정 {#conversion-tag-settings-google}

**[!UICONTROL Select an Account]:** 해당 Google 광고 계정.

**[!UICONTROL Type of Conversion]:** 추적할 변환 유형: *[!UICONTROL Click on a webpage element]*, *[!UICONTROL Calls to a phone number on your website]*, 또는 *[!UICONTROL Clicks to your number on your mobile website]*.

**[!UICONTROL Conversion Name]:** 전환 지표에 대한 고유한 이름.

**\[전환 범주\]:** 전환 범주. 사용 가능한 카테고리는 전환 유형에 따라 다릅니다. 대상 *[!UICONTROL Calls to a phone number on your website]* 및 *[!UICONTROL Clicks to your number on your mobile website]*, &quot;[!UICONTROL Phone Call Lead]기본적으로 &quot;&quot;가 선택됩니다.

**\[작업 유형\]:** 목표가 *[!UICONTROL Primary action used for bidding optimization]* 또는 *[!UICONTROL Secondary action not used for bidding optimization]*.

**[!UICONTROL Value]:** 측정 방법 [각 전환 값](https://support.google.com/google-ads/answer/3419241):

* *[!UICONTROL Use the same value for each conversion],* 통화를 선택하고 각 전환에 대한 값을 입력해야 합니다.

* *[!UICONTROL Use a different value for each conversion],* 통화를 선택하고 각 전환에 대한 기본값을 입력해야 합니다. 특정 웹 페이지에서 태그를 구현할 때 태그에서 기본값을 트랜잭션 특정 값으로 변경할 수 있습니다.

* *[!UICONTROL Don't use a value for this conversion action (Not recommended)]*

**[!UICONTROL Count]:** [클릭당 또는 상호 작용당 카운트할 전환 수](https://support.google.com/google-ads/answer/3438531): *[!UICONTROL Every (Recommended for every purchases because every purchase is valuable)]* 또는 *[!UICONTROL One (Recommended for leads, sign-ups and other conversions because only the first interaction is valuable)]*.

**[!UICONTROL Click Through Conversion Window]:** 전환이 기록된 광고 상호 작용 후 최대 일 수입니다. 검색, 표시 및 쇼핑 캠페인의 경우 기간은 1~90일 사이일 수 있습니다. 번호 선택 또는 선택 **[!UICONTROL Custom]** 숫자를 입력합니다.

**[!UICONTROL View Through Conversion Window]:** 사용자가 뷰스루 전환이 기록된 광고를 본 후 최대 일수. 검색, 표시 및 쇼핑 캠페인의 경우 기간은 1~90일 사이일 수 있습니다. 번호 선택 또는 선택 **[!UICONTROL Custom]** 숫자를 입력합니다.

**[!UICONTROL Attribution Model]:** [각 광고 인터랙션에 얻게 되는 크레딧의 양](https://support.google.com/google-ads/answer/6259715?sjid=8211249329930775138): *[!UICONTROL Data driven]*, *[!UICONTROL Last click]*, *[!UICONTROL First click]*, *[!UICONTROL Linear]*, *[!UICONTROL Time decay]*, 또는 *[!UICONTROL Position based]*.

>[!MORELIKETHIS]
>
>* [[!DNL Google Ads] 검색, 소셜 및 상거래의 전환 데이터](/help/search-social-commerce/campaign-management/introduction/google-conversion-data.md)
