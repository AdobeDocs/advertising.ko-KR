---
title: 생성 AI를 사용하여 재사용 가능한 대상 만들기
description: AI 지원 대상 에이전트를 사용하여 Adobe Advertising DSP에서 재사용 가능한 대상을 만드는 방법을 알아봅니다. 타겟 대상을 자연어 프롬프트로 설명합니다. 에이전트는 타겟 또는 제외로 사용할 타사 세그먼트를 제안하고 대상 표현식을 빌드합니다.
feature: DSP Audiences
hidefromtoc: true
hide: true
source-git-commit: 86053178969de362dda0c135ff8c85b9ec9f674e
workflow-type: tm+mt
source-wordcount: '986'
ht-degree: 0%

---

# 생성 AI를 사용하여 재사용 가능한 대상 만들기

*Beta 기능*

*영어로만 확인*

<!-- I thought it was all segment types? -->

<!-- Redo the legacy file to include the new info. It's probably cleanest to keep it as two separate procedures (gen AI and manually) rather than one big, long procedure. -->

AI 지원 대상 에이전트를 사용하면 명시된 요구 사항에 따라 사용할 수 있는 모든 타사 세그먼트를 사용하여 재사용 가능한 새로운 대상을 생성할 수 있습니다. 여러 배치에 대한 타겟 또는 제외로 대상을 사용할 수 있습니다.

<!-- Later:  Audiences built using generative AI have the indicator [icon] in **[!UICONTROL Audiences] > [!UICONTROL All Audiences]**. -->

>[!NOTE]
>
>이 기능은 베타 모드이며 변경될 수 있습니다. 대상을 만들고 배치에 사용하기 전에 생성된 대상 표현식이 원하는 대상을 나타내는지 확인하십시오.

1. 메인 메뉴에서 **[!UICONTROL Audiences]** > **[!UICONTROL All Audiences]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위에서 **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

1. 고유한 **[!UICONTROL Audience Name]**&#x200B;을(를) 입력하십시오.

1. (선택 사항) **[!UICONTROL Share with all advertisers in my account]** 옵션을 선택 취소합니다.

   대상을 공유하면 해당 대상은 계정 내의 모든 광고주에게 타겟 또는 제외로 사용할 수 있습니다. 그러나 대상자의 개별 세그먼트는 세그먼트가 공유된 사용자만 사용할 수 있습니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

1. 대상자 작성:

   Beta 권한이 있는 사용자의 경우 AI 옵션이 기본값입니다. [대상자를 직접 결합](/help/dsp/audiences/reusable-audience-create.md)하려면 맨 아래에 있는 &quot;수동 모드로 전환&quot; 단추를 클릭하십시오.

   1. 포함 및 제외할 대상 특성을 설명하는 하나 이상의 프롬프트를 입력합니다. 각 프롬프트를 제출하려면 ![프롬프트 제출](/help/dsp/assets/submit-prompt.png "프롬프트 제출")을 클릭하십시오.

      자세한 내용은 &quot;[프롬프트 작성](#writing-prompts)&quot; 및 &quot;[대상자 개요 만들기 모범 사례](#audience-brief-best-practices)&quot;를 참조하십시오.

      AI 에이전트는 관련 세그먼트를 찾을 때 기준에 따라 대상 표현식을 생성합니다. 또한 대상을 취합할 일치하는 세그먼트를 찾기 전에 승인을 요청합니다.

      선택적으로 요청을 무시하고 대신 추가 대상 기준을 계속 지정할 수 있습니다.

   1. AI 에이전트가 대상자를 적절히 설명하는 대상자 표현식을 제공하면 AI 에이전트에게 대상자 조립을 진행하도록 알립니다.

      &quot;진행&quot;, &quot;확인&quot;, &quot;확인&quot;, &quot;예&quot; 또는 다른 유사한 단어를 입력할 수 있습니다.

1. (필요한 경우) 추가 기준을 지정합니다. AI 에이전트가 모든 기준에 맞는 대상자 표현식을 제공하면 대상자 조립을 진행하도록 AI 에이전트에게 알립니다.

1. 어셈블된 대상자에 동의하면 **[!UICONTROL Create]**&#x200B;을(를) 클릭하여 지정된 대상자를 만듭니다.

   >[!NOTE]
   >
   >나중에 AI 에이전트를 사용하여 대상자를 편집할 수 없습니다. 대신 [대상 식을 수동으로 편집](/help/dsp/audiences/reusable-audience-edit.md)하세요.

## 프롬프트 작성 {#writing-prompts}

### 프롬프트에 포함해야 하는 것은 무엇입니까?

* 대상 대상을 설명하려면 명확하고 수사적인 언어를 사용하십시오.

  일반적으로 프롬프트는 대/소문자를 구분하지 않으며 명확성을 제공하는 것 외에는 구두점이 필요하지 않습니다.

* 포함하려는 모든 대상 특성과 제외하려는 특성에 대한 세부 정보를 지정하고 제공해야 합니다. 세부 정보를 많이 제공할수록 요구 사항에 맞는 결과를 얻을 수 있는 가능성이 커집니다.

* 포함하거나 제외할 위치, 장치 유형 및 데이터 공급자를 식별합니다.

* 대상을 저장하기 전에 기준 및 생성된 대상 표현식을 세분화하기 위한 세부 정보를 반복적으로 제공합니다.

* 실험을 통해 프롬프트에 대해 알아봅니다.

  대상자 에이전트는 생성된 대상자 표현식을 대상자로 자동으로 저장하지 않습니다. 프롬프트 영역 외부에 있는 [!UICONTROL Create] 단추만 클릭하여 대상자를 저장할 수 있으므로 보관하지 않을 변경 내용을 실행 취소할 수 있습니다.

대상자에 대한 프롬프트를 최적화하는 자세한 방법은 &quot;[대상자 개요 만들기 모범 사례](#audience-brief-best-practices)&quot;를 참조하십시오.

<!-- I think these are happening later:

DSP uses "smart" defaults based on the user's previous audiences (all user-created audiences or only ones created via AI prompting?)

you can use a predefined prompt (fill in the blanks, and some fields might have selectors where you can choose values)

Over time, DSP XXXX defaults [clarify this]

 onsider starting by asking for a general template, which contains placeholder values that you can replace with your desired values. The default template is something like "Create a xxx with NNN xxx."

you can give thumbs up or down to [what exactly?]. Verify what info is carried over from session to session and what starts from scratch.

-->

### 프롬프트에 무엇을 포함할 수 없습니까?

* 기존 대상 표현식에 대한 참조.

* 영어 이외의 언어로 된 텍스트.

### AI 에이전트 응답 예 및 회신 방법

AI 에이전트가 사용자의 응답이 필요한 경우 요청에 키워드를 사용하거나 동등한 일반적인 용어를 사용하여 응답할 수 있습니다.

#### 질문을 묻는 AI 에이전트 응답

`If you are okay with the proposed expression, I can start searching third party segments for each of the traits (based on the search filters above), and assemble the matching segments into the audience. Would you like me to proceed?`

긍정 응답: &quot;progress&quot;, &quot;okay&quot;, &quot;ok&quot;, &quot;yes&quot; 또는 다른 유사한 단어

요청을 무시하고 대신 추가 대상 기준을 계속 지정할 수도 있습니다.

#### 여러 옵션 중에서 선택하라는 AI 에이전트 응답

```
Would you like to:
1) Proceed with this expression,
2) Get maximum reach alternatives, or
3) Modify the expression manually?
```

답글: `1`, `proceed`, `2`, `maximum reach` 등.

요청을 무시하고 대신 추가 대상 기준을 계속 지정할 수도 있습니다.

## 대상 개요 만들기에 대한 우수 사례 {#audience-brief-best-practices}

대상자 요약은 캠페인의 대상 대상자를 정의하는 전략 작성입니다. 잘 만들어진 요약은 DSP 대상 에이전트가 타겟팅 가능한 대상을 취합하기 위해 가장 관련성이 높은 세그먼트를 식별하는 데 도움이 됩니다.

### 효과적인 대상 브리핑의 필수 구성 요소

#### 대상 속성

개요의 다음 목록에서 가능한 한 많은 속성 유형을 포함합니다. 제외할 속성에 대해 구체적으로 지정합니다.

<!-- What about these:

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

### 전망 캠페인을 위한 잘 구성된 대상자 브리프의 예

다음은 프리미엄 밀 키트 구독 서비스에 대한 인지도 및 평가판을 높이기 위한 캠페인에 대한 강력한 대상 브리핑의 예입니다.

`The target audience consists of adults aged 28-45 (60% female, 40% male) with household incomes of $85K or more, college-educated professionals living in the USA. Psychographically, they are health-conscious individuals who value convenience and quality, aspire to be home cooks, and are food enthusiasts seeking better work-life balance. They actively engage with cooking and culinary content, follow health and wellness trends, shop at farmers markets, and prefer organic foods. Behaviorally, they are online grocery shoppers who use subscription services, dine out at restaurants 2+ times per week, and engage with food content on social media. They are currently in-market for meal planning solutions and food subscription services, with many focused on weight management and healthy eating programmes. The audience includes young families with children and dual-income households, as well as career-focused professionals. The brief excludes current subscribers and those following vegan/vegetarian diets as the initial launch focuses on protein-centric meal plans.`

>[!MORELIKETHIS]
>
>* [재사용 가능한 대상 복제](/help/dsp/audiences/reusable-audience-duplicate.md)
>* [재사용 가능한 대상 편집](/help/dsp/audiences/reusable-audience-edit.md)
>* [재사용 가능한 대상에 대한 세부 정보 보기](/help/dsp/audiences/reusable-audience-view-details.md)
>* [재사용 가능한 대상 공유](/help/dsp/audiences/reusable-audience-share.md)
>* [재사용 가능한 대상 내보내기](/help/dsp/audiences/reusable-audience-export.md)
>* [재사용 가능한 대상의 세그먼트 키를 클립보드에 복사](/help/dsp/audiences/reusable-audience-clipboard.md)
>* [재사용 가능한 대상 삭제](/help/dsp/audiences/reusable-audience-delete.md)
