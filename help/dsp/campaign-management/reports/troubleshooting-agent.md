---
title: AI 지원 [!UICONTROL Troubleshooting Agent]을(를) 사용하여 성능 및 게재 문제 진단
description: AI 지원 문제 해결 에이전트를 사용하여 DSP 패키지 및 배치에 대한 지출, 게재 간격 및 배달 문제를 진단하는 방법을 알아봅니다.
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2:
  - id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 6032b798baa78c9c28196aa58024b8ed1061af9d
workflow-type: tm+mt
source-wordcount: 455
ht-degree: 0%

---

# AI 지원 [!UICONTROL Troubleshooting Agent]을(를) 사용하여 성능 및 게재 문제 진단

AI 지원 [!UICONTROL Troubleshooting Agent]은(는) 다음을 수행할 수 있습니다.

* 선택한 라이브 패키지 또는 배치에 대한 성능 및 게재 문제를 진단하는 데 도움이 됩니다. 지출 문제(지출 실패, 지출 감소, 지출 과다), 게재 관련 문제(과소 게재, 과잉 게재), 경매 및 게재 문제(낮은 입찰가, 낮은 승률, 노출 횟수 없음), 성과 문제(CPA, ROAS, CTR 또는 CVR의 변경 사항 등)에 대해 물을 수 있습니다.

* [Agentic Chat 인터페이스](/help/dsp/agent-chat.md)와(과) 동일한 방식으로 [Advertising DSP 안내서](/help/dsp/home.md) 및 (Advertising Creative을 사용하는 광고주) [Advertising Creative 안내서](/help/creative/home.md)에서 개념 및 방법 콘텐츠를 검색합니다. 캠페인 관리, 최적화, 대상자 관리, 거래, 보고서 및 기타 제품 기능에 대해 물을 수 있습니다.

에이전트는 설정을 변경하거나 캠페인 또는 캠페인 구성 요소를 만들거나 편집할 수 없습니다. 또한 일시 중지, 완료, 보관 또는 예약된 패키지 또는 배치에 대한 문제도 진단할 수 없습니다.

>[!IMPORTANT]
>
>AI가 생성한 응답은 정확하지 않거나 오해의 소지가 있을 수 있습니다. 비용이나 노력에 영향을 주는 결정에 사용하기 전에 항상 응답과 소스를 확인하십시오.

## 예제 쿼리

### 성능 및 게재 문제 해결

* 거래가 활발한데도 내 직업은 어제 지출을 중지했다. 왜요?

* 이 배치가 지난 5일 동안 왜 과소 지출되었습니까?

* 우리는 비행기의 절반이 지나가고 있고, 게을러지고 있다. 왜요?

### 제품 기능:

* 배치를 만들려면 어떻게 합니까?

* Adobe DSP에서 사용할 수 있는 타깃팅 선택 사항은 무엇입니까?

* 게재에 광고를 첨부하려면 어떻게 해야 합니까?

* 배치 설정에서 다양한 간격 조정 옵션을 사용하면 어떤 결과가 발생합니까?

* 각 유형의 최적화 목표를 언제 사용해야 합니까?

* 프로그램 보증(PG) 배치가 노출 횟수를 제공하는 이유는 무엇입니까?

* 가구 수준 데이터를 포함하는 보고서는 무엇입니까?

* [!DNL Creative]에서 타깃팅된 경험과 타깃팅되지 않은 경험의 차이점은 무엇입니까?

* [!DNL Creative] 경험에 대한 광고 태그를 만들려면 어떻게 합니까?

## 라이브 패키지 또는 배치에 대한 쿼리 제출

한 메시지에서 여러 질문을 할 수 있지만 한 번에 하나의 메시지만 표시됩니다. 다른 메시지를 보내기 전에 응답을 기다립니다.

1. 주 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 캠페인의 이름을 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * (패키지의 경우) [!UICONTROL Packages] 보기에서 패키지 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Troubleshooting Agent]**&#x200B;을(를) 클릭합니다.

   * (배치의 경우) 하위 메뉴에서 **[!UICONTROL Placements]**&#x200B;을(를) 클릭합니다. 배치 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Troubleshooting Agent]**&#x200B;을(를) 클릭합니다.

1. 쿼리를 입력하고 ![프롬프트 제출](/help/dsp/assets/submit-prompt.png "프롬프트 제출")을 클릭합니다.

   <!-- For more information, see "[Writing prompts](#writing-prompts)." -->

   응답에는 인라인 인용과 하단에 **[!UICONTROL Documentation Sources]** 목록이 포함됩니다. 후속 질문 및 제안 사항도 나타날 수 있습니다.

1. (선택 사항, 일반 제품 질문만 해당) 데이터 소스로 사용되는 페이지를 열려면 다음 중 하나를 수행하십시오.

   * 번호가 매겨진 인용구를 클릭합니다.

   * **[!UICONTROL Documentation Sources]**&#x200B;을(를) 클릭하여 응답에서 인용한 모든 페이지 목록을 표시한 다음 페이지 링크를 클릭합니다.