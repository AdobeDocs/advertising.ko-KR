---
title: Advertising Creative의 경험 정보
description: 개인화된 광고 경험을 구성하고 성능에 따라 광고 요소를 최적화하는 방법을 알아봅니다.
feature: Creative Experiences
exl-id: 91d4b4e5-c646-4485-8149-89f41dc9c3e6
source-git-commit: 8f81cf8ffaec7ca30ee3bbfd45d3577e75d77faf
workflow-type: tm+mt
source-wordcount: '804'
ht-degree: 0%

---

# Advertising Creative 2.0의 경험 정보

*베타가 닫힘*

<!-- Revisit Description metadata -->

<!-- MORE -->

[!DNL Advertising Creative 2.0]은(는) creative library에서 광고에 대해 두 가지 다른 광고 경험 구조를 제공합니다<!-- can use a single library only -->:

* **의사 결정 트리 타겟팅이 있는 경험:** [!DNL Creative]을(를) 사용하면 의사 결정 트리 모델을 사용하여 고객 여정 전반에 걸쳐 개인화된 광고 경험을 구성할 수 있습니다. 타겟 대상을 기반으로 모든 광고 요소(이미지, 헤드라인, 오퍼 및 랜딩 페이지)를 사용자 지정할 수 있습니다.

  예를 들어 특정 Adobe Analytics 대상 세그먼트에 있는 시카고와 뉴욕에 있는 사람들에 대해 동일한 크리에이티브 번들을 지정할 수 있지만, 동일한 세그먼트에 있는 시카고에 있는 사람들은 뉴요커가 아닌 다른 랜딩 페이지로 보낼 수 있습니다. 시카고 및 뉴욕시를 제외한 모든 지역에 거주하는 세그먼트에 있는 사람에 대해 다른 번들을 지정하고 세그먼트에 없는 다른 사람에 대해 세 번째 번들을 지정할 수도 있습니다.

  타깃팅 옵션에는 Adobe Audience Manager, Adobe Analytics 및 Advertising Cloud DSP의 자사 대상 세그먼트에 있는 뷰어, 국가, 주, 미국 내 DMA, 도시 및 우편번호를 비롯한 특정 지리적 위치에 있는 뷰어, DSP, 게시자 또는 파트너로부터 특정 키-값 쌍(데이터 전달 대상)이 전달되는 뷰어, [!DNL Creative]개의 재타깃팅 픽셀과 지정된 속성 값을 가진 뷰어, 특정 디바이스 유형, 운영 체제 및 브라우저가 있는 뷰어가 포함됩니다.

  각 경험에 크리에이티브 번들을 지정할 수 있습니다. 필요한 경우 크리에이티브 번들에 대한 최적화 및 예약을 사용자 지정하고 각 번들의 개별 크리에이티브에 대한 기본 랜딩 페이지 및 추적 URL<!-- and any flexible attributes -->을(를) 변경할 수 있습니다.

* **의사 결정 트리 타깃팅이 없는 경험:** [!DNL Creative]은(는) 대상을 좁히지 않고 광고 경험에 대한 광고 요소를 최적화합니다.<!-- For first-party creatives, [!DNL Creative] serves the ads. --> 각 경험에 대해 시작 및 종료 날짜와 일부 기본 설정을 지정하지만 대부분의 워크플로가 경험 내에 직접 있지 않습니다. 경험에 크리에이티브를 직접 추가하는 대신 [!UICONTROL Tag Manager] 내에서 경험에 대한 각 광고 크기에 대한 광고 태그를 만든 다음 광고 태그에 크리에이티브를 추가하고 크리에이티브 최적화 및 예약을 구성하고 랜딩 페이지 및 추적 URL을 사용자 지정합니다.

## 광고 최적화

<!-- MORE -->
[!DNL Creative]은(는) 성능에 따라 모든 경험에 대한 광고 요소를 최적화합니다. 특정 대상을 타깃팅하는 경험의 경우 타겟 대상 세트에 대한 개별 광고 요소의 성능에 따라 광고를 최적화할 수 있습니다. 특정 대상 타겟이 없는 경험의 경우 광고 요소는 순전히 개별 광고 요소의 성능에 따라 최적화됩니다.

## 경험 구현 및 관리

라이브 경험(필요한 모든 광고 요소 포함)을 만든 후에는 [전체 경험에 대한 JavaScript 또는 iframe 태그를 생성](experience-tag-export.md)할 수 있습니다. 이 태그는 선택적으로 Adobe Advertising DSP의 캠페인에 광고로 업로드하거나 서드파티 DSP의 광고로 구현할 수 있습니다. [!DNL Creative]은(는) 사용 가능한 광고 인벤토리와 타겟팅 및 광고 순환 옵션에 따라 경험 광고를 제공합니다.

## 경험에 대한 성능 데이터

[!UICONTROL Experiences] 보기에서 [!UICONTROL Metrics] 옵션을 활성화하면 각 경험 카드 또는 행은 경험이 받은 노출 횟수 및 클릭 수를 나타냅니다.

![지표 옵션](/help/creative/assets/metrics-option.png "지표 옵션")

<!-- insert screen shot of Metrics option?  If not, then add instructions elsewhere -->

<!-- I don't see this as of 1/9; why only in the table view?   You can also add conversion columns in the table view. -->

[!UICONTROL Creative] > [!UICONTROL Experiences] 보기에서 경험에 대한 자세한 성능 데이터를 볼 수 있습니다. 경험에서 성능을 모니터링하려면 [!UICONTROL Custom Creative Report]을(를) 만드십시오.

<!--
You can [view detailed performance data for any experience](experience-performance-details.md) from the Creative > Experiences view. To monitor performance across your experiences, [create custom reports](/help/dsp/reports/report-create.md).
-->

## 경험 상태 {#experience-statuses}

<!-- verify that these are all still the same -->

수동으로 설정한 *삭제됨*&#x200B;을(를) 제외하고 경험의 상태가 자동으로 설정됩니다.

*라이브:* 경험에 필요한 모든 요소가 포함되어 있으므로 DSP에서 광고로 구현할 경험 태그를 생성할 수 있습니다. <!-- A live experience may be scheduled to start in the future -->

*초안:* 경험의 모든 분기에 크리에이티브가 할당되지 않았으므로 경험이 완료되지 않았으며 경험 태그를 생성할 수 없습니다.

*처리 중:* 이전 라이브 경험이 편집되었지만 현재 완료되지 않았습니다. 경험 태그를 생성할 수 없습니다. **참고:** 경험에 대한 경험 태그를 이미 구현한 경우 이전 라이브 버전이 계속 제공됩니다. 나중에 경험을 완료하여 다시 라이브로 만들면 기존 태그 구현을 사용하여 새 버전이 제공됩니다.

*삭제됨:* 경험이 [!DNL Creative]에서 삭제되어 [!UICONTROL Experiences] 보기에 더 이상 표시되지 않습니다.

>[!NOTE]
>
>[!DNL Creative]의 경험 상태에 영향을 주지 않고 DSP 내에서 광고 상태를 변경할 수 있습니다.

## [!UICONTROL Experiences] 보기

[!UICONTROL Experiences] 보기는 타깃팅되고 타깃팅되지 않은 모든 경험을 표시합니다. 경험 이름, 상태, 시작 및 종료 날짜, 할당된 크리에이티브 또는 크리에이티브 번들의 수 및 차원, 경험에 동적 광고가 포함되는지 여부를 확인할 수 있습니다. [!UICONTROL Experiences] 보기에서 [!UICONTROL Metrics] 옵션을 활성화하면 각 경험 카드 또는 행은 경험이 받은 노출 횟수 및 클릭 수를 나타냅니다.

최적화, 경험에 크리에이티브 및 크리에이티브 번들 할당 등 경험을 만들고 관리할 수 있습니다. 광고 경험 태그를 만들고 이름을 바꾸고, JavaScript 및 iframe 포맷으로 태그를 내보내서 DSP에 구현할 수도 있습니다. Advertising DSP을 사용하는 광고주는 선택적으로 태그를 광고로 Advertising DSP 캠페인에 직접 업로드할 수 있습니다.

<!--
### Available actions

* [Download data within the view](experience-download-view.md)

        + [Assign and unassign creative bundles to a final node](/help/creative/experiences/experience-assign-creative-bundles.md)
* Experiences with decision tree targeting: [Create](/help/creative/experiences/experience-create-targeting.md) and [edit](/help/creative/experiences/experience-edit-targeting.md) experiences, [assign and unassign creative bundles](/help/creative/experiences/experience-assign-creative-bundles.md), [customize creative optimization and scheduling](/help/creative/experiences/experience-optimization-scheduling-targeting.md), and [customize the tracking URLs for creatives](/help/creative/experiences/experience-tracking-urls-targeting.md)

* Experiences without decision tree targeting: [Create](experience-create-no-targeting.md) and [edit](/help/creative/experiences/experience-edit-no-targeting.md)

* [Clone](experience-clone.md) an experience

* [Preview](experience-preview.md) an experience

* [Share a demo URL](experience-share-demo-url.md) for an experience

* [Export ad tags for an experience](experience-tag-export.md)

* [Delete](experience-delete.md) an experience

-->

<!-- You can add or remove labels for your experiences.-->

<!-- Add links to workflows once they're done -->

>[!MORELIKETHIS]
>
>* [의사 결정 트리 타깃팅으로 경험 만들기](experience-create-targeting.md)
>* [타깃팅하지 않고 경험 만들기](experience-create-no-targeting.md)
