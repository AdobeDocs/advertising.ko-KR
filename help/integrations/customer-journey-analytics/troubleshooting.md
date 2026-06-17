---
title: Customer Journey Analytics의 Adobe Advertising 데이터 문제 해결
description: Customer Journey Analytics에서 Adobe Advertising 데이터 문제를 해결하고 해결하는 방법에 대해 알아봅니다.
feature: Integration with Adobe Customer Journey Analytics
product_v2: id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2: id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: cdd65e7e-8839-44a2-bc21-0e03623b5dd1id: d3cdead0-685a-4489-9250-4bb709942f66
source-git-commit: d78aa2f6596190b644d9f920f51c179e43e86317
workflow-type: tm+mt
source-wordcount: 611
ht-degree: 0%

---

# Customer Journey Analytics의 Adobe Advertising 데이터 문제 해결

다음은 잠재적인 문제 및 그 원인입니다.

## 요약 보고

+++ Customer Journey Analytics for Advertising DSP 또는 Advertising Search, Social, Commerce에서 사용할 수 있는 요약 보고 데이터가 없습니다.

다음을 확인하십시오.

* Adobe Advertising에서 Customer Journey Analytics으로의 피드가 활성화됩니다. Adobe 계정 팀에 문의하십시오.

* Adobe Advertising 차원/분류/조회 데이터 세트와 요약 데이터 세트는 Customer Journey Analytics 연결에 포함됩니다.

* Adobe Advertising 차원 및 요약 지표는 Customer Journey Analytics 데이터 보기에 포함됩니다.

* Customer Journey Analytics Workspace이 올바른 데이터 보기를 참조하고 있습니다.

위의 모든 설정을 확인했지만 요약 데이터가 표시되지 않는 경우 [https://experienceleague.adobe.com/home#support](https://experienceleague.adobe.com/home?support-tab=home#support)에서 조직에 대한 지원 티켓을 여십시오.
.

+++

+++ 요약 보고 데이터는 Customer Journey Analytics for Advertiser 1에서 사용할 수 있지만 Advertiser 2에서는 사용할 수 없습니다.

Adobe Advertising에서 Customer Journey Analytics으로의 피드가 광고주 2에 대해 활성화되어 있는지 확인합니다. Adobe 계정 팀에 문의하십시오.

피드가 광고주에 대해 활성화되어 있지만 요약 데이터가 표시되지 않는 경우 [https://experienceleague.adobe.com/home#support](https://experienceleague.adobe.com/home?support-tab=home#support)에서 조직에 대한 지원 티켓을 여십시오.
.

+++

+++ (Search, Social 및 Commerce 사용자) 요약 보고 데이터는 한 [!DNL Google Ads], [!DNL Meta Ads] 또는 [!DNL Microsoft Advertising] 계정에 대해 Customer Journey Analytics에서 사용할 수 있지만 다른 계정에 대해서는 사용할 수 없습니다.

Adobe Advertising에서 Customer Journey Analytics으로의 피드가 특정 광고 네트워크 계정에 대해 활성화되어 있는지 확인합니다. Adobe 계정 팀에 문의하십시오.

계정에 대해 피드가 사용하도록 설정되어 있지만 요약 데이터가 표시되지 않는 경우 [https://experienceleague.adobe.com/home#support](https://experienceleague.adobe.com/home?support-tab=home#support)에서 조직에 대한 지원 티켓을 여십시오. 광고 네트워크 계정에 대한 [!UICONTROL Account ID]을(를) 포함합니다.
.

+++

+++ Customer Journey Analytics Workspace의 요약 보고 데이터가 Advertising DSP 또는 Advertising 검색, 소셜 및 Commerce의 데이터와 다르거나 일부 캠페인 및 캠페인 엔티티에 대한 요약 데이터가 누락되었습니다.

다음을 확인하십시오.

* [!DNL Workspace]과(와) Adobe Advertising 보고서 모두에서 동일한 날짜 범위를 사용하고 있습니다.

* [!DNL Workspace] 및 Adobe Advertising 보고서에 적용된 모든 필터 및 세그먼트로 인해 데이터에 차이가 발생하지 않습니다.

데이터 불일치가 확실하면 [https://experienceleague.adobe.com/home#support](https://experienceleague.adobe.com/home?support-tab=home#support)에서 조직에 대한 지원 티켓을 여십시오. 광고 네트워크 계정에 대한 [!UICONTROL Account ID]을(를) 포함합니다.
. 불일치의 증거를 보여주는 스크린샷과 스프레드시트를 포함하십시오. Adobe 계정 팀은 필요한 경우 데이터 피드를 소급하여 수정하여 불일치를 해결할 수 있습니다.

+++

## 이벤트 수준 보고

+++ 시나리오: CJA Customer Journey Analytics Workspace의 보고 차원(예: `Campaign`)에 전환 데이터(예: `Page Views`)를 사용할 수 없습니다.

장벽이 가장 적은 항목부터 시작하여 다음 사항을 확인하십시오.

* 적용 가능한 전환 지표는 Adobe Advertising에서 차원에 할당할 수 있는 웹/온라인 이벤트입니다.

* 올바른 데이터 보기를 사용하고 있습니다.

* Adobe Advertising은 해당 사이트에서 클릭스루 및 뷰스루를 추적하고 있습니다. <!-- Link to validation instructions in the user guide -->

* 분류 데이터 세트에 대한 Customer Journey Analytics 연결에서 [!DNL Key] 및 [!DNL Matching Key] 설정의 값이 올바릅니다. [!DNL Key]: `Tracking Code`(_customername.adLens2.trackingCode), [!DNL Matching Key]: `Tracking Code`(event._experience.adcloud.conversionDetails.trackingCode)

* [!DNL Adobe Advertising] 서비스가 Adobe Experience Platform 데이터 스트림에 추가되었으며, 데이터 스트림에 대해 매핑된 스키마가 `XDM ExperienceEvent Schema`이고, 필드 그룹 `Adobe Advertising Cloud ExperienceEvent Full Extension`이(가) 스키마에 추가되었습니다.

* Adobe Advertising 설정이 WebSDK Extension에 올바르게 구성되고 게시되었습니다.

위의 모든 설정을 확인했지만 전환 데이터가 여전히 표시되지 않는 경우 [https://experienceleague.adobe.com/home#support](https://experienceleague.adobe.com/home?support-tab=home#support)에서 조직에 대한 지원 티켓을 여십시오. 광고 네트워크 계정에 대한 [!UICONTROL Account ID]을(를) 포함합니다.
.

+++


<!--

+++ Question

Answer

+++

+++ Question

Answer

+++

+++ Question

Answer

+++

-->

>[!MORELIKETHIS]
>
>* [개요](overview.md)
>*  [!DNL Customer Journey Analytics]](ids.md)에서 사용하는 [Adobe Advertising ID
>* [필수 구성 요소](prerequisites.md)
>* [데이터 수집, 데이터 전송 및 보고 설정](set-up.md)
>* [Customer Journey Analytics의 Adobe Advertising 지표 및 차원](advertising-data-in-cja.md)
>* (Adobe Analytics 사용자) [Adobe Customer Journey Analytics에서 사용할 AMO ID 및 EF ID에 대한 내역 데이터 수집](/help/integrations/analytics/rvars-to-evars.md).
