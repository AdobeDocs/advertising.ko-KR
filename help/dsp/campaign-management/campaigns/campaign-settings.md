---
title: 캠페인 설정
description: 사용 가능한 캠페인 설정에 대한 설명을 참조하십시오.
feature: DSP Campaigns
exl-id: 461c3f9e-ef69-46e7-8eb1-37ccc085ba1f
source-git-commit: 4085c1b21c0fe84653978e449321868921841367
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# 캠페인 설정

## [!UICONTROL Basic Campaign Details]

**[!UICONTROL Name]:** 캠페인 이름.

**[!UICONTROL Advertiser]:** (기존 캠페인의 경우 읽기 전용) 해당 광고주(브랜드). 기존 광고주를 선택하거나 새 광고주를 만듭니다.

**[!UICONTROL Advertiser URL]:** 광고주의 공식 페이지입니다. 이 필드를 사용하면 인벤토리 파트너와의 광고 승인 프로세스를 가속화할 수 있습니다.

**[!UICONTROL Timezone]:** (기존 캠페인의 읽기 전용) 보고 및 입찰에 대한 시간대입니다.

**[!UICONTROL Customer PO]:** (선택 사항) 삽입 주문/구매 발주에 대한 고객 구매 발주.

**[캠페인 날짜]:** 캠페인 시작 및 종료 날짜.

## [!UICONTROL Campaign Goals]

**[!UICONTROL Margin Management]:** 캠페인 여백 관리 여부: *[!UICONTROL Yes]* 또는 *[!UICONTROL No]* (기본값).

다음을 선택할 때 *[!UICONTROL Yes],* 이익 유형과 금액을 지정합니다.

* **[!UICONTROL Margin Type]:** 여백 유형. 마진 관리를 활성화하고 캠페인을 저장하면 마진 유형을 변경할 수 없습니다.

   * *[!UICONTROL Fixed]:* (기본값) DSP에서 의 고정 이익 비율을 기준으로 지출을 자동으로 계산하고 제한할 수 있습니다. [!UICONTROL Gross Budget].

   * *[!UICONTROL Dynamic]:* 별도로 지정하여 배치 수준까지 여백을 관리할 수 있습니다. [!UICONTROL Budget Reserve %] 및 [!UICONTROL Gross Budget] 캠페인의 각 패키지 및 배치에 대해. DSP은 특정 마진을 보장하지 않고 각 배치의 재무 효율성을 기반으로 최적화됩니다. 고정 수량 또는 고정 비율로 단위 유형을 납품하는 데 동의한 여러 라인 품목으로 구성된 삽입 주문에 이 옵션을 사용합니다.

* **[!UICONTROL Fixed Margin %]:** (고정 여백이 있는 캠페인만 해당) 각 삽입 순서에 대한 기본 마크업 <!-- impression? -->백분율로 나타낸 것입니다. 이 금액은 다음에서 공제됩니다. [!UICONTROL Gross Budget] 순 캠페인 예산을 정의합니다.

* **[!UICONTROL Budget Reserve %]:** (고정 수익만 있는 캠페인, 선택 사항) 다음 중 지정된 비율을 예약합니다. [!UICONTROL Gross Budget] 안전장치로. 이 금액은 다음에서 공제됩니다. [!UICONTROL Gross Budget] 순 캠페인 예산을 정의합니다.

**[!UICONTROL Gross Budget]:** (마진 관리 전용 캠페인) 지정된 한계 조정이 적용되기 전의 총 캠페인 예산입니다.

필요에 따라 일일, 주간 또는 월간 총 예산을 추가할 수 있습니다.

1. 클릭 **[!UICONTROL Add an additional Gross Budget]**.

1. 다음을 입력합니다. **[!UICONTROL Gross Budget]** 예산 간격을 선택합니다. *[!UICONTROL Daily],* *[!UICONTROL Weekly],* 또는 *[!UICONTROL Monthly]*.

캠페인에 대한 지출 한도인 총 순 예산은 마진 설정을 기반으로 자동으로 계산되며 이 값 아래에 표시됩니다.

**[!UICONTROL Budget]:** (마진 관리 없는 캠페인) 전체 캠페인 예산.

**[!UICONTROL Estimated Tax Withholding]:** 국가 또는 지방세에 대한 계정 수준에서 광고 수수료, 광고 서비스 수수료 및/또는 데이터 수수료 총 지출의 백분율을 원천징수합니다. 세율은 예산 및 게재 조정 목적을 위한 추정치이므로 인보이스 세율은 다를 수 있습니다.

원천징수할 세금을 추정하려면

1. 클릭 **[!UICONTROL Update rates here]**.

1. 다음을 지정합니다. **[!UICONTROL Estimated tax rate]**&#x200B;백분율로 나타낸 것입니다.

1. 세금을 원천징수할 각 수수료 유형 옆의 체크박스를 선택합니다. 요금 유형은 다음과 같습니다.

   * *[!UICONTROL Include estimated tax - ads fee]:* 캠페인 관리 수수료에 대한 세금을 포함하여 모든 Advertising DSP 미디어 지출에 적용됩니다.

   * *[!UICONTROL Include estimated tax - ad serving fee]:* 미디어 및 데이터를 제외하고 Advertising DSP에 대한 모든 지출에 적용됩니다. 캠페인 관리 수수료에 대한 세금은 제외됩니다

   * *[!UICONTROL Include estimated tax - data fee]:* Advertising DSP에 지출되는 모든 데이터에 적용됩니다.

1. 클릭 **[!UICONTROL Submit]**.

>[!NOTE]
>
>* 미국에서 주는 광고, 광고 서비스 및 데이터에 걸쳐 세금 수수료를 포함하는 데 있어 다를 수 있습니다. 다른 나라의 조직에 대해서는 세 가지 범주의 세액을 모두 포함하여 부가가치세를 계상하도록 한다.
>
>* 계정의 수수료 설정에서 이러한 값을 구성할 수도 있습니다.<!--[fee settings](/help/dsp/admin/tax-withholdings.md). -->


**[!UICONTROL Cross Device Level]:** (2020년 6월 22일 이후에 생성된 기존 캠페인에 대한 읽기 전용, 2020년 6월 22일 이전에 생성된 캠페인에 대해서는 사용할 수 없음) DSP이 광고를 타깃팅하고 빈도 상한을 적용하는 수준: *동일한 장치* 장치를 타깃팅하거나 *사람* 알려진 모든 장치에서 사용자를 타겟팅할 수 있습니다.

**[!UICONTROL Device Graph]:** (기존 캠페인의 경우 읽기 전용, 사람 기반 크로스 디바이스 타깃팅만 있는 캠페인) 크로스 디바이스 타깃팅 및 빈도 관리에 사용할 디바이스 그래프:

* *[!UICONTROL LiveRamp - U.S. only]:* 를 사용하여 게재하는 노출에 대해 $0.35 CPM으로 모든 광고주가 크로스 디바이스 타깃팅에 사용할 수 있습니다. [!DNL LiveRamp] 장치 그래프(타겟팅된 대상 세그먼트 내에서 찾을 수 없는 장치의 경우). 배치 수준에서 크로스 디바이스 타깃팅을 설정할 수 있습니다.

   이 옵션은 또한 모든 광고주가 빈도 관리 및 속성 측정을 위해 수수료 없이 사용할 수 있습니다.

**[!UICONTROL Frequency Cap]:** (선택 사항) 고유 장치 또는 개인 횟수(지정된 횟수에 따라 다름) [!UICONTROL Cross Device Level])은 캠페인에서 광고를 제공합니다. 옵션은 다음과 같습니다 *[!UICONTROL Unlimited]* 또는 일별, 주별, 월별 특정 금액입니다.

>[!NOTE]
>
> 캠페인, 패키지 및 배치 수준에서 빈도 상한을 설정할 수 있습니다. DSP은 campaign 계층 구조에서 가장 엄격한 빈도 상한을 준수합니다.

**[!UICONTROL Packages]:** 다음 [패키지](/help/dsp/campaign-management/packages/package-about.md) 캠페인에 포함할 예정입니다. 기존 패키지를 선택하거나 포함할 패키지를 만듭니다. 패키지를 만드는 경우 다음에 대한 설명을 참조하십시오. [패키지 설정](/help/dsp/campaign-management/packages/package-settings.md) 추가 정보.

## [!UICONTROL Campaign Measurement]

>[!NOTE]
>
>다음 설정은 측정 및 보고 기능만 활성화합니다. 성능 최적화는 패키지 및 배치 수준에서만 실행됩니다.

### [!UICONTROL 3rd Party Metrics]

#### [!UICONTROL Viewability, Fraud, & Brand Safety]

**[!UICONTROL IAS]:** (선택 사항) [!DNL IAS] 지정된 설정을 사용하여 가시성, 사기, 브랜드 안전성 및 대상 확인에 대한 측정 및 보고. 추가 요금이 부과됩니다.

* **[!UICONTROL Measure On]:** 측정할 재고: *[!UICONTROL Display and VPAID video inventory]* (기본값) 또는 *[!UICONTROL Display, VPAID & VAST video inventory]*.

   >[!NOTE]
   >
   >비디오 보기는 VPAID 인벤토리에서만 측정할 수 있습니다.

* **[!UICONTROL IAS Account ID (AnID)]:** (자체 광고주 [!DNL IAS] 계정(선택 사항) 조직의 [!DNL IAS] 계정 ID, [!DNL IAS] 은 사용량에 대해 직접 청구합니다.

* **[!UICONTROL IAS Team ID]:** (자체 광고주 [!DNL IAS] 계정(선택 사항) 조직의 팀 ID입니다 [!DNL IAS] 계정, [!DNL IAS] 은 사용량에 대해 직접 청구합니다. <!-- verify -->

**[!UICONTROL MOAT]:** (선택 사항) [!DNL MOAT] 가시성, 사기, 브랜드 안전성 및 대상 확인에 대한 측정 및 보고. 추가 요금이 부과됩니다.

#### 대상 확인

**[!UICONTROL Nielsen]:** (선택 사항) [!DNL Nielsen] 지정된 설정을 사용하여 대상 확인의 측정 및 보고. 추가 요금이 부과됩니다.

* **[!UICONTROL Target Gender]:** 대상 성별: *[!UICONTROL Both]* (기본값), *[!UICONTROL Male]*, 또는 *[!UICONTROL Female]*

* **[!UICONTROL Target Age]:** 타겟팅할 나이 범위입니다. 필요에 따라 왼쪽 및 오른쪽 슬라이더를 사용하여 범위를 줄이십시오.

* **[!UICONTROL Target Country]:** (선택 사항) 타깃팅할 국가입니다. [!DNL Nielsen] 는 지원되는 국가에서만 제공되는 노출을 측정합니다.

**[!UICONTROL comScore vCE]:** (선택 사항) [!DNL Comscore validated Campaign Essentials (vCE)] 지정된 설정을 사용하여 대상 확인의 측정 및 보고. 추가 요금이 부과됩니다.

* **[!UICONTROL Target Gender]:** 대상 성별: *[!UICONTROL Both]* (기본값), *[!UICONTROL Male]*, 또는 *[!UICONTROL Female]*

* **[!UICONTROL Target Age]:** 타겟팅할 나이 범위입니다. 필요에 따라 왼쪽 및 오른쪽 슬라이더를 사용하여 범위를 줄이십시오.

* **[!UICONTROL Target Country]:** (선택 사항) 타깃팅할 국가입니다. [!DNL Comscore] 는 지원되는 국가에서만 제공되는 노출을 측정합니다.

### [!UICONTROL 1st Party Metrics]

**[!UICONTROL Viewability sensitivity]:** 을(를) 사용하여 가시성에 대한 자사 측정 및 보고 활성화 [!DNL IAB Open Video Viewability (OpenVV)] 지정된 감도 수준을 기반으로 하는 기술:

* *[!UICONTROL Standard (50% of ad in view for two consecutive seconds)]*

* *[!UICONTROL Strict (100% of ad in view and audio on for 50% duration)]*

>[!MORELIKETHIS]
>
>* [Campaign Management 정보](campaign-about.md)
>* [캠페인 만들기](campaign-create.md)
>* [캠페인 편집](campaign-edit.md)
>* [캠페인에 대한 변경 로그 보기](campaign-change-log.md)

