---
title: DSP에서 광고주의 전환 지표를 관리합니다.
description: Adobe Advertising이 DSP 광고주에게 추적하는 전환 지표를 사용하는 방법을 알아봅니다.
feature: Conversions
source-git-commit: e2746d58fa512f032a1e4ff851d23876cd63fc93
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---

# 광고주의 전환 지표 관리

광고주의 전환 지표는 Adobe Advertising 전체에서 사용됩니다.

* Advertising DSP에서는 캠페인 관리 보기, 사용자 지정 목표 및 사용자 지정 보고서에 전환 지표를 포함할 수 있습니다. 또한 광고주의 전환 지표를 사용하여 패키지를 최적화하는 데 사용되는 [사용자 지정 목표](/help/dsp/admin/custom-objectives-manage.md)를 만들 수도 있습니다.

* (Advertising 검색, 소셜 및 Commerce을 사용하는 광고주) 검색, 소셜 및 Commerce에서 전환 지표에 대한 데이터를 캠페인, 포트폴리오 및 목표 관리 보기의 열과 보고서에 표시할 수 있습니다. 충분한 액세스 권한이 있는 사용자는 전환 지표를 사용하여 목표를 만들 수도 있습니다. 목표는 포트폴리오를 최적화하는 데 사용됩니다.

<!--
The conversion metrics that Adobe Advertising tracks for an advertiser &mdash; including [conversion and site engagement metrics synced from Adobe Analytics](/help/integrations/analytics/analytics-data-in-advertising.md), [site events synced from Adobe Customer Journey Analytics](/help/integrations/customer-journey-analytics/overview.md), and custom feeds &mdash; are used throughout Advertising DSP. You can include conversion metrics in campaign management views, custom objectives, and custom reports. You can also use conversion metrics to create [custom objectives](/help/dsp/admin/custom-objectives-manage.md), which are used to optimize packages.

By default, none of an advertiser's conversion metrics are available for campaign management views, custom objectives, and reports. They are available only when you specifically make them available. When you make a conversion metric available, you can either use the metric name exactly as it is spelled in the retrieved data or change the display name that's shown in column headings for readability.

From the list of visible metrics, each user with access to the advertiser's data can customize the metrics they see for campaign management views, objectives, and reports by including or omitting specific metrics. Users with sufficient access privileges can also optimize for specific metrics by associating them with DSP package-level custom goals.

-->

DSP 사용자에 대해 추적되는 지표 유형은 다음과 같습니다.

* Adobe Advertising이 광고주를 위해 추적하는 전환 지표입니다.

* [전환 및 사이트 참여 지표가 Adobe Analytics에서 동기화됨](/help/integrations/analytics/analytics-data-in-advertising.md).

* [사이트 이벤트가 Adobe Customer Journey Analytics에서 동기화됨](/help/integrations/customer-journey-analytics/overview.md).

* 사용자 지정 피드의 전환.

사용 가능한 전환 지표 목록에서 광고주의 데이터에 대한 액세스 권한이 있는 각 사용자는 특정 지표를 선택하거나 생략하는 등 관리 보기 및 보고서에 사용할 수 있는 지표를 사용자 지정할 수 있습니다. 검색된 데이터의 맞춤법과 정확히 동일한 지표 이름을 사용하거나 가독성을 위해 열 제목에 표시되는 이름을 변경할 수 있습니다.

>[!IMPORTANT]
>
>기본적으로 광고주의 전환 지표는 캠페인 관리 보기, 사용자 지정 목표 및 사용자 지정 보고서에 포함할 수 없습니다. 전환 지표를 사용할 수 있도록 하려면 전환 지표를 명시적으로 사용할 수 있도록 해야 합니다.

>[!TIP]
>
>광고주(또는 광고 네트워크)가 전환 지표의 수집을 중지하면 내역 데이터를 보는 데 사용하지 않으려면 [관리 보기 및 보고서에서 해당 지표를 숨기십시오](#conversion-metrics-change-available).

## 광고주에 대해 추적된 전환 지표 보기

* 메인 메뉴에서 **[!UICONTROL Settings]>[!UICONTROL Conversions Beta]**&#x200B;을(를) 클릭합니다.

광고주를 위해 수집된 모든 전환 지표와 여기에 지정된 다른 표시 이름이 나열됩니다. 각 지표 행에는 지표의 소스가 포함됩니다.

## 전환 지표에 대한 표시 이름 변경

예를 들어, 이름이 *reg*&#x200B;인 전환 지표를 사용하여 등록 데이터를 수집하는 경우 선택적으로 표시 이름을 변경하여 &quot;등록&quot;으로 표시되도록 할 수 있습니다.

기존 표시 이름은 삭제할 수 없습니다.

1. 메인 메뉴에서 **[!UICONTROL Settings]>[!UICONTROL Conversions Beta]**&#x200B;을(를) 클릭합니다.

1. 행 위에 커서를 놓고 **[!UICONTROL Edit Display Name]**&#x200B;을(를) 클릭합니다.

1. 표시할 이름을 입력한 다음 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

   표시 이름은 고유해야 하며 다음 특수 문자를 포함할 수 없습니다. `\"<'>&`

## 캠페인 관리 보기, 사용자 정의 목표 및 사용자 정의 보고서에서 사용할 수 있는 전환 지표 변경 {#change-the-conversion-metrics-available-in-ui}

1. 메인 메뉴에서 **[!UICONTROL Settings]>[!UICONTROL Conversions]**&#x200B;을(를) 클릭합니다.

   광고주를 위해 수집된 모든 전환 지표와 표시를 위해 지정된 다른 이름이 나열됩니다.

1. (선택 사항) 목록을 필터링합니다.

   1. 목록 위에서 ![필터](/help/dsp/assets/filter.png "필터")를 클릭합니다.

   1. 필터를 지정한 다음 **[!DNL Apply]**&#x200B;을(를) 클릭합니다.

      AMO 클라이언트 ID, UI에 지표가 표시되는지 또는 숨겨지는지 여부, 데이터 소스별로 지표를 필터링할 수 있습니다.

1. 관리 보기 및 보고서에 사용할 수 있는 전환 지표를 변경합니다.

   * 지표를 표시하려면 행 위에 커서를 놓고 **[!UICONTROL Show in UI and Reports]**&#x200B;을(를) 클릭합니다.

   * 지표를 숨기려면 행 위에 커서를 놓고 **[!UICONTROL Hide in UI and Reports]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [캠페인 데이터 보기 관리](/help/dsp/campaign-management/reports/campaign-data-views-manage.md)
>* [사용자 지정 목표 관리](/help/dsp/admin/custom-objectives-manage.md)
