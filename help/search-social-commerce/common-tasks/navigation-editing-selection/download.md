---
title: 캠페인 관리 보기에서 데이터 다운로드
description: 대부분의 캠페인 관리 보기에서 데이터를 다운로드하는 방법을 알아봅니다.
exl-id: f549f03c-ed0b-4d7d-8d7e-91192c17e77e
feature: Search Common Tasks
source-git-commit: 67fe8581832dc0762d62908d01672e53cc95b847
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# 캠페인 관리 보기에서 데이터 다운로드

[!UICONTROL Keywords] - [!UICONTROL Keyword Negatives], [!UICONTROL Placements] - [!UICONTROL Placement Negatives], [!UICONTROL Audiences] 및 [!UICONTROL Extensions] 보기를 제외한 [!UICONTROL Search] > [!UICONTROL Campaigns] > [!UICONTROL Campaigns] 보기에서 데이터를 다운로드할 수 있습니다. 다음 중 하나를 다운로드할 수 있습니다.

* [!DNL XLSM] (매크로가 활성화된 [!DNL Microsoft Excel] 스프레드시트) 형식의 보고서입니다. 뷰에서 특정 행을 선택하면 보고서에는 선택한 각 행에 대해 하나의 행이 포함됩니다. 행을 선택하지 않으면 보기의 각 행에 대해 하나의 행이 만들어집니다.

* 모든 관련 하위 엔티티를 포함하는 TXT 형식의 일괄 시트 파일. 여러 광고 네트워크의 엔티티에 대해 행을 선택하면 각 관련 광고 네트워크에 대해 하나의 파일이 만들어집니다. 행을 선택하지 않으면 보기에 표시된 각 광고 네트워크에 대해 하나의 파일이 만들어집니다. 다른 광고 네트워크용으로 생성된 일괄 시트 파일에는 다른 데이터 열이 포함되어 있습니다.

  여러 캠페인에 대한 데이터를 생성하고 결합된 데이터가 500,000개 이상의 행으로 구성된 경우, 데이터는 캠페인에 의해 필요에 따라 `<bulksheet name>_1.txt`, `<bulksheet name>_2.txt` 등으로 이름이 지정된 둘 이상의 파일로 추가로 분할됩니다.

  [!UICONTROL Downloads] 패널의 각 일괄 시트 파일도 [!UICONTROL Bulksheets] 보기에 나열됩니다. 파일이 생성되면 파일을 다운로드할 수 있는 링크가 포함된 이메일 알림을 받게 됩니다. 컴파일되는 데이터 양에 따라 알림이 몇 분 이상 걸릴 수 있습니다. 그러나 파일 생성에 실패하면 오류 파일이 Bulksheets 보기에 나열되며 오류 파일에 대한 링크가 포함된 이메일 알림이 전송됩니다. [!UICONTROL Download] 패널 또는 [!UICONTROL Bulksheets] 탭에서 일괄 시트 파일을 삭제하면 두 위치에서 모두 삭제됩니다.

1. (선택 사항) 파일에 포함할 개별 행을 선택합니다.

   그렇지 않으면 보기의 모든 데이터가 포함됩니다.

1. 도구 모음 오른쪽에서 ![보고서 다운로드](/help/search-social-commerce/assets/download.png "보고서 다운로드")를 클릭합니다.

1. ![만들기](/help/search-social-commerce/assets/add.png "만들기") **[!UICONTROL Create]**&#x200B;을(를) 클릭하고 선택적으로 파일 이름을 추가한 다음 **[!UICONTROL Report]** 또는 **[!UICONTROL Bulksheet]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 보고서 작업이 완료되면 ![보고서 다운로드](/help/search-social-commerce/assets/download.png "보고서 다운로드")를 클릭하여 [!UICONTROL Available Reports] 패널을 본 다음 보고서를 다운로드하거나 삭제합니다.

   * 브라우저의 일반 절차에 따라 파일을 열거나 저장하려면 ![스프레드시트 다운로드](/help/search-social-commerce/assets/download-spreadsheet.png "스프레드시트 다운로드")를 클릭합니다.

     브라우저 절차에 대한 자세한 내용은 브라우저의 온라인 도움말을 참조하십시오.

   * 파일을 삭제하려면 ![삭제](/help/search-social-commerce/assets/delete.png "삭제")를 클릭하십시오.

>[!MORELIKETHIS]
>
>[성능 데이터 보고서 또는 일괄 시트 파일을 [!UICONTROL Downloads] 메뉴에서 삭제](/help/search-social-commerce/common-tasks/navigation-editing-selection/download-delete-data.md)
