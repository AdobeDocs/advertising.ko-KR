---
title: (새 UI)  [!DNL Google Ads] 전환 값 규칙 관리
description: 검색, 소셜 및 Commerce에서  [!DNL Google Ads] 전환 값 규칙을 보고 관리하는 방법을 알아봅니다.
feature: Conversions
feature_v2:
  - id: e6916c1b-e939-4e0b-99f5-768e83e1e99f
  - id: aed5e38a-3e62-42fa-8d16-cd080729b2a0
subfeature_v2:
  - id: a2f79fa9-a8fe-4c1c-961e-75dc3c47f954
source-git-commit: bf1ca7f6133c19bb68dbe0395416dca8ef647464
workflow-type: tm+mt
source-wordcount: 1844
ht-degree: 0%

---

# (새 UI) [!DNL Google Ads] 전환 값 규칙 관리

*Beta 기능*

[!DNL Google Ads] [전환 값 규칙](https://support.google.com/google-ads/answer/10518330)을(를) 사용하면 장치 유형, 위치 및 대상 세그먼트를 포함한 사용자 정보를 기반으로 전환 이벤트의 값을 조정할 수 있습니다. Google 스마트 입찰을 사용하여 검색, 디스플레이, 쇼핑 및 성과 최대 캠페인에서 가치 기반 입찰에 대한 규칙을 사용할 수 있습니다. 전환 최대화 및 Target ROAS 입찰 전략이 있는 캠페인의 경우 [!DNL Google Ads] 알고리즘이 더 높은 값으로 전환을 선호하기 시작합니다.

캠페인 수준 전환 값 규칙은 계정 수준 규칙을 재정의합니다. 전환이 여러 전환 값 규칙을 충족하면 규칙 중 하나만 적용됩니다. 일반적으로 가장 구체적인 규칙이 적용되지만, 다른 규칙 조건 유형의 우선 순위에 대해서는 [[!DNL Google Ads] 설명서를 참조하십시오](https://support.google.com/google-ads/answer/10520348).

## [!UICONTROL Conversion Value Rules] 보기 및 기능

Search, Social 및 Commerce은 [!DNL Google Ads] 계정의 전환 값 규칙을 자동으로 동기화합니다. [!DNL Google Ads] 인터페이스에서 만든 모든 규칙은 24시간 내에 동기화되며 [!UICONTROL Goals] > [!UICONTROL Conversion Value Rules] 보기에서 사용할 수 있습니다.

일부 계정은 전환 값 규칙을 관리할 수 있습니다.

* 개별 계정 또는 캠페인 수준에서 전환을 추적하는 계정에서 계정 수준 및 캠페인 수준 규칙의 상태를 [만들기](#google-conversion-value-rule-create), [편집](#google-conversion-value-rule-edit) 및 [변경](#google-conversion-value-rule-change-status)할 수 있습니다.

  계정은 [[!DNL Google Ads] 관리자 계정](/help/search-social-commerce/new-ui/)에 연결할 수 있지만 계정 간 전환 추적을 사용할 수 없습니다(이 경우 관리자 계정의 모든 계정에서 전환이 추적됨).

* 계정 간 전환 추적을 사용하는 계정의 계정 수준 및 캠페인 수준 규칙은 관리자 계정에서 상속되며 읽기 전용입니다.

## 검색, 소셜 및 Commerce 포트폴리오가 있는 전환 값 규칙

광고주 계정이 검색, 소셜 및 Commerce 목표를 [!DNL Google Ads]에 업로드하도록 구성되어 있고 목표가 있는 포트폴리오에 전환 값 규칙을 사용하는 캠페인을 포함하면 [!DNL Google Ads]이(가) 목표에 지정된 원래 전환 값에 전환 값 규칙을 적용합니다. 따라서 Search, Social 및 Commerce의 전환 데이터가 [!DNL Google Ads]의 전환 데이터와 다릅니다.

예를 들어 목표가 단일 전환 지표 &quot;잠재 고객&quot;을 사용하고 모바일 장치에서 전환한 가중치를 10으로 제공하고 비모바일 장치에서 전환한 가중치를 10으로 제공한다고 가정해 보겠습니다. Search, Social 및 Commerce은 두 장치 유형의 이벤트를 1개의 전환으로 계산하고 전환 값을 10으로 크레딧합니다. 그러나 해당 포트폴리오의 캠페인이 전환 값 규칙 &quot;장치가 모바일인 경우 2를 곱하십시오.&quot;를 사용한다고 가정해 봅시다. 해당 캠페인에 대해 모바일 잠재 고객 이벤트가 추적되면 [!DNL Google Ads]도 전환 수를 1로 크레딧하지만 전환 값은 (10 x 2) = 20으로 크레딧합니다.

규칙이 적용되기 전의 원래 전환 값을 포함하여 규칙에 대한 자세한 내용은 [의 전환 값 규칙 보고서 [!DNL Google Ads]](https://support.google.com/google-ads/answer/10519848)를 참조하십시오.

## [!DNL Google Ads] 전환 값 규칙 만들기 {#google-conversion-value-rule-create}

[!DNL Google Ads] 계정에 계정 수준 및 캠페인 수준 전환 값 규칙을 만들 수 있으며, 이 규칙을 통해 전환은 개별 계정 수준 또는 하위 계정 수준에서 추적됩니다. 마스터 계정 수준에서 추적되는 계정 간 전환이 있는 계정에 대한 규칙을 만들 수 없습니다.

각 규칙에는 최대 2개의 조건과 해당 조건이 충족될 때 적용할 전환값 조정이 포함됩니다. 계정의 모든 규칙은 동일한 유형의 기본 및 (선택 사항) 보조 조건을 사용해야 합니다. 예를 들어 규칙 1에 기본 조건 &quot;대상&quot;과 보조 조건 &quot;위치&quot;가 포함되어 있으면 계정의 다른 모든 규칙에는 기본 조건 &quot;대상&quot;이 있어야 합니다. 다른 규칙에 보조 조건이 포함된 경우 &quot;위치&quot;여야 합니다.

각 캠페인에 대해 여러 캠페인 수준 규칙을 만들 수 있습니다. 그러나 [!DNL Google Ads]은(는) 계정 수준 규칙이 이미 있는 경우 [!DNL Google Ads] 편집기 외부에서 새 계정 수준 규칙을 만들 수 있는 기능을 아직 제공하지 않습니다. 추가 계정 수준 규칙을 만들려면 [!DNL Google Ads]에 직접 로그인한 다음 [!DNL Google Ads] 편집기를 사용하십시오.

**참고:** 캠페인 수준 전환 값 규칙은 계정 수준 규칙을 재정의하며 전환에는 하나의 규칙만 적용할 수 있습니다. 자세한 내용은 [방법 [!DNL Google Ads] 전환이 여러 규칙에 대한 조건을 충족할 때 전환에 적용되는 규칙을 결정합니다](https://support.google.com/google-ads/answer/10520348).

1. 메인 메뉴에서 **[!UICONTROL Goals]>[!UICONTROL Conversion Value Rules]**&#x200B;을(를) 클릭합니다.

   기본적으로 **[!UICONTROL Campaign]** 탭이 선택되어 모든 캠페인 수준 규칙을 표시합니다.

1. (선택 사항) 계정 수준 규칙을 대신 만들려면 **[!UICONTROL Account]** 탭을 클릭합니다.

1. 도구 모음에서 **[!UICONTROL Create Campaign Rule]**([!UICONTROL Campaign] 탭) 또는 **[!UICONTROL Create Account Rule]**([!UICONTROL Account] 탭)을 클릭합니다.

1. 광고 네트워크 및 계정을 선택합니다. 캠페인 수준 규칙의 경우 캠페인도 선택합니다. **[!UICONTROL Next]**&#x200B;을(를) 클릭합니다.

1. [전환 규칙 설정](#google-ads-conversion-value-rule-settings)을 구성하십시오.

   기본 조건 및 값 조정을 구성해야 합니다. 선택적으로 보조 조건을 구성할 수 있습니다.

   조건 내에서 부울 연산자 `OR`을(를) 사용하여 여러 대상 또는 제외를 연결하므로 값 조정을 시작하는 모든 옵션을 충족할 수 있습니다. 보조 조건을 포함할 때 부울 연산자 `ALL`을(를) 사용하여 보조 조건이 기본 조건에 결합되므로 값 조정을 시작하려면 두 조건을 모두 충족해야 합니다. 예: \[위치가 알제리 또는 튀니지\]이고 \[장치가 모바일 또는 태블릿\]인 경우 1.5를 추가합니다.

   **참고:** 계정의 모든 규칙은 같은 유형의 기본 및 (선택 사항) 보조 조건을 사용해야 합니다. 예를 들어 규칙 1에 기본 조건 &quot;대상&quot;과 보조 조건 &quot;위치&quot;가 포함되어 있으면 계정의 다른 모든 규칙에는 기본 조건 &quot;대상&quot;이 있어야 합니다. 다른 규칙에 보조 조건이 포함된 경우 &quot;위치&quot;여야 합니다.

1. 설정을 검토하려면 **[!UICONTROL Review and Save]**&#x200B;을(를) 클릭하십시오.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## [!DNL Google Ads] 전환 값 규칙 편집 {#google-conversion-value-rule-edit}

전환이 개별 계정 수준 또는 하위 계정 수준에서 추적되는 계정/캠페인에서 전환 값 규칙을 편집할 수 있습니다. 마스터 계정 수준에서 추적되는 계정 간 전환이 있는 계정에 대한 규칙을 편집할 수 없습니다.

1. 메인 메뉴에서 **[!UICONTROL Goals]>[!UICONTROL Conversion Value Rules]**&#x200B;을(를) 클릭합니다.

   기본적으로 **[!UICONTROL Campaign]** 탭이 선택되어 모든 캠페인 수준 규칙을 표시합니다.

1. (선택 사항) 대신 모든 계정 수준 규칙을 보려면 **[!UICONTROL Account]** 탭을 클릭하십시오.

1. 규칙 옆에 있는 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 (/help/search-social-commerce/assets/edit-new.png &quot;편집)을 클릭합니다.

1. [전환 규칙 설정](#google-ads-conversion-value-rule-settings)을(를) 편집합니다.

   기존 규칙의 조건 유형은 편집할 수 없지만 조건 및 값 조정은 편집할 수 있습니다.

   기본 조건 및 값 조정을 구성해야 합니다. 선택적으로 보조 조건을 구성할 수 있습니다.

   **참고:** 보조 조건을 추가하는 경우 계정의 다른 규칙과 같은 조건 형식이어야 합니다. 예를 들어, 계정의 규칙 1 다른 규칙에 보조 조건 &quot;위치&quot;가 있는 경우 다른 규칙에 보조 조건이 포함되어 있으면 보조 조건은 &quot;위치&quot;여야 합니다. 보조 조건을 포함할 때 부울 연산자 `ALL`을(를) 사용하여 보조 조건이 기본 조건에 결합되므로 값 조정을 시작하려면 두 조건을 모두 충족해야 합니다.

1. 설정을 검토하려면 **[!UICONTROL Review and Save]**&#x200B;을(를) 클릭하십시오.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## [!DNL Google Ads] 전환 값 규칙의 상태 변경 {#google-conversion-value-rule-change-status}

개별 계정 수준에서 전환이 추적되는 계정 및 캠페인에서 전환 값 규칙을 일시 중지, 활성화 또는 삭제할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Goals]>[!UICONTROL Conversion Value Rules]**&#x200B;을(를) 클릭합니다.

   기본적으로 **[!UICONTROL Campaign]** 탭이 선택되어 모든 캠페인 수준 규칙을 표시합니다.

1. (선택 사항) 대신 모든 계정 수준 규칙을 보려면 **[!UICONTROL Account]** 탭을 클릭하십시오.

1. 변경할 각 행 옆의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서

   * 일시 중지된 규칙을 활성화(활성화)하려면 **[!UICONTROL ...]>[!UICONTROL Activate]**&#x200B;을(를) 클릭합니다.

   * 활성 규칙을 일시 중지하려면 **[!UICONTROL ...]>[!UICONTROL Pause]**&#x200B;을(를) 클릭합니다.

   * 활성 또는 일시 중지된 규칙을 삭제하려면 ![삭제](/help/search-social-commerce/assets/delete.png "삭제")를 클릭하십시오.

1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

## [!DNL Google Ads] 전환 값 규칙 설정 {#google-conversion-value-rule-settings}

| 섹션 | 매개 변수 | 설명 |
|---|---|---|
| [!UICONTROL Select Campaign] | [!UICONTROL Network] | 광고 네트워크입니다. |
| | [!UICONTROL Account] | 광고 네트워크 계정입니다. |
| | [!UICONTROL Campaign] | (캠페인 수준 전환 값 규칙만 해당) 광고 캠페인. |
| [!UICONTROL Conditions] > [!UICONTROL Primary Condition] | \[조건 유형\] | (기존 규칙의 읽기 전용) 값 조정을 트리거하기 위해 충족해야 하는 조건 유형:<ul><li>*[!UICONTROL Device]:* 모든 또는 특정 장치 형식을 대상으로 합니다.</li><li>*[!UICONTROL Location]:* 모든 국가 및 지역을 대상으로 하거나 특정 위치를 대상으로 하고 제외합니다.</li><li>*[!UICONTROL Audiences]:* 모든 또는 특정 대상을 타깃팅하려면</li></ul>**참고:** 계정의 모든 규칙은 같은 유형의 기본 및 (선택 사항) 보조 조건을 사용해야 합니다. 예를 들어 규칙 1에 기본 조건 &quot;대상&quot;과 보조 조건 &quot;위치&quot;가 포함되어 있으면 계정의 다른 모든 규칙에는 기본 조건 &quot;대상&quot;이 있어야 합니다. 다른 규칙에 보조 조건이 포함된 경우 &quot;위치&quot;여야 합니다. |
| | \[조건 유형\] > [!UICONTROL Device] 및 [!UICONTROL Device Level] | (장치 조건만 해당) 타깃팅할 장치 유형:<ul><li>*[!UICONTROL All devices]:** 모든 장치 형식을 대상으로 합니다.</li><li>*[!UICONTROL Select devices]:* 대상에 하나 이상의 장치 유형을 지정하려면: *[!UICONTROL Desktop]:*, *[!UICONTROL Mobile]* 및 *[!UICONTROL Tablet]:*.</li></ul>조건 내에서 부울 연산자 `OR`을(를) 사용하여 여러 대상을 연결하므로 값 조정을 시작하는 모든 옵션을 충족할 수 있습니다. 예: \[Device is Mobile OR Tablet\]인 경우 1.5를 추가합니다. |
| | \[조건 유형\] > [!UICONTROL Location] 및 [!UICONTROL Location Level] | (위치 조건만 해당) 위치 대상 및 제외:<ul><li>*[!UICONTROL All countries and territories]:* 모든 국가 및 위치를 대상으로 하거나 특정 위치를 대상으로 하고 제외합니다.</li><li>*[!UICONTROL Enter a location]:* 특정 위치를 타깃팅하고 제외합니다.</li></ul><ul><li>위치 또는 하위 위치를 확장하려면 이름 뒤에 있는 `>`을(를) 클릭합니다.</li><li>대상을 추가하려면 대상을 한 번 선택하여 녹색 확인 표시를 표시합니다.</li><li>대상을 제외하려면 빨간색 **[!UICONTROL X]**&#x200B;을(를) 표시하도록 대상을 다시 선택하십시오.</li><li>대상 또는 제외를 제거하려면 다음 중 하나를 수행합니다.<ul><li>[!UICONTROL Selections] 열의 항목 옆에 있는 ![삭제](/help/search-social-commerce/assets/delete.png "삭제")를 클릭합니다.</li><li>확인 표시 또는 [!UICONTROL X]이(가) 나타나지 않을 때까지 대상을 선택하십시오.</li></ul></li></ul>조건 내에서 부울 연산자 `OR`을(를) 사용하여 여러 대상 또는 제외를 연결하므로 값 조정을 시작하는 모든 옵션을 충족할 수 있습니다. 예: \[위치가 알제리 또는 튀니지\]이면 1.5를 추가합니다. |
| | \[조건 유형\] > [!UICONTROL Audience] 및 [!UICONTROL Audience Level] | (대상 조건만 해당) 대상은 다음과 같습니다.<ul><li>*[!UICONTROL All audience segments]:* 대상 세그먼트 [!DNL Google Ads]개를 모두 대상으로 합니다.</li><li>특정 [!DNL Google Ads]개 대상 세그먼트를 대상으로 *[!UICONTROL Enter audience segments]:*.</li></ul><ul><li>범주 또는 하위 범주를 해당 세그먼트로 확장하려면 이름 뒤에 있는 `>`을(를) 클릭합니다.</li><li>대상을 추가하려면 대상을 선택합니다.</li><li>대상을 제거하려면 대상을 선택 취소하거나 [!UICONTROL Selection] 열의 항목 옆에 있는 ![삭제](/help/search-social-commerce/assets/delete.png "삭제")를 클릭합니다.</li></ul>조건 내에서 부울 연산자 OR를 사용하여 여러 대상 또는 제외를 결합하므로 값 조정을 시작하는 데 모든 옵션이 충족될 수 있습니다. 예: \[대상이 할인 여행자 또는 가족 휴가객\]인 경우 1.5를 추가합니다.<br><br>**참고:** 대상 대상을 저장하면 대상을 추가할 수 있지만 [!DNL Google Ads] 편집기 외부에서 대상을 제거할 수 없습니다. 대상 대상을 제거해야 하는 경우 [!DNL Google Ads]에 직접 로그인한 다음 [!DNL Google Ads] 편집기를 사용하십시오. |
| [!UICONTROL Conditions] > [!UICONTROL Secondary Condition] | \[조건 유형\] | (선택 사항, 기존 규칙의 경우 읽기 전용) 값 조정을 트리거하기 위해 충족해야 하는 조건 유형입니다. 보조 조건을 포함할 때 부울 연산자 `ALL`을(를) 사용하여 보조 조건이 기본 조건에 결합되므로 값 조정을 시작하려면 두 조건을 모두 충족해야 합니다. 예: \[위치가 알제리 또는 튀니지\]이고 \[장치가 모바일 또는 태블릿\]인 경우 1.5를 추가합니다.<br><br>설명은 기본 조건의 항목을 참조하십시오.<br><br>**참고:** 계정의 모든 규칙은 동일한 유형의 기본 및 (선택 사항) 보조 조건을 사용해야 합니다. 예를 들어 규칙 1에 기본 조건 &quot;대상&quot;과 보조 조건 &quot;위치&quot;가 포함되어 있으면 계정의 다른 모든 규칙에는 기본 조건 &quot;대상&quot;이 있어야 합니다. 다른 규칙에 보조 조건이 포함된 경우 &quot;위치&quot;여야 합니다. |
| [!UICONTROL Value Adjustment] | [!UICONTROL Adjustment Operation] 및 [!UICONTROL Adjustment Value] | 조정 유형을 지정한 다음 양수 값을 입력합니다.<ul><li>*[!UICONTROL Add]:* 전달된 전환 값에 지정된 값을 추가합니다. 값은 0보다 커야 합니다.</li><li>*[!UICONTROL Multiply]:*&#x200B;은(는) 전달된 전환 값에 지정된 값을 곱합니다. 값은 0.5에서 10 사이여야 합니다.</li></ul> |

<!--
>[!MORELIKETHIS]
>
>* 
-->
