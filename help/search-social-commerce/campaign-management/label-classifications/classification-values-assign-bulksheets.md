---
title: 일괄 시트를 사용하여 계정 구성 요소에 분류 값 할당
description: 일괄 시트를 사용하여 계정 구성 요소에 분류 값을 할당하는 방법을 알아봅니다.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 7%

---

# 일괄 시트를 사용하여 계정 구성 요소에 분류 값 할당

일괄 시트를 사용하여 레이블 분류를 검색 엔티티에 대한 값(캠페인, 광고 그룹, 키워드, 광고, 배치, 단위 수준 제품 그룹 및 동적 검색 대상)과 연결할 수 있습니다. 각 레이블 분류는 최대 2000개의 값을 가질 수 있습니다.

각 엔티티는 분류당 하나의 레이블 값을 가질 수 있습니다. 예를 들어 Shoes_Campaign의 색상 값은 &quot;빨간색&quot;이고 지역 값은 &quot;Los Angeles&quot;일 수 있지만 색상 또는 지역 값을 여러 개 가질 수는 없습니다.

레이블 값은 하위 엔티티에 의해 상속되므로 상속된 값을 재정의하지 않는 한 하위 엔티티에 대한 값을 입력하지 마십시오.

>[!NOTE]
>
>일부 광고 네트워크 및 캠페인 유형에 대한 키워드 및 광고 사본은 다음과 같습니다 [변경할 수 없음](/help/search-social-commerce/campaign-management/faqs-campaigns.md)를 지정하면 기존 엔티티가 삭제되고 새 엔티티가 만들어집니다. 이러한 방식으로 기존 엔티티를 삭제하면 레이블 분류가 새 엔티티에 할당되지 않습니다.

1. [일괄 시트 다운로드](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-download.md) 여기에는 레이블 분류 값을 지정할 엔티티가 포함됩니다.

   * 다음에서 [!UICONTROL Rows and Columns] 탭을 확장하고 [!UICONTROL Campaign] 목록: [!UICONTROL Bulksheet Columns] 창.

   * 확장 [!UICONTROL Label Classification] 목록을 표시합니다.

   * 일괄 시트 파일에 열을 포함할 각 분류를 선택합니다.

      예를 들어 레이블 분류 &quot;색상&quot; 및 &quot;지역&quot;을 포함하는 경우 일괄 시트에는 &quot;색상&quot; 및 &quot;지역&quot; 열이 포함됩니다.

1. 편집기에서 파일을 열고 레이블 값을 연결할 엔티티의 레이블 분류 열에 추가합니다. 각 값의 최대 길이는 100자이며, ASCII 및 비 ASCII 문자를 포함할 수 있습니다.

   다음 섹션에서 예제 값을 참조하십시오.

   값을 추가하는 것 외에도 관련 행에서 기존 값을 제거하여 삭제할 수도 있습니다. 상위 엔티티와 하위 엔티티 모두에서 값을 제거하려면 a) 상위 엔티티 행만 포함하고 기존 분류 값을 제거하거나 b) 상위 엔티티와 하위 엔티티를 모두 포함하고 상위 및 하위 행 모두에서 기존 분류 값을 제거합니다.

1. [파일 업로드](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-upload.md) 연결을 만듭니다.

업로드된 레이블 값은 관련 엔티티 보기에 표시됩니다.

## 일괄 시트에서 업로드할 레이블 분류 값의 예

이 예에는 레이블 분류 &quot;색상&quot; 및 &quot;지역&quot;에 대한 열이 포함되어 있습니다. 고유한 일괄 시트의 경우 열을 고유한 레이블 분류 이름으로 대체하십시오.

| 계정 | 캠페인 | 광고 그룹 | 키워드 | 광고 | 배치 | 레이블 | 색상 | 지역 |
|---|---|---|---|---|---|---|---|---|
| Acct1 | C1 |  |  |  |  |  | 녹색 |  |
| Acct1 | C1 | AG1 |  |  |  |  |  |  |
| Acct1 | C1 | AG1 | K1 |  |  |  |  | 영국 |
| Acct1 | C1 | AG1 | K2 |  |  |  | 빨강 | AU |
| Acct1 | C1 | AG1 | K3 |  |  |  | 파랑 | DE |
| Acct1 | C1 | AG1 |  | A1 |  |  |  |  |
| Acct1 | C1 | AG1 |  | A1 |  |  | 빨강 |  |
| Acct1 | C1 | AG1 |  |  | P1 |  | 빨강 | AU |
| Acct1 | C1 | AG1 |  |  | P2 |  | 파랑 | DE |

>[!MORELIKETHIS]
>
>* [레이블 분류 정보](classification-about.md)
>* [레이블 분류 만들기](classification-create.md)
>* [캠페인 관리 보기에서 계정 구성 요소에 분류 값 할당](classification-values-assign-campaign-management.md)
>* [계정 구성 요소에서 레이블 분류 값 제거](classification-values-remove.md)
>* [레이블 분류 값 삭제](classification-values-delete.md)
>* [레이블 분류 삭제](classification-delete.md)

