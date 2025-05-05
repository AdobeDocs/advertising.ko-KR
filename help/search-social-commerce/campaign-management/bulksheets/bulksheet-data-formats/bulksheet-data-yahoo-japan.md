---
title: ' [!DNL Yahoo! Japan] 계정의 일괄 시트 데이터'
description: ' [!DNL Yahoo! Japan] 계정에 대해 다운로드한 일괄 시트의 머리글 필드 및 데이터 필드를 참조합니다.'
exl-id: 78eb41ce-3854-454c-adf2-ba0339e2aef7
feature: Search Bulksheets
source-git-commit: 5c750153ff9e4be2d02f572d96b171d7aa293dd9
workflow-type: tm+mt
source-wordcount: '2672'
ht-degree: 0%

---

# 부록 - [!DNL Yahoo! Japan] 계정에 대한 일괄 시트 데이터

[!DNL Yahoo! Japan] 계정의 데이터를 대량으로 다운로드할 수 있지만 일괄 시트를 광고 네트워크에 업로드하거나 게시할 수 없습니다.

<!-- Hiding because this is probably too long a list to be useful.

## Available header fields

Platform,Acct Name,Campaign Name,Campaign Budget,Delivery Method,Mobile Bid Adjustment,Location,Location Type,Ad Group Name,Max CPC,Keyword,Match Type,First Page Bid, Quality Score,Ad Name (Yahoo JP),Creative Preferred Devices,Ad Title,Ad Title2,Description Line 1,Description Line 2,Creative Type,Display URL,Display Path 1,Display Path 2,Base URL/Final URL,Destination URL,Tracking Template,Campaign Status,Ad Group Status,Keyword Status,Ad Status,Location Status,[Advertiser-specific Label Classification],Constraints,Campaign ID,Ad Group ID,Keyword ID,Ad ID,AMO ID,Error Message

{{$include /help/_includes/bulksheet-headers-note.md}}

-->

## 사용 가능한 데이터 필드

>[!TIP]
>
>다음 테이블은 넓습니다. 보기 영역을 확장하려면 왼쪽 창 상단의 ![왼쪽 창 숨기기](/help/dsp/assets/hide-left-pane.png "왼쪽 창 숨기기") 및 오른쪽 창 상단의 ![오른쪽 창 숨기기](/help/dsp/assets/hide-right-pane.png "오른쪽 창 숨기기")을 클릭하여 목차와 오른쪽 창을 일시적으로 숨길 수 있습니다. 표 하단에 있는 스크롤 막대를 사용하여 전체 내용을 볼 수도 있습니다.

| 필드 | 캠페인 | 광고 그룹 | 키워드 | 텍스트 광고 | 캠페인 위치 타겟 | 설명 |
|----|----|----|----|----|----|----|
| [!UICONTROL Platform] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함) 광고 플랫폼. 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Acct Name] | 필수/선택 사항 | 필수/선택 사항 | 필수/선택 사항 | 필수/선택 사항 | 필수/선택 사항 | 광고 네트워크 계정을 식별하는 고유한 이름. 각 행에 엔터티에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 경우 필요합니다. |
| [!UICONTROL Campaign Name] | 필수 | 필수 | 필수 | 필수 | 필수 | 계정에 대한 캠페인을 식별하는 고유한 이름. |
| [!UICONTROL Campaign Budget] | 필수: 만들기<br><br>선택 사항: 편집 또는 삭제 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 금전적 기호와 구두점을 포함하거나 포함하지 않는 캠페인에 대한 일일 지출 제한. 이 값은 재정의되지만 계정 예산을 초과할 수 없습니다. |
| [!UICONTROL Delivery Method] | 필수: 만들기<br><br>선택 사항: 편집 또는 삭제 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 매일 캠페인에 대한 광고를 표시하는 속도:<ul><li>*[!UICONTROL Standard (Distributed)]*(새 캠페인의 기본값): 광고 노출 횟수를 하루 전체에 분산합니다.</li><li>*[!UICONTROL Accelerated]:* 예산에 도달할 때까지 가능한 한 자주 광고를 표시합니다. 그 결과, 오늘 오후에 광고가 표시되지 않을 수 있습니다.</li></ul> |
| [!UICONTROL Mobile Bid Adjustment] | 선택 사항 | 선택 사항 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 캠페인 수준 또는 광고 그룹 수준에서 모바일 장치의 광고 입찰 여부를 지정합니다.<ul><li>기존 모바일 입찰 조정을 사용하려면 이 항목을 비워 둡니다.</li><li>모바일 장치에서 광고를 입찰하지 않으려면 `-100`을(를) 입력하십시오.</li><li>데스크탑 및 태블릿 장치의 광고와 동일한 입찰가를 사용하여 모바일 장치의 광고에 입찰하려면 `0`을(를) 입력합니다. 새 캠페인의 경우 이 항목을 비워 둘 수도 있습니다.</li><li>다른 입찰을 사용하여 모바일 디바이스에서 광고를 입찰하려면 입찰을 늘리거나 줄일 비율을 입력합니다. 값은 `-90`에서 `300`까지입니다.</li></ul>캠페인 수준에서 장치를 제외하는 경우 광고 그룹 수준에서 제외를 무시할 수 없습니다.<br><br><b>메모:</b><ul><li>광고 그룹은 캠페인 수준 설정을 상속하지만, 이를 재정의할 수 있습니다.</li><li>최적화된 포트폴리오에 캠페인을 할당하면 최적화 기능이 기본 키워드 수준의 입찰가를 자동으로 결정하여 포트폴리오가 목표를 달성할 수 있도록 합니다. 그런 다음 광고 네트워크는 모바일 광고에 대해 지정된 입찰가를 조정합니다.</li><li>캠페인이나 광고 그룹을 최적화된 포트폴리오에 할당하는 경우:<ul><li>최적화 기능은 포트폴리오가 목표를 달성할 수 있도록 기본 키워드 수준의 입찰을 자동으로 결정합니다. 그런 다음 검색 네트워크는 모바일 광고에 대해 지정된 대로 입찰가를 조정합니다.</li><li>포트폴리오가 &quot;[!UICONTROL Auto-optimize Bid Adjustment Values]&quot;(으)로 구성된 경우, 계산되는 이상적인 값이 포트폴리오 설정에 지정된 최소 및 최대 값 내에 있고 광고 그룹에서 모바일 광고에 대한 입찰을 제외하지 않는 한 최적화 기능은 광고 그룹 수준에서 입찰 조정을 변경합니다.</li></ul></li></ul> |
| [!UICONTROL Location] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 선택 사항 | 캠페인을 위한 광고를 배치할 지리적 위치입니다. 도시의 경우 &quot;&lt;<i>City</i>>, &lt;</i>Prefecture</i>>&quot; 형식(예: Adachi, Tokyo)을 사용합니다. 위치를 제외하려면 위치 앞에 빼기 기호(`-`)를 붙입니다. 캠페인에 대한 특정 값을 입력하지 않으면 모든 위치가 타깃팅됩니다. |
| [!UICONTROL Location Type] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수/선택 사항 | (특정 위치를 타깃팅할 때 필수) 지정된 위치가 [!UICONTROL Prefecture] 또는 [!UICONTROL City] 형식인지 여부입니다. |
| [!UICONTROL Ad Group Name] | 해당 사항 없음 | 필수 | 필수 | 필수 | 해당 사항 없음 | 캠페인 내에서 고유한 광고 그룹 이름입니다. 최대 길이는 50자입니다. |
| [!UICONTROL Max CPC] | 해당 사항 없음 | 선택 사항 | 선택 사항 | 해당 사항 없음 | 해당 사항 없음 | CPC(최대 클릭당 비용)로, 금전적 기호와 구두점을 사용하거나 사용하지 않고 검색 네트워크에서 광고 클릭에 대해 지불하는 가장 높은 금액입니다. 광고 그룹 및 키워드에 대한 값을 설정할 수 있습니다. 새 키워드의 기본값은 광고 그룹 수준에서 상속됩니다. |
| [!UICONTROL Keyword] | 선택 사항 / 해당 사항 없음 | 선택 사항 / 해당 사항 없음 | 필수 | 해당 사항 없음 | 해당 사항 없음 | 키워드 문자열입니다. [!DNL Yahoo! Japan]개의 키워드와 일치 유형을 변경할 수 있습니다. 즉, 기존 키워드를 삭제하지 않고 편집할 수 있습니다.<br><br>광고 그룹 또는 캠페인 수준에서 키워드를 제외하려면 [!UICONTROL Match Type]을(를) &quot;음수&quot;로 설정하십시오. 행에 광고 그룹 이름이 포함된 경우 광고 그룹에 대한 키워드는 제외됩니다. 행에 광고 그룹 이름이 포함되지 않으면 전체 캠페인에 대해 키워드가 제외됩니다. |
| [!UICONTROL Match Type] | 선택 사항 / 해당 사항 없음 | 선택 사항 / 해당 사항 없음 | 선택 사항: 만들기<br><br>필수/선택 사항: 편집 또는 삭제 | 해당 사항 없음 | 해당 사항 없음 | 키워드에 대한 키워드 일치 옵션: *[!UICONTROL Broad]*(새 키워드의 기본값), *[!UICONTROL Exact]*, *[!UICONTROL Phrase]*, *[!UICONTROL Negative Broad] 또는 *[!UICONTROL Negative Exact]*. 캠페인 수준 또는 광고 그룹 수준에서 부정적인 키워드를 정의합니다. [!DNL Yahoo! Japan]개의 키워드와 일치 유형을 변경할 수 있습니다. 즉, 기존 키워드를 삭제하지 않고 편집할 수 있습니다.<br><br>일치 유형이 여러 개인 키워드를 편집하려면 일치 유형 또는 키워드 ID 값이 필요합니다. |
| [!UICONTROL First Page Bid] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함) 검색 결과의 첫 페이지에 광고를 배치하는 데 필요한 입찰입니다. 이 값은 광고 네트워크에 게시되지 않습니다. |
| [!UICONTROL Quality Score] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함) 광고 네트워크에서 키워드에 할당한 현재 품질 점수입니다. 이 값은 광고 네트워크에 게시되지 않습니다. |
| [!UICONTROL Ad Name (Yahoo JP)] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 선택 사항: 만들기<br><br>필수/선택 사항: 편집 또는 삭제 | 해당 사항 없음 | 광고 그룹 내에서 광고 이미지를 식별하는 고유한 이름. 최대 길이는 50자입니다. 행에 [!UICONTROL AMO ID] 또는 [!UICONTROL Ad ID]을(를) 사용하지 않는 한 필수입니다. |
| [!UICONTROL Creative Preferred Devices] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 선택 사항 | 해당 사항 없음 | 광고를 표시할 장치 유형: *[!UICONTROL All]*(기본값) 또는 *[!UICONTROL Mobile]*. [!UICONTROL Mobile]의 경우 광고 네트워크에서 데스크톱 또는 태블릿 사용자가 아닌 모바일 장치 사용자에게 광고를 표시하려고 합니다. 그렇지 않으면 모든 장치 유형에 광고가 표시됩니다.<br><br>관리자 및 [!DNL Adobe] 계정 관리자만 이 설정을 편집할 수 있습니다. |
| [!UICONTROL Ad Title] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수 | 해당 사항 없음 | 광고의 헤드라인입니다. 최대 길이는 싱글바이트 30자 또는 더블바이트 15자입니다. 광고 사본을 변경하면 기존 광고가 삭제되고 새 광고가 만들어집니다. |
| [!UICONTROL Ad Title 2] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수 / 해당 사항 없음 | 해당 사항 없음 | (확장 텍스트 광고만 해당) 두 번째 헤드라인입니다. 최대 길이는 30자 또는 15개의 더블바이트 문자입니다. 광고 사본을 변경하면 기존 광고가 삭제되고 새 광고가 만들어집니다. |
| [!UICONTROL Description Line 1] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수 | 해당 사항 없음 | 광고 본문. 확장 텍스트 광고의 경우 최대 길이는 80개의 1바이트 문자 또는 40개의 2바이트 문자입니다. 광고 사본을 변경하면 기존 광고가 삭제되고 새 광고가 만들어집니다. |
| [!UICONTROL Description Line 2] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수 | 해당 사항 없음 | (표준 텍스트 광고만 해당) 광고 본문의 두 번째 줄입니다. 최대 길이는 싱글바이트 38자 또는 더블바이트 19자입니다. 광고 사본을 변경하면 기존 광고가 삭제되고 새 광고가 만들어집니다. <b>참고:</b> [!DNL Yahoo! Japan Ads]에서는 더 이상 표준 텍스트 광고를 만들고 편집할 수 없습니다. |
| [!UICONTROL Creative Type] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 선택 사항 | 해당 사항 없음 | 광고 형식:<ul><li>*[!UICONTROL Text]*(새 광고의 기본값): 컴퓨터, 태블릿 및 스마트폰에 표시될 수 있는 텍스트 광고입니다.</li><li>*[!UICONTROL Mobile]:*&#x200B;은(는) 사용되지 않습니다.</li></ul> |
| [!UICONTROL Display URL] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 필수 / 해당 사항 없음: 만들기<br><br>선택 사항 / 해당 사항 없음: 편집 또는 삭제 | 해당 사항 없음 | (기존 표준 텍스트 광고만, 읽기 전용) 광고에 표시되는 URL입니다. 최대 길이는 255개의 1바이트 문자 또는 127개의 2바이트 문자입니다. 또한 표시 URL과 랜딩 페이지 URL의 도메인은 동일해야 합니다. <b>참고:</b> [!DNL Yahoo! Japan Ads]에서 표준 텍스트 및 확장 텍스트 광고를 더 이상 만들고 편집하지 않습니다. |
| [!UICONTROL Display Path 1], [!UICONTROL Display Path 2] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 선택 사항 / 해당 사항 없음 | 해당 사항 없음 | (확장 텍스트 광고만 해당, 선택 사항) 디스플레이 URL에 추가되고 최종 URL에서 자동으로 추출되는 텍스트입니다. URL 앞에는 슬래시(`/`)가 표시됩니다. 경로에는 슬래시(`/`) 또는 줄바꿈(`\n`) 문자를 사용할 수 없습니다. 최대 길이는 15자 또는 7개의 더블바이트 문자입니다.<br><br>광고 사용자 지정기를 삽입하려면 다음 형식을 사용하십시오. 여기서 `Default text`은(는) 피드 파일에 유효한 값이 없을 때 삽입할 선택적 값입니다.<ul><li>[!DNL Google Ads]: `{CUSTOMIZER.AdCustomizerName:Default text}, such as {CUSTOMIZER.Discount:10%}`</li><li>[!DNL Microsoft Advertising]: `{CUSTOMIZER.Attribute name:Default text}, such as {CUSTOMIZER.Discount:10%}`</li></ul>예를 들어 [!UICONTROL Display Path 1]이(가) &quot;거래&quot;이면 디스플레이 URL은 `&lt;display URL&gt;/deals`이(가) 됩니다(예: www.example.com/deals). |
| [!UICONTROL Base URL/Final URL] | 해당 사항 없음 | 해당 사항 없음 | 선택 사항 | 필수 | 해당 사항 없음 | 최종 사용자가 광고를 클릭할 때 고려할 랜딩 페이지 URL(캠페인이나 계정에 대해 구성된 추가 매개 변수 포함). 키워드 수준의 기본/최종 URL은 광고 수준 이상의 URL을 무시합니다. |
| [!UICONTROL Destination URL] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함됨, 광고 네트워크에 게시되지 않음) 대상 URL이 있는 계정의 경우 이 URL은 광고를 광고주 웹 사이트의 기본 URL/랜딩 페이지에 연결하는 URL입니다(경우에 따라 클릭을 추적한 다음 사용자를 랜딩 페이지로 리디렉션하는 다른 사이트를 통해). 여기에는 Search, Social 및 Commerce 캠페인 또는 계정에 대해 구성된 추가 매개 변수가 포함됩니다. 추적 URL을 생성한 경우, 이는 계정 설정 및 캠페인 설정의 추적 매개 변수를 기반으로 합니다. 광고 네트워크별 매개 변수를 추가한 경우 검색, 소셜 및 Commerce에 대해 동일한 매개 변수로 대체될 수 있습니다.<br><br>최종 URL이 있는 계정의 경우 이 열은 기본 URL/최종 URL 열과 동일한 값을 표시합니다.<br><br>키워드 또는 배치 수준의 대상 URL은 광고 수준의 URL을 재정의합니다. |
| [!UICONTROL Tracking Template] | 선택 사항 | 선택 사항 | 선택 사항 | 선택 사항 | 선택 사항 | (선택 사항) 모든 오프랜딩 도메인 리디렉션 및 추적 매개 변수를 지정하고 또한 최종/랜딩 페이지 URL을 매개 변수에 임베드하는 추적 템플릿 또는 추적 URL. `!{lpurl}` 매개 변수를 사용하여 랜딩 페이지 URL을 지정하십시오. 예: 리디렉션을 포함하는 `{lpurl}?source={network}&id=5` 또는 `http://www.trackingservice.example.com/?url={lpurl}?source={network}&id=5`.<br><br>필요에 따라 서드파티 리디렉션 및 추적을 추가할 수 있습니다.<br><br>캠페인 설정에 &quot;[!UICONTROL EF Redirect]&quot; 및 &quot;[!UICONTROL Auto Upload]&quot;이(가) 포함된 경우 적용되는 Adobe Advertising 전환 추적의 경우 레코드를 저장할 때 Search, Social 및 Commerce에서 자동으로 리디렉션 및 추적 코드 접두사를 추가합니다.<br><br>가장 세분화된 수준의 추적 템플릿은 모든 상위 수준의 값을 재정의합니다. 예를 들어 계정 설정과 키워드 설정 모두에 값이 포함된 경우 키워드 값이 적용됩니다. |
| [!UICONTROL Campaign Status] | 선택 사항: 만들기 또는 편집<br><br>필수: 삭제 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 캠페인의 표시 상태: *[!UICONTROL Active]*(새 캠페인의 기본값), *[!UICONTROL Paused]*, *[!UICONTROL Ended]*(기존 캠페인만) 또는 *[!UICONTROL Deleted]*(기존 캠페인만). |
| [!UICONTROL Ad Group Status] | 해당 사항 없음 | 선택 사항: 만들기 또는 편집<br><br>필수: 삭제 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 광고 그룹의 표시 상태:  *[!UICONTROL Active]*, *[!UICONTROL Paused]* 또는 *[!UICONTROL Deleted]*(기존 광고 그룹만 해당). 새 광고 그룹의 기본값은 [!UICONTROL Active]입니다. 활성 또는 일시 중지된 광고 그룹을 삭제하려면 값 `Deleted`을(를) 입력하십시오. |
| [!UICONTROL Keyword Status] | 해당 사항 없음 | 해당 사항 없음 | 선택 사항: 만들기 또는 편집<br><br>필수: 삭제 | 해당 사항 없음 | 해당 사항 없음 | 키워드의 표시 상태: *[!UICONTROL Active]*, *[!UICONTROL Deleted]*(기존 키워드만), *[!UICONTROL Disapproved]*(편집할 수 없음), *[!UICONTROL Paused]*(기존 키워드만) 또는 *[!UICONTROL Pending]*(편집할 수 없음). 새 키워드의 기본값은 [!UICONTROL Active]입니다. 키워드를 삭제하려면 값 `Deleted`을(를) 입력하십시오. |
| [!UICONTROL Ad Status] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 선택 사항: 만들기 또는 편집<br><br>필수: 삭제 | 해당 사항 없음 | 광고의 표시 상태: *[!UICONTROL Active]*(새 광고의 기본값), *[!UICONTROL Deleted]*(기존 광고만), *[!UICONTROL Disapproved]*(편집할 수 없음), *[!UICONTROL Paused]* 또는 *[!UICONTROL Pending]*(편집할 수 없음). 새 광고의 기본값은 [!UICONTROL Active]입니다. 광고를 삭제하려면 값 `Deleted`을(를) 입력하십시오. |
| [!UICONTROL Location Status] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 선택 사항 | 위치 대상의 상태: *[!UICONTROL Active]* 또는 *[!UICONTROL Deleted]*(기존 위치만 해당). 새 위치의 기본값은 [!UICONTROL Active]입니다. 활성 위치를 삭제하려면 값 `Deleted`을(를) 입력하십시오. |
| \[광고주별 레이블 분류\] | 선택 사항 | 선택 사항 | 선택 사항 | 선택 사항 | 선택 사항 | (Color라는 레이블 분류의 경우 &quot;Color&quot;와 같이 광고주별 레이블 분류에 대해 이름이 지정됨) 엔티티와 연결된 지정된 분류의 값입니다. 엔티티당 분류당 하나의 값만 포함할 수 있습니다(예: 캠페인 A의 &quot;색상&quot; 레이블 분류의 경우 &quot;빨간색&quot;). 최대 길이는 100자이고 값에는 ASCII 및 비 ASCII 문자가 포함될 수 있습니다.<br><br>레이블 분류와 해당 레이블 값이 모든 하위 구성 요소에 적용됩니다. 나중에 추가되는 새 구성 요소는 자동으로 레이블과 연결됩니다. <br><br>분류 이름과 분류 값은 대/소문자를 구분하지 않습니다. |
| [!UICONTROL Constraints] | 선택 사항 | 선택 사항 | 선택 사항 | 선택 사항 | 해당 사항 없음 | 엔티티에 할당된 제약 조건입니다. 엔티티당 하나의 제약조건만 지정할 수 있습니다.<br><br>자식 엔터티에 의해 제약 조건이 상속되므로 상속된 값을 재정의하지 않는 한 자식 엔터티의 값을 입력할 필요가 없습니다. |
| [!UICONTROL Campaign ID] | 해당 사항 없음: 만들기<br><br>필수/선택 사항: 편집 또는 삭제 | 선택 사항 | 선택 사항 | 선택 사항 | 해당 사항 없음 | 기존 캠페인을 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(`'`)가 있어야 합니다.[^1] 행에 캠페인에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않은 경우 캠페인 이름을 변경할 때만 필요합니다. |
| [!UICONTROL Ad Group ID] | 해당 사항 없음 | 해당 사항 없음: 만들기<br><br>필수/선택 사항: 편집 또는 삭제 | 선택 사항 | 선택 사항 | 해당 사항 없음 | 기존 광고 그룹을 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(`'`)가 있어야 합니다.[^1] 행에 광고 그룹에 대한 &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않은 경우 광고 그룹 이름을 변경할 때만 필요합니다. |
| [!UICONTROL Keyword ID] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음: 만들기<br><br>필수/선택 사항: 편집<br><br>필수: 삭제 | 해당 사항 없음 | 해당 사항 없음 | 기존 키워드를 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(`'`)가 있어야 합니다.[^1] 행에 a) 키워드를 식별할 수 있는 속성 열이 충분하거나 b) &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 키워드를 편집하거나 삭제할 때만 필요합니다. |
| [!UICONTROL Ad ID] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음: 만들기<br><br>필수/선택 사항: 편집 또는 삭제 | 해당 사항 없음 | 기존 광고를 식별하는 고유 ID입니다. CSV 및 TSV 파일에서 앞에는 작은 따옴표(`'`)가 있어야 합니다.[^1] 반응형 검색 광고의 경우 광고 데이터를 편집하거나 삭제하려면 [!UICONTROL Ad ID] 또는 [!UICONTROL AMO ID]이(가) 필요합니다. 다른 모든 엔터티 형식의 경우 행에 a) 광고를 식별할 수 있는 충분한 광고 속성 열 또는 b) &quot;[!UICONTROL AMO ID]&quot;이(가) 포함되지 않는 한 광고 상태를 변경할 때만 [!UICONTROL AMO ID]이(가) 필요합니다. 그러나 [!UICONTROL Ad ID]과(와) [!UICONTROL AMO ID]을(를) 모두 포함하지 않고 광고 속성 열이 여러 광고와 일치하는 경우 광고 중 하나에 대한 상태만 변경됩니다.<br><br><b>참고:</b> a) 기존 광고에 대한 [!UICONTROL Status]을(를) 제외한 광고 속성 열 또는 b) 응답형 검색 광고에 대한 데이터를 편집하고 [!UICONTROL Ad ID]과(와) [!UICONTROL AMO ID]을(를) 포함하지 않으면 새 광고가 만들어지고 기존 광고가 변경되지 않습니다. |
| [!UICONTROL AMO ID] | 해당 없음: 만들기<br><br>선택 사항: 편집 또는 삭제 | 해당 없음: 만들기<br><br>선택 사항: 편집 또는 삭제 | 해당 없음: 만들기<br><br>선택 사항: 편집 또는 삭제 | 해당 없음: 만들기<br><br>선택 사항: 편집 또는 삭제 | 해당 사항 없음 | (생성된 일괄 시트에서) 동기화된 엔터티에 대해 [!DNL Adobe]이(가) 생성한 고유 식별자입니다. 반응형 검색 광고의 경우 [!UICONTROL Ad ID]을(를) 포함하지 않으면 [!UICONTROL AMO ID]에서 광고를 편집하거나 삭제해야 합니다. [!UICONTROL AMO ID]이(가) 있는 다른 모든 엔터티 형식의 데이터를 편집하려면 엔터티 ID와 상위 엔터티 ID를 포함하지 않으면 [!UICONTROL AMO ID]에서 데이터를 편집하거나 삭제해야 합니다.<br><br>검색, 소셜 및 Commerce에서는 값을 사용하여 편집할 올바른 ID를 결정하지만 ID를 광고 네트워크에 게시하지 않습니다. |
| [!UICONTROL EF Error Message] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함됨) 검색, 소셜 및 Commerce에서 행의 데이터에 대한 오류 메시지를 표시하는 자리 표시자입니다. 오류 메시지는 [!UICONTROL EF Errors]개 파일에 포함됩니다. 이 값은 광고 네트워크에 게시되지 않습니다. |
| [!UICONTROL SE Error Message] | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | 해당 사항 없음 | (정보 목적으로 생성된 일괄 시트에 포함됨) 행의 데이터에 대한 광고 네트워크의 오류 메시지를 표시하는 자리 표시자입니다. 오류 메시지는 [!UICONTROL SE Errors] 파일에 포함됩니다. 이 값은 광고 네트워크에 게시되지 않습니다. |

[^1]: Excel은 파일을 열 때 큰 숫자를 과학적 표기법(예: 2115585666의 경우 2.12E+09)으로 변환합니다. 표준 표기법에서 숫자를 보려면 열에서 셀을 선택하고 수식 입력줄 내부를 클릭합니다.

>[!MORELIKETHIS]
>
>* [부록 - 일괄 시트 오류](../bulksheet-errors.md)
>* [일괄 시트에서 수행할 수 있는 작업](bulksheet-operations.md)
>* [지원되는 일괄 시트 파일 형식](bulksheet-file-formats.md)
>* [일괄 시트 파일 다운로드/만들기](../bulksheet-download.md)
>*  [!DNL Naver][&#128279;](/help/search-social-commerce/tracking/formats-click-tracking-naver.md)에 대한 클릭 추적 형식
>* [일괄 시트 파일 또는 수정된 오류 파일 업로드](../bulksheet-upload.md)
