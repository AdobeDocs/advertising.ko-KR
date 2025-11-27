---
title: ' [!DNL Google Ads] 계정의 필수 일괄 시트 데이터'
description: ' [!DNL Google Ads] 계정의 일괄 시트에 있는 필수 머리글 필드 및 데이터 필드를 참조합니다.'
exl-id: 756b77fe-f95d-469f-9ae0-7424c2fad0b1
feature: Search Bulksheets
source-git-commit: 3ab2e38f6a2f70c03504363575b13dc0dc730282
workflow-type: tm+mt
source-wordcount: '7859'
ht-degree: 0%

---

# 부록 - [!DNL Google Ads] 계정에 대한 필수 일괄 시트 데이터

[!DNL Google Ads] 캠페인 데이터를 일괄적으로 만들고 업데이트하려면 [!DNL Google Ads] 계정용으로 특별히 형식이 지정된 검색, 소셜 및 Commerce 일괄 시트 파일을 사용할 수 있습니다. a) [기존 계정에 대한 일괄 시트 파일을 필요한 파일 형식으로 생성](../bulksheet-download.md)하거나, b) 수동으로 만들 수 있습니다(&quot;[지원되는 일괄 시트 파일 형식](bulksheet-file-formats.md)&quot;에서 지원되는 파일 형식에 대한 일반 정보를 참조하십시오).

각 일괄 시트에는 수행할 [특정 작업](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-operations.md)에 필요한 헤더 필드와 해당 데이터 필드가 포함되어야 합니다(예: 광고 만들기). 필드가 필요하지 않으면 헤더 및 데이터 행에서 필드를 생략할 수 있습니다. 벌크 시트 파일을 업로드하면 모든 사용자 지정 열이 삭제됩니다.

다음은 사용 가능한 모든 데이터 필드 테이블 및 개별 엔터티(예: 캠페인 및 키워드)에 대한 데이터를 추가, 편집 또는 삭제하는 데 필요한 필드를 나타내는 추가 테이블입니다.

## 사용 가능한 모든 데이터 필드 {#bulksheet-fields-all-google}

다음 표에서는 사용 가능한 모든 데이터 필드에 대해 설명합니다.

계정 엔터티와 관련된 데이터 필드에 대해서는 &quot;[각 계정 구성 요소를 만들거나 편집하거나 삭제하는 데 필요한 필드](#bulksheet-fields-per-component-google)&quot;를 참조하십시오.

>[!NOTE]
>
>* 모든 텍스트 열의 값은 대/소문자를 구분합니다.
>* 새 레코드를 만들 때 모든 필수 데이터 필드에 대한 값을 포함하지 않으면 일부 필드에 지정된 기본값이 할당됩니다.
>* 아래에 지정되지 않은 필드의 경우, 광고 네트워크의 기본값이 사용됩니다.
>* [!UICONTROL Download Bulksheet] 대화 상자에서 사용 가능한 일괄 시트 행 목록을 보려면 &quot;[광고 네트워크별 일괄 시트 행](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-download.md#bulksheet-rows-by-ad-network)&quot;을 참조하십시오.

| 필드 | 설명 |
| ---- | ---- |
| [!UICONTROL Platform] | (정보 목적으로 생성된 일괄 시트에 포함) 광고 플랫폼. 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Acct Name] | 광고 네트워크 계정을 식별하는 고유한 이름. 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 계정에 대한 캠페인을 식별하는 고유한 이름. |
| [!UICONTROL Campaign Budget] | 금전적 기호와 구두점을 포함하거나 포함하지 않는 캠페인에 대한 일일 지출 제한. 이 값은 재정의되지만 계정 예산을 초과할 수 없습니다. |
| [!UICONTROL Delivery Method] | <p>매일 캠페인에 대한 광고를 표시하는 속도:</p><ul><li><p><i>[!UICONTROL Standard (Distributed)]</i>(새 캠페인의 기본값): 광고 노출 횟수를 하루 전체에 분산합니다.</p></li><li><p><i>[!UICONTROL Accelerated]:</i>(2019년 10월에 더 이상 사용되지 않음) 예산에 도달할 때까지 가능한 한 자주 광고를 표시합니다. 그 결과, 오늘 오후에 광고가 표시되지 않을 수 있습니다.</p></li></ul> |
| [!UICONTROL Channel Type] | <p>광고를 게재할 채널. 하나 이상의 옵션을 지정합니다.</p><ul><li><p><i>[!UICONTROL Search]</i>(새 캠페인의 기본값): [!DNL Google Ads] 검색 네트워크([!DNL Google Ads] 검색 및 검색 파트너 웹 사이트 포함)와 선택적으로 [!DNL Google Ads] 디스플레이 네트워크에도 광고를 게재합니다. <b>참고:</b> 검색 네트워크와 디스플레이 네트워크를 모두 대상으로 하는 캠페인은 입찰 최적화를 위해 포트폴리오에 추가할 수 없습니다.</p></li><li><p><i>[!UICONTROL Display]</i>: [!DNL Google Ads] 디스플레이 네트워크에만 광고를 배치합니다.</p></li><li><p><i>[!UICONTROL Shopping]</i>: [!DNL Google Ads] 쇼핑 네트워크(일부 국가)와 [!DNL Google Ads] 검색 네트워크(검색 및 검색 파트너 웹 사이트 [!DNL Google Ads]개 포함)에 쇼핑 광고를 게재합니다. 쇼핑 광고를 만들려면 [!DNL Google Merchant Center] 계정에 제품이 있어야 하며 [검색, 소셜 및 Commerce에서 계정에서 데이터를 다운로드하도록 허용](/help/search-social-commerce/campaign-management/accounts/merchant-account-manage.md)해야 합니다. 쇼핑 광고를 만드는 프로세스에 대한 자세한 내용은 &quot;[쇼핑 캠페인 구현 [!DNL Google Ads] 2&rbrace;&quot;을 참조하십시오.](/help/search-social-commerce/campaign-management/special-workflows/google-shopping-campaigns.md)</p></li></ul> |
| [!UICONTROL Networks] | <p>광고를 배치할 위치. 하나 이상의 옵션을 지정합니다.</p><ul><li><p><i>[!UICONTROL Google Search]</i>: Google Search Network에서만 스폰서 검색 목록을 제공합니다.</p></li><li><p><i>[!UICONTROL Search Partners]</i>: Google의 검색 파트너에 대한 스폰서 검색 목록입니다.</p></li><li><p><i>[!UICONTROL Content]</i>: 네트워크 목록 표시에 대한 입찰을 진행합니다.</p></li><li><p><i>[!UICONTROL All]</i>(새 캠페인의 기본값): Google 검색, 파트너 검색 및 콘텐츠를 타깃팅합니다.</p></li></ul> |
| [!UICONTROL DSA Domain Name] | <p>(Search Network만 해당, 확장된 동적 검색 광고에만 적용) 광고 네트워크가 동적 검색 광고를 타깃팅하는 데 사용하는 콘텐츠가 있는 웹 사이트의 루트 도메인(예: example.com) 또는 하위 도메인(예: shoes.example.com)입니다.<br><br><b>메모:</b></p><ul><li><p>확장된 동적 검색 광고는 키워드가 아닌 웹 사이트 콘텐츠를 타겟팅합니다.</p></li><li><p>타겟팅할 광고 네트워크의 유기 검색 색인으로 도메인을 색인화해야 합니다.</p></li><li><p>도메인을 지정하지 않는 경우 각 광고 그룹에 대해 모든 웹 사이트 페이지 또는 그 하위 집합을 타겟팅하는 동적 검색 타겟을 만들어야 합니다.</p></li></ul> |
| [!UICONTROL DSA Domain Language] | (검색 네트워크만 해당, 확장된 동적 검색 광고에만 해당) 지정된 웹 사이트 도메인의 언어입니다. <b>참고:</b> 도메인에 여러 언어로 된 페이지가 포함되어 있고 이러한 페이지를 모두 대상으로 지정하려면 각 언어에 대해 별도의 캠페인을 만드십시오. |
| [!UICONTROL GDN Custom Bid Level] | (디스플레이 네트워크만 대상으로 하는 캠페인) 입찰 방법: <i>[!UICONTROL Ad Group]</i>(기본값), <i>[!UICONTROL Keyword]</i>, <i>[!UICONTROL Placement]</i>(웹 사이트) 또는 <i>[!UICONTROL None]</i>(기존 값을 다시 설정). 다른 차원(<i>연령</i>, <i>성별</i>, <i>관심 항목 및 목록</i>, <i>주제</i> 및 <i>수직</i>)은 [!DNL Google Ads] 인터페이스에서 사용할 수 있습니다. [!DNL Google Ads] 인터페이스를 사용하여 다른 차원별 입찰을 구성한 경우 해당 값이 표시되지만 여기에서 해당 차원을 선택하거나 입력할 수 없습니다.</p><p><b>참고:</b></p><ul><li><p>키워드로 입찰하면 키워드 수준에서 추적 템플릿을 만듭니다. 마찬가지로, 배치로 입찰하는 경우 배치 수준에서 추적 템플릿을 만듭니다. 다른 모든 차원에 대해 광고 수준에서 추적 템플릿을 만듭니다.</p></li><li><p>지원되지 않는 차원(연령, 성별, 관심사 및 목록 또는 주제)으로 입찰하는 경우 검색, 소셜 및 Commerce이 차원에 대한 입찰을 최적화하지 않으며 모든 속성이 광고 그룹에 적용됩니다.</p></li><li><p>검색 네트워크의 광고는 항상 키워드 입찰을 사용합니다.</p></li></ul> |
| [!UICONTROL Campaign Priority] | <p>(쇼핑 캠페인만 해당) 여러 캠페인이 동일한 제품을 광고할 때 사용하는 우선 순위입니다. <i>[!UICONTROL Low]</i>(새 캠페인의 기본값), <i>[!UICONTROL Medium]</i> 또는 <i>[!UICONTROL High]</i>.</p><p>동일한 제품이 둘 이상의 캠페인에 포함된 경우 광고 네트워크는 캠페인 우선 순위를 먼저 사용하여 광고 경매에 적합한 캠페인(및 관련 입찰)을 결정합니다. 모든 캠페인이 동일한 우선 순위를 갖는 경우 입찰이 가장 높은 캠페인이 적격입니다. |
| [!UICONTROL Merchant ID] | (판매자 피드에만 연결된 쇼핑 캠페인 및 대상 캠페인) 캠페인에 제품이 사용되는 판매자 계정의 고객 ID입니다. |
| [!UICONTROL Sales Country] | (쇼핑 캠페인 전용, 기존 캠페인의 경우 읽기 전용) 캠페인의 제품이 판매되는 국가입니다. 제품은 대상 국가와 연결되어 있으므로 이 설정은 캠페인에 광고되는 제품을 결정합니다. |
| [!UICONTROL Product Scope Filter] | ([!DNL Google Ads] 쇼핑 네트워크만 사용하는 캠페인) [!DNL Google Merchant Center] 계정의 제품에서 캠페인에 대한 쇼핑 광고를 만들 수 있습니다. dimension=attribute 형식을 사용하여 제품을 필터링할 제품 차원 및 속성 조합을 최대 7개까지 입력할 수 있습니다. &quot;>>&quot; 구분 기호로 여러 필터를 구분합니다. 사용 가능한 제품 차원 목록을 보려면 &quot;[쇼핑 캠페인 제품 필터](/help/search-social-commerce/campaign-management/campaigns/shopping-campaign-product-filters.md)&quot;을 참조하세요.</p><p>예: &quot;CategoryL1=animals>>CategoryL2=pet supplies>>Brand=Acme Pet Supplies&quot;</p><p>기존 값을 삭제하려면 <code>[delete] 값을 사용하십시오.</code> (대괄호를 포함).</p> |
| [!UICONTROL Languages] | <p>(검색 및 디스플레이 네트워크만 해당) 캠페인의 광고 대상 언어입니다.</p><p>새 캠페인에 대해 이 필드 또는 [!UICONTROL Geo Targeting] 필드 값을 입력하지 않으면 계정에 대해 지정된 통화는 기본 언어를 결정합니다. 단, 특정 언어로 매핑되지 않은 통화(예: EUR)가 포함된 캠페인은 모든 언어로 타깃팅됩니다. 이 필드에 값을 입력하지 않고 새 캠페인에 대한 [!UICONTROL Geo Targeting] 필드에 값을 입력하면 기본값은 <i>[!UICONTROL All]</i>입니다. 기존 캠페인에 대해 이 필드를 비워 두면 기존 값이 유지됩니다.</p><p>모든 언어를 대상으로 지정하려면 <span style="font-style: italic;">&lt;i[!UICONTROL >All]</i></span>을(를) 입력하십시오. 특정 언어를 타깃팅하려면 <a href="https://developers.google.com/adwords/api/docs/appendix/codes-formats?csw=1#languages" target="_blank">[!DNL Google Ads]개의 언어 이름</a>(예: 올바른 숫자 코드로 대체되는 <i>영어;일본어</i>) 또는 숫자 코드(예: <i>1000;1005</i>)를 사용하여 세미콜론으로 구분된 값을 입력하십시오. 값은 대/소문자를 구분하지 않습니다.</p> |
| [!UICONTROL Location] | 캠페인을 위해 광고를 배치하거나 광고를 제외할 지리적 위치입니다. 새 캠페인에 대해 이 필드 또는 언어 필드에 값을 입력하지 않으면 계정에 대해 지정된 통화가 기본 위치를 결정합니다. 단, 특정 위치에 매핑되지 않은 통화(예: EUR)가 있는 캠페인은 모든 위치를 타깃팅합니다. 이 필드에 값을 입력하지 않고 새 캠페인에 대한 [!UICONTROL Languages] 필드에 값을 입력하면 기본값은 <i>[!UICONTROL All]</i>입니다. 기존 캠페인에 대해 이 필드를 비워 두면 기존 값이 유지됩니다.</p><p>특정 위치를 타깃팅하려면 [[!DNL Google Ads] 위치 이름](https://developers.google.com/adwords/api/docs/appendix/geotargeting)&#x200B;(올바른 숫자 코드로 대체됨) 또는 위치 코드 중 하나를 사용하십시오.</p><ul><li><p>국가/지역: 국가/지역 이름(예: <i>미국;일본</i>) 또는 숫자 코드(예: <i>2840;2392</i>)를 입력합니다.</p></li><li><p>주/도/지역: 주/도/지역 이름을 관련 국가/지역 약어(예: <i>Tokyo, JP;New York, US</i>) 또는 숫자 코드(예: <i>20636;21167</i>)로 입력합니다.</p></li><li><p>미국 이외의 도시: 구/군/시 이름, 시/도/지역 이름 및 국가/지역 약어(예: <i>Adachi, Tokyo, JP;Kita, Tokyo, JP</i>) 또는 숫자 코드(예: <i>1028850;1009293</i>)를 입력합니다.</p></li><li><p>미국 대도시 지역: 도시 이름, 주 이름 및 국가 약어(예: <i>Buffalo NY, US;New York NY, US</i>) 또는 숫자 코드(예: <i>514;501</i>)를 입력합니다.</p></li></ul><p>위치를 제외하려면 위치 이름 또는 코드 앞에 빼기 기호(`-`)가 붙습니다(예: <i>-Japan</i>).</p><p><b>참고:</b> 값은 대/소문자를 구분하지 않습니다.</p> |
| [!UICONTROL Location Type] | (위치를 포함하는 경우) [위치 유형](https://developers.google.com/google-ads/api/data/geotargets)입니다. |
| [!UICONTROL Device] | 캠페인 또는 광고 그룹 수준에서 입찰 조정을 수행하는 장치 유형: <i>[!UICONTROL smartphone]</i>, <i>[!UICONTROL tablet]</i> 또는 <i>[!UICONTROL desktop]</i>. |
| [!UICONTROL Bid Adjustment] | <p>([!UICONTROL Location], [!UICONTROL Device] 또는 [!UICONTROL RLSA] 대상을 포함하는 경우) 특정 위치, 특정 장치 유형 또는 특정 대상 대상의 광고 입찰을 조정할지 여부를 지정합니다.</p><ul><li><p>키워드 수준의 입찰(0% 차이)을 사용하려면 0을 입력합니다. 새 대상의 경우 이 항목을 비워 둘 수도 있습니다.</p></li><li><p>이 대상에 대해 다른 입찰가를 사용하려면 입찰가를 높이거나 낮출 백분율을 입력합니다.</p></li><ul><li><p>위치 및 RLSA 타겟의 경우 유효한 백분율은 -90에서 900까지입니다.</p></li><li><p>장치 입찰 조정의 경우 유효한 백분율은 다음과 같습니다.</p></li><ul><li><p>(캠페인)-100(장치 유형에서 광고를 입찰하지 않음) 또는 -90-900</p></li><li><p>(광고 그룹) 스마트폰 및 태블릿의 경우 -100(장치 유형에 대해 입찰하지 않음), 모든 장치 유형의 경우 -90 ~ 900.</p></li></ul></ul><li><p>(기존 캠페인 및 광고 그룹) 기존 입찰 조정을 사용하려면 이 항목을 비워 둡니다.</p></li></ul> |
| [!UICONTROL Adobe Rec Bid Adjustment] | (정보 목적으로 생성된 일괄 시트에 포함됨) Adobe에서 캠페인 수준 위치 대상 또는 RLSA에 권장하는 읽기 전용 입찰 조정입니다. 가중 전환 지표를 사용하는 목표를 가진 포트폴리오([!UICONTROL Maximize Clicks] 목표가 아님)에 캠페인이 있고, 최근 90일 동안 최소 5번의 클릭으로 두 개 이상의 위치 대상 또는 RLSA가 포함된 경우 또는 비용 USD가 5개인 경우에만 계산됩니다.</p><p>위치 타겟 또는 RLSA를 수동으로 편집하여 권장 값을 사용하려는 경우, 위치 타겟 또는 RLSA를 만든 후 최소 2주를 기다린 후 충분한 데이터 수집을 허용하고 값을 일주일에 두 번 이상 변경하지 마십시오. |
| [!UICONTROL Device Targets] | <p>(기존 캠페인 유형만 해당) 광고를 표시할 수 있는 장치: <i>[!UICONTROL All]</i>, <i>[!UICONTROL Computers]</i>, <i>[!UICONTROL Smartphones]</i> 또는 <i>[!UICONTROL Tablets]</i>. 새 캠페인의 경우 기본값은 <i>[!UICONTROL All]</i>입니다.</p> |
| [!UICONTROL Device OS Targets (Google Adwords)] | (레거시 캠페인 유형만 해당, 장치 대상에 &quot;스마트폰&quot; 또는 &quot;태블릿&quot;이 포함된 경우 적용 가능) 광고가 표시될 수 있는 운영 체제: <i>[!UICONTROL All]</i>, <i>[!UICONTROL Android]</i>, <i>[!UICONTROL iOS]</i> 또는 <i>[!UICONTROL Palm]</i>. 새 캠페인의 경우 기본값은 <i>[!UICONTROL All]</i>입니다.</p> |
| [!UICONTROL Mobile Carriers (Google Adwords)] | <p>(기존 캠페인 유형만 해당; [!UICONTROL Device Targets]에 &quot;[!UICONTROL All]&quot; 또는 &quot;[!UICONTROL Smartphones]&quot;이(가) 포함된 경우에 적용 가능) 스마트폰이 연결될 수 있는 이동통신사: <i>[!UICONTROL All]</i> 또는 <i>사용 가능한 통신사 및 </i>용 코드 목록을 사용하는 &lt;c<i>통신사 코드</i>>,&lt;<a href="https://developers.google.com/adwords/api/docs/appendix/codes-formats?csw=1#mobile-carriers" target="_blank">국가 코드[!DNL Google Ads]</a>>(예: T-Mobile,US)로 표시된 하나 이상의 통신사. 세미콜론(예: T-Mobile, US, T-Mobile, GB)으로 여러 캐리어를 구분하십시오. 새 캠페인의 경우 기본값은 <i>[!UICONTROL All]</i>입니다.</p> |
| [!UICONTROL Ad Group Name] | <p>광고 그룹을 식별하는 고유한 이름. 최대 길이는 255자입니다. 후행 빈 문자는 저장되지 않습니다(예: &quot;광고 그룹 1&quot;이 &quot;광고 그룹 1&quot;로 저장됨). 이 필드는 캠페인 수준 사이트 링크 또는 캠페인 수준 장치 타겟에 적용할 수 없습니다.</p> |
| [!UICONTROL Ad Group Type] | <p>광고 그룹 유형: <i>[!UICONTROL Demand Gen]</i>(수요 창출 캠페인만 해당), <i>[!UICONTROL Display]</i>(디스플레이 캠페인만 해당), <i>[!UICONTROL Search Dynamic]</i>(확장된 동적 검색 광고의 경우), <i>[!UICONTROL Search Standard]</i>(검색 광고의 경우), <i>[!UICONTROL Shopping Product]</i>(쇼핑 제품 광고의 경우), <i>[!UICONTROL Shopping Showcase]</i>(만들기 및 편집이 지원되지 않음) 또는 <i>[!UICONTROL Unknown]</i>.</p> |
| [!UICONTROL Max CPC] | <p>(CPC 캠페인만 해당) CPC(최대 클릭당 비용)는 금전적 기호와 구두점 유무에 관계없이 광고 네트워크에서 광고 클릭에 대해 지불하는 가장 높은 금액입니다. 광고 그룹 및 키워드, 제품 그룹, 동적 검색 타겟에 대한 값을 설정할 수 있습니다. 새 키워드의 기본값은 광고 그룹 수준에서 상속됩니다. 제품 그룹의 경우 가장 낮은 제품 그룹 계층의 값을 설정할 수 있습니다. 새 계층의 기본값은 상위 계층에서 상속됩니다.</p><p>최적화된 포트폴리오의 기존 제품 그룹 및 동적 검색 타겟의 경우 업데이트는 하루 동안만 유효하며 다음 최적화 주기 동안 덮어쓰여집니다.</p> |
| [!UICONTROL Max Content CPC] | <p>(CPC 캠페인만 해당) CPC(최대 클릭당 콘텐츠 비용)는 금전적 기호와 구두점 유무에 관계없이 디스플레이 네트워크 사이트에서 광고 클릭에 대해 지불하는 가장 높은 금액입니다. 배치 타깃팅되지 않은 캠페인의 광고 그룹 수준에서 값을 설정하고 편집할 수 있습니다.</p> |
| [!UICONTROL Audience Target Method] | <p>(검색 네트워크에만 있는 캠페인 및 표시 네트워크에는 기존의 읽기 전용 [!DNL Gmail] 캠페인):</p><ul><li><p><i>[!UICONTROL Target and Bid]</i>: 광고 그룹에 대한 다른 타겟도 충족하는 타겟 대상자와 연결된 사용자에게만 광고를 표시합니다.</p></li><li><p><i>[!UICONTROL Bid Only]</i>: 다른 광고 그룹 수준의 타겟을 만족시키는 한 타겟 대상자와 연결되지 않은 사람에게도 광고를 표시할 수 있습니다.</p><p>그러나 해당 대상자에 대해 더 높은 입찰가를 설정하여 특정 대상자에게 광고가 표시될 가능성을 높일 수 있습니다.</p></li></ul> |
| [!UICONTROL Keyword] | 키워드 문자열입니다. 최대 길이는 80자이고 10단어 이하이며 문자, 숫자 및 다음 특수 문자만 포함할 수 있습니다. 공백 `# $ & _ - " [ ] ' + . / :`</p><p><b>참고:</b></p><ul><li><p>광고 그룹 또는 캠페인 수준에서 키워드를 제외하려면 [!UICONTROL Match Type]을(를) <i>[!UICONTROL Negative]</i>(으)로 설정합니다. 행에 광고 그룹 이름이 포함된 경우 광고 그룹에 대한 키워드는 제외됩니다. 행에 광고 그룹 이름이 포함되지 않으면 전체 캠페인에 대해 키워드가 제외됩니다.</p></li><li><p>[!DNL Google Ads] 키워드 또는 일치 유형을 변경하면 기존 키워드가 삭제되고 새 키워드가 만들어집니다.</p></li></ul> |
| [!UICONTROL Placement] | (컨텐츠를 사용하는 캠페인만 일치) 광고가 표시될 수 있는 디스플레이 네트워크의 배치입니다. 다음 중 하나를 지정합니다.</p><ul><li><p>웹 사이트: 올바른 URL을 입력하십시오. 최상위 도메인, 첫 번째 수준 하위 도메인 또는 단일 디렉터리 이름의 도메인일 수 있습니다. URL에는 물음표(?)를 포함할 수 없습니다. 예:<code><br />www.example.com<br />example.com<br />autos.example.com<br />example.com/widgets</code></p></li><li><p>특정 페이지의 광고 위치: `<URL> >> <location,sublocation>` 형식(예: `finance.google.com >> Company pages,Top right`)을 사용합니다.</p></li><li><p>주제 범주: 구문 `<category::<category> > <subcategory>` 등을 사용합니다(예: `category::Industries > Energy & Utilities > Oil & Gas`).</p></li></ul><p><b>참고:</b> 광고 그룹 또는 캠페인 수준에서 배치를 제외하려면 [!UICONTROL Match Type]을(를) <i>[!UICONTROL Negative]</i>(으)로 설정하십시오. 행에 광고 그룹 이름이 포함된 경우 광고 그룹에 대한 배치가 제외됩니다. 행에 광고 그룹 이름이 포함되지 않은 경우 전체 캠페인에 대한 배치가 제외됩니다.</p> |
| [!UICONTROL Auto Target Expression] | <p>(&quot;[!UICONTROL Use my website contents to target my ads]&quot;(으)로 캠페인 설정을 사용하지 않는 경우 필요합니다. 그렇지 않으면 선택 사항입니다.) 광고 그룹에 대한 동적 검색 대상입니다.</p><p>모든 대상에 대해 별표(*)를 사용합니다.</p><p>최대 3개의 동적 검색 조건을 대상으로 지정하려면 `<category>=<target>` 형식을 사용하십시오. 여기서 `<category>`에는 아래 범주가 포함될 수 있습니다. &quot;\[blank space\] 및 \[blank space\]&quot;를 사용하여 개별 범주에 대한 여러 대상을 조인하고 &quot;[blank space] 및 [blank space]&quot;을(를) 사용하여 여러 범주에 조인합니다.</p><ul><li><p><i>[!UICONTROL Category]</i>: 특정 [!DNL Google Ads] 콘텐츠 범주가 있는 인덱싱된 페이지에 대해 확장된 동적 검색 광고를 표시합니다.</p></li><li><p><i>[!UICONTROL URL]</i>: 특정 URL을 가진 인덱싱된 페이지에 대한 확장된 동적 검색 광고를 표시합니다. 여기서 값은 URL 내 어디에나 포함될 수 있습니다.</p></li><li><p><i>[!UICONTROL Page Title]</i>: 페이지 제목에 특정 텍스트가 있는 인덱싱된 페이지에 대한 확장된 동적 검색 광고를 표시합니다.</p></li><li><p><i>[!UICONTROL Page Content]</i>: 특정 콘텐츠가 있는 인덱싱된 페이지에 대한 확장된 동적 검색 광고를 표시합니다.</p></li></ul><p>예: url=shoes.example.com 및 페이지 제목=footwear</p> |
| [!UICONTROL Parent Product Groupings] | 상위 제품 그룹의 계층입니다.<br><br>예: `All Products>>ProductTypeL1=a>>ProductTypeL2=b` |
| [!UICONTROL Product Grouping] | <p>제품 그룹(예: &quot;brand=acme&quot; 또는 &quot;모든 제품&quot;).</p><p><b>참고:</b></p><ul><li><p>지정한 제품 그룹이 [!UICONTROL Parent Product Groupings] 계층에 없으면 Search, Social 및 Commerce에서 필요한 계층 구조의 일부를 만듭니다.</p></li><li><p>기본 입찰이 광고 그룹 기본 입찰로 설정된 [!UICONTROL All Products] 쇼핑 캠페인에서 광고 그룹을 만들 때 Search, Social 및 Commerce에서 자동으로 &quot;[!DNL Google Ads]&quot; 그룹을 만듭니다. Search, Social 및 Commerce은 제품 그룹 계층의 각 수준에서 광고 그룹 기본 입찰이 있는 &quot;[!UICONTROL Everything Else]&quot; 그룹을 자동으로 만듭니다. 이러한 기본 그룹을 명시적으로 생성하고 제외하거나 입찰을 변경할 수 있습니다.</p></li><li><p>각 광고 그룹은 &quot;[!UICONTROL All Products]&quot; 및 7개의 다른 계층을 포함하여 최대 8개의 제품 그룹 계층을 포함할 수 있습니다.</p></li></ul> |
| [!UICONTROL Partition Type] | 제품 그룹에 대한 파티션 형식: <i>subdivision</i>(하위 제품 그룹이 있는 경우) 또는 <i>unit</i>(하위 제품 그룹이 없는 경우). |
| [!UICONTROL Match Type] | <p>동적 검색 대상 또는 제품 그룹의 경우: 동적 검색 대상 또는 제품 그룹에 대한 키워드 일치 옵션: <i>[!UICONTROL Dynamic Ad Target]</i>(새 동적 검색 대상의 기본값), <i>[!UICONTROL Product Group]</i>(새 제품 그룹의 기본값) 또는 <i>[!UICONTROL Negative Product Group]</i>(제품 그룹을 제외).</p><p>키워드의 경우: 키워드에 대한 키워드 일치 옵션: <i>[!UICONTROL Broad]</i>, <i>[!UICONTROL Phrase]</i>, <i>[!UICONTROL Exact]</i> 또는 <i>[!UICONTROL Negative]</i>(디스플레이 네트워크에서 키워드 또는 배치를 제외); 쇼핑 광고와 함께 사용되는 제품 그룹의 일치 유형은 <i>[!UICONTROL Product Group]</i>입니다. <i>[!UICONTROL Negative]</i>을(를) 사용하는 경우 제외할 일치 유형도 포함해야 합니다(예: &quot;음수 구&quot;).</p><p>새 키워드의 경우 기본값은 <i>[!UICONTROL Broad]</i>입니다. 일치 유형 또는 키워드 ID 값은 여러 일치 유형이 있는 키워드를 편집하는 데만 필요합니다.</p><p><b>참고:</b></p><ul><li><p>일치 유형은 키워드를 사용하지 않는 확장된 동적 검색 광고에 적용할 수 없습니다.</p></li><li><p>[!DNL Google Ads] 키워드의 일치 유형을 변경하면 기존 키워드가 삭제되고 새 키워드가 만들어집니다.</p></li><li><p>Broad Match 수정자의 경우 &quot;Broad&quot;를 선택하고 가까운 변형이 필요한 키워드 내의 단어 앞에 +를 삽입합니다(예: &quot;red&quot; 및 &quot;shoes&quot;의 가까운 변형이 필요한 &quot;+red +shoes&quot;). <b>참고:</b> 이제 Broad 일치 한정자의 동작이 일부 언어에 대해 Phrase match와 동일하며 2021년 7월 이후 새로운 broad match 한정자 키워드를 만들 수 없습니다. 자세한 내용은 [[!DNL Google Ads] 설명서](https://support.google.com/google-ads/answer/7042511)를 참조하세요.</p> |
| [!UICONTROL First Page Bid] | (정보 목적으로 생성된 일괄 시트에 포함) 검색 결과의 첫 페이지에 광고를 배치하는 데 필요한 입찰입니다. 이 값은 광고 네트워크에 게시되지 않습니다. |
| [!UICONTROL Quality Score] | (정보 목적으로 생성된 일괄 시트에 포함됨) 검색 엔진이 키워드에 할당한 현재 품질 점수입니다. 이 값은 광고 네트워크에 게시되지 않습니다.) |
| [!UICONTROL Creative Preferred Devices] | (텍스트 광고, 확장된 동적 검색 광고 및 향상된 사이트 링크, 선택 사항) 광고를 표시할 장치 유형은 <i>[!UICONTROL All]</i>(기본값) 또는 <i>[!UICONTROL Mobile]</i>입니다. <i>[!UICONTROL Mobile]</i>을(를) 지정하면 네트워크에서 데스크톱 또는 태블릿 사용자가 아닌 모바일 장치 사용자에게 광고를 표시하려고 합니다. 그렇지 않으면 네트워크는 모든 디바이스 유형에 광고를 표시합니다.</p><p><b>참고:</b></p><ul><li><p>관리자 및 [!DNL Adobe] 계정 관리자 사용자만 이 설정을 편집할 수 있습니다.</p></li><li><p>네트워크는 기본 장치 유형에 광고를 표시할 것을 보장하지 않습니다.</p></li><li><p>향상된 새 사이트링크는 기존의 향상된 사이트링크가 있거나 사이트링크가 없는 캠페인에서만 만들 수 있습니다.</p></li></ul> |
| [!UICONTROL Ad Title], [!UICONTROL Ad Title 2]-15 | (확장된 텍스트 광고 및 반응형 검색 광고만 해당) 각각 수직 파이프(&vert;)로 구분된 광고의 헤드라인 각 광고 제목 필드의 최대 길이는 동적 텍스트(예: 키워드 및 광고 사용자 정의 값)를 포함하여 30자 또는 15개의 더블바이트 문자입니다.</p><p>반응형 검색 광고의 경우 [!UICONTROL Ad Title], [!UICONTROL Ad Title 2] 및 [!UICONTROL Ad Title 3]이(가) 필요하며 다른 모든 광고 제목 필드는 선택 사항입니다. 필수가 아닌 필드의 기존 값을 삭제하려면 <code>[delete] 값을 사용하십시오.</code> (대괄호를 포함).</p><p>반응형 검색 광고의 경우 다음 형식을 사용하여 광고 사용자 지정자를 삽입합니다. <code>{CUSTOMIZER.AdCustomizerName:DefaultText}</code>, 예: <code>{CUSTOMIZER.Discount:10%}</code></p><p>만들거나 편집할 수 없지만 확장된 텍스트 광고는 삭제할 수 있습니다. [!DNL Google Ads]은(는) 2022년 6월에 더 이상 사용되지 않습니다. |
| [!UICONTROL Ad Title 1 Position]-[!UICONTROL Ad Title 15 Position] | <p>(반응형 검색 광고만 해당; 선택 사항) 해당 광고 제목을 고정할 위치: `[null]`(모든 위치에 대해 광고 제목을 사용할 수 있는 값 없음), <i>1</i>, <i>2</i> 또는 <i>3</i>. 예를 들어 [!UICONTROL Ad Title Position]의 값이 1이면 광고 제목은 위치 1에만 나타납니다. 기본적으로 모든 광고 제목은 null입니다(값 없음).</p><p>기존 값을 삭제하려면 <code>[delete] 값을 사용하십시오.</code> (대괄호를 포함).</p><p><b>참고:</b> 여러 광고 제목을 같은 위치에 고정할 수 있습니다. 광고 네트워크는 해당 위치에 고정된 광고 제목 중 하나를 사용합니다. 위치 3에 고정된 제목은 광고와 함께 표시되지 않을 수 있습니다.</p> |
| [!UICONTROL Description Line 1]-[!UICONTROL Description Line 4] | <p>(확장된 동적 검색 광고, 확장된 텍스트 광고 및 반응형 검색 광고만 해당) 광고 본문입니다. 각 설명 필드의 최대 길이는 동적 텍스트(예: 키워드 및 광고 사용자 정의 값)를 포함하여 90자 또는 45개의 더블바이트 문자입니다.</p><p>반응형 검색 광고의 경우 `{CUSTOMIZER.AdCustomizerName:DefaultText}`과(와) 같은 `{CUSTOMIZER.Discount:10%}` 형식을 사용하여 광고 사용자 지정자를 삽입합니다.</p><p>확장된 동적 검색 광고의 경우 [!UICONTROL Description Line 1] 및 [!UICONTROL Description Line 2]만 사용하십시오. <b>참고:</b> 이 광고 형식의 경우 광고 복사본을 변경하면 기존 광고가 삭제되고 새 광고가 만들어집니다.</p><p>만들거나 편집할 수 없지만 확장된 텍스트 광고는 삭제할 수 있습니다. [!DNL Google Ads]은(는) 2022년 6월에 더 이상 사용되지 않습니다.</p><p>반응형 검색 광고의 경우 [!UICONTROL Description Line 1] 및 [!UICONTROL Description Line 2]이(가) 필요하며 [!UICONTROL Description Line 3] 및 [!UICONTROL Description Line 4]은(는) 선택 사항입니다. 기존 값을 삭제하려면 <code>[delete] 값을 사용하십시오.</code> (대괄호를 포함).</p> |
| [!UICONTROL Description Line 1 Position]-[!UICONTROL Description Line 4 Position] | (반응형 검색 광고만 해당; 선택 사항) 해당 설명을 고정할 위치입니다. `[null]`(값 없음), <i>1</i>, <i>2</i> 또는 <i>3</i>. 예를 들어 [!UICONTROL Description 1 Position]의 값이 1이면 [!UICONTROL Description 1]은(는) 위치 1에만 나타납니다. 기본적으로 설명은 위치에 고정되지 않습니다.</p><p>기존 값을 삭제하려면 값 `[delete]`(대괄호 포함)을 사용하십시오.</p><p><b>참고:</b> 동일한 위치에 여러 설명을 고정할 수 있습니다. 광고 네트워크는 해당 위치에 고정된 설명 중 하나를 사용합니다. 위치 2에 고정된 설명은 광고와 함께 표시되지 않을 수 있습니다. |
| [!UICONTROL Display URL] | 광고에 포함된 URL.<br><br>확장된 동적 검색 광고의 경우 [!DNL Google Ads]은(는) 웹 사이트 도메인에서 동적으로 이 값을 생성하므로 값을 입력할 필요가 없습니다.<br><br>반응형 검색 광고의 경우 값을 입력할 필요가 없습니다. 표시 URL은 최종 URL의 도메인에서 자동으로 추출됩니다. 선택적으로 경로 1 및 경로 2 필드를 사용하여 URL을 사용자 지정할 수 있습니다.<br><br>만들거나 편집할 수 없지만 확장된 텍스트 광고를 삭제할 수 있습니다. [!DNL Google Ads]은(는) 2022년 6월에 더 이상 사용되지 않습니다.<br><br><b>참고:</b>(최종 URL이 있는 계정) 표시 URL과 최종 URL의 도메인 이름은 일치해야 합니다.</p> |
| [!UICONTROL Display Path 1] | <p>(확장된 텍스트 광고<span> 및 반응형 검색 광고</span>만 해당)</p><p>(선택 사항) 최종 URL에서 자동으로 추출되는 표시 URL에 추가되는 텍스트입니다. URL 앞에는 슬래시(/)가 표시됩니다. 경로에는 슬래시(/) 또는 줄바꿈(\n) 문자를 사용할 수 없습니다. 최대 길이는 15자 또는 7개의 더블바이트 문자입니다.</p><p>광고 사용자 지정기를 삽입하려면 다음 형식을 사용하십시오. 여기서 `Default text`은(는) 피드 파일에 유효한 값이 포함되지 않은 경우 삽입할 선택적 값입니다.&lt; `{CUSTOMIZER.AdCustomizerName:Default text}`, 예: `{CUSTOMIZER.Discount:10%}`</p><p>예를 들어 [!UICONTROL Display Path 1]이(가) &quot;거래&quot;이면 표시 URL은 &lt;<i>표시 URL</i>>/거래입니다(예: www.example.com/deals).</p><p>만들거나 편집할 수 없지만 확장된 텍스트 광고는 삭제할 수 있습니다. [!DNL Google Ads]은(는) 2022년 6월에 더 이상 사용되지 않습니다.</p> |
| [!UICONTROL Display Path 2] | 두 번째 표시 경로입니다. [!UICONTROL Display Path 1]의 항목을 참조하십시오.<br><br>예: [!UICONTROL Display Path 1]이(가) &quot;거래&quot;이고 [!UICONTROL Display Path 2]이(가) &quot;로컬&quot;이면 디스플레이 URL은 &lt;<i>디스플레이 URL</i>>/거래/로컬입니다(예: www.example.com/deals/local).</p><p>만들거나 편집할 수 없지만 확장된 텍스트 광고는 삭제할 수 있습니다. [!DNL Google Ads]은(는) 2022년 6월에 더 이상 사용되지 않습니다.</p> |
| [!UICONTROL Promotion Line] | (제품 목록 광고만 해당) 검색 결과의 제품 목록에 포함될 선택적 프로모션 라인입니다. 최대 길이는 45자입니다.</p><p>프로모션 라인은 페이지에서 광고가 표시되는 위치에 따라 광고에 대한 다른 위치(예: 광고 아래)에 표시될 수 있습니다. |
| [!UICONTROL Link Name] | <p>사이트링크 텍스트입니다. 최대 25자를 포함할 수 있습니다.</p><p>새 사이트링크의 경우 사이트링크 행 내에 캠페인 이름을 포함해야 합니다. 광고 그룹 수준의 사이트링크의 경우 광고 그룹 이름도 포함해야 합니다.</p><p><b>참고:</b> 데스크톱 및 태블릿의 광고에는 35자의 기존 텍스트가 계속 표시되지만 모바일 장치에는 표시되지 않습니다.</p> |
| [!UICONTROL Mobile App Platform (Google Adwords)] | (기존 앱 설치 광고만 해당) 모바일 애플리케이션이 실행되는 운영 체제: <i>Android™</i> 또는 <i>ios</i>. |
| [!UICONTROL Mobile App ID (Google Adwords)] | (기존 앱 설치 광고만 해당) <p>애플리케이션 ID 또는 패키지 이름입니다. |
| [!UICONTROL Mobile App Name (Google Adwords)] | (기존 앱 설치 광고만 해당) 애플리케이션 이름. |
| [!UICONTROL Start Date] | <p>(향상된 사이트 링크만 해당) 사이트 링크에 대한 입찰이 이루어질 수 있는 첫 번째 날짜로서 광고주의 시간대 및 <i>m/d/yyyy</i>, <i>m/d/yy</i>, <i>m-d-yyyy</i> 또는 <i>m-d-yy</i> 중 하나입니다. 향상된 새 사이트링크의 기본값은 현재 날짜입니다.</p><p><b>참고:</b> 향상된 새 사이트링크는 기존의 향상된 사이트링크가 있거나 사이트링크가 없는 캠페인에서만 만들 수 있습니다.</p> |
| [!UICONTROL End Date] | <p>(향상된 사이트 링크만 해당) 사이트 링크에 대한 입찰이 이루어질 수 있는 마지막 날짜, 광고주의 시간대 및 다음 형식 중 하나입니다.  <i>m/d/yyyy</i>, <i>m/d/yy</i>, <i>m-d-yyyy</i> 또는 <i>m-d-yy</i>. 기본값은 없음(종료 날짜 없음)입니다.</p><p><b>참고:</b> 향상된 새 사이트링크는 기존의 향상된 사이트링크가 있거나 사이트링크가 없는 캠페인에서만 만들 수 있습니다.</p> |
| [!UICONTROL Exclude Tablet (Google Adwords)] | (기존 앱 설치 광고만 해당)</p><p>(선택 사항) [!DNL Google Ads]이(가) 태블릿 사용자에게 광고를 표시하지 못하도록 합니다. 값에는 <i>예</i> 및 <i>아니요</i>가 포함될 수 있습니다. |
| [!UICONTROL Landing Page Suffix] | 정보를 추적하기 위해 최종 URL 끝에 추가할 모든 매개 변수입니다. 예: `param2=value1&param3=value2`<br><br>자세한 내용은 &quot;[클릭 추적 형식 [!DNL Google Ads]](/help/search-social-commerce/tracking/formats-click-tracking-google.md)을 참조하세요.&quot;<br><br>하위 수준의 최종 URL 접미사가 계정 수준 접미사를 재정의합니다. 간편하게 유지 관리할 수 있도록 개별 계정 구성 요소에 대해 다른 추적이 필요하지 않은 경우 계정 수준 접미사만 사용하십시오. 광고 그룹 수준 이하에서 접미사를 구성하려면 [!DNL Google Ads] 편집기를 사용하십시오. |
| [!UICONTROL Tracking Template] | 모든 랜딩 도메인 리디렉션 및 추적 매개 변수를 지정하고 [!DNL ValueTrack] 매개 변수에 최종 URL을 임베드하는 추적 템플릿입니다. 가장 세부적인 수준의 추적 템플릿(키워드를 가장 세부적인 수준으로 사용)은 모든 상위 수준의 값을 무시합니다.<br><br>캠페인 설정에 &quot;[!UICONTROL EF Redirect]&quot; 및 &quot;[!UICONTROL Auto Upload]&quot;이(가) 포함된 경우 적용되는 Adobe Advertising 전환 추적의 경우 레코드를 저장할 때 검색, 소셜 및 Commerce에서 자동으로 리디렉션 및 추적 코드를 추가합니다.<br><br>서드파티 리디렉션 및 추적의 경우 값을 입력하십시오. 추적 템플릿의 최종 URL을 나타내는 [!DNL ValueTrack] 매개 변수 목록에 대해서는 [!DNL ValueTrack]설명서[[!DNL Google Ads] 의 &quot;사용 가능한 &#x200B;](https://support.google.com/google-ads/answer/2375447) 매개 변수&quot;에 대한 섹션에서 &quot;추적 템플릿만&quot; 매개 변수를 참조하십시오.<br><br>기존 값을 삭제하려면 `[delete]` 값(대괄호 포함)을 사용하십시오. |
| [!UICONTROL Base URL/Final URL] | 캠페인 또는 계정에 대해 구성된 추가 매개 변수를 포함하여 검색 엔진 사용자가 광고를 클릭할 때 취하는 랜딩 페이지 URL입니다. 키워드 수준의 기본/최종 URL은 광고 수준 이상의 URL을 재정의합니다.<br><br>기존 값을 삭제하려면 `[delete]` 값(대괄호 포함)을 사용하십시오. |
| [!UICONTROL Destination URL] | (정보 목적으로 생성된 일괄 시트에 포함됨, 검색 엔진에 게시되지 않음) 대상 URL이 있는 계정의 경우, 광고가 광고주 웹 사이트의 기본 URL/랜딩 페이지에 연결되는 URL입니다(경우에 따라 클릭을 추적한 다음 사용자를 랜딩 페이지로 리디렉션하는 다른 사이트를 통해). 여기에는 Search, Social 및 Commerce 캠페인 또는 계정에 대해 구성된 추가 매개 변수가 포함됩니다. 추적 URL을 생성한 경우, 이는 계정 설정 및 캠페인 설정의 추적 매개 변수를 기반으로 합니다. 검색 엔진별 매개 변수를 추가한 경우 이 매개 변수는 검색, 소셜 및 Commerce에 대한 동등한 매개 변수로 대체될 수 있습니다.<br><br>최종 URL이 있는 계정의 경우 이 열은 기본 URL/최종 URL 열과 동일한 값을 표시합니다. |
| [!UICONTROL Custom URL Param] | 변수가 검색 계정 또는 캠페인 설정에 대한 추적 매개 변수에 포함된 경우 `{custom_code}` 동적 변수를 대체할 데이터입니다. 추적 URL에 사용자 지정 값을 삽입하려면 추적 URL 생성 옵션을 사용하여 일괄 시트 파일을 업로드해야 합니다. |
| [!UICONTROL Creative Type] | 광고 형식: <i>[!UICONTROL Text ad]</i>, <i>[!UICONTROL Expanded text ad]</i>, <i>[!UICONTROL Demand Gen Carousel Ad]</i>(다중 이미지 회전 광고), <i>[!UICONTROL Demand Gen Image Ad (single-image ads)]</i>, <i>[!UICONTROL Demand Gen Product Ad]</i>, <i>[!UICONTROL Demand Gen Video Ad]</i>, <i>[!UICONTROL Dynamic search ad]</i>(더 이상 사용되지 않는 광고 유형), <i>[!UICONTROL Expanded Dynamic Search ad]</i>, &lt;[!UICONTROL i>Display ad]</i>, <i>[!UICONTROL App Install ad]</i>(더 이상 사용되지 않음), <i>[!UICONTROL Image]</i>, <i>[!UICONTROL Product ad<]/i>(쇼핑 광고) 또는 <i>[!UICONTROL Responsive search ad]</i>. 새 광고의 기본값은 <i>[!UICONTROL Text ad]</i>입니다.<br><br>제품 광고의 상태를 만들거나 편집하는 데 필요합니다. |
| [!UICONTROL Param1] | <p>광고 복사본에 포함될 수 있거나 일괄 시트 파일의 광고 URL을 표시할 수 있는 `{param1}` 광고 매개 변수의 숫자 값입니다. 최대 길이는 25자이며, 다음 숫자 문자를 포함할 수 있습니다.</p><ul><li><p>통화 기호나 코드 앞에 값을 추가하거나 추가할 수 있습니다. 예를 들어 `£2.000,00` 및 `2000GBP`은(는) 유효합니다.</p></li><li><p>값은 쉼표(`,`) 또는 마침표(`.`)를 구분 기호로 포함할 수 있으며, 소수 값은 선택적 마침표(`.`) 또는 쉼표(`,`)로 사용할 수 있습니다. 예를 들어 `1,000.00` 및 `2.000,10`은(는) 유효합니다.</p></li><li><p>값은 앞에 붙거나 퍼센트 기호(`%`), 더하기 기호(`+`) 또는 빼기 기호(`- `)를 추가할 수 있습니다. 예를 들어 `20%`, `208+` 및 `-42.32`이(가) 유효합니다.</p></li><li><p>두 숫자는 슬래시로 포함될 수 있습니다. 예를 들어 `4/1` 및 `0.95/0.45`은(는) 유효합니다.</p></li></ul><p>기존 값을 삭제하려면 값 `[delete]`(대괄호 포함)을 사용하십시오.</p> |
| [!UICONTROL Param2] | 광고 복사본에 포함될 수 있거나 일괄 시트 파일의 광고 URL을 표시할 수 있는 `{param2}` 광고 매개 변수의 숫자 값입니다. 자세한 내용은 Param1의 항목을 참조하십시오. |
| [!UICONTROL Audience] | 검색 광고(RLSA) 타겟 대상자 또는 캠페인 또는 광고 그룹의 제외된 대상자에 대한 리마케팅 목록입니다. &quot;대상 유형&quot; 필드에 대상인지 아니면 제외인지를 지정합니다. |
| [!UICONTROL Target Type] | (대상이 지정된 경우) 지정된 대상이 <i>포함</i>(대상)인지 <i>제외</i>인지 여부. |
| [!UICONTROL Campaign Status] | 캠페인의 표시 상태: <i>[!UICONTROL Active]</i>, <i>[!UICONTROL Paused]</i>, <i>[!UICONTROL Ended]</i>(편집할 수 없음) 또는 <i>[!UICONTROL Deleted]</i>(기존 캠페인만). 새 캠페인의 기본값은 <i>[!UICONTROL Active]</i>입니다. 활성 캠페인이나 일시 중지된 캠페인을 삭제하려면 값 <i>[!UICONTROL Deleted]</i>을(를) 입력하십시오. |
| [!UICONTROL Ad Group Status] | 광고 그룹의 표시 상태: <i>[!UICONTROL Active]</i>, <i>[!UICONTROL Paused]</i> 또는 <i>[!UICONTROL Deleted]</i>(기존 광고 그룹만 해당). 새 광고 그룹의 기본값은 [!UICONTROL Active]입니다. 활성 또는 일시 중지된 광고 그룹을 삭제하려면 값 `Deleted`을(를) 입력하십시오. |
| [!UICONTROL Keyword Status] | 키워드의 표시 상태: <i>[!UICONTROL Active]</i>, <i>[!UICONTROL Paused]</i> 또는 <i>[!UICONTROL Deleted]</i>(기존 키워드만 해당). 새 키워드의 기본값은 [!UICONTROL Active]입니다. 활성 또는 일시 중지된 키워드를 삭제하려면 값 <i>[!UICONTROL Deleted]</i>을(를) 입력하십시오. |
| [!UICONTROL Ad Status] | 광고의 표시 상태: <i>[!UICONTROL Active]</i>, <i>[!UICONTROL Deleted]</i>(기존 광고만), <i>[!UICONTROL Disapproved]</i>(편집할 수 없음) 또는 <i>[!UICONTROL Paused]</i>. 새 광고의 기본값은 [!UICONTROL Active]입니다. 활성 또는 일시 중지된 광고를 삭제하려면 값 <i>[!UICONTROL Deleted]</i>을(를) 입력하십시오. |
| [!UICONTROL Placement Status] | 웹 사이트 배치 상태: <i>[!UICONTROL Active]</i>, <i>[!UICONTROL Paused]</i> 또는 <i>[!UICONTROL Deleted]</i>(기존 광고만 해당). 새 웹 사이트의 기본값은 <i>활성입니다.</i> 활성 또는 일시 중지된 배치를 삭제하려면 값 <i>[!UICONTROL Deleted]</i>을(를) 입력하십시오. |
| [!UICONTROL Target Status] | 동적 검색 대상의 상태: <i>[!UICONTROL Active]</i>, <i>[!UICONTROL Paused]</i> 또는 <i>[!UICONTROL Deleted]</i>(기존 대상만). 새 대상의 기본값은 <i>활성입니다.</i> 활성 또는 일시 중지된 대상을 삭제하려면 값 <i>[!UICONTROL Deleted]</i>을(를) 입력하십시오. |
| [!UICONTROL Product Group Status] | 제품 그룹의 표시 상태: <i>[!UICONTROL Active]</i> <span>또는</span> <i>[!UICONTROL Deleted]</i>(기존 제품 그룹만 해당). 새 제품 그룹의 기본값은 <i>[!UICONTROL Active]</i>입니다. 활성 제품 그룹을 삭제하려면 값 <i>[!UICONTROL Deleted]</i>을(를) 입력하십시오. |
| [!UICONTROL Sitelink Status] | 사이트 링크의 표시 상태: <i>활성 또는 삭제됨</i>(기존 사이트 링크만 해당). 새 사이트 링크의 기본값은 <i>[!UICONTROL Active]</i>입니다. 활성 사이트 링크를 삭제하려면 값 <i>[!UICONTROL Deleted]</i>을(를) 입력하십시오. |
| [!UICONTROL Location Status] | 위치 대상의 상태: <i>[!UICONTROL Active]</i> 또는 <i>[!UICONTROL Deleted]</i>(기존 위치만 해당). 새 위치의 기본값은 [!UICONTROL Active]입니다. 활성 위치를 삭제하려면 값 <i>[!UICONTROL Deleted]</i>을(를) 입력하십시오. |
| [!UICONTROL RLSA Target Status] | 캠페인 또는 광고 그룹 수준의 RLSA 대상 또는 제외의 상태: <i>[!UICONTROL Active]</i> 또는 [!UICONTROL Deleted]</i>(기존 대상만). 새 대상 또는 제외의 기본값은 <i>[!UICONTROL Active]</i>입니다. 활성 대상 또는 제외를 삭제하려면 값 <i>[!UICONTROL Deleted]</i>을(를) 입력하십시오. |
| [!UICONTROL Device Target Status] | <p>캠페인 또는 광고 그룹 수준 장치 대상의 상태: <i>[!UICONTROL Active]</i> 또는 <i>[!UICONTROL Deleted]</i>. 새 캠페인 및 광고 그룹의 경우 기본값은 <i>[!UICONTROL Active]</i>입니다.</p> |
| \[광고주별 레이블 분류\] | (Color라는 레이블 분류의 경우 &quot;Color&quot;와 같이 광고주별 레이블 분류에 대해 이름이 지정됨) 엔티티와 연결된 지정된 분류의 값입니다. 엔티티당 분류당 하나의 값만 포함할 수 있습니다(예: 캠페인 A의 &quot;색상&quot; 레이블 분류의 경우 &quot;빨간색&quot;). 최대 길이는 100자이고 값에는 ASCII 및 비 ASCII 문자가 포함될 수 있습니다.<br><br>레이블 분류와 해당 레이블 값이 모든 하위 구성 요소에 적용됩니다. 나중에 추가되는 새 구성 요소는 자동으로 레이블과 연결됩니다. 제품 그룹에 대한 레이블 분류는 단위(가장 세부적인) 수준에 적용됩니다.<br><br>분류 이름과 분류 값은 대소문자를 구분하지 않습니다. |
| [!UICONTROL Constraints] | 엔티티에 할당된 제약 조건입니다. 엔티티당 하나의 제약조건만 지정할 수 있습니다.<br><b>>제약 조건은 하위 엔터티에 상속되므로 상속된 값을 재정의하지 않는 한 하위 엔터티의 값을 입력할 필요가 없습니다. |
| [!UICONTROL Campaign ID] | 기존 캠페인을 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 캠페인에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않은 경우 캠페인 이름을 변경할 때만 필요합니다. |
| [!UICONTROL Ad Group ID] | 기존 광고 그룹을 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 광고 그룹에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않은 경우 캠페인 이름을 변경할 때만 필요합니다. |
| [!UICONTROL Keyword ID] | 기존 키워드를 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 a) 키워드를 식별할 수 있는 충분한 속성 열 또는 b) &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 키워드를 변경할 때만 필요합니다.&quot; |
| [!UICONTROL Ad ID] | <p>기존 광고를 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 반응형 검색 광고의 경우 광고 데이터를 편집하거나 삭제하려면 광고 ID나 AMO ID가 필요합니다. 다른 모든 엔터티 형식의 경우 행에 a) 광고를 식별할 수 있는 충분한 광고 속성 열 또는 b) &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 광고 상태를 변경할 때만 광고 ID가 필요합니다.&quot; 그러나 [!UICONTROL Ad ID]과(와) [!UICONTROL AMO ID]을(를) 모두 포함하지 않고 광고 속성 열이 여러 광고와 일치하는 경우 광고 중 하나에 대한 상태만 변경됩니다.</p><p><b>참고:</b> a) 기존 광고의 상태를 제외한 광고 속성 열 또는 b) 응답형 검색 광고에 대한 데이터를 편집하고 [!UICONTROL Ad ID] 및 [!UICONTROL AMO ID]을(를) 포함하지 않으면 새 광고가 만들어지고 기존 광고가 변경되지 않습니다.</p> |
| [!UICONTROL Placement ID] | 웹 사이트 배치를 식별하는 고유 ID입니다. 행에 a) 배치를 식별할 수 있는 충분한 속성 열 또는 b) &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 배치를 변경하거나 삭제할 때만 필요합니다.&quot; |
| [!UICONTROL Target ID] | 기존 자동 타겟을 식별하는 고유 ID입니다. 행에 대상에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 자동 대상을 변경하거나 삭제할 때만 필요합니다. |
| [!UICONTROL Product Group ID] | 기존 제품 그룹을 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에는 a) 제품 그룹을 식별하는 데 충분한 속성 열 또는 b) &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 제품 그룹을 변경하거나 삭제할 때만 필요합니다.&quot; |
| [!UICONTROL Sitelink ID] | 기존 사이트링크를 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 a) 사이트 링크를 식별할 수 있는 충분한 속성 열 또는 b) &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 사이트 링크를 변경하거나 삭제하는 경우에만 필요합니다.&quot; 그러나 [!UICONTROL Sitelink ID]과(와) [!UICONTROL AMO ID]을(를) 모두 포함하지 않고 속성 열이 여러 사이트 링크와 일치하는 경우 사이트 링크 중 하나의 상태만 변경됩니다.</p><p><b>참고:</b> 기존 사이트 링크의 상태를 제외한 사이트 링크 속성 열을 편집하고 [!UICONTROL Sitelink ID] 및 [!UICONTROL AMO ID]을(를) 포함하지 않으면 새 사이트 링크가 만들어지고 기존 사이트 링크는 변경되지 않습니다. |
| [!UICONTROL RLSA Target ID] | 기존 캠페인 또는 광고 그룹 수준의 RLSA 대상 또는 제외를 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 대상에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되어 있지 않은 경우 대상 또는 제외를 변경하거나 삭제할 때만 필요합니다. |
| [!UICONTROL Device Target ID] | <p>기존 캠페인 수준 또는 광고 그룹 수준의 장치 대상 또는 제외를 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(&#39;)가 있어야 합니다.[^1] 행에 대상에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되어 있지 않은 한 대상을 변경하거나 삭제할 때만 필요합니다.</p> |
| [!UICONTROL AMO ID] | (생성된 일괄 시트에서) 동기화된 엔티티에 대해 Adobe이 생성한 고유 식별자입니다. 반응형 검색 광고의 경우 광고 ID를 포함하지 않는 한 광고를 편집하거나 삭제하려면 AMO ID가 필요합니다. AMO ID가 있는 다른 모든 엔티티 유형의 데이터를 편집하려면 엔티티 ID와 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하려면 AMO ID가 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |
| [!UICONTROL EF Error Message] | (정보 목적으로 생성된 일괄 시트에 포함됨) 행의 데이터에 대한 광고 네트워크의 오류 메시지를 표시하는 자리 표시자입니다. 오류 메시지는 [!UICONTROL EF Errors] 파일에 포함됩니다. 이 값은 광고 네트워크에 게시되지 않습니다. |
| [!UICONTROL SE Error Message] | (정보 목적으로 생성된 일괄 시트에 포함됨) 행의 데이터에 대한 광고 네트워크의 오류 메시지를 표시하는 자리 표시자입니다. 오류 메시지는 [!UICONTROL SE Errors] 파일에 포함됩니다. 이 값은 광고 네트워크에 게시되지 않습니다. |
| [!UICONTROL Exemption Request] | (정보 목적으로 생성된 일괄 시트에 포함됨) 광고가 위반하는 [!DNL Google Ads] 광고 정책의 이름과 텍스트를 표시하는 자리 표시자입니다. |
| [!UICONTROL Retail Hash] | (고급 캠페인 관리를 사용하여 생성된 일괄 시트에 정보 목적으로 포함됨) 고급(ACM) 보기를 사용하여 항목이 생성되었음을 나타내는 영숫자 해시 코드(예: f9639f40cdf56524b541e5dacf55a991). |

[^1]: [!DNL Excel]은(는) 파일을 열 때 큰 숫자를 과학적 표기법(예: 2115585666 2.12E+09)으로 변환합니다. 표준 표기법에서 숫자를 보려면 열에서 셀을 선택하고 수식 입력줄 내부를 클릭합니다.

## 각 계정 구성 요소를 생성, 편집 또는 삭제하는 데 필요한 필드 {#bulksheet-fields-per-component-google}

다음 섹션에는 특정 계정 엔티티와 관련된 필드가 포함되어 있습니다.

>[!NOTE]
>
>필드가 작업에 적용되지 않으면 필드에 입력된 값이 무시됩니다.

### 캠페인 필드

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-google)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Campaign Budget] | 캠페인을 만드는 데 필요합니다. |
| [!UICONTROL Delivery Method] | 캠페인을 만드는 데 필요합니다. |
| [!UICONTROL Channel Type] | 캠페인을 만드는 데 필요합니다. |
| [!UICONTROL Networks] | 캠페인을 만드는 데 필요합니다. |
| [!UICONTROL DSA Domain Name] | 검색 네트워크에서 동적 검색 광고를 사용하여 캠페인을 만드는 데 필요합니다. |
| [!UICONTROL DSA Domain Language] | 검색 네트워크에서 동적 검색 광고를 사용하여 캠페인을 만드는 데 필요합니다. |
| [!UICONTROL Campaign Priority] | 쇼핑 캠페인을 만드는 데 필요합니다. |
| [!UICONTROL Merchant ID] | 쇼핑 캠페인을 만드는 데 필요합니다. |
| [!UICONTROL Sales Country] | 쇼핑 캠페인을 만드는 데 필요합니다. |
| [!UICONTROL Product Scope Filter] | (쇼핑 캠페인) 선택 사항 |
| [!UICONTROL Languages] | 선택 사항 |
| [!UICONTROL Device Targets] | 선택 사항 |
| [!UICONTROL Device Targets (Google Adwords)] | 선택 사항 |
| [!UICONTROL Mobile Carriers (Google Adwords)] | 선택 사항 |
| [!UICONTROL Audience Target Method] | 해당 사항 없음 |
| [!UICONTROL Landing Page Suffix] | 선택 사항 |
| [!UICONTROL Tracking Template] | 선택 사항 |
| [!UICONTROL Campaign Status] | 캠페인을 삭제하는 데에만 필요합니다. |
| \[광고주별 레이블 분류\] | 선택 사항 |
| [!UICONTROL Constraints] | 선택 사항 |
| [!UICONTROL Campaign ID] | 행에 캠페인에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 캠페인 이름을 변경할 때만 필요합니다. |
| [!UICONTROL AMO ID] | 엔티티 ID 및 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

### 광고 그룹 필드

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-google)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Networks] | 해당 사항 없음 |
| [!UICONTROL GDN Custom Bid Level] | 선택 사항 |
| [!UICONTROL Ad Group Name] | 필수 |
| [!UICONTROL Ad Group Type] | 광고 그룹을 만드는 데 필요합니다. |
| [!UICONTROL Max CPC] | 선택 사항 |
| [!UICONTROL Max Content CPC] | 선택 사항 |
| [!UICONTROL Audience Target Method] | 필수 |
| [!UICONTROL Tracking Template] | 선택 사항 |
| [!UICONTROL Ad Group Status] | 광고 그룹을 삭제하는 데에만 필요합니다. |
| \[광고주별 레이블 분류\] | 선택 사항 |
| [!UICONTROL Constraints] | 선택 사항 |
| [!UICONTROL Ad Group ID] | 행에 광고 그룹에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 광고 그룹 이름을 변경할 때만 필요합니다. |
| [!UICONTROL AMO ID] | 엔티티 ID 및 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

### 키워드 필드

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-google)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Ad Group Name] | 필수 |
| [!UICONTROL Max CPC] | 선택 사항 |
| [!UICONTROL Keyword] | 필수 |
| [!UICONTROL Match Type] | 여러 일치 유형이 있는 키워드를 편집하거나 삭제하려면 일치 유형 또는 키워드 ID 값이 필요합니다. |
| [!UICONTROL Tracking Template] | 선택 사항 |
| [!UICONTROL Base URL/Final URL] | 선택 사항 |
| [!UICONTROL Custom URL Param] | 선택 사항 |
| [!UICONTROL Param1] | 선택 사항 |
| [!UICONTROL Param2] | 선택 사항 |
| [!UICONTROL Keyword Status] | 키워드를 삭제하는 데에만 필요합니다. |
| \[광고주별 레이블 분류\] | 선택 사항 |
| [!UICONTROL Constraints] | 선택 사항 |
| [!UICONTROL Campaign ID] | 선택 사항 |
| [!UICONTROL Ad Group ID] | 선택 사항 |
| [!UICONTROL Keyword ID] | 행에 a) 키워드를 식별하기에 충분한 속성 열 또는 b) &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 키워드를 편집하거나 삭제할 때만 필요합니다. |
| [!UICONTROL AMO ID] | 엔티티 ID 및 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

### 배치 필드

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-google)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Ad Group Name] | 필수 |
| [!UICONTROL Max Placement CPC (Google Adwords)] | 선택 사항 |
| [!UICONTROL Max Placement CPM (Google Adwords)] | 선택 사항 |
| [!UICONTROL Placement] | 필수 |
| [!UICONTROL Match Type] | 필수 |
| [!UICONTROL Tracking Template] | 선택 사항 |
| [!UICONTROL Base URL/Final URL] | 선택 사항 |
| [!UICONTROL Custom URL Param] | 선택 사항 |
| [!UICONTROL Placement Status] | 배치를 삭제하는 데에만 필요합니다. |
| \[광고주별 레이블 분류\] | 선택 사항 |
| [!UICONTROL Constraints] | 선택 사항 |
| [!UICONTROL Campaign ID] | 선택 사항 |
| [!UICONTROL Ad Group ID] | 선택 사항 |
| [!UICONTROL Placement ID] | 행에 a) 배치를 식별하기에 충분한 속성 열 또는 b) &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 배치를 편집하거나 삭제할 때만 필요합니다. |
| [!UICONTROL AMO ID] | 엔티티 ID 및 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

### 확장된 동적 검색 광고

이제 [!DNL Google Ads]에서 이 광고 유형을 &quot;동적 검색 광고&quot;라고 합니다. 동적 검색 광고 만들기에 대한 자세한 내용은 &quot;[동적 검색 광고 구현 [!DNL Google Ads] 2&rbrace;을 참조하세요.&quot;](https://experienceleague.adobe.com/docs/advertising/search-social-commerce/campaign-management/management/special-workflows/google-dynamic-search-ads.html)

이 광고 유형의 경우 [!UICONTROL Creative (except RSA)] 대화 상자에서 &quot;[!UICONTROL Download Bulksheet]&quot; 행을 사용하십시오.

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-google)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Ad Group Name] | 필수 |
| [!UICONTROL Creative Preferred Devices] | 선택 사항 |
| [!UICONTROL Description Line 1]-[!UICONTROL Description Line 2] | 광고를 만들거나 설명을 편집하는 데 필요합니다. <b>참고:</b> 이 광고 형식의 경우 광고 복사본을 변경하면 기존 광고가 삭제되고 새 광고가 만들어집니다. |
| [!UICONTROL Display URL] | 필수 |
| [!UICONTROL Tracking Template] | 선택 사항 |
| [!UICONTROL Creative Type] | 제품 광고의 상태를 만들거나 편집하는 데 필요합니다. |
| [!UICONTROL Ad Status] | 광고를 삭제하는 데 필요합니다. |
| \[광고주별 레이블 분류\] | 선택 사항 |
| [!UICONTROL Campaign ID] | 선택 사항 |
| [!UICONTROL Ad Group ID] | 선택 사항 |
| [!UICONTROL Ad ID] | 행에 a) 광고를 식별할 수 있는 충분한 광고 속성 열 또는 b) &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 광고 상태를 변경할 때만 필요합니다. 그러나 [!UICONTROL Ad ID]과(와) [!UICONTROL AMO ID]을(를) 모두 포함하지 않고 광고 속성 열이 여러 광고와 일치하는 경우 광고 중 하나에 대한 상태만 변경됩니다. |
| [!UICONTROL AMO ID] | 엔티티 ID 및 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

### 제품 목록/쇼핑 광고 필드

쇼핑 광고 만들기에 대한 자세한 내용은 &quot;[쇼핑 캠페인 구현 [!DNL Google Ads] 2&rbrace;&quot;을 참조하십시오.](https://experienceleague.adobe.com/docs/advertising/search-social-commerce/campaign-management/management/special-workflows/google-shopping-campaigns.html)

이 광고 유형의 경우 [!UICONTROL Creative (except RSA)] 대화 상자에서 &quot;[!UICONTROL Download Bulksheet]&quot; 행을 사용하십시오.

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-google)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Ad Group Name] | 필수 |
| [!UICONTROL Promotion Line] | 선택 사항 |
| [!UICONTROL Tracking Template] | 선택 사항 |
| [!UICONTROL Base URL/Final URL] | 선택 사항 |
| [!UICONTROL Custom URL Param] | 선택 사항 |
| [!UICONTROL Creative Type] | 제품 광고의 상태를 만들거나 편집하는 데 필요합니다. |
| [!UICONTROL Ad Status] | 광고를 삭제하는 데 필요합니다. |
| \[광고주별 레이블 분류\] | 선택 사항 |
| [!UICONTROL Constraints] | 선택 사항 |
| [!UICONTROL Campaign ID] | 선택 사항 |
| [!UICONTROL Ad Group ID] | 선택 사항 |
| [!UICONTROL Ad ID] | 행에 a) 광고를 식별할 수 있는 충분한 광고 속성 열 또는 b) &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 광고 상태를 변경할 때만 필요합니다. 그러나 [!UICONTROL Ad ID]과(와) [!UICONTROL AMO ID]을(를) 모두 포함하지 않고 광고 속성 열이 여러 광고와 일치하는 경우 광고 중 하나에 대한 상태만 변경됩니다. |
| [!UICONTROL AMO ID] | 엔티티 ID 및 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

### 반응형 검색 광고 필드

이 광고 유형의 경우 [!UICONTROL Responsive Search Ad] 대화 상자에서 &quot;[!UICONTROL Download Bulksheet]&quot; 행을 사용하십시오.

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-google)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Ad Group Name] | 필수 |
| [!UICONTROL Ad Title], [!UICONTROL Ad Title 2]-15 | 반응형 검색 광고의 경우 광고를 만들려면 [!UICONTROL Ad Title], [!UICONTROL Ad Title 2] 및 [!UICONTROL Ad Title 3]이(가) 필요하며 다른 모든 광고 제목 필드는 선택 사항입니다. 필수가 아닌 필드의 기존 값을 삭제하려면 값 `[delete]`(대괄호 포함)을(를) 사용합니다. |
| [!UICONTROL Ad Title 1 Position]-[!UICONTROL Ad Title 15 Position] | 선택 사항 |
| [!UICONTROL Description Line 1]-[!UICONTROL Description Line 4] | 반응형 검색 광고의 경우 광고를 만들려면 [!UICONTROL Description Line 1] 및 [!UICONTROL Description Line 2]이(가) 필요하며 [!UICONTROL Description Line 3] 및 [!UICONTROL Description Line 4]은(는) 선택 사항입니다. 기존 값을 삭제하려면 값 `[delete]`(대괄호 포함)을 사용하십시오. |
| [!UICONTROL Description Line 1 Position]-[!UICONTROL Description Line 4 Position] | 선택 사항 |
| [!UICONTROL Display Path 1] | 선택 사항 |
| [!UICONTROL Display Path 2] | 선택 사항 |
| [!UICONTROL Tracking Template] | 선택 사항 |
| [!UICONTROL Base URL/Final URL] | 광고를 만드는 데 필요합니다. |
| [!UICONTROL Custom URL Param] | 선택 사항 |
| [!UICONTROL Creative Type] | 선택 사항 |
| [!UICONTROL Ad Status] | 광고를 삭제하는 데 필요합니다. |
| \[광고주별 레이블 분류\] | 선택 사항 |
| [!UICONTROL Campaign ID] | 선택 사항 |
| [!UICONTROL Ad Group ID] | 선택 사항 |
| [!UICONTROL Ad ID] | 행에 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않은 경우 광고를 편집하거나 삭제하는 데 필요합니다. |
| [!UICONTROL AMO ID] | 광고 ID를 포함하지 않는 한 광고를 편집하거나 삭제하는 데 필요합니다. |

### 텍스트 광고 필드

이 광고 유형의 경우 [!UICONTROL Creative (except RSA)] 대화 상자에서 &quot;[!UICONTROL Download Bulksheet]&quot; 행을 사용하십시오.

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-google)&quot;을 참조하세요.

>[!NOTE]
>
>확장된 텍스트 광고는 2022년 6월에 더 이상 사용되지 않습니다. 기존 텍스트 광고만 삭제할 수 있습니다.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Ad Group Name] | 필수 |
| [!UICONTROL Creative Preferred Devices] | 읽기 전용 |
| [!UICONTROL Ad Title], 광고 제목 2-3 | 읽기 전용 |
| [!UICONTROL Description Line 1]-[!UICONTROL Description Line 2] | 읽기 전용 |
| [!UICONTROL Display URL] | 읽기 전용 |
| [!UICONTROL Display Path 1] | 읽기 전용 |
| [!UICONTROL Display Path 2] | 읽기 전용 |
| [!UICONTROL Tracking Template] | 읽기 전용 |
| [!UICONTROL Base URL/Final URL] | 읽기 전용 |
| [!UICONTROL Custom URL Param] | 읽기 전용 |
| [!UICONTROL Creative Type] | 선택 사항 |
| [!UICONTROL Ad Status] | 필수 |
| \[광고주별 레이블 분류\] | 선택 사항 |
| [!UICONTROL Campaign ID] | 선택 사항 |
| [!UICONTROL Ad Group ID] | 선택 사항 |
| [!UICONTROL Ad ID] | 행에 a&rpar; 광고 또는 b&rpar; &quot;[!UICONTROL AMO ID]&quot;을(를) 식별하는 데 충분한 광고 속성 열이 포함되지 않는 한 광고 상태를 변경할 때만 필요합니다. 그러나 [!UICONTROL Ad ID]과(와) [!UICONTROL AMO ID]을(를) 모두 포함하지 않고 광고 속성 열이 여러 광고와 일치하는 경우 광고 중 하나에 대한 상태만 변경됩니다. |
| [!UICONTROL AMO ID] | 엔티티 ID 및 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

### 동적 검색 대상(자동 타겟) 필드

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-google)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Ad Group Name] | 필수 |
| [!UICONTROL Max CPC] | 선택 사항 |
| [!UICONTROL Auto Target Expression] | 캠페인 설정 &quot;[!UICONTROL Use my website contents to target my ads]&quot;을(를) 사용할 수 없는 경우에만 필요합니다. |
| [!UICONTROL Match Type] | 선택 사항 |
| [!UICONTROL Target Status] | 대상을 삭제하는 데 필요합니다. |
| \[광고주별 레이블 분류\] | 선택 사항 |
| [!UICONTROL Constraints] | 선택 사항 |
| [!UICONTROL Campaign ID] | 선택 사항 |
| [!UICONTROL Ad Group ID] | 선택 사항 |
| [!UICONTROL Target ID] | 행에 대상에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 자동 대상을 변경하거나 삭제할 때만 필요합니다. |
| [!UICONTROL AMO ID] | 엔티티 ID 및 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

### 쇼핑 제품 그룹 필드

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-google)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Ad Group Name] | 필수 |
| [!UICONTROL Max CPC] | 제품 그룹을 만드는 데 필요합니다. |
| [!UICONTROL Parent Product Groupings] | 필수 |
| [!UICONTROL Product Grouping] | 필수 |
| [!UICONTROL Partition Type] | 제품 그룹을 만드는 데 필요합니다. |
| [!UICONTROL Match Type] | 선택 사항 |
| [!UICONTROL Tracking Template] | 선택 사항 |
| [!UICONTROL Base URL/Final URL] | 필수 |
| [!UICONTROL Product Group Status] | 제품 그룹을 삭제하는 데에만 필요합니다. |
| \[광고주별 레이블 분류\] | 선택 사항 |
| [!UICONTROL Constraints] | 선택 사항 |
| [!UICONTROL Campaign ID] | 선택 사항 |
| [!UICONTROL Ad Group ID] | 선택 사항 |
| [!UICONTROL Product Group ID] | 행에 a) 제품 그룹을 식별하는 데 충분한 속성 열 또는 b) &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 제품 그룹을 변경하거나 삭제할 때만 필요합니다. |
| [!UICONTROL AMO ID] | 엔티티 ID 및 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

### 캠페인 수준 및 광고 그룹 수준의 사이트링크 필드

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-google)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Ad Group Name] | 광고 그룹 수준 사이트 링크에 필요합니다. 캠페인 수준 사이트 링크에 적용할 수 없습니다. |
| [!UICONTROL Creative Preferred Devices] | 선택 사항 |
| [!UICONTROL Link Name] | 필수 |
| [!UICONTROL Start Date] | 선택 사항 |
| [!UICONTROL End Date] | 선택 사항 |
| [!UICONTROL Tracking Template] | 선택 사항 |
| [!UICONTROL Base URL/Final URL] | 필수 |
| [!UICONTROL Sitelink Status] | 사이트링크를 삭제하는 데에만 필요합니다. |
| [!UICONTROL Campaign ID] | 선택 사항 |
| [!UICONTROL Ad Group ID] | 선택 사항 |
| [!UICONTROL Sitelink ID] | 행에 a) 사이트 링크를 식별할 수 있는 충분한 속성 열 또는 b) &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 사이트 링크를 변경하거나 삭제하는 경우에만 필요합니다. 그러나 [!UICONTROL Sitelink ID]과(와) [!UICONTROL AMO ID]을(를) 모두 포함하지 않고 속성 열이 여러 사이트 링크와 일치하는 경우 사이트 링크 중 하나의 상태만 변경됩니다.<br><br><b>참고:</b> 기존 사이트 링크에 대해 [!UICONTROL Status]을(를) 제외한 사이트 링크 속성 열을 편집하고 [!UICONTROL Sitelink ID] 또는 [!UICONTROL AMO ID]을(를) 포함하지 않으면 새 사이트 링크가 만들어지고 기존 사이트 링크는 변경되지 않습니다. |
| [!UICONTROL AMO ID] | 엔티티 ID 및 상위 엔티티 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

### 위치 대상

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-google)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Location] | 필수 |
| [!UICONTROL Location Type] | 선택 사항 |
| [!UICONTROL Bid Adjustment] | 선택 사항 |
| [!UICONTROL Location Status] | 위치 대상을 삭제하는 데에만 필요합니다. |
| [!UICONTROL Campaign ID] | 선택 사항 |
| [!UICONTROL AMO ID] | [!UICONTROL Campaign ID]을(를) 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

### 캠페인 수준 및 광고 그룹 수준 장치 대상 필드

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-google)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Device] | 장치 대상을 만들거나 편집하는 데 필요합니다. |
| [!UICONTROL Bid Adjustment] | 선택 사항 |
| [!UICONTROL Ad Group Name] | 광고 그룹 수준 장치 대상에 필요합니다. 캠페인 수준 장치 타겟에는 적용할 수 없습니다. |
| [!UICONTROL Device Target Status] | 장치 대상을 삭제하는 데에만 필요합니다. |
| [!UICONTROL Campaign ID] | 선택 사항 |
| [!UICONTROL Ad Group ID] | 선택 사항, 광고 그룹 수준 장치 대상에만 적용됩니다. |
| [!UICONTROL Device Target ID] | 행에 대상에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 대상을 변경하거나 삭제할 때만 필요합니다. |
| [!UICONTROL AMO ID] | 장치 대상 ID를 포함하지 않는 한 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |

### 캠페인 수준 및 광고 그룹 수준의 RLSA 대상/제외 필드

각 데이터 필드에 대한 설명은 &quot;[사용 가능한 모든 데이터 필드](#bulksheet-fields-all-google)&quot;을 참조하세요.

| 필드 | 필수? |
| ---- | ---- |
| [!UICONTROL Acct Name] | 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 |
| [!UICONTROL Bid Adjustment] | 선택 사항 |
| [!UICONTROL Ad Group Name] | 광고 그룹 수준의 타겟 및 제외에 필요합니다. 캠페인 수준 타겟 및 제외에 적용할 수 없습니다. |
| [!UICONTROL Audience] | 새 대상 또는 제외를 만드는 데 필요합니다. |
| [!UICONTROL Target Type] | 새 대상 또는 제외를 만드는 데 필요합니다. |
| [!UICONTROL RLSA Target Status] | 대상 또는 제외를 삭제하는 데에만 필요합니다. |
| [!UICONTROL Campaign ID] | 선택 사항 |
| [!UICONTROL Ad Group ID] | 선택 사항, 광고 그룹 수준 타겟 및 제외에만 적용할 수 있습니다. |
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
