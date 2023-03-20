---
title: 범용 비디오에 대한 FAQ
description: 범용 비디오 광고에 대해 자세히 알아보십시오.
feature: DSP Placements, DSP Ads
source-git-commit: 58cbb5b85a1dc790aaf762ba55fd2badeef6fe68
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 0%

---

# 범용 비디오에 대한 FAQ

## 범용 비디오 배치 및 광고를 만들려면 어떻게 합니까?

범용 비디오 배치에는 범용 비디오 광고만 포함할 수 있고 범용 비디오 광고는 범용 비디오 배치에만 연결할 수 있습니다.

다른 유형의 배치 및 비디오를 만드는 방법과 유사하게 만듭니다.

1. 원하는 캠페인 내에서, [범용 비디오 배치 만들기](/help/dsp/campaign-management/placements/placement-create.md), 선택 [!UICONTROL Placement Type] **[!UICONTROL Universal Video]**.

   타겟팅할 환경(데스크톱, 모바일, 연결된 TV)을 하나 이상 지정해야 합니다.

1. 범용 비디오 배치와 동일한 캠페인에서 [단일 범용 비디오 광고 만들기](/help/dsp/campaign-management/ads/ad-create.md) 또는 [여러 범용 비디오 광고 만들기](/help/dsp/campaign-management/ads/ad-create-multiple.md).

   여러 광고를 만드는 경우 &quot;[!UICONTROL Universal Video]&quot; [!UICONTROL Ad Type]:

   * 대상 [!DNL Google] 또는 [!DNL Flashtalking] 광고: 에서[!UICONTROL Review ad types]&quot; 파일을 업로드한 후 **[!UICONTROL Ad Type]** 필드 및 선택 **[!UICONTROL Universal Video]**.

   * 다른 유형의 광고 태그의 경우: 업로드하는 스프레드시트 파일 내에서 각 광고에 대한 광고 유형 필드를 다음으로 지정합니다 **[!UICONTROL Universal Video]**.

1. [광고 설정을 엽니다](/help/dsp/campaign-management/ads/ad-edit.md) 새로운 각 광고에 대해 적용 가능한 비디오 형식을 선택합니다.

   * **[!UICONTROL VPAID]:** 뷰가능 여부는 항상 측정됩니다.
   * **[!UICONTROL VPAID & VAST (Default)]:** 뷰가능 측정을 허용하지 않는 인벤토리를 포함합니다.
   * **[!UICONTROL VAST]** - 연결된 TV 인벤토리에 적합합니다.

   참조:[범용 비디오 광고 설정](/help/dsp/campaign-management/ads/ad-settings-universal-video.md)&quot;&quot;을 참조하십시오.

1. [새로운 범용 비디오 광고 첨부](/help/dsp/campaign-management/ads/ad-attach-to-placement.md) 범용 비디오 배치로 이동합니다.

## 범용 비디오 배치를 위해 연결된 TV 환경을 선택한 경우 일부 최적화 목표 및 패키지를 사용할 수 없는 이유는 무엇입니까?

가장 낮은 클릭당 비용과 같이 표준 연결된 TV 배치와 호환되지 않는 목표는 범용 비디오 배치에서 연결된 TV 환경에 대해 지원되지 않습니다. 마찬가지로 호환되지 않는 최적화 목표가 있는 패키지도 선택할 수 없습니다.

## 언제 **[!UICONTROL VAST]** 비디오 형식이 범용 비디오 광고에 사용됩니까?

사용 **[!UICONTROL VAST]** 다음 시나리오 중 하나에서 다음을 수행합니다.

* 배치 타겟은 연결된 TV 인벤토리를 포함합니다.
* 배치는 Google Ad Manager, Appnexus, SpotX 또는 Freewheel의 비디오 인벤토리를 타겟으로 합니다. 이러한 SSP는 VPAID 및 VAST 비디오 형식을 지원하지 않습니다.

## 여러 범용 비디오 광고를 동일한 범용 비디오 배치에 첨부할 수 있습니까?

예.
