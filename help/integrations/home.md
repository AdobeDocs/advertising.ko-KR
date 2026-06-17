---
title: 새로운 기능
description: Adobe Advertising CX Enterprise(이전 Adobe Experience Cloud)의 Adobe과 기타 제품 및 서비스 간의 통합 업데이트에 대해 알아봅니다.
cloud: Experience Cloud
product: advertising cloud
index: true
exl-id: e5874077-d2a8-43bb-ad4e-55547442c8a4
TQID: 'https://experienceleague.adobe.com/6-dzP-cjgKB5-HBvIpy8iU3B8FEbWAfP8r5UEad23Ok'
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2:
  - id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
  - id: f2860a4b-f905-4545-bead-1bbc92564592
  - id: aed5e38a-3e62-42fa-8d16-cd080729b2a0
  - id: d0d9f2ed-c163-44e1-97a1-4ace121416b8
subfeature_v2:
  - id: d1e2786d-1070-4f97-93d7-f5b95de25b2b
  - id: c3eaaeae-eb91-4543-a4dd-99c59c76fbda
  - id: c200bb82-3e43-4606-9aba-5cab31617ba0
  - id: cfd751d4-ee56-4323-8fd1-dc174b031709
  - id: ea6cf12e-f4da-4e2b-a9c1-e64da280b6f3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: a93c33ee47bd1a8df137a69598b367e985def4ee
workflow-type: tm+mt
source-wordcount: 1006
ht-degree: 0%

---

# 새로운 기능

다음 기능은 새로운 기능이거나 최근에 변경되었습니다.

| 날짜 | 기능 | 설명 | 추가 정보 |
| ---- | ------- | ----------- | -------------------- |
| 2026년 6월 9일 | Adobe Customer Journey Analytics과 통합 | [!DNL Analytics for Advertising]이(가) 아닌 Customer Journey Analytics을 사용하는 광고주는 기본적으로 Adobe Experience Platform [!DNL Web SDK]을(를) 사용하여 Adobe Advertising과 Customer Journey Analytics 간에 데이터를 교환할 수 있습니다. | &quot;[Adobe Advertising과 Customer Journey Analytics 간의 통합 개요](/help/integrations/customer-journey-analytics/overview.md)&quot;를 참조하십시오. |
| 2026년 6월 3일 | [!DNL Adobe Analytics for Advertising] | 이제 Advertising Creative 및 [!DNL Adobe Analytics for Advertising]을(를) 사용하는 광고주는 Adobe Analytics에서 변형 및 분기 수준 데이터를 볼 수 있습니다. [!DNL Creative] 경험에서 광고를 실행하는 데 사용되는 DSP에 관계없이 데이터가 표시됩니다. Advertising DSP 배치에서 광고를 실행하는 경우 캠페인 및 배치 수준 데이터뿐만 아니라 비용 관련 지표도 표시됩니다.<br><br>추가 설정이 필요하지 않습니다. | [!DNL Analytics]에 표시되는 Advertising Creative [트래픽 지표](https://experienceleague.adobe.com/ko/docs/analytics/components/metrics/amo-metrics) 및 [분류](https://experienceleague.adobe.com/ko/docs/analytics/components/dimensions/amo-id#classifications)을(를) 참조하십시오. |
| 2025년 9월 8일 | Customer Journey Analytics과 통합 | (Beta 기능) [!DNL Analytics for Advertising]이(가) 아닌 Customer Journey Analytics을 사용하는 광고주는 이제 [Adobe Experience Platform [!DNL Web SDK]](https://experienceleague.adobe.com/docs/experience-platform/edge/home.html?lang=ko)을(를) 사용하여 Adobe Advertising과 Customer Journey Analytics 간에 기본적으로 데이터를 교환할 수 있습니다. | &quot;[Adobe Advertising과 Customer Journey Analytics 간의 통합 개요](/help/integrations/customer-journey-analytics/overview.md)&quot;를 참조하십시오. |
| 2025년 3월 26일 | [!DNL Adobe Analytics for Advertising] | (Search, Social 및 Commerce이 있는 광고주; [!DNL Microsoft Advertising] 계정; [!DNL Adobe Analytics for Advertising]) 추적 옵션이 [!UICONTROL Auto Upload]인 계정의 경우, 모든 캠페인 유형에 대한 랜딩 페이지 접미사에 있는 AMO ID 매개 변수의 형식이 최신 형식으로 업데이트되었습니다. 이전에는 대부분의 계정에 대한 성과 최대 캠페인이 새 형식으로 마이그레이션되었습니다.<br><br>아직 새 형식으로 마이그레이션되지 않은 [!UICONTROL Auto Upload] 추적 옵션이 없는 계정의 경우 새 AMO ID 형식을 포함하도록 각 랜딩 페이지 접미사를 수동으로 업데이트해야 합니다.<br><br>현재 형식: `s_kwcid=AL!{userid}!10!{AdId}!!!!{OrderItemId}!!{CampaignId}!{AdGroupId}` | &quot;[개요 [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md)&quot; 및 [AMO ID 형식](https://experienceleague.adobe.com/ko/docs/analytics/components/dimensions/amo-id#dimension-items)을(를) 참조하십시오.&quot; |
| 2024년 11월 13일 | [!DNL Analytics for Advertising] | ([!DNL Analytics for Advertising] 및 Adobe Customer Journey Analytics이 있는 광고주) 예약된 변수를 사용하여 AMO ID 및 EF ID를 캡처하는 경우 가능한 한 빨리 AMO ID 및 EF ID에 대한 예약된 변수를 표준 [!DNL eVars]에 복사하여 Adobe Advertising과 Adobe Customer Journey Analytics 간의 향후 통합을 준비할 수 있습니다. 이를 통해 작업을 완료하는 즉시 AMO ID 및 EF ID에 대한 내역 데이터를 수집할 수 있으며 내역 데이터는 나중에 사용할 수 있습니다. 예약된 변수를 사용하며 이 작업을 완료해야 하는 경우 Adobe 계정 팀에 알려줍니다. | &quot;[Adobe Customer Journey Analytics에서 사용할 AMO ID 및 EF ID에 대한 내역 데이터 수집](/help/integrations/analytics/rvars-to-evars.md)&quot;을 참조하십시오. |
| 2024년 10월 29일 릴리스 | [!DNL Adobe Analytics for Advertising] | (성과 최대 캠페인 [!DNL Adobe Analytics for Advertising] 및 [!DNL Microsoft Advertising]개를 사용하는 광고주) 이제 광고와 키워드가 포함되지 않은 성과 최대 캠페인의 추적 URL에서 새 AMO ID([!DNL s_kwcid]) 매개 변수를 구현할 때 성과 최대 캠페인에 대한 자산 그룹 수준 데이터를 Adobe Analytics에서 사용할 수 있습니다. 성과 최대 캠페인이 있는 대부분의 계정에 대한 추적이 이미 새 형식으로 마이그레이션되었습니다. [!UICONTROL Auto Upload] 추적 옵션이 없는 성과 최대 캠페인이 이미 새 형식으로 마이그레이션되지 않은 계정의 경우, 새 AMO ID 형식을 포함하도록 각 랜딩 페이지 접미사를 수동으로 업데이트해야 합니다.성과 최대 캠페인에 대한 <br><br>Adobe Analytics 데이터는 검색, 소셜 및 Commerce에서도 사용할 수 있습니다. | 새 [AMO ID 형식](https://experienceleague.adobe.com/ko/docs/analytics/components/dimensions/amo-id#dimension-items) 및 [추적 URL에 매개 변수를 추가하는 시기와 방법](/help/integrations/analytics/ids.md)을 참조하세요. |
| 2023년 12월 16일 | 도움말 | 새 문서에서는 검색, 소셜 및 Commerce의 광고에서 클릭스루 트래픽에 대해 [!DNL Target]에서 A/B 테스트를 설정하는 방법과 [!DNL Analytics]에서 테스트를 측정하고 시각화하는 방법에 대한 팁을 설명합니다. | &quot;[Adobe Target에서 검색, 소셜 및 Commerce 광고에 대한 A/B 테스트 구성](/help/integrations/target/ab-tests-search.md)&quot;을 참조하십시오. |
| 2023년 8월 8일 | [!DNL Analytics for Advertising] | 표준, 사용자 지정 및 예약 전환 지표와 트래픽 지표를 포함한 일부 [!DNL Analytics] 성공 이벤트 지표는 DSP과 검색, 소셜 및 Commerce에서 자동으로 사용할 수 있습니다. 이제 [!DNL eVar] 및 [!DNL prop] 수준의 데이터를 사용자 지정 성공 이벤트에 통합하여 기존 [!DNL Analytics] [!DNL eVars] 및 [!DNL props]을(를) 기반으로 나만의 성공 지표를 구성할 수도 있습니다. | &quot;[Adobe Analytics에서 전환 지표 만들기 [!DNL eVars] 및 [!DNL Props]](/help/integrations/analytics/conversion-metrics-from-evars.md)&quot;를 참조하십시오. |
| 2023년 7월 13일 | 보고 | ([!DNL Analytics for Advertising]을(를) 사용하는 DSP 사용자) 연결된 TV(CTV) 배치에 대한 뷰스루 전환은 이제 Adobe Analytics 내에서 사용할 수 있는 전환 데이터에 포함됩니다. | &quot;[개요 [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md#integration-examples)&quot;에서 &quot;통합 사용 방법의 예&quot; 섹션을 참조하십시오. |
| 2022년 11월 1일 | 도움말 | 새 문서에서는 Advertising DSP과 Adobe Target 간의 클릭스루 및 뷰스루 신호 공유를 구현하고, DSP 광고에 대해 [!DNL Target]에서 A/B 테스트 활동을 설정하고, 테스트 데이터를 보기 위해 Adobe Analytics Analysis Workspace을 설정하는 방법에 대해 설명합니다. | &quot;[Advertising DSP 광고를 위한 Adobe Target에서 A/B 테스트 구성](/help/integrations/target/ab-tests-dsp.md)&quot;을 참조하십시오. |
| 2022년 8월 17일 | 도움말 | 새 장에서는 Adobe Advertising을 Adobe Audience Manager과 통합하는 모든 방법을 설명합니다. | &quot;[Adobe Audience Manager과 Adobe Advertising 통합](/help/integrations/audience-manager/overview.md)&quot;에 대한 개요를 포함하여 &quot;Adobe Audience Manager과 통합&quot; 장을 참조하십시오. |
| 2021년 4월 27일 | [!DNL Analytics for Advertising] | 클릭 데이터를 Adobe Analytics으로 보내기 위해 [!DNL Analytics for Advertising] 매크로를 [!DNL Google Campaign Manager 360] 광고 태그에 추가하는 이유와 방법을 알아봅니다. | &quot;[추가 [!DNL Analytics for Advertising] 매크로를  [!DNL Google Campaign Manager 360] 광고 태그](/help/integrations/analytics/macros-google-campaign-manager.md)에 추가&quot;를 참조하십시오.&quot; |
| 2021년 4월 19일 | [!DNL Analytics for Advertising] | 매크로를 [!DNL Flashtalking] 광고 태그에 추가하여 클릭 데이터를 Adobe Analytics으로 보내는 방법과 방법에 대해 알아봅니다. | &quot;[추가 [!DNL Analytics for Advertising] 매크로를  [!DNL Flashtalking] 광고 태그](/help/integrations/analytics/macros-flashtalking.md)에 추가&quot;를 참조하십시오.&quot; |
| 2021년 10월 27일 | [!DNL Analytics for Advertising] | 조직이 데이터 수집을 위해 기존 Adobe Analytics `visitorAPI.js` 라이브러리에서 [Adobe Experience Platform [!DNL Web SDK]](https://experienceleague.adobe.com/docs/experience-platform/edge/home.html?lang=ko) 라이브러리(`alloy.js`)로 전환하려는 경우 일부 내용을 변경하여 ID 결합을 사용하도록 설정해야 합니다. | &quot;[Adobe Experience Platform과 함께  [!DNL Last Event Service] JavaScript 라이브러리 사용 [!DNL Web SDK]](/help/integrations/analytics/web-sdk.md)&quot;을(를) 참조하십시오. |
| 2021년 5월 26일 | 도움말 | 이제 &quot;[!DNL Analytics for Advertising]&quot; 장에 &quot;Working in [!DNL Analytics Marketing Channels]&quot;에 대한 하위 챕터가 포함됩니다. | &quot;[처리 규칙 기본 사항 [!DNL Marketing Channels]](/help/integrations/analytics/marketing-channels/mc-overview.md)," "[&#128279;](/help/integrations/analytics/marketing-channels/mc-ids.md)Using Adobe Advertising IDs to create [!DNL Marketing Channels] 2&rbrace;&quot;, &quot;[Adobe Advertising 데이터 사용 [!DNL Analytics Marketing Channels] &quot;, &quot;](/help/integrations/analytics/marketing-channels/mc-ac-data.md)&quot; 및 &quot;[Adobe Advertising과  [!DNL Marketing Channels]](/help/integrations/analytics/marketing-channels/mc-data-variances.md) 간에 채널 데이터가 다를 수 있는 이유&quot;를 참조하십시오.&quot; |
| 2021년 5월 26일 | 도움말 | [!DNL Analytics for Advertising]에 대한 모든 비디오 튜토리얼에 대한 링크가 추가되었습니다. | &quot;[Adobe Advertising 통합에 대한 비디오 튜토리얼](https://experienceleague.adobe.com/docs/advertising-learn/tutorials/overview.html?lang=ko)&quot;을(를) 참조하십시오. |

{style="table-layout:auto"}

<!--
 At some point, just make this an overview page instead?

Adobe Advertising is integrated with the following Adobe CX Enterprise products:

* [Adobe Analytics](/help/integrations/analytics/overview.md)

* Adobe Audience Manager

* Adobe Campaign (Adobe Advertising Search only)

 -->
