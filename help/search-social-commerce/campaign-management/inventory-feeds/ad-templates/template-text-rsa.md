---
title: 인벤토리 피드에 대한 텍스트 광고 및 반응형 검색 광고 템플릿 설정
description: 재고 피드에 대한 텍스트 광고 및 반응형 검색 광고 템플릿에 대한 설정을 참조하십시오.
exl-id: bf57fbb5-b7b0-4bd6-9dd2-def3825a1da6
feature: Search Inventory Feeds
source-git-commit: 67fe8581832dc0762d62908d01672e53cc95b847
workflow-type: tm+mt
source-wordcount: '3325'
ht-degree: 0%

---

# 인벤토리 피드에 대한 텍스트 광고 및 반응형 검색 광고 템플릿 설정


*[!DNL Google Ads], [!DNL Microsoft Advertising], [!DNL Yahoo! Japan Ads] (삭제 작업만) 및 [!DNL Yandex] 계정만*

>[!NOTE]
>
>* 다음 문자는 템플릿에서 열 이름 및 수정자 이름을 지정하기 위해 예약되어 있으므로 모든 특성 필드에 텍스트로 사용할 수 없습니다. `[ ] < > `
>* [!DNL Yandex templates]에서는 URL에서만 동적 매개 변수 `{param1}` 및 `{param2}`을(를) 사용할 수 있으며 광고 설명에서는 동적 가격 삽입을 사용할 수 없습니다.

## \[모든 탭 위로\]

<!-- **Template Name:** -->

{{$include /help/_includes/inventory-feed-template-name.md}}

<!-- **Status:** -->

{{$include /help/_includes/inventory-feed-template-status.md}}

<!-- **Account:** -->

{{$include /help/_includes/inventory-feed-template-account.md}}

## \[왼쪽 패널\]

<!-- **[!UICONTROL Feed &amp; Columns]:** -->

{{$include /help/_includes/inventory-feed-template-feed-and-columns.md}}

<!-- **[!UICONTROL Modifiers]:** -->

{{$include /help/_includes/inventory-feed-template-modifiers.md}}

## [!UICONTROL Campaigns]

<!-- **[!UICONTROL Campaign]:** -->

{{$include /help/_includes/inventory-feed-template-campaign.md}}

**[!UICONTROL Map Only]:**(선택 사항) 캠페인을 만들지 않고 모든 새 광고 그룹([!DNL Yandex]에서는 사용할 수 없음), 키워드 및 광고를 기존 캠페인에 매핑합니다. 이 옵션을 활성화하면 매핑 방법을 선택합니다.

캠페인 수준에서 [!UICONTROL Map Only]을(를) 사용하려면 제품 분류법과 밀접하게 연결되어 있고 데이터 피드에 쉽게 매핑되는 기존 계정 구조가 필요합니다.

**[!UICONTROL Map Method]:**([!UICONTROL Map Only]이(가) 캠페인에 대해 활성화된 경우) 새 광고 그룹([!DNL Yandex]에는 사용할 수 없음), 키워드 및 광고가 기존 캠페인에 매핑되는 방법:

* *[!UICONTROL Contains Anywhere]:* 이름이 지정된 문자열을 포함하는 기존 캠페인(있는 경우)에 데이터를 추가합니다.

* *[!UICONTROL Contains Exactly]:* 이름이 지정된 문자열을 포함하는 기존 캠페인(있는 경우)에 데이터를 추가합니다.

* *[!UICONTROL Exactly Matches]*(기본값): 같은 이름의 기존 캠페인(있는 경우)에 데이터를 추가합니다.

일치하는 항목이 없으면 캠페인에 대한 모든 데이터가 무시됩니다. 여러 캠페인 일치 항목이 발견되면 키워드 및 광고가 해당 항목 모두에 매핑됩니다.

**[!UICONTROL Campaign Tracking Template]:**(최종/고급 URL만 있는 계정; 선택 사항) 모든 랜딩 도메인 리디렉션 및 추적 매개 변수를 지정하고 매개 변수에 최종 URL을 임베드하는 캠페인 수준 추적 템플릿입니다. 이 값은 계정 수준 설정을 무시하지만, 더 세분화된 수준에서(키워드를 가장 세분화된 수준으로) 추적 템플릿이 이 값을 무시합니다.

* 캠페인 설정에 &quot;[!UICONTROL EF Redirect]&quot; 및 &quot;[!UICONTROL Auto Upload]&quot;이(가) 포함된 경우 적용되는 Adobe Advertising 전환 추적의 경우 레코드를 저장할 때 Search, Social 및 Commerce에서 자동으로 리디렉션 및 추적 코드를 추가합니다.

* 최종 URL을 포함하려면 다음을 수행하십시오.

   * ([!DNL Google Ads] 및 [!DNL Microsoft Advertising]만 해당) 추적 템플릿의 최종 URL을 나타내는 매개 변수 목록은 [[!DNL Google Ads] 설명서](https://support.google.com/google-ads/answer/6305348)의 &quot;사용 가능한 [!DNL ValueTrack] 매개 변수&quot;에 대한 섹션에서 ([!DNL Microsoft Advertising]만 해당) [[!DNL Microsoft Advertising] 설명서](https://help.ads.microsoft.com/#apex/3/en/56799/2) 또는 ([!DNL Google Ads]만 해당) &quot;추적 템플릿 전용&quot; 매개 변수를 참조하십시오.

   * ([!DNL Yahoo! Japan Ads]만 해당) `!{unescapedurl}` 매개 변수를 사용하여 랜딩 페이지 URL을 나타냅니다.

   * 필요에 따라 URL 매개 변수와 캠페인에 대해 정의된 사용자 지정 매개 변수를 앰퍼샌드(&amp;)로 구분하여 포함할 수 있습니다(예: `{lpurl}?matchtype={matchtype}&device={device}`).

* 서드파티 리디렉션 및 추적의 경우 값을 입력합니다.

<!-- **[!UICONTROL Campaign Final URL Suffix]:** -->

{{$include /help/_includes/final-url-suffix.md}}

<!-- **[!UICONTROL Stock Level]:** -->

{{$include /help/_includes/inventory-feed-template-campaign-stock-level.md}}

<!-- **[!UICONTROL This column has non-numeric values]:** -->

{{$include /help/_includes/inventory-feed-template-nonnumeric-values.md}}

### [!UICONTROL Campaign Level Negative Keywords]

{{$include /help/_includes/inventory-feed-template-campaign-negative-keywords.md}}

### [!UICONTROL Manage Settings for NEW Campaigns]

<!-- Flag/check box **[!UICONTROL Manage Settings for NEW Campaigns]:** -->

{{$include /help/_includes/inventory-feed-template-campaign-manage-settings-new-campaigns.md}}

<!-- **[!UICONTROL Initial Budget]:** -->

{{$include /help/_includes/inventory-feed-template-campaign-initial-budget.md}}

**[!UICONTROL Networks]:**([!DNL Google Ads] 및 [!DNL Yandex] 캠페인 설정) 광고를 게재할 네트워크:

* *[!UICONTROL Search]:* 스폰서 검색 목록에 대한 입찰을 실시합니다.

  ([!DNL Google Ads] 캠페인) [!DNL Google Ads] 검색 파트너 목록에 대한 입찰을 포함하려면 **[!UICONTROL Search partners]** 옆에 있는 확인란을 선택하십시오.

* *[!UICONTROL Content]:* 콘텐츠(디스플레이) 네트워크 목록에 배치 입찰을 진행합니다. **참고:** 템플릿을 사용하여 배치를 만들 수 없습니다. 이 옵션을 선택하는 경우 각 광고 그룹에 대한 배치를 만들고 <!-- insert link --> 일괄 시트 또는 <!-- insert links --> 광고 그룹 및 [!UICONTROL Search] > [!UICONTROL Campaigns] 보기의 배치 설정을 사용하여 각 광고 그룹에 대해 타깃팅할 페이지를 표시 네트워크에서 지정합니다.

**[!UICONTROL Languages]:**([!DNL Google Ads] 검색 및 디스플레이 네트워크만 해당) 캠페인의 광고에 대한 하나 이상의 대상 언어입니다.

[!DNL Google Ads]은(는) 사용자의 [!DNL Google] 언어 설정 또는 [!DNL Google Display Network]에 있는 검색 쿼리, 현재 페이지 또는 최근에 본 페이지의 언어에서 사용자의 언어를 결정합니다.

<!-- **[!UICONTROL Locations]:** -->

{{$include /help/_includes/inventory-feed-template-campaign-locations.md}}

## [!UICONTROL Ad Groups]

<!-- **[!UICONTROL Ad Group]:** -->

{{$include /help/_includes/inventory-feed-template-ad-group.md}}

<!-- **[!UICONTROL Map Only]:** -->

{{$include /help/_includes/inventory-feed-template-ad-group-map-only.md}}

<!-- **[!UICONTROL Map Method]:** -->

{{$include /help/_includes/inventory-feed-template-ad-group-map-method.md }}

**[!UICONTROL Ad Group Tracking Template]:**(최종/고급 URL만 있는 계정) 모든 오프랜딩 도메인 리디렉션 및 추적 매개 변수를 지정하고 매개 변수에 최종 URL을 임베드하는 광고 그룹 수준 추적 템플릿입니다.

캠페인 설정에 &quot;[!UICONTROL EF Redirect]&quot; 및 &quot;[!UICONTROL Auto Upload]&quot;이(가) 포함된 경우 적용되는 Adobe Advertising 전환 추적의 경우 레코드를 저장할 때 Search, Social 및 Commerce에서 자동으로 리디렉션 및 추적 코드를 추가합니다.

서드파티 리디렉션 및 추적의 경우 값을 입력합니다. 랜딩 페이지 URL을 나타내려면 다음을 수행합니다.

* Yahoo! Japan Ads 계정에서 매개 변수 {lpurl}을(를) 사용합니다.

* Microsoft Advertising 및 Google Ads 계정에 사용할 수 있는 매개 변수의 경우 [[!DNL Microsoft Advertising] 설명서](https://help.ads.microsoft.com/#apex/3/en/56799) 또는 [[!DNL Google Ads] 설명서](https://support.google.com/google-ads/answer/6305348)의 &quot;사용 가능한 [!DNL ValueTrack] 매개 변수&quot;에 대한 섹션에서 &quot;추적 템플릿만&quot; 매개 변수를 참조하십시오.

이 값은 계정 및 캠페인 수준 설정을 재정의하지만, 더 세분화된 수준에서(키워드를 가장 세분화된 수준으로) 추적 템플릿이 이 값을 재정의합니다.

### [!UICONTROL Ad Group Level Negative Keywords]

{{$include /help/_includes/inventory-feed-template-ad-group-negative-keywords.md}}

### [!UICONTROL Manage Settings for NEW Ad Groups]

<!-- Flag/check box **[!UICONTROL Manage Settings for NEW Ad Groups]:** -->

{{$include /help/_includes/inventory-feed-template-ad-group-manage-settings-new-ad-groups.md}}

<!-- **[!UICONTROL Languages]:** -->

{{$include /help/_includes/inventory-feed-template-ad-group-language-microsoft.md}}

## [!UICONTROL Keywords]

**[!UICONTROL Keywords]:** 지정된 광고 그룹(또는 [!DNL Yandex] 계정에 대한 캠페인)에 대한 키워드입니다. 이 키워드는 정적 텍스트, 지정된 파일의 열 및 수정자의 조합으로 구성될 수 있습니다. 열 이름 및 수정자는 지정된 피드 파일이 템플릿을 통해 전파될 때 실제 데이터로 대체됩니다.

열 이름이나 한정자 그룹을 동적 매개 변수로 삽입하려면 입력 필드를 클릭한 다음 열 목록에서 열 이름을 클릭하거나 한정자 목록에서 [한정자 이름](/help/search-social-commerce/campaign-management/inventory-feeds/modifiers-manage.md)을 클릭합니다. 동일한 키워드에 대해 여러 키워드 또는 여러 일치 유형을 지정하려면 별도의 행에 입력합니다. 키워드 일치 유형을 지정하려면 열 이름 주위에 다음 일치 유형 구문을 사용합니다.

* [!DNL Google Ads], [!DNL Microsoft Advertising] 및 [!DNL Yahoo! Japan Ads] 템플릿의 경우:

   * 동적 매개 변수의 경우: Broad Match = `[keyword]`, [!UICONTROL Keyword] 열의 첫 번째 용어에 대한 Broad Match 수정자(예: +blue suede shoes) = `+[keyword]`, 키워드 열의 각 용어에 대한 Broad Match 수정자(예: +blue +suede +shoes) = `+[keyword]+`, Phrase Match = `"[keyword]"`, Exact Match = `[[keyword]]`

   * 정적 키워드의 경우: Broad Match = `keyword`, Broad Match 수정자 = `+keyword` 또는 Phrase Match = `"keyword"`

     정적 키워드는 동적 매개 변수처럼 대괄호(`[]`)로 둘러싸여 있으므로 여기에 정확한 일치 및 표준 일치 구문으로 입력할 수 없습니다.

* [!DNL Yandex] 템플릿의 경우:

   * 동적 매개 변수의 경우: `[keyword]`과(와) 같은 열 이름을 삽입합니다. 일치 유형을 나타내려면 [[!DNL Yandex]별 구문](https://yandex.com/support/direct/keywords/symbols-and-operators.html)을 사용하십시오. **참고:** 광범위한 일치 용어의 경우 다음 구문을 사용하십시오. Broad Match Modifier for the first term in the Keyword column (예: +blue suede shoes) = `+[keyword]`, Broad Match Modifier for each term in the Keyword column (예: +blue +suede +shoes) = `+[keyword]+`

   * 정적 키워드의 경우: 검색 키워드만 지원됩니다. 키워드에 [[!DNL Yandex]별 구문](https://yandex.com/support/direct/keywords/symbols-and-operators.html)을(를) 사용하십시오. 단어 순서를 나타내는 대괄호(`[]`)는 지원되지 않습니다.

>[!NOTE]
>
>* 키워드 매개 변수 전이나 후에 쉼표로 구분된 값을 괄호로 묶어 키워드 필드에 여러 수정자 값을 수동으로 포함할 수 있습니다(두 위치에 모두 포함되지는 않음). 예를 들어 `(cheap, discount, affordable)[product]`은(는) 각 제품에 대해 세 개의 별도 광고를 생성합니다.
>* 일치 유형을 지정하지 않으면 기본 일치 유형 &quot;broad&quot;가 사용됩니다.
>* 음수 일치는 지원되지 않습니다.
>* 이제 Google broad match 수정자는 일부 언어에 대해 구문 일치와 동일한 일치 동작을 가지며 새 broad match 수정자 키워드를 만들 수 없습니다. 자세한 내용은 [[!DNL Google Ads] 설명서](https://support.google.com/google-ads/answer/10286719)를 참조하세요.

**[!UICONTROL Map Only]:** 새 키워드를 만들지 않고 지정된 키워드가 있는 광고 그룹(또는 [!DNL Yandex] 계정의 캠페인)에 새 광고를 추가합니다. 이 옵션을 활성화하려면 확인란을 선택합니다. 이 옵션을 활성화하면 키워드가 존재하기 때문에 지정된 키워드에 있는 모든 Param 1 및 Param 2 변수가 적용되지 않습니다.

**[!UICONTROL Keyword Final URL]:**(최종/고급 URL이 있는 계정; 선택 사항) 광고 네트워크 사용자가 광고를 클릭할 때 사용하는 랜딩 페이지 URL입니다. 표시 URL과 동일한 도메인을 포함해야 하며 최종 URL의 모든 매개 변수는 광고 클릭 후 랜딩 페이지 URL의 매개 변수와 일치해야 합니다. 랜딩 페이지 도메인 또는 하위 도메인 내에는 리디렉션이 포함될 수 있지만 랜딩 페이지 도메인 외부에는 리디렉션이 포함되지 않습니다.

[!DNL Google Merchant Center] 피드를 사용하고 이 값을 &quot;[!DNL Link]&quot; 열에 포함하는 경우 이 필드에 해당 열을 삽입합니다.

>[!NOTE]
>
>* 템플릿을 통해 전파된 데이터를 게시할 때 추적 URL을 생성하는 경우 계정 추적 설정을 기반으로 추적 매개 변수가 이 값에 추가됩니다.
>* ([!DNL Google Ads] 계정) 병렬 추적을 활성화하는 소스의 클릭에 대체되지 않는 매크로를 사용하지 마십시오. 광고주가 매크로를 사용해야 하는 경우 Adobe 계정 팀은 고객 지원 팀 또는 구현 팀과 협력하여 매크로를 추가해야 합니다.

**[!UICONTROL Keyword Tracking Template]:**(final/advanced URL이 있는 계정; 선택 사항) 모든 오프랜딩 도메인 리디렉션 및 추적 매개 변수를 지정하고 매개 변수에 최종 URL을 임베드하는 추적 템플릿입니다. 가장 세부적인 수준의 추적 템플릿(키워드를 가장 세부적인 수준으로 사용)은 다른 모든 수준의 값을 재정의합니다.

* 캠페인 설정에 &quot;[!UICONTROL EF Redirect]&quot; 및 &quot;[!UICONTROL Auto Upload]&quot;이(가) 포함된 경우 적용되는 Adobe Advertising 전환 추적의 경우 레코드를 저장할 때 Search, Social 및 Commerce에서 자동으로 리디렉션 및 추적 코드를 추가합니다.

* 선택적으로 서드파티 리디렉션 및 추적을 입력할 수 있습니다.

* 랜딩 페이지 URL을 나타내려면 다음을 수행합니다.

   * ([!DNL Google Ads] 및 [!DNL Microsoft Advertising]만 해당) 추적 템플릿의 최종 URL을 나타내는 매개 변수 목록은 [[!DNL Google Ads] 설명서](https://support.google.com/google-ads/answer/6305348)의 &quot;사용 가능한 [!DNL ValueTrack] 매개 변수&quot;에 대한 섹션에서 ([!DNL Microsoft Advertising]만 해당) [[!DNL Microsoft Advertising] 설명서](https://help.ads.microsoft.com/#apex/3/en/56799) 또는 ([!DNL Google Ads]만 해당) &quot;추적 템플릿 전용&quot; 매개 변수를 참조하십시오.

   * ([!DNL Yahoo! Japan Ads]만 해당) `!{lpurl}` 매개 변수를 사용하여 랜딩 페이지 URL을 나타냅니다.

**[!UICONTROL Param 1]**, **[!UICONTROL Param 2]\[[!DNL Google Ads] templates\]:** ([!DNL Google Ads] templates only) 광고 복사본에 포함하거나 템플릿에서 만든 모든 광고의 URL을 표시할 수 있는 [!DNL Google Ads] `{param1}` 또는 `{param2}` 변수를 나타내는 지정된 파일의 열입니다. 동적 매개 변수를 삽입하려면 입력 필드를 클릭한 다음 열 목록에서 열 이름을 클릭합니다. 열 이름은 피드 파일이 템플릿을 통해 전파될 때 실제 데이터로 대체됩니다.

두 매개 변수 중 하나를 사용하는 경우 매개 변수를 새 키워드에만 적용하거나 템플릿에서 만들지 않은 기존 키워드의 값도 업데이트하는 옵션이 있습니다.

* **[!UICONTROL Do Not Apply to Existing Keywords]**(기본값): 템플릿을 사용하여 만든 새 키워드에 대한 매개 변수의 값을 삽입합니다.

* **[!UICONTROL Apply to Existing Keywords: Constant]:** Search, Social 및 Commerce은 피드에서 새 키워드를 만들 뿐만 아니라 템플릿을 사용하여 만들지 않은 광고 그룹의 모든 기존 키워드에 대한 매개 변수의 값도 업데이트합니다. 해당 모든 키워드에 사용되는 단일 숫자 값을 입력합니다. 템플릿에는 하나 이상의 키워드가 포함되어야 합니다.

* **[!UICONTROL Apply to Existing Keywords: Min]:** 피드에서 새 키워드를 만드는 것 외에도 Search, Social 및 Commerce은 피드 파일에 매개 변수에 대한 숫자 값이 들어 있는 한 템플릿을 사용하여 만들지 않은 광고 그룹의 모든 기존 키워드에 대한 매개 변수 값도 업데이트합니다. 여기에는 최대 1개의 소수점이 있지만 쉼표, 통화 기호나 코드 또는 기타 문자가 없습니다. 피드 파일의 매개 변수에 대한 최소값은 모든 기존 키워드에 사용됩니다. 예를 들어 피드 파일에 21500 및 22000 값이 [!UICONTROL Param1]개 있는 경우 기존 키워드의 [!UICONTROL Param1] 값이 21500으로 변경됩니다. 템플릿에는 하나 이상의 키워드가 포함되어야 합니다. **팁:** 키워드의 값이 같도록 테마별로 구성된 광고 그룹이 있는 경우에만 이 옵션을 사용하십시오.

피드 파일의 데이터 필드는 최대 25자일 수 있으며 다음 비숫자 문자가 포함된 숫자 데이터로만 구성될 수 있습니다.

* (매개 변수 &quot;[!UICONTROL Apply to Existing Keywords: Min]&quot;을(를) 사용하는 경우) 최대 소수 첫째 자리까지만 사용할 수 있습니다.

* (&quot;[!UICONTROL Apply to Existing Keywords: Min]&quot; 매개 변수를 사용하지 않는 경우):

   * 통화 기호나 코드 앞에 값을 추가하거나 추가할 수 있습니다. 예를 들어 £2.000,000 및 2000GBP가 유효합니다.

   * 값에는 쉼표(,) 또는 마침표(.)가 포함될 수 있습니다. 선택적 마침표(.)가 있는 구분 기호로 또는 분수 값의 경우 쉼표(,)가 표시됩니다. 예를 들어 1,000.00과 2.000,10이 유효합니다.

   * 값 앞에 퍼센트 기호(%), 더하기 기호(+) 또는 빼기 기호(-)를 붙이거나 붙일 수 있습니다. 예를 들어 20%, 208+ 및 -42.32가 유효합니다.

   * 두 숫자는 슬래시로 포함될 수 있습니다. 예를 들어, 4/1 및 0.95/0.45가 유효합니다.

**[!UICONTROL Param 2]\[[!DNL Microsoft Advertising] templates\]:** ([!DNL Microsoft Advertising] templates only) 제목, 텍스트, 표시 URL 또는 최종 URL에 `{Param2}` 동적 대체 문자열이 포함된 경우 광고에서 대체 값으로 사용할 문자열입니다. 최대 길이는 70자이지만 사용하는 광고 요소의 최대 길이에 유의하십시오(예: 광고 제목에는 최대 25자가 포함될 수 있음).

**[!UICONTROL Param 3]:** ([!DNL Microsoft Advertising] 템플릿만 해당) 제목, 텍스트, 표시 URL 또는 최종 URL에 `{Param3}` 동적 대체 문자열이 포함된 경우 광고에서 대체 값으로 사용할 문자열입니다. 최대 길이는 70자이지만 사용하는 광고 요소의 최대 길이에 유의하십시오(예: 광고 제목에는 최대 25자가 포함될 수 있음).

**[!UICONTROL Initial Bid (&lt;Match Type or Ad Type>)]:** 일치 유형 또는 광고 유형이 지정된 각 키워드에 대한 초기 입찰입니다.

## [!UICONTROL Ads]

**[!UICONTROL Ad Type]:**([!DNL Google Ads] 및 [!DNL Microsoft Advertising] 캠페인만 해당) 광고 유형: *[!UICONTROL Expanded Search Ads]* 또는 *[!UICONTROL Responsive Search Ads]*.

**[!UICONTROL Prefill]:**(선택 사항) 원본 광고 복사 필드의 텍스트로 모든 대체 광고 복사 필드를 미리 채웁니다.

### [!UICONTROL Headlines]

**[!UICONTROL Pin]:**(반응형 검색 광고만 해당) 제목/헤드라인이 포함되어야 하는 광고 위치(예: &quot;[!UICONTROL Pinned at position 1]&quot;). 기본값은 [!UICONTROL Unpinned]입니다.

각 직책에 대해 하나 이상의 제목을 사용할 수 있어야 합니다. 여러 제목을 동일한 위치에 고정하면 최종 광고에는 항상 지정된 위치의 해당 제목 중 하나가 포함됩니다. 위치 3에 고정된 제목은 광고와 함께 표시되지 않을 수 있습니다.

**[!UICONTROL Headline 1]**, **[!UICONTROL Headline 2]**, **[!UICONTROL Headline 3]:**(반응형 검색 광고만 해당) 광고 제목(헤드라인). 각 광고 변형에는 최소 3개 이상, 최대 15개의 광고 제목이 포함되어야 합니다. 광고 네트워크에는 최대 3개의 헤드라인이 있는 광고가 표시됩니다. 각 제목의 최대 길이는 동적 텍스트(예: 키워드 및 광고 사용자 지정 값)를 포함하여 30자입니다.

<!-- using a snippet for the note instead of an include because this is used multiple times on the page, which ExL doesn't support for includes -->

{{inventory-feed-template-insert-ad-customizer}}

**[!UICONTROL Ad Title]:**(기존 Microsoft Advertising 표준 텍스트 광고만, 읽기 전용) 광고의 제목 또는 첫 줄입니다. Microsoft Advertising에서는 표준 텍스트 광고를 더 이상 만들고 편집하지 않습니다.

**[!UICONTROL Headline 1]**, **[!UICONTROL Headline 2]:**([!DNL Google Ads] 및 [!DNL Yahoo! Japan Ads] 확장/확장 텍스트 광고 템플릿만 해당) 광고의 헤드라인입니다. 각 행의 최대 길이는 동적 매개 변수가 대체된 후 30자 또는 15개의 더블바이트 문자입니다.

<!-- using a snippet for the note instead of an include because this is used multiple times on the page, which ExL doesn't support for includes -->

{{inventory-feed-template-insert-dynamic-parameter}}

**[!UICONTROL Headline 3]:**([!DNL Google Ads]개의 확장된 텍스트 광고 템플릿만 해당, 선택 사항) 광고의 세 번째 헤드라인입니다. 최대 길이(동적 매개 변수가 대체된 후)는 30자 또는 15개의 더블바이트 문자입니다.

**[!UICONTROL Title]:** ([!DNL Yandex]만 해당) 광고의 제목 또는 첫 줄입니다. 최대값은 33자입니다.

**[!UICONTROL Title Part 1]**, **[!UICONTROL Title Part 2]:**(Microsoft Advertising 확장 텍스트 광고만 해당) 광고의 헤드라인입니다. 각 행의 최대 길이는 동적 매개 변수가 대체된 후 30자 또는 15개의 더블바이트 문자입니다.

<!-- using a snippet for the note instead of an include because this is used multiple times on the page, which ExL doesn't support for includes -->

{{inventory-feed-template-insert-dynamic-parameter}}

**[!UICONTROL Ad Text]:**(Microsoft Advertising 확장 텍스트 광고만 해당) 광고 본문입니다. 최대 길이(동적 매개 변수가 대체된 후)는 80자 또는 40개의 더블바이트 문자(예: 중국어, 일본어 및 한국어)입니다.

### [!UICONTROL Descriptions]

**[!UICONTROL Description]:** 광고 본문입니다.

* (Google Ads 확장 텍스트 광고 템플릿) 최대 길이(동적 매개 변수가 대체된 후)는 90자 또는 45개의 더블바이트 문자입니다.

* (야후! 일본 광고 템플릿) 최대 길이(동적 매개 변수가 대체된 후)는 80자 또는 40개의 더블바이트 문자입니다.

* (Yandex 템플릿) 최대 길이(동적 매개 변수가 대체된 후)는 75자이며 한 단어는 22자를 초과할 수 없습니다.

<!-- using a snippet for the note instead of an include because this is used multiple times on the page, which ExL doesn't support for includes -->

{{inventory-feed-template-insert-dynamic-parameter}}

**[!UICONTROL Pin]:**(반응형 검색 광고만 해당) 설명을 포함해야 하는 광고 위치입니다(예: &quot;[!UICONTROL Pinned at position 1]&quot;). 기본값은 [!UICONTROL Unpinned]입니다. 각 위치에 대해 하나 이상의 설명을 사용할 수 있어야 합니다.

여러 설명을 동일한 위치에 고정하면 최종 광고는 항상 지정된 위치에 이러한 설명 중 하나를 포함합니다. 위치 2에 고정된 설명은 광고와 함께 표시되지 않을 수 있습니다.

**[!UICONTROL Description 1]**, **[!UICONTROL Description 2]:**(반응형 검색 광고만 해당) 광고 설명. 각 광고 변형에는 최소 2개 이상, 최대 4개의 광고 설명이 포함되어야 합니다. 광고 네트워크에는 최대 2개의 설명과 함께 광고가 표시됩니다. 최소 2개를 입력하십시오. 각 설명의 최대 길이는 동적 텍스트(예: 키워드 및 광고 사용자 값)를 포함하여 90자입니다.

<!-- using a snippet for the note instead of an include because this is used multiple times on the page, which ExL doesn't support for includes -->

{{inventory-feed-template-insert-ad-customizer}}

**[!UICONTROL Description 2]:**(Google 확장 텍스트 광고 템플릿만 해당, 선택 사항) 광고의 두 번째 줄입니다. 최대 길이(동적 매개 변수가 대체된 후)는 90자 또는 45자의 더블바이트입니다.

### [!UICONTROL Path]

**[!UICONTROL Display Path 1]**, **[!UICONTROL Display Path 2]:**(확장된 텍스트 및 반응형 검색 광고만 해당, 선택 사항) 기본 URL 뒤에 연속으로 포함할 하나 또는 두 개의 URL 경로. 광고의 제품 또는 서비스에 대해 보다 자세히 설명해야 합니다. 예를 들어 기본 URL www.example.com에 &quot;Shoes&quot; [!UICONTROL Display Path 1]과(와) &quot;Outdoor&quot; [!UICONTROL Display Path 2]을(를) 추가하면 URL은 www.example.com/Shoes/Outdoor입니다. 각 필드의 최대 길이(동적 매개 변수가 대체된 후)는 15자 또는 7개의 더블바이트 문자입니다.

반응형 검색 광고의 경우 다음 형식을 사용하여 광고 사용자 지정자를 삽입합니다. 여기서 `Default text`은(는) 피드 파일에 유효한 값이 없을 때 삽입할 선택적 값입니다.

* [!DNL Google Ads]: `{CUSTOMIZER.AdCustomizerName:Default text}`(예: `{CUSTOMIZER.Discount:10%}`)

* [!DNL Microsoft Advertising]: `{CUSTOMIZER.Attribute name:Default text}`(예: `{CUSTOMIZER.Discount:10%}`)

**[!UICONTROL Display URL]:**(기존 [!DNL Microsoft Advertising] 및 [!DNL Yahoo! Japan Ads] 표준 텍스트 광고만, 읽기 전용) 광고에 표시되는 URL입니다.

[!DNL Microsoft Advertising] 및 [!DNL Yahoo! Japan Ads]에서는 표준 텍스트 광고를 만들고 편집하는 것을 더 이상 사용하지 않습니다.

**[!UICONTROL Base URL]:**(대상 URL만 있는 계정) 사용자를 가져오는 페이지입니다. 여기에는 서드파티 리디렉션 및 추적 코드가 포함될 수 있습니다. Adobe Advertising 전환 추적 서비스를 사용하고 캠페인 설정에 [!UICONTROL EF Redirect] 사용 및 광고 수준에서 추적 추가가 포함된 경우 검색, 소셜 및 Commerce은 자동으로 자체 리디렉션 및 추적 코드를 광고에 추가합니다.

열 이름이나 한정자 그룹을 동적 매개 변수로 삽입하려면 입력 필드를 클릭한 다음 열 목록에서 열 이름을 클릭하거나 [!UICONTROL Modifiers] 목록에서 [한정자 이름](/help/search-social-commerce/campaign-management/inventory-feeds/modifiers-manage.md)을 클릭합니다.

**[!UICONTROL Final URL]:**(최종/고급 URL이 있는 계정) 사용자가 광고를 클릭할 때 사용하는 랜딩 페이지 URL입니다. 표시 URL과 동일한 도메인을 포함해야 하며 최종 URL의 모든 매개 변수는 광고 클릭 후 랜딩 페이지 URL의 매개 변수와 일치해야 합니다. 랜딩 페이지 도메인 또는 하위 도메인 내에는 리디렉션이 포함될 수 있지만 랜딩 페이지 도메인 외부에는 리디렉션이 포함되지 않습니다.

[!DNL Google Merchant] 센터 피드를 사용하고 이 값을 &quot;[!UICONTROL Link]&quot; 열에 포함하는 경우 이 필드에 해당 열을 삽입합니다.

>[!NOTE]
>
>* 템플릿을 통해 전파된 데이터를 게시할 때 추적 URL을 생성하는 경우 계정 추적 설정에 따라 추적 매개 변수가 이 값에 추가됩니다.
>* ([!DNL Google Ads] 계정 ) 병렬 추적을 활성화하는 소스의 클릭에 대체되지 않는 매크로를 사용하지 마십시오. 광고주가 매크로를 사용해야 하는 경우 Adobe 계정 팀은 고객 지원 팀 또는 구현 팀과 협력하여 매크로를 추가해야 합니다.

**[!UICONTROL Tracking Template]:**(final/advanced URL이 있는 계정; 선택 사항) 모든 오프랜딩 도메인 리디렉션 및 추적 매개 변수를 지정하고 매개 변수에 최종 URL을 임베드하는 추적 템플릿입니다. 가장 세부적인 수준의 추적 템플릿(키워드를 가장 세부적인 수준으로 사용)은 다른 모든 수준의 값을 재정의합니다.

캠페인 설정에 &quot;[!UICONTROL EF Redirect]&quot; 및 &quot;[!UICONTROL Auto Upload]&quot;이(가) 포함된 경우 적용되는 Adobe Advertising 전환 추적의 경우 레코드를 저장할 때 Search, Social 및 Commerce에서 자동으로 리디렉션 및 추적 코드를 추가합니다.

서드파티 리디렉션 및 추적의 경우 값을 입력합니다. 랜딩 페이지 URL을 나타내려면 다음을 수행합니다.

* Yahoo! Japan Ads 계정에서 매개 변수 {lpurl}을(를) 사용합니다.

* Microsoft Advertising 및 Google Ads 계정에 사용할 수 있는 매개 변수의 경우 [[!DNL Microsoft Advertising] 설명서](https://help.ads.microsoft.com/#apex/3/en/56799) 또는 [[!DNL Google Ads] 설명서](https://support.google.com/google-ads/answer/6305348)의 &quot;사용 가능한 [!DNL ValueTrack] 매개 변수&quot;에 대한 섹션에서 &quot;추적 템플릿만&quot; 매개 변수를 참조하십시오.

**\[원본 광고 필드 아래의 대체 광고 필드\]:**(선택 사항) 광고에 대한 대체 광고 복사본 집합입니다. 이 집합은 전달하는 동안 동적 매개 변수가 데이터로 채워지면 원본 광고 복사본에 허용된 최대 길이를 초과하는 경우 사용할 수 있습니다.

>[!NOTE]
>
>* [!UICONTROL Prefill] 옵션을 선택하면 대체 필드가 원본 필드로 미리 채워지며 필요에 따라 편집할 수 있습니다.
>* 최대 길이를 초과하는 광고 복사 필드만 대체 값으로 바뀝니다. 예를 들어 원래 헤드라인이나 제목만 너무 긴 경우 생성된 광고 변형은 대체 헤드라인이나 제목과 원래 설명을 사용합니다. 따라서 대체 광고 사본을 원본 광고 사본과 결합할 때 적절한지 확인하십시오.
>* 원본 광고 사본이 검색 엔진의 길이 요구 사항을 충족하면 대체 광고 사본은 무시됩니다.

**\[Component\] [!UICONTROL Ad Label Classifications] > \[Label Classification and Value\]:**(선택 사항) 템플릿을 사용하여 만들거나 편집한 광고 변형에 할당할 최대 5개의 기존 레이블 분류에 대한 값입니다. 레이블 분류를 지정할 각 캠페인 구성 요소에 대해 다음을 수행합니다.

1. 확인란을 클릭합니다.

1. 광고 변동 템플릿에 대한 레이블 분류 값을 구성합니다.

   * 구성 요소에 지정할 각 레이블 분류 및 값에 대해 다음 작업을 수행하십시오.

      1. **[!UICONTROL Add Label Classification]**&#x200B;을(를) 클릭합니다.

      1. 기존 레이블 분류를 선택한 다음 기존 값을 선택하거나 새 값을 입력합니다.

         각 값의 최대 길이는 100자이며, ASCII 및 비 ASCII 문자를 포함할 수 있습니다.

         레이블 분류 값에 대한 동적 매개 변수로 열 이름을 삽입하려면 입력 필드(두 번째 필드)를 클릭한 다음 열 목록에서 열 이름을 클릭합니다.

         캠페인 구성 요소당 분류당 하나의 값만 포함할 수 있습니다. 예를 들어 캠페인의 Color=Red이지만 Color=Red 및 Color=Blue는 아닐 수 있습니다.

         * 기존 레이블 분류 값을 변경하려면 새 값을 선택하거나 입력합니다.

         * 기존 레이블 분류 값을 제거하려면 값 옆에 있는 **[!UICONTROL X]**&#x200B;을(를) 클릭합니다.

## [!UICONTROL Feed Filters]

<!-- **\[Feed Filter\]:** -->

{{$include /help/_includes/inventory-feed-template-feed-filter.md}}

## [!UICONTROL Label Classifications]

<!-- **\[Component\] [!UICONTROL Label Classifications] &gt; `[Label Classification and Value`]:** -->

{{$include /help/_includes/inventory-feed-template-label-classifications.md}}

>[!MORELIKETHIS]
>
>* [인벤토리 피드를 사용하여 광고 관리 자동화 정보](../inventory-feeds-about.md)
>* [수정자 관리](../modifiers-manage.md)
>* [인벤토리 데이터 피드 파일 관리](/help/search-social-commerce/campaign-management/inventory-feeds/feed-files-manage.md)
>* [템플릿을 통해 피드 데이터 전파](../feed-data-propagate.md)
>* [인벤토리 피드에서 광고 네트워크로 캠페인 데이터 게시](../propagated-data-post.md)
