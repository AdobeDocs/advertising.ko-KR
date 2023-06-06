---
title: 클릭 추적 URL에 대한 선택적 추적 매개 변수
description: 클릭 추적 URL에 추가할 수 있는 선택적 검색, 소셜 및 상거래 추적 매개 변수와 광고 네트워크별 추적 매개 변수에 대해 알아봅니다.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '1211'
ht-degree: 0%

---

# 클릭 추적 URL에 대한 선택적 추적 매개 변수

*Google 광고, Microsoft 광고 및 Yahoo! 일본 계정만*

최종 URL 또는 대상 URL에 대한 표준 추적 매개 변수만 사용하는 대신, 광고 네트워크 계정에 대한 특정 데이터를 추적하기 위해 매개 변수를 더 추가할 수 있습니다. 계정 설정 또는 캠페인 설정에 다음 매개 변수의 조합을 추가할 수 있습니다.

* 정적 텍스트 문자열을 계정/캠페인의 기본 URL에 매개 변수로 추가할 수 있습니다.

* 계정/캠페인의 기본 URL에 Adobe 광고 및 광고 네트워크별 매개 변수를 추가하여 더 많은 데이터를 추적할 수 있습니다.

   * Adobe 광고 매개 변수는 반정적입니다. Adobe 광고는 기본 URL을 광고 네트워크에 업로드할 때 데이터 값을 삽입합니다. 예를 들어 를 추가할 때 `campaign={ef_campaign}` 를 기본 URL로 입력하면 Adobe 광고는 `{ef_campaign}` URL을 업로드할 때 실제 캠페인 이름(예: &quot;Back-to-school-Campaign&quot;)이 사용됩니다.

      **참고:** 값이 삽입되면 정적인 상태로 유지됩니다. 키워드나 광고를 다른 광고 그룹으로 이동하거나 광고 그룹을 다른 캠페인으로 이동하는 경우 {ef_adgroup} 또는 {ef_campaign} 매개 변수는 자동으로 업데이트되지 않으므로 새 대상 URL 또는 기본(최종) URL을 수동으로 생성해야 합니다.

   * 광고 네트워크별 매개 변수는 동적이며 사용자가 광고를 클릭할 때 검색 엔진이 데이터 값을 삽입합니다. 예를 들어 를 추가할 때 `{param1}` 광고 네트워크는 최종 사용자가 광고를 클릭할 때 기본 URL을 실제 {param1} 값으로 대체합니다.

>[!NOTE]
>
>* 여러 매개 변수는 쉼표 또는 앰퍼샌드(`&`).
>* 다음 매개 변수는 대/소문자를 구분하지 않습니다.
>* 추가된 매개 변수의 특수 문자는 생성된 대상 URL 또는 기본(최종) URL에서 다음과 같이 대체됩니다.
>  * `=` 다음으로 대체됨 `%3D`
>  * `?` 다음으로 대체됨 `%26`
>  * 빈 공백은 다음으로 대체됩니다. `%2B`

   >  예를 들어 매개 변수를 추가하는 경우 `campaign={ef_campaign}` 키워드의 기본 URL http://www.example.com에 매핑되면 해당 키워드의 기본 URL이 `http://www.example.com/campaign%3D{ef_campaign}`.


## 검색, 소셜 및 상거래 정적 추적 매개 변수

광고 네트워크의 계정에 대해 다음 매개 변수를 사용할 수 있으며, 필요에 따라 특정 광고 네트워크의 매개 변수와 결합할 수 있습니다. 이러한 매개 변수 중 일부는 계정의 추적 방법이 &quot;&quot;일 때 특정 광고 네트워크에 대해 자동으로 추가되는 매개 변수를 복제합니다[!UICONTROL EF Direct].&quot;

다음 매개 변수는 모두 키-값 쌍으로 지정해야 합니다. 하나의 값 쌍에 여러 매개 변수를 포함할 수 있습니다. 예를 들어 캠페인 이름을 삽입하려면 다음을 사용합니다 `<your_parameter_name>={ef_campaign}`, 예: `campaign={ef_campaign}`. 지정된 일치 유형 이름을 사용하여 일치 유형을 삽입하려면 `<your_parameter_name>={ef_mt_broad:<value>}{ef_mt_exact:<value>}{ef_mt_phrase:<value>}`, 예: `matchtype={ef_mt_broad:<b>}{ef_mt_exact:<e>}{ef_mt_phrase:<p>}`. 적용할 수 없는 일치 유형은 결과 URL에 표시되지 않습니다.

| 매개 변수 | 설명 |
| ---- | ---- |
| {custom_code}</code> | 업로드된 일괄 시트 파일의 &quot;사용자 지정 URL 매개 변수&quot; 열의 데이터를 추적 URL에 삽입하려면 다음을 수행합니다. {custom_code}은(는) 추적 URL에서 하나 이상의 키-값 쌍의 값 끝에서만 사용할 수 있습니다. 예: a={custom_code}</code>; a={ef_campaignid}{custom_code}</code>; a={ef_campaignid}{custom_code}&amp;b={custom_code}</code><br><br><b>참고:</b> 일괄 시트 파일의 사용자 지정 값을 추적 URL에 삽입하려면 &quot;추적 URL 생성&quot; 옵션을 사용하여 일괄 시트 파일을 업로드하십시오. 일괄 시트 파일 사용에 대한 자세한 내용은 &quot;[일괄 시트를 사용하여 캠페인 데이터 관리 기본 정보](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-about.md).&quot; |
| {ef_uniqueid}</code> | Adobe 광고에서 만든 고유 ID를 삽입합니다. 추적 메서드가 &quot;EF Redirect&quot;이면 자동으로 추가됩니다. |
| {ef_userid}</code> | Adobe 광고가 광고주에게 할당하는 고유 사용자 ID를 삽입하기 위해. |
| {ef_sid}</code> | Search, Social 및 Commerce가 광고 네트워크에 할당하는 숫자 ID를 삽입하려면 다음을 수행합니다. <i>[!UICONTROL 3]</i> 대상 [!DNL Google Ads], <i>[!UICONTROL 10]</i> 대상 [!DNL Microsoft® Advertising], <i>[!UICONTROL 45]</i> 대상 [!DNL Meta], <i>[!UICONTROL 86]</i> 대상 [!DNL Yahoo! Display Network], <i>[!UICONTROL 87]</i> 대상 [!DNL Naver], <i>[!UICONTROL 88]</i> 대상 [!DNL Baidu], <i>[!UICONTROL 90]</i> 대상 [!DNL Yandex], <i>[!UICONTROL 94]</i> 대상 [!DNL Yahoo! Japan Ads], <i>[!UICONTROL 105]</i> 대상 [!DNL Yahoo Native] (더 이상 사용되지 않음) 또는 <i>[!UICONTROL 106]</i> 대상 [!DNL Pinterest] (사용하지 않음). |
| {ef_searchengine}</code> | 광고 네트워크 이름을 삽입합니다. |
| {ef_campaign}</code> | 캠페인 이름을 삽입합니다. |
| {ef_campaignid}</code> | 캠페인 ID를 삽입합니다. <b>참고:</b> 새 캠페인에 대한 ID는 캠페인이 광고 네트워크에 게시될 때까지 생성되지 않습니다. 계정이 &quot;EF 리디렉션&quot; 및 &quot;자동 업로드&quot; 옵션을 사용하는 경우, Adobe 광고는 다음날 관련 대상 URL 또는 최종 URL에 캠페인 ID를 자동으로 삽입합니다. 계정이 &quot;EF 리디렉션&quot; 및 &quot;자동 업로드&quot; 옵션을 사용하지 않고 관련 대상 URL 또는 최종 URL에 캠페인 ID를 삽입하려면 캠페인을 만들고, &quot;추적 URL 생성&quot; 옵션을 사용하여 새 캠페인에 대한 일괄 시트 파일을 다운로드한 다음, 파일을 광고 네트워크에 게시해야 합니다. |
| {ef_adgroup}</code> | 광고 그룹 이름을 삽입합니다. |
| {ef_adgroupid}</code> | 광고 그룹 ID를 삽입합니다. <b>참고:</b> 새 광고 그룹의 ID는 광고 그룹이 광고 네트워크에 게시될 때까지 생성되지 않습니다. 계정이 &quot;EF 리디렉션&quot; 및 &quot;자동 업로드&quot; 옵션을 사용하는 경우, Adobe 광고는 다음날 관련 대상 URL 또는 최종 URL에 광고 그룹 ID를 자동으로 삽입합니다. 계정이 &quot;EF 리디렉션&quot; 및 &quot;자동 업로드&quot; 옵션을 사용하지 않고 관련 대상 URL 또는 최종 URL에 광고 그룹 ID를 삽입하려면 광고 그룹을 만들고, &quot;추적 URL 생성&quot; 옵션을 사용하여 새 광고 그룹에 대한 일괄 시트 파일을 다운로드한 다음, 파일을 광고 네트워크에 게시해야 합니다. |
| {ef_keyword}</code> | 키워드를 삽입합니다. |
| {ef_keywordid}</code> | 키워드 ID를 삽입합니다. <b>참고:</b> 새 키워드의 ID는 키워드가 광고 네트워크에 게시될 때까지 생성되지 않습니다. 계정이 &quot;EF 리디렉션&quot; 및 &quot;자동 업로드&quot; 옵션을 사용하는 경우, Adobe 광고는 다음날 관련 대상 URL 또는 최종 URL에 키워드 ID를 자동으로 삽입합니다. 계정이 &quot;EF 리디렉션&quot; 및 &quot;자동 업로드&quot; 옵션을 사용하지 않고 관련 대상 URL 또는 최종 URL에 키워드 ID를 삽입하려면 키워드를 만들고, &quot;추적 URL 생성&quot; 옵션을 사용하여 새 키워드에 대한 일괄 시트 파일을 다운로드한 다음, 파일을 광고 네트워크에 게시해야 합니다. |
| {ef_matchtype}</code> | 키워드 일치 유형을 &quot;Broad&quot;, &quot;Exact&quot; 또는 &quot;Phrase&quot;로 삽입하려면 &quot;EF 리디렉션&quot; 추적 메서드를 사용하여 Google 광고 및 Microsoft 광고에 대해 자동으로 포함됩니다. |
| {ef_adid}</code> | 광고 ID를 삽입합니다. <b>참고:</b> 새 광고에 대한 ID는 광고가 광고 네트워크에 게시될 때까지 생성되지 않습니다. 계정이 &quot;EF 리디렉션&quot; 및 &quot;자동 업로드&quot; 옵션을 사용하는 경우, Adobe 광고는 다음날 관련 대상 URL 또는 최종 URL에 광고 ID를 자동으로 삽입합니다. 계정이 &quot;EF 리디렉션&quot; 및 &quot;자동 업로드&quot; 옵션을 사용하지 않고 관련 대상 URL 또는 최종 URL에 광고 ID를 삽입하려면 광고를 만들고, &quot;추적 URL 생성&quot; 옵션을 사용하여 새 광고에 대한 일괄 시트 파일을 다운로드한 다음, 파일을 광고 네트워크에 게시해야 합니다. |

## Google 광고 동적 추적 매개 변수

다음을 참조하십시오 [https://support.google.com/google-ads/answer/2375447](https://support.google.com/google-ads/answer/2375447).

## Microsoft Advertising 동적 추적 매개 변수

다음을 참조하십시오 [https://help.bingads.microsoft.com/#apex/3/en/51091/2](https://help.bingads.microsoft.com/#apex/3/en/51091/2).

## Yahoo 기본 동적 추적 매개 변수

다음을 참조하십시오 [https://developer.yahoo.com/nativeandsearch/guide/resources/dynamic-parameters](https://developer.yahoo.com/nativeandsearch/guide/resources/dynamic-parameters).

## 야후! 일본 광고 동적 추적 매개 변수

다음을 참조하십시오 [https://help.marketing.yahoo.co.jp/en/?p=115](https://help.marketing.yahoo.co.jp/en/?p=115).

## Yandex 동적 추적 매개 변수

다음을 참조하십시오 [https://yandex.com/support/direct/statistics/url-tags.html](https://yandex.com/support/direct/statistics/url-tags.html).

>[!MORELIKETHIS]
>
>* [Adobe 광고 전환 추적 서비스에 대한 클릭 추적 URL 형식 정보](/help/search-social-commerce/tracking/formats-click-tracking-about.md)

