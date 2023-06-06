---
title: 만들기 [!DNL Excel] 스프레드시트 보고서 피드용 템플릿
description: 특수 형식의 스프레드시트 템플릿을 만드는 방법에 대해 알아봅니다.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# 만들기 [!DNL Excel] 스프레드시트 보고서 피드용 템플릿

*기본 보고서 및 모델 정확도 보고서의 경우에만*

스프레드시트 피드를 생성하려면 먼저 특별 포맷된 피드를 생성해야 합니다 [!DNL Microsoft® Excel] 일반 보고서 템플릿을 사용하는 스프레드시트 템플릿입니다. 선택적으로 다음을 사용자 지정할 수 있습니다. [!DNL Excel] 추가 열 및 그래프를 포함하는 스프레드시트입니다.

1. 위치 **[!UICONTROL Search]> [!UICONTROL Insights & Reports] >[!UICONTROL Reports]**, 를 사용하여 원하는 보고서 유형 생성 [!UICONTROL Date Aggregation] 의 단위[!UICONTROL Daily]&quot;원하는 다른 모든 데이터 매개 변수와 함께 보고서를 템플릿으로 저장합니다.

   >[!NOTE]
   >
   > * 다음에 대한 스프레드시트 피드를 생성할 수 있습니다. [!UICONTROL Portfolio], [!UICONTROL Search Engine], [!UICONTROL Search Engine Account], [!UICONTROL Campaign], [!UICONTROL Ad Group], [!UICONTROL Ad Variation], [!UICONTROL Keyword], 및 [!UICONTROL Forecast Accuracy] 보고서. 를 사용하는 경우 [!UICONTROL Ad Group Report]를 사용하면 더 빠른 결과를 위해 포함된 광고 그룹의 수를 제한할 수 있습니다.
   > * 다음 [!UICONTROL Date Range] 템플릿에 정의된 단위가 사용되지 않습니다. 나중에 스프레드시트 피드를 구성할 때 데이터를 새로 고칠 날짜를 정의합니다.


1. 보고서가 생성되면 다음 위치로 이동합니다. **[!UICONTROL Search]> [!UICONTROL Insights & Reports] >[!UICONTROL Reports]** 및 보고서 출력의 TSV 또는 XLS 버전을 파일로 내보냅니다.

1. 위치 [!DNL Excel], 보고서에 대한 사용자 지정 템플릿을 만듭니다.

   1. 에서 보고서 파일 열기 [!DNL Excel].

   1. 통합 문서 준비:

      1. 보고서 매개 변수를 표시하는 상위 행을 삭제합니다. XLS 파일의 경우 &quot;[!UICONTROL Total]&quot;행. 선택적으로 일부 데이터 행을 삭제할 수 있지만 a) 원래 순서의 모든 열이 있는 데이터 헤더 행과 b) 하나 이상의 데이터 행을 유지합니다. 수동으로 데이터를 추가하지 마십시오.

         >[!NOTE]
         >
         > 마지막 열에는 0이 아닌 값이 포함되어야 합니다.

      2. 시작 날짜별로 데이터를 오름차순으로 정렬합니다(가장 오래된 항목부터 가장 최근 항목까지).

      3. 워크시트 탭 이름을 &quot;에서 변경합니다.[!UICONTROL Sheet1]&quot; - &quot;[!UICONTROL RAW].&quot;

         이 특정 탭 이름을 사용하면 데이터를 새로 고칠 수 있습니다.

      4. (선택 사항) 필요한 경우 보고서 템플릿의 열 오른쪽에 사용자 정의 열을 추가합니다.
   1. (선택 사항) 별도의 워크시트에서 피벗 테이블을 만듭니다. 작업이 완료되면 피벗 테이블의 셀을 마우스 오른쪽 단추로 클릭하고 를 선택합니다 **[!UICONTROL Pivot Table Options]**&#x200B;를 클릭하고 **[!UICONTROL Data]** 탭을 선택한 다음 **[!UICONTROL Refresh data when opening the file]**.

   1. 파일을 다른 이름으로 저장 [!DNL Excel] .XLSX 형식의 스프레드시트입니다.


>[!MORELIKETHIS]
>
>* [스프레드시트 보고서 피드 정보](spreadsheet-feed-about.md)
>* [스프레드시트 보고서 피드 만들기](spreadsheet-feed-create.md)
>* [스프레드시트 보고서 피드 설정 편집](spreadsheet-feed-edit.md)
>* [스프레드시트 보고서 피드 설정](spreadsheet-feed-settings.md)
>* [스프레드시트 보고서 피드 파일 보기 또는 저장](spreadsheet-feed-view-or-save.md)
>* [스프레드시트 보고서 피드 수동 새로 고침](spreadsheet-feed-refresh.md)
>* [스프레드시트 보고서 피드 삭제](spreadsheet-feed-delete.md)

