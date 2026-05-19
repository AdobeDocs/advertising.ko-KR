---
title: 재사용 가능한 대상 만들기
description: 대상 세그먼트 및 다른 저장된 대상으로 구성된 재사용 가능한 대상을 만드는 방법을 알아봅니다. 필요한 경우 타겟 대상을 자연어 프롬프트로 설명하여 AI 지원 대상 에이전트를 사용합니다. 에이전트는 타겟 또는 제외로 사용할 서드파티 세그먼트를 제안하고 대상 표현식을 빌드합니다.
feature: DSP Audiences
exl-id: 5f4a0abb-c285-4452-a6c3-a91d5281df9b
TQID: https://experienceleague.adobe.com/KhAxVTvMx4yBz3tfDtng3nOur2IodZAFFHMUQM1lKhQ
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2:
  - id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
subfeature_v2:
  - id: fef5c122-6482-4d17-a8ce-4e70b906f1f4
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: a4b509995f362ed81e00485409b0c729b5130e35
workflow-type: tm+mt
source-wordcount: 1667
ht-degree: 0%

---

# 재사용 가능한 대상 만들기

<!-- "Saved audience" is used in UI (where?), but "saved" is a state, not a type. "Reusable audience" sounds better in a description. "Audience template" isn't right, either, since it implies you can edit it on the fly to create a new, different audience. Some other term? -->

대상 세그먼트 및 여러 배치에 대한 타겟 또는 제외로 사용할 수 있는 기타 저장된 대상의 그룹인 재사용 가능한 대상을 저장하고 관리할 수 있습니다. 명시된 요구 사항에 따라 사용할 수 있는 모든 자사 및 타사 세그먼트를 사용하여 재사용 가능한 새 대상을 생성하려면 수동으로 대상을 만들거나 AI 지원 대상 에이전트를 사용하십시오.

>[!NOTE]
>
>(DSP에서 해시된 이메일 ID를 LiveRamp RampID 세그먼트로 변환하는 광고주) 활성, 예약됨 또는 일시 중지된 배치에 첨부되지 않은 자사 RampID 세그먼트는 일시 중지됩니다. 세그먼트는 세그먼트 목록에 &quot;자동 일시 중지됨&quot;으로 표시됩니다.

## 재사용 가능한 대상 수동 만들기

1. 메인 메뉴에서 **[!UICONTROL Audiences]** > **[!UICONTROL All Audiences]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위에서 **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

1. [!UICONTROL New Audience] 설정에서:

   1. 고유한 **[!UICONTROL Audience Name]**&#x200B;을(를) 입력하십시오.

   1. (선택 사항) **[!UICONTROL Share with all advertisers in my account]** 옵션을 선택 취소합니다.

      대상을 공유하면 해당 대상은 계정 내의 모든 광고주에게 타겟 또는 제외로 사용할 수 있습니다. 그러나 대상자의 개별 세그먼트는 세그먼트가 공유된 사용자만 사용할 수 있습니다. 예를 들어 동일한 [!DNL Analytics] 계정에 매핑되지 않은 광고주와 Adobe Analytics 세그먼트가 포함된 대상을 공유하는 경우 해당 광고주의 해당 대상에서는 세그먼트가 미리 표시되지 않습니다. 해당 광고주가 사용할 수 있는 세그먼트만 대상에서 미리 봅니다.

   1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

1. 오른쪽 패널에서 **[!UICONTROL Switch to manual mode]** 단추를 클릭합니다.

   AI 옵션이 기본값입니다.

1. 대상자 작성:

   >[!NOTE]
   >
   >대상을 만들면 자세한 [대상 크기 데이터](audience-about.md)가 오른쪽 패널에서 업데이트됩니다

   * [[!UICONTROL Third Party Segments], [!UICONTROL First Party Segments], [!UICONTROL Adobe Segments], [!UICONTROL Custom Segments] 및 [!UICONTROL Saved Audiences] 탭](audience-settings.md)에서 사용 가능한 세그먼트를 사용하여 수동으로 세그먼트 논리를 만들려면 다음을 수행하십시오.

      * (선택 사항) 세그먼트 이름, 설명 또는 경로를 검색합니다.

        검색 결과에는 사용하는 정확한 용어에 따라 세그먼트가 포함됩니다. 여러 용어를 입력할 때 세그먼트에 대한 모든 용어를 찾아야 합니다.

      * 첫 번째 세그먼트를 추가하려면 왼쪽 패널에서 세그먼트를 찾은 다음 세그먼트 이름 옆에 있는 확인란을 선택합니다.

      * 기존 세그먼트 그룹에 세그먼트를 추가하려면 다음 작업을 수행하십시오.

         1. 오른쪽 패널에서 세그먼트 그룹을 클릭합니다.

         1. (선택 사항) 필요에 따라 그룹 논리를 *[!UICONTROL Include Any]*, *[!UICONTROL Include All]* 또는 *[!UICONTROL Exclude All]*(으)로 변경합니다.

            *[!UICONTROL Exclude All]*&#x200B;은(는) 첫 번째 세그먼트 그룹에서 사용할 수 없습니다. 제외만 포함하는 대상의 경우 이 대상을 *[!UICONTROL Include Any]*(으)로 만든 다음 배치 내에서 제외된 대상 메뉴에서 해당 대상을 선택합니다.

         1. 왼쪽 패널에서 새 세그먼트를 찾은 다음 세그먼트 이름 옆에 있는 확인란을 선택합니다.

            세그먼트 그룹이 새 세그먼트로 자동으로 업데이트됩니다.

      * 새 세그먼트 그룹을 추가하려면:

         1. 오른쪽 패널에서 **[!UICONTROL + New Group]**&#x200B;을(를) 클릭합니다.

            1. (선택 사항) 필요에 따라 이전 그룹과 새 그룹 간의 논리를 *[!UICONTROL And]* 또는 *[!UICONTROL Or]*(으)로 변경합니다.

            1. 왼쪽 패널에서 새 그룹의 세그먼트를 찾은 다음 세그먼트 이름 옆에 있는 확인란을 선택합니다.

            1. (선택 사항) 필요에 따라 그룹 논리를 *[!UICONTROL Include Any]*, *[!UICONTROL Include All]* 또는 *[!UICONTROL Exclude All]*(으)로 변경합니다.

   * 기존 대상의 세그먼트 논리를 사용하려면 다음을 수행합니다.

      1. 다음 방법 중 하나로 기존 대상에서 세그먼트 논리를 복사합니다.

         * 모든 대상 보기에서 대상 행 위에 커서를 놓고 **[!UICONTROL More]** > **[!UICONTROL Copy to Clipboard]**&#x200B;을(를) 클릭합니다.

         * 기존 대상에 대한 설정에서 세그먼트 논리 패널의 맨 위에서 **[!UICONTROL More]** > **[!UICONTROL Copy to Clipboard]**&#x200B;을(를) 클릭합니다.

         * 텍스트 편집기에서 영숫자 세그먼트 ID와 [부울 구문](audience-segment-logic-syntax.md)을 사용하여 세그먼트 논리를 수동으로 만든 다음 클립보드에 복사합니다.

      1. **[!UICONTROL paste in an audience rule to begin building]**&#x200B;을(를) 클릭하고 기존 세그먼트 논리를 입력 필드에 붙여 넣은 다음 **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

         >[!NOTE]
         >
         >대상에 이미 세그먼트 논리가 포함되어 있는 경우 새 세그먼트 논리에 붙여넣으면 기존 논리를 덮어씁니다.

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

## 생성 AI를 사용하여 재사용 가능한 대상 만들기

*Beta 기능*

*영어만 지원*

>[!NOTE]
>
>이 기능은 베타 모드이며 변경될 수 있습니다. 대상을 만들고 배치에 사용하기 전에 생성된 대상 표현식이 원하는 대상을 나타내는지 확인하십시오.

<!-- Later:  Audiences built using generative AI have the indicator [icon] in **[!UICONTROL Audiences] > [!UICONTROL All Audiences]**. -->

1. 메인 메뉴에서 **[!UICONTROL Audiences]** > **[!UICONTROL All Audiences]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위에서 **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

1. [!UICONTROL New Audience] 설정에서:

   1. 고유한 **[!UICONTROL Audience Name]**&#x200B;을(를) 입력하십시오.

   1. (선택 사항) **[!UICONTROL Share with all advertisers in my account]** 옵션을 선택 취소합니다.

      대상을 공유하면 해당 대상은 계정 내의 모든 광고주에게 타겟 또는 제외로 사용할 수 있습니다. 그러나 대상자의 개별 세그먼트는 세그먼트가 공유된 사용자만 사용할 수 있습니다. 예를 들어 동일한 [!DNL Analytics] 계정에 매핑되지 않은 광고주와 Adobe Analytics 세그먼트가 포함된 대상을 공유하는 경우 해당 광고주의 해당 대상에서는 세그먼트가 미리 표시되지 않습니다. 해당 광고주가 사용할 수 있는 세그먼트만 대상에서 미리 봅니다.

   1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

1. 대상자 작성:

   1. 포함 및 제외할 대상 특성을 설명하는 하나 이상의 프롬프트를 입력합니다. 각 프롬프트를 제출하려면 ![프롬프트 제출](/help/dsp/assets/submit-prompt.png "프롬프트 제출")을 클릭하십시오.

      자세한 내용은 &quot;[프롬프트 작성](#writing-prompts)&quot; 및 &quot;[대상자 개요 작성에 대한 모범 사례](#audience-brief-best-practices)&quot;를 참조하십시오.

      해당하면 에이전트는 보다 효과적인 대상 개요를 만드는 데 도움이 되는 추가 세그먼트 필터를 제안합니다. 제안을 수락하거나 거부할 수 있습니다.

      대상 에이전트가 관련 세그먼트를 찾을 때 기준에 따라 부울 대상 표현식을 만듭니다. 또한 대상을 취합할 일치하는 세그먼트를 찾기 전에 승인을 요청합니다. 선택적으로 요청을 무시하고 대신 추가 대상 기준을 계속 지정할 수 있습니다.

   1. 대상 에이전트가 대상을 적절히 설명하는 대상 표현식을 제공하면 대상 에이전트에게 대상 어셈블 작업을 진행하도록 알립니다.

      &quot;진행&quot;, &quot;확인&quot;, &quot;확인&quot;, &quot;예&quot; 또는 다른 유사한 단어를 입력할 수 있습니다. 에이전트는 각 트레이트에 대해 제안된 모든 세그먼트(예: &quot;상위&quot;)를 나열합니다. 트레이트를 확장하여 해당 트레이트에 대해 제안된 개별 세그먼트에 대한 세부 정보를 확인합니다.

   1. (필요한 경우) 추가 기준을 지정합니다. 대상 에이전트가 모든 기준을 충족하는 대상 표현식을 제공하면 대상 조립을 진행하도록 대상 에이전트에게 알립니다.

      대상을 모으려면 &quot;진행&quot;, &quot;확인&quot;, &quot;확인&quot;, &quot;예&quot; 또는 다른 유사한 단어를 입력합니다. 에이전트는 각 트레이트에 대해 제안된 모든 세그먼트(예: &quot;상위&quot;)를 나열합니다. 트레이트를 확장하여 해당 트레이트에 대해 제안된 개별 세그먼트에 대한 세부 정보를 확인합니다.

1. 어셈블된 대상자에 동의하면 **[!UICONTROL Create]**&#x200B;을(를) 클릭하여 지정된 대상자를 만듭니다.

   >[!NOTE]
   >
   >나중에 대상자 에이전트를 사용하여 대상자를 편집할 수 없습니다. 대신 [대상 식을 수동으로 편집](/help/dsp/audiences/reusable-audience-edit.md)하세요.

### 프롬프트 작성의 기본 사항 {#writing-prompts}

<!-- Change heading level for this whole section to fit under AI procedure -->

#### 프롬프트에 포함해야 하는 것은 무엇입니까?

* 대상 대상을 설명하려면 명확하고 수사적인 언어를 사용하십시오.

   * 당신은 완전한 문장이나 일련의 특징들을 입력할 수 있다. 명확성을 위해 필요한 경우를 제외하고는 구두점이 필요하지 않습니다.

   * 일반적으로 프롬프트는 대/소문자를 구분하지 않습니다.

   * Audience Agent는 가장 일반적인 동의어를 인식합니다.

* 포함하려는 모든 대상 특성과 제외하려는 특성에 대한 세부 정보를 지정하고 제공해야 합니다. 세부 정보를 많이 제공할수록 요구 사항에 맞는 결과를 얻을 수 있는 가능성이 커집니다.

* 포함하거나 제외할 위치, 장치 유형 및 데이터 공급자를 식별합니다.

* 대상을 저장하기 전에 기준 및 생성된 대상 표현식을 세분화하기 위한 세부 정보를 반복적으로 제공합니다.

* 실험을 통해 프롬프트에 대해 알아봅니다.

  프롬프트가 명확하지 않으면 Audience Agent에서 다른 프롬프트를 요청하므로 다시 시도할 수 있습니다.

  대상자 에이전트는 생성된 대상자 표현식을 대상자로 자동으로 저장하지 않습니다. 프롬프트 영역 외부에 있는 [!UICONTROL Create] 단추만 클릭하여 대상자를 저장할 수 있으므로 보관하지 않을 변경 내용을 실행 취소할 수 있습니다.

대상자에 대한 프롬프트를 최적화하는 자세한 방법은 &quot;[대상자 브리프 만들기에 대한 모범 사례](#audience-brief-best-practices)&quot;를 참조하십시오.

<!--
Consider starting by asking for what you should include.

you can give thumbs up or down to [what exactly?].

Verify what info is carried over from session to session and what starts from scratch.

-->

#### 프롬프트에 무엇을 포함할 수 없습니까?

* 기존 대상 표현식에 대한 참조.

* 영어 이외의 언어로 된 텍스트.

#### Audience Agent 응답 예 및 회신 방법

대상 에이전트가 사용자의 응답이 필요한 경우 요청에 키워드를 사용하거나 일반적인 동의어를 사용하여 답장할 수 있습니다.

#### 질문을 하는 대상 에이전트

`If you are okay with the proposed expression, I can start searching segments for each of the traits (based on the search filters above), and assemble the matching segments into the audience. Would you like me to proceed?`

긍정 응답: &quot;progress&quot;, &quot;okay&quot;, &quot;ok&quot;, &quot;yes&quot; 또는 다른 유사한 단어

요청을 무시하고 대신 추가 대상 기준을 계속 지정할 수도 있습니다.

##### 여러 옵션 중에서 선택하라는 대상 에이전트

`Would you like to:`
`1) Proceed with this expression,`
`2) Get maximum reach alternatives, or`
`3) Modify the expression manually?`

답글: `1`, `proceed`, `2`, `maximum reach` 등.

요청을 무시하고 대신 추가 대상 기준을 계속 지정할 수도 있습니다.

### 대상자 개요 작성을 위한 우수 사례 {#audience-brief-best-practices}

대상자 요약은 캠페인의 대상 대상자를 정의하는 전략 작성입니다. 잘 만들어진 요약은 DSP 대상 에이전트가 타겟팅 가능한 대상을 취합하기 위해 가장 관련성이 높은 세그먼트를 식별하는 데 도움이 됩니다.

#### 효과적인 대상 브리핑의 필수 구성 요소

브리핑의 다음 목록에서 가능한 한 많은 대상 속성 유형을 포함하십시오. 제외할 속성에 대해 구체적으로 지정합니다.

<!--
 What about these:

* Device specifications
* Presence in audiences from specific third-party data providers
* Presence of a universal ID
* Target cost per thousand (CPM) impressions or a total target cost

-->

* **인구 통계**

  연령 범위, 성별, 결혼 상태, 가구 구성(가족 규모, 자녀 유무, 다세대 가구)과 같은 속성을 포함합니다.

* **사회경제적 지표**

  가구 소득(HHI) 밴드, 교육 수준, 직업/직책, 취업 여부, 주택 소유 여부 등을 통해 재정 여력을 설정한다.

* **지리적 매개 변수**

  국가/국가, 지역(EMEA, APAC, NA), 인구 밀도(도시/교외/농촌)를 포함한 위치 범위를 정의합니다.

* **관심 분야 및 관심도**

  취미(스포츠, 예술, 야외 활동), 미디어 소비 패턴, 브랜드 관심도 및 라이프스타일 활동(여행, 식사, 엔터테인먼트)과 같은 열정과 선호도를 식별합니다.

* **심령술**

  포부(상태 추구, 자기 개선), 핵심 가치(지속 가능성, 혁신, 전통), 성격 특성(위험 추구자, 얼리 어답터) 및 구매 동기를 포함한 사고방식과 가치를 캡처합니다.

* **동작 신호**

  구매 행동(쇼핑 빈도, 채널 환경 설정, 브랜드 충성도), 온라인 행동(웹 사이트 방문, 컨텐츠 참여, 소셜 미디어 활동) 및 오프라인 행동(스토어 방문, 이벤트 참석, 멤버십)을 포함한 관찰할 수 있는 작업입니다.

* **마켓 내 의도**

  조사 중인 제품/서비스 범주, 구매 타임라인(즉시, 단기, 장기) 및 구매 결정을 트리거하는 관련 Life Event를 통해 구매 준비 상태를 식별합니다.

* **수명 단계**

  현재 단계 이해(학생, 진학 단계, 중등 단계, 임원, 퇴직 단계), 가족 단계(신혼부부, 새부모, 빈부모), 주요 생애 전환.

#### 전망 캠페인을 위한 잘 구성된 대상자 브리프의 예

다음은 프리미엄 밀 키트 구독 서비스에 대한 인지도 및 평가판을 높이기 위한 캠페인에 대한 강력한 대상 브리핑의 예입니다.

`The target audience consists of adults aged 28-45 (60% female, 40% male) with household incomes of $85K or more, college-educated professionals living in the USA. Psychographically, they are health-conscious individuals who value convenience and quality, aspire to be home cooks, and are food enthusiasts seeking better work-life balance. They actively engage with cooking and culinary content, follow health and wellness trends, shop at farmers markets, and prefer organic foods. Behaviorally, they are online grocery shoppers who use subscription services, dine out at restaurants 2+ times per week, and engage with food content on social media. They are currently in-market for meal planning solutions and food subscription services, with many focused on weight management and healthy eating programmes. The audience includes young families with children and dual-income households, as well as career-focused professionals. The brief excludes current subscribers and those following vegan/vegetarian diets as the initial launch focuses on protein-centric meal plans.`

>[!MORELIKETHIS]
>
>* [대상자 관리 정보](audience-about.md)
>* [대상 설정](audience-settings.md)
>* [대상 세그먼트 논리에 대한 구문](audience-segment-logic-syntax.md)
>* [사용 가능한 타사 데이터 공급자](third-party-data-providers.md)
>* [사용자 지정 세그먼트 만들기 및 구현](custom-segment-create.md)
>* [[!UICONTROL CCPA Opt-Out-of-Sale] 세그먼트 만들기 및 구현](ccpa-opt-out-segment-create.md)
>* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)
