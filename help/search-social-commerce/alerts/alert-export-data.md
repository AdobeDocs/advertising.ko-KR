---
title: 사용자 지정 경고에 대한 데이터 내보내기
description: 트리거된 경고에 대한 데이터를 파일로 내보내는 방법을 알아봅니다.
exl-id: e3467b39-21ed-431e-b5f4-c3dc2dd5266d
feature: Search Alerts
source-git-commit: 03475909ca942010e4380456079519f0c18adca3
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# 사용자 지정 경고에 대한 데이터 내보내기

트리거된 경고에 대한 데이터 또는 경고 템플릿에 대해 가장 최근에 트리거된 경고에 대한 데이터를 [!DNL Microsoft Excel] 통합 문서([XLS](/help/search-social-commerce/glossary.md#w-x) 파일), 탭으로 구분된 값([TSV](/help/search-social-commerce/glossary.md#s-t)) 파일 또는 쉼표로 구분된 값([CSV](/help/search-social-commerce/glossary.md#c-d)) 파일로 내보낼 수 있습니다. 다운로드 가능한 보고서는 경고가 트리거된 후 자동으로 삭제된 후 10일 동안 사용할 수 있습니다.

1. 다음 중 하나를 수행합니다.

   * (경고 템플릿에 대해 가장 최근에 트리거된 경고에 대한 데이터를 내보내려면) 기본 메뉴에서 경고 템플릿 보기로 열리는 **[!UICONTROL Search]> [!UICONTROL Insights & Reports] >[!UICONTROL Custom Alerts]**&#x200B;을(를) 클릭합니다.

   * (특정 트리거된 경고에 대한 데이터를 내보내려면) 기본 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Insights & Reports] >[!UICONTROL Custom Alerts]**&#x200B;을(를) 클릭합니다. 하위 메뉴에서 **[!UICONTROL Triggered Alerts]**&#x200B;을(를) 클릭합니다.

1. 템플릿 또는 보고서 이름 옆에 있는 [!UICONTROL Export] 열에서 형식 이름을 클릭한 다음 브라우저의 일반 절차에 따라 파일을 열거나 저장합니다.

   * **[!UICONTROL XLS]:** XLS(단일 워크시트)가 있는 [!DNL Excel] 통합 문서의 경우. 이 보고서는 맨 위에 매개 변수와 함께 레이블이 지정된 워크시트를 하나 포함하고 구성 요소에 대한 데이터를 사용할 수 있는 경우 포함된 각 구성 요소에 대해 하나의 행이 있습니다. 데이터가 없는 행은 생략됩니다. 기본 보고서에는 각 숫자 열에 대한 합계가 포함됩니다.

   * TSV 파일용 **[!UICONTROL TSV]:**. 이 보고서에는 포함된 각 구성 요소에 대한 매개 변수와 하나의 행이 포함됩니다.

   * CSV 파일용 **[!UICONTROL CSV]:**. 이 보고서에는 포함된 각 구성 요소에 대한 매개 변수와 하나의 행이 포함됩니다.

>[!MORELIKETHIS]
>
>* [사용자 지정 경고 정보](alert-about.md)
>* [사용자 지정 경고 템플릿 만들기](alert-template-create.md)
>* [사용자 지정 경고 템플릿 편집](alert-template-edit.md)
>* [사용자 지정 경고 템플릿 일시 중지](alert-template-pause.md)
>* [사용자 지정 경고 템플릿 활성화](alert-template-activate.md)
>* [사용자 지정 경고 템플릿을 삭제](alert-template-delete.md)
>* [사용자 지정 경고 템플릿 설정](alert-template-settings.md)
>* [사용자 지정 경고 보기](alert-view.md)
