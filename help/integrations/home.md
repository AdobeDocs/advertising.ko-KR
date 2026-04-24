---
title: 새로운 기능
description: Adobe Advertising과 Adobe CX Enterprise(이전 Adobe Experience Cloud)의 다른 제품 및 서비스 간의 통합 업데이트에 대해 알아봅니다.
cloud: Experience Cloud
product: advertising cloud
index: true
exl-id: e5874077-d2a8-43bb-ad4e-55547442c8a4
TQID: https://experienceleague.adobe.com/6-dzP-cjgKB5-HBvIpy8iU3B8FEbWAfP8r5UEad23Ok
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2:
  - id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
  - id: f2860a4b-f905-4545-bead-1bbc92564592
subfeature_v2:
  - id: d1e2786d-1070-4f97-93d7-f5b95de25b2b
  - id: d9510790-d834-436d-8423-8d69cd50464a
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: d3cdead0-685a-4489-9250-4bb709942f66
source-git-commit: c4d69b3aac9c963d13e3083f71931e507e58e616
workflow-type: tm+mt
source-wordcount: 870
ht-degree: 0%

---

# 새로운 기능

다음 기능은 새로운 기능이거나 최근에 변경되었습니다.

| 날짜 | 기능 | 설명 | 추가 정보 |
| ---- | ------- | ----------- | -------------------- |
| 2025년 9월 8일 | Customer Journey Analytics과 통합 | (Beta 기능) [!DNL Analytics for Advertising]이(가) 아닌 Customer Journey Analytics을 사용하는 광고주는 이제 [Adobe Experience Platform [!DNL Web SDK]](https://experienceleague.adobe.com/docs/experience-platform/edge/home.html)을(를) 사용하여 Adobe Advertising과 Customer Journey Analytics 간에 기본적으로 데이터를 교환할 수 있습니다. | &quot;[Adobe Advertising과 Customer Journey Analytics 간의 통합 개요](/help/integrations/customer-journey-analytics/overview.md)&quot;를 참조하십시오. |
| 2025년 3월 26일 | [!DNL Adobe Analytics for Advertising] | (Search, Social 및 Commerce이 있는 광고주; [!DNL Microsoft Advertising] 계정; [!DNL Adobe Analytics for Advertising]) 추적 옵션이 [!UICONTROL Auto Upload]인 계정의 경우, 모든 캠페인 유형에 대한 랜딩 페이지 접미사에 있는 AMO ID 매개 변수의 형식이 최신 형식으로 업데이트되었습니다. 이전에는 대부분의 계정에 대한 성과 최대 캠페인이 새 형식으로 마이그레이션되었습니다.<br><br>아직 새 형식으로 마이그레이션되지 않은 [!UICONTROL Auto Upload] 추적 옵션이 없는 계정의 경우 새 AMO ID 형식을 포함하도록 각 랜딩 페이지 접미사를 수동으로 업데이트해야 합니다.<br><br>현재 형식: `s_kwcid=AL!{userid}!10!{AdId}!!!!{OrderItemId}!!{CampaignId}!{AdGroupId}` | &quot;[개요 [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md)&quot; 및 [AMO ID 형식](https://experienceleague.adobe.com/en/docs/analytics/components/dimensions/amo-id#dimension-items)을(를) 참조하십시오.&quot; |
| 2024년 11월 13일 | [!DNL Analytics for Advertising] | ([!DNL Analytics for Advertising] 및 Adobe Customer Journey Analytics이 있는 광고주) 예약된 변수를 사용하여 AMO ID 및 EF ID를 캡처하는 경우 가능한 한 빨리 AMO ID 및 EF ID에 대한 예약된 변수를 표준 [!DNL eVars]에 복사하여 Adobe Advertising과 Adobe Customer Journey Analytics 간의 향후 통합을 준비할 수 있습니다. 이를 통해 작업을 완료하는 즉시 AMO ID 및 EF ID에 대한 내역 데이터를 수집할 수 있으며 내역 데이터는 나중에 사용할 수 있습니다. Your Adobe Account Team will let you know if you use reserved variables and need to complete this task. | See &quot;[Collect historical data for AMO IDs and EF IDs for use in Adobe Customer Journey Analytics](/help/integrations/analytics/rvars-to-evars.md).&quot; |
| Released 29 October 2024 | [!DNL Adobe Analytics for Advertising] | (성과 최대 캠페인 [!DNL Adobe Analytics for Advertising] 및 [!DNL Microsoft Advertising]개를 사용하는 광고주) 이제 광고와 키워드가 포함되지 않은 성과 최대 캠페인의 추적 URL에서 새 AMO ID([!DNL s_kwcid]) 매개 변수를 구현할 때 성과 최대 캠페인에 대한 자산 그룹 수준 데이터를 Adobe Analytics에서 사용할 수 있습니다. 성과 최대 캠페인이 있는 대부분의 계정에 대한 추적이 이미 새 형식으로 마이그레이션되었습니다. [!UICONTROL Auto Upload] 추적 옵션이 없는 성과 최대 캠페인이 이미 새 형식으로 마이그레이션되지 않은 계정의 경우, 새 AMO ID 형식을 포함하도록 각 랜딩 페이지 접미사를 수동으로 업데이트해야 합니다.<br><br>Adobe Analytics data for your performance max campaigns is also available in Search, Social, &amp; Commerce. | See the new [AMO ID format](https://experienceleague.adobe.com/en/docs/analytics/components/dimensions/amo-id#dimension-items) and [when and how to add the parameter to your tracking URLs](/help/integrations/analytics/ids.md). |
| 16 December 2023 | Help | A new document explains how to set up A/B tests in [!DNL Target] for click-through traffic from ads in Search, Social, &amp; Commerce, as well as tips on how to measure and visualize your tests in [!DNL Analytics]. | See &quot;[Configure A/B tests in Adobe Target for Search, Social, &amp; Commerce ads](/help/integrations/target/ab-tests-search.md).&quot; |
| 8 August 2023 | [!DNL Analytics for Advertising] | Some [!DNL Analytics] success event metrics, including standard, custom, and reserved conversion metrics and traffic metrics, are automatically available in DSP and in Search, Social, &amp; Commerce. Now, you now can also configure your own success metrics based on your existing [!DNL Analytics] [!DNL eVars] and [!DNL props] by funneling [!DNL eVar]- and [!DNL prop]-level data into a custom success event. | See &quot;[Create Conversion Metrics from Adobe Analytics [!DNL eVars] and [!DNL Props]](/help/integrations/analytics/conversion-metrics-from-evars.md).&quot; |
| 13 July 2023 | Reporting | (DSP users with [!DNL Analytics for Advertising]) View-through conversions for connected TV (CTV) placements are now included in conversion data available within Adobe Analytics. | See the section on &quot;Examples of How to Use the Integration&quot; in &quot;[Overview of [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md#integration-examples).&quot; |
| 1 November 2022 | Help | A new document explains how to implement click-through and view-through signal sharing between Advertising DSP and Adobe Target, set up an A/B test activity in [!DNL Target] for your DSP ads, and how to set up Adobe Analytics Analysis Workspace to view the test data. | See &quot;[Configure A/B tests in Adobe Target for Advertising DSP ads](/help/integrations/target/ab-tests-dsp.md).&quot; |
| 17 August 2022 | 도움말 | 새 장에서는 Adobe Advertising을 Adobe Audience Manager과 통합하는 모든 방법을 설명합니다. | &quot;[Adobe Audience Manager과 Adobe Advertising 통합](/help/integrations/audience-manager/overview.md)&quot;에 대한 개요를 포함하여 &quot;Adobe Audience Manager과 통합&quot; 장을 참조하십시오. |
| 2021년 4월 27일 | [!DNL Analytics for Advertising] | 클릭 데이터를 Adobe Analytics으로 보내기 위해 [!DNL Analytics for Advertising] 매크로를 [!DNL Google Campaign Manager 360] 광고 태그에 추가하는 이유와 방법을 알아봅니다. | &quot;[추가 [!DNL Analytics for Advertising] 매크로를  [!DNL Google Campaign Manager 360] 광고 태그](/help/integrations/analytics/macros-google-campaign-manager.md)에 추가&quot;를 참조하십시오.&quot; |
| 2021년 4월 19일 | [!DNL Analytics for Advertising] | 매크로를 [!DNL Flashtalking] 광고 태그에 추가하여 클릭 데이터를 Adobe Analytics으로 보내는 방법과 방법에 대해 알아봅니다. | &quot;[추가 [!DNL Analytics for Advertising] 매크로를  [!DNL Flashtalking] 광고 태그](/help/integrations/analytics/macros-flashtalking.md)에 추가&quot;를 참조하십시오.&quot; |
| 2021년 10월 27일 | [!DNL Analytics for Advertising] | 조직이 데이터 수집을 위해 기존 Adobe Analytics `visitorAPI.js` 라이브러리에서 [Adobe Experience Platform [!DNL Web SDK]](https://experienceleague.adobe.com/docs/experience-platform/edge/home.html) 라이브러리(`alloy.js`)로 전환하려는 경우 일부 내용을 변경하여 ID 결합을 사용하도록 설정해야 합니다. | &quot;[Adobe Experience Platform과 함께  [!DNL Last Event Service] JavaScript 라이브러리 사용 [!DNL Web SDK]](/help/integrations/analytics/web-sdk.md)&quot;을(를) 참조하십시오. |
| 2021년 5월 26일 | 도움말 | 이제 &quot;[!DNL Analytics for Advertising]&quot; 장에 &quot;Working in [!DNL Analytics Marketing Channels]&quot;에 대한 하위 챕터가 포함됩니다. | &quot;[처리 규칙 기본 사항 [!DNL Marketing Channels]](/help/integrations/analytics/marketing-channels/mc-overview.md)," "[&#128279;](/help/integrations/analytics/marketing-channels/mc-ids.md)Using Adobe Advertising IDs to create [!DNL Marketing Channels] 2&rbrace;&quot;, &quot;[Adobe Advertising 데이터 사용 [!DNL Analytics Marketing Channels] &quot;, &quot;](/help/integrations/analytics/marketing-channels/mc-ac-data.md)&quot; 및 &quot;[Adobe Advertising과  [!DNL Marketing Channels]](/help/integrations/analytics/marketing-channels/mc-data-variances.md) 간에 채널 데이터가 다를 수 있는 이유&quot;를 참조하십시오.&quot; |
| 2021년 5월 26일 | 도움말 | [!DNL Analytics for Advertising]에 대한 모든 비디오 튜토리얼에 대한 링크가 추가되었습니다. | &quot;[Adobe Advertising 통합에 대한 비디오 튜토리얼](https://experienceleague.adobe.com/docs/advertising-learn/tutorials/overview.html)&quot;을(를) 참조하십시오. |

{style="table-layout:auto"}

<!--
 At some point, just make this an overview page instead?

Adobe Advertising is integrated with the following Adobe CX Enterprise products:

* [Adobe Analytics](/help/integrations/analytics/overview.md)

* Adobe Audience Manager

* Adobe Campaign (Adobe Advertising Search only)

 -->
