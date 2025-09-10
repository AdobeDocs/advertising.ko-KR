---
title: Customer Journey Analytics에서 사용하는 Adobe Advertising ID
description: Customer Journey Analytics에서 사용하는 Adobe Advertising ID
feature: Integration with Adobe Customer Journey Analytics
exl-id: af60dcb4-4d1a-4097-ac30-688bd8b9f644
source-git-commit: dede10acca1540a10699be3c14564a6f9360edd2
workflow-type: tm+mt
source-wordcount: '76'
ht-degree: 0%

---

# Customer Journey Analytics에서 사용하는 Adobe Advertising ID

*Adobe Advertising-Adobe Customer Journey Analytics 통합만 있는 광고주*

*Advertising DSP 및[!DNL Advertising Search, Social, & Commerce]*&#x200B;에 적용 가능

*Beta 기능*

Adobe Advertising에서는 현장 성능 추적에 *EF ID*&#x200B;와 *AMO ID*, 이렇게 두 개의 ID를 사용합니다.

<!-- Rewrite for CJA:

When an ad impression occurs, Adobe Advertising creates the AMO ID and EF ID values and stores them. For click-through traffic, these IDs are included in the landing page URL using the `ef_id` and `s_kwcid` (for the AMO ID) query string parameters.

Adobe Advertising distinguishes between a click-through or view-through entry to the website using the following criteria:

* A view-through entry is captured when a user visits the site after viewing an ad but not clicking it. [!DNL Analytics] or Web SDK records a view-through if two conditions are met:

    * The visitor has no click-throughs for a [!DNL DSP] or [!DNL Search, Social, & Commerce] ad during the [click lookback window](/help/integrations/analytics/prerequisites.md#lookback-a4adc).

    * The visitor has seen at least one [!DNL DSP] ad during the [impression lookback window](/help/integrations/analytics/prerequisites.md#lookback-a4adc). The last impression is passed as the view-through.

* A click-through entry is captured when a site visitor clicks an ad before entering the site. [!DNL Analytics] or Web SDK captures a click-through when either of the following conditions occurs:

    * The URL includes an EF ID and AMO ID as added to the landing page URL by Adobe Advertising.

    * The URL contains no tracking codes, but the Adobe Advertising JavaScript code detects a click within the last two minutes.

![Adobe Advertising view-based [!DNL Analytics] integration](/help/integrations/assets/a4adc-view-through-process.png)

*Figure 1: Adobe Advertising view-based [!DNL Analytics] integration*

![Adobe Advertising click URL-based [!DNL Analytics] integration](/help/integrations/assets/a4adc-click-through-process.png)

*Figure 2: Adobe Advertising click URL-based [!DNL Analytics] integration*

-->

<!-- ## Adobe Advertising EF IDs {#ef-id} -->

{{$include /help/_includes/ef-id.md}}

<!-- ## Adobe Advertising AMO IDs {#amo-id} -->

{{$include /help/_includes/amo-id.md}}

<!-- rewrite for CJA:

### AMO ID Dimension in [!DNL Customer Journey Analytics]

In Analytics reports, you can find AMO ID data by searching for the [!UICONTROL AMO ID] dimension and using the [!UICONTROL AMO ID Instances] metric. The [!UICONTROL AMO ID] dimension houses all AMO ID values captured, whereas the [!UICONTROL AMO ID Instances] metric indicates how often an AMO ID value was captured by the site. For example, if the same search ad was clicked four times but Analytics tracked seven site entries, then [!UICONTROL AMO ID Instances] would be seven (7) and [!UICONTROL Clicks] would be four (4).

For any reporting or auditing within [!DNL Analytics], the best practice is to use the AMO ID along with its corresponding instance. For more information, see "[Click-Through Data Validation for [!DNL Analytics for Advertising]](data-variances.md#data-validation)" in "Expected Data Variances Between [!DNL Analytics] and Adobe Advertising."

-->

>[!MORELIKETHIS]
>
>* [개요](overview.md)
>* [필수 구성 요소](prerequisites.md)
>* [데이터 수집, 데이터 전송 및 보고 설정](set-up.md)
>* [Customer Journey Analytics의 Adobe Advertising 지표 및 차원](advertising-data-in-cja.md)
