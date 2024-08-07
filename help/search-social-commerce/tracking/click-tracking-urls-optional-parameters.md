---
title: 클릭 추적 URL에 대한 선택적 추적 매개 변수
description: 클릭 추적 URL에 추가할 수 있는 선택적 검색, 소셜 및 Commerce 추적 매개 변수와 광고 네트워크별 추적 매개 변수에 대해 알아봅니다.
exl-id: df53bb8c-63ad-47f9-af44-57bd4bd58d71
feature: Search Tracking
source-git-commit: f633f2af545f034b08b378653b4b967710402a03
workflow-type: tm+mt
source-wordcount: '1097'
ht-degree: 0%

---

# 클릭 추적 URL에 대한 선택적 추적 매개 변수

*[!DNL Google Ads], [!DNL Microsoft Advertising], [!DNL Yahoo! Japan] 및 [!DNL Yandex] 계정만*

최종 URL 또는 대상 URL에 대한 표준 추적 매개 변수만 사용하는 대신, 광고 네트워크 계정에 대한 특정 데이터를 추적하기 위해 매개 변수를 더 추가할 수 있습니다. 계정 설정 또는 캠페인 설정에 다음 매개 변수의 조합을 추가할 수 있습니다.

* 정적 텍스트 문자열을 계정/캠페인의 기본 URL에 매개 변수로 추가할 수 있습니다.

* 계정/캠페인의 기본 URL에 Adobe Advertising 및 광고 네트워크별 매개 변수를 추가하여 더 많은 데이터를 추적할 수 있습니다.

   * Adobe Advertising 매개 변수는 반정적입니다. Adobe Advertising은 기본 URL을 광고 네트워크에 업로드할 때 데이터 값을 삽입합니다. 예를 들어 기본 URL에 `campaign={ef_campaign}`을(를) 추가하면 Adobe Advertising은 URL을 업로드할 때 `{ef_campaign}`을(를) 실제 캠페인 이름(예: &quot;Back-to-school-Campaign&quot;)으로 대체합니다.

     **참고:** 값이 삽입되면 정적인 상태로 유지됩니다. 키워드나 광고를 다른 광고 그룹으로 이동하거나 광고 그룹을 다른 캠페인으로 이동하면 {ef_adgroup} 또는 {ef_campaign} 매개 변수가 자동으로 업데이트되지 않으므로 새 대상 URL 또는 기본(최종) URL을 수동으로 생성해야 합니다.

   * 광고 네트워크별 매개 변수는 동적이며 사용자가 광고를 클릭할 때 검색 엔진이 데이터 값을 삽입합니다. 예를 들어 기본 URL에 `{param1}`을(를) 추가하면 광고 네트워크는 최종 사용자가 광고를 클릭할 때 실제 {param1} 값으로 대체합니다.

>[!NOTE]
>
>* 여러 매개 변수는 쉼표 또는 앰퍼샌드(`&`)로 구분하십시오.
>* 다음 매개 변수는 대/소문자를 구분하지 않습니다.
>* 추가된 매개 변수의 특수 문자는 생성된 대상 URL 또는 기본(최종) URL에서 다음과 같이 대체됩니다.
>  * `=`이(가) `%3D`(으)로 대체되었습니다.
>  * `?`이(가) `%26`(으)로 대체되었습니다.
>  * 빈 공백은 `%2B`(으)로 대체됩니다.
>  예를 들어 키워드의 기본 URL http://www.example.com에 매개 변수 `campaign={ef_campaign}`을(를) 추가하면 해당 키워드의 기본 URL이 `http://www.example.com/campaign%3D{ef_campaign}`(으)로 생성됩니다.

## 검색, 소셜 및 Commerce 정적 추적 매개 변수

광고 네트워크의 계정에 대해 다음 매개 변수를 사용할 수 있으며, 필요에 따라 특정 광고 네트워크의 매개 변수와 결합할 수 있습니다. 이러한 매개 변수 중 일부는 계정의 추적 메서드가 &quot;[!UICONTROL EF Direct]&quot;일 때 특정 광고 네트워크에 대해 자동으로 추가된 매개 변수와 중복됩니다.

다음 매개 변수는 모두 키-값 쌍으로 지정해야 합니다. 하나의 값 쌍에 여러 매개 변수를 포함할 수 있습니다. 예를 들어 캠페인 이름을 삽입하려면 `campaign={ef_campaign}`과(와) 같은 `<your_parameter_name>={ef_campaign}`을(를) 사용합니다. 지정된 일치 유형 이름을 사용하여 일치 유형을 삽입하려면 `<your_parameter_name>={ef_mt_broad:<value>}{ef_mt_exact:<value>}{ef_mt_phrase:<value>}`(예: `matchtype={ef_mt_broad:<b>}{ef_mt_exact:<e>}{ef_mt_phrase:<p>}`)을(를) 사용합니다. 적용할 수 없는 일치 유형은 결과 URL에 표시되지 않습니다.

| 매개 변수 | 설명 |
| ---- | ---- |
| <code>{custom_code}</code> | 업로드된 일괄 시트 파일의 &quot;사용자 지정 URL 매개 변수&quot; 열의 데이터를 추적 URL에 삽입하려면 다음을 수행합니다. {custom_code}은(는) 추적 URL에서 하나 이상의 키-값 쌍의 값 끝에서만 사용할 수 있습니다. 예: <code>a={custom_code}</code>; <code>a={ef_campaignid}{custom_code}</code>; <code>a={ef_campaignid}{custom_code}&amp;b={custom_code}</code><br><br><b>참고:</b> 일괄 시트 파일의 사용자 지정 값을 추적 URL에 삽입하려면 &quot;추적 URL 생성&quot; 옵션을 사용하여 일괄 시트 파일을 업로드하십시오. 일괄 시트 파일 사용에 대한 자세한 내용은 &quot;[일괄 시트를 사용한 캠페인 데이터 관리 정보](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-about.md)&quot;를 참조하십시오. |
| <code>{ef_uniqueid}</code> | Adobe Advertising에서 만든 고유 ID를 삽입하려면 추적 메서드가 &quot;EF Redirect&quot;이면 자동으로 추가됩니다. |
| <code>{ef_userid}</code> | Adobe Advertising이 광고주에게 할당하는 고유 사용자 ID를 삽입합니다. |
| <code>{ef_sid}</code> | Search, Social 및 Commerce이 광고 네트워크에 할당하는 숫자 ID를 삽입하려면, [!DNL Google Ads]의 <i>[!UICONTROL 3]</i>, [!DNL Microsoft Advertising]의 <i>[!UICONTROL 10]</i>, [!DNL Meta]의 <i>[!UICONTROL 45]</i>, [!DNL Yahoo! Display Network]의 <i>[!UICONTROL 86]</i>, [!DNL Naver]의 <i>[!UICONTROL 87]</i>, [!DNL Baidu]의 <i>[!UICONTROL 88]</i>, [!DNL Yandex]의 <i>[!UICONTROL 90]</i>, [!DNL Yahoo! Japan Ads]의 <i>[!UICONTROL 94]</i>, [!DNL Yahoo Native]의 <i>[!UICONTROL 105]</i>(더 이상 사용되지 않음) 또는 [!DNL Pinterest]의 <i>[!UICONTROL 106]</i>(더 이상 사용되지 않음)입니다. |
| <code>{ef_searchengine}</code> | 광고 네트워크 이름을 삽입합니다. |
| <code>{ef_campaign}</code> | 캠페인 이름을 삽입합니다. |
| <code>{ef_campaignid}</code> | 캠페인 ID를 삽입합니다. <b>참고:</b> 새 캠페인의 ID는 캠페인이 광고 네트워크에 게시될 때까지 만들어지지 않습니다. 계정에서 &quot;[!UICONTROL EF Redirect]&quot; 및 &quot;자동 업로드&quot; 옵션을 사용하는 경우 Adobe Advertising은 다음날 관련 대상 URL 또는 최종 URL에 캠페인 ID를 자동으로 삽입합니다. 계정에서 &quot;[!UICONTROL EF Redirect]&quot; 및 [!UICONTROL Auto Upload]&quot; 옵션을 사용하지 않고 관련 대상 URL 또는 최종 URL에 캠페인 ID를 삽입하려면 캠페인을 만들고, &quot;추적 URL 생성&quot; 옵션을 사용하여 새 캠페인에 대한 일괄 시트 파일을 다운로드한 다음 파일을 광고 네트워크에 게시해야 합니다. |
| <code>{ef_adgroup}</code> | 광고 그룹 이름을 삽입합니다. |
| <code>{ef_adgroupid}</code> | 광고 그룹 ID를 삽입합니다. <b>참고:</b> 새 광고 그룹의 ID는 광고 그룹이 광고 네트워크에 게시될 때까지 만들어지지 않습니다. 계정에서 &quot;[!UICONTROL EF Redirect]&quot; 및 &quot;자동 업로드&quot; 옵션을 사용하는 경우 Adobe Advertising은 다음날 관련 대상 URL 또는 최종 URL에 광고 그룹 ID를 자동으로 삽입합니다. 계정이 [!UICONTROL EF Redirect]&quot; 및 [!UICONTROL Auto Upload]&quot; 옵션을 사용하지 않고 관련 대상 URL 또는 최종 URL에 광고 그룹 ID를 삽입하려면 광고 그룹을 만들고, &quot;추적 URL 생성&quot; 옵션을 사용하여 새 광고 그룹에 대한 일괄 시트 파일을 다운로드한 다음, 파일을 광고 네트워크에 게시해야 합니다. |
| <code>{ef_keyword}</code> | 키워드를 삽입합니다. |
| <code>{ef_keywordid}</code> | 키워드 ID를 삽입합니다. <b>참고:</b> 새 키워드의 ID는 키워드가 광고 네트워크에 게시될 때까지 만들어지지 않습니다. 계정에서 &quot;[!UICONTROL EF Redirect]&quot; 및 [!UICONTROL Auto Upload]&quot; 옵션을 사용하는 경우 Adobe Advertising은 다음날 관련 대상 URL 또는 최종 URL에 키워드 ID를 자동으로 삽입합니다. 계정에서 &quot;[!UICONTROL EF Redirect]&quot; 및 [!UICONTROL Auto Upload]&quot; 옵션을 사용하지 않고 관련 대상 URL 또는 최종 URL에 키워드 ID를 삽입하려면 키워드를 만들고, &quot;추적 URL 생성&quot; 옵션을 사용하여 새 키워드에 대한 일괄 시트 파일을 다운로드한 다음 파일을 광고 네트워크에 게시해야 합니다. |
| <code>{ef_matchtype}</code> | 키워드 일치 유형을 &quot;Broad&quot;, &quot;Exact&quot; 또는 &quot;Phrase&quot;로 삽입하려면 &quot;[!UICONTROL EF Redirect]&quot; 추적 메서드를 사용하여 [!DNL Google Ads] 및 [!DNL Microsoft Advertising]에 대해 자동으로 포함됩니다. |
| <code>{ef_adid}</code> | 광고 ID를 삽입합니다. <b>참고:</b> 새 광고의 ID는 광고가 광고 네트워크에 게시될 때까지 만들어지지 않습니다. 계정에서 &quot;[!UICONTROL EF Redirect]&quot; 및 [!UICONTROL Auto Upload]&quot; 옵션을 사용하는 경우 Adobe Advertising은 다음날 관련 대상 URL 또는 최종 URL에 광고 ID를 자동으로 삽입합니다. 계정이 &quot;[!UICONTROL EF Redirect]&quot; 및 [!UICONTROL Auto Upload]&quot; 옵션을 사용하지 않고 관련 대상 URL 또는 최종 URL에 광고 ID를 삽입하려면 광고를 만들고, &quot;추적 URL 생성&quot; 옵션을 사용하여 새 광고에 대한 일괄 시트 파일을 다운로드한 다음 파일을 광고 네트워크에 게시해야 합니다. |

## [!DNL Google Ads]개의 동적 추적 매개 변수

[https://support.google.com/google-ads/answer/2375447](https://support.google.com/google-ads/answer/2375447)을(를) 참조하세요.

## [!DNL Microsoft Advertising]개의 동적 추적 매개 변수

[https://help.bingads.microsoft.com/#apex/3/en/51091/2](https://help.bingads.microsoft.com/#apex/3/en/51091/2)을(를) 참조하세요.

## 야후! 일본 광고 동적 추적 매개 변수

[https://ads-help.yahoo-net.jp/s/article/H000044463?language=en_US](https://ads-help.yahoo-net.jp/s/article/H000044463?language=en_US)을(를) 참조하세요.

## [!DNL Yandex]개의 동적 추적 매개 변수

[https://yandex.com/support/direct/statistics/url-tags.html](https://yandex.com/support/direct/statistics/url-tags.html)을(를) 참조하세요.

>[!MORELIKETHIS]
>
>* [Adobe Advertising 전환 추적 서비스의 클릭 추적 URL 형식 정보](/help/search-social-commerce/tracking/formats-click-tracking-about.md)
