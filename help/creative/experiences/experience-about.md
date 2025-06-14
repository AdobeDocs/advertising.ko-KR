---
title: Advertising Creative의 경험
description: 개인화된 광고 경험을 구성하고 성능에 따라 광고 요소를 최적화하는 방법을 알아봅니다.
feature: Creative Experiences
exl-id: 91d4b4e5-c646-4485-8149-89f41dc9c3e6
source-git-commit: 2ddda1e23e3a3413ef93ca0705f0b9688c893f64
workflow-type: tm+mt
source-wordcount: '904'
ht-degree: 0%

---

# Advertising Creative 2.0의 경험 정보

*베타가 닫힘*

[!DNL Advertising Creative 2.0]은(는) Creative Library의 광고에 대해 두 가지 다른 광고 경험 구조를 제공합니다<!-- can use a single library only -->:

* **의사 결정 트리 타겟팅이 있는 경험:** [!DNL Creative]을(를) 사용하면 의사 결정 트리 모델을 사용하여 고객 여정 전반에 걸쳐 개인화된 광고 경험을 구성할 수 있습니다. 타겟 대상을 기반으로 모든 광고 요소(이미지, 헤드라인, 오퍼 및 랜딩 페이지)를 사용자 지정할 수 있습니다.

  예를 들어 특정 Adobe Analytics 대상 세그먼트에 있는 시카고와 뉴욕에 있는 사람들에게 동일한 광고 번들을 지정할 수 있지만, 시카고에 있는 사람들을 뉴욕 시민이 아닌 다른 랜딩 페이지로 보낼 수 있습니다. 시카고 및 뉴욕시를 제외한 모든 지역에 거주하는 세그먼트에 있는 사람에 대해 다른 번들을 지정하고 세그먼트에 없는 다른 사람에 대해 세 번째 번들을 지정할 수도 있습니다.

  타겟팅 옵션은 다음과 같습니다.

   * Adobe Audience Manager, Adobe Analytics 및 Advertising Cloud DSP의 자사 대상 세그먼트

   * 국가, 주, 미국 내 DMA, 도시 및 우편번호를 포함한 특정 지리적 위치

   * DSP, 게시자 또는 파트너로부터 특정 키-값 쌍(데이터 패스 대상)이 전달되는 뷰어

   * [!DNL Creative] 재타겟팅 픽셀 및 지정된 특성 값

   * 특정 디바이스 유형, 운영 체제 및 브라우저

  의사 결정 트리에 Target 대상 분기를 만들면 Creative 번들을 해당 분기에 할당하여 Target 대상을 잠재적 크리에이티브와 연결할 수 있습니다. 각 경험에 대해 크리에이티브 번들에 대한 최적화 및 예약을 사용자 정의하고 각 번들의 개별 크리에이티브에 대한 기본 랜딩 페이지 및 추적 URL<!-- later: and any flexible attributes -->을(를) 변경할 수 있습니다.

* **의사 결정 트리 타깃팅이 없는 경험:** [!DNL Creative]은(는) 대상을 좁히지 않고 광고 경험에 대한 광고 요소를 최적화합니다. 각 경험에 대해 시작 및 종료 날짜와 일부 기본 설정을 지정하지만 대부분의 워크플로는 경험 내에 직접 있지 않습니다. 경험에 크리에이티브를 직접 추가하는 대신 [!UICONTROL Tag Manager]을(를) 사용하여 경험의 각 광고 크기에 대한 광고 태그를 만든 다음, 여기에 크리에이티브를 추가하고, 크리에이티브 최적화 및 일정을 구성하고, 랜딩 페이지 및 추적 URL을 사용자 지정<!-- later: and any flexible attributes -->합니다.

## 광고 최적화

<!-- MORE -->
[!DNL Creative]은(는) 성능에 따라 모든 경험에 대한 광고 요소를 최적화합니다. 특정 대상을 타깃팅하는 경험의 경우 타겟 대상 세트에 대한 개별 광고 요소의 성능에 따라 광고를 최적화할 수 있습니다. 특정 대상 타겟이 없는 경험의 경우 광고 요소는 순전히 개별 광고 요소의 성능에 따라 최적화됩니다.

## 경험 구현 및 관리

필요한 모든 광고 요소가 포함된 라이브 경험을 만든 후에는 [전체 경험에 대한 JavaScript 또는 iframe 태그를 생성](experience-tag-export.md)할 수 있습니다. 경험 태그를 Adobe Advertising DSP의 캠페인에 광고로 업로드하거나 서드파티 DSP에서 광고로 구현할 수 있습니다. [!DNL Creative]은(는) 사용 가능한 광고 인벤토리와 타겟팅 및 광고 순환 옵션을 기반으로 자사 광고를 제공하고 경험에 대한 타사 광고를 트리거합니다.

## 경험에 대한 성능 데이터

다음 성능 데이터를 사용할 수 있습니다.

* [!UICONTROL Creative] > [!UICONTROL Experiences] 보기에서 [!UICONTROL Metrics] 옵션을 활성화하면 각 경험 카드 또는 행은 경험이 받은 노출 횟수 및 클릭 수를 나타냅니다.

  ![지표 옵션](/help/creative/assets/metrics-option.png "지표 옵션")

  <!-- insert screen shot of Metrics option?  If not, then add instructions elsewhere -->

  <!-- I don't see this as of 1/9; why only in the table view?   You can also add conversion columns in the table view. -->

* [!UICONTROL Experiences] 보기에서 [경험에 대한 자세한 성능 데이터를 볼 수 있습니다](experience-performance-details.md).

* 경험에서 성능을 모니터링하려면 [사용자 지정 Creative 보고서](/help/creative/report-custom-creative.md)를 만드십시오.

## 경험 상태 {#experience-statuses}

수동으로 설정한 *삭제됨,*&#x200B;을(를) 제외하고 경험의 상태가 자동으로 설정됩니다.

| 상태 | 설명 |
| ------ | ----------- |
| [!UICONTROL Live] | 경험에는 모든 필수 요소가 포함되므로 DSP에서 광고로 구현할 경험 태그를 생성할 수 있습니다. 라이브 경험이 나중에 시작되도록 예약할 수 있습니다. |
| [!UICONTROL Draft] | 경험의 모든 분기에 크리에이티브가 할당되지 않았으므로 경험이 완료되지 않고 경험 태그를 생성할 수 없습니다. |
| [!UICONTROL Processing] | 이전 라이브 경험이 편집되었지만 현재 완료되지 않았습니다. 경험 태그를 생성할 수 없습니다. **참고:** 경험에 대한 경험 태그를 이미 구현한 경우 이전 라이브 버전이 계속 제공될 수 있습니다. 나중에 경험을 완료하여 다시 라이브로 만들면 기존 태그 구현을 사용하여 새 버전을 제공할 수 있습니다. |
| [!UICONTROL Deleted] | 경험이 [!DNL Creative]에서 삭제되어 [!UICONTROL Experiences] 보기에 더 이상 표시되지 않습니다. |

>[!NOTE]
>
>[!DNL Creative]의 경험 상태에 영향을 주지 않고 DSP 내에서 광고 상태를 변경할 수 있습니다.

## [!UICONTROL Experiences] 보기

[!UICONTROL Experiences] 보기는 타깃팅되고 타깃팅되지 않은 모든 경험을 표시합니다. 경험 이름, 상태, 시작 및 종료 날짜, 할당된 크리에이티브 또는 크리에이티브 번들의 수 및 차원, 경험에 동적 광고가 포함되는지 여부를 확인할 수 있습니다. [!UICONTROL Experiences] 보기에서 [!UICONTROL Metrics] 옵션을 활성화하면 각 경험 카드 또는 행은 경험이 받은 노출 횟수 및 클릭 수를 나타냅니다.

경험을 만들고 관리하고, 광고 경험 태그를 만들고 이름을 바꾸고, DSP에서 구현할 수 있도록 JavaScript 및 iframe 형식으로 태그를 내보낼 수 있습니다. Advertising DSP을 사용하는 광고주는 선택적으로 광고 태그를 Advertising DSP 캠페인에 직접 업로드할 수 있습니다.

### 사용 가능한 작업

다음은 사용할 수 있는 주요 작업입니다. 전체 목록이 필요하면 크리에이티브 > 경험 챕터에 대한 목차를 참조하십시오.

* [보기 내에서 데이터 다운로드](experience-download-view.md)

* 타깃팅이 있는 경험을 [만들기](/help/creative/experiences/experience-create-targeting.md) 및 [편집](/help/creative/experiences/experience-edit-targeting.md)

* 타깃팅하지 않고 경험에 대해 [만들기](/help/creative/experiences/experience-create-no-targeting.md), [편집](/help/creative/experiences/experience-edit-no-targeting.md) 및 [수동으로 광고 태그 만들기](/help/creative/experiences/experience-tag-create-manually.md)

* 경험을 [복제](experience-clone.md)

* 경험 [미리 보기](experience-preview.md)

* 경험을 위해 [데모 URL 공유](experience-share-demo-url.md)

* [경험에 대한 광고 태그 내보내기](experience-tag-export.md)(선택적 Advertising DSP 캠페인에 직접 광고 태그 업로드 포함)

* 경험 [삭제](experience-delete.md)

>[!MORELIKETHIS]
>
>* [의사 결정 트리 타깃팅으로 경험 만들기](experience-create-targeting.md)
>* [타깃팅하지 않고 경험 만들기](experience-create-no-targeting.md)
