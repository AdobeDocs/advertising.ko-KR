---
title: ' [!DNL Roku] 인벤토리 사용'
description: 재고 옵션, 승인된 타사 추적 공급업체 및  [!DNL Roku]별 배치에 대한 모범 사례를 포함하여 DSP이  [!DNL Roku]과(와) 파트너 관계에 대해 알아봅니다.
feature: DSP On Demand Inventory, DSP Private Inventory
exl-id: e7a1aa80-d7f0-4a4e-96b1-6b362a32106e
source-git-commit: f3099c84fe2d6b1610ddf4ca07d59b119718afee
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---

# [!DNL Roku] 인벤토리 사용

Advertising DSP은 [!DNL Roku]에 광고를 위한 기능을 제공합니다.

## 대상 일치

[!DNL Roku] 및 DSP 파트너 관계는 [!DNL Roku] 인벤토리에서 1:1 결정론적 대상 타기팅을 위해 [!DNL DSP] 대상을 [!DNL Roku] ID에 일치시킵니다.

## [!DNL Roku] 인벤토리 옵션

a) [!DNL Roku](으)로 직접 비공개 거래 ID를 설정한 다음 거래 ID 데이터를 DSP에 입력하거나, b) [!DNL On Demand] 갤러리를 방문하여 [!DNL Roku] 프로필을 구독할 수 있습니다.

>[!NOTE]
>
>열려 있는 마켓플레이스 및 교환에서 [!DNL Roku] 인벤토리를 사용할 수 없습니다.

* 비공개 거래의 경우 [DSP에서 거래 ID에 대한 정보를 설정](/help/dsp/inventory/deal-id-create.md)한 다음 [!DNL Roku] 배치 내에서 &quot;[!UICONTROL Roku Network - Audience]&quot; 및 &quot;[!UICONTROL The Roku Channel - Audience]&quot;을(를) 타깃팅하세요.<!-- Or do you target the deal ID?? I see those strings for Roku On Demand inventory. Clarify if all Roku private deals show up as one or the other of these in Roku Private inventory in Roku placement settings. -->

* [다음 [!DNL Roku] 인벤토리를  [!DNL On Demand] 갤러리](/help/dsp/inventory/on-demand-inventory-subscribe.md) 내에서 구독하고 [!DNL Roku] 배치 내에서 승인된 거래를 타깃팅할 수 있습니다.

   * [!DNL The CW], [!DNL ABC] 및 [!DNL ESPN]과(와) 같은 프리미엄 콘텐츠 파트너와 [!DNL Roku] 에코시스템에서 인벤토리를 위한 &quot;[!UICONTROL Roku Network - Audience]&quot;.
   * [!DNL Roku]개의 소유 및 운영(O&amp;O) 앱 콘텐츠에 대한 &quot;[!UICONTROL The Roku Channel - Audience]&quot;.

### [!DNL Roku]을(를) 사용하여 개인 마켓플레이스 맞춤화의 이점

비공개 거래를 사용하면 필요에 따라 거래 매개변수를 사용자 정의할 수 있습니다.

* **협상된 가격:** [!DNL Roku] 영업 팀과 협력하여 캠페인 요구 사항에 맞는 거래를 협상하고 구성하십시오.

* **규모 우선 순위:** PMP(비공개 마켓플레이스)가 항상 적용되는 거래(예: [!DNL On Demand]개 거래)보다 우선 순위가 높습니다.

* **빈도 관리:** [!DNL Roku] 기본 빈도 상한은 사용자당 30분마다 1개의 광고이지만 시간, 일, 주, 월 또는 전체 비행 기간으로 상한을 사용자 지정할 수 있습니다.<!-- Within the DSP placement settings? NO - you negotiate this with Roku, but Christine to confirm with Amanda whether you should be able to edit this in placement. -->

* **[!DNL Roku]데이터 타깃팅:** [!DNL Roku] 대상은 [!DNL Roku] 장치 및 TV 신호, [!DNL The Roku Channel]에서 추적한 데이터(예: TV 장르 선호도, 스트리밍 TV 동작 및 케이블 구독 상태) 및 [!DNL Roku] CRM(고객 관계 관리) 시스템의 추가 데이터로 만들어집니다.

* 차단 목록에 추가하다 **[!DNL Roku]콘텐츠 타깃팅:** 비공개 거래는 장르, 앱 응용 프로그램, 시즌 및 텐트폴 이벤트별로 타깃팅할 수 있으며 [!DNL The Roku Channel] 내에서만 볼 수 있습니다.

## [!DNL Roku]개 배치

DSP 캠페인에서 배치 유형 &quot;[!UICONTROL Connected TV (Roku)]&quot;을(를) 사용하여 [특정 배치를 만들기 [!DNL Roku]합니다](/help/dsp/campaign-management/placements/placement-create.md). 정의된 목표를 가진 [!DNL Roku]별 패키지에 [!DNL Roku]개의 배치를 포함합니다.

각 [!DNL Roku] 배치는 하나 이상의 [!DNL Roku] 거래 또는 소스를 대상으로 해야 합니다. [!DNL Roku]과(와) 일치하는 DSP의 대상 세그먼트를 사용하려면 [!DNL Roku](옵트인) 결정적 데이터 세트에 대해 일치시킬 수 있는 대상 세그먼트를 하나 이상 포함하십시오.

### [!DNL Roku]이(가) 승인한 타사 추적 공급업체

[!DNL Roku] 배치에는 [!DNL Acxiom], [!DNL Comscore], [!DNL Data Plus Math], [!DNL Experian], [!DNL Factual], [!DNL Kantar], [!DNL Marketing Evolution], [!DNL Neustar], [!DNL Nielsen], [!DNL Nielsen Catalina Solutions], [!DNL NinthDecimal], [!DNL Oracle], [!DNL Placed], [!DNL Polk] 및 [!DNL Research Now] 공급업체의 전환 픽셀과 타사 이벤트 픽셀이 포함될 수 있습니다.

### 배치 전략별 우수 사례

다음은 [!DNL Roku]별 배치에 대한 권장 사례입니다.

증분 도달 범위를 최대화하려면

* [!DNL The Roku Channel]을(를) 사용하여 이미 도달한 대상을 제외하여 [!DNL Roku O&O]에서 노출된 대상을 제외합니다.

* [!DNL Roku] 플랫폼에서 이미 도달한 대상을 제외하여 [!DNL All Roku]에서 노출된 대상을 제외합니다.

가장 빠른 설정의 경우:

* [[!DNL On Demand] 인벤토리](/help/dsp/inventory/on-demand-inventory-subscribe.md)에서 [!DNL The Roku Channel]의 기존 상시 거래를 대상으로 하여 [!DNL Roku]개의 소유 및 운영 인벤토리에 빠르게 액세스할 수 있습니다.
* [[!DNL On Demand] 인벤토리](/help/dsp/inventory/on-demand-inventory-subscribe.md)에서 [!DNL Roku Network]에 대해 항상 유지되는 기존 거래를 대상으로 하여 [!DNL Roku] 플랫폼 전반에서 빠르게 확장할 수 있습니다.

최대 크기 조절:

* 협상된 가격으로 [!DNL Roku] 공급에 대한 우선 순위 액세스를 위해 [!DNL Roku] 개인 마켓플레이스를 사용자 지정합니다.

>[!MORELIKETHIS]
>
>* [거래 ID 세부 정보 수동으로 만들기](/help/dsp/inventory/deal-id-create.md)
> * [Premium 인벤토리 거래 구독 및 액세스 요청 [!DNL On Demand] 2}](/help/dsp/inventory/on-demand-inventory-subscribe.md)
>* [배치 만들기](/help/dsp/campaign-management/placements/placement-create.md)
