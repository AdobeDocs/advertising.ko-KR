---
title: 스프레드시트 보고서 피드용  [!DNL Excel] 템플릿 만들기
description: 특수 형식의 스프레드시트 템플릿을 만드는 방법에 대해 알아봅니다.
exl-id: 74bf3cdf-7d56-431a-8aff-11ed3840a7cd
feature: Search Reports
source-git-commit: 67fe8581832dc0762d62908d01672e53cc95b847
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# 스프레드시트 보고서 피드용 [!DNL Excel] 템플릿 만들기

*기본 보고서 및 모델 정확도 보고서에만 해당*

스프레드시트 피드를 만들려면 먼저 일반 보고서 템플릿을 사용하여 특수 형식의 [!DNL Microsoft Excel] 스프레드시트 템플릿을 만들어야 합니다. 선택적으로 추가 열 및 그래프를 포함하도록 [!DNL Excel] 스프레드시트를 사용자 지정할 수 있습니다.

1. **[!UICONTROL Search]> [!UICONTROL Insights & Reports] >[!UICONTROL Reports]**&#x200B;에서 &quot;[!UICONTROL Daily]&quot;의 [!UICONTROL Date Aggregation] 단위와 원하는 다른 모든 데이터 매개 변수를 사용하여 원하는 보고서 유형을 생성하고 보고서를 템플릿으로 저장합니다.

   >[!NOTE]
   >
   > * [!UICONTROL Portfolio], [!UICONTROL Search Engine], [!UICONTROL Search Engine Account], [!UICONTROL Campaign], [!UICONTROL Ad Group], [!UICONTROL Ad Variation], [!UICONTROL Keyword] 및 [!UICONTROL Forecast Accuracy] 보고서에 대한 스프레드시트 피드를 만들 수 있습니다. [!UICONTROL Ad Group Report]을(를) 사용하는 경우 더 빠른 결과를 위해 포함된 광고 그룹의 수를 제한하십시오.
   > * 템플릿에 정의된 [!UICONTROL Date Range] 단위가 사용되지 않습니다. 나중에 스프레드시트 피드를 구성할 때 데이터를 새로 고칠 날짜를 정의합니다.

1. 보고서가 생성되면 **[!UICONTROL Search]> [!UICONTROL Insights & Reports] >[!UICONTROL Reports]**(으)로 이동하여 보고서 출력의 TSV 또는 XLS 버전을 파일로 내보냅니다.

1. [!DNL Excel]에서 보고서에 대한 사용자 지정 템플릿을 만듭니다.

   1. [!DNL Excel]에서 보고서 파일을 엽니다.

   1. 통합 문서 준비:

      1. 보고서 매개 변수를 표시하는 상위 행을 삭제합니다. XLS 파일의 경우 &quot;[!UICONTROL Total]&quot; 행도 삭제합니다. 선택적으로 일부 데이터 행을 삭제할 수 있지만 a) 원래 순서의 모든 열이 있는 데이터 헤더 행과 b) 하나 이상의 데이터 행을 유지합니다. 수동으로 데이터를 추가하지 마십시오.

         >[!NOTE]
         >
         > 마지막 열에는 0이 아닌 값이 포함되어야 합니다.

      2. 시작 날짜별로 데이터를 오름차순으로 정렬합니다(가장 오래된 항목부터 가장 최근 항목까지).

      3. 워크시트 탭 이름을 &quot;[!UICONTROL Sheet1]&quot;에서 &quot;[!UICONTROL RAW]&quot;(으)로 변경합니다.&quot;

         이 특정 탭 이름을 사용하면 데이터를 새로 고칠 수 있습니다.

      4. (선택 사항) 필요한 경우 보고서 템플릿의 열 오른쪽에 사용자 정의 열을 추가합니다.

   1. (선택 사항) 별도의 워크시트에서 피벗 테이블을 만듭니다. 작업이 완료되면 피벗 테이블의 셀을 마우스 오른쪽 단추로 클릭하고 **[!UICONTROL Pivot Table Options]**&#x200B;을(를) 선택하고 **[!UICONTROL Data]** 탭을 클릭한 다음 **[!UICONTROL Refresh data when opening the file]**&#x200B;을(를) 선택합니다.

   1. 파일을 .XLSX 형식의 [!DNL Excel] 스프레드시트로 저장합니다.

>[!MORELIKETHIS]
>
>* [스프레드시트 보고서 피드 정보](spreadsheet-feed-about.md)
>* [스프레드시트 보고서 피드 만들기](spreadsheet-feed-create.md)
>* [스프레드시트 보고서 피드 설정 편집](spreadsheet-feed-edit.md)
>* [스프레드시트 보고서 피드 설정](spreadsheet-feed-settings.md)
>* [스프레드시트 보고서 피드 파일 보기 또는 저장](spreadsheet-feed-view-or-save.md)
>* [스프레드시트 보고서 피드 수동으로 새로 고침](spreadsheet-feed-refresh.md)
>* [스프레드시트 보고서 피드 삭제](spreadsheet-feed-delete.md)
