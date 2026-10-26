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
source-git-commit: ffe7424d4e225a95b279b06a7df3b85bf0cbcdbf
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 0%
---
# Advertising DSP의 AI Assistant 정보

DSP의 AI Assistant는 단일 채팅박스에서 DSP에서 사용할 수 있는 모든 아젠틱 워크플로를 수행할 수 있는 대화형 인터페이스입니다. 새 작업을 만들거나 이전 작업을 계속하는 데 도움을 요청할 수 있습니다.

대화 기록은 모든 워크플로우에 대해 유지되며 각 대화의 이름은 자동으로 지정됩니다. 쿼리가 다른 사용자와 공유되지 않습니다.

<!-- Update this:  ![Example of a query and response](/help/dsp/assets/agent-chat-response.png "Example of a query and response") -->

## 지원되는 워크플로

다음 워크플로를 통해 작업을 보다 효과적으로 수행할 수 있습니다.

<!-- And links to all sections/pages -->

| 기능 | 설명 | 응답 |
| --- | --- | --- |
| [문제 해결](troubleshooting-agent.md) | (Beta 기능) 선택한 라이브 패키지 또는 배치에 대한 성능 및 게재 문제를 진단합니다.<ul><li>배치만: 과소비, 과소 지출 및 지출 실패 진단 에이전트는 관련 게재 간격, 입찰, 타기팅 및 예산 상한 요소를 평가합니다.</li><li>패키지만 해당: 상승하는 CPA 또는 하락하는 ROAS를 포함한 성능 문제를 진단합니다. 에이전트는 CTR, CPC, 클릭 수 또는 노출 수와 같은 참여 지표를 진단하지 않습니다.</li></ul>각 대화는 하나의 패키지 또는 배치에 대한 하나의 진단을 다룹니다. 결과를 받은 후 새 대화를 시작하여 다른 문제, 패키지 또는 배치를 진단합니다.<br><br>에이전트에서 설정을 변경하거나 캠페인 또는 캠페인 구성 요소를 만들거나 편집할 수 없습니다. 또한 일시 중지, 완료, 보관 또는 예약된 패키지 또는 배치를 진단할 수 없습니다. | 응답에는 성능을 제한하는 요소가 포함되며 문제 해결을 위한 권장 사항이 제공됩니다. |
| [인사이트](insights-agent.md) | (Beta 기능) 보고서를 수동으로 만들지 않고 캠페인 지표와 전체 보고서를 가져올 수 있습니다. 캠페인에 대한 지출 또는 CPA와 같은 특정 지표에 대한 간단한 질문을 하거나 특정 차원(단일 캠페인, 배치 또는 대상자 등) 또는 차원 간(캠페인 및 광고주별 분류)에 대한 보다 복잡한 보고서를 요청할 수 있습니다. 결과를 CSV 파일로 다운로드할 수 있습니다. | 전체 보고서를 미리 보고 보고서를 [!DNL Microsoft Excel] 쉼표로 구분된 값 파일(.csv)로 다운로드할 수 있는 링크와 함께 보고서의 처음 몇 행이 표시됩니다. |
| [제품 설명서 검색](documentation-search.md) | [Advertising DSP 안내서](/help/dsp/home.md) 및 Advertising Creative을 사용하는 광고주의 경우 [Advertising Creative 안내서](/help/creative/home.md)에서 개념 및 방법 콘텐츠를 검색합니다. 답변은 [Experience League](https://experienceleague.adobe.com/en/docs/advertising)에서 이러한 제품에 대해 문서화된 내용만 기반으로 합니다.<br><br>캠페인 관리, 최적화, 대상 관리, 거래, 보고서 및 기타 제품 기능에 대해 질문하십시오. | 응답에는 인라인 인용과 맨 아래에 확장 가능한 [!UICONTROL Documentation Sources] 목록이 포함됩니다. 인용 또는 소스 목록을 클릭하여 관련 페이지를 엽니다.<br><br>응답에는 쿼리를 구체화하고 추가 정보를 찾는 데 도움이 되는 후속 질문과 제안도 포함될 수 있습니다. |

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
