---
title: AI Assistant를 사용하여 보고서 생성
description: Adobe Advertising DSP AI Assistant의 인사이트 에이전트를 사용하여 캠페인 지표를 쿼리하고, 보고서를 생성하고, CSV 파일을 다운로드하는 방법을 알아봅니다.
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
    internal-label: Demand Side Platform
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 0f6d32b5409cc95f09d0b0f28cdeee72a7861892
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%
---
# AI Assistant를 사용하여 보고서 생성

*Beta 기능*

*영어만 지원*

AI Assistant의 인사이트 에이전트를 사용하여 수동으로 보고서를 생성하지 않고도 캠페인, 캠페인 구성 요소, Advertising Creative 경험, 광고주 및 광고 타겟에 대한 지표와 전체 보고서를 얻을 수 있습니다. 캠페인에 대한 지출 또는 CPA와 같은 특정 지표에 대한 간단한 질문을 하거나 특정 차원(단일 캠페인 또는 대상자 등) 또는 차원 간(각 캠페인 및 광고주에 대한 분류의 경우)에 대한 보다 복잡한 보고서를 요청할 수 있습니다. 결과를 CSV 파일로 다운로드할 수 있습니다.

>[!IMPORTANT]
>
>AI가 생성한 응답은 정확하지 않거나 오해의 소지가 있을 수 있습니다. 비용이나 노력에 영향을 주는 결정에 사용하기 전에 항상 응답과 소스를 확인하십시오.

## 예제 쿼리

* [캠페인 이름]이(가) 지난 주에 소비한 금액은 얼마입니까?

* 이번 달에 [Campaign Name]에서 받은 전환은 몇 개입니까?

* [캠페인 이름]에 대한 패키지로 CPA를 표시합니다.

* 어떤 배치가 20% 이상 느립니까?

* 지난 15일 동안의 모든 캠페인 및 패키지에 대한 순 지출을 비교합니다.

## 쿼리 제출

한 메시지에서 여러 질문을 할 수 있지만 한 번에 하나의 메시지만 표시됩니다. 다른 메시지를 보내기 전에 응답을 기다립니다.

1. 페이지의 오른쪽 상단에서 ![무대화](/help/dsp/assets/agent-chat.png "무대화")를 클릭합니다.

1. 쿼리를 빌드합니다.

   1. 다음 중 하나를 수행합니다.

      * 자신만의 쿼리를 입력하십시오.

      * 쿼리의 예를 보려면 다음과 같이 하십시오.

        1. 섹션을 확장하려면 **[!UICONTROL Insights]**&#x200B;을(를) 클릭하십시오.

        1. (선택 사항) 예제 쿼리의 텍스트를 입력 필드에 복사하려면 다음을 수행합니다.

           1. 예제를 클릭합니다.

           1. (선택 사항) 필요에 따라 텍스트를 편집합니다.

   1. (선택 사항) 쿼리를 특정 차원 값(예: 특정 캠페인)에 집중하려면 선택적으로 차원 값을 표시할 위치에 커서를 삽입하고 ![엔티티 언급](/help/dsp/assets/prompt-entity.png "엔티티 언급")을 클릭한 다음 차원을 선택하고 차원 값을 선택합니다.

      예를 들어 [!UICONTROL Campaign] 차원의 경우 보고할 모든 캠페인 목록에서 선택할 수 있습니다.

      사용 가능한 차원은 다음과 같습니다.

      * 캠페인 엔터티: [!UICONTROL Campaign], [!UICONTROL Package], [!UICONTROL Placement], [!UICONTROL Ad]
      * 광고주: [!UICONTROL Advertiser]
      * Advertising Creative 엔터티: [!UICONTROL Experience]
      * 광고 대상: [!UICONTROL Audience], [!UICONTROL City], [!UICONTROL Country], [!UICONTROL State], [!UICONTROL DMA], [!UICONTROL Retargeting Pixel], [!UICONTROL Device OS], [!UICONTROL Device Browser], [!UICONTROL Device Type], [!UICONTROL Zip Code]

   쿼리에 대한 자세한 내용은 &quot;[쿼리 및 프롬프트 작성에 대한 모범 사례](ai-assistant-about.md#writing-queries)&quot;를 참조하십시오.

1. ![쿼리 제출](/help/dsp/assets/submit-prompt.png "쿼리 제출")을 클릭하거나 키보드에서 **Enter** 키를 누릅니다. 에이전트가 추가 정보를 요청하는 경우 필요한 정보를 제공합니다.

   전체 보고서를 미리 보고 보고서를 다운로드할 수 있는 링크와 함께 보고서의 처음 몇 행이 표시됩니다.

   생성된 보고서의 몇 개 행이 표시됩니다.

>[!TIP]
>
>다른 문제, 다른 패키지 또는 배치에 대해 질문하려면 [새 대화를 시작](#conversation-new)하세요.

## 챗박스에서 전체 보고서 다운로드 또는 미리보기

* 전체 보고서의 복사본을 다운로드하려면 ![내보내기](/help/dsp/assets/download.png "내보내기")를 클릭하세요.

  브라우저의 일반 절차에 따라 파일이 [!DNL Microsoft Excel] 쉼표로 구분된 값 파일(.csv)로 다운로드됩니다. 파일 이름은 &quot;DSP_Insights_Report_&lt;job_number>&quot;입니다.

* 측면 패널에서 전체 보고서를 미리 보려면 ![미리 보기](/help/dsp/assets/agent-chat-preview.png "미리 보기")를 클릭합니다. 미리 보기에서 보고서를 다운로드하려면 ![내보내기](/help/dsp/assets/download.png "내보내기")을(를) 클릭합니다.

  보고서를 다운로드하는 경우 브라우저의 일반 절차에 따라 쉼표로 구분된 값 파일(.csv)로 다운로드됩니다. [!DNL Microsoft Excel]파일 이름은 &quot;DSP_Insights_Report_&lt;job_number>&quot;입니다.

## 새 대화 시작 {#conversation-new}

각 대화 또는 쿼리 스레드는 별도로 저장되므로 이전 대화를 구분할 수 있습니다.

1. [대화상자](#ai-assistant-open)의 맨 위에서 ![새 대화 시작](/help/dsp/assets/new-selection.png "새 대화 시작")을 클릭하세요.

1. [쿼리 제출](#query-submit).

## 대화 상자 확장 및 최소화

1. [chatbox](#ai-assistant-open)의 맨 위에서 ![전체 화면 시작](/help/dsp/assets/fullscreen.png "전체 화면 시작")을 클릭하여 전체 화면 모드를 시작합니다.

1. 대화 상자를 패널 모드로 되돌리려면 **[!UICONTROL < Back>]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [Advertising DSP의 AI Assistant 정보](ai-assistant-about.md)
>* [이전 AI 지원 대화로 작업](previous-conversations.md)
