---
title: 캠페인 설정
description: 사용 가능한 캠페인 설정에 대한 설명을 참조하십시오.
feature: DSP Campaigns
exl-id: 461c3f9e-ef69-46e7-8eb1-37ccc085ba1f
source-git-commit: 7ee798e11375863e776ac3e802efc9112280e750
workflow-type: tm+mt
source-wordcount: '1034'
ht-degree: 0%

---

# 캠페인 설정

## [!UICONTROL Basic Campaign Details]

**[!UICONTROL Name]:** 캠페인 이름.

**[!UICONTROL Advertiser]:**(기존 캠페인의 경우 읽기 전용) 해당 광고주(브랜드)입니다. 기존 광고주를 선택하거나 새 광고주를 만듭니다.

**[!UICONTROL Advertiser URL]:** 광고주의 공식 페이지입니다. 이 필드를 사용하면 인벤토리 파트너와의 광고 승인 프로세스를 가속화할 수 있습니다.

**[!UICONTROL Timezone]:**(기존 캠페인의 경우 읽기 전용) 보고 및 입찰을 위한 표준 시간대입니다.

**[!UICONTROL Customer PO]:**(선택 사항) 삽입 주문/구매 주문에 대한 고객 구매 주문입니다.

**[캠페인 날짜]:** 캠페인 시작 및 종료 날짜입니다.

## [!UICONTROL Campaign Goals]

**[!UICONTROL Margin Management]:** 캠페인 여백 관리 여부: *[!UICONTROL Yes]* 또는 *[!UICONTROL No]*(기본값).

*[!UICONTROL Yes],*&#x200B;을(를) 선택하는 경우 여백 유형과 금액을 지정하십시오.

* **[!UICONTROL Margin Type]:** 여백 형식입니다. 마진 관리를 활성화하고 캠페인을 저장하면 마진 유형을 변경할 수 없습니다.

   * *[!UICONTROL Fixed]:*(기본값) DSP에서 [!UICONTROL Gross Budget]의 고정 이익 비율에 따라 지출을 자동 계산하고 제한할 수 있습니다.

   * *[!UICONTROL Dynamic]:* 캠페인의 각 패키지 및 배치에 대해 별도의 [!UICONTROL Budget Reserve %] 및 [!UICONTROL Gross Budget]을(를) 지정하여 배치 수준까지 여백을 관리할 수 있습니다. DSP은 특정 마진을 보장하지 않고 각 배치의 재무 효율성을 기반으로 최적화됩니다. 고정 수량 또는 고정 비율로 단위 유형을 납품하는 데 동의한 여러 라인 품목으로 구성된 삽입 주문에 이 옵션을 사용합니다.

* **[!UICONTROL Fixed Margin %]:**(고정 여백만 있는 캠페인) 각 삽입 순서 <!-- impression? -->에 대한 기본 마크업입니다(백분율). 이 금액은 [!UICONTROL Gross Budget]에서 공제되어 순 캠페인 예산을 정의합니다.

* **[!UICONTROL Budget Reserve %]:**(고정 수익만 있는 캠페인; 선택 사항) [!UICONTROL Gross Budget]의 지정된 비율을 보호로 예약합니다. 이 금액은 [!UICONTROL Gross Budget]에서 공제되어 순 캠페인 예산을 정의합니다.

**[!UICONTROL Gross Budget]:**(마진 관리 전용 캠페인) 지정된 제한 조정이 적용되기 전의 총 캠페인 예산입니다.

필요에 따라 일일, 주간 또는 월간 총 예산을 추가할 수 있습니다.

1. **[!UICONTROL Add an additional Gross Budget]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Gross Budget]**&#x200B;을(를) 입력하고 예산 간격: *[!UICONTROL Daily],* *[!UICONTROL Weekly],* 또는 *[!UICONTROL Monthly]*&#x200B;을(를) 선택하십시오.

캠페인에 대한 지출 한도인 총 순 예산은 마진 설정을 기반으로 자동으로 계산되며 이 값 아래에 표시됩니다.

**[!UICONTROL Budget]:**(마진 관리 없는 캠페인) 전체 캠페인 예산.

**[!UICONTROL Estimated Tax Withholding]:** 국가 또는 지방세에 대한 계정 수준에서 광고 수수료, 광고 서비스 수수료 및/또는 데이터 수수료의 총 지출 비율을 원천징수합니다. 세율은 예산 및 게재 조정 목적을 위한 추정치이므로 인보이스 세율은 다를 수 있습니다.

원천징수할 세금을 추정하려면

1. **[!UICONTROL Update rates here]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Estimated tax rate]**&#x200B;을(를) 백분율로 지정하십시오.

1. 세금을 원천징수할 각 수수료 유형 옆의 체크박스를 선택합니다. 요금 유형은 다음과 같습니다.

   * *[!UICONTROL Include estimated tax - ads fee]:* 캠페인 관리 비용에 대한 세금을 포함하여 모든 Advertising DSP 미디어 지출에 적용됩니다.

   * *[!UICONTROL Include estimated tax - ad serving fee]:* 미디어 및 데이터를 제외한 Advertising DSP의 모든 지출에 적용됩니다. 캠페인 관리 수수료에 대한 세금은 제외됩니다

   * *[!UICONTROL Include estimated tax - data fee]:*&#x200B;은(는) Advertising DSP에서 사용하는 모든 데이터에 적용됩니다.

1. **[!UICONTROL Submit]**&#x200B;을(를) 클릭합니다.

>[!NOTE]
>
>* 미국에서 주는 광고, 광고 서비스 및 데이터에 걸쳐 세금 수수료를 포함하는 데 있어 다를 수 있습니다. 다른 나라의 조직에 대해서는 세 가지 범주의 세액을 모두 포함하여 부가가치세를 계상하도록 한다.
>
>* 계정의 수수료 설정에서 이러한 값을 구성할 수도 있습니다.<!--[fee settings](/help/dsp/admin/tax-withholdings.md). -->

**[!UICONTROL Cross Device Level]:**(2020년 6월 22일 이후에 생성된 기존 캠페인에 대한 읽기 전용, 2020년 6월 22일 이전에 생성된 캠페인에 대해서는 사용할 수 없음) DSP에서 광고를 타깃팅하고 빈도 상한을 적용하는 수준: *장치를 타깃팅하는 동일한 장치* 또는 알려진 모든 장치에서 사용자를 타깃팅하는 *사람*. **참고:** 범용 ID를 대상으로 하는 배치에는 장치 간 지원을 사용할 수 없습니다.

**[!UICONTROL Device Graph]:**(기존 캠페인의 경우 읽기 전용, 사용자 기반 교차 장치 타깃팅만 있는 캠페인) 교차 장치 타깃팅 및 빈도 관리에 사용할 장치 그래프:

* *[!UICONTROL LiveRamp - U.S. only]:* [!DNL LiveRamp] 장치 그래프를 사용하여 전달되는 노출 횟수(즉, 타깃팅된 대상 세그먼트 내에서 찾을 수 없는 장치의 경우)에 대해 $0.35 CPM의 교차 장치 타깃팅에 대해 모든 광고주가 사용할 수 있습니다. 배치 수준에서 크로스 디바이스 타깃팅을 설정할 수 있습니다.

  이 옵션은 또한 모든 광고주가 빈도 관리 및 속성 측정을 위해 수수료 없이 사용할 수 있습니다.

  장치 간 지원은 레거시 ID를 대상으로 하는 배치에만 적용되지만, 범용 ID([!DNL LiveRamps] 포함)를 대상으로 하는 배치에는 적용되지 않습니다. 범용 ID에 대한 타겟팅, 빈도 관리 및 속성은 ID 수준에서만 적용됩니다.

**[!UICONTROL Frequency Cap]:**(선택 사항) 캠페인에서 고유한 장치, 유니버설 ID 또는 개인(지정된 [!UICONTROL Cross Device Level] 및 배치의 [!UICONTROL Targeting] 설정에 따라 다름)에 광고를 제공할 수 있는 횟수입니다. 옵션에는 *[!UICONTROL Unlimited]* 또는 일, 주 또는 월당 특정 금액이 포함됩니다.

>[!NOTE]
>
> 캠페인, 패키지 및 배치 수준에서 빈도 상한을 설정할 수 있습니다. DSP은 campaign 계층 구조에서 가장 엄격한 빈도 상한을 따릅니다.

**[!UICONTROL Packages]:** 캠페인에 포함할 [패키지](/help/dsp/campaign-management/packages/package-about.md)입니다. 기존 패키지를 선택하거나 포함할 패키지를 만듭니다. 패키지를 만드는 경우 자세한 내용은 [패키지 설정](/help/dsp/campaign-management/packages/package-settings.md)에 대한 설명을 참조하십시오.

## [!UICONTROL Campaign Measurement]

>[!NOTE]
>
>다음 설정은 측정 및 보고 기능만 활성화합니다. 성능 최적화는 패키지 및 배치 수준에서만 실행됩니다.

### [!UICONTROL 3rd Party Metrics]

#### [!UICONTROL Viewability, Fraud, & Brand Safety]

**[!UICONTROL IAS]:**(선택 사항) 지정한 설정을 사용하여 가시성, 사기, 브랜드 안전성 및 대상 확인에 대한 [!DNL IAS] 측정 및 보고를 사용하도록 설정합니다. 추가 요금이 부과됩니다.

* **[!UICONTROL Measure On]:** 측정할 인벤토리: *[!UICONTROL Display and VPAID video inventory]*(기본값) 또는 *[!UICONTROL Display, VPAID & VAST video inventory]*.

  >[!NOTE]
  >
  >비디오 보기는 VPAID 인벤토리에서만 측정할 수 있습니다.

* **[!UICONTROL IAS Account ID (AnID)]:**(광고주가 자체 [!DNL IAS] 계정을 가지고 있음, 선택 사항) 조직의 [!DNL IAS] 계정 ID입니다. [!DNL IAS]은(는) 사용을 위해 직접 청구합니다.

* **[!UICONTROL IAS Team ID]:**(광고주가 자체 [!DNL IAS] 계정을 가지고 있음, 선택 사항) [!DNL IAS]에서 직접 사용량에 대해 청구하는 조직의 [!DNL IAS] 계정에 대한 팀 ID입니다. <!-- verify -->

#### 대상 확인

**[!UICONTROL Comscore Campaign Ratings]:**(선택 사항) 지정된 설정을 사용하여 [!DNL Comscore]에서 확인된 [!DNL Campaign Ratings] 측정 및 대상 확인 보고를 사용하도록 설정합니다. 추가 요금이 부과됩니다.

* **[!UICONTROL Target Gender]:** 대상 성별: *[!UICONTROL Both]*(기본값), *[!UICONTROL Male]* 또는 *[!UICONTROL Female]*

* **[!UICONTROL Target Age]:** 대상 연령 범위입니다. 필요에 따라 왼쪽 및 오른쪽 슬라이더를 사용하여 범위를 줄이십시오.

* **[!UICONTROL Target Country]:**(선택 사항) 대상 국가입니다. 지원되는 국가에서만 제공되는 측정값 노출 수 [!DNL Comscore]개.

### [!UICONTROL Attention Measurement]{#attention-measurement}

**[!UICONTROL Adelaide]:** 배치 수준 [!UICONTROL Attention Score] 지표(노출 횟수의 가중 평균 [!DNL Adelaide] &quot;[!DNL Attention Units]&quot; 수)에 대한 추적을 사용하도록 설정합니다. [!DNL Roku] 연결된 TV, VPAID 전용 프리롤 및 팟캐스트가 아닌 오디오를 제외한 모든 배치 유형에 대해 지표를 사용할 수 있습니다. DSP은 연결된 모든 광고 프로그램에 JavaScript 태그를 자동으로 연결하며, [!DNL Adelaide]은(는) 노출 데이터를 추적하여 DSP에 매일 보냅니다. 날짜를 사용하여 더 나은 주의 점수로 배치 전략에 대한 지출을 수동으로 최적화할 수 있습니다.

[!UICONTROL Attention Score] 필드는 보고서의 [!UICONTROL Metrics] 섹션([!UICONTROL Campaigns], [!UICONTROL Packages] 및 [!UICONTROL Placements] 보기 내)과 [배치 세부 정보 보기](/help/dsp/campaign-management/reports/placement-details-view.md)의 [!UICONTROL Sites], [!UICONTROL Ads] 및 [!UICONTROL Inventory] 탭에서 사용할 수 있습니다.

측정에 [!DNL Adelaide] 세그먼트를 사용하면 [!DNL Adelaide] 측정 태그가 있는 광고에서 게재된 각 노출에 대한 CPM 요금이 발생합니다. 이 요금은 [배치 수준 주의 타기팅](/help/dsp/campaign-management/placements/placement-settings.md)에 대한 요금과는 별개입니다.

<!--
Example JavaScript tag:

`<script src="https://www.example.com/aam?asid=0123456789&ad=${TM_AD_ID_NUM}&adv=${TM_ADVERTISER_ID}&ca=${TM_CAMPAIGN_ID_NUM}&df=${NS_PLATFORM_ID}&dt=${NS_DEVICE_GROUPING}&pl=${TM_PLACEMENT_ID_NUM}&ra=${TM_RANDOM}&st=${TM_SITE_URL_URLENC}"></script>`
-->

### [!UICONTROL 1st Party Metrics]

**[!UICONTROL Viewability sensitivity]:** 지정된 감도 수준에 따라 [!DNL IAB Open Video Viewability (OpenVV)] 기술을 사용하여 자사 측정 및 조회 보고를 사용하도록 설정합니다.

* *[!UICONTROL Standard (50% of ad in view for two consecutive seconds)]*

* *[!UICONTROL Strict (100% of ad in view and audio on for 50% duration)]*

>[!MORELIKETHIS]
>
>* [Campaign Management 정보](campaign-about.md)
>* [캠페인 만들기](campaign-create.md)
>* [캠페인 편집](campaign-edit.md)
>* [캠페인에 대한 변경 로그 보기](campaign-change-log.md)
