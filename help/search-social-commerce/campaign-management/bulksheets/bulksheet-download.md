---
title: 일괄 시트 파일 다운로드/만들기
description: 광고 네트워크에 대한 계정 데이터를 다운로드하여 일괄 시트 파일을 만드는 방법을 알아봅니다.
exl-id: 42558276-b930-49de-90a0-445433ee66b9
feature: Search Bulksheets
source-git-commit: 052574217d7ddafb8895c74094da5997b5ff83db
workflow-type: tm+mt
source-wordcount: '1756'
ht-degree: 0%

---

# 일괄 시트 파일 다운로드/만들기

하나 이상의 계정에 대해 사용자 지정 설정을 사용하여 일괄 시트를 만들 수 있습니다 [지원되는 광고 네트워크](bulksheet-about.md#bulksheet-functionality-by-network). Bulksheets에는 검색, 소셜 및 상거래 내의 데이터가 포함됩니다.

동기화된 캠페인의 경우 선택적으로 데이터를 다운로드하기 전에 광고 네트워크와 동기화하여 광고 네트워크측의 최근 데이터 변경 사항을 포함할 수 있습니다. 모든 광고 네트워크에 대해 선택적으로 파일에 포함할 새 클릭 추적 URL을 생성할 수 있습니다.

>[!NOTE]
>
>다음을 수행할 수도 있습니다. [캠페인 관리 보기에 표시되는 열을 기반으로 일괄 시트 파일 만들기](/help/search-social-commerce/common-tasks/navigation-editing-selection/download.md).

1. 메인 메뉴에서 **[!UICONTROL Search]** > **[!UICONTROL Campaigns]** > **[!UICONTROL Bulksheets]**.

1. 도구 모음에서 를 클릭합니다 **[!UICONTROL Download Bulksheet]**.

1. 다음을 지정합니다. [일괄 시트 설정](#bulksheet-download-settings):

1. 다음에서 **[!UICONTROL Selections]** 탭에서 필드에 정보를 입력하거나 선택합니다.

1. (선택 사항) **[!UICONTROL Rows and Columns]** 탭에서 일괄 시트에 행을 포함할 계정 구성 요소와 구성 요소 상태를 지정한 다음 선택한 각 구성 요소에 포함할 열을 지정합니다.

   사용 가능한 일괄 시트 행 목록은 &quot;[광고 네트워크별 일괄 시트 행](#bulksheet-rows-by-ad-network).&quot;

1. (선택 사항) **[!UICONTROL Filters]** 을 탭한 다음, 일괄 시트에 포함할 특정 캠페인, 광고 그룹, 광고/크리에이티브, 키워드, 배치 및 기타 엔티티에 대한 기준을 나타냅니다.

   1. 매개 변수(엔티티 이름 또는 ID, 광고, 키워드 또는 배치의 임의의 요소)를 선택하고 연산자를 선택한 다음 해당 값을 입력합니다. 예를 들어 의 헤드라인에 &quot;shoes&quot;가 있는 광고만 반환하려면 [!DNL Google Ads] 계정, 선택 *제목*, 선택 *[!UICONTROL contains]*&#x200B;을 클릭한 다음 을 입력합니다 `shoes` 입력 필드에서 을 클릭합니다.

   1. (추가 필터를 적용하려면) 각 추가 필터에 대해 **[!UICONTROL +Add Filter]**, 선택 **[!UICONTROL AND]** 또는 **[!UICONTROL OR]**&#x200B;를 클릭하고 광고 요소 또는 키워드와 연산자를 선택한 다음 해당 값을 입력합니다.

1. 클릭 **[!UICONTROL Download]**.

작업이 시작되면 창에 알림이 표시되지만 열려 있으므로 원하는 경우 추가 일괄 시트를 계속 만들 수 있습니다. 선택한 새 계정에 적용할 수 있는 지정된 필터 및 제외는 유지됩니다. 작업이 시작되면 Bulksheets 보기에 파일이 나열됩니다. 파일이 생성되면 파일에 대한 링크가 포함된 이메일 알림을 받게 됩니다. 컴파일되는 데이터의 양에 따라 알림이 몇 분 이상 걸릴 수 있습니다. 그러나 파일 생성에 실패하면 오류 파일이 Bulksheets 보기에 나열되며 오류 파일에 대한 링크가 포함된 이메일 알림을 받게 됩니다.

## 일괄 시트 다운로드 설정 {#bulksheet-download-settings}

| 탭 | 매개 변수 | 설명 |
|----|----|----|
| [!UICONTROL Selections] | [!UICONTROL SE Accounts] | 데이터를 업로드할 계정, 캠페인 또는 광고 그룹:<ul><li>계정과 모든 캠페인 및 광고 그룹을 선택하려면 계정 이름 옆에 있는 확인란을 선택한 다음 >> 를 클릭하여 계정으로 이동합니다. [!UICONTROL Selected Filters] 열.</li><li>개별 캠페인 또는 광고 그룹을 선택하려면 계정 옆에 있는 를 클릭하여 확장한 다음(필요한 경우), 캠페인 옆에 있는 를 클릭하여 확장한 다음, 캠페인 또는 광고 그룹 이름 옆에 있는 확인란을 선택한 다음, >> 를 클릭하여 이동하십시오. [!UICONTROL Selected Filters] 열. 예를 들어, 계정 1에서 캠페인 1에 대한 데이터만 가져오려면 계정 1을 확장하고 캠페인 1 옆의 확인란을 선택한 다음 로 이동합니다. [!UICONTROL Selected Filters] 열.</li></ul><b>참고:</b><ul><li>단일 일괄 시트가 여러 광고 네트워크 내의 여러 계정에 적용될 수 있습니다. 광고 네트워크별 열은 광고 네트워크 이름이 있는 일괄 시트로 레이블이 지정됩니다(예: &quot;이동통신사(Google 광고)&quot;).</li><li>어떤 유형의 구성 요소인지 확인하려면 그 위에 커서를 놓습니다.</li><li>캠페인의 경우, 광고 네트워크 이름의 첫 글자는 의 계정 이름 뒤에 괄호 안에 있습니다(예: &quot;Acme Realty (G)&quot;). [!DNL Google Ads] 계정).</li><li>기본적으로 활성 및 활성화된 계정과 해당 활성 구성 요소만 나열됩니다. 일시 중지 및 삭제된 구성 요소를 보려면 ![아래쪽 화살표](/help/search-social-commerce/assets/arrow-down-expand.png "아래쪽 화살표") 다음에 [!UICONTROL Show] 및 선택 **[!UICONTROL All]. |
| | [!UICONTROL Generate Tracking URLs] | (선택 사항) 추적 템플릿이 있는 계정의 추적 템플릿 및 랜딩 페이지 접미사(적용 가능한 광고 네트워크용) 또는 키워드, 광고, 배치, 사이트링크 및 와 같은 대상 URL이 있는 계정에 포함된 추적 코드가 있는 대상 URL을 포함합니다. [!DNL Google Ads] 일괄 시트의 제품 그룹. 기본적으로 이 옵션이 선택되어 있습니다.<br><br>이 옵션을 선택하면 의 매개 변수에 따라 URL이 생성됩니다. [!UICONTROL Campaign Tracking] 섹션에 있는 마지막 항목이 될 필요가 없습니다. 기본적으로 추적 URL이 이미 있는 경우 새 URL이 필요하지 않으면 다시 생성되지 않습니다(예: 키워드 일치 유형, 광고 텍스트 또는 계정의 추적 매개 변수가 변경된 경우).<br><br><b>참고:</b><ul><li>광고주가 Adobe Advertising 전환 추적을 사용하고 관련 계정이 추적 URL을 자동으로 생성 및 업로드하도록 구성되지 않은 경우, 기본 URL이 변경되면 새 추적 URL을 생성해야 합니다.</li><li>이 옵션을 선택하지 않으면 나중에 파일을 업로드하거나 게시할 때 추적 URL을 계속 생성할 수 있습니다.</li></ul> |
| | [!UICONTROL Perform Pre-sync] | (선택 사항) Search, Social 및 Commerce에 파일을 지정된 캠페인과 동기화하여 모든 데이터가 동일한지 확인합니다. 기본적으로 이 옵션은 선택되어 있지 않습니다.<br><b>참고:</b> 검색, 소셜 및 커머스는 하루에 한 번, 광고 네트워크에서 새 캠페인을 감지할 때마다, 검색, 소셜 및 커머스 내에서 캠페인 데이터를 변경할 때마다 광고 네트워크와 자동으로 동기화됩니다. 캠페인 또는 계정 데이터에 대한 최근 변경 내용이 광고 네트워크에서 직접 이루어졌거나 광고 네트워크의 데스크톱 편집기를 사용했다고 생각되면 이 옵션을 선택합니다. 이 옵션을 선택하면 일괄 시트를 만드는 데 시간이 더 오래 걸립니다. |
| | [!UICONTROL Bulksheet Name] | 새 일괄 시트 이름 및 파일 형식입니다. 기본적으로 파일은 탭으로 구분된 값 형식으로 만들어지며 다음 중 하나로 이름이 지정됩니다.<ul><li>(광고 네트워크의 모든 계정용) `&lt;search_engine name&gt;_&lt;creation date in the format MMDDYYYY&gt;.tsv`</li><li>(단일 계정의 경우) `&lt;account name&gt;_&lt;search_engine name&gt;_&lt;creation date in the format MMDDYYYY&gt;.tsv`</li><li>(여러 계정의 경우) `MultipleAccounts_&lt;search_engine name&gt;_&lt;creation date in the format MMDDYYYY&gt;.tsv`.</li></ul>파일 이름을 바꿀 수 있습니다. 이름에는 다음 문자를 사용할 수 없습니다. `# % &amp; * | \ : &quot; &lt; &gt; . ? or /`.<br><br>필요한 경우 파일 유형을 변경합니다. 옵션은 다음과 같습니다 *[!UICONTROL .tsv]* (탭으로 구분된 값의 경우), *[!UICONTROL .txt]* (유니코드 호환 ASCII 텍스트의 경우), *[!UICONTROL .csv]* (쉼표로 구분된 값의 경우) 또는 *[!UICONTROL .zip]* (TSV 파일로 압축 해제하는 압축 ZIP 형식용).<br><br><b>팁:</b> 국제 문자가 포함된 일괄 시트의 경우 TSV 또는 TXT 형식을 사용하십시오. |
| [!UICONTROL Rows and Columns] | [!UICONTROL Bulksheet Rows] | 항목 당 하나의 데이터 행이 있는 일괄 시트에 포함할 엔티티 및 해당 상태. 예를 들어 활성 캠페인을 포함하는 경우 일괄 시트에는 활성 캠페인당 하나의 행이 포함됩니다. 선택한 상태의 선택한 엔티티만 포함됩니다. 기본값은 지정된 광고 네트워크를 기반으로 미리 선택됩니다. 기본적으로 선택한 엔티티의 활성 인스턴스만 포함됩니다. 사용 가능한 일괄 시트 행 목록은 &quot;[광고 네트워크별 일괄 시트 행](#bulksheet-rows-by-ad-network).&quot;<br><br>엔티티를 추가하거나 제거하려면 엔티티 옆에 있는 확인란을 각각 선택하거나 선택을 취소합니다. 엔티티의 상태를 추가하거나 제거하려면 상태 메뉴 옆의 를 클릭한 다음 엔티티 옆의 확인란을 선택하거나 선택을 취소합니다. |
| | [!UICONTROL Cascading Status Hierarchy] | AND 작업을 사용하여 하위 엔티티의 범위를 지정된 상위 엔티티 상태의 범위로 필터링합니다. 예를 들어 &quot;활성 캠페인&quot;, &quot;활성 광고 그룹&quot; 및 &quot;활성 키워드&quot;를 선택하면 일괄 시트에는 활성 캠페인의 활성 광고 그룹에 있는 활성 키워드만 포함됩니다.<br><br>이 옵션을 선택하지 않으면 상위 상태가 고려되지 않고 필터가 OR 작업을 사용합니다. 예를 들어 &quot;활성 캠페인&quot;, &quot;활성 광고 그룹&quot; 및 &quot;활성 키워드&quot;를 선택하면 일괄 시트에는 모든 활성 캠페인, 상위 캠페인 상태에 관계없이 모든 활성 광고 그룹 및 상위 캠페인 및 광고 그룹 상태에 관계없이 모든 활성 키워드가 포함됩니다. |
| | [!UICONTROL Bulksheet Columns] | 다운로드한 일괄 시트 파일에 포함할 열:<ul><li>*[!UICONTROL AMO ID]*: (다음의 경우 필수)[!UICONTROL SE ID]&quot;선택되지 않음) 다음을 포함 [!DNL Adobe]각 엔티티/행에 대해 생성된 고유 식별자. Search, Social 및 Commerce는 값을 사용하여 편집할 올바른 ID를 결정하지만 광고 네트워크에 게시하지 않습니다. 나중에 를 사용하여 엔티티의 데이터를 편집할 수 있습니다. [!UICONTROL AMO ID] 를 식별자로 사용하십시오.</li><li>*[!UICONTROL SE ID]*: (다음의 경우 필수)[!UICONTROL AMO ID]&quot;선택되지 않음) 포함된 각 열 및 해당 상위 엔티티에 대한 광고 네트워크의 고유 식별자를 포함합니다. 나중에 를 사용하여 엔티티의 데이터를 편집하는 경우 [!UICONTROL SE ID] 식별자로 상위 엔티티(상위 엔티티 포함)에 대한 행도 포함해야 합니다 [!UICONTROL SE ID] 값).</li><li>*[!UICONTROL Platform]*: 다음을 포함합니다. [!UICONTROL Platform column] 각 행의 시작 부분에 광고 플랫폼을 나타냅니다(예: &quot;Baidu&quot;).</li><li>*[!UICONTROL Acct Name]*: (다음의 경우 필수)[!UICONTROL AMO ID]&quot;선택되지 않음) 각 엔티티/행에 대한 광고 네트워크 계정 이름을 포함합니다.</li><li>\[포함할 열\]: 의 선택한 각 엔티티와 관련된 모든 열, 없음 또는 선택한 열만 포함합니다. [!UICONTROL Bulksheet Rows] 섹션. 엔티티와 관련된 개별 열을 보려면 ![오른쪽 화살촉](/help/search-social-commerce/assets/compressed-item.png "오른쪽 화살촉") 엔티티 이름 옆에 있는 을 클릭합니다. 기본적으로 모든 관련 열이 선택한 각 엔티티 행에 포함됩니다. 엔티티 또는 개별 열 옆의 확인란을 선택 취소하여 일괄 시트에서 제외합니다.</li></ul><br><br><b>팁:</b> Bulksheet 파일의 각 행에서 항목을 식별하기 위한 적절한 열을 포함해야 합니다. 예를 들어 [!UICONTROL Bulksheet Rows] 선택기를 사용하지만 모든 키워드 관련 열은 제외됩니다. 결과 일괄 시트에는 각 키워드 인스턴스에 대해 하나의 행이 포함됩니다. 그러나 AMO ID나 SE ID도 아닌 키워드 관련 열이 포함되지 않으므로 특정 행에 관련된 키워드 인스턴스를 식별할 수 없으며, 적절한 ID 열과 값을 수동으로 추가하지 않으면 일괄 시트를 사용하여 데이터를 업데이트할 수 없습니다. |
| [!UICONTROL Filters] | | 일괄 시트에 포함할 특정 캠페인, 광고 그룹, 광고/크리에이티브, 키워드 및/또는 배치에 대한 기준:<ol><li>매개 변수(엔티티 이름 또는 ID 또는 광고, 키워드 또는 배치의 임의의 요소)를 선택하고 연산자를 선택한 다음 해당 값을 입력합니다.<br>예를 들어 의 헤드라인에 &quot;shoes&quot;가 있는 광고만 반환하려면 [!DNL Google Ads] 계정, 선택 *[!UICONTROL Headline]*, 선택 *[!UICONTROL contains]*&#x200B;을 클릭한 다음 을 입력합니다 `shoes` 입력 필드에서 을 클릭합니다.</li><li>(추가 필터를 적용하려면) 각 추가 필터에 대해 **[!UICONTROL +Add Filter]**, 선택 **[!UICONTROL AND]** 또는 **[!UICONTROL OR]**&#x200B;를 클릭하고 광고 요소 또는 키워드와 연산자를 선택한 다음 해당 값을 입력합니다.</li></ul> |

## 광고 네트워크별 일괄 시트 행 {#bulksheet-rows-by-ad-network}

| 일괄 시트 행 | [!DNL Baidu] | [!DNL Google Ads] | [!DNL Microsoft® Advertising] | [!DNL Naver] | [!DNL Pinterest] | [!DNL Yahoo! Display Network] | [!DNL Yahoo! Japan Ads] | [!DNL Yahoo Native] | 얀덱스 | 메모 |
|----|----|----|----|-------|----|----|----|----|----|----|
| [!UICONTROL Campaign] | 예 | 예 | 예 | 예 | 예 | 예 | 예 | 예 | 예 | — |
| [!UICONTROL Adgroup] | 예 | 예 | 예 | 예 | 예 | 예 | 예 | 예 | 예 | — |
| [!UICONTROL Creative] *또는* [!UICONTROL Creative (except RSA)] | 예 | 예 | 예 | — | — | 예 | 예 | 예 | 예 | ([!DNL Google  Ads])에서 사용할 수 있는 반응형 검색 광고를 제외한 모든 광고 유형에 사용합니다. [!UICONTROL Responsive Search Ad] 행. |
| [!UICONTROL Responsive Search Ad] | — | 예 | 예 | — | — | — | — | — | — | — |
| [!UICONTROL Keyword] | 예 | 예 | 예 | 예 | 예 | — | 예 | 예 | 예 | 음수가 아닌 키워드에만 사용합니다. 캠페인 또는 광고 그룹 수준에서 만든 부정적 키워드를 보려면 [!UICONTROL Campaign Negative Keyword] 또는 [!UICONTROL Adgroup Negative Keyword] 가능한 경우 행. |
| [!UICONTROL Promoted Pin] | — | — | — | — | 예 | — | — | — | — | — |
| [!UICONTROL Placement] | — | 예 | — | — | — | — | — | — | — | — |
| [!UICONTROL Auto Target] | — | 예 | 예 | — | — | — | — | — | — | 광고 그룹의 동적 검색 대상에 를 사용합니다. |
| [!UICONTROL Shopping Product Group] | — | 예 | 예 | — | — | — | — | — | — | — |
| [!UICONTROL Campaign Site Link] | — | 예 | 예 | — | — | — | — | 예 | — | — |
| [!UICONTROL Campaign Negative Keyword] | 예 | 예 | 예 | — | — | — | 예 | 예 | — | 캠페인 또는 광고 그룹 수준에서 만든 부정적 키워드에 대해서만 사용합니다. 음수가 아닌 키워드를 보려면 [!UICONTROL Keyword] 가능한 경우 행. |
| [!UICONTROL Campaign Negative Website] | — | 예 | 예 | — | — | — | — | 예 | — | — |
| [!UICONTROL Adgroup Site Link] | — | 예 | — | — | — | — | — | 예 | — | — |
| [!UICONTROL Creative Site Link] | — | — | — | — | — | — | — | — | 예 | — |
| [!UICONTROL Adgroup Negative Keyword] | 예 | 예 | 예 | — | — | — | 예 | 예 | — | — |
| [!UICONTROL Adgroup Negative Website] | — | 예 | 예 | — | — | — | — | — | — | — |
| [!UICONTROL Campaign Location Target] | 예 | 예 | 예 | — | — | — | 예 | 예 | — | — |
| [!UICONTROL Adgroup Location Target] | — | — | 예 | — | — | — | — | 예 | — | — |
| [!UICONTROL Campaign Device Target] | — | 예 | 예 | — | — | — | — | 예 | — | — |
| [!UICONTROL Adgroup Device Target] | — | 예 | 예 | — | — | — | — | 예 | — | — |
| [!UICONTROL Campaign RLSA Target] | — | 예 | 예 | — | — | — | — | — | — | — |
| [!UICONTROL Adgroup RLSA Target] | — | 예 | 예 | — | — | — | — | — | — | — |
| [!UICONTROL Campaign RLSA Negative] | — | 예 | — | — | — | — | — | — | — | — |
| [!UICONTROL Adgroup RLSA Negative] | — | 예 | — | — | — | — | — | — | — | — |

>[!MORELIKETHIS]
>
>* [일괄 시트를 사용하여 캠페인 데이터 관리 기본 정보](bulksheet-about.md)
>* [게시물 일괄 시트 또는 수정된 오류 파일](bulksheet-post.md)
>* [일괄 시트 파일의 랜딩 페이지 유효성 검사](bulksheet-validate-landing-pages.md)
>* [생성 또는 업로드한 일괄 시트 파일 내보내기](bulksheet-export.md)
