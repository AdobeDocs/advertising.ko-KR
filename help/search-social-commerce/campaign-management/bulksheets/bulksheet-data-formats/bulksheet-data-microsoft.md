---
title: ' [!DNL Microsoft Advertising] 계정의 필수 일괄 시트 데이터'
description: ' [!DNL Microsoft Advertising] 계정의 일괄 시트에 있는 필수 머리글 필드 및 데이터 필드를 참조합니다.'
exl-id: 2a5f0e7b-f020-4cca-9b77-807c2ee5c273
feature: Search Bulksheets
source-git-commit: c5739a7c3564f84c57500b54f17ca25591e09a43
workflow-type: tm+mt
source-wordcount: '6934'
ht-degree: 0%

---

# 부록 - [!DNL Microsoft Advertising] 계정에 대한 필수 일괄 시트 데이터

[!DNL Microsoft Advertising] 캠페인 데이터를 일괄적으로 만들고 업데이트하려면 [!DNL Microsoft Advertising] 계정용으로 특별히 형식이 지정된 검색, 소셜 및 Commerce 일괄 시트 파일을 사용할 수 있습니다. a) [기존 계정에 대한 일괄 시트 파일을 필요한 파일 형식으로 생성](../bulksheet-download.md)하거나, b) 수동으로 만들 수 있습니다(&quot;[지원되는 일괄 시트 파일 형식](bulksheet-file-formats.md)&quot;에서 지원되는 파일 형식에 대한 일반 정보를 참조하십시오).

각 일괄 시트에는 수행할 [특정 작업](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-operations.md)에 필요한 헤더 필드와 해당 데이터 필드가 포함되어야 합니다(예: 광고 만들기). 필드가 필요하지 않으면 헤더 및 데이터 행에서 필드를 생략할 수 있습니다. 벌크 시트 파일을 업로드하면 모든 사용자 지정 열이 삭제됩니다.

다음은 사용 가능한 모든 데이터 필드 테이블 및 개별 엔터티(예: 캠페인 및 키워드)에 대한 데이터를 추가, 편집 또는 삭제하는 데 필요한 필드를 나타내는 추가 테이블입니다.

## 사용 가능한 모든 데이터 필드 {#bulksheet-fields-all-microsoft}

다음 표에서는 사용 가능한 모든 데이터 필드에 대해 설명합니다.

계정 엔터티와 관련된 데이터 필드에 대해서는 &quot;[각 계정 구성 요소를 만들거나 편집하거나 삭제하는 데 필요한 필드](#bulksheet-fields-per-component-microsoft)&quot;를 참조하십시오.

| 필드 | 설명 |
|----|----|
| [!UICONTROL Platform] | (정보 목적으로 생성된 일괄 시트에 포함) 광고 플랫폼. 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Acct Name] | 광고 네트워크 계정을 식별하는 고유한 이름. 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 계정에 대한 캠페인을 식별하는 고유한 이름. 최대 길이는 128자입니다. |
| [!UICONTROL Campaign Budget] | 금전적 기호와 문장 부호를 사용하거나 사용하지 않는 일별 또는 월별 캠페인 예산. 0.05보다 작을 수는 없습니다. |
| [!UICONTROL Channel Type] | 캠페인이 타겟팅하는 채널 유형: <i>[!UICONTROL Audience]</i>, <i>[!UICONTROL DynamicSearchAds]</i>, <i>[!UICONTROL Search]</i> 또는 <i>[!UICONTROL Shopping]</i>. |
| [!UICONTROL Delivery Method] | (일일 예산이 있는 캠페인만 해당) 매일 캠페인에 대한 광고를 표시하는 속도:<ul><li><i>[!UICONTROL Standard (Distributed)]</i>(새 캠페인의 기본값): 광고 노출 횟수를 하루 전체에 분산합니다.</li><li><i>[!UICONTROL Accelerated]:</i> 예산에 도달할 때까지 가능한 한 자주 광고를 표시합니다. 그 결과, 오늘 오후에 광고가 표시되지 않을 수 있습니다.</li></ul> |
| [!UICONTROL Campaign Priority] | (쇼핑 캠페인만 해당) 여러 캠페인이 동일한 제품을 광고할 때 사용하는 우선 순위입니다. <i>[!UICONTROL Low]</i>(새 캠페인의 기본값), <i>[!UICONTROL Medium]</i> 또는 <i>[!UICONTROL High]</i>.<br><br>동일한 제품이 두 개 이상의 캠페인에 포함된 경우 광고 네트워크에서는 먼저 캠페인 우선 순위를 사용하여 광고 경매에 적합한 캠페인(및 관련 입찰)을 결정합니다. 모든 캠페인이 동일한 우선 순위를 갖는 경우 입찰이 가장 높은 캠페인이 적격입니다. |
| [!UICONTROL Has EU Political Ads] | (유럽 연합(EU)에서 대상을 타겟팅하는 캠페인에 적용) EU 규정 2024/90: <i>[!UICONTROL Yes]</i> 또는 <i>[!UICONTROL No]</i>에 따라 유럽 연합에서 제공되는 광고에 대한 요구 사항에 따라 캠페인에 정치적 광고가 포함되어 있는지 여부. |
| [!UICONTROL Merchant ID] | (판매자 피드에만 연결된 쇼핑 캠페인 및 대상 캠페인) 캠페인에 제품이 사용되는 판매자 계정의 고객 ID입니다. |
| [!UICONTROL Sales Country] | (쇼핑 캠페인 전용, 기존 캠페인의 경우 읽기 전용) 캠페인의 제품이 판매되는 국가입니다. 제품은 대상 국가와 연결되어 있으므로 이 설정은 캠페인에 광고되는 제품을 결정합니다. |
| [!UICONTROL Product Scope Filter] | (쇼핑 네트워크만 사용하는 캠페인) 판매자 계정의 제품으로서, 캠페인에 대한 제품 광고를 만들 수 있습니다. dimension=attribute 형식을 사용하여 제품을 필터링할 제품 차원 및 속성 조합을 최대 7개까지 입력할 수 있습니다. &quot;>>&quot; 구분 기호로 여러 필터를 구분합니다. 사용 가능한 제품 차원 목록을 보려면 &quot;[쇼핑 캠페인 제품 필터](/help/search-social-commerce/campaign-management/campaigns/shopping-campaign-product-filters.md)&quot;을 참조하세요.<br><br> 예: &quot;`CategoryL1==Animals & Pet Supplies>>CategoryL2=Pet Supplies>>Brand=Acme Pet Supplies`&quot;<br><br> 기존 값을 삭제하려면 값 `[delete]`(대괄호 포함)을(를) 사용하십시오. |
| [!UICONTROL DSA Domain Name] | (a) &quot;<i>[!UICONTROL DynamicSearchAds]</i>&quot; 또는 b) <i>[!UICONTROL Search]</i> 요소가 설정되지 않은 경우 &quot;[!DNL ExperimentId]&quot; 유형의 캠페인) 동적 검색 광고를 타깃팅할 웹 사이트의 도메인 이름입니다. 최대 길이는 2,048자입니다. 도메인 이름에 `www`이(가) 포함된 경우 트리밍되어 사용되지 않습니다.<br><br>기존 캠페인의 경우 도메인을 편집할 수 없지만 다른 속성을 업데이트하려면 도메인을 포함해야 합니다. |
| [!UICONTROL DSA Domain Language] | (a) &quot;<i>[!UICONTROL DynamicSearchAds]</i>&quot; 또는 b) <i>[!UICONTROL Search]</i> 요소가 설정되지 않은 경우 &quot;[!DNL ExperimentId]&quot; 유형의 캠페인) 동적 검색 광고를 타깃팅할 웹 사이트 페이지의 언어입니다. 지원되는 도메인 언어는 [!UICONTROL Dutch], [!UICONTROL English], [!UICONTROL French], [!UICONTROL German], [!UICONTROL Italian], [!UICONTROL Spanish] 및 [!UICONTROL Swedish]입니다.<br><br>기존 캠페인의 경우 언어를 편집할 수 없지만 다른 속성을 업데이트하려면 언어를 포함해야 합니다. |
| [!UICONTROL Ad Group Name] | 광고 그룹을 식별하는 고유한 이름. 최대 길이는 128자입니다. 후행 빈 문자가 저장되지 않습니다(예: &quot;광고 그룹 1&quot;이 &quot;광고 그룹 1&quot;로 저장됨). |
| [!UICONTROL Ad Group Type] | (검색 네트워크의 캠페인, 기존 광고 그룹의 읽기 전용) 광고 그룹 유형은 <i>[!UICONTROL Audience]</i>(대상 캠페인만 해당), <i>[!UICONTROL Search Dynamic]</i>(동적 검색 광고만 해당) 및 <i>[!UICONTROL Search Standard]</i>(반응형 검색 광고 및 기존 확장 텍스트 광고만 해당)입니다. 일부 캠페인 유형에는 여러 광고 그룹 유형이 포함될 수 있습니다. |
| [!UICONTROL Keyword] | (검색 네트워크의 캠페인만 해당) 키워드 문자열입니다. 최대 길이는 50자입니다.<br><br><b>메모:</b><ul><li>광고 그룹 또는 캠페인 수준에서 키워드를 제외하려면 [!UICONTROL Match Type]을(를) `Negative`(으)로 설정합니다. 행에 광고 그룹 이름이 포함된 경우 광고 그룹에 대한 키워드는 제외됩니다. 행에 광고 그룹 이름이 포함되지 않으면 전체 캠페인에 대해 키워드가 제외됩니다.</li><li>[!DNL Microsoft Advertising] 키워드를 변경하면 기존 키워드가 삭제되고 새 키워드 ID로 새 키워드가 만들어집니다. 그러나 일치 유형을 변경해도 기존 키워드는 삭제되지 않습니다.</li></ul> |
| 배치 | 더 이상 사용되지 않음 |
| [!UICONTROL Audience] | 캠페인 또는 광고 그룹의 RLSA(검색 광고) 타겟 대상에 대한 리마케팅 목록입니다. |
| [!UICONTROL Target Type] | (RLSA 대상만 해당) 대상 유형: <i>[!UICONTROL Inclusion]</i> 또는 <i>[!UICONTROL Exclusion]</i>. |
| [!UICONTROL Auto Target Expression] | 광고 그룹에 대한 동적 검색 타겟. 모든 대상에 대해 &quot;[!UICONTROL All Web Pages]&quot;을(를) 사용합니다.<br><br>최대 3개의 동적 검색 조건을 지정하려면 `<category>=<target>` 형식을 사용하십시오. 여기서 &lt;category>에는 아래 범주가 포함될 수 있습니다. &quot;`[blank space] and [blank space]`&quot;을(를) 사용하여 개별 범주에 대한 여러 대상을 조인하고 &quot;`[blank space] and [blank space]`&quot;을(를) 사용하여 여러 범주에 조인합니다.<br><ul><li><i>범주:</i> 특정 Google 콘텐츠 범주가 있는 인덱싱된 페이지에 대한 동적 검색 광고를 표시합니다.</li><li><i>URL:</i> 특정 URL이 있는 인덱싱된 페이지에 대한 동적 검색 광고를 표시합니다. 여기서 값은 URL 내의 어디에나 포함될 수 있습니다.</li><li><i>페이지 제목:</i> 페이지 제목에 특정 텍스트가 있는 인덱싱된 페이지에 대한 동적 검색 광고를 표시합니다.</li><li><i>페이지 콘텐츠:</i> 특정 콘텐츠가 있는 인덱싱된 페이지에 대한 동적 검색 광고를 표시합니다.</li></ul>예: url=shoes.example.com 및 페이지 제목=footwear<br>예: 모든 웹 페이지 |
| [!UICONTROL Location] | 캠페인 또는 광고 그룹에 광고를 배치할 지리적 위치입니다. 값은 대/소문자를 구분하지 않습니다. 캠페인 또는 광고 그룹에 대한 값을 입력하지 않으면 모든 위치가 타깃팅됩니다. 특정 위치를 대상으로 지정하려면 [!DNL Microsoft Advertising] 위치 코드 형식을 사용하여 위치를 입력하십시오. 위치 목록을 다운로드하려면 [!DNL Microsoft Advertising] 광고 계정 자격 증명을 사용하여 [!DNL Microsoft Advertising] 개발자 포털에 로그인하십시오. <b>참고:</b> 위치를 제외하려면 위치 코드 앞에 `-`과 같이 빼기 기호(`-United States`)를 붙입니다. |
| [!UICONTROL Location Type] | 위치 유형(예: 도시, 국가, 도시 지역, 우편 번호 및 주). 위치 목록을 다운로드하려면 [!DNL Microsoft Advertising] 광고 계정 자격 증명을 사용하여 [!DNL Microsoft Advertising] 개발자 포털에 로그인하십시오. |
| [!UICONTROL Match Type] | (검색 네트워크의 캠페인만 해당) 키워드 일치 옵션입니다. 동적 검색 대상 또는 제품 그룹에 대한 키워드 일치 옵션을 포함할 수 있습니다. 값에는 <i>[!UICONTROL Broad]</i>(새 키워드의 기본값), <i>[!UICONTROL Exact]</i>, <i>[!UICONTROL Phrase]</i>, <i>[!UICONTROL Content]</i>(광고 그룹이 콘텐츠 네트워크를 타깃팅할 때 키워드에 대해 자동으로 설정됨), <i>[!UICONTROL Negative]</i>(콘텐츠 네트워크의 키워드를 제외하기 위해), <i>[!UICONTROL Dynamic Ad Target]</i>(새 동적 검색 대상의 기본값), <i>[!UICONTROL Product Group]</i>(새 제품 그룹의 기본값) 또는 <i>[!UICONTROL Negative Product Group]</i>(제품 그룹을 제외하기 위해)이 포함됩니다.  여러 일치 유형이 있는 키워드를 편집하거나 삭제하려면 일치 유형 또는 키워드 ID 값이 필요합니다.<br><br>Broad Match 한정자의 경우 &quot;Broad&quot;를 선택하고 필요한 키워드 내의 단어 앞에 `+`을(를) 삽입하십시오(예: &quot;`+red +shoes`&quot; &quot;red&quot; 및 &quot;shoes&quot; 둘 다 필요).<br><br>[!DNL Microsoft Advertising] 키워드에 대한 일치 형식을 변경해도 기존 키워드는 삭제되지 않습니다. |
| [!UICONTROL Max CPC] | (검색 네트워크의 캠페인) 키워드, 제품 그룹 또는 동적 검색 대상을 기반으로 한 광고 클릭에 대해 지급할 가장 높은 금액인 클릭당 최대 비용(CPC)으로서, 금전 기호와 구두점이 있거나 없습니다.  최적화된 포트폴리오의 기존 키워드 및 제품 그룹 레코드의 경우 업데이트는 하루 동안만 유효하며 다음 최적화 주기 동안 덮어쓰여집니다. <b>참고:</b> 음수 키워드에 대한 입찰을 설정할 수 없습니다. |
| [!UICONTROL Max Content CPC] | (2017년에만 더 이상 사용되지 않는 콘텐츠 네트워크 이전에 생성된 CPC 캠페인의 읽기 전용 ) 금전 기호 및 구두점을 사용하거나 사용하지 않고 디스플레이 네트워크 사이트에서 광고 클릭에 대해 지불하는 가장 높은 금액인 클릭당 최대 콘텐츠 비용(CPC)입니다. |
| [!UICONTROL Audience Target Method] | (대상 광고 그룹):<ul><li><i>[!UICONTROL Target and Bid]:</i> 광고 그룹의 다른 타겟도 충족하는 타겟 대상자와 연결된 사용자에게만 광고를 표시합니다.</li><li><i>[!UICONTROL Bid Only]:</i>다른 광고 그룹 수준의 타겟을 만족시키는 한 타겟 대상자와 연결되지 않은 사람에게도 광고를 표시할 수 있습니다.</li></ul> 그러나 해당 대상자에 대해 더 높은 입찰가를 설정하여 특정 대상자에게 광고가 표시될 가능성을 높일 수 있습니다. |
| [!UICONTROL Parent Product Groupings] | 상위 제품 그룹의 계층입니다.<br><br>예: `All Products>>ProductTypeL1=a>>ProductTypeL2=b` |
| [!UICONTROL Product Grouping] | 제품 그룹(예: &quot;brand=acme&quot; 또는 &quot;모든 제품&quot;).<br><br><b>메모:</b><ul><li>지정된 제품 그룹이 상위 제품 그룹 계층에 없으면 Search, Social 및 Commerce에서 필요한 계층의 일부를 만듭니다.</li><li>기본 입찰이 광고 그룹 기본 입찰로 설정된 쇼핑 캠페인에서 광고 그룹을 만들 때마다 Search, Social 및 Commerce에서 자동으로 &quot;[!UICONTROL All Products]&quot; 그룹을 만듭니다. Search, Social 및 Commerce은 제품 그룹 계층의 각 수준에서 광고 그룹 기본 입찰이 있는 &quot;[!UICONTROL Everything Else]&quot; 그룹을 자동으로 만듭니다. 이러한 기본 그룹을 명시적으로 생성하고 제외하거나 입찰을 변경할 수 있습니다.</li><li>각 광고 그룹은 &quot;[!UICONTROL All Products]&quot; 및 7개의 다른 계층을 포함하여 최대 8개의 제품 그룹 계층을 포함할 수 있습니다.</li></ul> |
| [!UICONTROL Partition Type] | 제품 그룹의 파티션 형식: <i>[!UICONTROL subdivision]</i>(자식 제품 그룹이 있는 경우) 또는 <i>[!UICONTROL unit]</i>(자식 제품 그룹이 없는 경우). |
| [!UICONTROL Ad Title], [!UICONTROL Ad Title 2]-[!UICONTROL Ad Title 15] | (확장된 텍스트 광고, 멀티미디어 광고, 반응형 광고 및 반응형 검색 광고만 해당) 광고의 헤드라인입니다. 각 광고 제목 필드의 최대 길이는 동적 텍스트(예: 키워드 값, `{Param2}` 및 `{Param3}` 동적 대체 변수, 광고 사용자 지정)를 포함하여 30자 또는 15개의 더블바이트 문자입니다.<br><br> 반응형 검색 광고의 경우 다음 형식을 사용하여 광고 사용자 지정자를 삽입합니다. 여기서 &quot;기본 텍스트&quot;는 피드 파일에 유효한 값이 없을 때 삽입할 선택적 값입니다. `{CUSTOMIZER.Attribute name:Default text}, such as {CUSTOMIZER.Discount:10%}`<br><br>확장된 텍스트 광고의 경우 광고 제목 및 광고 제목 2가 필요하며 [!UICONTROL Ad Title 3]은(는) 선택 사항입니다. [!DNL Microsoft Advertising]은(는) 2022년 8월에 확장 텍스트 광고를 더 이상 사용하지 않으며 이제 보고하거나 삭제할 수만 있습니다.<br><br>멀티미디어 광고, 반응형 광고 및 반응형 검색 광고의 경우 [!UICONTROL Ad Title], [!UICONTROL Ad Title 2] 및 [!UICONTROL Ad Title 3]이(가) 필요하며 다른 모든 광고 제목 필드는 선택 사항입니다.<br><br>필수가 아닌 필드의 기존 값을 삭제하려면 값 `[delete]`(대괄호 포함)을 사용하십시오.<br><br>확장된 텍스트 광고를 제외한 모든 광고 유형에 대해 광고 복사본을 변경하면 기존 광고가 삭제되고 동일한 속성을 가진 새 광고가 만들어집니다. |
| [!UICONTROL Ad Title 1 Position]-[!UICONTROL Ad Title 15 Position] | (반응형 검색 광고만 해당, 선택 사항) 해당 광고 제목을 고정할 위치: `[null]`(값 없음, 모든 위치에 대한 광고 제목 가능), 1, 2 또는 3. 예를 들어 [!UICONTROL Ad Title Position]의 값이 1이면 [!UICONTROL Ad Title]은(는) 위치 1에만 나타날 수 있습니다. 기본적으로 모든 광고 제목은 null입니다(값 없음). 기존 값을 삭제하려면 값 `[delete]`(대괄호 포함)을 사용하십시오.<br><br><b>참고:</b> 여러 광고 제목을 같은 위치에 고정할 수 있습니다. 광고 네트워크는 해당 위치에 고정된 광고 제목 중 하나를 사용합니다. 위치 3에 고정된 제목은 광고와 함께 표시되지 않을 수 있습니다. |
| [!UICONTROL Description Line 1]-[!UICONTROL Description Line 4] | (텍스트 광고, 동적 검색 광고, 멀티미디어 광고, 반응형 광고, 반응형 검색 광고 및 향상된 캠페인 수준 사이트링크만 해당) 광고 또는 사이트링크의 본문.<br><br>사이트 링크의 경우 선택적으로 [!UICONTROL Description Line 1]과(와) [!UICONTROL Description Line 2]을(를) 모두 사용하여 광고 네트워크에서 링크 텍스트 아래에 표시할 수 있는 추가 텍스트를 포함합니다. 각 설명 필드에는 최대 35개의 1바이트 문자 또는 17개의 2바이트 문자가 포함될 수 있습니다.<br><br>광고의 경우 각 설명 필드의 최대 길이는 90자 또는 45개의 더블바이트 문자이며, 동적 텍스트(예: 키워드 및 광고 사용자 지정 값)도 포함합니다.<br><br>반응형 검색 광고의 경우 다음 형식을 사용하여 광고 사용자 지정자를 삽입합니다. 여기서 기본 텍스트는 피드 파일에 올바른 값이 포함되지 않았을 때 삽입할 선택적 값입니다. `{CUSTOMIZER.Attribute name:Default text}, such as {CUSTOMIZER.Discount:10%}`<br><br>텍스트 광고 및 동적 검색 광고의 경우 설명 줄 1이 필요하며 [!UICONTROL Description Line 2]은(는) 선택 사항입니다.<br><br>멀티미디어 광고, 반응형 광고 및 반응형 검색 광고의 경우 [!UICONTROL Description Line 1] 및 [!UICONTROL Description Line 2]이(가) 필요하며 [!UICONTROL Description Line 3] 및 [!UICONTROL Description Line 4]은(는) 선택 사항입니다.<br><br>기존 값을 삭제하려면 `[delete]` 값(대괄호 포함)을 사용하십시오.<br><br><b>메모:</b><ul><li>(표준 텍스트 광고) 결합된 제목과 텍스트는 최소 3단어 이상이어야 합니다.</li><li>(확장된 텍스트 광고) 이 필드에는 선택적으로 {Param2} 및 {Param3} 동적 대체 변수가 포함될 수 있습니다. 그럴 경우 광고 텍스트의 최대 길이는 300개의 싱글바이트 문자 또는 150개의 더블바이트 문자입니다. [!DNL Microsoft Advertising]은(는) 2022년 8월에 확장 텍스트 광고를 더 이상 사용하지 않으며 이제 보고하거나 삭제할 수만 있습니다.</li><li>(동적 검색 광고) 동적 대체 텍스트는 허용되지 않습니다.</li><li>확장된 텍스트 광고를 제외한 모든 광고 유형의 경우 광고 사본을 변경하면 기존 광고가 삭제되고 새 광고가 만들어집니다.</li></ul> |
| [!UICONTROL Description Line 1 Position]-[!UICONTROL Description Line 4 Position] | (반응형 검색 광고만 해당, 선택 사항) 해당 설명을 고정할 위치입니다. `[null]`(값 없음, 설명을 모든 위치에 사용할 수 있게 함), 1, 2 또는 3. 예를 들어 [!UICONTROL Description 1 Position]의 값이 1이면 설명 1은 위치 1에만 나타날 수 있습니다. 기본적으로 설명은 위치에 고정되지 않습니다.<br><br>기존 값을 삭제하려면 `[delete]` 값(대괄호 포함)을 사용하십시오.<br><br><b>참고:</b> 동일한 위치에 여러 설명을 고정할 수 있습니다. 광고 네트워크는 해당 위치에 고정된 설명 중 하나를 사용합니다. 위치 2에 고정된 설명은 광고와 함께 표시되지 않을 수 있습니다. |
| [!UICONTROL Business Name] | (멀티미디어 광고만 해당) 비즈니스 이름으로, 최대 25자입니다. |
| [!UICONTROL Promotion Line] | (제품 목록 광고만 해당) 검색 결과의 제품 목록에 포함될 고유한 프로모션 라인(예: &quot;지금 무료 배송!&quot;). 최대 길이는 45자입니다.<br><br>홍보 줄이 페이지에 광고가 표시되는 위치에 따라 광고와 관련된 다른 위치(광고 아래 등)에 표시될 수 있습니다. |
| [!UICONTROL Display URL] | 광고에 포함된 URL.<br><br>확장된 동적 검색 광고의 경우 광고 네트워크는 웹 사이트 도메인에서 동적으로 이 값을 생성하므로 값을 입력할 필요가 없습니다.<br><br>확장된 텍스트 광고 및 반응형 검색 광고의 경우 값을 입력할 필요가 없습니다. 표시 URL은 최종 URL의 도메인에서 자동으로 추출됩니다. 선택적으로 경로 1 및 경로 2 필드를 사용하여 URL을 사용자 지정할 수 있습니다.<br><br><b>메모:</b><ul><li>(최종 URL이 있는 계정) 표시 URL과 최종 URL의 도메인 이름은 일치해야 합니다.</li><li>[!DNL Microsoft Advertising]은(는) 2022년 8월에 확장 텍스트 광고를 더 이상 사용하지 않으며 이제 보고하거나 삭제할 수만 있습니다.</li></ul> |
| [!UICONTROL Display Path 1] | (확장된 텍스트 광고, 동적 검색 광고 및 반응형 검색 광고만 해당) 최종 URL에서 자동으로 추출되는 표시 URL에 추가되는 텍스트. 각 경로는 URL 앞에 슬래시(/)가 붙습니다. 경로에는 슬래시(/) 또는 줄바꿈(\n) 문자를 사용할 수 없습니다. 각 경로의 최대 길이는 15자 또는 7개의 더블바이트 문자입니다.<br><br>광고 사용자 지정기를 삽입하려면 다음 형식을 사용하십시오. 여기서 &quot;기본 텍스트&quot;는 피드 파일에 유효한 값이 포함되지 않은 경우 삽입할 선택적 값입니다. `{CUSTOMIZER.Attribute name:Default text}`(예: `{CUSTOMIZER.Discount:10%}`<br><br>). 예를 들어 [!UICONTROL Display Path 1]이(가) &quot;거래&quot;인 경우 표시 URL은 &lt;display URL>/deals(예: www.example.com/deals)입니다.<br><br>[!DNL Microsoft Advertising]은(는) 2022년 8월에 확장 텍스트 광고를 더 이상 사용하지 않으며 이제 보고하거나 삭제할 수만 있습니다. |
| [!UICONTROL Display Path 1] | (확장된 텍스트 광고, 동적 검색 광고 및 반응형 검색 광고만 해당) 추가 표시 경로입니다. [!UICONTROL Display Path 1]의 항목을 참조하십시오.<br><br>예: [!UICONTROL Display Path 1]이(가) &quot;거래&quot;이고 [!UICONTROL Display Path 2]이(가) &quot;로컬&quot;인 경우 표시 URL은 &lt;<i>표시 URL</i>>/거래/로컬이 됩니다(예: www.example.com/deals/local). |
| [!UICONTROL Start Date] | (향상된 사이트 링크만 해당) 사이트 링크에 대한 입찰이 배치될 수 있는 첫 번째 날짜로 광고주의 시간대 및 m/d/yyyy, m/d/yy, m-d-yyyy 또는 m-d-yy 중 하나입니다. 향상된 새 사이트링크의 기본값은 현재 날짜입니다. <b>참고:</b> 향상된 새 사이트링크는 기존의 향상된 사이트링크가 있거나 사이트링크가 없는 캠페인에서만 만들 수 있습니다. |
| [!UICONTROL End Date] | 광고주의 시간대와 m/d/yyyy, m/d/yy, m-d-yyyy 또는 m-d-yy 형식 중 하나로 사이트 링크가 광고와 함께 표시될 수 있는 마지막 날짜입니다. 새 사이트 링크의 경우 기본값은 `[blank]`입니다(즉, 종료 날짜 없음). |
| [!UICONTROL Call To Action] | 광고에 포함할 call to action. 가능한 값의 목록은 [API 참조를 참조하십시오](https://learn.microsoft.com/en-us/advertising/campaign-management-service/calltoaction). 하지만 작업에 대한 여러 단어 호출을 일괄 시트에 여러 단어(예: &quot;BetNow&quot; 대신 &quot;Bet Now&quot;)로 입력하십시오. |
| [!UICONTROL Call To Action Language] | call to action 옵션의 언어입니다. 가능한 언어 목록은 [API 참조를 참조하십시오](https://learn.microsoft.com/en-us/advertising/campaign-management-service/languagename). |
| [!UICONTROL Base URL/Final URL] | 캠페인 또는 계정에 대해 구성된 추가 매개 변수를 포함하여 검색 엔진 사용자가 광고를 클릭할 때 취하는 랜딩 페이지 URL입니다. 키워드 수준의 기본/최종 URL은 광고 수준 이상의 URL을 재정의합니다.<br><br>기존 값을 삭제하려면 `[delete]` 값(대괄호 포함)을 사용하십시오. |
| [!UICONTROL Destination URL] | (정보 목적으로 생성된 일괄 시트에 포함됨, 검색 엔진에 게시되지 않음) 대상 URL이 있는 계정의 경우, 광고가 광고주 웹 사이트의 기본 URL/랜딩 페이지에 연결되는 URL입니다(경우에 따라 클릭을 추적한 다음 사용자를 랜딩 페이지로 리디렉션하는 다른 사이트를 통해). 여기에는 Search, Social 및 Commerce 캠페인 또는 계정에 대해 구성된 추가 매개 변수가 포함됩니다. 추적 URL을 생성한 경우, 이는 계정 설정 및 캠페인 설정의 추적 매개 변수를 기반으로 합니다. 검색 엔진별 매개 변수를 추가한 경우 이 매개 변수는 검색, 소셜 및 Commerce에 대한 동등한 매개 변수로 대체될 수 있습니다.<br><br>최종 URL이 있는 계정의 경우 이 열은 기본 URL/최종 URL 열과 동일한 값을 표시합니다. |
| [!UICONTROL Custom URL Param] | 변수가 검색 계정 또는 캠페인 설정에 대한 추적 매개 변수에 포함된 경우 `{custom_code}` 동적 변수를 대체할 데이터입니다. 추적 URL에 사용자 지정 값을 삽입하려면 추적 URL 생성 옵션을 사용하여 일괄 시트 파일을 업로드해야 합니다. |
| [!UICONTROL Creative Type] | 광고 형식: <i>[!UICONTROL Dynamic Search Ad]</i>, <i>[!UICONTROL Expanded Text Ad]</i>, <i>[!UICONTROL Expanded Dynamic Search Ad]</i>, <i>[!UICONTROL Multimedia Ad]</i>, <i>[!UICONTROL Product Ad]</i>(쇼핑 광고), <i>[!UICONTROL Responsive Search Ad]</i> 또는 <i>[!UICONTROL Text ad]</i>. 새 광고의 기본값은 <i>[!UICONTROL Text ad]</i>입니다. |
| [!UICONTROL Ad Group Start Date] | 광고주의 시간대 및 m/d/yyyy, m/d/yy, m-d-yyyy 또는 m-d-yy 형식 중 하나로 광고 그룹에 대한 입찰이 배치될 수 있는 첫 번째 날짜입니다. 새 광고 그룹의 경우 기본값은 현재 날짜입니다. |
| [!UICONTROL Ad Group End Date] | 광고주의 시간대와 m/d/yyyy, m/d/yy, m-d-yyyy 또는 m-d-yy 형식 중 하나로 광고 그룹에 대해 입찰이 배치될 수 있는 마지막 날짜입니다. 새 광고 그룹의 경우 기본값은 [blank]입니다(즉, 종료 날짜 없음). |
| [!UICONTROL Tracking Template] | (선택 사항) 모든 오프랜딩 도메인 리디렉션 및 추적 매개 변수를 지정하고 매개 변수에 최종 URL을 임베드하는 추적 템플릿입니다. 가장 세부적인 수준의 추적 템플릿(키워드를 가장 세부적인 수준으로 사용)은 모든 상위 수준의 값을 무시합니다.<br><br>캠페인 설정에 &quot;[!UICONTROL EF Redirect]&quot; 및 &quot;[!UICONTROL Auto Upload]&quot;이(가) 포함된 경우 적용되는 Adobe Advertising 전환 추적의 경우 레코드를 저장할 때 Search, Social 및 Commerce에서 자동으로 리디렉션 및 추적 코드를 추가합니다.<br><br>서드파티 리디렉션 및 추적의 경우 값을 입력하십시오.<br><br>추적 템플릿의 최종 URL을 나타내는 매개 변수 목록을 보려면 [!DNL Microsoft Advertising] 설명서를 참조하십시오.<br><br> 기존 값을 삭제하려면 값 `[delete]`(대괄호 포함)을(를) 사용하십시오. |
| [!UICONTROL Landing Page Suffix] | 정보를 추적하기 위해 최종 URL 끝에 추가할 모든 매개 변수입니다. 예: `param2=value1&param3=value2`<br><br>자세한 내용은 &quot;[클릭 추적 형식 [!DNL Microsoft Advertising]](/help/search-social-commerce/tracking/formats-click-tracking-microsoft.md)을 참조하세요.&quot;<br><br>하위 수준의 최종 URL 접미사가 계정 수준 접미사를 재정의합니다. 간편하게 유지 관리할 수 있도록 개별 계정 구성 요소에 대해 다른 추적이 필요하지 않은 경우 계정 수준 접미사만 사용하십시오. 광고 그룹 수준 이하에서 접미사를 구성하려면 [!DNL Microsoft Advertising] 편집기를 사용하십시오. |
| 네트워크 상태 검색 | 검색 네트워크의 다양한 요소에 광고 그룹을 배치할지 여부:<ul><li><i>모두:</i> 모든 Bing 검색 네트워크 및 신디케이트된 검색 파트너에 광고를 게재합니다.</li><li><i>OwnedAndOperatedOnly:</i>Bing 및 Yahoo에만 광고를 배치합니다. 웹 사이트.</li><li><i>SyndicatedSearchOnly:</i> Bing 및 Yahoo에만 광고를 배치합니다. 신디케이트된 검색 파트너.</li><li><i>해제:</i> 검색 네트워크가 아닌 콘텐츠 네트워크에만 광고를 게재합니다.</li></ul> 새 광고 그룹의 경우 기본값은 [켜짐]입니다. |
| [!UICONTROL Content Network Status] | 더 이상 사용되지 않음 |
| [!UICONTROL Languages] | 광고 그룹의 광고 대상 언어: [!UICONTROL English], [!UICONTROL French], [!UICONTROL Finnish], [!UICONTROL German], [!UICONTROL Norwegian], [!UICONTROL Spanish] 또는 [!UICONTROL Swedish]. 새 캠페인의 기본값은 [!UICONTROL English]입니다.<br><br>이 설정은 광고를 표시할 국가 및 지역을 결정합니다. 캠페인의 위치 대상과 호환되는 언어를 선택해야 합니다. |
| [!UICONTROL Budget Type] | 예산이 <i>[!UICONTROL Daily]</i>(기본값)인지 <i>[!UICONTROL Monthly]</i>인지 여부.<br><br>참고: 최적화된 포트폴리오에 캠페인을 할당하면 이 값은 자동으로 [!UICONTROL Daily]&#x200B;(으)로 설정됩니다. |
| [!UICONTROL Device] | 캠페인 또는 광고 그룹 수준에서 입찰 조정을 수행하는 장치 유형: <i>[!UICONTROL smartphone]</i>, <i>[!UICONTROL tablet]</i> 또는 <i>[!UICONTROL desktop]</i>. |
| [!UICONTROL Bid Adjustment] | 지정된 대상 유형에 대한 입찰 조정입니다. 예를 들어 키워드 수준의 입찰가가 1USD이고 스마트폰 입찰가 조정이 50%라면 스마트폰 입찰가는 1.50USD이다. 기본적으로 모든 타겟은 키워드 수준의 입찰에서 입찰됩니다. 유효한 백분율은 다음과 같습니다.<ul><li>스마트폰 및 태블릿: -100(장치 유형에 대해 입찰하지 않음) 및 -90 ~ 900</li><li>데스크탑: 0 ~ 900</li></ul> |
| [!UICONTROL Creative Preferred Devices] | 광고 또는 사이트 링크를 표시할 장치 유형: <i>[!UICONTROL All]</i>(기본값) 또는 <i>[!UICONTROL Mobile]</i>. 모바일을 지정하면 네트워크에서 데스크탑 또는 태블릿 사용자가 아닌 모바일 장치 사용자에게 광고 또는 사이트링크를 표시하려고 합니다. 그렇지 않으면 네트워크는 모든 디바이스 유형에 광고 또는 사이트링크를 표시합니다. <b>참고:</b> 네트워크에서 기본 장치 유형에 광고를 표시할 수 있는 것은 아닙니다. |
| [!UICONTROL Param2] | 키워드의 기본 URL 또는 광고의 제목, 설명 또는 기본 URL에 `{Param2}` 동적 대체 문자열이 포함된 경우 대체 값으로 사용할 문자열입니다. 최대 길이는 70자이지만 이 길이를 사용하는 광고 요소의 최대 길이에 유의하십시오(예: 제목 1과 제목 2를 합한 길이는 최대 76자일 수 있음). 기존 값을 삭제하려면 값 `[delete]`(대괄호 포함)을 사용하십시오. |
| [!UICONTROL Param3] | 키워드의 기본 URL 또는 광고의 제목, 설명 또는 기본 URL에 `{Param3}` 동적 대체 문자열이 포함된 경우 대체 값으로 사용할 문자열입니다. 최대 길이는 70자이지만 이 길이를 사용하는 광고 요소의 최대 길이에 유의하십시오(예: 제목 1과 제목 2를 합한 길이는 최대 76자일 수 있음). 기존 값을 삭제하려면 값 `[delete]`(대괄호 포함)을 사용하십시오. |
| [!UICONTROL Link Name] | 사이트링크 텍스트입니다. 캠페인 내에서 고유해야 합니다. Description1과 Description2를 지정하는 경우 사이트링크 텍스트에 최대 25개의 싱글바이트 또는 12개의 더블바이트 문자를 포함할 수 있습니다. 그렇지 않으면 사이트링크 텍스트에 최대 35개의 싱글바이트 또는 17개의 더블바이트 문자를 포함할 수 있습니다.<br><br>[!DNL Microsoft Advertising]은(는) 설명이 있는 향상된 사이트링크를 두 개, 네 개 또는 여섯 개, 설명이 없는 단일 행에 광고가 있는 사이트링크를 네 개 또는 여섯 개 표시할 수 있습니다.<br><br>기존의 향상된 사이트 링크가 있거나 사이트 링크가 없는 캠페인에서만 새로운 향상된 사이트 링크를 만들 수 있습니다. |
| [!UICONTROL Campaign Status] | 캠페인의 표시 상태: <i>[!UICONTROL Active]</i>, <i>[!UICONTROL Paused]</i> 또는 <i>[!UICONTROL Deleted]</i>(기존 캠페인만 해당). 새 캠페인의 기본값은 [!UICONTROL Active]입니다. 활성 캠페인이나 일시 중지된 캠페인을 삭제하려면 값 `Deleted`을(를) 입력하십시오. |
| [!UICONTROL Ad Group Status] | 광고 그룹의 표시 상태: <i>[!UICONTROL Active]</i>, <i>[!UICONTROL Paused]</i> 또는 <i>[!UICONTROL Deleted]</i>(기존 광고 그룹만 해당). 새 광고 그룹의 기본값은 [!UICONTROL Active]입니다. 활성 또는 일시 중지된 광고 그룹을 삭제하려면 값 `Deleted`을(를) 입력하십시오. |
| [!UICONTROL Keyword Status] | 키워드의 표시 상태: <i>[!UICONTROL Active]</i>, <i>[!UICONTROL Paused]</i> 또는 <i>[!UICONTROL Deleted]</i>(기존 키워드만 해당). 새 키워드의 기본값은 [!UICONTROL Active]입니다. 활성 또는 일시 중지된 키워드를 삭제하려면 값 `Deleted`을(를) 입력하십시오. <b>참고:</b> 일치 유형이 여러 개인 키워드에 대한 추적 URL을 만드는 경우 각 일치 유형의 키워드 상태는 같아야 합니다. |
| [!UICONTROL Placement Status] | 더 이상 사용되지 않음 |
| [!UICONTROL Ad Status] | 광고의 표시 상태: <i>[!UICONTROL Active]</i>, <i>[!UICONTROL Deleted]</i>(기존 광고만), <i>[!UICONTROL Disapproved]</i>(편집할 수 없음) 또는 <i>[!UICONTROL Paused]</i>. 새 광고의 기본값은 [!UICONTROL Active]입니다. 활성 또는 일시 중지된 광고를 삭제하려면 값 `Deleted`을(를) 입력하십시오. |
| [!UICONTROL Target Status] | 동적 검색 대상의 상태: <i>[!UICONTROL Active]</i>, <i>[!UICONTROL Paused]</i> 또는 <i>[!UICONTROL Deleted]</i>(기존 대상만). 새 대상의 기본값은 [!UICONTROL Active]입니다. 활성 또는 일시 중지된 대상을 삭제하려면 값 `Deleted`을(를) 입력하십시오. |
| [!UICONTROL Sitelink Status] | 사이트 링크의 표시 상태: <i>[!UICONTROL Active]</i> 또는 <i>[!UICONTROL Deleted]</i>(기존 사이트 링크만 해당). 새 사이트 링크의 기본값은 [!UICONTROL Active]입니다. 활성 사이트 링크를 삭제하려면 값 `Deleted`을(를) 입력하십시오. |
| [!UICONTROL Location Status] | 위치 대상의 상태: <i>[!UICONTROL Active]</i> 또는 <i>[!UICONTROL Deleted]</i>(기존 위치만 해당). 새 위치의 기본값은 [!UICONTROL Active]입니다. 활성 위치를 삭제하려면 값 `Deleted`을(를) 입력하십시오. |
| [!UICONTROL Product Group Status] | 제품 그룹의 표시 상태: <i>[!UICONTROL Active]</i> 또는 <i>[!UICONTROL Deleted]</i>(기존 제품 그룹만 해당). 새 제품 그룹의 기본값은 [!UICONTROL Active]입니다. 활성 제품 그룹을 삭제하려면 값 `Deleted`을(를) 입력하십시오. |
| [!UICONTROL Device Target Status] | 캠페인 또는 광고 그룹 수준 장치 대상의 상태: <i>[!UICONTROL Active]</i> 또는 <i>[!UICONTROL Deleted]</i>. 새 캠페인 및 광고 그룹의 경우 기본값은 [!UICONTROL Active]입니다. |
| [!UICONTROL RLSA Target Status] | 캠페인 또는 광고 그룹 수준의 RLSA 대상 또는 (Google 광고만) 제외의 상태: <i>[!UICONTROL Active]</i> 또는 <i>[!UICONTROL Deleted]</i>(기존 대상만). 새 대상 또는 제외의 기본값은 [!UICONTROL Active]입니다. 활성 대상 또는 제외를 삭제하려면 값 `Deleted`을(를) 입력하십시오. |
| \[광고주별 레이블 분류\] | (Color라는 레이블 분류의 경우 &quot;Color&quot;와 같이 광고주별 레이블 분류에 대해 이름이 지정됨) 엔티티와 연결된 지정된 분류의 값입니다. 엔티티당 분류당 하나의 값만 포함할 수 있습니다(예: 캠페인 A의 &quot;색상&quot; 레이블 분류의 경우 &quot;빨간색&quot;). 최대 길이는 100자이고 값에는 ASCII 및 비 ASCII 문자가 포함될 수 있습니다.<br><br>레이블 분류와 해당 레이블 값이 모든 하위 구성 요소에 적용됩니다. 나중에 추가되는 새 구성 요소는 자동으로 레이블과 연결됩니다. 제품 그룹에 대한 레이블 분류는 단위(가장 세부적인) 수준에 적용됩니다.<br><br>분류 이름과 분류 값은 대소문자를 구분하지 않습니다. |
| [!UICONTROL Constraints] | 엔티티에 할당된 제약 조건입니다. 엔티티당 하나의 제약조건만 지정할 수 있습니다.<br><b>>제약 조건은 하위 엔터티에 상속되므로 상속된 값을 재정의하지 않는 한 하위 엔터티의 값을 입력할 필요가 없습니다. |
| [!UICONTROL Campaign ID] | 기존 캠페인을 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 캠페인에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않은 경우 캠페인 이름을 변경할 때만 필요합니다. |
| [!UICONTROL Ad Group ID] | 기존 광고 그룹을 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 광고 그룹에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않은 경우 캠페인 이름을 변경할 때만 필요합니다. |
| [!UICONTROL Placement ID] | 더 이상 사용되지 않음 |
| [!UICONTROL Keyword ID] | 기존 키워드를 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 a) 키워드를 식별할 수 있는 충분한 속성 열 또는 b) &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 키워드를 변경할 때만 필요합니다.&quot; |
| [!UICONTROL Ad ID] | <p>기존 광고를 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 반응형 검색 광고의 경우 광고 데이터를 편집하거나 삭제하려면 광고 ID나 AMO ID가 필요합니다. 다른 모든 엔터티 형식의 경우 행에 a) 광고를 식별할 수 있는 충분한 광고 속성 열 또는 b) &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 광고 상태를 변경할 때만 AMO ID가 필요합니다.&quot; 그러나 [!UICONTROL Ad ID]과(와) [!UICONTROL AMO ID]을(를) 모두 포함하지 않고 광고 속성 열이 여러 광고와 일치하는 경우 광고 중 하나에 대한 상태만 변경됩니다.</p><p><b>참고:</b> a) 기존 광고의 상태를 제외한 광고 속성 열 또는 b) 응답형 검색 광고에 대한 데이터를 편집하고 [!UICONTROL Ad ID] 및 [!UICONTROL AMO ID]을(를) 포함하지 않으면 새 광고가 만들어지고 기존 광고가 변경되지 않습니다. </p> |
| [!UICONTROL Sitelink ID] | 기존 사이트링크를 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 a) 사이트 링크를 식별할 수 있는 충분한 속성 열 또는 b) &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 사이트 링크를 변경하거나 삭제하는 경우에만 필요합니다.&quot; 그러나 [!UICONTROL Sitelink ID]과(와) [!UICONTROL AMO ID]을(를) 모두 포함하지 않고 속성 열이 여러 사이트 링크와 일치하는 경우 사이트 링크 중 하나의 상태만 변경됩니다.</p><p><b>참고:</b> 기존 사이트 링크의 상태를 제외한 사이트 링크 속성 열을 편집하고 [!UICONTROL Sitelink ID] 및 [!UICONTROL AMO ID]을(를) 포함하지 않으면 새 사이트 링크가 만들어지고 기존 사이트 링크는 변경되지 않습니다. |
| [!UICONTROL Product Group ID] | 기존 제품 그룹을 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에는 a) 제품 그룹을 식별하는 데 충분한 속성 열 또는 b) &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 제품 그룹을 변경하거나 삭제할 때만 필요합니다.&quot; |
| 위치 ID | 위치 대상에 대한 고유한 [!DNL Microsoft Advertising] 식별자입니다. 위치 목록을 다운로드하려면 [!DNL Microsoft Advertising] 광고 계정 자격 증명을 사용하여 [!DNL Microsoft Advertising] 개발자 포털에 로그인하십시오. 행에 대상에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않은 경우 위치 대상을 변경하거나 삭제할 때만 필요합니다. |
| [!UICONTROL Target ID] | 기존 자동 타겟을 식별하는 고유 ID입니다. 행에 대상에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 자동 대상을 변경하거나 삭제할 때만 필요합니다. |
| [!UICONTROL RLSA Target ID] | 기존 캠페인 또는 광고 그룹 수준의 RLSA 타겟을 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 대상에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되어 있지 않은 경우 대상 또는 제외를 변경하거나 삭제할 때만 필요합니다. |
| [!UICONTROL AMO ID] | (생성된 일괄 시트에서) 동기화된 엔티티에 대해 Adobe이 생성한 고유 식별자입니다. 반응형 검색 광고의 경우 광고 ID를 포함하지 않는 한 광고를 편집하거나 삭제하려면 AMO ID가 필요합니다. AMO ID가 있는 다른 모든 엔티티 유형의 데이터를 편집하려면 엔티티 ID와 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하려면 AMO ID가 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |
| [!UICONTROL EF Error Message] | (정보 목적으로 생성된 일괄 시트에 포함됨) 행의 데이터에 대한 광고 네트워크의 오류 메시지를 표시하는 자리 표시자입니다. 오류 메시지는 [!UICONTROL EF Errors] 파일에 포함됩니다. 이 값은 광고 네트워크에 게시되지 않습니다. |
| [!UICONTROL SE Error Message] | (정보 목적으로 생성된 일괄 시트에 포함됨) 행의 데이터에 대한 광고 네트워크의 오류 메시지를 표시하는 자리 표시자입니다. 오류 메시지는 [!UICONTROL SE Errors] 파일에 포함됩니다. 이 값은 광고 네트워크에 게시되지 않습니다. |
| [!UICONTROL Exemption Request] | (정보 목적으로 생성된 일괄 시트에 포함됨) 광고가 위반하는 모든 Google 광고 정책의 이름과 텍스트를 표시하는 자리 표시자입니다. |
| [!UICONTROL Retail Hash] | (고급 캠페인 관리를 사용하여 생성된 일괄 시트에 정보 목적으로 포함됨) 고급(ACM) 보기를 사용하여 항목이 생성되었음을 나타내는 영숫자 해시 코드(예: f9639f40cdf56524b541e5dacf55a991). |

[^1]: [!DNL Excel]은(는) 파일을 열 때 큰 숫자를 과학적 표기법(예: 2115585666 2.12E+09)으로 변환합니다. 표준 표기법에서 숫자를 보려면 열에서 셀을 선택하고 수식 입력줄 내부를 클릭합니다.

## 각 계정 구성 요소를 생성, 편집 또는 삭제하는 데 필요한 필드 {#bulksheet-fields-per-component-microsoft}

다음 섹션에는 특정 계정 엔티티와 관련된 필드가 포함되어 있습니다.

>[!NOTE]
>
>필드가 작업에 적용되지 않으면 필드에 입력된 값이 무시됩니다.

### 캠페인 필드

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-microsoft)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수. |
| [!UICONTROL Campaign Budget] | 캠페인을 만드는 데 필요합니다. |
| [!UICONTROL Channel Type] | 캠페인을 만드는 데 필요합니다. |
| [!UICONTROL Delivery Method] | 선택 사항 |
| [!UICONTROL Campaign Priority] | 쇼핑 캠페인을 만드는 데 필요합니다. |
| [!UICONTROL Has EU Political Ads] | 캠페인을 만드는 데 필요합니다. |
| [!UICONTROL Merchant ID] | 쇼핑 캠페인을 만드는 데 필요합니다. |
| [!UICONTROL Sales Country] | 쇼핑 캠페인을 만드는 데 필요합니다. |
| [!UICONTROL Product Scope Filter] | (쇼핑 캠페인) 선택 사항 |
| [!UICONTROL DSA Domain Name] | [!UICONTROL DynamicSearchAds] 요소가 설정되지 않은 경우 a) &quot;[!UICONTROL Search]&quot; 또는 b) &quot;[!DNL ExperimentId]&quot; 유형의 캠페인을 만드는 데 필요합니다. |
| [!UICONTROL DSA Domain Language] | [!UICONTROL DynamicSearchAds] 요소가 설정되지 않은 경우 a) &quot;[!UICONTROL Search]&quot; 또는 b) &quot;[!DNL ExperimentId]&quot; 유형의 캠페인을 만드는 데 필요합니다. |
| [!UICONTROL Tracking Template] | 선택 사항 |
| [!UICONTROL Landing Page Suffix] | <p>선택 사항 |
| [!UICONTROL Budget Type] | 캠페인을 만드는 데 필요합니다. |
| [!UICONTROL Device] | 선택 사항 |
| [!UICONTROL Bid Adjustment] | 선택 사항 |
| [!UICONTROL Campaign Status] | 캠페인을 삭제하는 데에만 필요합니다. |
| \[광고주별 레이블 분류\] | 선택 사항 |
| [!UICONTROL Constraints] | 선택 사항 |
| [!UICONTROL Campaign ID] | 행에 캠페인에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 캠페인 이름을 변경할 때만 필요합니다. |
| [!UICONTROL AMO ID] | 엔티티 ID 및 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

### 광고 그룹 필드

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-microsoft)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Ad Group Name] | 필수 |
| [!UICONTROL Ad Group Type] | 광고 그룹을 만드는 데 필요합니다. |
| [!UICONTROL Audience Target Method] | 대상 광고 그룹을 만드는 데에만 필요합니다. |
| [!UICONTROL Ad Group Start Date] | 선택 사항 |
| [!UICONTROL Ad Group End Date] | 선택 사항 |
| [!UICONTROL Tracking Template] | 선택 사항 |
| [!UICONTROL Search Network Status] | (검색 네트워크의 캠페인만 해당) 선택 사항 |
| [!UICONTROL Languages] | 선택 사항 |
| [!UICONTROL Device] | 선택 사항 |
| [!UICONTROL Bid Adjustment] | 선택 사항 |
| [!UICONTROL Ad Group Status] | 광고 그룹을 삭제하는 데에만 필요합니다. |
| \[광고주별 레이블 분류\] | 선택 사항 |
| [!UICONTROL Constraints] | 선택 사항 |
| [!UICONTROL Ad Group ID] | 행에 광고 그룹에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 광고 그룹 이름을 변경할 때만 필요합니다. |
| [!UICONTROL AMO ID] | 엔티티 ID 및 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

### 키워드 필드

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-microsoft)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Ad Group Name] | 필수 |
| [!UICONTROL Keyword] | 필수 |
| [!UICONTROL Match Type] | 여러 일치 유형이 있는 키워드를 편집하거나 삭제하려면 일치 유형 또는 키워드 ID 값이 필요합니다. |
| [!UICONTROL Max CPC] | 선택 사항 |
| [!UICONTROL Base URL/Final URL] | 선택 사항 |
| [!UICONTROL Custom URL Param] | 선택 사항 |
| [!UICONTROL Tracking Template] | 선택 사항 |
| [!UICONTROL Param1] | 선택 사항 |
| [!UICONTROL Param2] | 선택 사항 |
| [!UICONTROL Keyword Status] | 키워드를 삭제하는 데에만 필요합니다. |
| \[광고주별 레이블 분류\] | 선택 사항 |
| [!UICONTROL Constraints] | 선택 사항 |
| [!UICONTROL Campaign ID] | 선택 사항 |
| [!UICONTROL Ad Group ID] | 선택 사항 |
| [!UICONTROL Keyword ID] | 행에 a) 키워드를 식별하기에 충분한 속성 열 또는 b) &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 키워드를 편집하거나 삭제할 때만 필요합니다. |
| [!UICONTROL AMO ID] | 엔티티 ID 및 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

### 동적 검색 광고 필드

>[!NOTE]
>
>지원 만들기를 사용할 수 없습니다.

이 광고 유형의 경우 [!UICONTROL Creative (except RSA)] 대화 상자에서 &quot;[!UICONTROL Download Bulksheet]&quot; 행을 사용하십시오.

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-microsoft)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Ad Group Name] | 필수 |
| [!UICONTROL Description Line 1]-[!UICONTROL Description Line 2] | 설명을 편집하는 데 필요합니다. <b>참고:</b> 이 광고 형식의 경우 광고 복사본을 변경하면 기존 광고가 삭제되고 새 광고가 만들어집니다. |
| [!UICONTROL Display Path 1] | 필드를 편집하는 데 필요합니다. |
| [!UICONTROL Display Path 2] | 필드를 편집하는 데 필요합니다. |
| [!UICONTROL Creative Type] | 제품 광고의 상태를 만들거나 편집하는 데 필요합니다. |
| [!UICONTROL Creative Preferred Devices] | 선택 사항 |
| [!UICONTROL Ad Status] | 광고를 삭제하는 데 필요합니다. |
| \[광고주별 레이블 분류\] | 선택 사항 |
| [!UICONTROL Campaign ID] | 선택 사항 |
| [!UICONTROL Ad Group ID] | 선택 사항 |
| [!UICONTROL Ad ID] | 행에 a&rpar; 광고 또는 b&rpar; &quot;[!UICONTROL AMO ID]&quot;을(를) 식별하는 데 충분한 광고 속성 열이 포함되지 않는 한 광고 상태를 변경할 때만 필요합니다. 그러나 [!UICONTROL Ad ID]과(와) [!UICONTROL AMO ID]을(를) 모두 포함하지 않고 광고 속성 열이 여러 광고와 일치하는 경우 광고 중 하나에 대한 상태만 변경됩니다. |
| [!UICONTROL AMO ID] | 엔티티 ID 및 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

### 제품(쇼핑) 광고 필드

쇼핑 광고 만들기에 대한 자세한 내용은 &quot;[쇼핑 캠페인 구현 [!DNL Microsoft Advertising] 2&rbrace;&quot;을 참조하십시오.](https://experienceleague.adobe.com/docs/advertising/search-social-commerce/campaign-management/management/special-workflows/microsoft-shopping-campaigns.html?lang=ko)

이 광고 유형의 경우 [!UICONTROL Creative (except RSA)] 대화 상자에서 &quot;[!UICONTROL Download Bulksheet]&quot; 행을 사용하십시오.

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-microsoft)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Ad Group Name] | 필수 |
| [!UICONTROL Promotion Line] | 선택 사항 |
| [!UICONTROL Base URL/Final URL] | 선택 사항 |
| [!UICONTROL Custom URL Param] | 선택 사항 |
| [!UICONTROL Creative Type] | 제품 광고의 상태를 만들거나 편집하는 데 필요합니다. |
| [!UICONTROL Tracking Template] | 선택 사항 |
| [!UICONTROL Ad Status] | 광고를 삭제하는 데 필요합니다. |
| \[광고주별 레이블 분류\] | 선택 사항 |
| [!UICONTROL Constraints] | 선택 사항 |
| [!UICONTROL Campaign ID] | 선택 사항 |
| [!UICONTROL Ad Group ID] | 선택 사항 |
| [!UICONTROL Ad ID] | 행에 a) 광고를 식별할 수 있는 충분한 광고 속성 열 또는 b) &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 광고 상태를 변경할 때만 필요합니다. 그러나 [!UICONTROL Ad ID]과(와) [!UICONTROL AMO ID]을(를) 모두 포함하지 않고 광고 속성 열이 여러 광고와 일치하는 경우 광고 중 하나에 대한 상태만 변경됩니다. |
| [!UICONTROL AMO ID] | 엔티티 ID 및 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

### 반응형(멀티미디어) 광고 필드

이 광고 유형의 경우 [!UICONTROL Creative (except RSA)] 대화 상자에서 &quot;[!UICONTROL Download Bulksheet]&quot; 행을 사용하십시오.

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-microsoft)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Ad Group Name] | 필수 |
| [!UICONTROL Ad Title], [!UICONTROL Ad Title 2]-[!UICONTROL Ad Title 15] | 반응형 광고의 경우 광고를 만들려면 [!UICONTROL Ad Title], [!UICONTROL Ad Title 2] 및 [!UICONTROL Ad Title 3]이(가) 필요하며 다른 모든 광고 제목 필드는 선택 사항입니다. 필수가 아닌 필드의 기존 값을 삭제하려면 값 `[delete]`(대괄호 포함)을(를) 사용합니다. <b>참고:</b> 이 광고 형식의 경우 광고 복사본을 변경하면 기존 광고가 삭제되고 새 광고가 만들어집니다. |
| [!UICONTROL Description Line 1]-[!UICONTROL Description Line 4] | 광고를 만들려면 [!UICONTROL Description Line 1] 및 [!UICONTROL Description Line 2]이(가) 필요하며 [!UICONTROL Description Line 3] 및 [!UICONTROL Description Line 4]은(는) 선택 사항입니다. <b>참고:</b> 이 광고 형식의 경우 광고 복사본을 변경하면 기존 광고가 삭제되고 새 광고가 만들어집니다. |
| [!UICONTROL Business Name] | 광고를 만들거나 삭제하는 데 필요합니다. |
| [!UICONTROL Call To Action] | 광고를 만드는 데 필요합니다. |
| [!UICONTROL Call To Action Language] | 광고를 만드는 데 필요합니다. |
| [!UICONTROL Base URL/Final URL] | 광고를 만드는 데 필요합니다. |
| [!UICONTROL Creative Type] | 선택 사항입니다. |
| [!UICONTROL Tracking Template] | 선택 사항 |
| [!UICONTROL Ad Status] | 광고를 삭제하는 데 필요합니다. |
| \[광고주별 레이블 분류\] | 선택 사항 |
| [!UICONTROL Campaign ID] | 선택 사항 |
| [!UICONTROL Ad Group ID] | 선택 사항 |
| [!UICONTROL Ad ID] | 행에 a) 광고를 식별할 수 있는 충분한 광고 속성 열 또는 b) &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 광고 상태를 변경할 때만 필요합니다. 그러나 [!UICONTROL Ad ID]과(와) [!UICONTROL AMO ID]을(를) 모두 포함하지 않고 광고 속성 열이 여러 광고와 일치하는 경우 광고 중 하나에 대한 상태만 변경됩니다. |
| [!UICONTROL AMO ID] | 엔티티 ID 및 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

### 반응형 검색 광고 필드

이 광고 유형의 경우 [!UICONTROL Responsive Search Ad] 대화 상자에서 &quot;[!UICONTROL Download Bulksheet]&quot; 행을 사용하십시오.

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-microsoft)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Ad Group Name] | 필수 |
| [!UICONTROL Ad Title], [!UICONTROL Ad Title 2]-[!UICONTROL Ad Title 15] | 반응형 검색 광고의 경우 광고를 만들려면 [!UICONTROL Ad Title], [!UICONTROL Ad Title 2] 및 [!UICONTROL Ad Title 3]이(가) 필요하며 다른 모든 광고 제목 필드는 선택 사항입니다. 필수가 아닌 필드의 기존 값을 삭제하려면 값 `[delete]`(대괄호 포함)을(를) 사용합니다. |
| [!UICONTROL Ad Title 1 Position]-[!UICONTROL Ad Title 15 Position] | 선택 사항 |
| [!UICONTROL Description Line 1]-[!UICONTROL Description Line 4] | 반응형 검색 광고의 경우 광고를 만들려면 [!UICONTROL Description Line 1] 및 [!UICONTROL Description Line 2]이(가) 필요하며 [!UICONTROL Description Line 3] 및 [!UICONTROL Description Line 4]은(는) 선택 사항입니다. 기존 값을 삭제하려면 값 `[delete]`(대괄호 포함)을 사용하십시오. |
| [!UICONTROL Description Line 1 Position]-[!UICONTROL Description Line 4 Position] | 선택 사항 |
| [!UICONTROL Display Path 1] | 선택 사항 |
| [!UICONTROL Display Path 2] | 선택 사항 |
| [!UICONTROL Base URL/Final URL] | 광고를 만드는 데 필요합니다. |
| [!UICONTROL Custom URL Param] | 선택 사항 |
| [!UICONTROL Creative Type] | 선택 사항 |
| [!UICONTROL Tracking Template] | 선택 사항 |
| [!UICONTROL Ad Status] | 광고를 삭제하는 데 필요합니다. |
| \[광고주별 레이블 분류\] | 선택 사항 |
| [!UICONTROL Campaign ID] | 선택 사항 |
| [!UICONTROL Ad Group ID] | 선택 사항 |
| [!UICONTROL Ad ID] | 행에 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않은 경우 광고를 편집하거나 삭제하는 데 필요합니다. |
| [!UICONTROL AMO ID] | 광고 ID를 포함하지 않는 한 광고를 편집하거나 삭제하는 데 필요합니다. |

### 텍스트 광고 필드

이 광고 유형의 경우 [!UICONTROL Creative (except RSA)] 대화 상자에서 &quot;[!UICONTROL Download Bulksheet]&quot; 행을 사용하십시오.

>[!NOTE]
>
>확장된 텍스트 광고는 더 이상 사용되지 않습니다. 기존 텍스트 광고만 삭제할 수 있습니다.

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-microsoft)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Ad Group Name] | 필수 |
| [!UICONTROL Ad Title], [!UICONTROL Ad Title 2]-[!UICONTROL Ad Title 3] | 읽기 전용 |
| [!UICONTROL Description Line 1]-[!UICONTROL Description Line 2] | 읽기 전용 |
| [!UICONTROL Display URL] | 읽기 전용 |
| [!UICONTROL Display Path 1] | 읽기 전용 |
| [!UICONTROL Display Path 2] | 읽기 전용 |
| [!UICONTROL Base URL/Final URL] | 읽기 전용 |
| [!UICONTROL Custom URL Param] | 읽기 전용 |
| [!UICONTROL Creative Type] | 선택 사항 |
| [!UICONTROL Tracking Template] | 읽기 전용 |
| [!UICONTROL Creative Preferred Devices] | 읽기 전용 |
| [!UICONTROL Ad Status] | 필수 |
| \[광고주별 레이블 분류\] | 선택 사항 |
| [!UICONTROL Campaign ID] | 선택 사항 |
| [!UICONTROL Ad Group ID] | 선택 사항 |
| [!UICONTROL Ad ID] | 행에 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않은 경우 광고 상태를 변경할 때만 필요합니다. |
| [!UICONTROL AMO ID] | 광고 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

### 동적 검색 대상(자동 타겟) 필드

>[!NOTE]
>
>지원 만들기를 사용할 수 없습니다.

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-microsoft)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Ad Group Name] | 필수 |
| [!UICONTROL Auto Target Expression] | 필수. |
| [!UICONTROL Match Type] | 선택 사항 |
| [!UICONTROL Max CPC] | 선택 사항 |
| [!UICONTROL Custom URL Param] | 선택 사항 |
| [!UICONTROL Target Status] | 대상을 삭제하는 데 필요합니다. |
| \[광고주별 레이블 분류\] | 선택 사항 |
| [!UICONTROL Constraints] | 선택 사항 |
| [!UICONTROL Campaign ID] | 선택 사항 |
| [!UICONTROL Ad Group ID] | 선택 사항 |
| [!UICONTROL Target ID] | 행에 대상에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 자동 대상을 변경하거나 삭제할 때만 필요합니다. |
| [!UICONTROL AMO ID] | 엔티티 ID 및 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

### 쇼핑 제품 그룹 필드

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-microsoft)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Ad Group Name] | 필수 |
| [!UICONTROL Match Type] | 제품 그룹을 만드는 데 필요합니다. |
| [!UICONTROL Max CPC] | 제품 그룹을 만드는 데 필요합니다. |
| [!UICONTROL Parent Product Groupings] | 필수 |
| [!UICONTROL Product Grouping] | 필수 |
| [!UICONTROL Partition Type] | 제품 그룹을 만드는 데 필요합니다. |
| [!UICONTROL Base URL/Final URL] | 필수 |
| [!UICONTROL Tracking Template] | 선택 사항 |
| [!UICONTROL Product Group Status] | 제품 그룹을 삭제하는 데에만 필요합니다. |
| \[광고주별 레이블 분류\] | 선택 사항 |
| [!UICONTROL Constraints] | 선택 사항 |
| [!UICONTROL Campaign ID] | 선택 사항 |
| [!UICONTROL Ad Group ID] | 선택 사항 |
| [!UICONTROL Product Group ID] | 행에 a) 제품 그룹을 식별하는 데 충분한 속성 열 또는 b) &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 제품 그룹을 변경하거나 삭제할 때만 필요합니다. |
| [!UICONTROL AMO ID] | 엔티티 ID 및 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

### 캠페인 수준 사이트링크 필드

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-microsoft)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| 설명 라인 1 | 선택 사항 |
| [!UICONTROL Description Line 2] | 선택 사항 |
| [!UICONTROL Start Date] | 선택 사항 |
| [!UICONTROL End Date] | 선택 사항 |
| [!UICONTROL Base URL/Final URL] | 필수 |
| [!UICONTROL Custom URL Param] | 선택 사항 |
| [!UICONTROL Tracking Template] | 선택 사항 |
| [!UICONTROL Creative Preferred Devices] | 선택 사항 |
| [!UICONTROL Link Name] | 필수 |
| [!UICONTROL Sitelink Status] | 사이트링크를 삭제하는 데에만 필요합니다. |
| [!UICONTROL Campaign ID] | 선택 사항 |
| [!UICONTROL Sitelink ID] | 행에 a) 사이트 링크를 식별할 수 있는 충분한 속성 열 또는 b) &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 사이트 링크를 변경하거나 삭제하는 경우에만 필요합니다. 그러나 [!UICONTROL Sitelink ID]과(와) [!UICONTROL AMO ID]을(를) 모두 포함하지 않고 속성 열이 여러 사이트 링크와 일치하는 경우 사이트 링크 중 하나의 상태만 변경됩니다.<br><br><b>참고:</b> 기존 사이트 링크의 상태를 제외한 사이트 링크 속성 열을 편집하고 [!UICONTROL Sitelink ID] 또는 [!UICONTROL AMO ID]을(를) 포함하지 않으면 새 사이트 링크가 만들어지고 기존 사이트 링크는 변경되지 않습니다. |
| [!UICONTROL AMO ID] | 엔티티 ID 및 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

### 위치 대상 필드

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-microsoft)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Location] | 필수 |
| [!UICONTROL Location Type] | 대상을 만드는 데 필요합니다. |
| [!UICONTROL Bid Adjustment] | 선택 사항 |
| [!UICONTROL Location Status] | 위치 대상을 삭제하는 데에만 필요합니다. |
| [!UICONTROL Campaign ID] | 선택 사항 |
| [!UICONTROL AMO ID] | 캠페인 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

### 캠페인 수준 및 광고 그룹 수준 장치 대상 필드

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-microsoft)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Device] | 장치 대상을 삭제하는 데 필요합니다. |
| [!UICONTROL Bid Adjustment] | 선택 사항 |
| [!UICONTROL Ad Group Name] | 광고 그룹 수준 장치 대상에 필요합니다. 캠페인 수준 장치 타겟에는 적용할 수 없습니다. |
| [!UICONTROL Device Target Status] | 장치 대상을 삭제하는 데에만 필요합니다. |
| [!UICONTROL Campaign ID] | 선택 사항 |
| [!UICONTROL Ad Group ID] | 선택 사항, 광고 그룹 수준 장치 대상에만 적용됩니다. |
| [!UICONTROL AMO ID] | 장치 대상 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

### 캠페인 수준 및 광고 그룹 수준 RLSA 대상 필드

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-microsoft)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Ad Group Name] | 광고 그룹 수준 타겟에 필요합니다. 캠페인 수준 타겟에는 적용되지 않습니다. |
| [!UICONTROL Audience] | 새 대상을 만드는 데 필요합니다. |
| [!UICONTROL Target Type] | 선택 사항 |
| [!UICONTROL Bid Adjustment] | 선택 사항 |
| [!UICONTROL RLSA Target Status] | 대상을 삭제하는 데 필요합니다. |
| [!UICONTROL Campaign ID] | 선택 사항 |
| [!UICONTROL Ad Group ID] | 선택 사항, 광고 그룹 수준 타겟에만 적용됩니다. |
| [!UICONTROL RLSA Target ID] | 행에 대상에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 대상을 변경하거나 삭제할 때만 필요합니다. |
| [!UICONTROL AMO ID] | RLSA 대상 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

>[!MORELIKETHIS]
>
>* [부록 - 일괄 시트 오류](../bulksheet-errors.md)
>* [일괄 시트에서 수행할 수 있는 작업](bulksheet-operations.md)
>* [지원되는 일괄 시트 파일 형식](bulksheet-file-formats.md)
>* [일괄 시트 파일 다운로드/만들기](../bulksheet-download.md)
>* [에 대한  [!DNL Naver]](/help/search-social-commerce/tracking/formats-click-tracking-naver.md)클릭 추적 형식
>* [일괄 시트 파일 또는 수정된 오류 파일 업로드](../bulksheet-upload.md)
