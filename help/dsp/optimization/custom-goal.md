---
title: 사용자 정의 목표
description: 가장 낮은 CPA 또는 가장 높은 ROAS에 최적화된 패키지에서 성공 이벤트를 정의하는 사용자 정의 목표에 대해 알아봅니다.
feature: DSP Optimization
exl-id: e40b82bc-2558-4e78-b269-9b9a3f0f5219
source-git-commit: df5d34c7d86174107278e0cd4f5a99329a21ca61
workflow-type: tm+mt
source-wordcount: '1191'
ht-degree: 0%

---

# 사용자 정의 목표

사용자 지정 목표는 광고주가 비즈니스 목표를 달성하는 데 필요한 성공 이벤트를 정의합니다. 최적화 목표 &quot;[!UICONTROL Highest Return on Ad Spend (ROAS)"]&quot; 또는 &quot;[!UICONTROL Lowest Cost per Acquisition (CPA)]&quot;을(를) 사용하는 각 패키지에는 전체 최적화 목표를 달성하는 데 도움이 되도록 사용자 지정 목표가 포함되어야 합니다. 사용자 지정 목표를 *의*&#x200B;목표[!DNL Advertising Search, Social, & Commerce]&#x200B;(으)로 만들 수 있습니다. DSP에 대한 각 목표의 이름 앞에는 &quot;ADSP_&quot;가 붙어야 합니다.

<!-- update image or omit it

![custom goals](/help/dsp/assets/objective-goals.png)
 -->

각 사용자 지정 목표(목표)는 하나 이상의 전환 지표와 해당 지표의 상대적 가중치로 구성됩니다. 사용 가능한 전환 지표에는 Adobe Advertising 전환 픽셀을 사용하여 Adobe Analytics을 통해 추적된 모든 지표가 포함됩니다. DSP 사용자 지정 목표에는 비모바일 가중치만 고려되지만 모든 광고 유형에 사용됩니다.

예를 들어 세 개의 전환 지표가 캠페인 중 하나의 특정 패키지와 관련이 있다고 가정해 보겠습니다. &quot;PDF 다운로드&quot;(20 USD), &quot;이메일 등록&quot;(30 USD) 및 &quot;주문 확인&quot;(40 USD)입니다. 고객 조치의 일회성 통화 가치에 따라 가중치를 부여하려면 지표의 상대 가중치는 1, 1.5 및 2가 됩니다.

[사용자 지정 목표를 만들기](#custom-goal-create)하면 Adobe Sensei을 사용하여 보고 및 알고리즘 최적화를 위해 [패키지에 할당](/help/dsp/campaign-management/packages/package-settings.md)할 수 있습니다.

가중치 권장 사항은 목표의 DSP 기반 지표에 대해 자동으로 생성되며, 한 번의 클릭으로 모든 가중치 권장 사항을 적용할 수 있습니다. &quot;ADSP_&quot;가 접두사로 붙은 목표의 모든 가중치 변경 사항은 2일 이내에 DSP에서 알고리즘적으로 적용됩니다. 가중치 권장 사항에 대한 자세한 내용은 Search, Social 및 Commerce 내에서 사용할 수 있는 &quot;목표&quot;에 대한 최적화 안내서 장을 참조하십시오.

## 사용자 지정 목표 만들기 {#custom-goal-create}

사용자 지정 목표를 만들려면 [!DNL Search, Social, & Commerce] 클라이언트 설정 내에서 DSP 계정이 동일한 Adobe Experience Cloud 조직 ID를 가진 [!DNL Search, Social, & Commerce] 계정에 연결되어 있어야 합니다. DSP 계정이 [!DNL Search, Social, & Commerce] 계정에 연결되어 있지 않으면 Adobe 계정 팀에 문의하십시오.

1. [Advertising 검색, 소셜 및 Commerce에 로그인](/help/search-social-commerce/getting-started/sign-in.md){target="_blank"}.

1. 목표에 포함할 지표가 추적되고 제품에서 사용할 수 있는지 확인하고 표시 이름을 포함하십시오.

   1. 메인 메뉴에서 **[!UICONTROL Goals]** > **[!UICONTROL Conversions]**&#x200B;을(를) 클릭합니다.

      전환 보기는 새 브라우저 또는 브라우저 탭에서 열립니다.

   1. 지표를 찾고 지표에 대해 **[!UICONTROL Show in UI and Reports]**&#x200B;이(가) 활성화되어 있는지 확인하십시오.

      >[!NOTE]
      >
      >* [!DNL Analytics]개의 사용자 지정 이벤트가 이 명명 규칙을 따릅니다. `custom_event_[*event #*]_[*Analytics report suite ID*]`. 예: `custom_event_16_examplersid`

   1. 지표에 **[!UICONTROL Display Name]** 열의 값이 없으면 셀을 클릭하고 표시 이름을 입력한 다음 **[!UICONTROL Apply]을(를) 클릭합니다.**

1. [사용자 지정 목표를 *목표*](/help/search-social-commerce/new-ui/goals/objectives/objective-create.md){target="_blank"}(으)로 만듭니다. 다음 사항을 고려하십시오.

   * Advertising DSP 패키지에 사용되는 목표의 경우 목표 이름 앞에 &quot;ADSP_Registrations&quot;와 같은 &quot;ADSP_&quot;가 붙어야 합니다. 접두사는 대/소문자를 구분하지 않습니다.

   * DSP에 속하는 지표만 포함합니다. 검색, 소셜 및 Commerce 또는 기타 광고 네트워크에 속하는 모든 지표는 무시됩니다.

   * 하나 이상의 지표에는 지표 유형 *[!UICONTROL Goal]*&#x200B;이(가) 있어야 합니다.

   * DSP은 모든 광고에 비모바일 가중치를 사용합니다. 지정된 모든 모바일 가중치는 무시됩니다.

   >[!NOTE]
   >
   >* [!DNL Analytics]개의 사용자 지정 이벤트가 이 명명 규칙을 따릅니다. `custom_event_[*event #*]_[*Analytics report suite ID*]`. 예: `custom_event_16_examplersid`
   >* [!DNL Analytics]개의 차원 및 세그먼트를 Adobe Advertising 최적화에 사용할 수 없습니다.

   >[!TIP]
   >
   >최적의 성능을 위해서는 사용자 지정 목표(목표)의 결합된 지표가 하루에 10개 이상의 전환을 수행해야 합니다. 그렇지 않은 경우 제품 페이지나 애플리케이션 시작과 같은 추가 지원 전환 지표를 목표에 추가하는 것이 좋습니다. 지침이 필요하면 [사용자 지정 목표 작성에 대한 우수 사례](#custom-goal-best-practices)를 참조하십시오.

최적화 목표 &quot;[!UICONTROL Highest Return on Ad Spend (ROAS)"] 또는 &quot;[!UICONTROL Lowest Cost per Acquisition (CPA)]&quot;을(를) 사용하는 패키지의 DSP 패키지 설정에서 목표 이름이 이제 [!UICONTROL Custom Goals] 목록에 포함됩니다. 패키지의 사용자 지정 목표로 목표를 선택하면 [!UICONTROL Conversion Metric] 목록에 목표에 대한 모든 목표 지표가 포함됩니다.

## 사용자 지정 목표 빌드를 위한 우수 사례 {#custom-goal-best-practices}

### 단일 지표를 사용한 사용자 정의 목표

다음 예에서는 단일 전환 지표를 대상으로 하는 목표를 구성하는 방법을 보여 줍니다.

#### 최적화 목표가 &quot;[!UICONTROL Highest Return on Ad Spend (ROAS)]&quot;인 캠페인의 예

캠페인 목표가 매출([!UICONTROL Highest Return on Ad Spend (ROAS)])이고 모든 장치 유형의 매출이 동일하게 중요한 경우 비모바일 가중치가 1(1)인 &quot;[!UICONTROL Revenue]&quot; 지표를 포함하십시오. 모바일 가중치는 무시됩니다. 지표 유형 *[!UICONTROL Goal]*&#x200B;을(를) 선택하십시오.

<!-- update image or delete 

![example of a ROAS custom goal with a single conversion metric](/help/dsp/assets/custom-goal-roas.png)

-->

>[!NOTE]
>
> 비모바일 가중치는 1(으)로, 모든 디바이스에서 디스플레이 광고를 위해 추적된 매출의 각 $1에 대해 1(1)의 값과 동일합니다. 예를 들어 비모바일 가중치가 1인 $250 전환은 전환에 대해 $250로 보고됩니다. 전환 지표에 0.5의 비모바일 가중치가 할당되면 Adobe Advertising에서 $250 전환은 $125로 보고됩니다($250 전환 * 0.5 [!UICONTROL Non-mobile Weight] = $125).

#### 최적화 목표가 &quot;[!UICONTROL Lowest Cost per Acquisition (CPA)]&quot;인 캠페인의 예

캠페인 목표가 CPA(취득당 최저 비용)이고 성공 이벤트(예: &quot;애플리케이션 제출&quot;)가 하나만 필요한 경우 해당 지표를 하나 포함하고 지표 유형을 *[!UICONTROL Goal]*(으)로 지정하십시오. 가장 좋은 방법은 비모바일 가중치를 1로 설정하는 것입니다. 모바일 가중치는 무시됩니다.

<!-- update image or delete 

![example of a CPA custom goal with a single conversion metric](/help/dsp/assets/custom-goal-roas.png)

-->

>[!NOTE]
>
> 비모바일 가중치는 1(1)로, 모든 디바이스에서 디스플레이 광고를 위해 추적된 각 전환에 대해 1(1)의 값과 동일합니다. 예를 들어 10개의 애플리케이션 제출 전환이 추적되면 10개의 애플리케이션 제출 전환이 보고됩니다. 그러나 전환 지표에 0.5의 비모바일 가중치가 할당되면 Adobe Advertising에서 10개의 전환이 5개(10개 전환 * 0.5 [!UICONTROL Non-mobile Weight] = 5)로 보고됩니다.

### 여러 지표를 사용하는 사용자 정의 목표

사용자 지정 목표에서 여러 지표를 사용하는 두 가지 시나리오가 있습니다.

* 캠페인 목표에는 여러 개의 성공 이벤트가 있습니다. 예를 들어 두 개 이상의 온사이트 작업(PDF 다운로드, 연락처 및 이메일 등록)을 광고하는 경우 모든 작업은 CPA 목표에 기여하는 작업입니다. 목표에 각각 비모바일 가중치가 1인 세 개의 개별 지표가 포함되어 있는 경우 [!DNL Adobe Sensei] 알고리즘은 각 지표 및 사용자 장치 유형을 동일한 중요도로 처리합니다. 서로 다른 지표에 다양한 비용이나 중요도가 있는 경우 그에 따라 상대적 가중치를 조정합니다.

<!-- update image or delete it and adjust the wording above

   ![example of a custom goal with multiple metrics](/help/dsp/assets/custom-goal-multiple-properties.png)

-->

* 사용자 지정 목표의 단일 전환 지표는 최적화된 성능에 필요한 하루 최소 10개의 전환을 달성하지 못합니다. 이는 최소 일일 패키지 지출 또는 제한된 수의 자연 전환으로 인해 발생할 수 있습니다. 사용자 지정 목표에 추가 지원 지표를 추가하면 일별 전환 임계값 10개를 달성할 수 있습니다. 10개의 지원 이벤트는 각 가중치가 1보다 작은 경우에도 패키지가 10일 임계값을 충족하는 데 도움이 될 수 있습니다. 그러나 이러한 많은 이벤트를 추가할 필요는 없습니다.

  사용자 지정 목표에 지원 지표를 추가할 때 기본 성공 이벤트에 대한 상대적 중요도에 따라 가중치를 부여하고 데이터 포인트의 수량을 염두에 두십시오. 이렇게 하면 Adobe Sensei 알고리즘이 여러 지표의 균형을 맞추고 목표를 향해 최적화할 수 있습니다.

  다음 예제 목표에는 각각 다른 비모바일 가중치를 갖는 세 개의 지표(애플리케이션 제출 = 1, 애플리케이션 시작 = 0.1, 광고주 랜딩 페이지 = 0.01)가 포함됩니다. 즉, 각 애플리케이션 제출 전환은 평균 10개의 애플리케이션 시작 전환과 100개의 광고주 랜딩 페이지 전환과 동일한 값을 비즈니스에 제공합니다.

<!-- update image or delete it and adjust the wording above

   ![example of a custom goal with multiple metrics](/help/dsp/assets/custom-goal-multiple-properties2.png)

-->

대신, 랜딩 페이지 방문 횟수를 애플리케이션 제출과 동일하게 가중하면 랜딩 페이지 방문 횟수가 자연히 많을수록 목표를 압도하고 랜딩 페이지 방문 횟수로 왜곡될 수 있습니다.<!--reword-->

>[!MORELIKETHIS]
>
>* [최적화 목표 및 사용 방법](optimization-goals.md)
>* [패키지 설정](/help/dsp/campaign-management/packages/package-settings.md)
> * [DSP에서 캠페인을 최적화하는 방법](optimization-how-dsp-optimizes-campaigns.md)
