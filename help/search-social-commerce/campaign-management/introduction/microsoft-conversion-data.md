---
title: '[!DNL Microsoft Advertising] 전환 데이터'
description: 의 유형에 대해 알아보기 [!DNL Microsoft Advertising]- 추적된 전환 데이터를 검색, 소셜 및 Commerce에서 사용할 수 있습니다.
feature: Search Campaign Management, Conversions
exl-id: 0ebc70a0-1fb7-48db-b45d-7409e8bb6f64
source-git-commit: 67fe8581832dc0762d62908d01672e53cc95b847
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 0%

---

# [!DNL Microsoft Advertising] 검색, 소셜 및 상거래의 전환 데이터

검색, 소셜 및 Commerce은 사용자가 추적한 모든 전환을 자동으로 동기화합니다. [[!DNL Microsoft Advertising] 범용 이벤트 추적(UET) 태그](https://about.ads.microsoft.com/solutions/tools/universal-event-tracking) (뷰스루 변환 포함), 보고 및 최적화를 위한 웹 사이트 전환용.

모든 지표는 캠페인 관리 보기 및 기본 보고서에서 자동으로 사용할 수 있으며, 의 최적화를 위한 포트폴리오 목표에서도 사용할 수 있습니다 [!DNL Microsoft Advertising] 캠페인.

## 사용 가능한 전환 데이터

Search, Social 및 Commerce은 다음에 대한 전환에 대한 데이터를 동기화합니다. &quot;[!DNL Include in 'Conversions']&quot; 옵션이 활성화되어 지난 35일 동안 데이터를 가져온 다음 변경 사항을 매일 09까지 가져옵니다.:00-10:광고주의 시간대에 00입니다. 각 클릭에 대해 새로운 전환이 추적되므로 내역 데이터가 매일 변경될 수 있습니다.

각각에 대한 2개의 지표 [[!DNL Microsoft Advertising]-추적된 전환](https://help.ads.microsoft.com/apex/index/3/en-us/n5012) (설정하는 위치: [!DNL Microsoft Advertising])에 구성된 전환 이름을 사용하여 검색, 소셜 및 Commerce에서 자동으로 사용할 수 있습니다 [!DNL Microsoft Advertising]. 각 전환에 대한 지표는 다음과 같습니다.

* `<conversion-name>` — 키워드에 대한 전환 값(예: Purchase)입니다.

  >[!TIP]
  >
  >다음을 포함하는 포트폴리오의 목표에서 이 유형의 전환 지표 사용 [!DNL Microsoft Advertising] 최대 전환 값 및 Target ROAS 입찰 전략이 포함된 캠페인

* `CT_<conversion-name>` — &quot;CT_&quot; 접두사로 시작하는 전환 수(개수)(예: CT_Purchase)입니다.

  >[!TIP]
  >
  >다음을 포함하는 포트폴리오의 목표에서 이 유형의 전환 지표 사용 [!DNL Microsoft Advertising] 최대 전환 수 및 Target CPA 입찰 전략이 있는 캠페인.

클릭 시간과 계정에 대해 기능이 활성화된 날짜로부터의 전환/트랜잭션 시간을 기반으로 데이터를 사용할 수 있습니다.

[!DNL Microsoft Advertising] 각 전환 기록 기준 [입찰 단위](/help/search-social-commerce/glossary.md#a-b), 장치 및 클릭 날짜(전환 날짜 아님). 속성은 의 각 지표에 대한 기본 속성 설정을 기반으로 합니다. [!DNL Microsoft Advertising]; Adobe Advertising 수준 데이터를 클릭할 수 없기 때문에 이벤트 속성이 반영되지 않습니다.

>[!NOTE]
>
>* 전환 이름이 동일한 계정이 여러 개 있는 경우 Adobe Advertising에 중복 전환 이름이 표시될 수 있습니다. 이 경우 [표시 이름 변경](/help/search-social-commerce/admin/conversion-metrics/conversion-metric-edit-display-name.md) 의 중복 지표 중 하나에 대해 [!UICONTROL Admin] > [!UICONTROL Conversions]. 두 개의 서로 다른 지표에 동일한 이름이 있을 때는 보고가 정확하지 않습니다.
>* 입찰 단위 수준의 데이터는 동일한 수준의 광고 네트워크에 있는 데이터와 일치합니다. 그러나 상위 수준에 대한 광고 네트워크의 자체 전환 데이터에는 하위 입찰 단위에 귀속되지 않는 추가 전환이 포함될 수 있습니다. 검색, 소셜 및 Commerce의 데이터는 항상 입찰 단위 수준에서 롤업되므로, 예를 들어 캠페인 수준 보고서의 합계는 광고 네트워크의 캠페인 수준 보고서와 동일하지 않을 수 있습니다.
>* 데이터 분산은 일반적으로 추가 전환이 아직 동기화되지 않은 날의 후반보다 오전 동기화 후에 더 적습니다. 오전에 데이터의 유효성을 검사하는 것이 좋습니다.
>* 데이터는 대상 또는 지리적 위치 수준에서 사용할 수 없으므로 RLSA 및 위치 입찰 조정을 자동으로 최적화하는 데 사용되지 않습니다.

## 에서 전환 데이터를 비교하는 방법 [!DNL Microsoft Advertising] 검색, 소셜 및 Commerce의 데이터 포함

다음 보고서 설정을 사용하여 비교 가능한 데이터의 유효성을 검사합니다.

### 에서 사용할 보고서 설정 [!DNL Microsoft Advertising]

선택한 전환 작업에 대한 보고서를 일별로 생성하고 모든 광고 상태에 대한 데이터를 포함하십시오.

### 검색, 소셜 및 Commerce에서 사용할 보고서 설정

검색, 소셜 및 Commerce에서 보기 또는 보고서 옵션을 사용하여 클릭 날짜(트랜잭션 날짜가 아님)를 기반으로 전환을 봅니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Insights & Reports] >[!UICONTROL Reports]**.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL Create Report]**, 커서를 위로 가져갑니다. **[!UICONTROL Basic Reports]**&#x200B;을 클릭한 다음 을 클릭합니다 **[!UICONTROL Search Engine Account Report]**.

1. 다음에서 [!UICONTROL Report Settings] 창에서 다음 보고서 설정을 지정합니다.

   1. 다음에서 **[!UICONTROL Conversions Based]** 섹션에서 다음을 선택합니다. **[!UICONTROL Click date]**.

   1. 에 사용한 것과 동일한 날짜 범위를 지정합니다. [!DNL Microsoft Advertising] 보고서.

   1. 다음에서 **[!UICONTROL Search/Content]** 섹션, 선택 **[!UICONTROL Search Only]**.

   1. 다음에서 **[!UICONTROL Search Engine Hierarchy]** 섹션을 확장합니다. [!UICONTROL Microsoft Advertising] 섹션을 만들고 계정을 선택합니다.

   1. 를 엽니다. [!UICONTROL Columns] 탭을 클릭하고 다음을 추가합니다 [!DNL Microsoft Advertising] 비교할 지표입니다.

1. 클릭 **[!UICONTROL Create]**.

>[!MORELIKETHIS]
>
>* [광고 네트워크 계정 및 캠페인 구현 개요](campaign-implemention-overview.md)
>* [광고 네트워크 캠페인의 성능 모니터링 및 관리](monitor-performance-campaigns.md)
>* [광고주에 대해 추적된 전환 지표 보기](/help/search-social-commerce/admin/conversion-metrics/conversion-metric-view-tracked.md)
