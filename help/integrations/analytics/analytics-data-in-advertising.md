---
title: Adobe Advertising의 [!DNL Analytics] 데이터
description: Adobe Advertising의 [!DNL Analytics] 데이터
feature: Integration with Adobe Analytics
exl-id: e11b0617-44e3-4f28-a065-aa9f6cf3eb5d
source-git-commit: 73cdb171523b55f48b5ae5c5b2b4843f542336a6
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---

# Adobe Advertising의 [!DNL Analytics] 데이터

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

## Analytics 세그먼트

[!DNL Analytics]에서 만들어 Experience Cloud에 게시한 모든 세그먼트.

새 세그먼트가 Adobe Advertising에 표시되는 데 24-48시간이 소요됩니다. 기존 세그먼트에 대한 업데이트는 약 8시간 이내에 동기화됩니다.

<!-- I added "metric" to some of the links below, even though it looks redundant, because of syntax limitations: If you use [!DNL] or [!UICONTROL] as the sole text of a link (such as [[!UICONTROL Revenue]], the tag is included in the link text (such as "[!UICONTROL Revenue]") when it's published. -->

## 사이트 참여 지표

>[!NOTE]
>
>* [!DNL Analytics]이(가) EF ID [!DNL eVar]에 대한 이벤트를 Adobe Advertising에 전달합니다.  기본 통합은 계산된 지표 또는 다른 차원([!DNL eVars])을 Adobe Advertising으로 보내는 것을 지원하지 않습니다. 그러나 계산된 지표를 사용자 지정 이벤트에서 완전히 캡처할 수 있는 경우 Adobe Advertising은 사용자 지정 이벤트를 수집할 수 있습니다.
>* [!DNL Analytics]이(가) 매시간 Adobe Advertising에 데이터를 전달합니다.

* [!UICONTROL Timespent_secs_1stvisit]: 방문자가 처음 방문하는 동안 사이트에서 보낸 시간(초)입니다.
* [!UICONTROL Timespent_secs_total]: 전환 확인 기간 내의 모든 방문에서 사이트에서 보낸 총 시간(초)입니다.
* [!UICONTROL Pageviews_1stvisit]: 방문자가 처음 방문하는 동안 사이트에 대한 페이지 보기 수입니다.
* [!UICONTROL Pageviews_total]: 전환 확인 기간 내에 있는 모든 방문에 대한 사이트의 총 페이지 보기 수입니다.
* [[!UICONTROL Bounces] 지표](https://experienceleague.adobe.com/docs/analytics/components/metrics/bounces.html)
* [[!UICONTROL Visits] 지표](https://experienceleague.adobe.com/docs/analytics/components/metrics/visits.html)
* [!UICONTROL ef_id_instances]: [!DNL Analytics]에서 [!UICONTROL EF ID]을(를) 수집한 횟수입니다.

## 전환 지표

[!DNL Analytics]이(가) 전환 지표를 매일 Adobe Advertising에 전달합니다.

### 표준 전환 지표

* [[!UICONTROL Revenue] 지표](https://experienceleague.adobe.com/docs/analytics/components/metrics/revenue.html)
* [[!UICONTROL Orders] 지표](https://experienceleague.adobe.com/docs/analytics/components/metrics/orders.html)
* [[!UICONTROL Units] 지표](https://experienceleague.adobe.com/docs/analytics/components/metrics/units.html)
* [[!UICONTROL Carts] 지표](https://experienceleague.adobe.com/docs/analytics/components/metrics/carts.html)
* [[!UICONTROL Cart Views] 지표](https://experienceleague.adobe.com/docs/analytics/components/metrics/cart-views.html)
* [[!UICONTROL Checkouts] 지표](https://experienceleague.adobe.com/docs/analytics/components/metrics/checkouts.html)
* [[!UICONTROL Cart Additions] 지표](https://experienceleague.adobe.com/docs/analytics/components/metrics/cart-additions.html)
* [[!UICONTROL Cart Removals] 지표](https://experienceleague.adobe.com/docs/analytics/components/metrics/cart-removals.html)

### 사용자 지정 전환 지표

이러한 지표는 보고서 세트마다 다르므로 사용 가능한 지표는 각 고객 및 보고서 세트에 따라 다릅니다.

### [!DNL eVars] 및 [!DNL Props]에서 만든 사용자 지정 전환 지표

사용 가능한 지표는 고객마다 다릅니다. &quot;[Adobe Analytics에서 전환 지표 만들기 [!DNL eVars] 및 [!DNL Props]](/help/integrations/analytics/conversion-metrics-from-evars.md)&quot;를 참조하십시오.

### 예약된 전환 지표

이러한 지표는 보고서 세트마다 다르므로 사용 가능한 지표는 각 고객 및 보고서 세트에 따라 다릅니다.

>[!MORELIKETHIS]
>
>* [개요 [!DNL Analytics for Advertising]](overview.md)
>* Analysis Workspace의 [Adobe Advertising 지표](/help/integrations/analytics/advertising-metrics-in-analytics.md)
