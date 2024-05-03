---
title: 배치 설정
description: 사용 가능한 배치 설정에 대한 설명을 참조하십시오.
feature: DSP Placements
exl-id: 5b2574be-5d08-4cf7-910e-deac48d7e035
source-git-commit: 9586b743df5af61db81f781224bed28b02e0c4a8
workflow-type: tm+mt
source-wordcount: '3540'
ht-degree: 0%

---

# 배치 설정

## [!UICONTROL Basics]

**[!UICONTROL Placement name]** 배치 이름입니다.

>[!TIP]
>상황에 맞는 명명 규칙을 사용하십시오. 제안된 명명 규칙 중 하나는 &quot;*\&lt;campaign name=&quot;&quot;>: \&lt;ad unit=&quot;&quot;>: \&lt;duration>: \&lt;targeting>*.&quot;

**[!UICONTROL Status]:** 배치 상태: *[!UICONTROL Active]* (기본값) 또는 *[!UICONTROL Paused]*.

>[!TIP]
>가장 좋은 방법은 시작할 준비가 될 때까지 배치를 일시 중지하는 것입니다.

**[!UICONTROL Details]:** (읽기 전용) 해당 광고 유형, 배치를 만들거나 만든 계정, 상위 캠페인. 자세한 내용을 보려면 **[!UICONTROL Show more]**.

**[!UICONTROL Templates]:** 기존 배치 템플릿 목록을 엽니다. 템플릿에서 타깃팅 설정을 자동으로 채우려면 다음을 수행합니다.

1. 다음 중 하나를 수행합니다.

   * 템플릿의 모든 대상을 재사용하려면 템플릿 이름 옆에 있는 확인란을 선택합니다.

   * 템플릿에서 개별 대상 유형을 재사용하려면 템플릿 이름을 확장하고 재사용할 대상 유형 옆의 확인란을 선택합니다.

1. 클릭 **[!UICONTROL Apply]**.

**[!UICONTROL Ad specs for forecast]:** (비디오 광고 형식만 해당) 오른쪽의 예측 프로젝션을 계산하는 데 사용되는 광고 기간 및/또는 광고 사양입니다. 필드는 광고 유형에 따라 다릅니다.

**[!UICONTROL Environment]:** (범용 비디오 광고 형식만 해당) 배치에 대상으로 포함할 장치 환경(데스크탑, 모바일, 연결된 TV)입니다. 최소 하나 이상을 지정하십시오.

사용자 지정 보고서에서 배치 수준 차원 &quot;장치 환경&quot;은 타깃팅된 환경을 나타냅니다.

**[!UICONTROL Placement tags]:** (선택 사항) 이 배치를 찾는 데 도움이 되는 키워드 또는 닉네임.

## 목표

**[!UICONTROL Package]:** (선택 사항) 배치가 지정된 패키지입니다. 클릭 ![편집](/help/dsp/assets/edit.png) 기존 패키지를 선택하거나 패키지를 만듭니다. 패키지에 배치를 할당하면 [!UICONTROL Goals] 섹션에 패키지의 비행 날짜, 게재 목표 및 예산을 업데이트했습니다.

**[!UICONTROL Flight Dates]:** 배치의 시작 날짜와 종료 날짜입니다. 승인된 광고는 배치가 활성 상태이고 활성 패키지 또는 캠페인에 할당된 경우 비행 중에 실행할 수 있습니다.

패키지(해당되는 경우) 또는 캠페인에 대한 날짜는 기본적으로 자동으로 채워집니다.

>[!NOTE]
>
>* 비행 날짜는 캠페인 비행 날짜와 패키지 비행 날짜 내에 포함되어야 합니다.

### 패키지 수준 게재 간격이 있는 패키지에 할당된 배치

**[!UICONTROL Placement Funding]:** 배치 예산 책정 방법:

* *[!UICONTROL Optimize based on performance]:* 패키지 수준에서 예산을 제어합니다.
* *[!UICONTROL Set a Fixed Minimum or Maximum Budget]:* 최소 및/또는 최대 배치 예산을 설정할 수 있습니다. 최소 하나 이상의 예산 유형을 지정합니다.

   * *[!UICONTROL Maximum Budget]*: 값과 기간(*[!UICONTROL All time]*, *[!UICONTROL Daily]*, *[!UICONTROL Weekly]*, *[!UICONTROL Monthly]*).

   * *[!UICONTROL Minimum Budget]*: 패키지 예산의 최소 예산 비율. 간격 상한을 지정하면 최소 예산 값은 항상 간격 상한의 백분율로 계산됩니다. 그렇지 않으면 패키지 예산의 백분율로 계산됩니다.

**[!UICONTROL Max Bid]:** 1000회 노출에 대해 지불할 최대 금액입니다.

**[!UICONTROL Placement Pre-bid Filters]:** 입찰이 진행되려면 최대 5개의 KPI 임계값(예: 최소 가시성 지표 또는 클릭스루 비율)이 충족되어야 합니다. 최적화 전술로 사전 입찰 필터를 사용할 수 있지만 각 규칙은 이 배치가 입찰할 수 있는 기회를 제한할 수 있습니다. 필터를 추가하거나 편집하려면:

1. 클릭 ![편집](/help/dsp/assets/edit.png).
1. 다음 중 하나를 수행합니다.
   * 필터를 추가하려면 다음 작업을 수행하십시오.
      1. 클릭 **[!UICONTROL Add Filter]**.
      1. 다음 **[!UICONTROL Only bid if]**&#x200B;을 클릭하고 지표를 선택한 다음 값을 입력합니다.
   * 필터를 제거하려면 **[!UICONTROL X]** 필터 행에서 다음을 수행합니다.
1. 클릭 **[!UICONTROL Save]**.

에서 각 사전 입찰 필터에 대한 설명 보기 &quot;[배치 수준 사전 입찰 필터 및 사용 방법](/help/dsp/optimization/optimization-pre-bid-filters.md).&quot;

### 기타 모든 배치

**[!UICONTROL Budget Goal]:** 총 예산 상한 및 예산 간격(*[!UICONTROL All time]*, *[!UICONTROL Daily]*, *[!UICONTROL Weekly]*, *[!UICONTROL Monthly]*).

**[!UICONTROL Gross Budget Goal]:** (마진 관리 전용 캠페인에 배치) 총 예산 상한 및 예산 간격(*[!UICONTROL All time]*, *[!UICONTROL Daily]*, *[!UICONTROL Weekly]*, *[!UICONTROL Monthly]*).

**[!UICONTROL Optimization Goal]:**  패키지의 최적화 목표입니다. 에서 각 최적화 목표에 대한 설명을 참조하십시오.[최적화 목표 및 사용 방법](/help/dsp/optimization/optimization-goals.md)&quot;.

**[!UICONTROL Target Goal]:** 타겟 목표. 성과를 추적하는 데 사용됩니다.

>[!NOTE]
>
>이 필드는 벤치마크일 뿐이며 의사 결정에는 사용되지 않습니다.

**[!UICONTROL Pace on]:** 게재 간격 기본:

* **[!UICONTROL Budget goal]:** (기본값) 이 옵션은 할당된 예산 내에서 가능한 한 많은 노출 횟수를 제공합니다.

* **[!UICONTROL Impressions]:** 이 옵션은 지정된 수량이 지정된 간격 내에 도달할 때까지 노출을 전달합니다. 이 옵션을 선택할 때 노출 횟수와 간격을 지정합니다. *[!UICONTROL All time],* *[!UICONTROL Daily],* *[!UICONTROL Monthly],* 또는 *[!UICONTROL Weekly]*.

**[!UICONTROL Max Bid]:** 1000회 노출에 대해 지불할 최대 금액입니다.

**[!UICONTROL Flight pacing]:** (배치 수준 게재 간격 전용 배치) 광고 게재 간격 지정 방법:

* *[!UICONTROL Even]:* (기본값) 각 항공편 전체에 걸쳐 게재를 균등하게 처리하며, 타겟은 항공편 전반부에 게재되는 게재의 50%입니다.

* *[!UICONTROL Slightly Ahead]:* (기본값) 게재를 가속화하여 플라이트 기간 중간에 55~65% 완료됩니다.

* *[!UICONTROL Frontload]:* 배달 속도를 높여 비행 중간에 65~75% 완료됩니다.

* *[!UICONTROL Aggressive Frontload]:* 배달 속도를 높여 비행 중간에 75~85% 완료됩니다.

**[!UICONTROL Intraday pacing]:** (배치 수준 게재 속도만 있는 배치) 플라이트 내에서 매일 광고 게재의 속도를 지정하는 방법:

* *[!UICONTROL Even]:* (기본값) 재고 가용성에 따라 게재의 배율을 조정합니다. 일반적으로 경매량이 많은 낮에는 시간당 더 많은 광고가 게재되고 아침과 저녁에는 더 적은 수의 광고가 게재된다.

* *[!UICONTROL ASAP]:* (기본값) 게재 속도를 의 두 배로 가속화합니다. *균일*.

  >[!CAUTION]
  >
  >이 옵션은 성능에 부정적인 영향을 줄 수 있습니다. 성능 최적화에 비해 게재 우선 순위 및 비용을 완전히 우선시하는 경우에만 사용하십시오.

**[!UICONTROL Placement Pre-bid Filters]:** (선택 사항) 입찰이 진행되려면 최대 5개의 필터가 충족되어야 합니다. 최적화 전술로 사전 입찰 필터를 사용할 수 있지만 각 규칙은 이 배치가 입찰할 수 있는 기회를 제한할 수 있습니다. 필터를 추가하거나 편집하려면:

1. 클릭 ![편집](/help/dsp/assets/edit.png).
1. 다음 중 하나를 수행합니다.
   * 필터를 추가하려면 다음 작업을 수행하십시오.
      1. 클릭 **[!UICONTROL Add Filter]**.
      1. 다음 **[!UICONTROL Only bid if]**&#x200B;을 클릭하고 지표를 선택한 다음 값을 입력합니다.
   * 필터를 제거하려면 **[!UICONTROL X]** 필터 행에서 다음을 수행합니다.
1. 클릭 **[!UICONTROL Save]**.

## [!UICONTROL Geo-Targeting]

**[!UICONTROL Audience Location]:** (선택 사항) 배치에 광고를 포함하거나 제외할 특정 위치입니다. 위치를 지정하지 않으면 모든 위치가 타깃팅됩니다.

>[!NOTE]
>
>Roku 배치에 도시 및 DMA 위치를 사용할 수 없습니다.

위치를 지정하려면 다음을 수행합니다.

1. 클릭 ![편집](/help/dsp/assets/edit.png).
1. 다음 중 하나를 수행합니다.
   * 국가, 주, 도시, DMA, 연방 입법 지구 또는 주 입법 지구를 포함하거나 제외하려면 다음을 수행합니다.
      1. 왼쪽 열에서 위치 유형을 선택합니다.
      1. (필요한 경우) 확장할 위치를 클릭합니다.
      1. 위치 옆에 있는 *[!UICONTROL Include]* 타겟으로 포함하거나 *[!UICONTROL Exclude]* 타겟으로 제외합니다.
   * 우편 번호를 검색하고 선택한 모든 결과를 포함하거나 제외하려면
      1. 클릭 **[!UICONTROL Search Postal Code]**.
      1. 국가를 선택합니다.
      1. 도시 이름을 입력한 다음 을(를) 클릭합니다. ![편집](/help/dsp/assets/search.png).
      1. 올바른 검색 결과를 클릭합니다.
      1. 클릭 *[!UICONTROL Include All]* 모든 위치를 대상으로 포함 또는 *[!UICONTROL Exclude All]* 타겟으로 모든 위치를 제외합니다.
   * 우편 번호를 입력하거나 붙여 넣고 모두 포함하거나 제외하려면 다음을 수행합니다.
      1. 클릭 **[!UICONTROL Paste Postal Code]**.
      1. 국가를 선택합니다.
      1. 최대 1000개의 우편 번호를 입력하거나 붙여넣습니다.
한 줄에 하나의 우편 번호를 포함하거나, 쉼표 또는 탭으로 구분된 여러 값을 입력합니다.
      1. 클릭 *[!UICONTROL Include All]* 모든 위치를 대상으로 포함 또는 *[!UICONTROL Exclude All]* 타겟으로 모든 위치를 제외합니다.
   * 에서 위치를 제거하려면 [!UICONTROL Included] 또는 [!UICONTROL Excluded] 목록, 클릭 **[!UICONTROL X]** 오른쪽 열의 위치 옆에 있습니다.
1. 클릭 **[!UICONTROL Done]**.

>[!NOTE]
>
>* 모든 국가에 주, 도시 또는 우편 번호 위치가 있는 것은 아닙니다.
>* DMA(지정 시장 지역), 연방 입법 지구 및 주 입법 지구는 미국 지역에서만 사용할 수 있습니다.

## [!UICONTROL Inventory Targeting]

**[!UICONTROL Inventory Sources]:** 대상으로 포함하거나 제외할 인벤토리 소스입니다. 대부분의 배치 유형에는 기본적으로 모든 재고 유형과 각 유형의 모든 소스가 포함됩니다. 대상 [!DNL Roku] 배치, 재고 유형 및 소스를 지정해야 합니다. 다음 유형의 재고 중에서 선택할 수 있습니다.

* [!UICONTROL Public]: (Roku를 제외한 모든 배치 유형) DSP이 액세스할 수 있는 모든 오픈 Exchange 인벤토리를 포함합니다. 공개 인벤토리를 포함 및 제외할 수 있습니다.

  소스 또는 피드별로 목록을 볼 수 있습니다. 피드별로 목록을 볼 때 피드 이름, 피드 키 또는 선택한 특성 태그로 검색할 수 있습니다.

* [!UICONTROL Private] | [!UICONTROL Roku Private]: 기존 비공개 거래(또는 기존 비공개) [!DNL Roku] 다음에 대한 거래 [!DNL Roku] 배치)를 DSP에서 설정한 게시자가 있는 경우입니다. 공개 인벤토리를 포함할 수 있지만 제외할 수는 없습니다.

  키워드, 키, 거래 ID 또는 사용자 지정 태그로 목록을 검색할 수 있습니다.

   * *[!UICONTROL Ensure Fixed or Floor Price for the bid]*: (선택 사항) 거래의 고정 가격 및 최저 가격을 입찰하도록 입찰 가격 알고리즘을 무시합니다.

* [!UICONTROL On Demand] | [!UICONTROL Roku On Demand]: 모두 [premium, 보증 불가 [!UICONTROL On Demand] 인벤토리](/help/dsp/inventory/on-demand-inventory-about.md) (또는 [!UICONTROL On Demand] [!DNL Roku] 다음에 대한 거래 [!DNL Roku] 구독 중인 배치) [!DNL DSP]. 포함 및 제외할 수 있습니다 [!UICONTROL On Demand] 인벤토리.

  소스 또는 피드별로 목록을 볼 수 있습니다. 피드별로 목록을 볼 때 피드 이름, 피드 키 또는 선택한 게시자 영역, 범주 태그 또는 특성 태그별로 검색할 수 있습니다.

   * *[!UICONTROL Ensure Fixed or Floor Price for the bid]*: (선택 사항) 거래의 고정 가격 및 최저 가격을 입찰하도록 입찰 가격 알고리즘을 무시합니다.

재고 타깃팅을 지정하려면 다음을 수행합니다.

* 재고 유형을 제외하려면 이름 옆에 있는 확인란의 선택을 취소합니다.
* 재고 유형을 대상으로 지정하려면
   1. 재고 유형명 옆에 있는 체크박스를 선택합니다.
   1. (선택 사항) 포함할 소스를 변경합니다.
      1. 클릭 ![편집](/help/dsp/assets/edit.png).
      1. ([!UICONTROL Public] 및 [!UICONTROL On Demand] inventory) 클릭 **[!UICONTROL View by Source]** 또는 **[!UICONTROL View by Feed]** 소스를 나열하는 방법을 변경합니다.
      1. (해당되는 경우) 필요에 따라 재고를 필터링합니다.
      1. 포함 및 제외할 소스를 지정합니다.
         * 포함 [!UICONTROL Public] 또는 [!UICONTROL On Demand] 소스, 클릭 **[!UICONTROL Include]** 소스 이름 옆에 있습니다.
         * 포함할 항목 [!UICONTROL Private] 소스:
            * 거래에 모든 인벤토리를 포함하려면 **[!UICONTROL Include all]** 거래 이름 옆에 있습니다.
            * 개별 재고 출처를 포함하려면 거래명을 확장한 다음 출처명 옆에 있는 확인란을 누릅니다.
         * 제외하려면 [!UICONTROL Public] 또는 [!UICONTROL On source], 클릭 **[!UICONTROL Exclude]** 소스 이름 옆에 있습니다.
   1. (선택 사항) 타깃팅 정보가 있는 CSV 파일을 브라우저의 다운로드 위치에 다운로드하려면 다음을 클릭하십시오. **[!UICONTROL Save & Export]**.
   1. 클릭 **[!UICONTROL Save]**.

>[!TIP]
>
>을(를) 구독한 경우 [!UICONTROL On Demand] 인벤토리를 작성하지만 타겟팅할 게시자 또는 거래를 찾을 수 없습니다. 그런 다음 거래의 상태를 확인하십시오. 상태에 대한 자세한 내용은 [정보 [!DNL On Demand] Premium 재고](/help/dsp/inventory/on-demand-inventory-about.md).

**[!UICONTROL Exclude out-stream]:** (비디오 배치만 해당) 아웃스트림 트래픽을 제외합니다.

아웃스트림 광고는 대개 비디오 플레이어에서 일반 비디오 광고가 아니라 콘텐츠 위에 팝업 또는 콘텐츠로 채워집니다(기본 경험에서).

## [!UICONTROL Site Targeting]

**[!UICONTROL Traffic type]:** 타깃팅할 트래픽 유형. 옵션은 다음과 같습니다 **[!UICONTROL Websites]** 및 **[!UICONTROL Apps]**.

**[!UICONTROL Site tier]:** (사용 가능한 경우 **[!UICONTROL Paste list of targeted sites]** 은(는) *[!UICONTROL Off]*) 타겟팅할 사이트의 품질입니다. 계층 1-3은 모두 브랜드에 적합하며 DSP 매핑 팀의 검사 및 승인을 받았습니다.

* *[!UICONTROL Tier 1]:* 전국적으로 인식할 수 있는 프리미엄 사이트 및 애플리케이션.

* *[!UICONTROL Tier 2]:* 계층 1을 비롯하여 계층 1보다 덜 널리 알려진 품질 사이트 및 애플리케이션을 대상으로 합니다.

* *[!UICONTROL Tier 3]:* 타겟 계층 1-2와 틈새 고객을 위한 합법적이고 브랜드 안전한 사이트 및 애플리케이션입니다. 도달 또는 데이터 타겟팅 구매에 계층 3을 사용합니다.

* *[!UICONTROL All Sites]:* 계층 1-3 및 선별되거나 분류되지 않은 새로운 인벤토리를 타겟팅합니다. 이 인벤토리는 도달에 사용할 수 있습니다.

>[!NOTE]
>
>인벤토리는 배치의 광고 단위에만 적용됩니다.

>[!TIP]
>
>성과 캠페인의 경우 모범 사례는 다음을 선택하는 것입니다. *[!UICONTROL All Sites]*.

**[!UICONTROL Site Categories]:** (선택 사항이며, 다음과 같은 경우에 사용 가능 **[!UICONTROL Paste list of targeted sites]** 은(는) *[!UICONTROL Off]*) 타겟으로 포함하거나 제외할(두 가지 모두를 제외할 수는 없음) 선택한 사이트 계층 내의 사이트 카테고리입니다. 제목을 기반으로 DSP이 매핑한 세로 사이트 목록 중에서 선택합니다.

1. 클릭 ![편집](/help/dsp/assets/edit.png).
1. 포함 또는 제외할 사이트 범주를 지정합니다.
   * 사이트 범주를 포함하려면 다음 작업을 수행하십시오.
      1. 클릭 **[!UICONTROL Include categories]**.
      1. 타깃팅할 각 카테고리 옆에 있는 확인란을 선택합니다.
   * 사이트 범주를 제외하려면 다음 작업을 수행하십시오.
      1. 클릭 **[!UICONTROL Exclude categories]**.
      1. 제외할 각 범주 옆에 있는 확인란을 선택합니다.
1. (선택 사항) 타깃팅 정보가 있는 CSV 파일을 브라우저의 다운로드 위치에 다운로드하려면 다음을 클릭하십시오. **[!UICONTROL Export]**.
1. 클릭 **[!UICONTROL Save]**.

**[!UICONTROL Exclude Sites]:** (선택 사항이며, 다음과 같은 경우에 사용 가능 **[!UICONTROL Paste list of targeted sites]** 은(는) *[!UICONTROL Off]*) 제외할 사이트입니다. 사이트를 검색하여 선택하거나 도메인 이름을 입력하거나 붙여넣을 수 있습니다.

1. 클릭 ![편집](/help/dsp/assets/edit.png).
1. 사이트를 지정합니다.
   * 사이트를 검색하려면 다음 작업을 수행하십시오.
      1. 클릭 **[!UICONTROL Search]**.
      1. 키워드를 입력하거나, 사이트 계층을 선택하거나, 사이트 카테고리를 선택합니다.
      1. 검색 결과에서 제외할 사이트를 선택합니다.
         * 개별 사이트를 제외하려면 사이트 옆에 있는 확인란을 선택합니다.
         * (50개 이상의 결과를 사용할 수 있는 경우) 처음 50개의 결과를 제외하려면 **[!UICONTROL Exclude these 50]**. 모든 검색 결과를 제외하려면 **[!UICONTROL Exclude these \<*NN *\>]**.
   * 도메인 이름을 입력하려면 다음을 수행합니다.
      1. 클릭 **[!UICONTROL Paste]**.
      1. 별도의 줄에 도메인 이름을 하나 이상 입력합니다.
      1. 클릭 **[!UICONTROL Exclude All]**.
1. 클릭 **[!UICONTROL Done]** 다 끝나면

>[!NOTE]
>
>* DSP 외에 계정 수준 및 광고주 수준의 차단된 사이트 목록도 적용됩니다 [전역적으로 차단된 사이트 목록](/help/dsp/introduction/features/brand-safety-media-quality.md): 광고에는 안전하지 않은 것으로 간주되는 사이트가 포함됩니다.
>* 차단된 사이트 목록은 항상 타겟팅된 사이트 목록보다 우선 적용됩니다. 배치가 둘 다 광고에 대한 동일한 타겟을 제외하고 포함하면 타겟은 제외됩니다.

**[!UICONTROL Language]:** (선택 사항) 타깃팅할 단일 언어입니다.

**[!UICONTROL Site List Preview]:** (읽기 전용) 배치에 대해 타겟팅되고 차단된 모든 사이트.

선택적으로 타겟팅되고 차단된 사이트 목록을 쉼표로 구분된 값(CSV) 파일로 내보낼 수 있습니다. 목록을 내보내려면 **[!UICONTROL Export full site list]**&#x200B;를 클릭한 다음 브라우저의 일반 절차에 따라 파일을 열거나 저장합니다.

**[!UICONTROL Allow unscreened sites]:** (표준 디스플레이 배치만 해당) 감사되지 않은 사이트에서 광고 게재를 활성화합니다. 배치가 개인 인벤토리를 타겟팅하면 이 옵션은 차단된 사이트에 광고를 게재할 수 있습니다.

**[!UICONTROL Paste list of targeted sites]:** 특정 사이트만 타겟팅할 수 있습니다. 이 옵션을 활성화하면 다른 사이트 타겟팅 옵션이 비활성화됩니다.

**[!UICONTROL Sites]:** (사용 가능한 경우 **[!UICONTROL Paste list of targeted sites]** 은(는) *[!UICONTROL On]*) 타겟팅할 사이트 사이트를 검색하여 선택하거나 도메인 이름을 입력하거나 붙여넣을 수 있습니다.

1. 클릭 ![편집](/help/dsp/assets/edit.png).
1. 사이트를 지정합니다.
   * 사이트를 검색하려면 다음 작업을 수행하십시오.
      1. 클릭 **[!UICONTROL Search]**.
      1. 키워드를 입력하거나, 사이트 계층을 선택하거나, 사이트 카테고리를 선택합니다.
      1. 검색 결과에서 포함할 사이트를 선택합니다.
         * 개별 사이트를 제외하려면 사이트 옆에 있는 확인란을 선택합니다.
         * (50개 이상의 결과를 사용할 수 있는 경우) 처음 50개의 결과를 포함하려면 **[!UICONTROL Include these 50]**. 모든 검색 결과를 포함하려면 **[!UICONTROL Include these \<*NN *\>]**.
   * 도메인 이름을 입력하려면 다음을 수행합니다.
      1. 클릭 **[!UICONTROL Paste]**.
      1. 별도의 줄에 도메인 이름을 하나 이상 입력합니다.
      1. 클릭 **[!UICONTROL Include All]**.
1. 클릭 **[!UICONTROL Done]**.

## [!UICONTROL Audience Targeting]

**[!UICONTROL Included Audiences]:** 다음을 포함한 배치의 모든 대상 타겟 [타사 세그먼트, 자사 세그먼트, Adobe 세그먼트, 사용자 지정 세그먼트 및 저장된 대상자](/help/dsp/audiences/audience-settings.md). 선택한 모든 세그먼트 및 저장된 대상자 전체에 걸쳐 중복 제거된 총 활성 대상자 크기도 표시됩니다. 기존 대상을 선택하거나, 나중에 다시 사용할 수 있는 대상을 만들거나, 특정 대상 세그먼트를 선택할 수 있습니다.

* 기존 대상자를 선택하려면 ![선택](/help/dsp/assets/chevron-down.png) 다음에 [!UICONTROL Included Audiences]을 선택한 다음 대상자를 선택합니다.
* 대상자를 만들려면 ![선택](/help/dsp/assets/chevron-down.png) 다음에 [!UICONTROL Included Audiences]을 선택한 다음 을 선택합니다 **[!UICONTROL + Create Audience]**. 자세한 내용은 [재사용 가능한 대상 만들기](/help/dsp/audiences/reusable-audience-create.md)3단계부터 시작합니다.
* 특정 대상 세그먼트를 선택하려면 **[!UICONTROL Select segments for this placement only]**. 세그먼트 논리를 선택합니다. 자세한 내용은 의 6단계를 참조하십시오.[재사용 가능한 대상 만들기](/help/dsp/audiences/reusable-audience-create.md).&quot; 완료되면 다음을 클릭합니다. **저장**.

**[!UICONTROL Excluded Audiences]:** 를 사용하는 대상을 포함하여 배치에 대해 제외할 모든 대상 [타사 세그먼트, 자사 세그먼트, Adobe 세그먼트, 사용자 지정 세그먼트 및 저장된 대상자](/help/dsp/audiences/audience-settings.md). 제외된 모든 대상에 걸쳐 중복 제거된 총 활성 대상 크기도 표시됩니다. 기존 대상을 선택하거나 나중에 다시 사용할 수 있는 새 대상을 만들 수 있습니다.

* 기존 대상자를 선택하려면 ![선택](/help/dsp/assets/chevron-down.png) 다음에 [!UICONTROL Excluded Audiences]을 선택한 다음 대상자를 선택합니다.

* 대상자를 만들려면 ![선택](/help/dsp/assets/chevron-down.png) 다음에 [!UICONTROL Excluded Audiences]을 선택한 다음 을 선택합니다 **+ 대상 만들기**. 자세한 내용은 [재사용 가능한 대상 만들기](/help/dsp/audiences/reusable-audience-create.md)3단계부터 시작합니다.

* 특정 대상 세그먼트를 선택하려면 **[!UICONTROL Select segments for this placement only]**. 세그먼트 논리를 선택합니다. 자세한 내용은 의 6단계를 참조하십시오.[재사용 가능한 대상 만들기](/help/dsp/audiences/reusable-audience-create.md).&quot; 완료되면 다음을 클릭합니다. **저장**.

**[!UICONTROL Cross Device Targeting]:** (하나 이상의 세그먼트 또는 대상자를 선택하고 [campaign은 사용자 기반 교차 장치 타깃팅용으로 구성되었습니다.](/help/dsp/campaign-management/campaigns/campaign-settings.md). 지정한 세그먼트에 없는 장치도, 개인의 알려진 모든 장치(캠페인 설정에 지정된 장치 그래프에 따라)로 타깃팅을 확장할 수 있습니다. 캠페인에 대해 지정된 그래프에 따라 요금이 적용될 수 있습니다. 장치 그래프 데이터는 북미에서만 사용할 수 있습니다.

**[!UICONTROL Placement Cap]:** (선택 사항) 고유 장치 또는 개인 횟수(지정된 횟수에 따라 다름) [!UICONTROL Cross Device Level] 캠페인의 경우) 배치에서 광고가 제공됩니다. 옵션은 다음과 같습니다 *[!UICONTROL Unlimited]* 또는 일별, 주별, 월별 특정 금액입니다.

>[!NOTE]
>
> 캠페인, 패키지 및 배치 수준에서 빈도 상한을 설정할 수 있습니다. DSP은 campaign 계층 구조에서 가장 엄격한 빈도 상한을 따릅니다.

**[!UICONTROL Secondary Cap]:** (선택 사항, 숫자를 포함할 때 사용 가능) [!UICONTROL Placement Cap]) 주 배치 캡 내의 추가 제한. 노출 횟수와 기간을 선택합니다(예: 12시간당 3회).

**[!UICONTROL Day Parting]:** (선택 사항) 광고가 실행될 수 있는 특정 요일 및 시간입니다. 시간 분할 간격을 지정하려면 다음을 수행합니다.

1. 클릭 ![편집](/help/dsp/assets/edit.png).
1. 적용 가능한 시간대를 선택합니다.
1. 간격 지정:
   * 사전 설정된 간격을 선택하려면 간격 단추 중 하나를 클릭합니다. 옵션에는 *가 포함됩니다.[!UICONTROL Weekends]**, *[!UICONTROL Weekdays]*, *[!UICONTROL Morning]*, *[!UICONTROL Lunch]*, *[!UICONTROL Dinner]*, 또는 *[!UICONTROL Prime]* (primetime).
   * 간격을 수동으로 선택하려면 셀 내부를 클릭하고 선택적으로 드래그하여 간격을 선택합니다.
1. 클릭 **[!UICONTROL Save]**.

**[!UICONTROL Topic Targeting]:** (선택 사항, (으)로 구성된 광고주가 사용 가능 [!DNL Comscore] 및 [!DNL Grapeshot] 세그먼트) 특정 세그먼트 이름 또는 ID 출처 [!DNL Comscore] 및 [!DNL Grapeshot] 을(를) 대상으로 포함합니다. 이 기능에 대한 추가 비용이 발생할 수 있습니다. 이 기능을 활성화하고 주제 세그먼트를 설정하려면 Adobe 계정 팀에 문의하십시오.

주제 타깃팅을 지정하려면 다음을 수행합니다.

1. 클릭 ![편집](/help/dsp/assets/edit.png).
1. 타겟팅할 세그먼트 지정:
   1. 왼쪽 열에서 파트너를 선택합니다(*[!UICONTROL Comscore]* 또는 *[!UICONTROL Grapeshot]*).
   1. 입력 필드에 세그먼트 이름 또는 세그먼트 ID를 입력합니다.
1. (선택 사항) 주제 정보가 포함된 CSV 파일을 브라우저의 다운로드 위치에 다운로드하려면 다음을 클릭하십시오. **[!UICONTROL Export]**.
1. 클릭 **[!UICONTROL Save]**.

>[!TIP]
>
>* 주제 타깃팅은 배치가 입찰할 수 있는 인벤토리를 제한하므로 전체 구매에서 작은 비율에만 주제 타깃팅을 사용하십시오.
>
>* 에 대한 세그먼트 내에서 부정적인 타깃팅을 설정합니다. [!DNL Comscore] 또는 [!DNL Grapeshot].

**[!UICONTROL Device Targeting]:** (선택 사항) 대상으로 포함 및 제외할 특정 장치 정보(장치 유형, 제조업체, 운영 체제, 브라우저 및 연결 유형 등)입니다. 장치 타깃팅을 지정하려면:

1. 클릭 ![편집](/help/dsp/assets/edit.png).
1. 포함 및 제외할 장치 세부 정보를 지정합니다.
   1. 왼쪽 열에서 범주를 선택합니다.
   1. 타깃팅 지정:
      * 값을 포함하려면 **[!UICONTROL Include]** 값 이름 옆에 있습니다.
      * 값을 제외하려면 **[!UICONTROL Exclude]** 값 이름 옆에 있습니다.
1. (선택 사항) 장치 타깃팅 정보가 있는 CSV 파일을 브라우저의 다운로드 위치에 다운로드하려면 를 클릭합니다 **[!UICONTROL Export]**.
1. 클릭 **[!UICONTROL Save]**.

**[!UICONTROL ISP Targeting]:** (선택 사항) 특정 인터넷 서비스 공급자(ISP)가 대상으로 포함 또는 제외(둘 다 아님)해야 합니다. ISP 타깃팅을 지정하려면 다음을 수행하십시오.

1. 클릭 ![편집](/help/dsp/assets/edit.png).
1. 포함 또는 제외할 ISP를 지정합니다.
   * ISP를 포함하려면:
      1. 클릭 **[!UICONTROL Include ISPs]**.
      1. (선택 사항) 키워드로 목록을 필터링합니다.
      1. 타깃팅할 각 ISP 옆에 있는 확인란을 선택합니다.
   * ISP를 제외하려면 다음을 수행하십시오.
      1. 클릭 **[!UICONTROL Exclude ISPs]**.
      1. (선택 사항) 키워드로 목록을 필터링합니다.
      1. 제외할 각 ISP 옆에 있는 확인란을 선택합니다.
1. (선택 사항) ISP 타깃팅 정보가 있는 CSV 파일을 브라우저의 다운로드 위치에 다운로드하려면 를 클릭합니다 **[!UICONTROL Export]**.
1. 클릭 **[!UICONTROL Save]**.

## [!UICONTROL Brand Safety and Media Targeting]

**[!UICONTROL Contextual filtering]:** 유형 [!DNL Comscore], [!DNL DoubleVerify], [!DNL Integral Ad Science], 및 [!DNL Peer39] 적용할 컨텍스트 필터. 새 배치에 대해 광고주 수준 기본값이 선택되지만 설정을 변경할 수 있습니다.

* [!UICONTROL DoubleVerify]:

   * **[!UICONTROL Block sites that are]:** (선택 사항) 기본적으로 차단되는 하나 이상의 재고 컨텍스트 유형. 추가 요금이 부과될 수 있습니다.

* [!UICONTROL Peer 39]:

   * **타겟 사이트는 다음과 같습니다.** (선택 사항) 기본적으로 타깃팅할 하나 이상의 재고 속성 유형. 추가 요금이 부과될 수 있습니다.

* [!UICONTROL ComScore]:

   * **다음과 같은 사이트 차단:** (선택 사항) 기본적으로 차단해야 할 하나 이상의 재고 속성 유형. 추가 요금이 부과될 수 있습니다.

* [!UICONTROL Integral Ad Science]

   * **[!UICONTROL Adult Content]:** (선택 사항) 기본적으로 광고를 차단할 성인 콘텐츠의 정도: *[!UICONTROL Do Not Block]* (기본값), *[!UICONTROL Standard]*, 또는 *[!UICONTROL Strict]*. 추가 요금이 부과될 수 있습니다.

   * **[!UICONTROL Alcohol Content]:** (선택 사항) 기본적으로 광고를 차단할 알코올 도입니다. *[!UICONTROL Do Not Block]* (기본값), *[!UICONTROL Standard]*, 또는 *[!UICONTROL Strict]*. 추가 요금이 부과될 수 있습니다.

**[!UICONTROL Pre-bid fraud blocking]:** 다음을 통해 측정된 사기성 트래픽 및 의심스러운 활동을 기반으로 차단할 사이트 유형 [!DNL DoubleVerify], [!DNL Integral Ad Science], 및 [!DNL Peer39]. 새 배치에 대해 광고주 수준 기본값이 선택되지만 설정을 변경할 수 있습니다.

* [!UICONTROL DoubleVerify]:

   * **[!UICONTROL Block Fraud Sites (100% Invalid traffic) and User-Based Fraud and IVT Devices]:** 기본적으로 는 새 배치에 대해 납치된 장치의 트래픽을 포함하여 100% 잘못된 모든 트래픽을 차단합니다. 추가 요금이 부과될 수 있습니다.

   * **[!UICONTROL Also block sites with]:** (선택 사항) DSP에서 기본적으로 광고를 차단하게 하는 추가적인 수준의 사기 및 잘못된 트래픽:  *[!UICONTROL None]* (추가 트래픽을 차단하지 않는 기본값), *[!UICONTROL >2% Average Fraud/IVT levels (lowest reach)]*, *[!UICONTROL >4% Average Fraud/IVT levels]*, *[!UICONTROL >6% Average Fraud/IVT levels]*, *[!UICONTROL >10% Average Fraud/IVT levels]*, 또는 *[!UICONTROL >25% Average Fraud/IVT levels]*. 추가 요금이 부과될 수 있습니다.

* [!UICONTROL Peer 39]:

   * **[!UICONTROL Block sites that are]:** (선택 사항) DSP에서 기본적으로 광고를 차단하게 하는 하나 이상의 사기 유형: *[!UICONTROL Fraud]* (사기로 모든 사이트를 차단함), *[!UICONTROL Fraud: Bot Sites_Non-Human traffic]*, 및/또는 *[!UICONTROL Fraud: Zero Ads]*. 추가 요금이 부과될 수 있습니다.

* [!UICONTROL Integral Ad Science]:

   * **[!UICONTROL Block sites that are]:** (선택 사항) DSP이 기본적으로 광고를 차단하도록 하는 의심스러운 웹 사이트 또는 앱 활동 유형입니다. *[!UICONTROL None]* (의심스러운 활동에 따라 광고를 차단하지 않는 기본값), *[!UICONTROL Suspicious Activity - High Risk]*, 또는 *[!UICONTROL Suspicious Activity - High or Moderate Risk]*. 추가 요금이 부과될 수 있습니다.

**[!UICONTROL Ads.txt filtering]:**

레벨 [Ads.txt](https://iabtechlab.com/ads-txt-about/) 각 게시자의 승인된 디지털 판매자 목록을 적용하여 사용할 사전 입찰 필터링. 새 배치에 대해 광고주 수준 기본값이 선택되지만 설정을 변경할 수 있습니다.

* *[!UICONTROL Opt out of ads.txt (default)]*: 모든 판매자로부터 재고를 구입합니다.
* *[!UICONTROL Ads.txt sellers + sites without ads.txt]*: 도메인의 승인된 직접 판매자 및 리셀러의 인벤토리 구매에 우선 순위를 두십시오.
* *[!UICONTROL Ads.txt sellers only]*: 도메인의 승인된 직접 판매자 및 리셀러에서만 인벤토리를 구매합니다.
* *[!UICONTROL Ads.txt sellers only]*: 도메인의 승인된 직접 판매자로부터만 인벤토리를 구매합니다.

**[!UICONTROL DoubleVerify Authentic Brand Safety]:** (다음으로 구성된 광고주) [!UICONTROL DoubleVerify Authentic Brand Safety] option) 활성화 [!DNL DoubleVerify Authentic Brand Safety]: 지정된 세그먼트 ID에 대해 구성된 사용자 지정 브랜드 안전 규칙을 사용하여 입찰 후 노출을 차단합니다. DSP은 광고주 설정에 지정된 세그먼트 ID에 대한 사용을 위해 계정에 청구합니다.

## [!UICONTROL Tracking] {#placement-tracking}

>[!NOTE]
>
>([!DNL Roku] 배치) 이(가) 승인한 서드파티 추적 공급업체 [!DNL Roku] include [!DNL Acxiom], [!DNL comScore], [!DNL Data Plus Math], [!DNL Experian], [!DNL Factual], [!DNL Kantar], [!DNL Marketing Evolution], [!DNL Neustar], [!DNL Nielsen], [!DNL Nielsen Catalina Solutions], [!DNL NinthDecimal], [!DNL Oracle], [!DNL Placed], [!DNL Polk], 및 [!DNL Research Now].

**[!UICONTROL Event Pixels]:** (선택 사항) 배치의 모든 새 광고에 기본적으로 첨부할 서드파티 이벤트 추적 픽셀. 이벤트 픽셀을 지정하려면:

1. 클릭 ![편집](/help/dsp/assets/edit.png).
1. 다음 중 하나를 수행합니다.
   * 기존 픽셀을 선택하려면 픽셀 행에서 확인란을 선택합니다.
   * 픽셀을 만들려면 다음 작업을 수행하십시오.
      1. 클릭 **[!UICONTROL Create]**.
      1. 다음 정보를 입력합니다.
         * **[!UICONTROL Pixel name]:** 픽셀 이름입니다. 최대 길이는 500자입니다. 픽셀을 쉽게 식별하는 데 도움이 되는 이름을 사용합니다.
         * **[!UICONTROL Pixel event fires on]:** 픽셀을 실행하도록 트리거하는 이벤트입니다. 사용 가능한 이벤트는 광고 유형에 따라 다릅니다.
         * **[!UICONTROL Pixel type]:** 픽셀이 *[!UICONTROL IMG URL]* (1x1 픽셀 이미지 파일), *[!UICONTROL HTML]*, 또는 *[!UICONTROL JavaScript URL]*.
         * **[!UICONTROL Pixel URL]:** 픽셀 이미지의 URL.
      1. 클릭 **[!UICONTROL Create and attach]**.
   1. 클릭 **[!UICONTROL Save]**.

**[!UICONTROL Conversion Pixels]:** (선택 사항) 배치의 모든 새 광고에 기본적으로 첨부할 전환 추적 픽셀입니다. 변환 픽셀을 지정하려면 다음을 수행합니다.

1. 클릭 ![편집](/help/dsp/assets/edit.png).
1. 다음 중 하나를 수행합니다.
   * 기존 픽셀을 선택하려면 픽셀 행에서 확인란을 선택합니다.
   * 픽셀을 만들려면 다음 작업을 수행하십시오.
      1. 클릭 **[!UICONTROL Create]**.
      1. 다음 정보를 입력합니다.
         * **[!UICONTROL Conversion pixel name]:** 픽셀 이름입니다. 최대 길이는 500자입니다. 픽셀을 쉽게 식별하는 데 도움이 되는 이름을 사용합니다.
         * **[!UICONTROL Conversion category]:** 전환 유형입니다.
         * **[!UICONTROL Impression conversion window]:** 광고 노출 후 전환으로 인한 노출 횟수입니다. 기본값은 30일입니다.
         * **[!UICONTROL Click conversion window]:** 광고 클릭 발생 후 전환으로 인한 클릭의 기여도(일). 기본값은 30일입니다.
         * **[!UICONTROL Notes]:** (선택 사항) 픽셀에 대한 설명 또는 기타 정보입니다.
      1. 클릭 **[!UICONTROL Create and attach]**.
      1. 관련 웹 페이지에서 변환 픽셀을 구현합니다.
         1. 메인 메뉴에서 다음 위치로 이동합니다. **[!UICONTROL Resources]** > **[!UICONTROL Conversion pixels]**.
         1. 픽셀 행에서 **[!UICONTROL edit]**.
         1. 에서 값을 복사합니다. [!UICONTROL HTML Tag] 및 [!UICONTROL Flash Tag] 광고주 또는 웹 사이트 담당자에게 제공할 필드(필요한 경우).

            광고주의 IT 부서 또는 다른 그룹은 태그 배포를 예약하거나 그에 대한 정보를 받아야 할 수 있습니다.
   1. 클릭 **[!UICONTROL Save]**.

**[!UICONTROL 3rd-party Fees]:** (선택 사항) 1000회 노출당 청구할 수 없는 비용으로 추적할 정적 서드파티 요금. 다른 값을 입력하지 않으면 새 배치에 패키지 수준 기본값이 자동으로 적용됩니다.

>[!NOTE]
>
>청구 가능 요금은 다음에 반영됩니다. [!UICONTROL Net CPM] 지표.

>[!MORELIKETHIS]
>
>* [배치 관리 정보](placement-about.md)
>* [배치 만들기](placement-create.md)
>* [배치 편집](placement-edit.md)
>* [배치에 대한 입찰 승수 관리](placement-manage-bid-multipliers.md)
>* [배치에 대한 변경 로그 보기](placement-change-log.md)
>* [키보드 단축키](/help/dsp/campaign-management/reports/keyboard-shortcuts.md)
>* [Campaign Management에 대한 FAQ](/help/dsp/campaign-management/faq-campaign-management.md)
