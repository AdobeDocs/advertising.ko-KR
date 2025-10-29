---
title: 배치 설정
description: 사용 가능한 배치 설정에 대한 설명을 참조하십시오.
feature: DSP Placements
exl-id: 5b2574be-5d08-4cf7-910e-deac48d7e035
source-git-commit: f8f877552018de50649fbba22c56452775e72df3
workflow-type: tm+mt
source-wordcount: '4436'
ht-degree: 0%

---

# 배치 설정

## [!UICONTROL Basics]

**[!UICONTROL Placement name]** 배치 이름입니다.

>[!TIP]
>상황에 맞는 명명 규칙을 사용하십시오. 제안된 명명 규칙 중 하나는 &quot;*\&lt;캠페인 이름\>: \&lt;광고 단위\>: \&lt;기간\>: \&lt;타깃팅\>*&quot;입니다.

**[!UICONTROL Status]:** 배치 상태: *[!UICONTROL Active]*(기본값) 또는 *[!UICONTROL Paused]*.

>[!TIP]
>가장 좋은 방법은 시작할 준비가 될 때까지 배치를 일시 중지하는 것입니다.

**[!UICONTROL Details]:**(읽기 전용) 해당 광고 유형, 배치를 만들거나 만든 계정 및 상위 캠페인입니다. 자세한 내용을 보려면 **[!UICONTROL Show more]**&#x200B;을(를) 클릭하십시오.

**[!UICONTROL Templates]:** 기존 배치 템플릿 목록을 엽니다. 템플릿에서 타깃팅 설정을 자동으로 채우려면 다음을 수행합니다.

1. 다음 중 하나를 수행합니다.

   * 템플릿의 모든 대상을 재사용하려면 템플릿 이름 옆에 있는 확인란을 선택합니다.

   * 템플릿에서 개별 대상 유형을 재사용하려면 템플릿 이름을 확장하고 재사용할 대상 유형 옆의 확인란을 선택합니다.

1. **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

**[!UICONTROL Ad specs for forecast]:**(비디오 광고 형식만 해당) 오른쪽의 예측 프로젝션을 계산하는 데 사용되는 광고 기간 및/또는 광고 사양입니다. 필드는 광고 유형에 따라 다릅니다.

**[!UICONTROL Environment]:**(범용 비디오 광고 형식만 해당) 배치에 대상으로 포함할 장치 환경(데스크톱, 모바일, 연결된 TV)입니다. 최소 하나 이상을 지정하십시오.

사용자 지정 보고서에서 배치 수준 차원 &quot;장치 환경&quot;은 타깃팅된 환경을 나타냅니다.

**[!UICONTROL Placement tags]:**(선택 사항) 이 배치를 찾는 데 도움이 되는 키워드 또는 닉네임입니다.

## 목표

**[!UICONTROL Package]:**(선택 사항) 배치가 지정된 패키지입니다. 기존 패키지를 선택하거나 패키지를 만들려면 ![편집](/help/dsp/assets/edit.png)을 클릭합니다. 패키지에 배치를 할당하면 패키지의 비행 날짜, 배달 목표 및 예산이 포함된 [!UICONTROL Goals] 섹션이 업데이트됩니다.

**[!UICONTROL Flight Dates]:** 배치의 시작 날짜와 종료 날짜입니다. 승인된 광고는 배치가 활성 상태이고 활성 패키지 또는 캠페인에 할당된 경우 비행 중에 실행할 수 있습니다.

패키지(해당되는 경우) 또는 캠페인에 대한 날짜는 기본적으로 자동으로 채워집니다.

>[!NOTE]
>
>* 비행 날짜는 캠페인 비행 날짜와 패키지 비행 날짜 내에 포함되어야 합니다.

### 패키지 수준 게재 간격이 있는 패키지에 할당된 배치

**[!UICONTROL Placement Funding]:** 배치에 대한 예산을 책정하는 방법:

* *[!UICONTROL Optimize based on performance]:* 패키지 수준에서 예산을 제어합니다.
* *[!UICONTROL Set a Fixed Minimum or Maximum Budget]:* 최소 및/또는 최대 배치 예산을 설정할 수 있습니다. 최소 하나 이상의 예산 유형을 지정합니다.

   * *[!UICONTROL Maximum Budget]*: 값 및 기간(*[!UICONTROL All time]*, *[!UICONTROL Daily]*, *[!UICONTROL Weekly]*, *[!UICONTROL Monthly]*)을 입력하십시오.

   * *[!UICONTROL Minimum Budget]*: 패키지 예산의 최소 예산 비율입니다. 간격 상한을 지정하면 최소 예산 값은 항상 간격 상한의 백분율로 계산됩니다. 그렇지 않으면 패키지 예산의 백분율로 계산됩니다.

**[!UICONTROL Max Bid]:** 1000회 노출 시 최대 결제 금액입니다.

**[!UICONTROL Min Bid]:**(비공개 및 [!DNL On-Demand] 거래에만 해당) 인벤토리 유형에 따른 최소 입찰가입니다. 옵션을 선택합니다.

* *[!UICONTROL None]*: 인벤토리 유형에 대한 최소 입찰이 없습니다. 계산된 입찰가가 타겟팅된 거래의 고정/기본 가격보다 낮은 경우 DSP은 입찰하지 않습니다. 이는 규모에 영향을 미칠 수 있습니다.

* *[!UICONTROL Fixed/floor price for Private deals only]*: DSP은 알고리즘 계산식 입찰이 더 적더라도 타깃팅된 비공개 딜에 대해 최소 고정/최저 가격을 입찰합니다. 성능에 영향을 줄 수 있습니다.

* *[!UICONTROL Fixed/floor price for On-demand deals only]*: DSP은 알고리즘 계산식 입찰이 더 적더라도 타겟팅된 [!DNL On-Demand] 거래의 고정/최저 가격을 입찰합니다. 성능에 영향을 줄 수 있습니다.

* *[!UICONTROL Fixed/floor price for both Private and On-demand deals]*: DSP은 알고리즘 계산식 입찰이 더 적더라도 타겟팅된 비공개 및 [!DNL On-Demand] 거래의 고정/최저 가격을 입찰합니다. 성능에 영향을 줄 수 있습니다.

**[!UICONTROL Placement Pre-bid Filters]:** 입찰을 진행하려면 충족해야 하는 최대 5개의 KPI 임계값(예: 최소 가시성 지표 또는 클릭스루 비율)이 있습니다. 최적화 전술로 사전 입찰 필터를 사용할 수 있지만 각 규칙은 이 배치가 입찰할 수 있는 기회를 제한할 수 있습니다. 필터를 추가하거나 편집하려면:

1. ![편집](/help/dsp/assets/edit.png)을 클릭합니다.
1. 다음 중 하나를 수행합니다.
   * 필터를 추가하려면 다음 작업을 수행하십시오.
      1. **[!UICONTROL Add Filter]**&#x200B;을(를) 클릭합니다.
      1. **[!UICONTROL Only bid if]** 옆에 있는 지표를 선택한 다음 값을 입력하십시오.
   * 필터를 제거하려면 필터 행에서 **[!UICONTROL X]**&#x200B;을(를) 클릭합니다.
1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

&quot;[배치 수준 사전 입찰 필터 및 사용 방법](/help/dsp/optimization/optimization-pre-bid-filters.md)&quot;에서 각 사전 입찰 필터에 대한 설명을 참조하십시오.

### 기타 모든 배치

**[!UICONTROL Budget Goal]:** 총 예산 상한 및 예산 간격(*[!UICONTROL All time]*, *[!UICONTROL Daily]*, *[!UICONTROL Weekly]*, *[!UICONTROL Monthly]*)입니다.

**[!UICONTROL Gross Budget Goal]:**(마진 관리 전용 캠페인에 배치) 총 예산 상한 및 예산 간격(*[!UICONTROL All time]*, *[!UICONTROL Daily]*, *[!UICONTROL Weekly]*, *[!UICONTROL Monthly]*).

**[!UICONTROL Optimization Goal]:** 패키지의 최적화 목표입니다. &quot;[최적화 목표 및 사용 방법](/help/dsp/optimization/optimization-goals.md)&quot;에서 각 최적화 목표에 대한 설명을 참조하십시오.

**[!UICONTROL Target Goal]:** 성능을 추적하는 데 사용되는 대상 목표입니다.

>[!NOTE]
>
>이 필드는 벤치마크일 뿐이며 의사 결정에는 사용되지 않습니다.

**[!UICONTROL Pace on]:** 게재 간격 기준:

* **[!UICONTROL Budget goal]:**(기본값) 이 옵션은 할당된 예산 내에서 가능한 한 많은 노출 횟수를 제공합니다.

* **[!UICONTROL Impressions]:** 이 옵션은 지정된 간격 내에 지정된 수량에 도달할 때까지 노출을 전달합니다. 이 옵션을 선택할 때 노출 횟수와 간격: *[!UICONTROL All time],* *[!UICONTROL Daily],* *[!UICONTROL Monthly],* 또는 *[!UICONTROL Weekly]*&#x200B;을(를) 지정합니다.

**[!UICONTROL Max Bid]:** 1000회 노출 시 최대 결제 금액입니다.

**[!UICONTROL Flight pacing]:**(배치 수준 게재 속도만 있는 배치) 광고 게재 속도를 조정하는 방법:

* *[!UICONTROL Even]:*(기본값) 각 항공편 전체에 걸쳐 게재를 균등하게 처리하며, 목표는 항공편 전반부의 50%입니다.

* *[!UICONTROL Slightly Ahead]:*(기본값) 게재를 가속화하여 플라이트 기간 중간에 55~65% 완료됩니다.

* *[!UICONTROL Frontload]:* 배달 속도를 높여 비행 중간에 65~75% 완료됩니다.

* *[!UICONTROL Aggressive Frontload]:* 배달 속도를 높여 비행 중간에 75~85% 완료됩니다.

**[!UICONTROL Intraday pacing]:**(배치 수준 게재 속도만 있는 배치) 비행 내에서 매일 광고 게재의 속도를 조정하는 방법:

* *[!UICONTROL Even]:*(기본값) 인벤토리 가용성에 따라 게재 크기를 조정합니다. 일반적으로 경매량이 많은 낮에는 시간당 더 많은 광고가 게재되고 아침과 저녁에는 더 적은 수의 광고가 게재된다.

* *[!UICONTROL ASAP]:*(기본값) 게재를 *짝수*&#x200B;의 두 배 속도로 가속합니다.

  >[!CAUTION]
  >
  >이 옵션은 성능에 부정적인 영향을 줄 수 있습니다. 성능 최적화에 비해 게재 우선 순위 및 비용을 완전히 우선시하는 경우에만 사용하십시오.

**[!UICONTROL Placement Pre-bid Filters]:**(선택 사항) 입찰을 진행하려면 최대 5개의 필터를 충족해야 합니다. 최적화 전술로 사전 입찰 필터를 사용할 수 있지만 각 규칙은 이 배치가 입찰할 수 있는 기회를 제한할 수 있습니다. 필터를 추가하거나 편집하려면:

1. ![편집](/help/dsp/assets/edit.png)을 클릭합니다.
1. 다음 중 하나를 수행합니다.
   * 필터를 추가하려면 다음 작업을 수행하십시오.
      1. **[!UICONTROL Add Filter]**&#x200B;을(를) 클릭합니다.
      1. **[!UICONTROL Only bid if]** 옆에 있는 지표를 선택한 다음 값을 입력하십시오.
   * 필터를 제거하려면 필터 행에서 **[!UICONTROL X]**&#x200B;을(를) 클릭합니다.
1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## [!UICONTROL Geo-Targeting]

**[!UICONTROL Audience Location]:**(선택 사항) 배치에 광고를 포함하거나 제외할 특정 위치입니다. 위치를 지정하지 않으면 모든 위치가 타깃팅됩니다.

>[!NOTE]
>
>Roku 배치에 도시 및 DMA 위치를 사용할 수 없습니다.

위치를 지정하려면 다음을 수행합니다.

1. ![편집](/help/dsp/assets/edit.png)을 클릭합니다.
1. 다음 중 하나를 수행합니다.
   * 국가, 주, 도시, DMA, 연방 입법 지구 또는 주 입법 지구를 포함하거나 제외하려면 다음을 수행합니다.
      1. 왼쪽 열에서 위치 유형을 선택합니다.
      1. (필요한 경우) 확장할 위치를 클릭합니다.
      1. 위치 옆에 있는 *[!UICONTROL Include]*&#x200B;을(를) 클릭하여 대상으로 포함하거나 *[!UICONTROL Exclude]*&#x200B;을(를) 클릭하여 대상으로 제외합니다.
   * 우편 번호를 검색하고 선택한 모든 결과를 포함하거나 제외하려면
      1. **[!UICONTROL Search Postal Code]**&#x200B;을(를) 클릭합니다.
      1. 국가를 선택합니다.
      1. 구/군/시 이름을 입력한 다음 ![편집](/help/dsp/assets/search.png)을 클릭합니다.
      1. 올바른 검색 결과를 클릭합니다.
      1. 모든 위치를 대상으로 포함하려면 *[!UICONTROL Include All]*&#x200B;을(를) 클릭하고, 모든 위치를 대상으로 제외하려면 *[!UICONTROL Exclude All]*&#x200B;을(를) 클릭하십시오.
   * 우편 번호를 입력하거나 붙여 넣고 모두 포함하거나 제외하려면 다음을 수행합니다.
      1. **[!UICONTROL Paste Postal Code]**&#x200B;을(를) 클릭합니다.
      1. 국가를 선택합니다.
      1. 최대 1000개의 우편 번호를 입력하거나 붙여넣습니다.
한 줄에 하나의 우편 번호를 포함하거나, 쉼표 또는 탭으로 구분된 여러 값을 입력합니다.
      1. 모든 위치를 대상으로 포함하려면 *[!UICONTROL Include All]*&#x200B;을(를) 클릭하고, 모든 위치를 대상으로 제외하려면 *[!UICONTROL Exclude All]*&#x200B;을(를) 클릭하십시오.
   * [!UICONTROL Included] 또는 [!UICONTROL Excluded] 목록에서 위치를 제거하려면 오른쪽 열의 위치 옆에 있는 **[!UICONTROL X]**&#x200B;을(를) 클릭합니다.
1. **[!UICONTROL Done]**&#x200B;을(를) 클릭합니다.

>[!NOTE]
>
>* 모든 국가에 주, 도시 또는 우편 번호 위치가 있는 것은 아닙니다.
>* DMA(지정 시장 지역), 연방 입법 지구 및 주 입법 지구는 미국 지역에서만 사용할 수 있습니다.

## [!UICONTROL Inventory Targeting]

**[!UICONTROL Inventory Sources]:** 대상으로 포함하거나 제외할 인벤토리 소스입니다. 대부분의 배치 유형에는 기본적으로 모든 재고 유형과 각 유형의 모든 소스가 포함됩니다. [!DNL Roku] 배치의 경우 인벤토리 유형 및 소스를 지정해야 합니다. 다음 유형의 재고 중에서 선택할 수 있습니다.

* [!UICONTROL Public]: (Roku를 제외한 모든 배치 유형) DSP이 액세스할 수 있는 모든 열려 있는 exchange 인벤토리입니다. 공개 인벤토리를 포함 및 제외할 수 있습니다.

  소스 또는 피드별로 목록을 볼 수 있습니다. 피드별로 목록을 볼 때 피드 이름, 피드 키 또는 선택한 특성 태그로 검색할 수 있습니다.

* [!UICONTROL Private] | [!UICONTROL Roku Private]: DSP에서 설정한 게시자와의 기존 비공개 거래(또는 [!DNL Roku] 배치에 대한 기존 비공개 [!DNL Roku] 거래) 및 기존 [비공개 거래 목록](/help/dsp/inventory/lists-deals-manage.md). 공개 인벤토리를 포함할 수 있지만 제외할 수는 없습니다.

  [!UICONTROL Deals] 탭에서 키워드, 키, 거래 ID 또는 사용자 지정 태그로 목록을 검색할 수 있습니다. [!UICONTROL Deal Lists] 탭에서 거래 목록 이름 또는 거래 목록 ID별로 목록을 검색할 수 있습니다.

* [!UICONTROL On Demand] | [!UICONTROL Roku On Demand]: [에서 구독한 모든 [!UICONTROL On Demand]premium, 보장되지 않는 ](/help/dsp/inventory/on-demand-inventory-about.md) 인벤토리[!UICONTROL On Demand]&#x200B;(또는 [!DNL Roku] 배치에 대해 [!DNL Roku]개의 [!DNL DSP] 거래). [!UICONTROL On Demand] 인벤토리를 포함 및 제외할 수 있습니다.

  소스 또는 피드별로 목록을 볼 수 있습니다. 피드별로 목록을 볼 때 피드 이름, 피드 키 또는 선택한 게시자 영역, 범주 태그 또는 특성 태그별로 검색할 수 있습니다.

재고 타깃팅을 지정하려면 다음을 수행합니다.

* 재고 유형을 제외하려면 이름 옆에 있는 확인란의 선택을 취소합니다.
* 재고 유형을 대상으로 지정하려면
   1. 재고 유형명 옆에 있는 체크박스를 선택합니다.
   1. (선택 사항) 포함할 소스를 변경합니다.
      1. ![편집](/help/dsp/assets/edit.png)을 클릭합니다.
      1. ([!UICONTROL Public] 및 [!UICONTROL On Demand] 인벤토리) **[!UICONTROL View by Source]** 또는 **[!UICONTROL View by Feed]**&#x200B;을(를) 클릭하여 원본 나열 방법을 변경합니다.
      1. (해당되는 경우) 필요에 따라 재고를 필터링합니다.
      1. 포함 및 제외할 소스를 지정합니다.
         * [!UICONTROL Public] 또는 [!UICONTROL On Demand] 인벤토리의 경우:
            * 원본을 포함하려면 원본 이름 옆에 있는 **[!UICONTROL Include]**&#x200B;을(를) 클릭합니다.
            * 원본을 제외하려면 원본 이름 옆에 있는 **[!UICONTROL Exclude]**&#x200B;을(를) 클릭합니다.
         * [!UICONTROL Private] 인벤토리의 경우:
            * [!UICONTROL Deals] 탭에서:
               * 거래에 모든 인벤토리를 포함하려면 거래 이름 옆에 있는 **[!UICONTROL Include all]**&#x200B;을(를) 클릭합니다.
               * 개별 재고 출처를 포함하려면 거래명을 확장한 다음 출처명 옆에 있는 확인란을 누릅니다.
            * [!UICONTROL Deal Lists] 탭에서 거래 목록 이름 옆의 확인란을 클릭합니다.
   1. (선택 사항) 타깃팅 정보가 포함된 CSV 파일을 브라우저의 다운로드 위치로 다운로드하려면 **[!UICONTROL Export]**&#x200B;을(를) 클릭합니다.
   1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

>[!TIP]
>
>[!UICONTROL On Demand] 인벤토리를 구독했지만 타겟팅할 게시자나 거래를 찾을 수 없는 경우 거래의 상태를 확인하십시오. 상태에 대한 자세한 내용은 [정보 [!DNL On Demand] 프리미엄 인벤토리](/help/dsp/inventory/on-demand-inventory-about.md)를 참조하세요.

재고 특성별 **[!UICONTROL Video targeting]:** 대상(제외는 아님) 인벤토리를 구성합니다. 동일한 비디오 속성에 대해 여러 값을 타겟팅하면 선택한 속성 중 하나를 타겟팅할 수 있습니다(예: \[Player size = large 또는 Player size = HD\]). 여러 속성을 대상으로 하는 경우 지정된 각 속성이 있어야 합니다(예: \[Duration = 30-60분] 및 \[Player size = large 또는 Player size = HD\]).

* 플레이어 크기별 **[!UICONTROL Player size]:** 대상(제외할 수 없음) 인벤토리를 구성합니다. 이 설정은 데스크탑 및 모바일 환경에 대한 프리롤 배치, 모바일 표준 프리롤 배치 및 범용 비디오 배치에 적용됩니다. 기본적으로 모든 크기가 타깃팅됩니다. 대상 범위를 좁히려면 특정 대상 크기 및/또는 *알 수 없음*&#x200B;을 선택하세요.

* 재생이 시작되는 방식별 **[!UICONTROL Playback mode]:** 대상(제외는 아님) 인벤토리를 작성합니다. 이 설정은 데스크탑 및 모바일 환경에 대한 프리롤 배치, 모바일 표준 프리롤 배치 및 범용 비디오 배치에 적용됩니다. 기본적으로 모든 모드가 타깃팅됩니다. 대상 범위를 좁히려면 특정 대상 모드 및/또는 *알 수 없음*&#x200B;을 선택하세요.

* **[!UICONTROL Skippability]:** 스킵할 수 있는지 여부에 따라 대상(제외할 수는 없음) 인벤토리를 구성합니다. 이 설정은 프리롤, 모바일 표준 프리롤, 연결된 TV 및 범용 비디오 배치를 포함한 모든 VAST/VPAID 배치에 적용됩니다. 기본적으로 모든 옵션이 타깃팅됩니다. 대상 범위를 좁히려면 특정 대상 및/또는 *알 수 없음*&#x200B;을 선택하세요.

광고 위치별 **[!UICONTROL Position targeting]:** 대상(제외는 아님) 인벤토리. 이 설정은 프리롤, 모바일 표준 프리롤, 연결된 TV 및 범용 비디오 배치를 포함한 모든 VAST/VPAID 배치에 적용됩니다. 기본적으로 모든 Position을 타겟팅합니다. 대상 범위를 좁히려면 특정 대상 위치 및/또는 *알 수 없음*&#x200B;을 선택하세요.

## [!UICONTROL Site or App and Keyword Targeting]

**[!UICONTROL Traffic type]:** 대상에 대한 트래픽 유형입니다. 옵션은 **[!UICONTROL Websites]** 및 **[!UICONTROL Apps]**&#x200B;입니다.

**[!UICONTROL Tier]:**(**[!UICONTROL Toggle for Sites or Apps Tiering]**&#x200B;이(가) *[!UICONTROL On]*&#x200B;인 경우 사용 가능) 대상 트래픽의 품질입니다. 계층 1-3은 모두 브랜드에 적합하며 DSP 매핑 팀에서 승인했습니다.

* 전국적으로 인식할 수 있는 Premium 사이트 및 응용 프로그램이 *[!UICONTROL Tier 1]:*&#x200B;개 있습니다.

* *[!UICONTROL Tier 2]:*&#x200B;은(는) 계층 1과 계층 1보다 덜 널리 알려진 품질 사이트 및 응용 프로그램을 대상으로 합니다.

* *[!UICONTROL Tier 3]:* 대상 계층 1-2와 적절한 브랜드 보호 사이트 및 응용 프로그램을 적절히 사용할 수 있도록 합니다. 도달 또는 데이터 타겟팅 구매에 계층 3을 사용합니다.

* *[!UICONTROL All Sites or Apps]:*&#x200B;은(는) 계층 1-3과 선별되거나 분류되지 않은 새 인벤토리를 대상으로 하며 도달 시 사용할 수 있습니다.

>[!NOTE]
>
>인벤토리는 배치의 광고 단위에만 적용됩니다.

>[!TIP]
>
>성과 캠페인의 경우 가장 좋은 방법은 *[!UICONTROL All Sites]*&#x200B;을(를) 선택하는 것입니다.

**[!UICONTROL Site or App Categories]:**(선택 사항) 선택한 트래픽 유형 내의 사이트 범주 및 (지정된 경우) 타겟으로 포함하거나 제외할 사이트 계층(둘 다 포함하지는 않음)입니다. DSP이 제목을 기반으로 매핑한 세로 사이트 목록 중에서 선택합니다.

1. ![편집](/help/dsp/assets/edit.png)을 클릭합니다.
1. 포함 또는 제외할 사이트 범주를 지정합니다.
   * 사이트 범주를 포함하려면 다음 작업을 수행하십시오.
      1. **[!UICONTROL Include categories]**&#x200B;을(를) 클릭합니다.
      1. 타깃팅할 각 카테고리 옆에 있는 확인란을 선택합니다.
   * 사이트 범주를 제외하려면 다음 작업을 수행하십시오.
      1. **[!UICONTROL Exclude categories]**&#x200B;을(를) 클릭합니다.
      1. 제외할 각 범주 옆에 있는 확인란을 선택합니다.
1. (선택 사항) 타깃팅 정보가 포함된 CSV 파일을 브라우저의 다운로드 위치로 다운로드하려면 **[!UICONTROL Export]**&#x200B;을(를) 클릭합니다.
1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

**[!UICONTROL Exclude Sites or Apps]:**(선택 사항, **[!UICONTROL Toggle for Sites or Apps Tiering]**&#x200B;이(가) *[!UICONTROL On]*&#x200B;인 경우 사용 가능) 제외할 사이트/앱 및 [URL 목록](/help/dsp/resources/lists-url-manage.md). [!UICONTROL Paste URL] 탭에서 사이트를 검색하여 선택하거나 도메인 이름을 입력하거나 붙여 넣을 수 있습니다. [!UICONTROL URL Lists] 탭에서 URL 목록을 선택할 수 있습니다.

1. ![편집](/help/dsp/assets/edit.png)을 클릭합니다.
1. 사이트를 지정합니다.
   * [!UICONTROL Paste URL] 탭에서:
      * 사이트를 검색하려면 다음 작업을 수행하십시오.
         1. **[!UICONTROL Search]**&#x200B;을(를) 클릭합니다.
         1. 키워드를 입력하거나, 사이트 계층을 선택하거나, 사이트 카테고리를 선택합니다.
         1. 검색 결과에서 제외할 사이트를 선택합니다.
            * 개별 사이트를 제외하려면 인접한 확인란을 선택합니다.
            * (50개 이상의 결과를 사용할 수 있는 경우) 처음 50개의 결과를 제외하려면 **[!UICONTROL Exclude these 50]**&#x200B;을(를) 클릭합니다. 모든 검색 결과를 제외하려면 **[!UICONTROL Exclude these \<*NN *\>]**을(를) 클릭합니다.
      * 도메인 이름을 입력하려면 다음을 수행합니다.
         1. **[!UICONTROL Paste]**&#x200B;을(를) 클릭합니다.
         1. 별도의 줄에 도메인 이름을 하나 이상 입력합니다.
         1. **[!UICONTROL Exclude All]**&#x200B;을(를) 클릭합니다.
   * [!UICONTROL URL Lists] 탭에서:
      1. (선택 사항) 검색 필드에 목록 이름의 전체 또는 일부를 입력하여 URL 목록을 검색합니다.
      1. 제외할 각 URL 목록 옆에 있는 확인란을 선택합니다.
1. 완료되면 **[!UICONTROL Done]**&#x200B;을(를) 클릭합니다.

>[!NOTE]
>
>* 광고에는 안전하지 않은 것으로 간주되는 사이트가 포함된 DSP [전역 차단 사이트 목록](/help/dsp/introduction/features/brand-safety-media-quality.md) 외에 계정 수준 및 광고주 수준의 차단 사이트 목록도 적용됩니다.
>* 차단된 사이트 목록은 항상 타겟팅된 사이트 및 사이트 목록을 재정의합니다. 배치가 둘 다 광고에 대한 동일한 타겟을 제외하고 포함하면 타겟은 제외됩니다.

**[!UICONTROL Context of Sites or App]:**(선택 사항) 타깃팅하거나 제외할 컨텍스트 기반 대상 세그먼트. 다음 L 중에서 선택

* **[!UICONTROL Marketplace]** 탭: 모든 사용자가 지정된 요금으로 사용할 수 있는 [!DNL Peer39]개의 세그먼트를 나열합니다.

* **[!UICONTROL Custom Segments]** 탭: 조직의 [!DNL Peer39] 사용자 지정 세그먼트를 나열합니다.

* **[!UICONTROL Paste Segments]** 탭: (조직에 [!DNL Comscore] 파트너십이 있는 광고주, Adobe 계정 팀의 활성화 이후에 사용 가능) 조직의 [!DNL Comscore] 컨텍스트 세그먼트에 대해 하나 이상의 세그먼트 ID 또는 세그먼트 이름을 입력합니다. 여러 값을 쉼표로 구분합니다(예: Segment1, Segment2, Segment3).

**[!UICONTROL Language]:**(선택 사항) 타깃팅할 단일 언어입니다.

**[!UICONTROL Site or app list preview]:**(읽기 전용, **[!UICONTROL Toggle for Sites or Apps Tiering]**&#x200B;이(가) *[!UICONTROL On]*&#x200B;인 경우 사용 가능) 계정 수준, 광고주 수준 및 DSP 전역 차단 사이트 목록의 사이트/앱을 포함하여 배치에 대해 타깃팅되고 차단된 모든 사이트/앱입니다.

선택적으로 타겟팅되고 차단된 사이트 목록을 쉼표로 구분된 값(CSV) 파일로 내보낼 수 있습니다. 목록을 내보내려면 **[!UICONTROL Export full site list]**&#x200B;을(를) 클릭한 다음 브라우저의 일반 절차에 따라 파일을 열거나 저장합니다.

**[!UICONTROL Allow unscreened sites]:**(표준 표시 배치만 해당) 감사되지 않은 사이트에서 광고 배달을 사용하도록 설정합니다. 배치가 개인 인벤토리를 타겟팅하면 이 옵션은 차단된 사이트에 광고를 게재할 수 있습니다.

**[!UICONTROL Toggle for Sites or Apps Tiering]:** 타겟팅하거나 제외할 사이트 또는 앱 계층을 지정할 수 있습니다.

## [!UICONTROL Audience Targeting]

**[!UICONTROL Included Audiences]:** [타사 세그먼트, 자사 세그먼트, Adobe 세그먼트, 사용자 지정 세그먼트 및 저장된 대상을 포함하여 배치에 대한 모든 대상 대상](/help/dsp/audiences/audience-settings.md). 선택한 모든 세그먼트 및 저장된 대상자 전체에 걸쳐 중복 제거된 총 활성 대상자 크기도 표시됩니다. 기존 대상을 선택하거나, 나중에 다시 사용할 수 있는 대상을 만들거나, 특정 대상 세그먼트를 선택할 수 있습니다.

* 기존 대상을 선택하려면 ![ 옆에 있는 ](/help/dsp/assets/chevron-down.png)선택[!UICONTROL Included Audiences]을 클릭한 다음 대상을 선택하십시오.
* 대상을 만들려면 ![ 옆에 있는 ](/help/dsp/assets/chevron-down.png)선택[!UICONTROL Included Audiences]을 클릭한 다음 **[!UICONTROL + Create Audience]**&#x200B;을(를) 선택하십시오. 지침은 3단계부터 [재사용 가능한 대상 만들기](/help/dsp/audiences/reusable-audience-create.md)를 참조하십시오.
* 특정 대상 세그먼트를 선택하려면 **[!UICONTROL Select segments for this placement only]**&#x200B;을(를) 클릭하십시오. 세그먼트 논리를 선택합니다. 지침은 &quot;[재사용 가능한 대상 만들기](/help/dsp/audiences/reusable-audience-create.md)&quot;의 6단계를 참조하십시오. 완료되면 **저장**&#x200B;을 클릭하세요.

>[!NOTE]
>
>활성, 예약됨 또는 일시 중지됨 배치에 첨부되지 않은 자사 RampID 세그먼트는 일시 중지됩니다. 세그먼트는 세그먼트 목록에 &quot;자동 일시 중지됨&quot;으로 표시됩니다.

**[!UICONTROL Excluded Audiences]:** [타사 세그먼트, 자사 세그먼트, Adobe 세그먼트, 사용자 지정 세그먼트 및 저장된 대상을 포함하여 배치에 대해 제외할 대상](/help/dsp/audiences/audience-settings.md)입니다. 제외된 모든 대상에 걸쳐 중복 제거된 총 활성 대상 크기도 표시됩니다. 기존 대상을 선택하거나 나중에 다시 사용할 수 있는 새 대상을 만들 수 있습니다.

* 기존 대상을 선택하려면 ![ 옆에 있는 ](/help/dsp/assets/chevron-down.png)선택[!UICONTROL Excluded Audiences]을 클릭한 다음 대상을 선택하십시오.

* 대상을 만들려면 ![ 옆에 있는 ](/help/dsp/assets/chevron-down.png)선택[!UICONTROL Excluded Audiences]을 클릭한 다음 **+ 대상 만들기**&#x200B;를 선택하십시오. 지침은 3단계부터 [재사용 가능한 대상 만들기](/help/dsp/audiences/reusable-audience-create.md)를 참조하십시오.

**[!UICONTROL Targeting]:** 타깃팅할 사용자 ID의 유형입니다. 배치가 라이브 상태가 된 후(즉, 비행이 시작된 후) 이 설정을 변경할 수 없습니다.

기존 ID와 범용 ID를 모두 선택하면 범용 ID에 입찰 기본 설정이 지정됩니다.

* *[!UICONTROL Legacy IDs (Cookies, MAIDS, CTV)]*: (기본값) 쿠키, 모바일 광고 ID 또는 연결된 TV(CTV) ID를 기준으로 사용자를 타깃팅합니다. ID는 브라우저, 인앱 또는 CTV 인벤토리를 기반으로 선택됩니다.

* *[!UICONTROL Universal ID Beta]*: 사용자 개인 정보 보호 중심의 ID를 대상으로 합니다. ID 유형을 하나 선택하십시오. 사용 가능한 옵션은 [!UICONTROL Geo-Targeting] 섹션에서 선택한 지리적 대상에 의해 결정됩니다. [[!DNL RampID] DSP으로 직접 가져온 세그먼트](/help/dsp/audiences/sources/source-import-liveramp-segments.md), DSP에서 PII를 범용 ID로 변환하는 세그먼트[ 또는 ](/help/dsp/audiences/sources/source-about.md)범용 ID를 추적하는 사용자 지정 세그먼트[에 사용합니다.](/help/dsp/audiences/custom-segment-create.md)

   * *[!UICONTROL ID5]*: 이메일 주소 및 기타 신호에서 [!DNL ID5] ID를 확률적으로 만들었습니다.<!-- What countries/geos are these available for? Everywhere?-->개의 ID5 ID를 무료로 사용할 수 있습니다. **참고:** [!DNL Eyeota]의 타사 세그먼트에는 ID5 ID가 포함될 수 있습니다.

   * *[!UICONTROL RampID]*: 사용자의 전자 메일 주소를 사용하여 사이트에 로그인한 [!DNL LiveRamp] [!DNL RampIDs]명의 사용자를 대상으로 합니다.<!-- Verify --> [!DNL RampIDs]은(는) 북미, 오스트레일리아 및 뉴질랜드의 사용자가 사용할 수 있습니다.

   * *[!UICONTROL Unified ID2.0]*: 이메일 주소를 사용하여 사이트에 로그인한 사용자의 [!DNL Unified ID2.0]&#x200B;(UID2) ID를 타겟팅합니다.<!-- Verify -->[!DNL UID2 IDs]은(는) 유럽 경제 지역 및 일부 추가 국가에서 사용할 수 없습니다. [금지 국가 목록](/help/policies/universal-id-policy.md#prohibited-countries-uid2)을 참조하세요.

  **[!UICONTROL Terms of service]**: 유니버설 ID 사용에 대한 서비스 약관. 데이터를 새 ID 유형으로 변환하려면 사용자나 DSP 계정의 다른 사용자가 약관에 한 번 동의해야 합니다. 관리 서비스 계약을 보유한 고객의 경우 Adobe 계정 팀이 사용자의 동의를 얻고 조직을 대신하여 약관에 동의합니다. 용어를 읽으려면 **>**&#x200B;을(를) 클릭합니다. 약관에 동의하려면 약관의 맨 아래로 스크롤하여 **[!UICONTROL Accept]**&#x200B;을(를) 클릭합니다.

**[!UICONTROL Cross Device Targeting]:**([campaign이 사용자 기반 교차 장치 타깃팅에 대해 구성된 경우 사용 가능](/help/dsp/campaign-management/campaigns/campaign-settings.md)), 레거시 ID만 타깃팅하고(범용 ID는 아님), 하나 이상의 세그먼트 또는 대상을 선택했습니다. 지정한 세그먼트에 없는 장치도, 개인의 알려진 모든 장치(캠페인 설정에 지정된 장치 그래프에 따라)로 타깃팅을 확장할 수 있습니다. 캠페인에 대해 지정된 그래프에 따라 요금이 적용될 수 있습니다. 장치 그래프 데이터는 북미에서만 사용할 수 있습니다.

**[!UICONTROL Placement Cap]:**(선택 사항) 게재에서 고유한 장치, 유니버설 ID 또는 사용자(캠페인에 대해 지정된 [!UICONTROL Cross Device Level] 및 배치의 [!UICONTROL Targeting] 설정에 따라 다름)가 광고를 제공할 수 있는 횟수입니다. 옵션에는 *[!UICONTROL Unlimited]* 또는 일, 주 또는 월당 특정 금액이 포함됩니다.

>[!NOTE]
>
> 캠페인, 패키지 및 배치 수준에서 빈도 상한을 설정할 수 있습니다. DSP은 캠페인 계층에서 가장 엄격한 빈도 상한을 준수합니다.

**[!UICONTROL Secondary Cap]:**(선택 사항, 숫자 [!UICONTROL Placement Cap]을(를) 포함하는 경우 사용 가능) 기본 배치 상한 내의 추가 제한입니다. 노출 횟수와 기간을 선택합니다(예: 12시간당 3회).

**[!UICONTROL Day Parting]:**(선택 사항) 광고가 실행될 수 있는 특정 요일 및 시간입니다. 시간 분할 간격을 지정하려면 다음을 수행합니다.

1. ![편집](/help/dsp/assets/edit.png)을 클릭합니다.
1. 적용 가능한 시간대를 선택합니다.
1. 간격 지정:
   * 사전 설정된 간격을 선택하려면 간격 단추 중 하나를 클릭합니다. 옵션에는 *[!UICONTROL Weekends]**, *[!UICONTROL Weekdays]*, *[!UICONTROL Morning]*, *[!UICONTROL Lunch]*, *[!UICONTROL Dinner]* 또는 *[!UICONTROL Prime]*(primetime)이 포함됩니다.
   * 간격을 수동으로 선택하려면 셀 내부를 클릭하고 선택적으로 드래그하여 간격을 선택합니다.
1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

**[!UICONTROL Topic Targeting]:**(선택 사항, [!DNL Proximic by Comscore] 세그먼트로 구성된 광고주에게 사용 가능) 대상으로 포함할 특정 세그먼트 이름 또는 [!DNL Proximic by Comscore]의 ID입니다. 이 기능에 대한 추가 비용이 발생할 수 있습니다. 이 기능을 활성화하고 주제 세그먼트를 설정하려면 Adobe 계정 팀에 문의하십시오.

주제 타깃팅을 지정하려면 다음을 수행합니다.

1. ![편집](/help/dsp/assets/edit.png)을 클릭합니다.
1. 타겟팅할 세그먼트 지정:
   1. 왼쪽 열에서 파트너(*[!UICONTROL Comscore]*)를 선택합니다.
   1. 입력 필드에 세그먼트 이름 또는 세그먼트 ID를 입력합니다.
1. (선택 사항) 주제 정보가 포함된 CSV 파일을 브라우저의 다운로드 위치에 다운로드하려면 **[!UICONTROL Export]**&#x200B;을(를) 클릭합니다.
1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

>[!TIP]
>
>* 주제 타깃팅은 배치가 입찰할 수 있는 인벤토리를 제한하므로 전체 구매에서 작은 비율에만 주제 타깃팅을 사용하십시오.
>
>* [!DNL Proximic by Comscore]의 세그먼트 내에서 부정적인 타깃팅을 설정합니다.

**[!UICONTROL Device Targeting]:**(선택 사항) 대상으로 포함 및 제외할 장치 유형, 제조업체, 운영 체제, 브라우저 및 연결 유형 등 특정 장치 정보입니다. 유형은 배치 유형에 따라 다릅니다. 장치 타깃팅을 지정하려면:

1. ![편집](/help/dsp/assets/edit.png)을 클릭합니다.
1. 포함 및 제외할 장치 세부 정보를 지정합니다.
   1. 왼쪽 열에서 범주를 선택합니다.
   1. 타깃팅 지정:
      * 값을 포함하려면 값 이름 옆에 있는 **[!UICONTROL Include]**&#x200B;을(를) 클릭합니다.
      * 값을 제외하려면 값 이름 옆에 있는 **[!UICONTROL Exclude]**&#x200B;을(를) 클릭합니다.
1. (선택 사항) 장치 타깃팅 정보가 포함된 CSV 파일을 브라우저의 다운로드 위치로 다운로드하려면 **[!UICONTROL Export]**&#x200B;을(를) 클릭합니다.
1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

**[!UICONTROL ISP Targeting]:**(선택 사항) 특정 ISP(인터넷 서비스 공급자)가 대상으로 포함 또는 제외(둘 다 아님)할 수 있습니다. ISP 타깃팅을 지정하려면 다음을 수행하십시오.

1. ![편집](/help/dsp/assets/edit.png)을 클릭합니다.
1. 포함 또는 제외할 ISP를 지정합니다.
   * ISP를 포함하려면:
      1. **[!UICONTROL Include ISPs]**&#x200B;을(를) 클릭합니다.
      1. (선택 사항) 키워드로 목록을 필터링합니다.
      1. 타깃팅할 각 ISP 옆에 있는 확인란을 선택합니다.
   * ISP를 제외하려면 다음을 수행하십시오.
      1. **[!UICONTROL Exclude ISPs]**&#x200B;을(를) 클릭합니다.
      1. (선택 사항) 키워드로 목록을 필터링합니다.
      1. 제외할 각 ISP 옆에 있는 확인란을 선택합니다.
1. (선택 사항) ISP 타깃팅 정보가 있는 CSV 파일을 브라우저의 다운로드 위치로 다운로드하려면 **[!UICONTROL Export]**&#x200B;을(를) 클릭하십시오.
1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## [!UICONTROL Brand Safety and Media Quality]

**[!UICONTROL DoubleVerify ABS segment ID]:**(선택 사항; [!DNL DoubleVerify] 고객만 해당; 데스크톱 프리롤, 표준 및 클릭-재생 디스플레이, 기본 디스플레이 및 비디오 배치에만 사용 가능; [거래의 기본 프로그램 보장 배치](/help/dsp/inventory/programmatic-guaranteed-about.md)에는 지원되지 않음) 배치에 사용할 조직의 [!DNL DoubleVerify Authentic Brand Safety] 계정과 연결된 [!DNL DoubleVerify] 세그먼트 ID입니다. ID를 지정하면 지정된 세그먼트 ID에 대해 구성된 사용자 지정 브랜드 안전 규칙을 사용하여 입찰 후 노출을 차단합니다. DSP은 세그먼트 ID에 대한 사용을 위해 계정에 청구합니다.

ID는 &quot;51&quot;로 시작하고 8자리 숫자로 구성되어야 합니다. 기본적으로 광고주 계정 설정에 세그먼트 ID가 지정되어 있으면 광고주 수준 ID가 입력되지만, 다른 세그먼트를 사용하도록 ID를 변경하거나 해당 ID를 삭제하여 기능을 비활성화할 수 있습니다.

**[!UICONTROL Contextual filtering]:**(데스크톱 및 모바일 웹 디스플레이, 기본 및 비디오 광고에 적용 가능) 적용할 [!DNL Comscore], [!DNL DoubleVerify], [!DNL Integral Ad Science] 및 [!DNL Peer39] 컨텍스트 필터의 유형. 새 배치에 대해 광고주 수준 기본값이 선택되지만 설정을 변경할 수 있습니다.

<!-- Looks like we didn't rename this:
**[!UICONTROL Brand Safety categories]:** Types of [!DNL Comscore], [!DNL DoubleVerify], [!DNL Integral Ad Science], and [!DNL Peer39] brand safety category filters to apply. The advertiser-level defaults are selected for new placements, but you can change the settings:
-->

* [!UICONTROL DoubleVerify]:

   * **[!UICONTROL Block sites that are]:**(선택 사항) 기본적으로 차단되는 하나 이상의 재고 컨텍스트 유형. 추가 요금이 부과될 수 있습니다.

* [!UICONTROL Peer 39]:

   * **타깃팅할 사이트:**(선택 사항) 기본적으로 타깃팅할 하나 이상의 재고 특성 유형. 추가 요금이 부과될 수 있습니다.

* [!UICONTROL ComScore]:

   * **사이트 차단:** (선택 사항) 기본적으로 차단해야 할 하나 이상의 인벤토리 특성 유형. 추가 요금이 부과될 수 있습니다.

* [!UICONTROL Integral Ad Science]

   * **[!UICONTROL Adult Content]:**(선택 사항) 기본적으로 광고를 차단할 성인 콘텐츠의 정도: *[!UICONTROL Do Not Block]*(기본값), *[!UICONTROL Standard]* 또는 *[!UICONTROL Strict]*. 추가 요금이 부과될 수 있습니다.

   * **[!UICONTROL Alcohol Content]:**(선택 사항) 기본적으로 광고를 차단할 알코올 도입니다. *[!UICONTROL Do Not Block]*(기본값), *[!UICONTROL Standard]* 또는 *[!UICONTROL Strict]*. 추가 요금이 부과될 수 있습니다.

**[!UICONTROL Pre-bid fraud blocking]:** [!DNL DoubleVerify], [!DNL Integral Ad Science] 및 [!DNL Peer39]을(를) 통해 측정된 사기 트래픽 및 의심스러운 활동을 기반으로 차단할 사이트 유형입니다. 새 배치에 대해 광고주 수준 기본값이 선택되지만 설정을 변경할 수 있습니다.

* [!UICONTROL DoubleVerify]: (데스크톱 및 모바일 웹 디스플레이, 기본, 비디오 및 표준 연결된 TV 광고에 적용 가능)

   * **[!UICONTROL Block Fraud Sites (100% Invalid traffic) and User-Based Fraud and IVT Devices]:** 기본적으로 새 배치에 대해 하이재핑된 장치의 트래픽을 포함하여 100% 잘못된 모든 트래픽을 차단합니다. 추가 요금이 부과될 수 있습니다.

   * **[!UICONTROL Also block sites with]:**(선택 사항) DSP에서 기본적으로 광고를 차단하는 추가적인 수준의 사기 및 잘못된 트래픽: *[!UICONTROL None]*(기본값: 추가 트래픽을 차단하지 않음), *[!UICONTROL >2% Average Fraud/IVT levels (lowest reach)]*, *[!UICONTROL >4% Average Fraud/IVT levels]*, *[!UICONTROL >6% Average Fraud/IVT levels]*, *[!UICONTROL >10% Average Fraud/IVT levels]* 또는 *[!UICONTROL >25% Average Fraud/IVT levels]*. 추가 요금이 부과될 수 있습니다.

* [!UICONTROL Peer 39]: (데스크톱 및 모바일 웹 디스플레이, 기본 및 비디오 광고에 적용 가능)

   * **[!UICONTROL Block sites that are]:**(선택 사항) DSP에서 기본적으로 광고를 차단하는 하나 이상의 사기 유형: *[!UICONTROL Fraud]*(사기로 모든 사이트를 차단함), *[!UICONTROL Fraud: Bot Sites_Non-Human traffic]* 및/또는 *[!UICONTROL Fraud: Zero Ads]*. 추가 요금이 부과될 수 있습니다.

* [!UICONTROL Integral Ad Science]: (데스크톱 및 모바일 웹 디스플레이, 기본 및 비디오 광고에 적용 가능)

   * **[!UICONTROL Block sites that are]:**(선택 사항) DSP에서 기본적으로 광고를 차단하는 의심스러운 웹 사이트 또는 앱 활동 유형: *[!UICONTROL None]*(기본적으로 의심스러운 활동에 따라 광고를 차단하지 않음), *[!UICONTROL Suspicious Activity - High Risk]* 또는 *[!UICONTROL Suspicious Activity - High or Moderate Risk]*. 추가 요금이 부과될 수 있습니다.

**[!UICONTROL Pre-bid viewability]:**(데스크탑 및 모바일 웹 디스플레이, 기본 및 비디오 광고에 적용 가능) [!DNL DoubleVerify] 및 [!DNL Integral Ad Science]이(가) 배치를 적용할 보기 가능 필터를 미리 입찰합니다. 새 배치에 대해 광고주 수준 기본값이 선택되지만 설정을 변경할 수 있습니다. 추가 요금이 부과될 수 있습니다.

**[!UICONTROL Ads.txt filtering]:**(데스크톱 및 모바일 웹 디스플레이, 기본, 비디오 및 오디오 광고에 적용 가능) 각 게시자의 Authorized Digital Sellers 목록을 적용하여 사용할 [Ads.txt](https://iabtechlab.com/ads-txt-about/) 수준의 사전 입찰 필터링. 새 배치에 대해 광고주 수준 기본값이 선택되지만 설정을 변경할 수 있습니다.

* *[!UICONTROL Opt out of ads.txt (default)]*: 모든 판매자의 인벤토리를 구매합니다.
* *[!UICONTROL Ads.txt sellers + sites without ads.txt]*: 도메인의 승인된 직접 판매자 및 리셀러로부터 인벤토리 구매의 우선 순위를 지정합니다.
* *[!UICONTROL Ads.txt sellers only]*: 도메인의 승인된 직접 판매자 및 리셀러에서만 인벤토리를 구매합니다.
* *[!UICONTROL Ads.txt sellers only]*: 도메인의 승인된 직접 판매자에서만 인벤토리를 구매합니다.

**[!UICONTROL Attention Targeting]:**(데스크톱 및 모바일 웹 디스플레이, 비디오 및 표준 연결된 TV 광고에 적용 가능) 지정된 사이트, 형식 및 광고 크기를 기반으로 특정 주의 수준(높음, 중간 또는 낮음)을 가진 [!DNL Adelaide] 사전 입찰 세그먼트를 타겟팅합니다. 세그먼트는 매주 업데이트됩니다. **참고:** 타깃팅에 [!DNL Adelaide] 세그먼트를 사용하면 [!DNL Adelaide] 주의 타깃팅으로 전달된 각 노출에 대해 CPM 비용이 발생합니다. 이 비용은 [주의 측정](/help/dsp/campaign-management/campaigns/campaign-settings.md)에 대한 비용과 별개입니다. 대화형 프리롤 배치의 경우 VAST 노출에 대해서만 요금이 부과됩니다.

## [!UICONTROL Tracking] {#placement-tracking}

>[!NOTE]
>
>([!DNL Roku]개 배치) [!DNL Roku]이(가) 승인한 서드파티 추적 공급업체는 [!DNL Acxiom], [!DNL Comscore], [!DNL Data Plus Math], [!DNL Experian], [!DNL Factual], [!DNL Kantar], [!DNL Marketing Evolution], [!DNL Neustar], [!DNL Nielsen], [!DNL Nielsen Catalina Solutions], [!DNL NinthDecimal], [!DNL Oracle], [!DNL Placed], [!DNL Polk] 및 [!DNL Research Now]입니다.

**[!UICONTROL Event Pixels]:**(선택 사항) 배치의 모든 새 광고에 기본적으로 첨부할 타사 이벤트 추적 픽셀입니다. 이벤트 픽셀을 지정하려면:

1. ![편집](/help/dsp/assets/edit.png)을 클릭합니다.
1. 다음 중 하나를 수행합니다.
   * 기존 픽셀을 선택하려면 픽셀 행에서 확인란을 선택합니다.
   * 픽셀을 만들려면 다음 작업을 수행하십시오.
      1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.
      1. 다음 정보를 입력합니다.
         * **[!UICONTROL Pixel name]:** 픽셀 이름입니다. 최대 길이는 500자입니다. 픽셀을 쉽게 식별하는 데 도움이 되는 이름을 사용합니다.
         * **[!UICONTROL Pixel event fires on]:** 픽셀을 실행하도록 트리거하는 이벤트입니다. 사용 가능한 이벤트는 광고 유형에 따라 다릅니다.
         * **[!UICONTROL Pixel type]:** 픽셀이 *[!UICONTROL IMG URL]*(1x1 픽셀 이미지 파일), *[!UICONTROL HTML]* 또는 *[!UICONTROL JavaScript URL]*&#x200B;인지 여부.
         * **[!UICONTROL Pixel URL]:** 픽셀 이미지의 URL.
      1. **[!UICONTROL Create and attach]**&#x200B;을(를) 클릭합니다.
   1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

**[!UICONTROL Conversion Pixels]:**(선택 사항) 기본적으로 배치의 모든 새 광고에 첨부할 전환 추적 픽셀입니다. 변환 픽셀을 지정하려면 다음을 수행합니다.

1. ![편집](/help/dsp/assets/edit.png)을 클릭합니다.
1. 다음 중 하나를 수행합니다.
   * 기존 픽셀을 선택하려면 픽셀 행에서 확인란을 선택합니다.
   * 픽셀을 만들려면 다음 작업을 수행하십시오.
      1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.
      1. 다음 정보를 입력합니다.
         * **[!UICONTROL Conversion pixel name]:** 픽셀 이름입니다. 최대 길이는 500자입니다. 픽셀을 쉽게 식별하는 데 도움이 되는 이름을 사용합니다.
         * **[!UICONTROL Conversion category]:** 변환 유형입니다.
         * **[!UICONTROL Impression conversion window]:** 광고 노출이 발생한 후 전환으로 노출이 귀속될 수 있는 일 수입니다. 기본값은 30일입니다.
         * **[!UICONTROL Click conversion window]:** 광고 클릭 발생 후 전환으로 인해 클릭이 발생할 수 있는 일 수입니다. 기본값은 30일입니다.
         * **[!UICONTROL Notes]:**(선택 사항) 픽셀에 대한 설명 또는 기타 정보입니다.
      1. **[!UICONTROL Create and attach]**&#x200B;을(를) 클릭합니다.
      1. 관련 웹 페이지에서 변환 픽셀을 구현합니다.
         1. 메인 메뉴에서 **[!UICONTROL Resources]** > **[!UICONTROL Conversion pixels]**(으)로 이동합니다.
         1. 픽셀 행에서 **[!UICONTROL edit]**&#x200B;을(를) 클릭합니다.
         1. 필요에 따라 [!UICONTROL HTML Tag] 및 [!UICONTROL Flash Tag] 필드의 값을 복사하여 광고주 또는 웹 사이트 연락처에 제공합니다.

            광고주의 IT 부서 또는 다른 그룹은 태그 배포를 예약하거나 그에 대한 정보를 받아야 할 수 있습니다.
   1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

**[!UICONTROL 3rd-party Fees]:** (선택 사항) 1000회 노출당 청구할 수 없는 비용으로 추적할 정적 타사 요금 비율입니다. 다른 값을 입력하지 않으면 새 배치에 패키지 수준 기본값이 자동으로 적용됩니다.

>[!NOTE]
>
>청구 가능 요금은 [!UICONTROL Net CPM] 지표에 반영됩니다.

>[!MORELIKETHIS]
>
>* [배치 관리 정보](placement-about.md)
>* [배치 만들기](placement-create.md)
>* [배치 편집](placement-edit.md)
>* [배치에 대한 입찰 승수 관리](placement-manage-bid-multipliers.md)
>* [배치에 대한 변경 로그 보기](placement-change-log.md)
>* [키보드 단축키](/help/dsp/campaign-management/reports/keyboard-shortcuts.md)
>* 캠페인 관리에 대한 [FAQ](/help/dsp/campaign-management/faq-campaign-management.md)
