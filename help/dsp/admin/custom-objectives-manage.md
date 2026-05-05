---
title: 사용자 정의 목표 관리
description: 패키지 수준 최적화 목표를 충족하는 데 도움이 되는 성공 이벤트를 정의하는 방법에 대해 알아봅니다.
role: User, Admin
feature: DSP Optimization, DSP Packages
source-git-commit: e2746d58fa512f032a1e4ff851d23876cd63fc93
workflow-type: tm+mt
source-wordcount: '1312'
ht-degree: 0%

---

# 사용자 정의 목표 관리

*검색, 소셜 및 Commerce 계정에 연결된 DSP 계정에 사용 가능*

목표는 광고주가 비즈니스 목표를 달성하기 위해 설정하는 성공 이벤트를 정의합니다. 목표는 DSP 패키지에 [사용자 지정 목표](/help/dsp/campaign-management/packages/package-settings.md)(으)로 사용할 수 있습니다. 최적화 목표 &quot;[!UICONTROL Highest Return on Ad Spend (ROAS)"]&quot; 또는 &quot;[!UICONTROL Lowest Cost per Acquisition (CPA)]&quot;을(를) 사용하는 각 패키지에는 전체 최적화 목표를 달성하는 데 도움이 되도록 사용자 지정 목표가 포함되어야 합니다.

목표는 추적 및 최적화할 지표(속성)와 해당 지표의 상대 가중치로 구성됩니다. 각 목표에는 다음이 포함될 수 있습니다.

* 광고주의 기본 성공 지표를 나타내는 **[!UICONTROL Goal]지표**. 여기에는 일반적으로 매출, 리드 또는 매출과 같은 패키지의 핵심 비즈니스 결과가 포함됩니다. 각 목표에는 하나 이상의 목표 지표가 있어야 합니다.

* 목표 지표를 유도하는 데 도움이 되거나, 예측하거나, 선행하거나, 기여하는 선택적 **[!UICONTROL Assist]지표**. 테스트 드라이브 및 체험판과 같은 참여 지표를 예로 들 수 있습니다.

  [!DNL Adobe AI]이(가) 가중치 지원 이벤트를 자동으로 할당 및 업데이트하여 목표 이벤트를 최대화하도록 할 수 있습니다. 고유한 가중치 지원 지표를 할당하려는 경우 DSP에서 Adobe Advertising 및 Adobe Analytics의 과거 성능 데이터를 기반으로 하여 선택적으로 지원 지표를 추천할 수 있습니다. 권장 사항을 적용할지 여부를 선택할 수 있습니다.

목표 옵션에 대한 모든 변경사항은 필드 레벨에서 추적되고 변경 로그에 나열됩니다.

>[!PREREQUISITES]
>
>목표를 만들려면 먼저 DSP 계정이 검색, 소셜 및 Commerce 고객이 아닌 경우에도 동일한 Adobe Experience Cloud 조직 ID를 사용하여 검색, 소셜 및 Commerce 계정에 연결되어 있어야 합니다. DSP 계정이 [!DNL Search, Social, & Commerce] 계정에 연결되어 있지 않으면 Adobe 계정 팀에 문의하십시오.

>[!NOTE]
>
>* Advertising 검색, 소셜 및 Commerce 도 목표를 사용합니다. 최적화 기능이 포트폴리오에 대한 클릭 및 수익 모델을 만들 수 있도록 각 검색, 소셜 및 Commerce 포트폴리오에는 목표가 있어야 합니다.
>* 여러 DSP 패키지 및/또는 여러 검색, 소셜 및 Commerce 포트폴리오에 동일한 목표를 사용할 수 있습니다.

## 사용 가능한 지표

목표에 다음 중 하나를 포함할 수 있습니다.

* Adobe Advertising이 [Adobe Advertising 전환 추적 픽셀](/help/search-social-commerce/tracking/conversion-tracking-advertising.md)을 사용하여 추적하는 지표입니다.

* (광고주: [!DNL Adobe Analytics for Advertising]) [전환 및 사이트 참여 지표가 Adobe Analytics에서 동기화됨](/help/integrations/analytics/overview.md).

<!-- Do DSP-only clients have these? * [Advertiser-tracked metrics from conversion feed files](/help/search-social-commerce/tracking/conversion-tracking-about.md).  -->

## 목표 상태

[!UICONTROL Settings] > [!UICONTROL Custom Objectives] 보기는 각 목표의 상태를 나타냅니다. 값은 다음과 같습니다.

* *[!UICONTROL Waiting]*: 권장 사항이 생성될 때까지 목표가 초안 상태입니다.

* *[!UICONTROL Active]*: 목표가 저장되고 사용 가능합니다.

## 권장 사항 상태

* *[!UICONTROL Not Initiated]*: 권장 사항이 요청되지 않았습니다.

* *[!UICONTROL Generating]*: 권장 사항이 생성되고 있습니다.

* *[!UICONTROL Ready]*: 권장 사항을 적용할 수 있습니다.

* *[!UICONTROL Error]*: 권장 사항을 생성할 수 없습니다.

## 목표 만들기

1. 메인 메뉴에서 **[!UICONTROL Settings]>[!UICONTROL Custom Objectives]**&#x200B;을(를) 클릭합니다.

1. 오른쪽 상단에서 **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

1. [목표 설정](#custom-objective-settings)을 입력하십시오.

   자동화된 입찰을 선택하면 속성(지표)을 목표에 &quot;[!UICONTROL Goal]&quot; 지표로 할당할 수 있습니다. 사용자 지정 입찰의 경우 속성을 &quot;[!UICONTROL Goal]&quot; 또는 가중치가 적용된 &quot;[!UICONTROL Assist]&quot; 지표로 할당할 수 있지만 목표 지표를 하나 이상 포함해야 합니다.

   목표 및 지원 레이블은 최적화에 영향을 주지 않습니다. 포함된 지표의 가중치만 최적화에 영향을 줍니다.

1. (사용자 지정 입찰이 있는 목표, 선택 사항) 과거 성과 데이터를 기반으로 권장 지원 지표를 생성하려면 아래 섹션에서 **[!UICONTROL Generate]**&#x200B;을(를) 클릭하십시오. **[!UICONTROL Generate Recommendation]**&#x200B;에서 **[!UICONTROL Generate]**&#x200B;을(를) 클릭합니다.

   권장 지표는 생성하는 데 최대 20분이 소요됩니다. 권장 사항이 생성되는 동안 사용자 지정 목표의 상태는 *[!UICONTROL Waiting]*&#x200B;입니다. 권장 사항이 생성되면 &quot;[권장 지원 이벤트를 보고 적용](#view-apply-recommendations)&quot;할 수 있습니다.

1. (권장 사항을 생성하지 않은 경우) 오른쪽 상단에서 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

최적화 목표 &quot;[!UICONTROL Highest Return on Ad Spend (ROAS)"] 또는 &quot;[!UICONTROL Lowest Cost per Acquisition (CPA)]&quot;을(를) 사용하는 패키지의 [DSP 패키지 설정](/help/dsp/campaign-management/packages/package-settings.md)에서 목표 이름이 이제 [!UICONTROL Custom Goals] 목록에 포함됩니다. 패키지의 사용자 지정 목표로 목표를 선택하면 [!UICONTROL Conversion Metric] 목록에 목표에 대한 모든 목표 지표가 포함됩니다.

## 목표 편집

1. 메인 메뉴에서 **[!UICONTROL Settings]>[!UICONTROL Custom Objectives]**&#x200B;을(를) 클릭합니다.

1. 행에서 **..*** > **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. [목표 설정](#custom-objective-settings)을 변경합니다.

1. (권장 사항을 사용할 수 있는 경우, 선택 사항) 권장 지표를 보고 선택적으로 적용합니다.

   1. 아래 섹션에서 **[!UICONTROL View Recommendations]**&#x200B;을(를) 클릭합니다.

   1. 권장 사항을 적용하려면 다음 중 하나를 수행합니다.

      * 권장 사항 옆에 있는 **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

      * 수동으로 권장 사항을 조정한 다음 권장 사항 옆에 있는 **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

   1. [!UICONTROL Recommendations] 목록을 닫으려면 **[!UICONTROL Close]**&#x200B;을(를) 클릭하십시오.

   변경 사항은 목표 설정이 동기화된 후에 적용됩니다.

1. (사용자 지정 입찰이 있는 목표, 선택 사항) 과거 성과 데이터를 기반으로 권장 지원 지표를 생성하려면 아래 섹션에서 **[!UICONTROL Generate]**&#x200B;을(를) 클릭하십시오. **[!UICONTROL Generate Recommendation]**&#x200B;에서 **[!UICONTROL Generate]**&#x200B;을(를) 클릭합니다.

   권장 지표는 생성하는 데 최대 20분이 소요됩니다. 권장 사항이 생성되는 동안 사용자 지정 목표의 상태는 *[!UICONTROL Waiting]*&#x200B;입니다. 권장 사항이 생성되면 &quot;[권장 지원 이벤트를 보고 적용](#view-apply-recommendations)&quot;할 수 있습니다.

1. (새 권장 사항을 생성하지 않은 경우) 오른쪽 상단에서 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 권장 지원 이벤트 보기 및 적용 {#view-apply-recommendations}

*사용자 지정 입찰이 있는 목표*

목표 상태가 *[!UICONTROL Active]*&#x200B;이고 [!UICONTROL Recommendation Status]이(가) *[!UICONTROL Ready]*&#x200B;인 경우 권장 사항을 보고 선택적으로 적용할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Settings]>[!UICONTROL Custom Objectives]**&#x200B;을(를) 클릭합니다.

1. 행에서 **..*** > **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. 아래 섹션에서 **[!UICONTROL View Recommendations]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 권장 사항을 적용하려면 다음 중 하나를 수행합니다.

   * 권장 사항 옆에 있는 **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

   * 수동으로 권장 사항을 조정한 다음 권장 사항 옆에 있는 **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

1. [!UICONTROL Recommendations] 목록을 닫으려면 **[!UICONTROL Close]**&#x200B;을(를) 클릭하십시오.

1. 오른쪽 상단에서 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

   변경 사항은 목표 설정이 동기화된 후에 적용됩니다.

## 사용자 정의 목표에 대한 변경 로그 보기

1. 메인 메뉴에서 **[!UICONTROL Settings]>[!UICONTROL Custom Objectives]**&#x200B;을(를) 클릭합니다.

1. 행에서 **..*** > **[!UICONTROL Change Log]**&#x200B;을(를) 클릭합니다.

<!--

Not used as of 2/6. If added, verify and edit:

## Delete an objective

You can delete an objective that's not assigned to a package.

1. In the main menu, click **[!UICONTROL Settings] > [!UICONTROL Custom Objectives]**.

1. In the row, click **...*** > **[!UICONTROL Delete]**.

1. In the confirmation message, click **[!UICONTROL Confirm]**.

-->

## 사용자 정의 목표 설정 {#custom-objective-settings}

<!-- Are we going to keep the heading "Properties" rather than "Metrics" (or Events, which is mentioned in the UI? Need a consistent naming convention. Ideally, it should be the same as the new SSC UI. -->

| 섹션 | 매개 변수 | 설명 |
|---------|-----------|-------------|
| 기본 세부 정보 | AMOClient | 광고주의 고유한 Adobe Advertising ID입니다. |
| 기본 세부 정보 | 목표 이름 | 목표의 이름입니다.<br><br>Advertising DSP의 모든 목표 이름에는 &quot;ADSP_Registrations&quot;와 같이 &quot;ADSP_&quot;(대/소문자 구분 안 함)가 붙어야 합니다. 패키지에 할당할 때 식별하기 쉬운 이름을 사용합니다. |
|  | 설명 | (선택 사항) 목표에 대한 설명입니다. 사용자 정의 목표 목록의 이름 위에 커서를 놓으면 설명이 나타납니다. 설명을 포함하지 않으면 목표 이름이 대신 반복됩니다. |
| 입찰 전략 |  | 구성할 수 있는 이벤트 유형을 결정하는 목표의 입찰 전략:<ul><li><b>[!UICONTROL Automated Bidding]:</b> 속성(지표)을 [!DNL goal] 지표로 목표에 할당합니다. [!DNL Adobe AI]은(는) 균형 잡힌 funnel 접근 방식을 사용하여 목표 이벤트를 최대화하기 위해 가중 지원 이벤트를 자동으로 할당하고 업데이트합니다.</li><li><b>[!UICONTROL Custom Bidding]:</b> 속성을 &quot;[!DNL goal]&quot; 또는 가중치가 적용된 &quot;[!DNL assist]&quot; 이벤트로 할당하여 고유한 입찰 전략을 설정하십시오. 사전 정의된 전략에 이 고급 옵션을 사용합니다.</li></ul>입찰 전략을 변경하면 이전에 선택한 모든 지표가 지워집니다. |
| 속성 | [!UICONTROL Available Metrics] | 광고주를 위해 추적된 모든 지표. 지표를 목표로 추가하려면 지표 이름 옆에 있는 <b>[!UICONTROL Goal]</b>을(를) 클릭합니다. ([!UICONTROL Custom Bidding]만 해당) 할당된 목표 지표를 지원하는 지표를 추가하려면 지표 이름 옆에 있는 <b>[!UICONTROL Assist]</b>을(를) 클릭합니다.<br><br><b>참고:</b> [!DNL Analytics]개의 사용자 지정 이벤트가 이 명명 규칙을 따릅니다. `custom_event_[*event #*]_[*Analytics report suite ID*]`. 예: `custom_event_16_examplersid.` [!DNL Analytics] 차원 및 세그먼트를 Adobe Advertising 최적화에 사용할 수 없습니다.<br><br><b>팁:</b> 최적의 성능을 위해 사용자 지정 목표(목표)의 결합된 지표는 하루에 총 10회 이상이어야 합니다. 그렇지 않은 경우 제품 페이지나 애플리케이션 시작과 같은 추가 지원 전환 지표를 목표에 추가하는 것이 좋습니다. 지침이 필요하면 [사용자 지정 목표 작성에 대한 우수 사례](#custom-goal-best-practices)를 참조하십시오. |
|  | 선택한 지표 | 목표에 포함된 각 전환 지표의 이름입니다. 다음 중 하나를 수행합니다.<ul><li>지표를 목표로 추가하려면 [!UICONTROL Available Metrics] 열의 지표 이름 옆에 있는 <b>[!UICONTROL Goal]</b>을(를) 클릭합니다.</li><li>([!UICONTROL Custom Bidding] 전략만 해당) 할당된 목표 지표를 지원하는 지표를 추가하려면 [!UICONTROL Available Metrics] 열의 지표 이름 옆에 있는 <b>[!UICONTROL Assist]</b>을(를) 클릭합니다. 그런 다음 목표에 있는 다른 지표에 대한 지표의 숫자 가중치를 입력합니다. 가중치는 0.001 내지 1이어야 하며, 소수를 포함할 수 있다. 기본 가중치는 1입니다.</li><li>([!UICONTROL Custom Bidding] 전략만 해당) 지원 지표의 가중치를 편집하려면 필드 내부를 클릭하고 목표의 다른 지표와 관련된 지표의 숫자 가중치를 입력합니다. 가중치는 0(영)보다 커야 하며 소수를 포함할 수 있습니다. 기본 가중치는 1입니다.</li><li>목표에서 지표를 제거하려면 지표 이름 위에 커서를 놓고 **[!UICONTROL X]**./li>을(를) 클릭합니다</ul>**메모:**<ul><li>다른 지표와 해당 가중치가 상대적으로 적절한지 확인하십시오. 예를 들어 달러 금액과 개수를 직접 비교할 수는 없습니다.</li><li>객관적 가중치 간의 상대적 변화가 크면 성능에 일시적 변동성이 발생할 수 있으므로 변화 후 성과를 모니터링한다.</li></ul>. |

>[!MORELIKETHIS]
>
>* [최적화 목표 및 사용 방법](/help/dsp/optimization/optimization-goals.md)
>* [사용자 지정 목표에 대한 모범 사례](/help/dsp/optimization/custom-goal.md)
>* [패키지 설정](/help/dsp/campaign-management/packages/package-settings.md)
>* [전환 관리](/help/dsp/admin/conversion-metrics-manage.md)
