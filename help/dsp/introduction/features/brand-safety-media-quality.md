---
title: 브랜드 안전 및 미디어 품질
description: 브랜드 안전 및 미디어 품질 기능에 대해 자세히 알아보십시오.
feature: DSP Introduction
exl-id: 8cdfd517-4cdb-4dbc-aae5-a8bda1e4e95e
source-git-commit: 7ee798e11375863e776ac3e802efc9112280e750
workflow-type: tm+mt
source-wordcount: '1402'
ht-degree: 0%

---

# 브랜드 안전 및 미디어 품질

<!-- Check on logo sizes in staging environment -- I made them all 100 pixels high except for DoubleVerify, which is 150 (harder to see at 100), but some instances look larger in VS Code. -->

Advertising DSP은 각 캠페인이 브랜드 안전 환경에서 실제 사용자에게 도달하도록 하는 일련의 브랜드 보호 기능을 제공합니다.

사기 행위 감시 팀은 [!DNL Interactive Advertising Bureau], [!DNL Trust and Accountability Group] [!DNL (TAG)] 및 [!DNL WhiteOps]과(와) 같은 업계 선두 파트너와 긴밀히 협력하여 플랫폼에서 인벤토리를 신중하게 조정합니다. DSP은 공급에 대한 사전 관리를 통해 플랫폼의 모든 광고주가 사람이 아닌 트래픽(보트, 크롤러, 데이터센터 트래픽 및 사기)으로부터 보호되고 브랜드가 안전한 컨텍스트에서만 전달되도록 합니다.

중앙의 품질 관리를 제공하는 것 외에도 광고주가 브랜드에 맞는 컨트롤을 디자인할 수 있는 권한을 부여한다고 생각합니다. DSP은 [!DNL Comscore], [!DNL DoubleVerify], [!DNL Integral Ad Science] 및 [!DNL Peer39]과의 통합을 제공하여 각 광고주가 원하는 수준의 사기 행위 방지, 컨텍스트 필터링 및 키워드 타깃팅을 선택할 수 있도록 합니다.

## 품질 이니셔티브

### [!DNL Ads.txt] 지원을 통한 인벤토리 확인

 [!DNL Authorized Digital Sellers]](https://iabtechlab.com/ads-txt)을(를) 의미하는 [[!DNL Ads.txt]은(는) 공개 시장에서 인벤토리의 적절한 표현을 용이하게 하기 위해 2017년 6월 [!DNL Interactive Advertising Bureau]([!DNL IAB])이 시작한 이니셔티브로, 트래픽 및 도메인 스푸핑의 불법 소스를 결합합니다. 참여하는 게시자 및 배포자는 도메인의 최상위 수준(예: `example.com/ads.txt`)에서 `ads.txt` 페이지를 유지함으로써 디지털 인벤토리를 판매할 수 있는 회사와 그러한 관계의 특성을 공개적으로 선언합니다.

DSP에서는 각 게시자의 `ads.txt` 파일을 읽고 확인된 [!DNL ads.txt] 판매자에서만 구매할 수 있는 옵션을 제공하여 [!DNL ads.txt]을(를) 지원합니다. 예를 들어, `nytimes.com`에 액세스하는 데 보이는 판매자를 New York Times의 `ads.txt` 파일과 일치시켜 합법적인 판매자와 그렇지 않은 판매자를 식별할 수 있으며, 배치가 확인된 판매자만 구매하도록 구성된 경우 위반자를 차단합니다. <!-- can we actually mention NY Times? -->

각 광고주에 대해 기본 [!DNL ads.txt] 컨트롤을 설정<!-- [default ads.txt controls for each advertiser](/help/dsp/admin/advertiser-settings.md) -->한 다음 선택적으로 [각 배치에 대한 설정을 사용자 지정](/help/dsp/campaign-management/placements/placement-settings.md)하여 다음과 같은 작업을 수행할 수 있습니다.

* 도메인의 승인된 직접 판매자에서만 인벤토리 구입

* 도메인의 승인된 직접 판매자 및 리셀러에서만 인벤토리 구입

* 도메인의 승인된 직접 판매자 및 리셀러로부터 인벤토리 우선 구매

* 모든 판매자의 재고 구매

### 플랫폼 사기 감시

DSP은 플랫폼 전반에서 사기 행각을 관리하기 위한 강력한 내부 도구 및 시스템을 구축했으며 [!DNL Whiteops] 및 [!DNL Integral Ad Science]과(와) 같은 업계 선도적인 공급업체와 파트너 관계를 맺고 있습니다.

또한 Adobe은 [!DNL IAB] 및 [!DNL TAG]과(와) 밀접하게 작동하여 [!DNL ads.txt](이전 섹션 참조), [!DNL IAB] 보트 및 스파이더 목록, [!DNL TAG] 데이터 센터 IP 목록과 같은 도구를 활용하여 강력한 업계 표준 사기 행위 차단을 보장하여 광고주를 보호합니다.

품질에 대한 다차원적 접근 방식을 통해 팀은 예외 항목과 잘못된 트래픽 패턴을 모니터링하여 보호된 인벤토리에서 3% 미만의 잘못된 트래픽을 보장합니다. 특정 도메인에 대한 인벤토리 또는 특정 게시자 또는 판매자의 인벤토리를 포함하여 의심되는 모든 인벤토리는 플랫폼 전체에서 즉시 차단됩니다.

### 인벤토리 매핑, 계층화 및 분류

인벤토리 매핑은 플랫폼에 추가되기 전에 모든 새 인벤토리에 필요한 세부 검토 및 온보딩 프로세스입니다. 이 프로세스는 DSP의 모든 인벤토리의 안전과 품질을 보장하기 위해 설계되었습니다.

* **매핑:** 인벤토리 팀은 다음과 같은 측면을 평가하면서 각 도메인을 신중하게 검토합니다.

   * 브랜드 안전

   * 광고 유형 확인

   * 일반 콘텐츠, 중복 도메인 및 가짜 광고 서비스

* **계층화:** 여러 계층에서 인벤토리를 분류하기 위해 전체 에코시스템에서 브랜드 유무를 전체적으로 검사합니다. 원하는 도달 수준에 대해 다음 계층에 [배치를 타깃팅](/help/dsp/campaign-management/placements/placement-settings.md)할 수 있습니다.

   * **[!UICONTROL T1]** — 세계적으로 인식할 수 있는 브랜드 이름 사이트

   * **[!UICONTROL T2]** — 최신 상태로, 사용자 생성 컨텐츠가 없고 일반적으로 글로벌 인식이 부족한 멋진 사이트

   * **[!UICONTROL T3]** — 사용자 생성 컨텐츠 및 틈새 컨텐츠

* **사이트 범주화:** 쉽게 콘텐츠를 타깃팅하고 차단하기 위해 속성의 콘텐츠를 기반으로 DSP이 정의한 사이트 범주로 각 속성에 태그를 지정합니다. 배치 목표를 기준으로 각 배치에 대해 [이러한 사이트 범주를 타기팅하거나 제외](/help/dsp/campaign-management/placements/placement-settings.md)할 수 있습니다.

### 사이트 차단을 위한 포괄적인 지원

DSP은 전체적으로 차단된 사이트 목록과 광고주 및 계정에 대해 사용자 지정 차단된 사이트 목록을 만드는 옵션을 모두 제공합니다.

#### 전역적으로 차단된 사이트 목록 DSP {#global-blocked-sites}

DSP은 광고를 실행하는 것이 안전하지 않은 것으로 간주되는 사이트의 전역 차단 사이트 목록을 유지 관리합니다. 이 목록에는 불쾌한 콘텐츠(예: 증오 또는 테러)를 제공하는 사이트와 봇, 가짜 프리롤, 일치하지 않는 도메인 및 기타 사기 활동에 의해 감염된 사이트가 포함됩니다.

광고주를 속이는 활동을 근절하기 위한 브랜드 안전 이니셔티브의 일환으로 차트 차단 사이트 목록의 조치를 사용하여 모든 사이트를 선별합니다. 브랜드 안전 검사를 통과하지 않는 모든 사이트는 전역적으로 차단된 사이트 목록에 추가됩니다. DSP은 이 목록을 동적으로 관리하기 때문에 최신 브랜드 안전성 분석을 기반으로 사이트는 언제든지 목록 상에서 이동하거나 목록에서 벗어날 수 있습니다.

전역적으로 차단된 사이트 목록에 사이트를 배치 대상으로 포함하면 해당 사이트에는 빨간색 느낌표(!)가 표시됩니다. 이는 플래그가 지정된 사이트에서 광고가 실행되지 않음을 나타냅니다.

>[!NOTE]
>
>[배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)에서 &quot;[!UICONTROL Allow unscreened sites]&quot; 옵션을 활성화하여 신뢰할 수 있는 개인 거래에 첨부된 표준 디스플레이 광고에 대해 전역 차단 사이트 목록을 선택적으로 우회할 수 있습니다. 필요한 경우 Adobe 계정 팀은 거래의 게시자 설정에서 공개(경매 수준) 거래에 대한 사이트 차단을 선택적으로 비활성화할 수도 있습니다.

#### 계정 수준 및 광고주 수준의 차단된 사이트 목록

사용자는 계정 수준 및 광고주 수준의 차단된 사이트 목록<!-- [account-level and advertiser-level blocked sites lists](/help/dsp/admin/blocked-sites-list-edit.md) -->을 유지 관리할 수도 있습니다. 이 목록은 모든 배치에 대해 자동으로 사용됩니다. 전역적으로 차단된 사이트 목록 외에 더 낮은 수준의 차단된 사이트 목록이 적용됩니다.

## 타사 통합

### 상황별 필터링

컨텍스트 기반 필터링을 사용하면 광고가 제공될 페이지의 컨텍스트를 기반으로 광고 기회를 타겟팅하거나 차단할 수 있습니다. Adobe은 업계 선도적인 공급업체 [!DNL Comscore], [!DNL DoubleVerify], [!DNL Integral Ad Science] 및 [!DNL Peer39]과의 통합을 통해 상황별 필터링을 제공합니다. 현재 필터의 예로는 [!UICONTROL Adult Content], [!UICONTROL Natural Disasters], [!UICONTROL Legal Drinking Age], [!UICONTROL MANGA], [!UICONTROL Epidemics] 및 [!UICONTROL G-rated Sites]이(가) 있습니다.

각 광고주에 대해 기본 상황별 필터 컨트롤을 설정<!-- [default contextual filter controls for each advertiser](/help/dsp/admin/advertiser-settings.md) -->한 다음 선택적으로 [각 배치에 대한 설정을 사용자 지정](/help/dsp/campaign-management/placements/placement-settings.md)할 수 있습니다. 이 기능을 사용하면 추가 비용이 발생할 수 있습니다.

![Comscore 로고](/help/dsp/assets/comscore-logo.png) ![DoubleVerify 로고](/help/dsp/assets/doubleverify-logo.png) ![Integral Ad Science 로고](/help/dsp/assets/ias-logo.png) ![Peer39 로고](/help/dsp/assets/peer39-logo.png)

### 사전 입찰 사기 차단

[!DNL DoubleVerify], [!DNL Integral Ad Science] 및 [!DNL Peer39]과(와)의 타사 통합을 활용하여 캠페인에서 사람이 아닌 트래픽을 차단합니다. 이러한 통합은 캠페인에서 일반적이고 정교한 잘못된 트래픽(GIVT 및 SIVT)을 모두 최소화하는 업계 최고의 사전 입찰 차단 기능을 제공합니다.

각 광고주에 대해 기본 사전 입찰 사기 행위 차단 컨트롤을 설정<!-- [default pre-bid fraud blocking controls for each advertiser](/help/dsp/admin/advertiser-settings.md) -->한 다음 선택적으로 [각 배치에 대한 설정을 사용자 지정](/help/dsp/campaign-management/placements/placement-settings.md)할 수 있습니다. 이 기능을 사용하면 추가 비용이 발생할 수 있습니다.

기능에 대한 자세한 내용은 원하는 공급업체에 직접 문의하거나 Adobe 계정 팀에 문의하십시오.

![DoubleVerify 로고](/help/dsp/assets/doubleverify-logo.png) ![Integral Ad Science 로고](/help/dsp/assets/ias-logo.png) ![Peer39 로고](/help/dsp/assets/peer39-logo.png)

### 사전 입찰 가시성 {#pre-bid-viewability}

업계 선도적인 파트너 [!DNL DoubleVerify] 및 [!DNL Integral Ad Science]이(가) 제공하는 사전 입찰 가시성 필터를 사용하면 광고주가 비디오 및 디스플레이 인벤토리에서 원하는 가시성 성능 목표를 달성할 수 있습니다.

각 광고주에 대해 기본 조회 필터를 설정<!-- [default pre-viewability filters for each advertiser](/help/dsp/admin/advertiser-settings.md) -->한 다음 선택적으로 [각 배치에 대한 설정을 사용자 지정](/help/dsp/campaign-management/placements/placement-settings.md)할 수 있습니다. 이 기능을 사용하면 추가 비용이 발생할 수 있습니다.

![DoubleVerify 로고](/help/dsp/assets/doubleverify-logo.png) ![Integral Ad Science 로고](/help/dsp/assets/ias-logo.png)

### 주의 타기팅 및 측정

[!DNL Adelaide]과(와)의 [!DNL Adobe's] 파트너십은 광고주에게 눈 추적, 노출 및 결과 데이터를 기반으로 미디어 품질을 측정하는 Adelaide 지표 &quot;[!DNL Attention Units]&quot;에 대한 지원을 제공합니다.

[배치 수준 사전 입찰 주의 타기팅](/help/dsp/campaign-management/placements/placement-settings.md)을 통해 광고주는 고객 참여를 개선하기 위해 특정 주의 수준을 타기팅할 수 있습니다.

또한 광고주는 모든 캠페인에서 최상의 비즈니스 결과를 생성하는 배치 전략을 이해하기 위해 배치 수준 [!UICONTROL Attention Score] 지표](/help/dsp/campaign-management/campaigns/campaign-settings.md#attention-measurement)(노출 횟수의 가중 평균 [!DNL Attention Units] 수)에 대한 [추적을 활성화할 수 있습니다.

각 기능에 대해 추가 비용이 적용됩니다.

### 주제 타기팅

DSP 주제 타깃팅을 사용하면 업계 최고의 컨텍스트 파트너 [!DNL Comscore]을(를) 활용하여 키워드 목록을 타깃팅하거나 차단할 수 있습니다. 주제 타깃팅은 유해한 콘텐츠 차단 또는 더 큰 성과를 보장하는 컨텍스트에서 지출 보장이 포함되든 간에 브랜드에 맞는 환경에서 광고가 항상 제공되도록 하는 데 도움이 됩니다.

주제 타깃팅을 사용하려면 파트너 플랫폼을 사용하여 직접 사용자 정의 주제 세그먼트를 만들어야 합니다. 세그먼트가 만들어지면 각 배치에 대해 [!UICONTROL Audience Targeting] 섹션에서 세그먼트 ID를 [타깃팅하거나 제외](/help/dsp/campaign-management/placements/placement-settings.md)할 수 있습니다. 이 기능에 대한 추가 비용이 발생할 수 있습니다.

[!DNL Comscore] 계정을 만들고 사용자 지정 주제 세그먼트를 만들려면 [https://agents.comscore.com](https://agents.comscore.com)에서 [!DNL Activation Segment Manager]에 대한 로그인을 요청할 수 있습니다. 사용자 지정 세그먼트 설정에 대한 전체 지침은 [[!DNL Comscore] 도움말 센터](https://comscoreactivation.zendesk.com/hc/)를 참조하세요. 사용자 지정 세그먼트에 대한 요금은 만들 때 [!DNL Segment Manager]에 표시됩니다.

![Comscore 로고](/help/dsp/assets/comscore-logo.png)

### [!DNL DoubleVerify Authentic Brand Safety]

DSP은(는) [!DNL DoubleVerify]과(와) 협력하여 [!DNL Authentic Brand Safety] 타깃팅 솔루션을 제공했습니다. 이를 통해 일관성을 위해 모든 구매 플랫폼에서 타깃팅할 중앙 집중식 브랜드 안전 요구 사항 집합을 만들 수 있습니다.

필요한 타깃팅으로 [!DNL DoubleVerify] 브랜드 안전 세그먼트를 빌드했으면 DSP 내에서 이를 사용하여 웹 환경 전반에서 사전 입찰을 사용하는 입찰 후 블록 규칙을 복제할 수 있습니다.

각 광고주에 대해 [!DNL DoubleVerify] 세그먼트 ID를 지정<!-- [specify a DoubleVerify segment ID for each advertiser](/help/dsp/admin/advertiser-settings.md) -->한 다음 선택적으로 [각 배치에 대해 [!UICONTROL Authentic Brand Safety]을(를) 활성화 또는 비활성화](/help/dsp/campaign-management/placements/placement-settings.md)할 수 있습니다. DSP은 세그먼트 ID에 대한 사용을 위해 계정에 청구합니다.

기능에 대한 자세한 내용은 [!DNL DoubleVerify]에 직접 문의하거나 Adobe 계정 팀에 문의하십시오.

![DoubleVerify 로고](/help/dsp/assets/doubleverify-logo.png)

>[!MORELIKETHIS]
>
>* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)
<!-- >* [Advertiser Account Settings](/help/dsp/admin/advertiser-settings.md) -->
