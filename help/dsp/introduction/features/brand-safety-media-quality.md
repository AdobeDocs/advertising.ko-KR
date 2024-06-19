---
title: 브랜드 안전 및 미디어 품질
description: 브랜드 안전 및 미디어 품질 기능에 대해 자세히 알아보십시오.
feature: DSP Introduction
exl-id: 8cdfd517-4cdb-4dbc-aae5-a8bda1e4e95e
source-git-commit: c8cad651585210d46cb0237e1843952e5e5cec3e
workflow-type: tm+mt
source-wordcount: '1348'
ht-degree: 0%

---

# 브랜드 안전 및 미디어 품질

<!-- Check on logo sizes in staging environment -- I made them all 100 pixels high except for DoubleVerify, which is 150 (harder to see at 100), but some instances look larger in VS Code. -->

Advertising DSP은 각 캠페인이 브랜드 안전 환경에서 실제 사용자에게 도달하도록 하는 일련의 브랜드 보호 기능을 제공합니다.

사기 행위 감시 팀은 다음과 같은 업계 선두 파트너와 긴밀히 협력합니다. [!DNL Interactive Advertising Bureau], [!DNL Trust and Accountability Group] [!DNL (TAG)], 및 [!DNL WhiteOps]: 플랫폼에서 신중하게 인벤토리를 큐레이션합니다. DSP은 공급에 대한 사전 관리를 통해 플랫폼의 모든 광고주가 사람이 아닌 트래픽(보트, 크롤러, 데이터센터 트래픽 및 사기)으로부터 보호되고 브랜드가 안전한 컨텍스트에서만 전달되도록 합니다.

중앙의 품질 관리를 제공하는 것 외에도 광고주가 브랜드에 맞는 컨트롤을 디자인할 수 있는 권한을 부여한다고 생각합니다. DSP은 와 통합을 제공합니다. [!DNL Comscore], [!DNL DoubleVerify], [!DNL Integral Ad Science], [!DNL Oracle Data Cloud], 및 [!DNL Peer39]를 사용하여 각 광고주가 원하는 수준의 사기 방지, 컨텍스트 기반 필터링 및 키워드 타깃팅을 선택할 수 있습니다.

## 품질 이니셔티브

### 을 사용한 인벤토리 확인 [!DNL Ads.txt] 지원

[[!DNL Ads.txt]: [!DNL Authorized Digital Sellers]](https://iabtechlab.com/ads-txt) 은(는) 다음에 의해 시작된 이니셔티브입니다. [!DNL Interactive Advertising Bureau] ([!DNL IAB]) 2017년 6월은 오픈 마켓에서 인벤토리의 적절한 표현을 용이하게 함으로써 트래픽 및 도메인 스푸핑의 불법 소스를 방지합니다. 참여하는 게시자 및 배포자는 을(를) 유지함으로써 디지털 인벤토리를 판매하도록 승인된 회사와 그러한 관계의 특성을 공개적으로 선언합니다. `ads.txt` 도메인의 최상위 수준에 있는 페이지 (예: `example.com/ads.txt`).

DSP 지원 [!DNL ads.txt] 각 게시자의 `ads.txt` 파일 및 확인된에서 만 구입할 수 있는 옵션 제공 [!DNL ads.txt] 판매자. 예를 들어, 판매자를 일치시키면 다음에 액세스할 수 있습니다 `nytimes.com` 뉴욕 타임즈로&#39; `ads.txt` 파일, 우리는 합법적인 것과 그렇지 않은 것을 식별할 수 있으며, 배치가 인증된 판매자로부터만 구매하도록 구성된 경우 위반자를 차단합니다. <!-- can we actually mention NY Times? -->

기본값을 설정할 수 있습니다. [!DNL ads.txt] 각 광고주에 대한 컨트롤<!-- [default ads.txt controls for each advertiser](/help/dsp/admin/advertiser-settings.md) -->, 필요한 경우 [각 배치에 대한 설정 사용자정의](/help/dsp/campaign-management/placements/placement-settings.md) 끝:

* 도메인의 승인된 직접 판매자에서만 인벤토리 구입

* 도메인의 승인된 직접 판매자 및 리셀러에서만 인벤토리 구입

* 도메인의 승인된 직접 판매자 및 리셀러로부터 인벤토리 우선 구매

* 모든 판매자의 재고 구매

### 플랫폼 사기 감시

DSP은 플랫폼 전반에 걸친 사기를 관리하기 위한 강력한 내부 도구 및 시스템을 구축했으며, 다음과 같은 업계 선두 공급업체와 협력하고 있습니다. [!DNL Whiteops] 및 [!DNL Integral Ad Science].

또한 Adobe은 과 밀접하게 작동합니다. [!DNL IAB] 및 [!DNL TAG] 와 같은 도구를 활용하여 광고주를 보호하기 위해 강력한 업계 표준 사기 행위 차단을 보장합니다. [!DNL ads.txt] ( 이전 섹션 참조), [!DNL IAB] 보트 및 스파이더 목록 및 [!DNL TAG] 데이터 센터 IP 목록입니다.

품질에 대한 다차원적 접근 방식을 통해 팀은 예외 항목과 잘못된 트래픽 패턴을 모니터링하여 보호된 인벤토리에서 3% 미만의 잘못된 트래픽을 보장합니다. 특정 도메인에 대한 인벤토리 또는 특정 게시자 또는 판매자의 인벤토리를 포함하여 의심되는 모든 인벤토리는 플랫폼 전체에서 즉시 차단됩니다.

### 인벤토리 매핑, 계층화 및 분류

인벤토리 매핑은 플랫폼에 추가되기 전에 모든 새 인벤토리에 필요한 세부 검토 및 온보딩 프로세스입니다. 이 프로세스는 DSP의 모든 인벤토리의 안전과 품질을 보장하기 위해 설계되었습니다.

* **매핑:** 인벤토리 팀은 다음과 같은 측면을 평가하면서 각 도메인을 신중하게 검토합니다.

   * 브랜드 안전

   * 광고 유형 확인

   * 일반 콘텐츠, 중복 도메인 및 가짜 광고 서비스

* **계층화:** 우리는 여러 계층에 걸쳐 인벤토리를 분류하기 위해 전체 에코시스템에서 브랜드 존재를 전체적으로 검사합니다. 다음을 수행할 수 있습니다. [배치 타기팅](/help/dsp/campaign-management/placements/placement-settings.md) 원하는 도달 범위를 얻기 위해 다음 계층으로 이동:

   * **[!UICONTROL T1]** — 브랜드 이름, 국제적으로 인식 가능한 사이트

   * **[!UICONTROL T2]** — 사용자가 생성한 컨텐츠가 없고 일반적으로 세계적으로 인정받지 못하는 최신 상태의 멋진 사이트

   * **[!UICONTROL T3]** — 사용자 생성 컨텐츠 및 틈새 컨텐츠

* **사이트 분류:** 간편한 콘텐츠 타겟팅 및 차단을 위해 속성의 콘텐츠를 기반으로 DSP이 정의한 사이트 범주로 각 속성에 태그를 지정합니다. 다음을 수행할 수 있습니다. [각 배치에 대해 이러한 사이트 카테고리를 타겟팅하거나 제외합니다.](/help/dsp/campaign-management/placements/placement-settings.md) 배치 목표를 기반으로 합니다.

### 사이트 차단을 위한 포괄적인 지원

DSP은 전체적으로 차단된 사이트 목록과 광고주 및 계정에 대해 사용자 지정 차단된 사이트 목록을 만드는 옵션을 모두 제공합니다.

#### 전역적으로 차단된 사이트 목록 DSP {#global-blocked-sites}

DSP은 광고를 실행하는 것이 안전하지 않은 것으로 간주되는 사이트의 전역 차단 사이트 목록을 유지 관리합니다. 이 목록에는 불쾌한 콘텐츠(예: 증오 또는 테러)를 제공하는 사이트와 봇, 가짜 프리롤, 일치하지 않는 도메인 및 기타 사기 활동에 의해 감염된 사이트가 포함됩니다.

광고주를 속이는 활동을 근절하기 위한 브랜드 안전 이니셔티브의 일환으로 차트 차단 사이트 목록의 조치를 사용하여 모든 사이트를 선별합니다. 브랜드 안전 검사를 통과하지 않는 모든 사이트는 전역적으로 차단된 사이트 목록에 추가됩니다. DSP은 이 목록을 동적으로 관리하기 때문에 최신 브랜드 안전성 분석을 기반으로 사이트는 언제든지 목록 상에서 이동하거나 목록에서 벗어날 수 있습니다.

전역적으로 차단된 사이트 목록에 사이트를 배치 대상으로 포함하면 해당 사이트에는 빨간색 느낌표(!)가 표시됩니다. 이는 플래그가 지정된 사이트에서 광고가 실행되지 않음을 나타냅니다.

>[!NOTE]
>
>신뢰할 수 있는 비공개 거래에 첨부된 표준 디스플레이 광고에 대해 선택적으로 글로벌 차단 사이트 목록을 우회할 수 있습니다.&quot;[!UICONTROL Allow unscreened sites]의 &quot; 옵션 [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md). 필요한 경우 Adobe 계정 팀은 거래의 게시자 설정에서 공개(경매 수준) 거래에 대한 사이트 차단을 선택적으로 비활성화할 수도 있습니다.

#### 계정 수준 및 광고주 수준의 차단된 사이트 목록

사용자는 계정 수준 및 광고주 수준의 차단된 사이트 목록을 유지 관리할 수도 있습니다<!-- [account-level and advertiser-level blocked sites lists](/help/dsp/admin/blocked-sites-list-edit.md) -->모든 배치에 자동으로 사용됩니다. 전역적으로 차단된 사이트 목록 외에 더 낮은 수준의 차단된 사이트 목록이 적용됩니다.

## 타사 통합

### 상황별 필터링

컨텍스트 기반 필터링을 사용하면 광고가 제공될 페이지의 컨텍스트를 기반으로 광고 기회를 타겟팅하거나 차단할 수 있습니다. Adobe은 업계 최고의 공급업체와의 통합을 통해 상황에 맞는 필터링을 제공합니다. [!DNL Comscore], [!DNL DoubleVerify], [!DNL Integral Ad Science], 및 [!DNL Peer39]. 현재 필터의 예는 다음과 같습니다 [!UICONTROL Adult Content], [!UICONTROL Natural Disasters], [!UICONTROL Legal Drinking Age], [!UICONTROL MANGA], [!UICONTROL Epidemics], 및 [!UICONTROL G-rated Sites].

각 광고주에 대해 기본 컨텍스트 필터 컨트롤을 설정할 수 있습니다<!-- [default contextual filter controls for each advertiser](/help/dsp/admin/advertiser-settings.md) -->, 필요한 경우 [각 배치에 대한 설정 사용자정의](/help/dsp/campaign-management/placements/placement-settings.md). 이 기능을 사용하면 추가 비용이 발생할 수 있습니다.

![Comscore 로고](/help/dsp/assets/comscore-logo.png) ![DoubleVery 로고](/help/dsp/assets/doubleverify-logo.png) ![필수 광고 과학 로고](/help/dsp/assets/ias-logo.png) ![Peer39 로고](/help/dsp/assets/peer39-logo.png)

### 사전 입찰 사기 차단

과 타사 통합 활용 [!DNL Comscore], [!DNL DoubleVerify], [!DNL Integral Ad Science], 및 [!DNL Peer39] 를 사용하여 캠페인에서 사람이 아닌 트래픽을 차단할 수 있습니다. 이러한 통합은 캠페인에서 일반적이고 정교한 잘못된 트래픽(GIVT 및 SIVT)을 모두 최소화하는 업계 최고의 사전 입찰 차단 기능을 제공합니다.

각 광고주에 대해 기본 사전 입찰 사기 방지 컨트롤을 설정할 수 있습니다<!-- [default pre-bid fraud blocking controls for each advertiser](/help/dsp/admin/advertiser-settings.md) -->, 필요한 경우 [각 배치에 대한 설정 사용자정의](/help/dsp/campaign-management/placements/placement-settings.md). 이 기능을 사용하면 추가 비용이 발생할 수 있습니다.

기능에 대한 자세한 내용은 원하는 공급업체에 직접 문의하거나 Adobe 계정 팀에 문의하십시오.

![Comscore 로고](/help/dsp/assets/comscore-logo.png) ![DoubleVery 로고](/help/dsp/assets/doubleverify-logo.png) ![필수 광고 과학 로고](/help/dsp/assets/ias-logo.png) ![Peer39 로고](/help/dsp/assets/peer39-logo.png)

### 사전 입찰 가시성 {#pre-bid-viewability}

업계 최고의 파트너가 제공하는 사전 입찰 가시성 필터 [!DNL DoubleVerify], [!DNL Oracle Advertising] ([!DNL Moat]), 및 [!DNL Integral Ad Science] 광고주가 비디오 및 디스플레이 인벤토리에서 원하는 조회 성능 목표를 달성할 수 있도록 허용합니다.

각 광고주에 대해 기본 조회 필터를 설정할 수 있습니다<!-- [default pre-viewability filters for each advertiser](/help/dsp/admin/advertiser-settings.md) -->, 필요한 경우 [각 배치에 대한 설정 사용자정의](/help/dsp/campaign-management/placements/placement-settings.md). 이 기능을 사용하면 추가 비용이 발생할 수 있습니다.

![DoubleVery 로고](/help/dsp/assets/doubleverify-logo.png) ![Oracle 광고 로고](/help/dsp/assets/oracle-advertising-logo.png) ![필수 광고 과학 로고](/help/dsp/assets/ias-logo.png)

### 주제 타기팅

DSP 주제 타깃팅을 사용하면 업계 최고의 컨텍스트 기반 파트너를 활용하여 키워드 목록을 타깃팅하거나 차단할 수 있습니다 [!DNL Comscore] 및 [!DNL Oracle Data Cloud] (이전 [!DNL Grapeshot]). 주제 타깃팅은 유해한 콘텐츠 차단 또는 더 큰 성과를 보장하는 컨텍스트에서 지출 보장이 포함되든 간에 브랜드에 맞는 환경에서 광고가 항상 제공되도록 하는 데 도움이 됩니다.

주제 타깃팅을 사용하려면 파트너 플랫폼을 사용하여 직접 사용자 정의 주제 세그먼트를 만들어야 합니다. 세그먼트가 만들어지면 다음을 수행할 수 있습니다. [에서 세그먼트 ID를 타깃팅하거나 제외합니다. [!UICONTROL Audience Targeting] 각 배치의 단면](/help/dsp/campaign-management/placements/placement-settings.md). 이 기능에 대한 추가 비용이 발생할 수 있습니다.

사용자 정의 주제 세그먼트를 만들려면 다음을 수행하십시오.

* 을(를) 만들려면 [!DNL Comscore] 계정 및 사용자 지정 세그먼트를 만들면 다음에 대한 로그인을 요청할 수 있습니다 [!DNL Activation Segment Manager] 위치: [https://agents.comscore.com](https://agents.comscore.com). 다음을 참조하십시오. [[!DNL Comscore] 도움말 센터](https://comscoreactivation.zendesk.com/hc/) 사용자 지정 세그먼트 설정에 대한 전체 지침 사용자 정의 세그먼트에 대한 요금은 다음에 표시됩니다. [!DNL Segment Manager] 만들 때 사용합니다.

* 시작하려면 [!DNL Oracle Data Cloud], 연락처 [!DNL Oracle Data Cloud] 또는 Adobe 계정 팀입니다.

![Comscore 로고](/help/dsp/assets/comscore-logo.png) ![Grapeshot 로고](/help/dsp/assets/oracle-grapeshot-logo.png)

### [!DNL DoubleVerify Authentic Brand Safety]

DSP은 과(와) 파트너 관계를 맺고 있습니다. [!DNL DoubleVerify] 을 제공합니다. [!DNL Authentic Brand Safety] 타깃팅 솔루션: 일관성을 유지하기 위해 모든 구매 플랫폼에서 타깃팅할 중앙 집중식 브랜드 안전 요구 사항 세트를 만들 수 있습니다.

을(를) 빌드하면 [!DNL DoubleVerify] 필요한 타깃팅이 있는 브랜드 안전 세그먼트를 사용하면 DSP 내에서 웹 환경 간에 사전 입찰을 사용하여 입찰 후 블록 규칙을 복제할 수 있습니다.

다음을 지정할 수 있습니다. [!DNL DoubleVerify] 각 광고주용 세그먼트 ID<!-- [specify a DoubleVerify segment ID for each advertiser](/help/dsp/admin/advertiser-settings.md) -->, 필요한 경우 [활성화 또는 비활성화 [!UICONTROL Authentic Brand Safety] 각 배치용](/help/dsp/campaign-management/placements/placement-settings.md). DSP은 세그먼트 ID에 대한 사용을 위해 계정에 청구합니다.

기능에 대한 자세한 내용은 [!DNL DoubleVerify] 직접 방문하거나 Adobe 계정 팀에 문의하십시오.

![DoubleVery 로고](/help/dsp/assets/doubleverify-logo.png)

>[!MORELIKETHIS]
>
>* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)
<!-- >* [Advertiser Account Settings](/help/dsp/admin/advertiser-settings.md) -->
