---
title: (새 UI) 목표 정보
description: 비즈니스 목표를 달성하기 위한 목표에 대해 알아봅니다.
feature: Search Objectives, Search Optimization
hide: true
source-git-commit: 62de95d7e3d21ae6c7f0a6f40e97352af71411e1
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# (새 UI) 목표 정보

*Beta 기능*

목표는 광고주가 수익을 극대화하거나 특정 판매 목표를 달성하기 위해 설정하는 등 비즈니스 목표를 충족하기 위해 설정하는 목표입니다. Advertising 검색, 소셜, Commerce 및 Advertising DSP 모두 사용 목표:

* 최적화 기능이 포트폴리오에 대한 클릭 및 수익 모델을 만들 수 있도록 각 검색, 소셜 및 Commerce 포트폴리오에는 목표가 있어야 합니다.

* DSP에서 목표는 검색, 소셜 및 Commerce 계정에 연결된 DSP 계정의 사용자 지정 목표로 표시됩니다. 최적화 목표 &quot;ROAS(광고 투자 수익률)&quot; 또는 &quot;CPA(획득당 최저 비용)&quot;를 사용하는 각 패키지에는 전체 최적화 목표를 달성하는 데 도움이 되는 사용자 지정 목표가 포함되어야 합니다.

목표는 추적 및 최적화할 전환 지표와 이러한 지표의 상대 가중치로 구성됩니다. 예를 들어 두 개의 온라인 구독 수준과 한 개의 인쇄 구독 수준을 가진 목표 &quot;이익 극대화&quot;를 가진 온라인 잡지에 20 USD의 &quot;기본 온라인 구독&quot;, 40 USD의 &quot;프리미엄 온라인 구독&quot; 및 30 USD의 &quot;인쇄 구독&quot;의 세 가지 지표가 있다고 가정합시다. 잡지가 구독의 일회성 금전적 가치에 따라 가중치를 부여하고자 한다면 지표의 상대적 가중치는 각각 1, 2, 1.5가 된다.

목표의 각 지표에 대해 다음 작업을 수행할 수 있습니다.

* 모바일 장치에서 전환에 대해 별도의 가중치를 구성합니다.

* 지표에 [!UICONTROL Goal] 지표 또는 [!UICONTROL Assist] 지표로 레이블을 지정합니다.

* 지표에 가중치 권장 사항을 적용합니다.

>[!NOTE]
>* (검색, 소셜 및 Commerce) [포트폴리오를 만들 때](/help/search-social-commerce/new-ui/manage/portfolios/portfolio-create.md) 또는 나중에 [포트폴리오 설정을 수정](/help/search-social-commerce/new-ui/manage/portfolios/portfolio-edit.md)할 때 목표를 포트폴리오와 연결할 수 있습니다.
>* (검색, 소셜 및 Commerce 계정에 연결된 DSP 계정이 있는 광고주) Advertising DSP에서 패키지 수준 게재 간격이 있는 패키지에 대한 [사용자 지정 최적화 목표](/help/dsp/campaign-management/packages/package-settings.md)(으)로 목표를 선택할 수 있습니다.
>* 여러 검색, 소셜 및 Commerce 포트폴리오 및/또는 여러 DSP 패키지에 동일한 목표를 사용할 수 있습니다.
>* [!UICONTROL Objectives] 보기의 각 목표에 대한 지표에는 DSP의 데이터가 포함되지 않습니다.

## 사용 가능한 지표

목표에 다음 중 하나를 포함할 수 있습니다.

* Adobe Advertising이 [Adobe Advertising 전환 추적 픽셀](/help/search-social-commerce/tracking/conversion-tracking-advertising.md)을 사용하여 추적하는 지표입니다.

* [전환 피드 파일에서 광고주가 추적한 지표](/help/search-social-commerce/tracking/conversion-tracking-about.md).<!-- Search only, or might DSP-only clients also have these? -->

* (광고주: [!DNL Adobe Analytics for Advertising]) [전환 및 사이트 참여 지표가 Adobe Analytics에서 동기화됨](/help/integrations/analytics/overview.md).

  검색, 소셜 및 Commerce에서 다음 [사이트 참여 지표](/help/integrations/analytics/analytics-data-in-advertising.md)은(는) 포트폴리오 입찰 알고리즘에 자동으로 반영됩니다. `timespent_secs_1stvisit`, `timespent_secs_total`, `pageviews_1stvisit`, `pageviews_total` 및 `bounces`.

* [!DNL Google] 지표:<!-- Search only, or might DSP-only clients also have these? -->

   * 동기화된 [[!DNL Google Ads] 계정에서 ](/help/search-social-commerce/campaign-management/introduction/google-conversion-data.md) 추적된 전환[!DNL Google Ads]입니다.

   * ([[!DNL Google Analytics] 통합](/help/search-social-commerce/admin/data-sources/data-source-about.md)을 사용하는 광고주) 페이지 보기 수, 세션, 바운스 비율(바운스/세션으로 계산됨) 및 세션 기간입니다.

     검색, 소셜 및 Commerce에서 이러한 지표는 포트폴리오 입찰 알고리즘에 자동으로 반영됩니다.

## 광고 네트워크에 목표를 업로드하는 옵션

필요에 따라 [계정 포트폴리오의 목표를  [!DNL Google Ads] 및/또는 [!DNL Microsoft Advertising] 전환으로](/help/search-social-commerce/tools/objective-upload-to-networks.md)업로드하여 캠페인 또는 광고 그룹 수준 최적화에 사용할 수 있습니다. 이 옵션을 활성화하면 검색, 소셜 및 Commerce이 EF ID(클릭 ID) 수준의 가중 수익 데이터를 매일 광고 네트워크에 전달합니다. 광고 네트워크 추적 지표를 생략합니다.

>[!MORELIKETHIS]
>
>* [목표 만들기](objective-create.md)
>* [목표 편집](objective-edit.md)
>* [목표 삭제](objective-delete.md)
>* [목표에 가중치 권장 사항 적용](objective-apply-weight-recommendations.md)
>* [목표 설정](objective-settings.md)
