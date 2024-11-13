---
title: Adobe Customer Journey Analytics에서 사용할 AMO ID 및 EF ID에 대한 내역 데이터 수집
description: Adobe Customer Journey Analytics에서 나중에 사용할 수 있도록 Adobe Analytics에서 예약된 변수에 대한 내역 데이터를 수집하는 방법을 알아봅니다
feature: Integration with Adobe Analytics
source-git-commit: 4cd58fd995b3df9fb7837077108207ce910157c1
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 0%

---

# Adobe Customer Journey Analytics에서 사용할 AMO ID 및 EF ID에 대한 내역 데이터 수집

*[!DNL Analytics for Advertising] 및 Adobe Customer Journey Analytics만 있는 광고주*

예약된 변수를 사용하여 [!DNL Analytics for Advertising] 통합을 위한 [AMO ID 및 EF ID](ids.md)을(를) 캡처하는 경우, AMO ID 및 EF ID에 대한 예약된 변수를 가능한 한 빨리 [standard [!DNL eVars]](https://experienceleague.adobe.com/en/docs/analytics/components/dimensions/evar)에 복사하여 Adobe Advertising과 Adobe의 차세대 [!DNL analytics] 솔루션인 [Adobe Customer Journey Analytics](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-overview/cja-overview) 간의 향후 통합을 준비할 수 있습니다. 이를 통해 작업을 완료하는 즉시 AMO ID 및 EF ID에 대한 내역 데이터를 수집할 수 있습니다. 예약된 변수를 사용하며 이 작업을 완료해야 하는 경우 Adobe 계정 팀에 알려줍니다.

<!-- You can also do the same for any other reserved variables you use for your [!DNL Analytics for Advertising] implementation. -->

<!-- This will allow Adobe Experience Platform, which supplies data to Customer Journey Analytics, to begin collecting historical data for your [!DNL rVars] as soon as you complete the task. -->

## Customer Journey Analytics을 위해 이전 데이터를 수집해야 하는 이유는 무엇입니까?

Customer Journey Analytics을 사용하면 Adobe Experience Platform의 데이터를 Adobe Analytics Analysis Workspace에 동기화할 수 있습니다. 현재 Experience Platform에 대한 [!DNL Analytics Data Connector]은(는) 예약된 변수에 대한 데이터를 [!DNL Analytics]에서 Experience Platform으로 보내지 않습니다. 따라서 예약된 변수에 의해 캡처된 AMO ID 및 EF ID의 데이터는 현재 Customer Journey Analytics 내에서 사용할 수 없습니다. <!-- Instead, XXXXXXXXXX what exactly? -->.<!-- Does the Analytics for Advertising implementation use the Analytics Data Connector in particular (why would it use anything?), and we're planning to implement the Web SDK to do it instead in the future? -->

Adobe Advertising은 Customer Journey Analytics을 사용하여 향후 구현을 계획하고 있습니다. 구현이 출시되면 [!DNL Analytics for Advertising] 통합에서 [!DNL Analytics] 추적을 사용하여 클릭스루 데이터 및 (DSP 사용자) 뷰스루 데이터를 수집해야 하지만, 조직에 두 제품이 모두 있는 경우 1\) [!DNL Analytics] <!-- (Analysis Workspace using data from [!DNL Analytics]) --> 및 2\) Customer Journey Analytics <!-- (Analysis Workspace using data from Experience Platform)-->에서 데이터를 볼 수 있습니다. 기능이 릴리스되면 Experience Platform은 Customer Journey Analytics에서 사용할 AMO ID 및 EF ID에 대한 데이터를 수집하기 시작하지만, 릴리스 날짜 이전의 내역 데이터는 존재하지 않습니다.

그러나 이제 간단한 [[!DNL Analytics] 처리 규칙](https://experienceleague.adobe.com/en/docs/analytics/admin/admin-tools/manage-report-suites/edit-report-suite/report-suite-general/c-processing-rules/processing-rules)을(를) 만들어 AMO ID 및 EF ID <!-- [!DNL rVars] -->을(를) [!DNL eVars]에 복사하면 AMO ID 및 EF ID <!-- [!DNL rVars] -->에 대한 데이터를 더 빨리 수집할 수 있습니다. 처리 규칙을 만들면 새 이벤트를 추적하는 즉시 AMO ID 및 EF ID <!-- [!DNL rVars] -->에 대한 데이터를 누적하기 시작합니다. 그러면 구현을 사용할 수 있게 되면 Customer Journey Analytics 내에서 이전 데이터를 사용할 수 있습니다.

>[!NOTE]
>
>처리 규칙은 받은 새 데이터에만 적용됩니다. 과거 데이터를 수집하기 위해 소급하여 작동하지 않습니다.

## AMO ID 및 EF ID에 대해 예약된 변수를 [!DNL eVars]에 복사합니다.

이 단계는 수동이며, 향후 Adobe Advertising과 통합할 것으로 예상되는 AMO ID 및 EF ID <!-- [!DNL rVars] -->을(를) 추적하는 각 보고서 세트에 대해 완료해야 합니다.

1. 다음 설정으로 [처리 규칙을 만듭니다](https://experienceleague.adobe.com/en/docs/analytics/admin/admin-tools/manage-report-suites/edit-report-suite/report-suite-general/c-processing-rules/c-processing-rules-configuration/t-processing-rules).

   * AMO ID 및 EF ID <!-- [!DNL rVar] --> 데이터를 Customer Journey Analytics에서 사용하기 위해 Experience Platform으로 마이그레이션하려는 보고서 세트를 선택하십시오.

   * [!UICONTROL Rule Title]의 경우 &quot;eVar에 AMO ID 및 EF ID 복사&quot;와 같은 수사적 이름을 사용합니다.

   * [!UICONTROL Always Execute] 섹션에서 다음 두 작업을 추가하여 새 eVar를 만듭니다.

      * `AMO ID`의 경우: ```Overwrite value of <new/unused eVar> with amo.s_kwcid(Context Data)```

      * `EF ID`의 경우: ```Overwrite value of <new/unused eVar> With amo.ef_id(Context Data)```

   * [!UICONTROL Reason for rule]의 경우 &quot;AMO ID 및 EF ID가 Adobe Analytics 커넥터를 통해 AEP로 전송됩니다.&quot;와 같은 설명 메모를 사용합니다.

1. 저장된 처리 규칙의 유효성을 확인합니다.

   처리 규칙을 저장하면 `AMO ID` 및 `AMO EF ID` <!-- the existing reserved variables -->에 대한 데이터가 복사되는 두 개의 새 eVar에 대한 데이터와 동일해야 합니다.

   예를 들어 새 eVar `eVar142`이(가) `amo.s_kwcid(Context Data)`에 매핑되어 있으면 `eVar142`과(와) `AMO ID`의 데이터가 동일해야 합니다.

처리 규칙 적용 방법에 대한 자세한 내용은 &quot;[처리 규칙 작동 방식](https://experienceleague.adobe.com/en/docs/analytics/admin/admin-tools/manage-report-suites/edit-report-suite/report-suite-general/c-processing-rules/c-processing-rules-configuration/processing-rules-about)&quot;을 참조하십시오.

>[!MORELIKETHIS]
>
>* [개요 [!DNL Analytics for Advertising]](overview.md)
