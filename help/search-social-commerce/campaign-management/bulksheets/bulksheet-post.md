---
title: 게시물 일괄 시트 또는 수정된 오류 파일
description: 일괄 시트 파일을 광고 네트워크에 게시하는 방법을 알아봅니다.
exl-id: 49b930ba-71b3-442d-a162-67cf7ae14e14
feature: Search Bulksheets
source-git-commit: f68b2eb267391972eed94e4fec3ea386fbf206c6
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 0%

---

# 게시물 일괄 시트 또는 수정된 오류 파일

기존 일괄 시트 파일 또는 수정된 오류 파일을 다음에 대한 관련 계정에 게시할 수 있습니다 [지원되는 광고 네트워크](bulksheet-about.md#bulksheet-functionality-by-network). 파일이 ZIP 형식인 경우 먼저 압축을 풀 필요가 없습니다.

일괄 시트 파일 및 오류 파일은 업로드되거나 생성된 후 30일이 지나면 자동으로 삭제됩니다.

>[!NOTE]
>파일을 업로드할 때 일괄 시트 파일 또는 오류 파일을 게시할 수도 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Bulksheets]**.

1. 게시할 각 파일 옆에 있는 확인란을 선택합니다.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL Post]**.

1. 대화 상자에서 [[!UICONTROL Post Bulksheet] 설정](#bulksheet-post-settings)을 클릭한 다음 을 클릭합니다 **[!UICONTROL Post]**.

   게시하는 모든 파일에 동일한 설정이 적용됩니다.

작업이 시작되면 행의 상태 및 예약된 게시 날짜가 [!UICONTROL Bulksheets] 보기. 파일이 게시되면 파일에 대한 링크가 포함된 이메일 알림이 전송됩니다. 컴파일된 데이터의 양에 따라 이메일 알림은 몇 분 이상 걸릴 수 있습니다. 그러나 데이터를 게시할 수 없는 경우 오류 파일이 [!UICONTROL Bulksheets] 을 확인하면 오류 파일에 대한 링크와 함께 이메일 알림이 전송됩니다.

>[!NOTE]
>
>* 많은 양의 데이터를 게시하는 데 시간이 더 오래 걸립니다. 에서 파일의 진행 상황을 따를 수 있습니다. [!UICONTROL Progress] 열의 [!UICONTROL Bulksheets] 보기.
>* 게시된 모든 데이터는 네트워크의 편집 절차에 따릅니다.
* 일괄 시트 파일이 게시되기 전에 게시를 취소할 수 있습니다.

## 일괄 시트 및 수정된 오류 파일에 대한 사후 설정 {#bulksheet-post-settings}

| 매개 변수 | 설명 |
|----|----|
| [!UICONTROL Account (Search Engine)] | 데이터가 게시되는 광고 네트워크 계정입니다. 여러 파일을 동시에 게시하거나 여러 계정에 적용되는 한 파일을 게시하는 경우 값은 다음과 같습니다. <i>여러 계정이 선택됨</i>.<br><br>광고 네트워크 이름의 첫 번째 문자는 계정 이름 뒤에 괄호 안에 있습니다(예: &quot;Acme Realty (G)&quot;). [!DNL Google Ads] 계정). |
| [!UICONTROL Scheduling] | 파일을 지정된 광고 네트워크에 게시하는 시기:<ul><li><i>[!UICONTROL Post to ad network now]</i> (기본값): 데이터 게시를 즉시 시작합니다.</li><li><i>[!UICONTROL Post to ad network on \[specified date\] \[specified time\]]:</i> 지정된 날짜와 시간에 데이터 게시를 시작합니다. 기본값은 내일 02:00(오전 2시)입니다. 날짜를 변경하려면 DD/MM/YYYY 또는 D/M/YYYY 형식으로 날짜를 입력하거나 ![캘린더](assets/calendar.png "캘린더") 캘린더를 열고 [날짜 선택](/advertising.en/help/search-social-commerce/campaign-management/bulksheets/assets/calendar.png). 시간을 변경하려면 시간을 HH/MM 또는 H/M 형식으로 입력하거나 목록에서 시간(15분 간격)을 선택합니다.</li></ul> |
| [!UICONTROL Generate Tracking URLs] | 모든 키워드, 광고, 배치, 사이트링크 및 추적에 대해 추적 템플릿이 있는 계정의 추적 템플릿 및 랜딩 페이지 접미사(적용 가능한 광고 네트워크의 경우)나 대상 URL이 있는 계정에 추적 코드가 포함된 대상 URL을 포함할지 여부 [!DNL Google Ads] 게시의 제품 그룹: <i>[!UICONTROL Yes]</i> (기본값) 또는 <i>[!UICONTROL No]</i>. 입찰 단위가 포트폴리오에 포함되어 있는지는 중요하지 않습니다.<br><br>다음을 선택하는 경우 <i>[!UICONTROL Yes]</i>를 입력하면 의 매개 변수에 따라 URL이 생성됩니다. [!UICONTROL Tracking Methods] 섹션(관련 계정 설정 또는 캠페인 설정). 기본적으로 추적 URL이 있으면 새 URL이 필요하지 않으면 다시 생성되지 않습니다(예: 키워드 일치 유형, 광고 텍스트 또는 관련 계정에 대한 추적 매개 변수가 변경된 경우).<br><br>다음을 선택하는 경우 <i>[!UICONTROL No]</i>그런 다음 업로드된 파일을 수동으로 게시하여 나중에 추적 URL을 생성할 수 있습니다.<br><br><b>참고:</b> 광고주가 Adobe Advertising 전환 추적을 사용하고 기본 URL이 변경된 경우, 계정이 추적 URL을 자동으로 생성하고 업로드하도록 구성되지 않은 경우, 새 추적 URL을 생성해야 합니다. |
| [!UICONTROL Enable budget changes on optimized campaigns] | 게시된 데이터를 기반으로 최적화된 포트폴리오에서 캠페인에 대한 예산 변경을 허용합니다. 기본적으로 이 옵션은 선택되어 있지 않습니다. 이 옵션을 선택하면 최적화 기능이 예산을 재할당해야 한다고 결정할 때까지(보통 다음 입찰 주기에서) 지정된 캠페인 예산 변경을 적용할 수 있습니다.<br><br><b>참고:</b> 최적화되지 않은 포트폴리오의 캠페인에 대해 게시된 데이터로 인한 예산 변경은 파일을 게시할 때 발생합니다. 변경 사항은 다음 날 캠페인 관리 보기에 표시됩니다. |
| [!UICONTROL Enable bidding on ads within portfolios] | 포함된 캠페인 구성 요소가 최적화된 포트폴리오에 있는 경우 이 기능은 최적화 전략을 재정의하고 지정된 종료 날짜까지 일괄 시트의 데이터를 기반으로 입찰 변경을 허용합니다. 이 옵션을 선택하는 경우 종료 날짜를 1-7일 후로 지정합니다. **[!UICONTROL Hold bulksheet bids until]** 필드. |

>[!MORELIKETHIS]
>
>* [일괄 시트를 사용하여 캠페인 데이터 관리 기본 정보](bulksheet-about.md)
>* [일괄 시트 파일 다운로드/만들기](bulksheet-download.md)
>* [일괄 시트 또는 수정된 오류 파일 업로드](bulksheet-upload.md)
>* [일괄 시트 파일의 랜딩 페이지 유효성 검사](bulksheet-validate-landing-pages.md)
>* [생성 또는 업로드한 일괄 시트 파일 내보내기](bulksheet-export.md)
