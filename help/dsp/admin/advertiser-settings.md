---
title: 광고주 계정 설정
description: 사용 가능한 광고주 설정에 대한 설명을 참조하십시오.
role: User, Admin
source-git-commit: 55190d02a2cdf74c39968ccd91abfecc2ce5539d
workflow-type: tm+mt
source-wordcount: '954'
ht-degree: 0%

---

# 광고주 계정 설정

*읽기 전용 사용자가 사용할 수 없음*

## [!UICONTROL General] 설정

**[!UICONTROL Advertiser Name]:** 광고주 이름입니다.

**[!UICONTROL Category]:** 광고주의 비즈니스가 작동하는 범주입니다. 재고에 입찰하면 카테고리가 게시자에게 전달됩니다. 광고에 맞는 카테고리를 선택해야 합니다. 그렇지 않으면 게시자가 광고를 거부할 수 있습니다.

>[!NOTE]
>
>*[!UICONTROL Other]*&#x200B;을(를) 선택하면 광고주가 DSP [!DNL On Demand Inventory]에 액세스할 수 없습니다.

**[!UICONTROL Advertiser URL]:** 광고주의 홈 페이지 또는 기본 웹 사이트 URL(`http://` 또는 `https://`(으)로 시작).

**[!UICONTROL Share all private exchange feeds into this advertiser]:**(새 광고주 계정만 해당) 조직의 DSP 계정에 대해 구성된 모든 비공개 교환 피드를 광고주가 사용할 수 있도록 합니다.

### [!UICONTROL Adobe IMS IDs]

추가 Adobe Experience Cloud 제품이 있는 광고주는 Experience Cloud을 위해 조직의 고유 ID를 사용하여 일부 제품 간에 데이터를 공유할 수 있습니다. [!UICONTROL Integrations] 섹션에서 특정 제품 통합을 구성할 수 있습니다.

**[!UICONTROL Account IMS org and ID]:**(여러 광고주가 있는 Experience Cloud 계정을 통해 라이선스가 부여된 추가 Experience Cloud 제품을 가진 광고주; 선택 사항) 광고주의 Experience Cloud 조직 ID입니다.

**[!UICONTROL Advertiser IMS org and ID]:**(추가 Experience Cloud 제품에 대한 직접 라이선스가 있는 광고주, 선택 사항) 광고주의 Experience Cloud 조직 ID입니다.

### [!UICONTROL Integrations]

(선택 사항) DSP 계정에 연결된 추가 Experience Cloud 제품. 제품은 [!UICONTROL Adobe IMS IDs] 섹션에 제공된 것과 동일한 Experience Cloud 조직 ID와 연결되어 있어야 합니다.

**[!UICONTROL Attribution services]** > **[!UICONTROL Adobe Media Optimizer]:**(광고주: [!DNL Advertising Search, Social, & Commerce] 또는 Adobe Advertising 전환 픽셀을 사용) DSP이 속성 데이터를 교환하는 [!DNL Search, Social, & Commerce] 계정.

**[!UICONTROL Report suites]** > **[!UICONTROL Adobe Analytics]:**(Adobe Analytics을 사용하는 광고주; 선택 사항; [!DNL EF Redirect] 및 토큰만 포함하는 Adobe Advertising 전환 추적 태그를 사용하여 수집된 데이터에만 적용 가능) DSP이 게시자 및 공급측 파트너로부터 수집한 데이터를 전송하는 하나 이상의 [!DNL Analytics] 보고서 세트. 또한 Analytics는 클라이언트 사이트에서 수집한 데이터를 DSP으로 전송합니다.

데이터가 보고서 세트에 표시되도록 하려면 적절한 [!DNL Search, Social, & Commerce] 광고주 수준 설정을 사용해야 합니다. 또한 광고주의 [!DNL Analytics] 계정이 Adobe Advertising에서 데이터를 받도록 구성되어 있어야 합니다.

>[!WARNING]
>
>이전에 연결된 보고서 세트를 제거하면 DSP이 더 이상 해당 세트와 데이터를 교환하지 않습니다. 데이터 변동이 발생할 것으로 예상됩니다.

[!DNL Analytics]과의 통합에 대한 자세한 내용은 &quot;[개요 [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md)&quot;를 참조하십시오.

**[!UICONTROL Audiences]** > **[!UICONTROL Adobe Analytics Cloud]:**(Adobe Audience Manager 또는 Adobe Analytics을 사용하는 광고주, 선택 사항) DSP이 광고주의 모든 Adobe 대상에 대한 세그먼트 메타데이터, 계층 데이터 및 고유 대상 데이터를 가져오는 Audience Manager 또는 [!DNL Analytics] 계정입니다. 여기에는 다음에 대한 데이터가 포함됩니다.

* Audience Manager 세그먼트
* Adobe Experience Cloud에 게시된 [!DNL Analytics]개 세그먼트
* Adobe Experience Cloud [!DNL Audience Library]을(를) 사용하여 만든 세그먼트
* Adobe Experience Platform에서 생성되어 Audience Manager을 통해 Adobe Advertising으로 전송되는 세그먼트

초기 동기화는 약 24시간이 소요됩니다. 그 후에는 데이터가 1~2초 지연으로 실시간으로 동기화됩니다.
<!-- I don't think this is true anymore:
Segment membership data is sent to Adobe Advertising only after one of the following:

* The segment is targeted in an Adobe Advertising placement or audience library
* The segment is added to the Adobe Advertising batch and real-time destinations within the Audience Manager user interface
-->

## [!UICONTROL Targeting] 설정

광고주의 새 배치에 대한 기본 타겟을 선택적으로 구성할 수 있습니다. 사용자는 새 배치에 대한 기본 대상을 재정의할 수 있습니다.

### [!UICONTROL Geo-targeting]

**[!UICONTROL Countries]:** 각 배치의 지역 타깃팅에 대한 기본 국가입니다. 사용자는 각 배치에 대해 국가를 변경하고 보다 구체적인 지역 타겟팅을 구성할 수 있습니다.

### [!UICONTROL Audience Targeting]

**[!UICONTROL Audiences to exclude]:** 기본적으로 제외할 대상 또는 세그먼트입니다. 사용자는 각 배치에 대한 제외를 변경할 수 있습니다.

### [!UICONTROL Media Quality]

#### [!UICONTROL Contextual Filtering]

적용할 [!DNL Comscore], [!DNL DoubleVerify], [!DNL Integral Ad Science] 및 [!DNL Peer39] 컨텍스트 필터의 형식입니다. [배치 수준](/help/dsp/campaign-management/placements/placement-settings.md)에서 광고주 수준 설정을 재정의할 수 있습니다.

##### [!UICONTROL DoubleVerify] {#doubleverify-context}

**[!UICONTROL Block sites that are]:**(선택 사항) 기본적으로 차단되는 하나 이상의 재고 컨텍스트 유형. 추가 요금이 부과될 수 있습니다.

##### [!UICONTROL Peer 39] {#peer39-context}

**[!UICONTROL Target sites that are]:**(선택 사항) 기본적으로 타깃팅할 하나 이상의 재고 특성 유형입니다. 추가 요금이 부과될 수 있습니다.

##### [!UICONTROL ComScore]

**[!UICONTROL Block sites that are]:**(선택 사항) 기본적으로 차단되는 하나 이상의 재고 특성 유형입니다. 추가 요금이 부과될 수 있습니다.

##### [!UICONTROL Integral Ad Science] {#ias-context}

**[!UICONTROL Adult Content]:**(선택 사항) 기본적으로 광고를 차단할 성인 콘텐츠의 정도: *[!UICONTROL Do Not Block]*(기본값), *[!UICONTROL Standard]* 또는 *[!UICONTROL Strict]*. 추가 요금이 부과될 수 있습니다.

**[!UICONTROL Alcohol Content]:**(선택 사항) 기본적으로 광고를 차단할 알코올 도입니다. *[!UICONTROL Do Not Block]*(기본값), *[!UICONTROL Standard]* 또는 *[!UICONTROL Strict]*. 추가 요금이 부과될 수 있습니다.

#### [!UICONTROL Pre-Bid Fraud Blocking]

[!DNL DoubleVerify], [!DNL Integral Ad Science] 및 [!DNL Peer39]을(를) 통해 측정된 사기 트래픽 및 의심스러운 활동을 기반으로 차단할 사이트 유형입니다. [배치 수준](/help/dsp/campaign-management/placements/placement-settings.md)에서 광고주 수준 설정을 재정의할 수 있습니다.

##### [!UICONTROL DoubleVerify] {#doubleverify-fraud}

**[!UICONTROL Block Fraud Sites (100% Invalid traffic) and User-Based Fraud and IVT Devices]:** 기본적으로 새 배치에 대해 하이재핑된 장치의 트래픽을 포함하여 100% 잘못된 모든 트래픽을 차단합니다. 추가 요금이 부과될 수 있습니다.

**[!UICONTROL Also block sites with]:**(선택 사항) DSP이 기본적으로 광고를 차단하도록 하는 추가적인 수준의 사기 및 잘못된 트래픽입니다. *[!UICONTROL None]*(기본값: 추가 트래픽을 차단하지 않음), *[!UICONTROL >2% Average Fraud/IVT levels (lowest reach)]*, *[!UICONTROL >4% Average Fraud/IVT levels]*, *[!UICONTROL >6% Average Fraud/IVT levels]*, *[!UICONTROL >10% Average Fraud/IVT levels]* 또는 *[!UICONTROL >25% Average Fraud/IVT levels]*. 추가 요금이 부과될 수 있습니다.

##### [!UICONTROL Peer 39] {#peer-39-fraud}

**[!UICONTROL Block sites that are]:**(선택 사항) DSP에서 기본적으로 광고를 차단하는 하나 이상의 사기 유형: *[!UICONTROL Fraud]*(사기로 모든 사이트를 차단함), *[!UICONTROL Fraud: Bot Sites_Non-Human traffic]* 및/또는 *[!UICONTROL Fraud: Zero Ads]*. 추가 요금이 부과될 수 있습니다.

##### [!UICONTROL Integral Ad Science] {#ias-fraud}

**[!UICONTROL Block sites that are]:**(선택 사항) DSP에서 기본적으로 광고를 차단하도록 하는 의심스러운 웹 사이트 또는 앱 활동 유형: *[!UICONTROL None]*(의심스러운 활동을 기반으로 광고를 차단하지 않는 기본값), *[!UICONTROL Suspicious Activity - High Risk]* 또는 *[!UICONTROL Suspicious Activity - High or Moderate Risk]*. 추가 요금이 부과될 수 있습니다.

#### [!UICONTROL Pre-Bid Viewability]

배치에 적용할 [!DNL DoubleVerify], [!DNL Oracle Advertising]([!DNL Moat]) 및 [!DNL Integral Ad Science]별 선택적 사전 입찰 가시성 필터입니다. 새 배치에 대해 광고주 수준 기본값이 선택됩니다. [배치 수준](/help/dsp/campaign-management/placements/placement-settings.md)에서 광고주 수준 설정을 재정의할 수 있습니다.

>[!NOTE]
>
>[!DNL Oracle]은(는) [!DNL MOAT]의 모든 서비스를 포함하여 2024년 9월 30일까지 광고 사업을 종료할 예정입니다.

##### [!UICONTROL DoubleVerify] {#doubleverify-viewability}

###### 비디오

**0}을(를) 사용합니다. **[!UICONTROL Include URL's whose average video viewability rate is]** 이 옵션을 사용하여 기준을 선택합니다.

**0} 사용&#x200B;**[!UICONTROL Impressions with Insufficient IAB Viewability Data]**

**0}을(를) 사용합니다. **[!UICONTROL Include URL's whose average completion & fully viewable rate is]** 이 옵션을 사용하여 기준을 선택합니다.

**0}을(를) 사용합니다. **[!UICONTROL Include URL's whose average player size composition is]** 이 옵션을 사용하여 기준을 선택합니다.

**0} 사용&#x200B;**[!UICONTROL Impressions with Insufficient Player Size Statistics]**

###### 표시

**0}을(를) 사용합니다. **[!UICONTROL Only target URL's or Apps that have historically achieved a display viewability rate of]** 이 옵션을 사용하여 기준을 선택합니다.

* **[!UICONTROL Impressions with Insufficient IAB Viewability Performance Data]**

* **[!UICONTROL Include Apps and URL's whose average entire creative (100% of pixels) viewable duration is]**. 이 옵션을 사용하여 기준을 선택합니다.

* **[!UICONTROL Impressions with Insufficient BXD Performance Data]**

##### [!UICONTROL Integral Ad Science] {#ias-viewability}

선택적 **[!UICONTROL Video Viewability Targets]** 필터 및 선택적 **[!UICONTROL Display Viewability Targets]** 필터입니다. 추가 요금이 부과될 수 있습니다.

##### [!UICONTROL Moat] {#moat-viewability}

선택적 **[!UICONTROL Video Viewability Standard]** 필터 및 선택적 **[!UICONTROL Display Viewability Standard]** 필터입니다. 추가 요금이 부과될 수 있습니다.

#### [!UICONTROL Ads.text]

**[!UICONTROL Ads.txt Filtering]:** 기본적으로 각 게시자의 [!DNL Authorized Digital Sellers] 목록을 활용하여 사용할 [[!DNL Ads.txt] 사전 입찰 필터링](https://iabtechlab.com/ads-txt-about/) 수준입니다.
* *[!UICONTROL Opt out of ads.txt (default)]*: 모든 판매자의 인벤토리를 구매합니다.
* *[!UICONTROL Ads.txt sellers + sites without ads.txt]*: 도메인의 승인된 직접 판매자 및 리셀러로부터 인벤토리 구매의 우선 순위를 지정합니다.
* *[!UICONTROL Ads.txt sellers only]*: 도메인의 승인된 직접 판매자 및 리셀러에서만 인벤토리를 구매합니다.
* *[!UICONTROL Ads.txt sellers only]*: 도메인의 승인된 직접 판매자에서만 인벤토리를 구매합니다.

[배치 수준](/help/dsp/campaign-management/placements/placement-settings.md)에서 광고주 수준 설정을 재정의할 수 있습니다.

#### [!UICONTROL Safe Site Block]

**[!UICONTROL Enable Site Safety Block]:** 기본적으로 실시간 입찰 필터를 사용하여 광고주가 타깃팅하는 사이트에서 광고가 제공되도록 합니다. <!-- Can remove this: Users can enable or disable the feature for each placement. I don't see this option, but I should probably verify. If this can't be edited at placement level, then remove "By default." If it can, say that you can override at placement level. -->

#### [!UICONTROL DoubleVerify Authentic Brand Safety]

**[!UICONTROL DoubleVerify Account]:** ([!DNL DoubleVerify]개 고객만 해당; 선택 사항) 조직의 [!DNL DoubleVerify] 계정과 연결된 브랜드 안전 세그먼트 ID입니다.

**[!UICONTROL Enable Authentic Brand Safety]:**(선택 사항) 기본적으로 지정된 세그먼트 ID에 대해 구성된 사용자 지정 브랜드 안전 규칙을 사용하여 입찰 후 노출을 차단하는 [!DNL DoubleVerify] 정품 브랜드 안전 기능을 사용합니다. DSP은 세그먼트 ID에 대한 사용을 위해 계정에 청구합니다.

배치 수준에서 광고주 수준 설정을 재정의할 수 있습니다.

>[!MORELIKETHIS]
>
>* [광고주 계정 만들기](/help/dsp/admin/advertiser-create.md)

<!-- >* [View the Advertiser List for the Account](/help/dsp/admin/advertiser-view.md) -->
