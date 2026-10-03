---
title: '[!UICONTROL Google AI Max Search Term Combination Report]'
description: '[!UICONTROL Google AI Max Search Term Combination Report]에 대해 알아봅니다.'
feature: Search Reports, Search Specialty Reports
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: 9166e3e1-13c1-5edf-bc2a-c6e22231df68
    internal-label: Search Reports
  - id: 7de556b7-2c2a-599d-853b-8c282aafa6e3
    internal-label: Search Specialty Reports
source-git-commit: 6d95caf72d11c404d866e8d091e1ffa89814ae73
workflow-type: tm+mt
source-wordcount: '310'
ht-degree: 0%
---
# [!UICONTROL Google AI Max Search Term Combination Report]

*AI 최대값에만 캠페인이 활성화된 [!DNL Google Ads] 계정에 적용 가능*

[!UICONTROL Google AI Max Search Term Combination Report]은(는) 특정 검색 쿼리가 AI가 생성한 헤드라인, 동적 랜딩 페이지 및 지정된 계정 내의 [!DNL Google Ads AI Max] 사용 캠페인에 있는 광고에 대한 전환 작업에 매핑되는 방법을 보여 줍니다. 이 보고서에는 다음 두 개의 시트가 포함됩니다.

* [!UICONTROL AI Max Search Term]장: 검색 네트워크 내의 검색을 기반으로 하는 특정 광고 조합 및 랜딩 페이지의 성능입니다. 시트에는 노출, 클릭 수 및 비용 데이터뿐만 아니라 보고서 설정에 지정된 선택적 [!DNL Google Ads] 추적 전환 지표가 포함됩니다. 기본적으로 데이터에는 지정된 데이터 범위에서 하나 이상의 노출을 받은 각 검색어, 헤드라인 및 랜딩 페이지 조합에 대한 하나의 행이 포함됩니다. 행은 기본적으로 캠페인에 의해 오름차순으로 정렬되며 선택한 다른 열에 의해 정렬됩니다.

  이 시트를 사용하여 강력한 부정적 키워드 목록을 빌드할 수 있도록 쿼리당 결과 광고 요소의 성능 및 의도를 분석합니다.

* <!-- [!UICONTROL Search Term x Conversion Action] sheet? -->[!UICONTROL AI Max Search Term #1] 시트: [!DNL Google Ads]에서 각 검색어와 일치 유형에 대한 전환 작업별로 전환 데이터를 추적했습니다. 각 행에는 전환 작업, 전환 수 및 전환 값과 보고서 설정에 지정된 기타 선택적 [!DNL Google Ads] 추적 전환 지표가 포함됩니다. 기본적으로 데이터에는 지정된 데이터 범위에서 각 검색어와 전환 작업 조합에 대한 하나의 행이 포함됩니다. 행은 첫 번째 시트의 행과 순서가 같습니다.

  <!-- Should it be this?  The sheet includes the number of conversions and the conversion value, all conversions and the all conversions value, and cross-device conversions. -->

  이 시트를 사용하여 각 검색어가 전환 작업으로 파생된 전환을 유도하는 방법을 이해합니다.

<!-- We're pulling data directly from GGL and not storing it, so no limitations on our end WRT date range. -->

## 기본 열

모든 기본 및 사용자 지정 열에 대한 설명은 &quot;[특성 보고서에 대한 보고서 열](specialty-report-columns.md)&quot;을 참조하십시오.

<!-- VERIFY -- probably more will be included by default -->

* [!UICONTROL Event Date]
* [!UICONTROL Account Name]
* [!UICONTROL Network Campaign ID]
* [!UICONTROL Campaign Name]
* [!UICONTROL Ad Group Name]
* [!UICONTROL Search Term]
* [!UICONTROL Headline 1]
* [!UICONTROL Headline 2]
* [!UICONTROL Landing Page]
* [!UICONTROL Impressions]
* [!UICONTROL Clicks]
* [!UICONTROL Cost]
* [!UICONTROL Conversion Action]&#x200B;(명시적으로 포함하지 않더라도 [!UICONTROL AI Max Search Term #1] 시트에 자동으로 포함됨)
* [!UICONTROL Conversions]&#x200B;(명시적으로 포함하지 않더라도 [!UICONTROL AI Max Search Term #1] 시트에 자동으로 포함됨)
* [!UICONTROL Conversions Value]&#x200B;(명시적으로 포함하지 않더라도 [!UICONTROL AI Max Search Term #1] 시트에 자동으로 포함됨)

>[!MORELIKETHIS]
>
>* [전문 보고서 정보](specialty-report-about.md)
>* [예약된 보고서 관리](/help/search-social-commerce/new-ui/reports/management/report-manage.md)
>* [특성 보고서 설정](specialty-report-settings.md)
>* 특성 보고서에 대한 [보고서 열](specialty-report-columns.md)
