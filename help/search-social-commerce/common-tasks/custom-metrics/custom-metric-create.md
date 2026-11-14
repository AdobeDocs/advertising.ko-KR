---
title: 사용자 지정 지표 만들기
description: 표준 지표에서 계산되는 사용자 지정 지표를 구성하는 방법을 알아봅니다.
exl-id: a9ce503a-67ee-477e-8f79-31b4a9c6e51a
feature: Search Common Tasks, Search Custom Metrics
TQID: 'https://experienceleague.adobe.com/g-J8AlulQ20I-vxQrPkPaP-Ap66bBIng0eKDPqhV9U4'
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: bcc57258-3285-5d02-a731-d86f57a58c47
    internal-label: Search Common Tasks
  - id: a1695a4d-41fb-5bb6-a22a-9e7a1b3222d7
    internal-label: Search Custom Metrics
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 9837cac1a920b1b3b88b04b150cb604832209eaf
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%
---
# 사용자 지정 지표 만들기

## (새 UI) 관리 보기에서 사용자 지정 지표 만들기

[!UICONTROL Manage] 메뉴의 대부분의 엔터티 보기에서 사용할 수 있습니다.<!-- [!UICONTROL Plan] > [!UICONTROL Simulations],-->* [!UICONTROL Setup] > [!UICONTROL Label Classifications], [!UICONTROL Goals] > [!UICONTROL Objectives] 및 [!UICONTROL Constraints], [!UICONTROL Targeting] > [!UICONTROL Placements]*

1. 데이터 테이블 위에서 다음 중 하나를 수행합니다.

   * 현재 적용된 보기의 이름(![보기](/help/search-social-commerce/assets/view.png "보기"))을 클릭합니다. 편집 가능한 보기의 이름 위에 커서를 놓고 ![편집](/help/search-social-commerce/assets/edit-new.png "편집")을(를) 클릭하여 보기 설정을 엽니다.

     만든 사용자 지정 지표는 모든 보기에서 사용할 수 있습니다.

   * 열 구성 설정을 열려면 ![사용자 지정 열](/help/search-social-commerce/assets/custom-columns-new.png "사용자 지정 열")을 클릭하세요.

1. 열리는 열 목록 아래에서 ![사용자 지정 지표 만들기](/help/search-social-commerce/assets/add.png "사용자 지정 지표 만들기") **[!UICONTROL Create Custom Metric]**&#x200B;를 클릭합니다.

1. [사용자 지정 지표 설정](custom-metric-settings.md)을 지정하십시오.

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

## (새 UI) 보고서 또는 보고서 템플릿 설정에서 사용자 지정 지표 만들기 {#create-from-report-settings}

1. 보고서 또는 보고서 템플릿 설정 내에서 **[!UICONTROL Columns]** 단계로 이동합니다.

1. **[!UICONTROL Custom Metrics]** 섹션에서 지표 설정을 지정합니다.

   * **[!UICONTROL Custom Metric Name]:** 지표의 이름을 입력합니다.

   * **[!UICONTROL Format]:** **[!UICONTROL Currency]**, **[!UICONTROL Number to 2 Decimal Places]**, **[!UICONTROL Number to 3 Decimal Places]**, **[!UICONTROL Number w/out Decimal Places]** 또는 **[!UICONTROL Percentage]**&#x200B;을(를) 선택하십시오.

   * **[수식 입력 필드]:** **[!UICONTROL Insert Metric]**&#x200B;에서 지표를 선택하고 연산자 단추(`+`, `-`, `*`, `/`, `(` 및 `)`)를 클릭하여 수식을 만듭니다. 수식을 수동으로 입력할 수도 있습니다. 각 지표 또는 연산자를 삽입할 위치에 커서를 놓습니다.

1. **[!UICONTROL Add Metric]**&#x200B;을(를) 클릭합니다.

   지표가 성공적으로 생성되면 사용 가능한 열 목록이 지표 이름으로 필터링됩니다. 지표를 만들어도 보고서에 자동으로 포함되지 않습니다.

1. 보고서에 지표를 포함하려면 사용 가능한 열 목록에서 지표를 선택하고 ![오른쪽 화살표](/help/search-social-commerce/assets/arrow-right-customize.png "오른쪽 화살표")를 클릭하여 선택한 열 목록으로 이동합니다.

## (기존 UI) 캠페인 관리 보기에서 사용자 지정 지표를 만듭니다

1. 데이터 테이블 위에서 다음 중 하나를 수행합니다.

   * 기본 보기 또는 사용자 지정 보기의 이름을 클릭하여 보기 설정을 엽니다.

   * 열 구성 설정을 열려면 ![사용자 지정 열](/help/search-social-commerce/assets/custom-columns.png "사용자 지정 열")을 클릭하세요.

1. 열리는 열 목록 아래에서 ![새 사용자 지정 지표 만들기](/help/search-social-commerce/assets/add.png "새 사용자 지정 지표 만들기") **[!UICONTROL Create New Custom Metric]**&#x200B;를 클릭합니다.

1. [사용자 지정 지표 설정](custom-metric-settings.md)을 지정하십시오.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## (기존 UI) 보고서 또는 보고서 템플릿 양식에서 사용자 지정 지표를 만듭니다

1. 보고서 또는 보고서 템플릿 양식 내에서 **[!UICONTROL Columns]** 탭으로 이동합니다.

1. 오른쪽 섹션에서 **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

1. [사용자 지정 지표 설정](custom-metric-settings.md)을 지정하십시오.

1. **[!UICONTROL Submit]**&#x200B;을(를) 클릭합니다.

## (기존 UI) [!UICONTROL Portfolios] 보기에서 사용자 지정 지표를 만듭니다

1. 데이터 테이블 위에서 ![선택한 보기 편집](/help/search-social-commerce/assets/view-settings.png "선택한 보기 편집")을 클릭합니다.

1. **[!UICONTROL Columns]** 탭을 클릭합니다.

1. 오른쪽 섹션에서 **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

1. [사용자 지정 지표 설정](custom-metric-settings.md)을 지정하십시오.

1. **[!UICONTROL Submit]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [사용자 지정 지표 정보](custom-metric-about.md)
>* [사용자 지정 지표 편집](custom-metric-edit.md)
>* [사용자 지정 지표 삭제](custom-metric-delete.md)
>* [사용자 지정 지표 설정](custom-metric-settings.md)
