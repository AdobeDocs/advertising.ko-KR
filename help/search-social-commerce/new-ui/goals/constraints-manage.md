---
title: 검색 입찰 단위에 대한 제한 관리
description: 레거시 키워드 수준 포트폴리오의 CPC 캠페인에서 입찰 단위 입찰을 제한하는 제한에 대해 알아봅니다.
feature: Search Campaign Management, Search Optimization
source-git-commit: bfca434eacf52ec7236804c54b7740442aa12961
workflow-type: tm+mt
source-wordcount: '2649'
ht-degree: 0%

---

# 검색 입찰 단위에 대한 제한 관리

*레거시 키워드 수준의 포트폴리오에서만 CPC 캠페인의 입찰 단위에 적용 가능*

입찰 단위 제한은 제한과 관련된 비용 및 수익 모델을 사용하는 모든 [입찰 단위](https://experienceleague.adobe.com/docs/advertising/search-social-commerce/glossary.html?lang=ko)에 대해 최적화된 입찰을 제한하는 규칙입니다.

## 제한 정보

각 제한은 특정 통화에 적용되며, 선택적으로 규칙이 적용되기 위해 지정된 데이터 평가 기간 동안 충족되어야 하는 트리거 조건을 포함합니다. 평가할 데이터에는 채널 유형, 일치 유형, 클릭 데이터, 전환 데이터 또는 파생 지표가 포함될 수 있습니다. 예를 들어 입찰을 특정 화폐 범위로 제한하거나, 지정된 금액만큼 입찰을 지속적으로 증감하거나, 포트폴리오의 평균 입찰가에 따라 입찰할 수 있습니다. 각 제한에는 적용 가능한 시작 일자가 있으며 특정 일자에 만료되거나 무기한 적용됩니다.

제한을 설정한 후에는 특정 입찰 단위나 특정 광고 그룹 또는 캠페인 내의 모든 입찰 단위에 할당할 수 있습니다. 각 입찰 단위는 하나의 제한을 가질 수 있습니다. 구속은 하위 엔티티에 상속되지만 재정의할 수 있습니다. 최하위 레벨에 지정된 구속은 항상 상위 레벨에 지정된 구속보다 우선합니다. 입찰 단위에 제한을 지정하면 입찰 단위에 비용 및 수익 모델이 있을 때 입찰 단위가 생성하는 수익의 양에 관계없이 입찰이 해당 입찰 단위에 대해 지정된 제한 내에서 작동합니다.

>[!CAUTION]
>
>입찰 단위에 제한을 지정할 때 입찰 최적화 시스템의 결정을 무시하고 입찰 단위에 대한 ROI에 대해 직접 책임을 집니다.

>[!NOTE]
>
>* 활성 제한은 최적화된 레거시 키워드 수준 포트폴리오에서 할당된 입찰 단위에 대해서만 입찰을 제한합니다. 하이브리드 포트폴리오에 있거나, 활성 포트폴리오에 있거나, 포트폴리오에 없는 입찰 단위에는 무시됩니다. **팁:** 포트폴리오 설정에서 포트폴리오 옵션을 &quot;캠페인 예산 제한 자동 조정&quot;으로 설정하십시오. 권장 &quot;다중&quot; 값은 &quot;1&quot;입니다.
> * 비용 및 수익 모델을 생성하기에 충분한 데이터가 없는 입찰 단위에 대해서는 입찰 제한이 무시됩니다.
>* (CPC 또는 eCPC 입찰 전략이 있는 캠페인) 입찰 제한이 포트폴리오 수준 입찰 제한과 충돌하면 제한 사항이 포트폴리오 수준 제한을 무시합니다. 예를 들어 포트폴리오의 최소 입찰가가 5 USD이지만 포트폴리오의 입찰 단위를 최소 입찰가 3 USD로 제한하면 입찰 단위는 3 USD 이상으로 입찰됩니다. 그러나 제한된 입찰 단위에 대한 전체 지출은 포트폴리오의 [&quot;제약 조건 관련 지출&quot; 매개 변수](#spend-around-constraints)에 의해 결정됩니다.
>* 제한은 기본 입찰에서 작동합니다. 기본 입찰에 대한 입찰 조정 유형(예: 모바일 디바이스의 최종 사용자에 대한 입찰 상승)은 입찰을 제한에 대한 허용 범위 밖으로 이동할 수 있습니다. 예를 들어 제한에 최대 CPC 6달러가 필요하고 기본 입찰가는 이미 6달러이며 포트폴리오가 모바일 장치에 대한 입찰 조정을 50%-60%로 자동 최적화하는 경우 최대 CPC는 6달러가 아닌 9.00-9.60USD입니다.

### 제한 유형 {#constraint-types}

* **[!UICONTROL Bid]:** 입찰을 금액 범위로 제한합니다.

* **[!UICONTROL Bid Shift]:** 입찰 범위 내에서 지정된 금액만큼 연결된 모든 입찰 단위에 대해 최적화된 입찰을 지속적으로 변경합니다. 입찰 전환은 &quot;제약 조건 관련 지출&quot;에 대한 포트폴리오의 설정에 관계없이 관련 포트폴리오를 입찰 전환으로 인해 발생한 총 금액만큼 초과 또는 과소 지출하게 합니다. 참고: 현재 CPC 입찰이 이미 최대 입찰가보다 크거나 같거나 최소 입찰가보다 작거나 같은 경우 제한이 무시되고 입찰가가 변경되지 않습니다. 또한 입찰 전환 제한은 비용 및 수익 모델을 생성하기에 충분한 데이터가 없는 입찰 단위에 적용되지 않습니다.

* **[!UICONTROL Incremental Bidding]:**(노출 수가 없는 키워드에만 적용 가능) 입찰이 지정된 대상에 도달할 때까지 지정된 비율로 입찰을 증감합니다.

* **[!UICONTROL Search Engine Min Bid]:** ([!DNL Google Ads] 계정 전용) 검색 엔진에서 결정한 최소 CPC 입찰가를 최소 입찰가로 사용합니다. 검색 엔진이 최소 입찰을 변경하면 그에 따라 입찰이 변경됩니다. 연관된 모든 입찰 단위에 대해 추가 입찰 제한을 선택적으로 지정할 수 있습니다.

* **[!UICONTROL Impression Share]:**([!DNL Google Ads] 및 [!DNL Microsoft Advertising] CPC 캠페인과 정확히 일치하는 항목만 있음) 광고가 최소 노출 점유율과 최대 노출 점유율 사이에 있는 경우 입찰을 금액 범위로 제한합니다. **참고:** 제약 조건이 비용 효율적이지 않으면 최적화 기능이 이를 재정의할 수 있습니다.

### 제한 적용 시기

입찰 단위를 제한하는 몇 가지 이유는 다음과 같습니다.

* 테스트되지 않은 키워드 및 광고를 신속하게 노출합니다.

* 새 포트폴리오, 계정, 캠페인 및 광고 그룹에 대한 위험을 완화합니다. 예를 들어 포트폴리오를 시작하기 전에 트래픽이 많은 입찰 단위에서 최대 입찰가를 설정한 다음 매일 값을 점진적으로 올릴 수 있습니다. 이를 통해 입찰 모델이 큰 입찰이 증가할 위험 없이 매일 조정할 수 있다.

* 전환율이 높은 테일 키워드가 입찰되지 않도록 하기 위해.

* 브랜드 또는 프로모션 중에 중요한 특정 용어를 입찰하기 위해.

### UI 내의 제한에 대한 정보를 볼 수 있는 위치

[[!UICONTROL Constraints] 보기](#constraints-view)을(를) 여는 것 외에도 다음과 같은 방법으로 제한 관련 정보를 볼 수 있습니다.

* 모든 제약 조건은 &quot;[!UICONTROL Constraints]&quot;이라는 단일 [레이블 분류](https://experienceleague.adobe.com/docs/advertising/search-social-commerce/campaign-management/label-classifications/classification-about.html?lang=ko)에 대한 레이블 값입니다.

   * &quot;[!UICONTROL Constraints]&quot;은(는) 기본 및 사용자 지정 보기 설정과 예약된 보고서의 &quot;[!UICONTROL Classifications]&quot; 목록에 포함되어 있습니다. 관련 엔티티에 할당된 구속을 보려는 위치에 열을 추가할 수 있습니다.

   * 일괄 시트를 다운로드하면 &quot;[!UICONTROL Constraints]&quot;이(가) [!UICONTROL Download Bulksheet] 대화 상자의 적용 가능한 엔터티에 대해 &quot;[!UICONTROL Classifications]&quot; 열 아래에 나열됩니다. 열을 포함할 때 다운로드된 일괄 시트에는 관련 엔티티에 할당된 모든 구속이 포함됩니다.

  [!UICONTROL Constraints] 분류가 [!UICONTROL Label Classifications] 보기에 포함되어 있지 않습니다. [!UICONTROL Constraints] 보기는 별개입니다. [!UICONTROL Constraints] 분류도 30개 레이블 분류 제한에 포함되지 않습니다.

* [[!UICONTROL Constraint Report]](/help/search-social-commerce/new-ui/reports/management/basic-advanced/constraint-report.md)에는 레이블 분류 아키텍처를 사용하는 제약 조건에 대한 비용, 클릭 및 선택적으로 변환 데이터가 포함됩니다.

### [!UICONTROL Constraints] 보기 {#constraints-view}

[!UICONTROL Goals] > [!UICONTROL Constraints] 보기에는 모든 제약 조건이 나열됩니다. 사용 가능한 열에는 제한 상태, 제한 유형, 시작 및 종료 날짜, 제한이 연결된 캠페인, 광고 그룹, 키워드, 광고, 배치, 자동 타겟 및 제품 그룹의 수, 노출 횟수, 클릭 수 및 비용 데이터, 표시되는 모든 전환 지표에 대한 매출 데이터가 포함됩니다.<!-- Clarify why "Ads" is listed, unless it's to identify the relevant ads -->

>[!IMPORTANT]
>
>[!UICONTROL Constraints] 보기의 행에 대한 성능 데이터가 제약 조건이 할당된 최상위 엔터티의 성능 데이터와 일치하지 않을 수 있습니다. 가장 낮은 수준에서 지정된 제약 조건은 항상 상위 수준에서 지정된 제약 조건을 무시하므로 캠페인이나 광고 그룹에 지정된 제약 조건이 하위 광고 그룹 및 키워드에 지정된 상태로 유지되지 않을 수 있습니다. 예를 들어 캠페인 A에 제한 A가 할당되면 캠페인 A의 모든 광고 그룹 및 키워드는 제한 A를 자동으로 상속합니다. 그러나 이러한 광고 그룹 및 키워드는 나중에 제한 B와 같은 다른 제한에 할당될 수 있고, 그런 다음 제한 A와의 연관성을 잃게 됩니다.

>[!NOTE]
>
>관련 엔터티 관리 보기(예: 캠페인 수준 제한에 대한 [!UICONTROL Campaigns] 보기)에서 입찰 단위에 제한을 할당하고 할당을 취소하십시오.

#### 사용 가능한 작업

* [제약 조건을 만듭니다](#constraint-create).

* [제한 설정 편집](#constraint-edit).

* [제한 상태를 변경합니다](#constraint-change-status).

## 제한 만들기 {#constraint-create}

1. 메인 메뉴에서 **[!UICONTROL Goals]>[!UICONTROL Constraints]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위의 오른쪽 위 도구 모음에서 **[!UICONTROL Create Constraint]**&#x200B;을(를) 클릭합니다.

1. [제약 조건 설정](#constraint-settings)을 입력하십시오.

   [!UICONTROL Constraint Type] 탭과 [!UICONTROL Conditions] 탭 사이를 이동하려면 열려는 탭을 클릭하거나 [!UICONTROL Next] 및 [!UICONTROL Back] 단추를 클릭합니다.

1. 설정을 검토하려면 **[!UICONTROL Review and Save]**&#x200B;을(를) 클릭하십시오.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

제약 조건을 만든 후에는 캠페인, 광고 그룹, 키워드, 배치 및 단위 수준 제품 그룹에 [할당할 수 있습니다](#constraint-assign).

## 제한 설정 편집 {#constraint-edit}

한 번에 하나의 제한 사항에 대한 설정을 편집할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Goals]>[!UICONTROL Constraints]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 도구 모음[&#128279;](/help/search-social-commerce/common-tasks/data-views/ad-hoc-settings/column-filter-apply-from-toolbar.md) 또는 [열 제목](/help/search-social-commerce/common-tasks/data-views/ad-hoc-settings/column-filter-apply-from-column-heading.md)에서  목록을 필터링합니다.

1. 편집할 제한 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 ![편집](/help/search-social-commerce/assets/edit-new.png "편집")을 클릭합니다.

1. [제한 설정](#constraint-settings)을(를) 편집합니다.

   [!UICONTROL Constraint Type] 탭과 [!UICONTROL Conditions] 탭 사이를 이동하려면 열려는 탭을 클릭하거나 [!UICONTROL Next] 및 [!UICONTROL Back] 단추를 클릭합니다.

1. 설정을 검토하려면 **[!UICONTROL Review and Save]**&#x200B;을(를) 클릭하십시오.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 제한 상태 변경 {#constraint-change-status}

활성 제한을 일시 중지하여 비활성화할 수 있습니다. 나중에 상태를 *활성*(으)로 다시 변경하여 활성화할 수 있습니다.

또한 제한을 삭제할 수 있습니다. 이렇게 하면 계정 구성 요소와의 모든 연결이 제거되고 나중에 사용할 수 없게 됩니다. 제한에 대한 보고서 데이터를 더 이상 사용할 수 없습니다. **참고:** 계정 구성 요소에서 제약 조건을 단순히 연결 해제하려면 &quot;[검색 입찰 단위에서 제약 조건 할당 해제](#constraints-unassign)&quot;를 참조하십시오.

1. 메인 메뉴에서 **[!UICONTROL Goals]>[!UICONTROL Constraints]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 도구 모음[&#128279;](/help/search-social-commerce/common-tasks/data-views/ad-hoc-settings/column-filter-apply-from-toolbar.md) 또는 [열 제목](/help/search-social-commerce/common-tasks/data-views/ad-hoc-settings/column-filter-apply-from-column-heading.md)에서  목록을 필터링합니다.

1. 상태를 변경할 각 제약 조건 옆의 확인란을 선택합니다.

   여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)&quot;을 참조하십시오.

1. 일괄 작업 도구 모음에서 상태 단추 를 클릭합니다.

   * 선택한 행을 모두 활성화하려면 ![활성화](/help/search-social-commerce/assets/activate-new.png "활성화")를 클릭합니다.

   * 선택한 모든 행을 일시 중지하려면 ![일시 중지](/help/search-social-commerce/assets/pause-new.png "일시 중지")를 클릭합니다.

   * 선택한 행을 모두 삭제하려면 ![삭제](/help/search-social-commerce/assets/delete-new.png "삭제")를 클릭하십시오.

1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

## 제한 설정 {#constraint-settings}

| 탭 | 매개 변수 | 설명 |
|---|---|---|
| \[기본 정보\] | [!UICONTROL Constraint Name] | 제약 조건의 고유 이름입니다. |
| | [!UICONTROL Currency] | 적용 가능한 입찰 단위가 입찰되는 통화. 다른 통화가 사용되는 입찰 단위는 무시됩니다. |
| | [!UICONTROL Status] | 제한 상태:<ul><li>**활성:**(기본값) 지정한 조건 및 날짜 범위 동안 제약 조건이 적용됩니다.</li><li>**일시 중지됨:** 제한이 적용되지 않습니다.</li></ul> |
| [!UICONTROL Constraint Type] | [!UICONTROL Constraint Type] | 제한 유형입니다. 제한 유형 및 각 제한 유형에 적합한 광고 네트워크에 대한 설명은 &quot;[제한 유형](#constraint-types)&quot;을(를) 참조하십시오. |
| | [!UICONTROL Start Date] | 제한이 적용되는 첫 번째 날입니다. 기본값은 현재 날짜입니다. 날짜를 변경하려면 날짜를 입력하거나 ![일정](/help/search-social-commerce/assets/calendar-new.png "일정")을 클릭하여 일정을 열고 날짜를 선택하세요. |
| | [종료 날짜] | 특정 날짜에 제한이 효과가 없게 되는지 여부. 입찰 단위가 회사 브랜드의 중심이 되는 경우와 같이 제한을 무기한으로 적용하려면 필드를 비워 둡니다. 특정 날짜에 대한 제한을 종료하려면 날짜를 입력하거나 ![달력](/help/search-social-commerce/assets/calendar-new.png "달력")을 클릭하여 달력을 열고 날짜를 선택하세요. **참고:** 제한 사항은 내일 전에 만료될 수 없습니다. |
| | [!UICONTROL Set constraint options for Bid] | ([!UICONTROL Bid] 제약 조건만 해당) 설정에는 다음이 포함됩니다.<ul><li>**[!UICONTROL Min Bid]:** 연결된 입찰 단위에 대한 최소 기본 입찰입니다.</li><li>**[!UICONTROL Max Bid]:** 연결된 입찰 단위에 대한 최대 기본 입찰입니다.</li></ul> |
| | [!UICONTROL Set constraint options for Bid Shift] | ([!UICONTROL Bid Shift] 제한만 해당) 기본 입찰에 지속적으로 적용할 입찰 전환 유형 및 금액:<ul><li>*[!UICONTROL Increases]:* 지정한 백분율 또는 통화 값만큼 입찰을 늘립니다. 변경할 금액을 입력한 다음 *$* 또는 *%*&#x200B;을(를) 선택하십시오. 또한 제한이 적용될 때 가능한 가장 높은 입찰(상한)인 **[!UICONTROL Max Limit]**&#x200B;을(를) 입력하십시오. **참고:** 현재 CPC 입찰이 이미 [!UICONTROL Max Limit]보다 크거나 같은 경우 제한이 무시되고 입찰이 변경되지 않습니다.</li><li>*[!UICONTROL Decreases]:* 지정한 비율이나 통화 값만큼 입찰을 줄입니다. 변경할 금액을 입력한 다음 *$ 또는 %*&#x200B;을(를) 선택합니다. 또한 제한이 적용될 때 가능한 최저가 입찰(최저가)인 **[!UICONTROL Min Limit]**&#x200B;을(를) 입력하십시오. **참고:** 현재 CPC 입찰이 이미 [!UICONTROL Min Limit]보다 작거나 같은 경우 제한이 무시되고 입찰이 변경되지 않습니다.</li></ul>**메모:**<ul><li>입찰 변경을 수행하면 &quot;[!UICONTROL Spend Around Constraints]&quot;에 대한 포트폴리오의 설정에 관계없이 관련 포트폴리오가 입찰 전환으로 인해 발생한 총 금액만큼 초과 또는 과소 지출됩니다.</li><li>제한 사항의 종료 날짜를 지정하고 최적화 기능이 포트폴리오의 캠페인에 대한 지출 제한을 자동으로 조정하는 경우 입찰이 종료 날짜 이후에 단순히 원래 금액으로 돌아가는 것이 아니라 최적으로 조정됩니다.</li><li>입찰 전환은 비용 및 수익 모델을 생성하기에 충분한 데이터가 없는 입찰 단위에 적용되지 않습니다.</li></ul> |
| | [!UICONTROL Set constraint options for Incremental Bidding] | ([!UICONTROL Incremental Bidding] 제한만 해당) 입찰 대상 및 대상에 도달할 때까지 입찰을 증분적으로 늘리거나 줄이는 데 필요한 횟수와 빈도:<ul><li>**[!UICONTROL Bid target]:** 대상 입찰 금액입니다.</li><li>**[!UICONTROL Incrementally change bids by]** 및 **[Type]:** 입찰을 점진적으로 증가 또는 감소시키는 방법과 입찰을 통화 값(**$**) 또는 백분율(*%*)로 변경할지 여부를 지정합니다.</li><li>**[!UICONTROL Every __ days]:** 입찰가를 늘리는 빈도.</li></ul>예를 들어 키워드 중 하나의 현재 입찰가는 100센트이고 입찰 목표인 500센트에 도달할 때까지 입찰가를 매일 10%씩 변경하려고 한다고 가정해 보겠습니다. 제한이 설정된 후 1일에 해당 키워드의 입찰가는 110센트(현재 입찰 + 10%)입니다. 2일에 입찰가는 120센트(1일에 대한 현재 입찰가 + 20%)입니다. 그러나 입찰 대상이 50센트이고 다른 매개 변수가 동일한 경우 입찰이 50센트에 도달할 때까지 입찰이 점진적으로 감소합니다. |
| | [!UICONTROL Set constraint options for Search Engine Min Bid] | ([!UICONTROL Search Engine Min Bid] 제약 조건) Google에서 검색 결과의 첫 페이지에 입찰 단위를 표시하는 데 필요한 최소 입찰가를 사용합니다([!UICONTROL Google First Page CPC]). 필요한 경우 **[!UICONTROL Min Bid]** 값 및/또는 **[!UICONTROL Max Bid]** 값을 입력하여 제한에 적합한 입찰의 범위를 정의합니다. 예를 들어 [!UICONTROL Min Bid]&#x200B;(2.50 USD)와 [!UICONTROL Max Bid]&#x200B;(4 USD)를 지정하는 경우 [!DNL Google Ads] 첫 페이지 입찰가가 2.50 USD 미만이거나 4 USD 이상이면 입찰 단위에 입찰하지 않습니다. |
| | [!UICONTROL Set constraint options for Impression Share] | ([!UICONTROL Impression Share] 제약 조건만 해당) 설정에는 다음이 포함됩니다.<ul><li>**[!UICONTROL Min Bid]**(선택 사항) 연결된 입찰 단위에 대한 최소 기본 입찰입니다.</li><li>**[!UICONTROL Max Bid]:**(선택 사항) 연결된 입찰 단위에 대한 최대 기본 입찰입니다.</li><li>**[!UICONTROL Min Impression Share]:** 적용 가능한 입찰 단위에 대한 제한을 트리거하는 가장 낮은 노출 점유율입니다. 10에서 90 사이여야 합니다. **참고:** 제약 조건이 비용 효율적이지 않으면 최적화 기능이 이를 재정의할 수 있습니다.</li><li>**[!UICONTROL Max Impression Share]:** 적용 가능한 입찰 단위에 대한 제한을 트리거하는 가장 높은 노출 점유율입니다. 10에서 90 사이여야 합니다.**참고:** 제약 조건이 비용 효율적이지 않으면 최적화 기능이 이를 재정의할 수 있습니다.</li></ul>> |
| [!UICONTROL Conditions] | [!UICONTROL Condition Type] | 제약 조건에 조건 적용 여부:<ul><li>*[!UICONTROL No Condition]:*(기본값) 지정한 날짜 범위 동안 제약 조건이 무조건 적용됩니다.</li><li>*[!UICONTROL Satisfy]:* 제약 조건은 지정된 데이터 평가 기간 동안 지정된 조건이 충족되는 경우에만 적용됩니다.</li></ul> |
| | [!UICONTROL Data Evaluation Period] | (조건이 설정된 경우) 지정된 기준에 대한 데이터를 평가할 기간입니다. *[!UICONTROL Custom date range]을(를) 선택하는 경우&#x200B;**은(는) `MM-DD-YYYY` 형식(예: 2026년 3월 29일 03-29-2026)으로 각 날짜를 입력하거나 ![달력 단추](/help/search-social-commerce/assets/calendar-new.png "달력 단추")를 클릭하여 달력을 열고 각 날짜를 선택하여 &#x200B;** [!UICONTROL Start Date]&#x200B;**&#x200B;과(와) &#x200B;** [!UICONTROL End Date]**&#x200B;을(를) 지정합니다. |
| | [!UICONTROL When to Apply Constraints] | (조건이 설정된 경우) 제한을 적용하려면 몇 개의 필터 조건을 충족해야 합니까?<ul><li>*[!UICONTROL Match All Filters]:* 지정한 모든 필터 조건이 충족될 때 제약 조건을 적용합니다.</li><li>*[!UICONTROL Match Any Filters]:* 지정한 필터 조건 중 하나 이상이 충족되면 제약 조건을 적용합니다.</li></ul> |
| | [!UICONTROL Filters] | (조건이 설정된 경우) 충족해야 하는 하나 이상의 기준. 필터를 만들려면 목록에서 속성 또는 지표를 선택합니다. 속성(예: [!UICONTROL Channel Type])의 경우 목록에서 적용 가능한 값을 선택합니다. 지표(예: [!UICONTROL Clicks])의 경우 연산자를 선택한 다음 해당 값을 입력합니다. 예를 들어 클릭수가 100개를 초과하는 입찰 단위만 반환하려면 **클릭수**&#x200B;을(를) 선택하고 **보다 큼**&#x200B;을(를) 선택한 다음 입력 필드에 `100`을(를) 입력합니다.</li></ul> |

## 입찰 단위 검색에 제한 할당 {#constraint-assign}

입찰 단위 제한을 단위 수준(하위 분류의 가장 낮은 수준)의 캠페인, 광고 그룹, 키워드, 배치, 쇼핑 제품 그룹 또는 동적 검색 대상에 적용할 수 있습니다.

각 엔티티에는 하나의 제약조건만 있을 수 있습니다. 한 개의 구속을 하나 이상의 엔티티에 동시에 지정할 수 있습니다.

>[!NOTE]
>
>나중에 광고의 키워드나 광고 사본을 편집하여 새 키워드나 광고를 만들 경우 새 엔티티에 제한이 할당되지 않습니다.

1. 메인 메뉴에서 관련 관리 보기를 엽니다.

   예를 들어 캠페인 수준에서 제약 조건을 할당하려면 [!UICONTROL Manage] > [!UICONTROL Campaigns]&#x200B;(으)로 이동합니다.

   <!-- for [campaigns](/help/search-social-commerce/new-ui/manage/campaigns/campaign-constraint-assignments-manage.md), [ad groups](/help/search-social-commerce/new-ui/manage/ad-groups/ad-group-constraint-assignments-manage.md), [keywords](/help/search-social-commerce/new-ui/target/keywords/keyword-assignments-manage.md), or [placements](/help/search-social-commerce/new-ui/target/placements/placement-assignments-manage.md). And ADD LINKS WHEN AVAILABLE for shopping product groups and dynamic search targets. -->

1. (선택 사항) 도구 모음[&#128279;](/help/search-social-commerce/common-tasks/data-views/ad-hoc-settings/column-filter-apply-from-toolbar.md) 또는 [열 제목](/help/search-social-commerce/common-tasks/data-views/ad-hoc-settings/column-filter-apply-from-column-heading.md)에서  목록을 필터링합니다.

1. 단일 구속을 지정할 각 엔티티 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **+[!UICONTROL Assign]** > **[!UICONTROL Constraint]**&#x200B;을(를) 클릭합니다.

1. 제약조건을 선택합니다.

1. **[!UICONTROL Assign Now]**&#x200B;을(를) 클릭합니다.

## 입찰 단위 검색에서 제한 할당 해제 {#constraints-unassign}

**참고:** 제약 조건을 삭제하여 나중에 사용할 수 없게 하려면 &quot;[제약 조건 상태 변경](#constraint-change-status)&quot;을 참조하세요.&quot;

1. 메인 메뉴에서 관련 관리 보기를 엽니다.

   예를 들어 캠페인 수준 제약 조건의 할당을 취소하려면 [!UICONTROL Manage] > [!UICONTROL Campaigns]&#x200B;(으)로 이동합니다.

1. 제약 조건을 할당 해제할 각 엔티티 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **-[!UICONTROL Unassign]** > **[!UICONTROL Constraint]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [캠페인에 대한 제한 할당 관리](/help/search-social-commerce/new-ui/manage/campaigns/campaign-constraint-assignments-manage.md)
>* [광고 그룹에 대한 제약 조건 할당 관리](/help/search-social-commerce/new-ui/manage/ad-groups/ad-group-constraint-assignments-manage.md)
>* [키워드에 대한 제약 조건 할당 관리](/help/search-social-commerce/new-ui/target/keywords/keyword-assignments-manage.md)
>* [배치에 대한 제한 할당 관리](/help/search-social-commerce/new-ui/target/placements/placement-assignments-manage.md)
>* [[!UICONTROL Constraint Report]](/help/search-social-commerce/new-ui/reports/management/basic-advanced/constraint-report.md)
