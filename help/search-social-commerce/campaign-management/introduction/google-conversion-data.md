---
title: "[!DNL Google Ads] 전환 데이터"
description: 의 유형에 대해 알아보기 [!DNL Google Ads]- 추적 전환 데이터는 검색, 소셜 및 상거래에서 사용할 수 있습니다.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---

# [!DNL Google Ads] 검색, 소셜 및 상거래의 전환 데이터

검색, 소셜 및 상거래 자동 동기화 [!DNL Google Ads]-에서 모든 캠페인에 대한 전환 데이터를 추적했습니다. [!DNL Google Ads] 보고 및 최적화를 위해 검색, 소셜 및 상거래에 검색 및 쇼핑 네트워크. Search, Social 및 Commerce는 다음에 대한 변환에 대한 데이터를 동기화합니다. &quot;[!DNL Include in 'Conversions']&quot; 옵션이 활성화되어 지난 30일 동안 데이터를 가져온 다음 변경 사항을 매일 데이터로 가져옵니다.

## 사용 가능한 전환 데이터

각각에 대해 최대 3개의 거래 속성 [[!DNL Google Ads]-추적된 전환](https://support.google.com/google-ads/answer/4677036) (설정하는 위치: [!DNL Google Ads])에 구성된 전환 이름을 사용하여 검색, 소셜 및 상거래에서 자동으로 사용할 수 있습니다 [!DNL Google Ads]. 각 전환에 대한 거래 속성은 다음과 같습니다.

* `GGL*` — (추적할 때) &quot;GGL&quot; 접두사로 시작하는 키워드에 대한 전환 값의 합계(예: GGL 구매).

* `GGL_CT*` — &quot;GGL_CT&quot; 접두사로 시작하는 전환 수(개수)(예: GGL_CT_Purchase)

* `GGL_XD_CT*` — (전환 유형에 사용할 수 있는 경우, 추적할 때) &quot;GGL_XD_CT_&quot; 접두사로 시작하는 Google에서 측정한 교차 장치 전환 수(개수)입니다(예: GGL_XD_CT_Purchase).

데이터는 계정에 대해 기능이 활성화된 날짜부터 사용할 수 있으며 09까지 매일 업데이트됩니다:00-10:광고주의 시간대에 00입니다.

[!DNL Google Ads] 각 전환 기록 기준 [입찰 단위](/help/search-social-commerce/glossary.md#a-b), 장치 및 클릭 날짜(전환 날짜 아님). 속성은 의 각 지표에 대한 기본 속성 설정을 기반으로 합니다. [!DNL Google Ads]; Adobe 광고 속성은 클릭 이벤트 수준 데이터를 사용할 수 없기 때문에 팩토링되지 않습니다. 매일 검색, 소셜 및 상거래는 이전 30일 동안의 전환 데이터를 가져온 다음, 다음 날짜의 클릭 날짜를 사용하여 이전 날 이후의 증분 전환을 계산합니다 [!DNL Google Ads] 전일을 트랜잭션 일자로 지정. 그 결과, 클릭할 때마다 새로운 전환이 추적되므로 내역 데이터가 매일 변경될 수 있습니다. 검색, 소셜 및 상거래의 데이터를 의 데이터와 비교하는 경우 [!DNL Google Ads], 보기 또는 보고서 옵션을 사용하여 &quot;&quot;를 봅니다.[!UICONTROL Conversions by: Click date]&quot;(트랜잭션 날짜별로 아님).

모든 지표는 캠페인 관리 보기 및 기본 보고서에서 자동으로 사용할 수 있으며 최적화를 위한 포트폴리오 목표에서도 사용할 수 있습니다.

>[!NOTE]
>
>* 전환 이름이 동일한 계정이 여러 개 있는 경우 Adobe 광고에서 중복 전환 이름이 표시될 수 있습니다. 이 경우 [표시 이름 변경](/help/search-social-commerce/admin/transaction-properties/transaction-property-edit-display-name.md) 의 중복 지표 중 하나에 대해 [!UICONTROL Admin] > [!UICONTROL Transaction Properties]. 두 개의 서로 다른 지표에 동일한 이름이 있을 때는 보고가 정확하지 않습니다.
>* 입찰 단위 수준의 데이터가 의 데이터와 일치함 [!DNL Google Ads] 같은 수준에서. 그러나 [!DNL Google Ads]&#39; 상위 수준에 대한 자체 전환 데이터에는 하위 입찰 단위에 귀속되지 않는 추가 전환이 포함될 수 있습니다. 검색, 소셜 및 상거래의 데이터는 항상 입찰 단위 수준에서 롤업되므로, 예를 들어 캠페인 수준 보고서의 합계는 Google 광고의 캠페인 수준 보고서와 동일하지 않을 수 있습니다.
>* 데이터 분산은 일반적으로 추가 전환이 아직 동기화되지 않은 날의 후반보다 오전 동기화 후에 더 적습니다. 오전에 데이터의 유효성을 검사하는 것이 좋습니다.
>* 다음에 대한 전환 데이터를 사용할 수 없음: [!DNL Google Display Network], [!DNL Gmail], [!DNL Mobile App], 및 [!DNL YouTube] 광고. 에서 데이터를 비교할 때 그러한 유형의 광고를 필터링합니다. [!DNL Google Ads] 검색, 소셜 및 커머스의 데이터로.
>* 다음에 대한 데이터 [!DNL Google Ads] 전환은 대상 또는 지리적 위치 수준에서 사용할 수 없으므로 RLSA 및 위치 입찰 조정을 자동으로 최적화하는 데 사용되지 않습니다.


## 에서 전환 데이터를 비교하는 방법 [!DNL Google Ads] 검색, 소셜 및 상거래의 데이터 포함

다음 보고서 설정을 사용하여 비교 가능한 데이터의 유효성을 검사합니다.

### 에서 사용할 보고서 설정 [!DNL Google Ads]

1. 기본 도구 모음에서 를 선택합니다. **[!DNL Reports]>[!DNL Report]**.

1. 선택 **[!DNL + Custom]>[!DNL Table]**.

1. 왼쪽 창에서 보고서의 행과 열을 지정합니다.

   1. 검색 **[!DNL Day]** 필드를 드래그하여 [!DNL Row] 섹션.

   1. 검색 **[!DNL All conv].** 필드를 드래그하여 [!DNL Column] 섹션.

   1. 검색 **[!DNL Conversion action]** 필드를 드래그하여 [!DNL Column] 섹션.

1. 보고서 설정 도구 모음에서 **[!DNL Filter]>[!DNL Ad status]**&#x200B;를 클릭한 다음 모든 상자를 선택합니다.

1. 보고서 설정 도구 모음에서 **[!DNL Download]>[!DNL Excel .csv]**.

### 검색, 소셜 및 상거래에 사용할 보고서 설정

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Insights & Reports] >[!UICONTROL Reports]**.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL Create Report]**, 커서를 위로 가져갑니다. **[!UICONTROL Basic Reports]**&#x200B;을 클릭한 다음 을 클릭합니다 **[!UICONTROL Search Engine Account Report]**.

1. 다음에서 [!UICONTROL Report Settings] 창에서 다음 보고서 설정을 지정합니다.

   1. 다음에서 **[!UICONTROL Conversions Based]** 섹션에서 다음을 선택합니다. **[!UICONTROL Click date]**.

   1. 에 사용한 것과 동일한 날짜 범위를 지정합니다. [!DNL Google Ads] 보고서.

   1. 다음에서 **[!UICONTROL Search/Content]** 섹션, 선택 **[!UICONTROL Search Only]**.

   1. 다음에서 **[!UICONTROL Search Engine Hierarchy]** 섹션을 확장합니다. [!UICONTROL Google Adwords] 섹션을 만들고 계정을 선택합니다.

   1. 를 엽니다. [!UICONTROL Columns] 탭을 클릭하고 다음을 추가합니다 [!DNL Google Ads] 비교할 지표(&quot;GGL&quot;로 시작).

1. 클릭 **[!UICONTROL Create]**.

>[!MORELIKETHIS]
>
>* [검색, 소셜 및 상거래의 캠페인 관리 기본 정보](campaign-management-about.md)
>* [광고 네트워크 계정 및 캠페인 구현 개요](campaign-implemention-overview.md)
>* [광고 네트워크 캠페인의 성능 모니터링 및 관리](monitor-performance-campaigns.md)
