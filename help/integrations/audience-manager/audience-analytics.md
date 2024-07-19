---
title: Adobe Advertising 고객용 '[!DNL Adobe] [!DNL Audience Analytics] '
description: 광고 사용 사례에  [!DNL Adobe] [!DNL Audience Analytics]을(를) 사용하는 방법 알아보기
feature: Integration with Adobe Audience Manager
exl-id: 457d4335-2762-4aab-94b8-12f8a79d109b
source-git-commit: 443f8907644bf3e480626e14713e8abb9bfca284
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Adobe Advertising 고객용 [!DNL Adobe] [!DNL Audience Analytics]

[[!DNL Adobe] [!DNL Audience Analytics]](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html)은(는) Adobe Audience Manager과 Adobe Analytics 간의 통합으로, Audience Manager 고객은 사이트 활동에 대한 풍부한 통찰력을 위해 세그먼트를 [!DNL Analytics]에 보낼 수 있습니다.

Adobe Advertising 고객은 [!DNL Audience Analytics]을(를) 사용하여 혜택을 누릴 수 있습니다. 통합을 통해 다음과 같은 작업을 수행할 수 있습니다.

* 상위 단계 활동이 다운스트림 사이트 활동에 미치는 영향을 확인하려면 Adobe Advertising 노출 데이터를 [!DNL Analytics]에 직접 전송하십시오.

* 상위 단계 노출 광고에서 마케팅 채널 및 사이트 시작 지점을 결정합니다.

* [!DNL Analytics for Advertising]과의 통합을 계층화하여 [!DNL Analytics for Advertising] 데이터와 [Audience Manager [!DNL Audience Marketplace]](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/audience-marketplace/audience-marketplace.html)의 타사 인구 통계 세그먼트를 통합하여 사용자 프로필에 대한 자세한 정보를 얻을 수 있습니다.

  [!DNL Audience Marketplace]에서는 &quot;활성화&quot; 구독 모델을 사용하여 서드파티 데이터 피드에 액세스할 수 있으므로 구매자가 데이터를 대상에 보낼 수 있습니다. 데이터가 [!DNL Analytics] 대상 내에서 사용되는 경우 활성화 요금이 적용되지 않습니다.

* (Advertising DSP을 사용하는 광고주) 전체적인 여정 관리 통찰력을 위해 노출 세그먼트를 더 추가합니다.

  Advertising DSP은 Adobe Experience Platform 또는 Audience Manager 노출 추적 픽셀의 구현을 통해 노출 데이터를 실행 가능한 신호로 Audience Manager에 보낼 수 있습니다. 동일한 데이터를 [!DNL Analytics](으)로 전달하면 고급 데이터 분석이 가능합니다. 자세한 내용은 &quot;[Adobe Audience Manager과 Adobe Advertising 미디어 데이터 통합 개요](/help/integrations/audience-manager/media-data-integration/overview.md)&quot;를 참조하십시오.

필수 구성 요소 및 워크플로를 포함하여 [!DNL Audience Analytics]에 대한 자세한 내용은 &quot;[Audience Analytics 개요](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html)&quot;를 참조하십시오.

## Adobe Advertising 데이터와 함께 [!DNL Audience Analytics] 데이터를 사용하는 방법의 예

다음은 [!DNL Analytics] [!DNL Analysis Workspace] 내에서 결합된 데이터를 사용할 수 있는 방법의 예입니다.

### 상위 단계 활동이 다운스트림 활동에 미치는 영향 참조

Audience Manager 노출 세그먼트를 사용하여 상위 단계 사이트 활동이 다운스트림 사이트 활동에 미치는 영향을 확인합니다. Adobe Advertising 또는 서드파티 매크로 ID를 추적 픽셀에 포함시켜 캠페인 수준에서 사용자가 노출된 사이트 수준까지 세부 수준에 미치는 영향을 추적합니다.

주요 이점:

* 단계/광고 유형별로 노출을 추적하고 [!DNL Audience Analytics]을(를) 사용하여 시작 비율을 결정하고 고객 여정의 다음 단계와 겹칩니다.

* 상위 단계 활동이 다운스트림 사이트 활동에 미치는 영향을 확인합니다.

* [!DNL Analytics for Advertising]<!-- which doesn't include the last exposure event -->과(와) [!DNL Audience Analytics] 데이터 <!-- (which includes the user's last exposure event) -->을(를) 연결하여 사이트에 대한 전체적인 여정을 확인합니다.

다음은 [!DNL Analysis Workspace]에서 만들 수 있는 보고서의 예입니다.

![상위 단계 활동이 다운스트림 사이트 활동에 미치는 영향 확인](/help/integrations/assets/audience-analytics-upper-funnel-exposure.png)

### 사용자 프로필 분석에 [!DNL Audience Analytics] 타사 세그먼트 데이터 사용

서드파티 Audience Manager 세그먼트를 사용하여 사용자가 사이트와 상호 작용하는 방법을 보다 풍부하게 분석할 수 있습니다. 이 정보를 사용하여 타사 세그먼트의 프로필이 미디어 캠페인 사이트에 대한 주요 성능 지표와 어떻게 관련되어 있는지 여부에 따라 미디어를 활성화할 새 타사 대상을 결정할 수 있습니다.

>[!TIP]
> [!DNL Analytics]에서 수집하는 다른 차원과 마찬가지로 [!DNL Analytics] 전체에서 Audience Manager `Audiences ID` 및 `Audiences Name` 차원을 사용합니다.

다음은 [!DNL Analysis Workspace]에서 만들 수 있는 보고서의 예입니다.

![서드파티 세그먼트를 사용하여 사용자 프로필 분석 강화](/help/integrations/assets/audience-analytics-third-party-report.png)

>[!MORELIKETHIS]
>
>* [Adobe Audience Manager과 통합 Adobe Advertising](/help/integrations/audience-manager/overview.md)
