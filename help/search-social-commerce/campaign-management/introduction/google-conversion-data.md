---
title: '[!DNL Google Ads] 전환 데이터'
description: 검색, 소셜 및 Commerce에서 사용할 수 있는  [!DNL Google Ads] 추적 전환 데이터 유형에 대해 알아봅니다.
exl-id: a4634410-446b-4e2e-a52f-22a494f731f9
feature: Search Campaign Management, Conversions
source-git-commit: d0f1c413134a0868ddec79ded7672af316267edd
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 0%

---

# 검색, 소셜 및 Commerce의 [!DNL Google Ads] 전환 데이터

Search, Social 및 Commerce은 보고와 최적화를 위해 [!DNL Google Ads] 검색 및 쇼핑 네트워크의 모든 캠페인에 대한 [!DNL Google Ads] 추적 전환 데이터를 Search, Social 및 Commerce에 자동으로 동기화합니다.

모든 지표는 캠페인 관리 보기 및 기본 보고서에서 자동으로 사용할 수 있으며 최적화를 위한 포트폴리오 목표에서도 사용할 수 있습니다.

## 사용 가능한 전환 데이터

검색, 소셜 및 Commerce은 &quot;[!DNL Include in 'Conversions']&quot; 옵션이 활성화된 전환에 대한 데이터를 동기화하여 지난 35일 동안 데이터를 가져온 다음 광고주의 시간대에서 매일 09:00-10:00까지 변경 사항을 가져옵니다. 각 클릭에 대해 새로운 전환이 추적되므로 내역 데이터가 매일 변경될 수 있습니다.

[[!DNL Google Ads]에서 추적된 각 전환](https://support.google.com/google-ads/answer/4677036)&#x200B;([!DNL Google Ads]에서 설정됨)에 대해 최대 3개의 지표를 [!DNL Google Ads]에 구성된 전환 이름을 사용하여 검색, 소셜 및 Commerce에서 자동으로 사용할 수 있습니다. 각 전환에 대한 지표는 다음과 같습니다.

<!--

* `<conversion-name>` &mdash; (When you track it) The conversion value for the keyword, beginning with the "GGL" prefix (such as GGL Purchase).

`CT_<conversion-name>` &mdash; The number (count) of conversions, beginning with the "GGL_CT" prefix (such as GGL_CT_Purchase).

* `XD_<conversion-name>` &mdash; (When available for the conversion type, when you track them) The number (count) of cross-device conversions, as measured by Google, beginning with the "GGL_XD_CT_" prefix (such as GGL_XD_CT_Purchase).

-->

* `GGL*` — (추적할 때) &quot;GGL&quot; 접두사로 시작하는 키워드에 대한 전환 값(예: GGL 구매)입니다.

* `GGL_CT*` — &quot;GGL_CT&quot; 접두사로 시작하는 전환 수(개수)(예: GGL_CT_Purchase).

* `GGL_XD_CT*` — (전환 유형에 사용 가능한 경우, 추적할 때) &quot;GGL_XD_CT_&quot; 접두사로 시작하는 Google에서 측정한 교차 장치 전환 수(개수)입니다(예: GGL_XD_CT_Purchase).

[!DNL Google Ads]은(는) [입찰 단위](/help/search-social-commerce/glossary.md#a-b), 장치 및 클릭 날짜별로 각 전환을 기록합니다(전환 날짜 아님). 속성은 [!DNL Google Ads]의 각 지표에 대한 기본 속성 설정을 기반으로 합니다. 클릭 이벤트 수준 데이터를 사용할 수 없으므로 Adobe Advertising 속성은 팩토링되지 않습니다.

>[!NOTE]
>
>* 전환 이름이 동일한 계정이 여러 개 있는 경우 Adobe Advertising에 중복 전환 이름이 표시될 수 있습니다. 이 경우 [!UICONTROL Admin] > [!UICONTROL Conversions]에서 중복 지표 중 하나에 대한 [표시 이름을 변경](/help/search-social-commerce/admin/conversion-metrics/conversion-metric-edit-display-name.md)합니다. 두 개의 서로 다른 지표에 동일한 이름이 있을 때는 보고가 정확하지 않습니다.
>* 입찰 단위 수준의 데이터가 동일한 수준의 [!DNL Google Ads]의 데이터와 일치합니다. 그러나 상위 수준에 대한 [!DNL Google Ads]의 자체 전환 데이터에는 하위 입찰 단위에 귀속되지 않는 추가 전환이 포함될 수 있습니다. 검색, 소셜 및 Commerce의 데이터는 항상 입찰 단위 수준에서 롤업되므로, 예를 들어 캠페인 수준 보고서의 합계는 Google 광고의 캠페인 수준 보고서와 동일하지 않을 수 있습니다.
>* 데이터 분산은 일반적으로 추가 전환이 아직 동기화되지 않은 날의 후반보다 오전 동기화 후에 더 적습니다. 오전에 데이터의 유효성을 검사하는 것이 좋습니다.
>* [!DNL Google Display Network], [!DNL Gmail], [!DNL Mobile App] 및 [!DNL YouTube] 광고에 전환 데이터를 사용할 수 없습니다. [!DNL Google Ads]의 데이터와 검색, 소셜 및 Commerce의 데이터를 비교할 때 이러한 유형의 광고를 필터링합니다.
>* [!DNL Google Ads] 전환에 대한 데이터는 대상 또는 지리적 위치 수준에서 사용할 수 없으므로 RLSA 및 위치 입찰 조정을 자동으로 최적화하는 데 사용되지 않습니다.

## [!DNL Google Ads]의 전환 데이터를 검색, 소셜 및 Commerce의 데이터와 비교하는 방법

검색, 소셜 및 Commerce의 데이터를 [!DNL Google Ads]의 데이터와 비교하는 경우 보기 또는 보고서 옵션을 사용하여 트랜잭션 날짜가 아닌 클릭 날짜를 기준으로 전환을 봅니다.

다음 보고서 설정을 사용하여 비교 가능한 데이터의 유효성을 검사합니다.

### [!DNL Google Ads]에서 사용할 보고서 설정

선택한 전환 작업에 대한 보고서를 일별로 생성하고 모든 광고 상태에 대한 데이터를 포함하십시오.

<!-- 

1. In the main toolbar, select **[!DNL Reports] > [!DNL Report]**.

1. Select **[!DNL + Custom] > [!DNL Table]**.

1. From the left pane, specify the rows and columns in the report:
   
   1. Search for the **[!DNL Day]** field and it drag to the [!DNL Row] section.

   1. Search for the **[!DNL All conv].** field and it drag to the [!DNL Column] section.

   1. Search for the **[!DNL Conversion action]** field and it drag to the [!DNL Column] section.

1. In the report settings toolbar, select **[!DNL Filter] > [!DNL Ad status]**, and then select all boxes.

1. In the report settings toolbar, select **[!DNL Download] > [!DNL Excel .csv]**.

-->

### 검색, 소셜 및 Commerce에서 사용할 보고서 설정

검색, 소셜 및 Commerce에서 보기 또는 보고서 옵션을 사용하여 클릭 날짜(트랜잭션 날짜가 아님)를 기반으로 전환을 봅니다.

1. 메인 메뉴에서 **[!UICONTROL Search, Social, & Commerce]> [!UICONTROL Insights & Reports] >[!UICONTROL Reports]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL Create Report]**&#x200B;을 클릭하고 **[!UICONTROL Basic Reports]** 위에 커서를 놓은 다음 **[!UICONTROL Search Engine Account Report]**&#x200B;을 클릭합니다.

1. [!UICONTROL Report Settings] 창에서 다음 보고서 설정을 지정합니다.

   1. 섹션의 **[!UICONTROL Conversions Based]**&#x200B;에서 **[!UICONTROL Click date]**&#x200B;을(를) 선택합니다.

   1. [!DNL Google Ads] 보고서에 사용한 날짜 범위와 동일한 날짜 범위를 지정하십시오.

   1. **[!UICONTROL Search/Content]** 섹션에서 **[!UICONTROL Search Only]**&#x200B;을(를) 선택합니다.

   1. **[!UICONTROL Search Engine Hierarchy]** 섹션에서 [!UICONTROL Google Adwords] 섹션을 확장하고 계정을 선택합니다.

   1. [!UICONTROL Columns] 탭을 열고 비교할 [!DNL Google Ads] 지표(&quot;GGL&quot;로 시작)를 추가합니다.

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [광고 네트워크 계정 및 캠페인 구현 개요](campaign-implemention-overview.md)
>* [광고 네트워크 캠페인의 성능 모니터링 및 관리](monitor-performance-campaigns.md)
>* [광고주에 대해 추적된 전환 지표를 봅니다](/help/search-social-commerce/admin/conversion-metrics/conversion-metric-view-tracked.md)
>* [변환 태그 만들기 [!DNL Google Ads]](/help/search-social-commerce/admin/conversion-metrics/conversion-tag-google.md)
>* [향상된 전환을 위해 오프라인 전환 데이터 업로드](/help/search-social-commerce/admin/conversion-metrics/upload-data-offline-conversions.md)
