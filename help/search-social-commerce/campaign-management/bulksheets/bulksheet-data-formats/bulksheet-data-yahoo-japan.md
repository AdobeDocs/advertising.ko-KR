---
title: 다음에 대한 일괄 시트 데이터 [!DNL Yahoo! Japan] 계정
description: 다운로드한 일괄 시트의 헤더 필드 및 데이터 필드 참조 [!DNL Yahoo! Japan] 계정.
exl-id: 78eb41ce-3854-454c-adf2-ba0339e2aef7
feature: Search Bulksheets
source-git-commit: 67fe8581832dc0762d62908d01672e53cc95b847
workflow-type: tm+mt
source-wordcount: '2668'
ht-degree: 0%

---

# 부록 - 다음에 대한 일괄 시트 데이터 [!DNL Yahoo! Japan] 계정

다음에 대한 데이터를 다운로드할 수 있습니다. [!DNL Yahoo! Japan] 계정은 대량으로 저장되지만 일괄 시트를 광고 네트워크에 업로드하거나 게시할 수 없습니다.

<!-- Hiding because this is probably too long a list to be useful.

## Available header fields

Platform,Acct Name,Campaign Name,Campaign Budget,Delivery Method,Mobile Bid Adjustment,Location,Location Type,Ad Group Name,Max CPC,Keyword,Match Type,First Page Bid, Quality Score,Ad Name (Yahoo JP),Creative Preferred Devices,Ad Title,Ad Title2,Description Line 1,Description Line 2,Creative Type,Display URL,Display Path 1,Display Path 2,Base URL/Final URL,Destination URL,Tracking Template,Campaign Status,Ad Group Status,Keyword Status,Ad Status,Location Status,[Advertiser-specific Label Classification],Constraints,Campaign ID,Ad Group ID,Keyword ID,Ad ID,AMO ID,Error Message

{{$include /help/_includes/bulksheet-headers-note.md}}

-->

## 사용 가능한 데이터 필드

>[!TIP]
>
>다음 테이블은 넓습니다. 필요한 경우 표 하단에 있는 스크롤 막대를 사용하여 전체 내용을 봅니다. 원할 경우 를 클릭하여 목차나 오른쪽 창을 일시적으로 숨길 수도 있습니다 ![왼쪽 창 숨기기](/help/search-social-commerce/assets/hide-left-pane.png "왼쪽 창 숨기기") 왼쪽 창 또는 ![오른쪽 창 숨기기](/help/search-social-commerce/assets/hide-right-pane.png "오른쪽 창 숨기기") 오른쪽 창의 맨 위에 있습니다.

| 필드 | 캠페인 | 광고 그룹 | 키워드 | 텍스트 광고 | 캠페인 위치 타겟 | 설명 |
|----|----|----|----|----|----|----|
| [!UICONTROL Platform] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함) 광고 플랫폼. 각 행에 &quot;가 포함되지 않은 경우 필수[!UICONTROL AMO ID]엔티티의 경우 &quot;. |
| [!UICONTROL Acct Name] | 필수/선택 사항 | 필수/선택 사항 | 필수/선택 사항 | 필수/선택 사항 | 필수/선택 사항 | 광고 네트워크 계정을 식별하는 고유한 이름. 각 행에 &quot;가 포함되지 않은 경우 필수[!UICONTROL AMO ID]엔티티의 경우 &quot;. |
| [!UICONTROL Campaign Name] | 필수 | 필수 | 필수 | 필수 | 필수 | 계정에 대한 캠페인을 식별하는 고유한 이름. |
| [!UICONTROL Campaign Budget] | 필수: 만들기<br><br>선택 사항: 편집 또는 삭제 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 금전적 기호와 구두점을 포함하거나 포함하지 않는 캠페인에 대한 일일 지출 제한. 이 값은 재정의되지만 계정 예산을 초과할 수 없습니다. |
| [!UICONTROL Delivery Method] | 필수: 만들기<br><br>선택 사항: 편집 또는 삭제 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 매일 캠페인에 대한 광고를 표시하는 속도:<ul><li>*[!UICONTROL Standard (Distributed)]* (새 캠페인의 기본값): 광고 노출을 하루 전체에 분산합니다.</li><li>*[!UICONTROL Accelerated]:* 예산에 도달할 때까지 가능한 한 자주 광고를 표시합니다. 그 결과, 오늘 오후에 광고가 표시되지 않을 수 있습니다.</li></ul> |
| [!UICONTROL Mobile Bid Adjustment] | 선택 사항 | 선택 사항 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 캠페인 수준 또는 광고 그룹 수준에서 모바일 장치의 광고 입찰 여부를 지정합니다.<ul><li>기존 모바일 입찰 조정을 사용하려면 이 항목을 비워 둡니다.</li><li>모바일 디바이스에서 광고를 입찰하지 않으려면 다음을 입력합니다. `-100`.</li><li>데스크탑 및 태블릿 디바이스의 광고와 동일한 입찰가를 사용하여 모바일 디바이스의 광고를 입찰하려면(0% 차이) 다음을 입력합니다. `0`. 새 캠페인의 경우 이 항목을 비워 둘 수도 있습니다.</li><li>다른 입찰을 사용하여 모바일 디바이스에서 광고를 입찰하려면 입찰을 늘리거나 줄일 비율을 입력합니다. 값은 다음에서 산출할 수 있습니다. `-90` 끝 `300`.</li></ul>캠페인 수준에서 장치를 제외하는 경우 광고 그룹 수준에서 제외를 무시할 수 없습니다.<br><br><b>참고:</b><ul><li>광고 그룹은 캠페인 수준 설정을 상속하지만, 이를 재정의할 수 있습니다.</li><li>최적화된 포트폴리오에 캠페인을 할당하면 최적화 기능이 기본 키워드 수준의 입찰가를 자동으로 결정하여 포트폴리오가 목표를 달성할 수 있도록 합니다. 그런 다음 광고 네트워크는 모바일 광고에 대해 지정된 입찰가를 조정합니다.</li><li>캠페인이나 광고 그룹을 최적화된 포트폴리오에 할당하는 경우:<ul><li>최적화 기능은 포트폴리오가 목표를 달성할 수 있도록 기본 키워드 수준의 입찰을 자동으로 결정합니다. 그런 다음 검색 네트워크는 모바일 광고에 대해 지정된 대로 입찰가를 조정합니다.</li><li>포트폴리오가 &quot;[!UICONTROL Auto-optimize Bid Adjustment Values],&quot; 그런 다음 계산되는 이상적인 값이 포트폴리오 설정에 지정된 최소 및 최대 값 내에 있고 광고 그룹이 모바일 광고에 대한 입찰을 제외하지 않는 한 최적화 기능은 광고 그룹 수준에서 입찰 조정을 변경합니다.</li></ul></li></ul> |
| [!UICONTROL Location] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 선택 사항 | 캠페인을 위한 광고를 배치할 지리적 위치입니다. 도시의 경우 &quot;&lt; 형식을 사용하십시오.<i>도시</i>>, &lt;</i>현</i>>&quot;(예: 도쿄 아다치). 위치를 제외하려면 빼기 기호(`-`). 캠페인에 대한 특정 값을 입력하지 않으면 모든 위치가 타깃팅됩니다. |
| [!UICONTROL Location Type] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수/선택 사항 | (특정 위치를 타깃팅할 때 필수) 지정된 위치가 유형인지 여부 [!UICONTROL Prefecture] 또는 [!UICONTROL City]. |
| [!UICONTROL Ad Group Name] | 해당 사항 없음 | 필수 | 필수 | 필수 | 해당 사항 없음 | 캠페인 내에서 고유한 광고 그룹 이름입니다. 최대 길이는 50자입니다. |
| [!UICONTROL Max CPC] | 해당 사항 없음 | 선택 사항 | 선택 사항 | 해당 사항 없음 | 해당 사항 없음 | CPC(최대 클릭당 비용)로, 금전적 기호와 구두점을 사용하거나 사용하지 않고 검색 네트워크에서 광고 클릭에 대해 지불하는 가장 높은 금액입니다. 광고 그룹 및 키워드에 대한 값을 설정할 수 있습니다. 새 키워드의 기본값은 광고 그룹 수준에서 상속됩니다. |
| [!UICONTROL Keyword] | 선택 사항 / 해당 사항 없음 | 선택 사항 / 해당 사항 없음 | 필수 | 해당 사항 없음 | 해당 사항 없음 | 키워드 문자열입니다. [!DNL Yahoo! Japan] 키워드 및 일치 유형은 변경할 수 있으므로 기존 키워드를 삭제하지 않고 편집할 수 있습니다.<br><br>광고 그룹 또는 캠페인 수준에서 키워드를 제외하려면 [!UICONTROL Match Type] &quot;부정적&quot;으로 변경되었습니다. 행에 광고 그룹 이름이 포함된 경우 광고 그룹에 대한 키워드는 제외됩니다. 행에 광고 그룹 이름이 포함되지 않으면 전체 캠페인에 대해 키워드가 제외됩니다. |
| [!UICONTROL Match Type] | 선택 사항 / 해당 사항 없음 | 선택 사항 / 해당 사항 없음 | 선택 사항: 만들기<br><br>필수/선택 사항: 편집 또는 삭제 | 해당 사항 없음 | 해당 사항 없음 | 키워드에 대한 키워드 일치 옵션: *[!UICONTROL Broad]* (새 키워드의 기본값), *[!UICONTROL Exact]*, *[!UICONTROL Phrase]*, *[!UICONTROL Negative Broad], 또는 *[!UICONTROL Negative Exact]*. 캠페인 수준 또는 광고 그룹 수준에서 부정적인 키워드를 정의합니다. [!DNL Yahoo! Japan] 키워드 및 일치 유형은 변경할 수 있으므로 기존 키워드를 삭제하지 않고 편집할 수 있습니다.<br><br>일치 유형 또는 키워드 ID 값은 여러 일치 유형이 있는 키워드를 편집하는 데만 필요합니다. |
| [!UICONTROL First Page Bid] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함) 검색 결과의 첫 페이지에 광고를 배치하는 데 필요한 입찰입니다. 이 값은 광고 네트워크에 게시되지 않습니다. |
| [!UICONTROL Quality Score] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함) 광고 네트워크에서 키워드에 할당한 현재 품질 점수입니다. 이 값은 광고 네트워크에 게시되지 않습니다. |
| [!UICONTROL Ad Name (Yahoo JP)] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 선택 사항: 만들기<br><br>필수/선택 사항: 편집 또는 삭제 | 해당 사항 없음 | 광고 그룹 내에서 광고 이미지를 식별하는 고유한 이름. 최대 길이는 50자입니다. 를 사용하지 않는 한 필수입니다. [!UICONTROL AMO ID] 또는 [!UICONTROL Ad ID] 행을 위해. |
| [!UICONTROL Creative Preferred Devices] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 선택 사항 | 해당 사항 없음 | 광고를 표시할 디바이스 유형: *[!UICONTROL All]* (기본값) 또는 *[!UICONTROL Mobile]*. 대상 [!UICONTROL Mobile], 광고 네트워크는 데스크탑 또는 태블릿 사용자가 아닌 모바일 장치 사용자에게 광고를 표시하려고 합니다. 그렇지 않으면 모든 장치 유형에 광고가 표시됩니다.<br><br>관리자만 및 [!DNL Adobe] 계정 관리자 사용자는 이 설정을 편집할 수 있습니다. |
| [!UICONTROL Ad Title] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수 | 해당 사항 없음 | 광고의 헤드라인입니다. 최대 길이는 싱글바이트 30자 또는 더블바이트 15자입니다. 광고 사본을 변경하면 기존 광고가 삭제되고 새 광고가 만들어집니다. |
| [!UICONTROL Ad Title 2] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수 / 해당 사항 없음 | 해당 사항 없음 | (확장 텍스트 광고만 해당) 두 번째 헤드라인입니다. 최대 길이는 30자 또는 15개의 더블바이트 문자입니다. 광고 사본을 변경하면 기존 광고가 삭제되고 새 광고가 만들어집니다. |
| [!UICONTROL Description Line 1] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수 | 해당 사항 없음 | 광고 본문. 확장 텍스트 광고의 경우 최대 길이는 80개의 1바이트 문자 또는 40개의 2바이트 문자입니다. 광고 사본을 변경하면 기존 광고가 삭제되고 새 광고가 만들어집니다. |
| [!UICONTROL Description Line 2] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수 | 해당 사항 없음 | (표준 텍스트 광고만 해당) 광고 본문의 두 번째 줄입니다. 최대 길이는 싱글바이트 38자 또는 더블바이트 19자입니다. 광고 사본을 변경하면 기존 광고가 삭제되고 새 광고가 만들어집니다. <b>참고:</b> [!DNL Yahoo! Japan Ads] 에서는 더 이상 표준 텍스트 광고를 만들고 편집할 수 없습니다. |
| [!UICONTROL Creative Type] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 선택 사항 | 해당 사항 없음 | 광고 형식:<ul><li>*[!UICONTROL Text]* (새 광고의 기본값): 컴퓨터, 태블릿 및 스마트폰에 표시될 수 있는 텍스트 광고입니다.</li><li>*[!UICONTROL Mobile]:* 사용하지 않음.</li></ul> |
| [!UICONTROL Display URL] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수 / 해당 사항 없음: 만들기<br><br>선택 사항 / 해당 사항 없음: 편집 또는 삭제 | 해당 사항 없음 | (기존 표준 텍스트 광고만, 읽기 전용) 광고에 표시되는 URL입니다. 최대 길이는 255개의 1바이트 문자 또는 127개의 2바이트 문자입니다. 또한 표시 URL과 랜딩 페이지 URL의 도메인은 동일해야 합니다. <b>참고:</b> [!DNL Yahoo! Japan Ads] 는 표준 텍스트 및 확장 텍스트 광고의 생성 및 편집을 더 이상 사용하지 않습니다. |
| [!UICONTROL Display Path 1], [!UICONTROL Display Path 2] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 선택 사항 / 해당 사항 없음 | 해당 사항 없음 | (확장 텍스트 광고만 해당, 선택 사항) 디스플레이 URL에 추가되고 최종 URL에서 자동으로 추출되는 텍스트입니다. URL 앞에는 슬래시(`/`). 경로에는 슬래시()를 사용할 수 없습니다.`/`) 또는 줄바꿈(`\n`)자. 최대 길이는 15자 또는 7개의 더블바이트 문자입니다.<br><br>광고 사용자 정의자를 삽입하려면 다음 형식을 사용하십시오. `Default text` 는 피드 파일에 유효한 값이 포함되지 않았을 때 삽입할 선택적 값입니다.<ul><li>[!DNL Google Ads]: `{CUSTOMIZER.AdCustomizerName:Default text}, such as {CUSTOMIZER.Discount:10%}`</li><li>[!DNL Microsoft Advertising]: `{CUSTOMIZER.Attribute name:Default text}, such as {CUSTOMIZER.Discount:10%}`</li></ul>예를 들어 다음과 같습니다. [!UICONTROL Display Path 1] 은 &quot;거래&quot;이고, 표시 URL은 다음과 같습니다. `&lt;display URL&gt;/deals`예: www.example.com/deals |
| [!UICONTROL Base URL/Final URL] | 해당 사항 없음 | 해당 사항 없음 | 선택 사항 | 필수 | 해당 사항 없음 | 최종 사용자가 광고를 클릭할 때 고려할 랜딩 페이지 URL(캠페인이나 계정에 대해 구성된 추가 매개 변수 포함). 키워드 수준의 기본/최종 URL은 광고 수준 이상의 URL을 무시합니다. |
| [!UICONTROL Destination URL] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함됨, 광고 네트워크에 게시되지 않음) 대상 URL이 있는 계정의 경우 이 URL은 광고를 광고주 웹 사이트의 기본 URL/랜딩 페이지에 연결하는 URL입니다(경우에 따라 클릭을 추적한 다음 사용자를 랜딩 페이지로 리디렉션하는 다른 사이트를 통해). 여기에는 Search, Social 및 Commerce 캠페인 또는 계정에 대해 구성된 추가 매개 변수가 포함됩니다. 추적 URL을 생성한 경우, 이는 계정 설정 및 캠페인 설정의 추적 매개 변수를 기반으로 합니다. 광고 네트워크별 매개 변수를 추가한 경우 검색, 소셜 및 Commerce에 대해 동일한 매개 변수로 대체될 수 있습니다.<br><br>최종 URL이 있는 계정의 경우 이 열은 기본 URL/최종 URL 열과 동일한 값을 표시합니다.<br><br>키워드 또는 배치 수준의 대상 URL은 광고 수준의 URL을 무시합니다. |
| [!UICONTROL Tracking Template] | 선택 사항 | 선택 사항 | 선택 사항 | 선택 사항 | 선택 사항 | (선택 사항) 모든 오프랜딩 도메인 리디렉션 및 추적 매개 변수를 지정하고 또한 최종/랜딩 페이지 URL을 매개 변수에 임베드하는 추적 템플릿 또는 추적 URL. 매개 변수 사용 `!{lpurl}` 랜딩 페이지 URL을 나타냅니다. 예: `{lpurl}?source={network}&id=5` 또는 `http://www.trackingservice.example.com/?url={lpurl}?source={network}&id=5` 리디렉션을 포함합니다.<br><br>원할 경우 서드파티 리디렉션 및 추적을 추가할 수 있습니다.<br><br>Adobe Advertising 전환 추적의 경우, 캠페인 설정에 이 포함되어 있을 때 적용됩니다.[!UICONTROL EF Redirect]&quot; 및 &quot;[!UICONTROL Auto Upload],&quot; Search, Social 및 Commerce은 레코드를 저장할 때 자체 리디렉션 및 추적 코드 앞에 자동으로 추가됩니다.<br><br>가장 세분화된 수준의 추적 템플릿은 모든 상위 수준의 값을 재정의합니다. 예를 들어 계정 설정과 키워드 설정 모두에 값이 포함된 경우 키워드 값이 적용됩니다. |
| [!UICONTROL Campaign Status] | 선택 사항: 만들기 또는 편집<br><br>필수: 삭제 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 캠페인의 표시 상태: *[!UICONTROL Active]* (새 캠페인의 기본값), *[!UICONTROL Paused]*, *[!UICONTROL Ended]* (기존 캠페인만) 또는 *[!UICONTROL Deleted]* (기존 캠페인만 해당). |
| [!UICONTROL Ad Group Status] | 해당 사항 없음 | 선택 사항: 만들기 또는 편집<br><br>필수: 삭제 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 광고 그룹의 표시 상태:  *[!UICONTROL Active]*, *[!UICONTROL Paused]*, 또는 *[!UICONTROL Deleted]* (기존 광고 그룹만 해당). 새 광고 그룹의 기본값은 입니다 [!UICONTROL Active]. 활성 또는 일시 중지된 광고 그룹을 삭제하려면 값을 입력합니다 `Deleted`. |
| [!UICONTROL Keyword Status] | 해당 사항 없음 | 해당 사항 없음 | 선택 사항: 만들기 또는 편집<br><br>필수: 삭제 | 해당 사항 없음 | 해당 사항 없음 | 키워드의 표시 상태: *[!UICONTROL Active]*, *[!UICONTROL Deleted]* (기존 키워드만), *[!UICONTROL Disapproved]* (편집할 수 없음), *[!UICONTROL Paused]* (기존 키워드만) 또는 *[!UICONTROL Pending]* (편집할 수 없음). 새 키워드의 기본값은 입니다 [!UICONTROL Active]. 키워드를 삭제하려면 값을 입력합니다 `Deleted`. |
| [!UICONTROL Ad Status] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 선택 사항: 만들기 또는 편집<br><br>필수: 삭제 | 해당 사항 없음 | 광고의 표시 상태: *[!UICONTROL Active]* (새 광고의 기본값), *[!UICONTROL Deleted]* (기존 광고만), *[!UICONTROL Disapproved]* (편집할 수 없음), *[!UICONTROL Paused]*, 또는 *[!UICONTROL Pending]* (편집할 수 없음). 새 광고의 기본값은 입니다 [!UICONTROL Active]. 광고를 삭제하려면 값을 입력합니다 `Deleted`. |
| [!UICONTROL Location Status] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 선택 사항 | 위치 대상의 상태: *[!UICONTROL Active]* 또는 *[!UICONTROL Deleted]* (기존 위치만 해당) 새 위치의 기본값은 입니다. [!UICONTROL Active]. 활성 위치를 삭제하려면 값을 입력합니다 `Deleted`. |
| \[광고주별 레이블 분류\] | 선택 사항 | 선택 사항 | 선택 사항 | 선택 사항 | 선택 사항 | (Color라는 레이블 분류의 경우 &quot;Color&quot;와 같이 광고주별 레이블 분류에 대해 이름이 지정됨) 엔티티와 연결된 지정된 분류의 값입니다. 엔티티당 분류당 하나의 값만 포함할 수 있습니다(예: 캠페인 A의 &quot;색상&quot; 레이블 분류의 경우 &quot;빨간색&quot;). 최대 길이는 100자이고 값에는 ASCII 및 비 ASCII 문자가 포함될 수 있습니다.<br><br>레이블 분류 및 해당 레이블 값은 모든 하위 구성 요소에 적용됩니다. 나중에 추가되는 새 구성 요소는 자동으로 레이블과 연결됩니다. <br><br>분류 이름과 분류 값은 대/소문자를 구분하지 않습니다. |
| [!UICONTROL Constraints] | 선택 사항 | 선택 사항 | 선택 사항 | 선택 사항 | 해당 사항 없음 | 엔티티에 할당된 제약 조건입니다. 엔티티당 하나의 제약조건만 지정할 수 있습니다.<br><br>구속은 하위 엔티티에 의해 상속되므로 상속된 값을 재정의하지 않는 한 하위 엔티티에 대한 값을 입력할 필요가 없습니다. |
| [!UICONTROL Campaign ID] | 해당 사항 없음: 만들기<br><br>필수/선택 사항: 편집 또는 삭제 | 선택 사항 | 선택 사항 | 선택 사항 | 해당 사항 없음 | 기존 캠페인을 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(`'`).[^1] 행에 &quot;&quot;가 포함되지 않은 경우 캠페인 이름을 변경할 때만 필요합니다.[!UICONTROL AMO ID]캠페인을 위한 &quot;입니다. |
| [!UICONTROL Ad Group ID] | 해당 사항 없음 | 해당 사항 없음: 만들기<br><br>필수/선택 사항: 편집 또는 삭제 | 선택 사항 | 선택 사항 | 해당 사항 없음 | 기존 광고 그룹을 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(`'`).[^1] 행에 &quot;&quot;가 포함되지 않은 경우 광고 그룹 이름을 변경할 때만 필요합니다.[!UICONTROL AMO ID]광고 그룹용 |
| [!UICONTROL Keyword ID] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음: 만들기<br><br>필수/선택 사항: 편집<br><br>필수: 삭제 | 해당 사항 없음 | 해당 사항 없음 | 기존 키워드를 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(`'`).[^1] 행에 a) 키워드를 식별할 수 있는 충분한 속성 열 또는 b) &quot;가 포함되지 않는 한, 키워드를 편집하거나 삭제할 때만 필요합니다.[!UICONTROL AMO ID].&quot; |
| [!UICONTROL Ad ID] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음: 만들기<br><br>필수/선택 사항: 편집 또는 삭제 | 해당 사항 없음 | 기존 광고를 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(`'`).[^1] 반응형 검색 광고의 경우 [!UICONTROL Ad ID] 또는 [!UICONTROL AMO ID] 광고 데이터를 편집하거나 삭제하는 데 필요합니다. 다른 모든 엔티티 유형의 경우 [!UICONTROL AMO ID] 행에 a) 광고를 식별할 수 있는 충분한 광고 속성 열 또는 b) &quot;가 포함되지 않는 한 광고 상태를 변경할 때만 필요합니다.[!UICONTROL AMO ID].&quot; 그러나 둘 다 포함하지 않는 경우 [!UICONTROL Ad ID] nor [!UICONTROL AMO ID], 그리고 광고 속성 열이 여러 광고와 일치하면 광고 중 하나의 상태만 변경됩니다.<br><br><b>참고:</b> a) 광고 속성 열을 편집하는 경우 [!UICONTROL Status] 기존 광고의 경우 또는 b) 응답형 검색 광고에 대한 모든 데이터이며 [!UICONTROL Ad ID] nor [!UICONTROL AMO ID]새 광고가 만들어지고 기존 광고는 변경되지 않습니다. |
| [!UICONTROL AMO ID] | 해당 사항 없음: 만들기<br><br>선택 사항: 편집 또는 삭제 | 해당 사항 없음: 만들기<br><br>선택 사항: 편집 또는 삭제 | 해당 사항 없음: 만들기<br><br>선택 사항: 편집 또는 삭제 | 해당 사항 없음: 만들기<br><br>선택 사항: 편집 또는 삭제 | 해당 사항 없음 | (생성된 일괄 시트에서) [!DNL Adobe]동기화된 엔터티에 대해 생성된 고유 식별자입니다. 반응형 검색 광고의 경우 [!UICONTROL AMO ID] 을 포함하지 않는 한 광고를 편집하거나 삭제해야 합니다. [!UICONTROL Ad ID]. 을 사용하여 다른 모든 엔티티 유형의 데이터를 편집하려면 다음과 같이 하십시오 [!UICONTROL AMO ID], [!UICONTROL AMO ID] 엔티티 ID 및 상위 엔티티 ID를 포함하지 않는 경우 데이터를 편집하거나 삭제하는 데 필요합니다.<br><br>Search, Social 및 Commerce은 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |
| [!UICONTROL EF Error Message] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함됨) 검색, 소셜 및 Commerce에서 행의 데이터에 대한 오류 메시지를 표시하는 자리 표시자입니다. 오류 메시지는에 포함됩니다. [!UICONTROL EF Errors] 파일. 이 값은 광고 네트워크에 게시되지 않습니다. |
| [!UICONTROL SE Error Message] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함됨) 행의 데이터에 대해 광고 네트워크에서 오류 메시지를 표시하는 자리 표시자입니다. 오류 메시지는에 포함됩니다. [!UICONTROL SE Errors] 파일. 이 값은 광고 네트워크에 게시되지 않습니다. |

[^1]: Excel은 파일을 열 때 큰 숫자를 과학적 표기법(예: 2.12E+2115585666)으로 변환합니다. 표준 표기법에서 숫자를 보려면 열에서 셀을 선택하고 수식 입력줄 내부를 클릭합니다.

>[!MORELIKETHIS]
>
>* [부록 - 일괄 시트 오류](../bulksheet-errors.md)
>* [일괄 시트에서 수행할 수 있는 작업](bulksheet-operations.md)
>* [지원되는 일괄 시트 파일 형식](bulksheet-file-formats.md)
>* [일괄 시트 파일 다운로드/만들기](../bulksheet-download.md)
>* [클릭 추적 형식 [!DNL Naver]](/help/search-social-commerce/tracking/formats-click-tracking-naver.md)
>* [일괄 시트 파일 또는 수정된 오류 파일 업로드](../bulksheet-upload.md)
