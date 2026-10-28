---
title: AI Assistant를 사용하여 성능 및 게재 문제 해결
description: Adobe Advertising DSP AI Assistant의 문제 해결 에이전트를 사용하여 DSP 패키지 및 배치에 대한 지출, 게재 및 전달 문제를 진단합니다.
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
source-git-commit: 41d3ab985831a1432e775277384661643a9f55c4
workflow-type: tm+mt
source-wordcount: '804'
ht-degree: 0%
---
# AI Assistant를 사용하여 성능 및 게재 문제 해결


*Beta 기능*

AI Assistant의 문제 해결 에이전트는 라이브 패키지 및 배치의 성능을 제한하는 요소를 식별하고 문제를 해결하기 위해 내역 데이터를 기반으로 단계별 지침 및 권장 사항을 제공합니다. 문제 해결 에이전트는 다음 유형의 성능 및 전달 문제를 진단하는 데 도움이 될 수 있습니다.

* (배치만 해당) 초과 지출, 부족 지출 및 지출 실패를 포함한 지출 문제 상담원은 진단의 일부로 관련 게재 간격, 입찰, 타기팅 및 예산 상한 요소를 평가합니다.

* (패키지만 해당) CPA 상승 또는 ROAS 하락을 포함한 성능 문제 에이전트는 CTR, CPC, 클릭 수 또는 노출 수와 같은 참여 지표를 진단하지 않습니다.

각 대화는 단일 패키지 또는 배치에 대한 단일 진단을 다룹니다. 에이전트가 결과를 전달하면 다른 문제 또는 다른 패키지 또는 배치에 대해 묻는 새 대화를 시작합니다.

에이전트는 설정을 변경하거나, 캠페인 또는 캠페인 구성 요소를 만들거나 편집하거나, 일시 중지, 완료, 보관 또는 예약된 패키지 또는 배치에 대한 문제를 진단할 수 없습니다.

>[!IMPORTANT]
>
>AI가 생성한 응답은 정확하지 않거나 오해의 소지가 있을 수 있습니다. 비용이나 노력에 영향을 주는 결정에 사용하기 전에 항상 응답과 소스를 확인하십시오.

## 예제 쿼리

### 배치 지출 문제 해결

* 거래가 활발한데도 내 직업은 어제 지출을 중지했다. 왜요?

* 이 배치가 지난 5일 동안 왜 과소 지출되었습니까?

* 우리는 비행기의 절반이 지나가고 있고, 게을러지고 있다. 왜요?

### 패키지 성능 문제 해결

* 지난 주에 이 패키지에 대한 CPA가 증가한 이유는 무엇입니까?

* 이 패키지에 대한 ROAS가 감소하는 이유는 무엇입니까?

## AI Assistant에서 쿼리 제출

한 메시지에서 여러 질문을 할 수 있지만 한 번에 하나의 메시지만 표시됩니다. 다른 메시지를 보내기 전에 응답을 기다립니다.

1. 페이지의 오른쪽 상단에서 ![무대화](/help/dsp/assets/agent-chat.png "무대화")를 클릭합니다.

1. 쿼리를 빌드합니다.

   * 자신만의 쿼리를 입력하십시오.

   * 쿼리의 예를 보려면 **[!UICONTROL Troubleshoot]**&#x200B;을(를) 클릭하여 섹션을 확장합니다.

     1. (선택 사항) 예제 쿼리의 텍스트를 입력 필드에 복사하려면 다음을 수행합니다.

        1. 예제를 클릭합니다.

        1. (선택 사항) 필요에 따라 텍스트를 편집합니다.

   쿼리에 대한 자세한 내용은 &quot;[쿼리 및 프롬프트 작성에 대한 모범 사례](ai-assistant-about.md#writing-queries)&quot;를 참조하십시오.

   >[!NOTE]
   >
   >* 날짜 범위를 지정하지 않으면 상담원은 문제 유형에 따라 적절한 기본값을 선택합니다. 예를 들어 날짜 범위를 지정하지 않고 캠페인 지표에 대해 묻는 경우 캠페인 기간에 대한 결과가 표시됩니다.
   >* 목표 CPA를 염두에 두고 있는 경우 쿼리에 포함합니다(예: &quot;50달러 목표에 대한 CPA 진단&quot;). 지정하지 않으면 에이전트는 기본 대상을 사용합니다.

1. ![쿼리 제출](/help/dsp/assets/submit-prompt.png "쿼리 제출")을 클릭하거나 키보드에서 **Enter** 키를 누릅니다.

1. AI 도우미가 추가 정보를 요청하는 경우 제공합니다.

>[!TIP]
>
>다른 문제, 다른 패키지 또는 배치에 대해 질문하려면 [새 대화를 시작](#conversation-new)하세요.

## [!UICONTROL Packages] 또는 [!UICONTROL Placements] 보기에서 쿼리 제출

한 메시지에서 여러 질문을 할 수 있지만 한 번에 하나의 메시지만 표시됩니다. 다른 메시지를 보내기 전에 응답을 기다립니다.

1. 주 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 캠페인의 이름을 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * (패키지의 경우) [!UICONTROL Packages] 보기에서 패키지 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Troubleshooting Agent]**&#x200B;을(를) 클릭합니다.

   * (배치의 경우) 하위 메뉴에서 **[!UICONTROL Placements]**&#x200B;을(를) 클릭합니다. 배치 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Troubleshooting Agent]**&#x200B;을(를) 클릭합니다.

1. 쿼리를 빌드합니다.

   * 자신만의 쿼리를 입력하십시오.

   * 쿼리의 예를 보려면 **[!UICONTROL Troubleshoot]**&#x200B;을(를) 클릭하여 섹션을 확장합니다.

     1. (선택 사항) 예제 쿼리의 텍스트를 입력 필드에 복사하려면 다음을 수행합니다.

        1. 예제를 클릭합니다.

        1. (선택 사항) 필요에 따라 텍스트를 편집합니다.

   쿼리에 대한 자세한 내용은 &quot;[쿼리 및 프롬프트 작성에 대한 모범 사례](ai-assistant-about.md#writing-queries)&quot;를 참조하십시오.

   >[!NOTE]
   >
   >* 날짜 범위를 지정하지 않으면 상담원은 문제 유형에 따라 적절한 기본값을 선택합니다. 예를 들어 날짜 범위를 지정하지 않고 캠페인 지표에 대해 묻는 경우 캠페인 기간에 대한 결과가 표시됩니다.
   >* 목표 CPA를 염두에 두고 있는 경우 쿼리에 포함합니다(예: &quot;50달러 목표에 대한 CPA 진단&quot;). 지정하지 않으면 에이전트는 기본 대상을 사용합니다.

1. ![쿼리 제출](/help/dsp/assets/submit-prompt.png "쿼리 제출")을 클릭하거나 키보드에서 **Enter** 키를 누릅니다.

1. AI 도우미가 추가 정보를 요청하는 경우 제공합니다.

>[!TIP]
>
>다른 문제, 다른 패키지 또는 배치에 대해 질문하려면 [새 대화를 시작](#conversation-new)하세요.

## 새 대화 시작 {#conversation-new}

각 대화(또는 쿼리 스레드)는 별도로 저장되므로 이전 대화를 구분할 수 있습니다.

1. [대화상자](#ai-assistant-open)의 맨 위에서 ![새 대화 시작](/help/dsp/assets/new-selection.png "새 대화 시작")을 클릭하세요.

1. [쿼리 제출](#query-submit).

## 대화 상자 확장 및 최소화

1. [chatbox](#ai-assistant-open)의 맨 위에서 ![전체 화면 시작](/help/dsp/assets/fullscreen.png "전체 화면 시작")을 클릭하여 전체 화면 모드를 시작합니다.

1. 대화 상자를 패널 모드로 되돌리려면 **[!UICONTROL < Back>]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [Advertising DSP의 AI Assistant 정보](ai-assistant-about.md)
>* [이전 AI 지원 대화로 작업](previous-conversations.md)
