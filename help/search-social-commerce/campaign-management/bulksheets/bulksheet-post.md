---
title: 게시물 일괄 시트 또는 수정된 오류 파일
description: 일괄 시트 파일을 광고 네트워크에 게시하는 방법을 알아봅니다.
exl-id: 49b930ba-71b3-442d-a162-67cf7ae14e14
feature: Search Bulksheets
source-git-commit: d0f1c413134a0868ddec79ded7672af316267edd
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 0%

---

# 게시물 일괄 시트 또는 수정된 오류 파일

기존 일괄 시트 파일 또는 수정된 오류 파일을 [지원되는 광고 네트워크](bulksheet-about.md#bulksheet-functionality-by-network)의 관련 계정에 게시할 수 있습니다. 파일이 ZIP 형식인 경우 먼저 압축을 풀 필요가 없습니다.

일괄 시트 파일 및 오류 파일은 업로드되거나 생성된 후 30일이 지나면 자동으로 삭제됩니다.

>[!NOTE]
>파일을 업로드할 때 일괄 시트 파일 또는 오류 파일을 게시할 수도 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Search, Social, & Commerce]> [!UICONTROL Campaigns] >[!UICONTROL Bulksheets]**&#x200B;을(를) 클릭합니다.

1. 게시할 각 파일 옆에 있는 확인란을 선택합니다.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL Post]**&#x200B;을(를) 클릭합니다.

1. 대화 상자에서 [[!UICONTROL Post Bulksheet] 설정](#bulksheet-post-settings)에 정보를 입력하거나 선택한 다음 **[!UICONTROL Post]**&#x200B;을(를) 클릭합니다.

   게시하는 모든 파일에 동일한 설정이 적용됩니다.

작업이 시작되면 [!UICONTROL Bulksheets] 보기에서 행의 상태 및 예약된 게시 날짜가 변경됩니다. 파일이 게시되면 파일에 대한 링크가 포함된 이메일 알림이 전송됩니다. 컴파일된 데이터의 양에 따라 이메일 알림은 몇 분 이상 걸릴 수 있습니다. 그러나 데이터를 게시할 수 없는 경우 오류 파일이 [!UICONTROL Bulksheets] 보기에 나열되며 오류 파일에 대한 링크와 함께 전자 메일 알림이 전송됩니다.

>[!NOTE]
>
>* 많은 양의 데이터를 게시하는 데 시간이 더 오래 걸립니다. [!UICONTROL Bulksheets] 보기의 [!UICONTROL Progress] 열에 있는 파일의 진행 상황을 따를 수 있습니다.
>* 게시된 모든 데이터는 네트워크의 편집 절차에 따릅니다.
* 일괄 시트 파일이 게시되기 전에 게시를 취소할 수 있습니다.

## 일괄 시트 및 수정된 오류 파일에 대한 사후 설정 {#bulksheet-post-settings}

| 매개 변수 | 설명 |
|----|----|
| [!UICONTROL Account (Search Engine)] | 데이터가 게시되는 광고 네트워크 계정입니다. 여러 개의 파일을 동시에 게시하거나 여러 계정에 적용되는 하나의 파일을 게시하는 경우 값은 <i>선택한 여러 계정</i>입니다.<br><br>광고 네트워크 이름의 첫 글자가 계정 이름 뒤에 괄호로 묶여 있습니다([!DNL Google Ads] 계정의 경우 &quot;Acme Realty(G)&quot;). |
| [!UICONTROL Scheduling] | 파일을 지정된 광고 네트워크에 게시하는 시기:<ul><li><i>[!UICONTROL Post to ad network now]</i>(기본값): 데이터 게시를 즉시 시작합니다.</li><li><i>[!UICONTROL Post to ad network on \[specified date\] \[specified time\]]:</i> 지정한 날짜와 시간에 데이터 게시를 시작합니다. 기본값은 내일 02:00(오전 2시)입니다. 날짜를 변경하려면 DD/MM/YYYY 또는 D/M/YYYY 형식으로 날짜를 입력하거나 ![달력](/help/search-social-commerce/assets/calendar.png "달력")을 클릭하여 달력을 열고 [날짜를 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/calendar.md)합니다. 시간을 변경하려면 시간을 HH/MM 또는 H/M 형식으로 입력하거나 목록에서 시간(15분 간격)을 선택합니다.</li></ul> |
| [!UICONTROL Generate Tracking URLs] | 게시에 있는 모든 키워드, 광고, 배치, 사이트링크 및 [!DNL Google Ads] 제품 그룹(<i>[!UICONTROL Yes]</i>(기본값) 또는 <i>[!UICONTROL No]</i>)에 대해 추적 템플릿이 있는 계정의 추적 템플릿 및 랜딩 페이지 접미사(적용 가능한 광고 네트워크의 경우)나 대상 URL이 있는 계정에 추적 코드가 포함된 대상 URL을 포함할지 여부입니다. 입찰 단위가 포트폴리오에 포함되어 있는지는 중요하지 않습니다.<br><br><i>[!UICONTROL Yes]</i>을(를) 선택하면 관련 계정 설정 또는 캠페인 설정의 [!UICONTROL Tracking Methods] 섹션에 있는 매개 변수에 따라 URL이 생성됩니다. 기본적으로 추적 URL이 있으면 새 URL이 필요하지 않으면 다시 생성되지 않습니다(예: 키워드 일치 유형, 광고 텍스트 또는 관련 계정에 대한 추적 매개 변수가 변경된 경우).<br><br><i>[!UICONTROL No]</i>을(를) 선택하면 나중에 업로드된 파일을 수동으로 게시하여 추적 URL을 생성할 수 있습니다.<br><br><b>참고:</b> 광고주가 Adobe Advertising 전환 추적을 사용하고 기본 URL이 변경된 경우, 계정이 자동으로 추적 URL을 생성하고 업로드하도록 구성되지 않은 한 새 추적 URL을 생성해야 합니다. |
| [!UICONTROL Enable budget changes on optimized campaigns] | 게시된 데이터를 기반으로 최적화된 포트폴리오에서 캠페인에 대한 예산 변경을 허용합니다. 기본적으로 이 옵션은 선택되어 있지 않습니다. 이 옵션을 선택하면 최적화 기능이 예산을 재할당해야 한다고 결정할 때까지(보통 다음 입찰 주기에서) 지정된 캠페인 예산 변경을 적용할 수 있습니다.<br><br><b>참고:</b> 최적화되지 않은 포트폴리오의 캠페인에 대해 게시된 데이터로 인한 예산 변경은 파일을 게시할 때 발생합니다. 변경 사항은 다음 날 캠페인 관리 보기에 표시됩니다. |
| [!UICONTROL Enable bidding on ads within portfolios] | 포함된 캠페인 구성 요소가 최적화된 포트폴리오에 있는 경우 이 기능은 최적화 전략을 재정의하고 지정된 종료 날짜까지 일괄 시트의 데이터를 기반으로 입찰 변경을 허용합니다. 이 옵션을 선택하는 경우 **[!UICONTROL Hold bulksheet bids until]** 필드에 1~7일 사이에 종료 날짜를 지정하십시오. |

>[!MORELIKETHIS]
>
>* [일괄 시트를 사용하여 캠페인 데이터 관리 정보](bulksheet-about.md)
>* [일괄 시트 파일 다운로드/만들기](bulksheet-download.md)
>* [일괄 시트 또는 수정된 오류 파일 업로드](bulksheet-upload.md)
>* [일괄 시트 파일의 랜딩 페이지 유효성 검사](bulksheet-validate-landing-pages.md)
>* [생성되거나 업로드된 일괄 시트 파일 내보내기](bulksheet-export.md)
