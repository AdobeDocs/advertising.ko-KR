---
title: ' [!DNL Google Ads] 향상된 잠재 고객 전환에 대한 전환 작업 만들기'
description: 잠재 고객에 대한 향상된 전환을 위해  [!DNL Google Ads] 전환 작업을 만드는 방법을 알아봅니다.
feature: Conversions
exl-id: faf4a6de-e82f-4afd-bda5-2602fb45aee5
source-git-commit: d0f1c413134a0868ddec79ded7672af316267edd
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# [!DNL Google Ads] 향상된 잠재 고객 전환에 대한 전환 작업 만들기

*[!DNL Google Ads]개의 계정만*

관리자 계정 수준에서 추적되는 전환이 아니라 개별 [!DNL Google Ads] 계정에 대해 추적할 잠재 고객에 대한 [!DNL Google Ads] 향상된 전환에 대한 전환 작업을 만들 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Search, Social, & Commerce]> [!UICONTROL Admin] >[!UICONTROL Conversions]**&#x200B;을(를) 클릭하면 **[!UICONTROL Summary]** 탭이 열립니다.

1. 데이터 테이블 위의 도구 모음에서 ![만들기](/help/search-social-commerce/assets/add.png "만들기")를 클릭합니다.

1. [전환 작업 설정](#conversion-action-settings-google)을 지정하십시오.

   1. 계정을 선택한 다음 전환 유형을 선택합니다. *[!UICONTROL Import conversion]*.

   1. **[!UICONTROL Next]**&#x200B;을(를) 클릭합니다.

   1. 전환 작업 옵션을 지정합니다.

   1. **[!UICONTROL Generate]**&#x200B;을(를) 클릭합니다.

1. 잠재 고객에 대한 향상된 전환을 위해 추적 태그를 만드는 방법에 대한 정보를 읽은 다음 **[!UICONTROL Next]**&#x200B;을(를) 클릭합니다.

   전환 태그를 만든 후 전환 지표를 추적하려는 웹 사이트에서 필요에 따라 구현합니다. 자세한 내용은 다음을 참조하십시오.

   * [!DNL Google] 태그를 사용하려면 &quot;[태그 [!DNL Google] 태그를 사용하는 리드에 대한 향상된 전환 설정](https://support.google.com/google-ads/answer/11347292)에서 &quot;[!DNL Google] 태그 설정 구성&quot;에 대한 [!DNL Google Ads] 지침을 참조하십시오.&quot;

   * [!DNL Google Tag Manager]을(를) 사용하려면 &quot;[&#x200B; [!DNL Google Tag Manager]](https://support.google.com/google-ads/answer/11021502?#configure)의 잠재 고객에 대한 향상된 전환 설정&quot;에서 &quot;[!DNL Google] 태그 설정을 구성&quot;하고 &quot;설정을 확인하고 컨테이너를 게시&quot;하는 [!DNL Google Ads] 지침을 참조하십시오.&quot;

1. **[!UICONTROL Done].** 클릭

전환 작업을 만들고 전환 추적 태그를 구현하면 조직에서 캡처한 오프라인 전환 데이터를 업로드하고 이를 전환 작업에 연결할 수 있습니다. 향상된 전환을 위해 &quot;[오프라인 전환 데이터 업로드](/help/search-social-commerce/admin/conversion-metrics/upload-data-offline-conversions.md)&quot;를 참조하십시오.

## 전환 작업 설정 {#conversion-action-settings-google}

**[!UICONTROL Select an Account]:** 적용 가능한 Google 광고 계정입니다.

**[!UICONTROL Type of Conversion]:** 추적할 변환 유형: *[!UICONTROL Import conversion]*&#x200B;을(를) 선택합니다. 다른 모든 유형은 다른 유형의 전환에 대한 전환 추적 태그(전환 작업 아님)를 만드는 데 사용됩니다.

**[!UICONTROL Conversion Name]:** 변환 작업의 고유한 이름입니다.

**\[전환 범주\]:** *적격 잠재 고객* 또는 *등록*&#x200B;과 같은 전환 범주.

**\[작업 유형\]:** 목표가 *[!UICONTROL Primary action used for bidding optimization]*&#x200B;인지 *[!UICONTROL Secondary action not used for bidding optimization]*&#x200B;인지 여부.

**[!UICONTROL Value]:** 각 전환의 [값을 측정하는 방법](https://support.google.com/google-ads/answer/13064207):

* 통화를 선택하고 각 전환에 대한 값을 입력해야 하는 *[!UICONTROL Use the same value for each conversion],*.

* 통화를 선택하고 각 전환에 대한 기본값을 입력해야 하는 *[!UICONTROL Use a different value for each conversion],*. 특정 웹 페이지에서 태그를 구현할 때 태그에서 기본값을 트랜잭션 특정 값으로 변경할 수 있습니다.

* *[!UICONTROL Don't use a value for this conversion action (Not recommended)]*

**[!UICONTROL Count]:** [클릭당 또는 상호 작용당 카운트할 전환 수](https://support.google.com/google-ads/answer/3438531): *[!UICONTROL Every (Recommended for every purchases because every purchase is valuable)]* 또는 *[!UICONTROL One (Recommended for leads, sign-ups and other conversions because only the first interaction is valuable)]*.

**[!UICONTROL Click Through Conversion Window]:** 전환이 기록된 광고 상호 작용 후 최대 일 수입니다. 검색, 표시 및 쇼핑 캠페인의 경우 기간은 1~90일 사이일 수 있습니다. 숫자를 선택하거나 **[!UICONTROL Custom]**&#x200B;을(를) 선택하고 숫자를 입력하세요.

**[!UICONTROL View Through Conversion Window]:** 사용자가 광고를 본 후 뷰스루 전환이 기록된 최대 일 수입니다. 검색, 표시 및 쇼핑 캠페인의 경우 기간은 1~90일 사이일 수 있습니다. 숫자를 선택하거나 **[!UICONTROL Custom]**&#x200B;을(를) 선택하고 숫자를 입력하세요.

**[!UICONTROL Attribution Model]:** [각 광고 상호 작용에 필요한 크레딧의 양](https://support.google.com/google-ads/answer/6259715?sjid=8211249329930775138): *[!UICONTROL Data driven]* 또는 *[!UICONTROL Last click]*.

>[!MORELIKETHIS]
>
>* [향상된 전환을 위해 오프라인 전환 데이터 업로드](/help/search-social-commerce/admin/conversion-metrics/upload-data-offline-conversions.md)
>* [잠재 고객에 대한  [!DNL Google Ads] 향상된 전환 구현](/help/search-social-commerce/campaign-management/special-workflows/google-enhanced-conversions-leads.md)
