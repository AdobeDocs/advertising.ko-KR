---
title: 구현 [!DNL Google Ads] 성과 최대 캠페인
description: 설정 워크플로에 대해 알아보기 [!DNL Google Ads] 성과 최대 캠페인
exl-id: afad96b2-d4a6-41ee-ad84-38aa1306d73e
feature: Search Campaign Management
source-git-commit: 05b9a55e19c9f76060eedb35c41cdd2e11753c24
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# 구현 [!DNL Google Ads] 성과 최대 캠페인

위치 [!DNL Google Ads] 성과 최대 캠페인에서는 광고 그룹, 광고 또는 키워드를 설정하지 않습니다. 대신 캠페인 설정 내에서 헤드라인, 설명 및 업로드된 이미지, 로고 를 포함하는 에셋 그룹을 하나 이상 지정합니다. [!DNL YouTube videos]. [!DNL Google Ads] 은 채널을 기반으로 광고를 게재할 자산을 자동으로 결합합니다(예: [!DNL YouTube], [!DNL Gmail], 또는 [!DNL Search]).

표 및 추세 차트 형식으로 성과 데이터와 함께 기존의 성과 최대 캠페인을 [!DNL Campaigns] 보기: 하위 수준에서 데이터를 사용할 수 없습니다. 캠페인 수준 성과 데이터는 보고서 및 Adobe Analytics(를 사용하는 광고주용)에서도 사용할 수 있습니다. [Analytics 통합](/help/integrations/analytics/overview.md). 의 성과 최대 캠페인에 대한 성과 데이터를 보려면 [!DNL Analytics], 캠페인은 다음을 사용해야 합니다. [amo ID 추적 코드가 업그레이드되었습니다.](/help/integrations/analytics/ids.md#amo-id-formats) ( 캠페인 ID 및 광고 그룹 ID를 추적합니다.)

>[!NOTE]
>
>* 모든 이미지 파일을 수동으로 업로드해야 합니다. 링크 대상 [!DNL Google Merchant Center] 제품 피드는 지원되지 않습니다.
>* 필요한 설정만 사용할 수 있습니다. 선택적 설정을 하려면에 로그인합니다. [!DNL Google Ads] 편집자.
>* 목록 그룹 지원을 사용할 수 없습니다. 목록 그룹에 대한 데이터를 관리하고 보려면 [!DNL Google Ads] 편집자.

## 설정 단계 [!DNL Google Ads] 성과 최대 캠페인

다음에서 개별적으로 성과 최대 캠페인을 설정할 수 있습니다. [!UICONTROL Campaigns] > [!UICONTROL Campaigns] 보기.

1. [캠페인 만들기](/help/search-social-commerce/campaign-management/campaigns/campaign-manage.md) 캠페인 유형 포함 **[!UICONTROL Performance Max]**.

   다음을 지정합니다. [!UICONTROL Campaign Details], [!UICONTROL Budget Options], [!UICONTROL Campaign Targeting], 및 [!UICONTROL URL Options]. 필요한 경우 다음을 입력합니다. [!UICONTROL Negative Keywords], 입력 [!UICONTROL Negative Websites], 및/또는 재정의 [!UICONTROL Campaign Tracking] 옵션.

1. 자산 그룹을 만들고 캠페인에 대한 자산을 업로드합니다.

   1. 캠페인 설정 하단에서 **[!UICONTROL Manage Asset Groups]**.

   1. 첫 번째 에셋 그룹에 대한 설정을 지정하고 에셋 그룹에 대한 이미지, 로고 및 선택적 비디오를 업로드합니다.

      다음을 참조하십시오 [자산 그룹 설정에 대한 설명](/help/search-social-commerce/campaign-management/campaigns/campaign-settings-google.md) 요구 사항 및 사양을 이해할 수 있습니다.

   1. 필요에 따라 에셋 그룹을 추가합니다.

1. 클릭 **[!UICONTROL Post]**.

1. (선택 사항) 최적화를 위해 하이브리드 포트폴리오에 캠페인을 추가합니다.
