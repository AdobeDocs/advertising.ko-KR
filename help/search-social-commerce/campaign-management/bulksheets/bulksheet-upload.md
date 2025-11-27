---
title: 일괄 시트 또는 수정된 오류 파일 업로드
description: 일괄 시트 파일 또는 수정된 랜딩 페이지 유효성 검사 오류 파일을 수동으로 업로드하는 방법을 알아봅니다.
exl-id: 44c76ca3-1d3e-43c2-868a-4868157d32b0
feature: Search Bulksheets
source-git-commit: 3ab2e38f6a2f70c03504363575b13dc0dc730282
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# 일괄 시트 또는 수정된 오류 파일 업로드

[지원되는 광고 네트워크](bulksheet-about.md#bulksheet-functionality-by-network)에 대해 장치 또는 네트워크에서 일괄 시트 파일, 수정된 랜딩 페이지 유효성 검사 오류 파일 및 기타 수정된 오류 파일을 업로드할 수 있습니다. 파일을 업로드할 때 파일의 모든 사용자 정의 열이 삭제됩니다.

1. 메인 메뉴에서 **[!UICONTROL Search, Social, & Commerce]> [!UICONTROL Campaigns] >[!UICONTROL Bulksheets]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL Upload Bulksheet]**&#x200B;을(를) 클릭합니다.

1. [[!UICONTROL Upload Bulksheet] 설정](#bulksheet-upload-settings)에서 정보를 입력하거나 선택하십시오.

1. **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

작업이 시작되면 파일이 [!UICONTROL Bulksheets] 보기에 나열됩니다. 파일이 완료되면 파일에 대한 링크가 포함된 이메일 알림이 전송됩니다. 컴파일된 데이터의 양에 따라 이메일 알림은 몇 분 이상 걸릴 수 있습니다. 그러나 파일 생성이 실패하면 오류 파일이 [!UICONTROL Bulksheets] 보기에 나열되고 오류 파일에 대한 링크와 함께 전자 메일 알림이 전송됩니다.

>[!NOTE]
>
>일괄 시트 데이터를 광고 네트워크에 게시하는 경우 [!UICONTROL Progress] 보기의 [!UICONTROL Bulksheets] 열에 있는 파일의 진행 상황을 따를 수 있습니다. 많은 양의 데이터를 게시하는 데 시간이 더 오래 걸립니다.

## 일괄 시트 및 수정된 오류 파일에 대한 업로드 설정 {#bulksheet-upload-settings}

| 매개 변수 | 설명 |
|----|----|
| [!UICONTROL File to Upload] | 업로드할 파일입니다. 전체 경로와 파일 이름을 입력하거나 <b>[!UICONTROL Browse]</b>을(를) 클릭하여 장치 또는 네트워크에서 파일을 찾아 파일을 지정하십시오.<br><br>일괄 시트 파일은 최대 2.5GB(약 250만 행)일 수 있으며 <i>[!UICONTROL .tsv]</i>(탭으로 구분된 값의 경우), <i>[!UICONTROL .txt]</i>(유니코드 호환 ASCII 텍스트의 경우), <i>[!UICONTROL .csv]</i>(쉼표로 구분된 값의 경우) 또는 <i>[!UICONTROL .zip]</i>(TSV 파일로 압축 해제하는 압축 ZIP 형식의 경우) 파일 확장명 중 하나를 포함해야 합니다. 파일 이름에는 다음 문자를 포함할 수 없습니다. `# % &amp; * \| \ : " < > . ? /`<br><br><b>팁:</b> 국제 문자가 포함된 데이터의 경우 TSV 또는 TXT 형식의 파일을 사용하십시오. |
| [!UICONTROL Single Account] | 파일이 하나의 계정에 적용되는지 여부: <i>[!UICONTROL Yes]</i>(하나의 계정에 대해) 또는 <i>[!UICONTROL No]</i>(여러 계정에 대해). |
| [!UICONTROL Account (Search Engine)] | (파일이 단일 계정에 적용되는 경우) 데이터를 업로드할 계정입니다. |
| [!UICONTROL Search Engine] | (파일이 여러 계정에 적용되는 경우) 데이터를 업로드할 광고 네트워크입니다. |
| [!UICONTROL Scheduling] | 파일을 지정된 광고 네트워크에 게시할 시기 또는 여부:<ul><li><i>[!UICONTROL Post to ad network now]</i>(기본값): 데이터 게시를 즉시 시작합니다.</li><li><i>[!UICONTROL Post to ad network on \[specified date\] \[specified time\]]:</i> 지정한 날짜와 시간에 데이터 게시를 시작합니다. 기본값은 내일 02:00(오전 2시)입니다. 날짜를 변경하려면 DD/MM/YYYY 또는 D/M/YYYY 형식으로 날짜를 입력하거나 ![달력](/help/search-social-commerce/assets/calendar.png "달력")을 클릭하여 달력을 열고 [날짜를 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/calendar.md)합니다. 시간을 변경하려면 시간을 HH/MM 또는 H/M 형식으로 입력하거나 목록에서 시간(15분 간격)을 선택합니다.</li><li><i>[!UICONTROL Preview only]:</i> 데이터를 광고 네트워크에 게시하지 않고 Search, Social, Commerce에 파일을 업로드하려면 파일을 나중에 게시할 수 있습니다. 일괄 시트 파일이 10MB보다 크지만 2GB보다 작은 경우 파일이 ZIP 형식이므로 게시하기 위해 파일의 압축을 풀 필요가 없습니다.</li></ul> |
| [!UICONTROL Generate Tracking URLs] | 게시에 있는 모든 키워드, 광고, 배치, 사이트링크 및 [!DNL Google Ads] 제품 그룹(<i>[!UICONTROL Yes]</i>(기본값) 또는 <i>[!UICONTROL No]</i>)에 대해 추적 템플릿이 있는 계정의 추적 템플릿 및 랜딩 페이지 접미사(적용 가능한 광고 네트워크의 경우)나 대상 URL이 있는 계정에 추적 코드가 포함된 대상 URL을 포함할지 여부입니다. 입찰 단위가 포트폴리오에 포함되어 있는지는 중요하지 않습니다.<br><br><i>[!UICONTROL Yes]</i>을(를) 선택하면 관련 계정 설정 또는 캠페인 설정의 [!UICONTROL Tracking Methods] 섹션에 있는 매개 변수에 따라 URL이 생성됩니다. 기본적으로 추적 URL이 있으면 새 URL이 필요하지 않으면 다시 생성되지 않습니다(예: 키워드 일치 유형, 광고 텍스트 또는 관련 계정에 대한 추적 매개 변수가 변경된 경우).<br><br><i>[!UICONTROL No]</i>을(를) 선택하면 나중에 업로드된 파일을 수동으로 게시하여 추적 URL을 생성할 수 있습니다.<br><br><b>참고:</b> 광고주가 Adobe Advertising 전환 추적을 사용하고 기본 URL이 변경된 경우, 계정이 자동으로 추적 URL을 생성하고 업로드하도록 구성되지 않은 한 새 추적 URL을 생성해야 합니다. |
| [!UICONTROL Enable budget changes on optimized campaigns] | 게시된 데이터를 기반으로 최적화된 포트폴리오에서 캠페인에 대한 예산 변경을 허용합니다. 기본적으로 이 옵션은 선택되어 있지 않습니다. 이 옵션을 선택하면 최적화 기능이 예산을 재할당해야 한다고 결정할 때까지(보통 다음 입찰 주기에서) 지정된 캠페인 예산 변경을 적용할 수 있습니다.<br><br><b>참고:</b> 최적화되지 않은 포트폴리오의 캠페인에 대해 게시된 데이터로 인한 예산 변경은 파일을 게시할 때 발생합니다. 변경 사항은 다음 날 캠페인 관리 보기에 표시됩니다. |
| [!UICONTROL Enable bidding on ads within portfolios] | 포함된 캠페인 구성 요소가 최적화된 포트폴리오에 있는 경우 이 기능은 최적화 전략을 재정의하고 지정된 종료 날짜까지 일괄 시트의 데이터를 기반으로 입찰 변경을 허용합니다. 이 옵션을 선택하는 경우 **[!UICONTROL Hold bulksheet bids until]** 필드에 1~7일 사이에 종료 날짜를 지정하십시오. |

>[!MORELIKETHIS]
>
>* [일괄 시트를 사용하여 캠페인 데이터 관리 정보](bulksheet-about.md)
>* [일괄 시트 파일 다운로드/만들기](bulksheet-download.md)
>* [일괄 시트 또는 수정된 오류 파일 게시](bulksheet-post.md)
>* [일괄 시트 파일의 랜딩 페이지 유효성 검사](bulksheet-validate-landing-pages.md)
>* [생성되거나 업로드된 일괄 시트 파일 내보내기](bulksheet-export.md)
