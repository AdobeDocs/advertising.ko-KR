---
title: AI 지원 채팅을 사용하여 제품 설명서 검색
description: AI 지원 채팅을 사용하여 Adobe Advertising DSP 및 [!DNL Creative] 설명서를 검색하는 방법에 대해 알아봅니다. 인용 및 제안 후속 프롬프트로 답변을 얻습니다.
feature: DSP Introduction, Creative Introduction
hidefromtoc: true
hide: true
exl-id: 30feb866-cc8c-4760-af94-2b2e08ebb361
source-git-commit: 54442a2bea5a2f34ca6eb59b7d3c8c36c4bb79bb
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# AI 지원 채팅 인터페이스를 사용하여 제품 설명서를 검색합니다

*Beta 기능*

*영어만 지원*

<!-- How will this work once we have unified shell, which has its own version of AI Assistant? -->

AI 채팅 인터페이스를 사용하여 [Advertising DSP 안내서](/help/dsp/home.md) 및 (Advertising Creative을 사용하는 광고주) [Advertising Creative 안내서](/help/creative/home.md)에서 개념 및 방법 콘텐츠를 검색할 수 있습니다. 답변은 [Experience League](https://experienceleague.adobe.com/en/docs/advertising)에서 이러한 제품에 대해 문서화된 내용만 기반으로 합니다.

응답에는 쿼리를 구체화하고 추가 정보를 찾는 데 도움이 되는 추가 프롬프트 및 후속 질문뿐만 아니라 인용 문항이 포함됩니다. 채팅 기록이 유지되고 쿼리가 다른 사용자와 공유되지 않습니다.

>[!NOTE]
>
>쿼리는 캠페인, 거래 또는 대상자 구성, 상태 또는 성능과 같은 계정에 대한 데이터를 반환하지 않습니다. 또한 문제를 해결하는 데 도움이 되지 않습니다.

![쿼리 및 응답의 예](/help/dsp/assets/agent-chat-response.png "쿼리 및 응답의 예")

>[!IMPORTANT]
>
>AI가 생성한 응답은 정확하지 않거나 오해의 소지가 있을 수 있습니다. 비용이나 노력에 영향을 주는 결정에 사용하기 전에 항상 응답과 소스를 확인하십시오.

## 예제 쿼리

캠페인 관리, 최적화, 대상자 관리, 거래, 보고서 및 기타 제품 기능에 대해 물을 수 있습니다. 다음은 예입니다.

* 게재에 광고를 첨부하려면 어떻게 해야 합니까?

* 배치 설정에서 다양한 간격 조정 옵션을 사용하면 어떤 결과가 발생합니까?

* 각 유형의 최적화 목표를 언제 사용해야 합니까?

* 프로그램 보증(PG) 배치가 노출 횟수를 제공하는 이유는 무엇입니까?

* 가구 수준 데이터를 포함하는 보고서는 무엇입니까?

* [!DNL Creative]에서 타깃팅된 경험과 타깃팅되지 않은 경험의 차이점은 무엇입니까?

* [!DNL Creative] 경험에 대한 광고 태그를 만들려면 어떻게 합니까?

## 쿼리 제출

한 메시지에서 여러 질문을 할 수 있지만 한 번에 하나의 메시지만 표시됩니다. 다른 메시지를 보내기 전에 응답을 기다립니다.

1. 페이지의 오른쪽 상단에서 ![무대화](/help/dsp/assets/agent-chat.png "무대화")를 클릭합니다.

1. 쿼리를 입력하고 ![프롬프트 제출](/help/dsp/assets/submit-prompt.png "프롬프트 제출")을 클릭합니다.

   자세한 내용은 &quot;[프롬프트 작성](#writing-prompts)&quot;을 참조하십시오.

   응답에는 인라인 인용과 하단에 **[!UICONTROL Documentation Sources]** 목록이 포함됩니다. 후속 질문 및 제안 사항도 나타날 수 있습니다.

1. (선택 사항) 데이터 소스로 사용되는 페이지를 열려면 다음 중 하나를 수행하십시오.

   * 번호가 매겨진 인용구를 클릭합니다.

   * **[!UICONTROL Documentation Sources]**&#x200B;을(를) 클릭하여 응답에서 인용한 모든 페이지 목록을 표시한 다음 페이지 링크를 클릭합니다.

## 응답에 대한 피드백 제공

<!-- Not actionable in terms of improving page content -->

* [!UICONTROL Documentation Sources] 목록 옆:

   * 유용한 응답을 보려면 ![엄지손가락 위로](/help/dsp/assets/thumbs-up.png "엄지손가락 위로")를 클릭하세요.

   * 도움이 되지 않는 응답은 ![Thumbs down](/help/dsp/assets/thumbs-down.png "Thumbs down")을 클릭합니다.

## 프롬프트 작성의 기본 사항 {#writing-prompts}

* **명확하고 구체적이어야 합니다.** 전체 질문(&quot;온디맨드 인벤토리를 어떻게 구독합니까?&quot;), 작업 구문(&quot;온디맨드 인벤토리에 구독&quot;) 또는 주제 구문(&quot;온디맨드 인벤토리&quot;)을 사용합니다.

* **가능한 경우 제품 기능(&quot;캠페인&quot; 또는 &quot;거래&quot;)에 대해 UI 조건을 일치**&#x200B;합니다.

  일반적인 작업(예: &quot;추가&quot;, &quot;첨부&quot; 또는 &quot;할당&quot;)의 경우 동의어를 사용할 수 있습니다.

* 결과를 좁히거나 넓히려면 **세부 정보를 추가**&#x200B;하십시오. 필요에 따라 후속 질문으로 구체화하십시오.

* **구두점 및 대문자화에 대해 걱정하지 마십시오**. 단, 의미에 영향을 주는 경우는 예외입니다.
