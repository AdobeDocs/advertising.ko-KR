---
title: (새 UI) 일괄 시트 파일 다운로드/만들기
description: 새 검색, 소셜 및 Commerce UI에서 광고 네트워크에 대한 계정 데이터를 다운로드하여 일괄 시트 파일을 만드는 방법을 알아봅니다.
feature: Search Bulksheets
product_v2: id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2: id: aed5e38a-3e62-42fa-8d16-cd080729b2a0
subfeature_v2: id: e58024d1-d6da-420c-80af-6be211808316id: f3d33161-c519-436e-bbbd-730ba428736b
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 47de92fd6d4b1d481380a58f75ec4735d95fca73
workflow-type: tm+mt
source-wordcount: 1637
ht-degree: 0%

---

# (새 UI) 일괄 시트 파일 다운로드/만들기

하나 이상의 [지원되는 광고 네트워크](about.md#bulksheet-functionality-by-network)에서 하나 이상의 계정에 대한 사용자 지정 설정을 사용하여 일괄 시트를 만들 수 있습니다. Bulksheets에는 검색, 소셜 및 Commerce 내의 데이터가 포함됩니다.

동기화된 캠페인의 경우 선택적으로 데이터를 다운로드하기 전에 광고 네트워크와 동기화하여 광고 네트워크측의 최근 데이터 변경 사항을 포함할 수 있습니다. 모든 광고 네트워크에 대해 선택적으로 파일에 포함할 새 클릭 추적 URL을 생성할 수 있습니다.

1. 주 메뉴에서 **[!UICONTROL Setup]** \> **[!UICONTROL Bulksheets]**&#x200B;을(를) 클릭합니다.

1. 도구 모음에서 **[!UICONTROL Bulk Operations]** \> **[!UICONTROL Download Bulksheet]**&#x200B;을(를) 클릭합니다.

1. [일괄 시트 설정 지정](#bulksheet-settings):

   1. **[!UICONTROL Selections]** 탭에서 일괄 시트 옵션을 포함하고 구성할 계정, 캠페인 또는 광고 그룹을 선택합니다.

   1. (선택 사항) **[!UICONTROL Rows and Columns]** 탭을 클릭하고 일괄 시트에 행을 포함할 계정 구성 요소와 구성 요소 상태를 지정한 다음 선택한 각 구성 요소에 포함할 열을 지정합니다.

      사용 가능한 일괄 시트 행 목록을 보려면 &quot;[광고 네트워크별 일괄 시트 행](#bulksheet-rows-by-ad-network)&quot;을(를) 참조하십시오.

   1. (선택 사항) **[!UICONTROL Filters]** 탭을 클릭한 다음, 일괄 시트에 포함할 특정 캠페인, 광고 그룹, 광고/광고, 키워드, 배치 및 기타 엔터티에 대한 기준을 지정합니다.

1. **[!UICONTROL Download]**&#x200B;을(를) 클릭합니다.

작업이 시작되면 알림이 표시되지만 필요한 경우 추가 일괄 시트를 계속 만들 수 있도록 열린 상태로 유지됩니다. 파일이 생성되면 파일에 대한 링크가 포함된 이메일 알림을 받게 됩니다. 컴파일되는 데이터의 양에 따라 알림이 몇 분 이상 걸릴 수 있습니다. 파일 생성에 실패하면 Bulksheets 보기에 오류 파일이 나열되며 오류 파일에 대한 링크가 포함된 이메일 알림을 받게 됩니다.

## 일괄 시트 설정 {#bulksheet-settings}

### 선택 탭 {#bulksheet-selections-settings}

**\[계정, 캠페인 및 광고 그룹 선택\]**

네트워크 및 계정 계층을 확장한 다음 일괄 시트에 포함할 데이터가 있는 각 계정, 캠페인 또는 광고 그룹 옆의 확인란을 선택합니다.

* 계정에 대한 모든 캠페인 및 광고 그룹을 포함하려면 계정 이름 옆에 있는 확인란을 선택합니다.

* 특정 캠페인을 포함하려면 계정을 확장한 다음 포함할 각 캠페인 옆에 있는 확인란을 선택합니다. 특정 광고 그룹을 포함하려면 캠페인을 더 확장하고 각 광고 그룹 옆에 있는 확인란을 선택합니다.

>[!NOTE]
>
>* 단일 일괄 시트는 여러 광고 네트워크 내의 여러 계정에 적용할 수 있습니다. 광고 네트워크별 열은 광고 네트워크 이름이 있는 일괄 시트로 레이블이 지정됩니다(예: &quot;이동통신사(Google 광고)&quot;).
>* 항목의 구성 요소 유형을 보려면 커서를 그 위에 놓습니다.
>* 기본적으로 활성 및 활성화된 계정과 해당 활성 구성 요소만 나열됩니다.

**[!UICONTROL Generate Tracking URLs]:**(선택 사항) 추적 템플릿이 있는 계정의 추적 템플릿과 랜딩 페이지 접미사(해당 광고 네트워크용) 또는 대상 URL이 있는 계정에 키워드, 광고, 배치, 사이트링크 및 [!DNL Google Ads] 제품 그룹에 대한 추적 코드가 포함된 대상 URL을 포함합니다. 기본적으로 이 옵션이 선택되어 있습니다.

이 옵션을 선택하면 계정 설정 또는 캠페인 설정의 [!UICONTROL Campaign Tracking] 섹션에 있는 매개 변수에 따라 URL이 생성됩니다. 기본적으로 추적 URL이 이미 있는 경우 새 URL이 필요하지 않으면 다시 생성되지 않습니다(예: 키워드 일치 유형, 광고 텍스트 또는 계정의 추적 매개 변수가 변경된 경우).

>[!NOTE]
>
>* 광고주가 Adobe Advertising 전환 추적을 사용하고 관련 계정이 추적 URL을 자동으로 생성 및 업로드하도록 구성되지 않은 경우, 기본 URL이 변경되면 새 추적 URL을 생성해야 합니다.
>* 이 옵션을 선택하지 않으면 나중에 파일을 업로드하거나 게시할 때 추적 URL을 계속 생성할 수 있습니다.

**[!UICONTROL Perform pre-sync]:**(선택 사항) Search, Social 및 Commerce에 모든 데이터가 동일한지 확인하기 위해 해당 파일을 지정된 캠페인과 동기화하도록 지시합니다. 기본적으로 이 옵션은 선택되어 있지 않습니다.

>[!NOTE]
>
>Search, Social 및 Commerce은 하루에 한 번, 광고 네트워크에서 새 캠페인을 감지할 때마다, Search, Social 및 Commerce 내에서 캠페인 데이터를 변경할 때마다 광고 네트워크와 자동으로 동기화됩니다. 캠페인 또는 계정 데이터에 대한 최근 변경 내용이 광고 네트워크에서 직접 이루어졌거나 광고 네트워크의 데스크톱 편집기를 사용했다고 생각되면 이 옵션을 선택합니다. 이 옵션을 선택하면 일괄 시트를 만드는 데 시간이 더 오래 걸립니다.

**[!UICONTROL Bulksheet Name]:** 새 일괄 시트 이름 및 파일 형식입니다. 기본적으로 파일은 탭으로 구분된 값 형식으로 만들어지며 다음 중 하나로 이름이 지정됩니다.

* (광고 네트워크의 모든 계정에 대해) `<search_engine name>_<creation date in the format MMDDYYYY>.tsv`
* (단일 계정의 경우) `<account name>_<search_engine name>_<creation date in the format MMDDYYYY>.tsv`
* (여러 계정의 경우) `MultipleAccounts_<search_engine name>_<creation date in the format MMDDYYYY>.tsv`

파일 이름을 바꿀 수 있습니다. 이름에는 다음 문자를 사용할 수 없습니다. `# % & * | \ : " < > . ? /`

필요한 경우 파일 유형을 변경합니다. 옵션에는 *[!UICONTROL .tsv]*(탭으로 구분된 값), *[!UICONTROL .txt (unicode)]*(유니코드 규격 ASCII 텍스트), *[!UICONTROL .csv]*(쉼표로 구분된 값) 또는 *[!UICONTROL .zip]*(TSV 파일로 압축 해제하는 압축 ZIP 형식)이 있습니다.

>[!TIP]
>
>국제 문자가 포함된 일괄 시트의 경우 TSV 또는 TXT 형식을 사용하십시오.

### 행 및 열 탭 {#bulksheet-rows-columns-settings}

**[!UICONTROL Bulksheet Rows]:** 항목 당 하나의 행이 있는 일괄 시트에서 데이터 행으로 포함할 엔터티 및 해당 상태입니다. 예를 들어 활성 캠페인을 포함하는 경우 일괄 시트에는 활성 캠페인당 하나의 행이 포함됩니다. 선택한 상태의 선택한 엔티티만 포함됩니다. 기본값은 지정된 광고 네트워크를 기반으로 미리 선택됩니다. 기본적으로 선택한 엔티티의 활성 인스턴스만 포함됩니다.

엔티티를 추가하거나 제거하려면 엔티티 옆에 있는 확인란을 선택하거나 선택을 취소합니다. 엔티티에 대한 상태를 추가하거나 제거하려면 엔티티 옆에 있는 상태 메뉴를 클릭한 다음 해당 상태에 대한 확인란을 선택하거나 선택 취소합니다.

광고 네트워크별 사용 가능한 행 목록을 보려면 &quot;[광고 네트워크별 일괄 시트 행](#bulksheet-rows-by-ad-network)&quot;을 참조하십시오.

**[!UICONTROL Cascading Status Hierarchy]:** AND 작업을 사용하여 자식 엔터티를 지정된 부모 엔터티 상태의 하위 엔터티로 필터링합니다. 예를 들어 &quot;활성 캠페인&quot;, &quot;활성 광고 그룹&quot; 및 &quot;활성 키워드&quot;를 선택하면 일괄 시트에는 활성 캠페인의 활성 광고 그룹에 있는 활성 키워드만 포함됩니다.

이 옵션을 선택하지 않으면 상위 상태가 고려되지 않고 필터가 OR 작업을 사용합니다. 예를 들어 &quot;활성 캠페인&quot;, &quot;활성 광고 그룹&quot; 및 &quot;활성 키워드&quot;를 선택하면 일괄 시트에는 모든 활성 캠페인, 상위 캠페인 상태에 관계없이 모든 활성 광고 그룹 및 상위 캠페인 및 광고 그룹 상태에 관계없이 모든 활성 키워드가 포함됩니다.

**[!UICONTROL Bulksheet Columns]:** 다운로드한 일괄 시트 파일에 포함할 열:

* *[!UICONTROL AMO ID]:*(&quot;[!UICONTROL SE ID]&quot;을(를) 선택하지 않은 경우 필수) 각 엔터티/행에 대해 [!DNL Adobe]에서 생성한 고유 식별자를 포함합니다. Search, Social 및 Commerce은 값을 사용하여 편집할 올바른 ID를 결정하지만 광고 네트워크에 게시하지 않습니다. 나중에 엔터티 ID 및 상위 엔터티 ID가 아닌 식별자로 [!UICONTROL AMO ID]을(를) 사용하여 엔터티의 데이터를 편집할 수 있습니다.

* *[!UICONTROL SE ID]:*(&quot;[!UICONTROL AMO ID]&quot;을(를) 선택하지 않은 경우 필수) 포함된 각 열 및 상위 엔터티에 대한 광고 네트워크의 고유 식별자를 포함합니다. 나중에 식별자로 [!UICONTROL SE ID]을(를) 사용하여 엔터티의 데이터를 편집하는 경우 상위 엔터티(해당 [!UICONTROL SE ID] 값 포함)의 행도 포함해야 합니다.

* *[!UICONTROL Platform]:*&#x200B;은(는) 광고 플랫폼(예: &quot;Baidu&quot;)을 나타내기 위해 각 행의 시작 부분에 [!UICONTROL Platform] 열을 포함합니다.

* *[!UICONTROL Acct Name]:*(&quot;[!UICONTROL AMO ID]&quot;을(를) 선택하지 않은 경우 필수) 각 엔터티/행의 광고 네트워크 계정 이름을 포함합니다.

* \[엔터티별 열\]: [!UICONTROL Bulksheet Rows]에서 선택한 각 엔터티와 관련된 모든 열이나 아무 열이나 선택한 열만 포함하려면 엔터티 이름 옆에 있는 ![오른쪽 화살표](/help/search-social-commerce/assets/compressed-item.png "오른쪽 화살표")를 클릭하여 확장한 다음 개별 열의 확인란을 선택하거나 취소합니다. 기본적으로 모든 관련 열이 선택한 각 엔티티 행에 포함됩니다.

>[!TIP]
>
>Bulksheet 파일의 각 행에서 항목을 식별하는 데 충분한 열을 포함해야 합니다. 예를 들어, [!UICONTROL Bulksheet Rows] 선택기당 키워드 행을 포함하지만 모든 키워드 관련 열은 제외하는 경우 결과 일괄 시트에는 특정 행에 속한 키워드 인스턴스를 식별할 수 없는 각 키워드 인스턴스에 대해 하나의 행이 포함됩니다. 이 경우 적절한 ID 열과 값을 수동으로 추가하지 않으면 일괄 시트를 사용하여 데이터를 업데이트할 수 없습니다.

### 필터 탭 {#bulksheet-filters-settings}

일괄 시트에 포함할 특정 캠페인, 광고 그룹, 광고/크리에이티브, 키워드 및/또는 배치에 대한 기준:

1. 매개 변수(엔티티 이름 또는 ID 또는 광고, 키워드 또는 배치의 임의의 요소)를 선택하고 연산자를 선택한 다음 해당 값을 입력합니다.

   예를 들어, [!DNL Google Ads] 계정의 헤드라인에 &quot;shoes&quot;가 있는 광고만 반환하려면 *[!UICONTROL Headline]*&#x200B;을(를) 선택하고 *[!UICONTROL contains]*&#x200B;을(를) 선택한 다음 입력 필드에 `shoes`을(를) 입력합니다.

1. (추가 필터를 적용하려면) 각 추가 필터에 대해 **[!UICONTROL +Add Filter]**&#x200B;을(를) 클릭하고 **[!UICONTROL AND]** 또는 **[!UICONTROL OR]**&#x200B;을(를) 선택한 다음 광고 요소나 키워드 및 연산자를 선택한 다음 적용 가능한 값을 입력하십시오.

## 광고 네트워크별 일괄 시트 행 {#bulksheet-rows-by-ad-network}

| 일괄 시트 행 | [!DNL Baidu] | [!DNL Google Ads] | [!DNL LY Ads] | [!DNL Microsoft Advertising] | [!DNL Naver] | [!DNL Pinterest] | [!DNL Yahoo! Display Network] | [!DNL Yahoo Native] | [!DNL Yandex] | 메모 |
|----|----|----|----|-------|----|----|----|----|----|----|
| [!UICONTROL Campaign] | 예 | 예 | 예 | 예 | 예 | 예 | 예 | 예 | 예 | — |
| [!UICONTROL Adgroup] | 예 | 예 | 예 | 예 | 예 | 예 | 예 | 예 | 예 | — |
| [!UICONTROL Creative] *또는* [!UICONTROL Creative (except RSA)] | 예 | 예 | 예 | 예 | — | — | 예 | 예 | 예 | ([!DNL Google Ads]) [!UICONTROL Responsive Search Ad] 행에서 사용할 수 있는 응답형 검색 광고를 제외한 모든 광고 유형에 사용합니다. |
| [!UICONTROL Responsive Search Ad] | — | 예 | — | 예 | — | — | — | — | — | — |
| [!UICONTROL Keyword] | 예 | 예 | 예 | 예 | 예 | 예 | — | 예 | 예 | 음수가 아닌 키워드에만 사용합니다. 캠페인 또는 광고 그룹 수준에서 만든 부정적 키워드를 보려면 [!UICONTROL Campaign Negative Keyword] 또는 [!UICONTROL Adgroup Negative Keyword] 행을 사용하십시오. |
| [!UICONTROL Promoted Pin] | — | — | — | — | — | 예 | — | — | — | — |
| [!UICONTROL Placement] | — | 예 | — | — | — | — | — | — | — | — |
| [!UICONTROL Auto Target] | — | 예 | — | 예 | — | — | — | — | — | 광고 그룹의 동적 검색 대상에 를 사용합니다. |
| [!UICONTROL Shopping Product Group] | — | 예 | — | 예 | — | — | — | — | — | — |
| [!UICONTROL Campaign Site Link] | — | 예 | — | 예 | — | — | — | 예 | — | — |
| [!UICONTROL Campaign Negative Keyword] | 예 | 예 | 예 | 예 | — | — | — | 예 | — | 캠페인 또는 광고 그룹 수준에서 만든 부정적 키워드에 대해서만 사용합니다. 음수가 아닌 키워드를 보려면 사용 가능한 경우 [!UICONTROL Keyword] 행을 사용하십시오. |
| [!UICONTROL Campaign Negative Website] | — | 예 | — | 예 | — | — | — | 예 | — | — |
| [!UICONTROL Adgroup Site Link] | — | 예 | — | — | — | — | — | 예 | — | — |
| [!UICONTROL Creative Site Link] | — | — | — | — | — | — | — | — | 예 | — |
| [!UICONTROL Adgroup Negative Keyword] | 예 | 예 | 예 | 예 | — | — | — | 예 | — | — |
| [!UICONTROL Adgroup Negative Website] | — | 예 | — | 예 | — | — | — | — | — | — |
| [!UICONTROL Campaign Location Target] | 예 | 예 | 예 | 예 | — | — | — | 예 | — | — |
| [!UICONTROL Adgroup Location Target] | — | — | — | 예 | — | — | — | 예 | — | — |
| [!UICONTROL Campaign Device Target] | — | 예 | — | 예 | — | — | — | 예 | — | — |
| [!UICONTROL Adgroup Device Target] | — | 예 | — | 예 | — | — | — | 예 | — | — |
| [!UICONTROL Campaign RLSA Target] | — | 예 | — | 예 | — | — | — | — | — | — |
| [!UICONTROL Adgroup RLSA Target] | — | 예 | — | 예 | — | — | — | — | — | — |
| [!UICONTROL Campaign RLSA Negative] | — | 예 | — | — | — | — | — | — | — | — |
| [!UICONTROL Adgroup RLSA Negative] | — | 예 | — | — | — | — | — | — | — | — |

각 광고 네트워크의 필수 열과 선택적 열에 대한 자세한 내용은 광고 네트워크별 일괄 시트 데이터 형식 문서를 참조하십시오.

* [ [!DNL Baidu] 계정의 필수 및 선택적 일괄 시트 데이터](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-baidu.md)
* [ [!DNL Google Ads] 계정의 필수 및 선택적 일괄 시트 데이터](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-google.md)
* [ [!DNL LY Ads] 계정의 필수 및 선택적 일괄 시트 데이터](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-yahoo-japan.md)
* [ [!DNL Microsoft Advertising] 계정의 필수 및 선택적 일괄 시트 데이터](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-microsoft.md)
* [ [!DNL Naver] 계정의 필수 및 선택적 일괄 시트 데이터](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-naver.md)
* [ [!DNL Yahoo! Display Network] 계정의 필수 및 선택적 일괄 시트 데이터](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-yahoo-display-network.md)
* [ [!DNL Yandex] 계정의 필수 및 선택적 일괄 시트 데이터](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-yandex.md)

>[!MORELIKETHIS]
>
>* [(새 UI) 일괄 시트를 사용하여 캠페인 데이터 관리에 대해 알아보기](about.md)
>* [(새 UI) 일괄 시트 또는 수정된 오류 파일을 업로드합니다](upload.md)
>* [(새 UI) 게시물 일괄 시트 또는 수정된 오류 파일](post.md)
>* [(새 UI) 일괄 시트 파일의 랜딩 페이지 유효성 검사](validate-landing-pages.md)
