---
title: DSP Planner 도구 정보
description: 지정된 예산 및 타깃팅 기준에 따라 연결된 TV(CTV) 배치에 대한 고유한 도달 범위를 예측하는 플래너 도구에 대해 알아봅니다.
feature: DSP Planner
exl-id: b25d4ac5-e85f-4a38-8765-6c5261987668
source-git-commit: 67fe8581832dc0762d62908d01672e53cc95b847
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 0%

---

# DSP Planner 도구 정보

<!-- rename all titles/descriptions from "CTV reach planner" to "campaign reach planner" -->

*Beta 기능*

플래너 도구를 사용하면 인벤토리 지출을 시작하기 전에 지정된 예산 및 타기팅 기준에 따라 연결된 TV(CTV) 배치에 대한 가구 수준의 고유한 도달 범위를 예측할 수 있습니다. 여러 도달 계획을 평가한 후 패키지 및 배치에서 원하는 결과에 가장 적합한 계획을 구현할 수 있습니다.

플래너 툴은 지난 90일 동안의 과거 입찰, 노출 및 도달 데이터를 사용하여 플랜 구성에 대한 고유 도달 거리, 평균 CPM, 평균 빈도 및 노출을 예측합니다.

## 계획자 예측

각 예측은 계획 설정으로 달성 가능한 도달 금액을 보여 주는 도달 예산 예측 곡선으로 구성됩니다. 시각화 위로 커서를 이동하면 더 높은 예산으로 증분 도달 기회를 볼 수 있습니다.

![계획자 예측](/help/dsp/assets/planner-forecast.png "계획자 예측")

또한 예측 결과에는 다양한 게시자가 고유한 도달 범위에 기여하여 중요한 검색 기회를 제공하는 방법을 보여 주는 [!UICONTROL Inventory Breakdown] 섹션도 포함됩니다.

>[!NOTE]
>
>* [!UICONTROL Inventory Breakdown] 섹션에는 개인 및 [!UICONTROL On Demand] 인벤토리에 대한 데이터만 표시됩니다.
>* 두 게시자에 대해 표시되는 예상 고유 도달 거리는 겹칠 수 있습니다.

## 플래너 보기

[!UICONTROL Planner] 보기에서 기존 CTV 도달 계획을 보고 새 계획을 만들 수 있습니다.

모든 계획에 대한 예측을 편집, 복제, 내보내기, 보관 또는 재생성할 수도 있습니다.

## FAQ

+++플래너 툴은 어떤 유형의 인벤토리를 지원합니까?

플래너 도구는 프로그램 보증(PG), 비공개 마켓플레이스(PMP), [!UICONTROL On Demand] 및 공개 등 모든 유형의 인벤토리를 지원합니다. 정확한 예측을 생성하려면 지난 7일 동안 최소 50,000번의 노출 횟수를 처리하는 것이 포함됩니다.

+++

+++[!UICONTROL Unable to generate forecast]이(가) 표시되는 이유는 무엇입니까?

이 오류의 가장 일반적인 이유 중 하나는 예산 또는 최대 입찰이 충분하지 않기 때문입니다. 최상의 결과를 얻으려면 최소 5000달러의 예산을 사용하십시오. [!UICONTROL Connected TV] 미디어 유형을 선택한 경우 최소 10USD의 최대 입찰가를 입력하십시오.

또한 포함된 게시자 또는 거래가 활성 상태이고 최근 노출 활동이 있는지 확인하십시오.

+++

+++예측을 기반으로 배치를 작성했지만 도달 예측에서 나타내는 고유한 도달 범위를 달성하지 못했습니다. 왜요?

도달 예측은 추정치일 뿐 계절성, 입찰 경쟁력, 수급 등 수시로 바뀌는 여러 요인이 얽혀 있어 실제 결과는 달라질 것으로 보인다. 완전히 정확할 것으로 예상되지는 않지만 최상의 결과를 얻을 수 있는 캠페인 전략에 대한 방향적 통찰력에 가장 유용합니다.

+++

+++계획자가 동일한 입력 설정으로 다른 예측 결과를 생성할 수 있습니까?

계획자는 최근에 관찰된 데이터를 기반으로 예측을 생성하므로 계획 설정이 동일하게 유지되더라도 예측된 출력이 다른 시간에 달라질 수 있습니다. 동일한 계획에 대해 여러 예측을 생성하고 각각에 대한 결과를 익스포트하는 것이 좋습니다.

+++

+++계획자 예측 결과를 저장할 수 있습니까?

예. 오른쪽 상단의 **[!UICONTROL ...]** > **[!UICONTROL Export]**&#x200B;을(를) 클릭하여 예측을 [!DNL Microsoft Excel] 스프레드시트로 내보낼 수 있습니다. 스프레드시트는 [!UICONTROL Budget] 및 [!UICONTROL Reach] 데이터 열을 사용하여 도달 예산 곡선에 표시된 정보를 캡처합니다.

>[!MORELIKETHIS]
>
>* [DSP Planner 도구 정보](planner-about.md)
>* [연결된 TV 도달 계획 만들기](planner-create.md)
>* [연결된 TV 도달 계획 복제](planner-duplicate.md)
>* [연결된 TV 도달 계획 편집](planner-edit.md)
>* [연결된 TV 도달 계획 내보내기](planner-export.md)
>* [연결된 TV 도달 계획에 대한 예측 다시 생성](planner-forecast.md)
>* [연결된 TV 도달 계획 보관](planner-archive.md)
>* [연결된 TV 도달 계획에 대한 설정](planner-settings.md)
