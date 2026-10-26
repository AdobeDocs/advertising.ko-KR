---
title: Advertising DSP의 AI Assistant 정보
description: 패키지 및 배치 문제 해결, 보고 및 제품 사용 도움말 검색에 DSP AI Assistant를 사용하는 방법을 알아봅니다.
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
source-git-commit: 8bab50fe8bf737d208d059d89b2592e16bc40c69
workflow-type: tm+mt
source-wordcount: '751'
ht-degree: 0%
---
# Advertising DSP의 AI Assistant 정보

DSP의 AI Assistant는 단일 채팅박스에서 DSP에서 사용할 수 있는 모든 아젠틱 워크플로를 수행할 수 있는 대화형 인터페이스입니다. 새 작업을 만들거나 이전 작업을 계속하는 데 도움을 요청할 수 있습니다.

대화 기록은 모든 워크플로우에 대해 유지되며 각 대화의 이름은 자동으로 지정됩니다. 쿼리가 다른 사용자와 공유되지 않습니다.

<!-- Update this:  ![Example of a query and response](/help/dsp/assets/agent-chat-response.png "Example of a query and response") -->

## 지원되는 워크플로

다음 워크플로를 통해 작업을 보다 효과적으로 수행할 수 있습니다.

<!-- And links to all sections/pages -->

| 기능 | 설명 | 예제 쿼리 | 응답 |
| --- | --- | --- | --- |
| [문제 해결](troubleshooting-agent.md) | 선택한 라이브 패키지 또는 배치에 대한 성능 및 게재 문제를 진단합니다.<ul><li>배치만: 과소비, 과소 지출 및 지출 실패 진단 에이전트는 관련 게재 간격, 입찰, 타기팅 및 예산 상한 요소를 평가합니다.</li><li>패키지만 해당: 상승하는 CPA 또는 하락하는 ROAS를 포함한 성능 문제를 진단합니다. 에이전트는 CTR, CPC, 클릭 수 또는 노출 수와 같은 참여 지표를 진단하지 않습니다.</li></ul>각 대화는 하나의 패키지 또는 배치에 대한 하나의 진단을 다룹니다. 결과를 받은 후 새 대화를 시작하여 다른 문제, 패키지 또는 배치를 진단합니다.<br><br>에이전트에서 설정을 변경하거나 캠페인 또는 캠페인 구성 요소를 만들거나 편집할 수 없습니다. 또한 일시 중지, 완료, 보관 또는 예약된 패키지 또는 배치를 진단할 수 없습니다. | 배치 지출 문제:<ul><li>거래가 활발한데도 내 직업은 어제 지출을 중지했다. 왜요?</li><li>이 배치가 지난 5일 동안 왜 과소 지출되었습니까?</li><li>우리는 비행기의 절반이 지나가고 있고, 게을러지고 있다. 왜요?</li></ul>패키지 성능 문제:<ul><li>지난 주에 이 패키지에 대한 CPA가 증가한 이유는 무엇입니까?</li><li>이 패키지에 대한 ROAS가 감소하는 이유는 무엇입니까?</li></ul> | 응답에는 성능을 제한하는 요소가 포함되며 문제 해결을 위한 권장 사항이 제공됩니다. |
| [인사이트](insights-agent.md) | 수동으로 보고서를 만들지 않고 캠페인 지표와 전체 보고서를 가져올 수 있습니다. 캠페인에 대한 지출 또는 CPA와 같은 특정 지표에 대한 간단한 질문을 하거나 특정 차원(단일 캠페인, 배치 또는 대상자 등) 또는 차원 간(캠페인 및 광고주별 분류)에 대한 보다 복잡한 보고서를 요청할 수 있습니다. 결과를 CSV 파일로 다운로드할 수 있습니다. | <ul><li>[캠페인 이름]이(가) 지난 주에 소비한 금액은 얼마입니까?<li>이번 달에 [Campaign Name]에서 받은 전환은 몇 개입니까?</li><li>어떤 배치가 20% 이상 느립니까?</li></li>[캠페인 이름]에 대한 패키지로 CPA 표시</li></ul> | 전체 보고서를 미리 보고 보고서를 [!DNL Microsoft Excel] 쉼표로 구분된 값 파일(.csv)로 다운로드할 수 있는 링크와 함께 보고서의 처음 몇 행이 표시됩니다. |
| [제품 설명서 검색](documentation-search.md) | [Advertising DSP 안내서](/help/dsp/home.md) 및 Advertising Creative을 사용하는 광고주의 경우 [Advertising Creative 안내서](/help/creative/home.md)에서 개념 및 방법 콘텐츠를 검색합니다. 답변은 [Experience League](https://experienceleague.adobe.com/en/docs/advertising)에서 이러한 제품에 대해 문서화된 내용만 기반으로 합니다.<br><br>캠페인 관리, 최적화, 대상 관리, 거래, 보고서 및 기타 제품 기능에 대해 질문하십시오. | <ul><li>게재에 광고를 첨부하려면 어떻게 해야 합니까?</li><li>Adobe DSP에서 사용할 수 있는 타깃팅 선택 사항은 무엇입니까?</li><li>배치 설정에서 다양한 간격 조정 옵션을 사용하면 어떤 결과가 발생합니까?</li><li>가구 수준 데이터를 포함하는 보고서는 무엇입니까?</li><li>[!DNL Creative] 경험에 대한 광고 태그를 만들려면 어떻게 합니까?</li></ul> | 응답에는 인라인 인용과 맨 아래에 확장 가능한 [!UICONTROL Documentation Sources] 목록이 포함됩니다. 인용 또는 소스 목록을 클릭하여 관련 페이지를 엽니다.<br><br>응답에는 쿼리를 구체화하고 추가 정보를 찾는 데 도움이 되는 후속 질문과 제안도 포함될 수 있습니다. |

## AI Assistant 열기 {#ai-assistant-open}

* 페이지의 오른쪽 상단에서 ![무대화](/help/dsp/assets/agent-chat.png "무대화")를 클릭합니다.

## 챗박스 펼치기

1. [chatbox](#ai-assistant-open)의 맨 위에서 ![전체 화면 시작](/help/dsp/assets/fullscreen.png "전체 화면 시작")을 클릭하여 전체 화면 모드를 시작합니다.

1. 대화 상자를 패널 모드로 되돌리려면 **[!UICONTROL < Back>]**&#x200B;을(를) 클릭합니다.

<!-- 

No ability to narrow down list of child entities for a selected parent as of 10/26/26.

## Submit a query {#query-submit}

1. [Open AI Assistant](#ai-assistant-open).

1. Build the query:

   * To see examples of queries by topic and optionally copy one to use:
   
     1. Click **[!UICONTROL Learn]**, **[!UICONTROL Troubleshoot]**, or **[!UICONTROL Insights]** to expand the section.
     
     1. (Optional) To copy the text of an example query into the input field:
     
        1. Click the example.
        
        1. (Optional) Edit the text to suit your needs. 

   * To enter your own query:
   
     1. (Insights and troubleshooting queries only; optional) To focus your query on a specific dimension value, such as a specific campaign, click ![Mention an entity](/help/dsp/assets/prompt-entity.png "Mention an entity"), select the dimension, and then select the dimension value.
     
        For example, for the dimension [!UICONTROL Campaign], you can select from a list of all your campaigns to report on.
        
        Available dimensions include:
        
        * Campaign entities: [!UICONTROL Campaign], [!UICONTROL Package], [!UICONTROL Placement], [!UICONTROL Ad]
        * The advertiser: [!UICONTROL Advertiser]
        * Advertising Creative entities: [!UICONTROL Experience]
        * Ad targets: [!UICONTROL Audience], [!UICONTROL City], [!UICONTROL Country], [!UICONTROL State], [!UICONTROL DMA], [!UICONTROL Retargeting Pixel], [!UICONTROL Device OS], [!UICONTROL Device Browser], [!UICONTROL Device Type], [!UICONTROL Zip Code]

     1. Enter your query, and then click ![Submit query](/help/dsp/assets/submit.png "Submit query") or press the **Enter** key on your keyboard.
        
   You can ask multiple questions in one message, but only one message at a time. Wait for a response before sending another.

   >[!NOTE]
   >
   >* (Troubleshooting and insight queries) If you don't specify a date range, then the agent selects a reasonable default based on the type of issue. For example, if you ask about campaign metrics without specifying a date range, then the results are for the duration of the campaign.
   >* (Troubleshooting queries) If you have a target CPA in mind, then include it in your query (for example, "diagnose CPA against a target of $50"). If you don't specify one, then the agent uses a default target.

1. If AI Assistant asks for additional information, provide it.

1. (Product documentation queries only; optional) To open a page used as a data source for the response, do either of the following:

   * Click the numbered citation.

   * Click **[!UICONTROL Documentation Sources]** to show a list of all pages cited in the response, and then click the page link.

>[!IMPORTANT]
>
>AI-generated responses may be inaccurate or misleading. Always verify responses and sources before using them for decisions that affect cost or effort.

>[!TIP]
>
>To ask another query that you want to be saved as a separate thread, [start a new conversation](#conversation-new).

## (Insight queries) Download or preview a full report from the chatbox

* To download a copy of the full report, click ![Export](/help/dsp/assets/download.png "Export").

   The file is downloaded as a [!DNL Microsoft Excel] comma-separated values file (.csv) according to your browser's normal procedure. The filename is "DSP_Insights_Report_<job_number>."

* To preview the full report in a side panel, click ![Preview](/help/dsp/assets/agent-chat-preview.png "Preview"). To download the report from the preview, click ![Export](/help/dsp/assets/download.png "Export").

   If you download the report, it's downloaded as a [!DNL Microsoft Excel] comma-separated values file (.csv) according to your browser's normal procedure. The filename is "DSP_Insights_Report_<job_number>."

## Start a new conversation {#conversation-new}

Each conversation, or query thread, is saved separately so you can distinguish between your previous conversations.

1. At the top of the [chatbox](#ai-assistant-open), click ![Start a new conversation](/help/dsp/assets/new-selection.png "Start a new conversation").

1. [Submit a query](#query-submit).

 -->

<!--

## Work with previous conversations

### List previous conversations

1. At the top of the [chatbox](#ai-assistant-open), click ![Threads history](/help/dsp/assets/threads.png "Threads history").

### Open a previous conversation

1. At the top of the [chatbox](#ai-assistant-open), click ![Threads history](/help/dsp/assets/threads.png "Threads history").

1. Click the conversation entry.

To repeat the same topic verbatim, copy the key details into a new conversation. Otherwise, you can ask AI Assistant to repeat a finite task within a specific conversation.

### Rename a previous conversation

1. At the top of the [chatbox](#ai-assistant-open), click ![Threads history](/help/dsp/assets/threads.png "Threads history").

1. Next to the conversation entry, click **[!UICONTROL ...] > [!UICONTROL Rename]**.

1. Edit the conversation name, and then click **[!UICONTROL Save]**.

-->

## 쿼리 및 프롬프트 작성에 대한 우수 사례 {#writing-queries}

* **명확하고 구체적인**. 전체 질문(&quot;온디맨드 재고를 어떻게 구독합니까?&quot;), 작업 구문(&quot;온디맨드 재고를 구독합니까&quot;) 또는 주제 구문(&quot;온디맨드 재고&quot;)을 사용합니다.

* **서로 다른 유형의 요청을 동일한 쿼리에 결합하지 마십시오**. 동일한 대화에 저장하지 않으려면 결합하십시오.

* **관련된 경우 날짜 범위를 포함**&#x200B;하여 원하는 데이터 범위를 좁힐 수 있습니다.

* **가능한 경우 제품 기능(&quot;캠페인&quot; 또는 &quot;거래&quot;)에 대해 UI 조건을 일치**&#x200B;합니다.

  일반적인 작업(예: &quot;추가&quot;, &quot;첨부&quot; 또는 &quot;할당&quot;)의 경우 동의어를 사용할 수 있습니다.

* 결과를 좁히거나 넓히려면 **세부 정보를 추가**&#x200B;하십시오. 필요에 따라 후속 질문으로 구체화하십시오.

* **구두점 및 대문자화에 대해 걱정하지 마십시오**. 단, 의미에 영향을 주는 경우는 예외입니다.

>[!MORELIKETHIS]
>
>* [AI 도우미를 사용하여 보고서 만들기](insights-agent.md)
>* [AI 도우미를 사용하여 성능 및 게재 문제 해결](troubleshooting-agent.md)
>* [재사용 가능한 대상 만들기](/help/dsp/audiences/reusable-audience-create.md)
>* [AI Assistant를 사용하여 제품 설명서 검색](documentation-search.md)
>* [이전 AI 지원 대화로 작업](previous-conversations.md)
