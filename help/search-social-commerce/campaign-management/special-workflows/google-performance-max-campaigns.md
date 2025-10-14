---
title: ' [!DNL Google Ads] 성과 최대 캠페인 구현'
description: ' [!DNL Google Ads] 성과 최대 캠페인을 설정하는 워크플로우에 대해 알아봅니다.'
exl-id: 4208774c-e4dd-499d-987e-933fe073c04f
feature: Search Campaign Management
source-git-commit: 283fced2b3faa64b6383b6ab2a41696cba0da06f
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# [!DNL Google Ads] 성과 최대 캠페인 구현

[!DNL Google Ads] 성과 최대 캠페인에서는 광고 그룹, 광고 또는 키워드를 설정하지 않습니다. 대신 캠페인 설정 내에서 헤드라인, 설명, 업로드한 이미지, 로고 및 [!DNL YouTube videos]을(를) 포함하는 자산 그룹을 하나 이상 지정합니다. [!DNL Google Ads]은(는) 채널을 기반으로 광고를 제공할 자산을 자동으로 결합합니다([!DNL YouTube], [!DNL Gmail] 또는 [!DNL Search]).

[!DNL Campaigns] 보기에서 표 및 추세 차트 형식으로 성과 데이터와 함께 기존의 성과 최대 캠페인을 볼 수 있습니다. 낮은 수준에서 데이터를 사용할 수 없습니다. 캠페인 수준 성과 데이터는 보고서 및 Adobe Analytics([Analytics 통합](/help/integrations/analytics/overview.md)을 사용하는 광고주용)에서도 사용할 수 있습니다. [!DNL Analytics]의 성과 최대 캠페인에 대한 성과 데이터를 보려면 캠페인이 [업그레이드된 AMO ID 추적 코드](/help/integrations/analytics/ids.md#amo-id-formats)(캠페인 ID 및 광고 그룹 ID를 추적)를 사용해야 합니다.

>[!NOTE]
>
>* 모든 이미지 파일을 수동으로 업로드해야 합니다. [!DNL Google Merchant Center] 제품 피드에 대한 링크는 지원되지 않습니다.
>* 필요한 설정만 사용할 수 있습니다. 옵션 설정을 보려면 [!DNL Google Ads] 편집기에 로그인합니다.
>* 목록 그룹 지원을 사용할 수 없습니다. 목록 그룹에 대한 데이터를 관리하고 보려면 [!DNL Google Ads] 편집기에 로그인하십시오.

## [!DNL Google Ads] 성과 최대 캠페인을 설정하는 단계

[!UICONTROL Campaigns] > [!UICONTROL Campaigns] 보기에서 개별적으로 성과 최대 캠페인을 설정할 수 있습니다.

1. [캠페인 유형 **[!UICONTROL Performance Max]**&#x200B;을(를) 사용하여 &#x200B;](/help/search-social-commerce/campaign-management/campaigns/campaign-manage.md) 캠페인을 만듭니다.

   [!UICONTROL Campaign Details], [!UICONTROL Budget Options], [!UICONTROL Campaign Targeting] 및 [!UICONTROL URL Options]을(를) 지정하십시오. 필요한 경우 [!UICONTROL Negative Keywords]을(를) 입력하고 [!UICONTROL Negative Websites]을(를) 입력하거나 [!UICONTROL Campaign Tracking] 옵션을 재정의합니다.

1. 자산 그룹을 만들고 캠페인에 대한 자산을 업로드합니다.

   1. 캠페인 설정의 맨 아래에서 **[!UICONTROL Manage Asset Groups]**&#x200B;을(를) 클릭합니다.

   1. 첫 번째 에셋 그룹에 대한 설정을 지정하고 에셋 그룹에 대한 이미지, 로고 및 선택적 비디오를 업로드합니다.

      요구 사항 및 사양을 이해하려면 [자산 그룹 설정에 대한 설명](/help/search-social-commerce/campaign-management/campaigns/campaign-settings-google.md)을 참조하세요.

   1. 필요에 따라 에셋 그룹을 추가합니다.

1. **[!UICONTROL Post]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 최적화를 위해 하이브리드 포트폴리오에 캠페인을 추가합니다.
