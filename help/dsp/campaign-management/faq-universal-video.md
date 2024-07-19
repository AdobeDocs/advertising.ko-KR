---
title: 범용 비디오에 대한 FAQ
description: 범용 비디오 광고에 대해 자세히 알아보십시오.
feature: DSP Placements, DSP Ads
exl-id: 48c744ae-90a3-47e9-a5dc-c4e3c01b75a0
source-git-commit: 8d65069b7da5d3c33cc7713c6c80af27eb6bf227
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 0%

---

# 범용 비디오에 대한 FAQ

[범용 비디오 광고](/help/dsp/campaign-management/ads/ad-about.md#ad-types)를 사용하면 단일 비디오 배치를 사용하여 VPAID 및 VAST 인벤토리를 위해 데스크톱, 모바일 및 연결된 TV 환경에서 비디오 인벤토리를 타깃팅할 수 있습니다.

## 범용 비디오 배치 및 광고를 만들려면 어떻게 해야 합니까?

범용 비디오 배치에는 범용 비디오 광고만 포함될 수 있으며, 범용 비디오 광고는 범용 비디오 배치에만 첨부할 수 있습니다.

범용 비디오 배치 및 광고를 만드는 방법은 다른 유형의 배치 및 비디오를 만드는 방법과 유사합니다.

1. 원하는 캠페인 내에서 [범용 비디오 배치를 만듭니다](/help/dsp/campaign-management/placements/placement-create.md). [!UICONTROL Placement Type] **[!UICONTROL Universal Video]**&#x200B;을(를) 선택합니다.

   타깃팅할 환경(데스크톱, 모바일, 연결된 TV)을 하나 이상 지정해야 합니다.

1. 범용 비디오 배치와 동일한 캠페인에서 [하나의 범용 비디오 광고를 만들거나](/help/dsp/campaign-management/ads/ad-create.md) [여러 개의 범용 비디오 광고를 만듭니다](/help/dsp/campaign-management/ads/ad-create-multiple.md).

   여러 광고를 만드는 경우 &quot;[!UICONTROL Universal Video]&quot;을(를) [!UICONTROL Ad Type](으)로 지정하십시오.

   * [!DNL Google] 또는 [!DNL Flashtalking] 광고의 경우: 파일을 업로드한 후 &quot;[!UICONTROL Review ad types]&quot; 단계에서 **[!UICONTROL Ad Type]** 필드를 클릭하고 **[!UICONTROL Universal Video]**&#x200B;을(를) 선택합니다.

   * 기타 유형의 광고 태그: 업로드하는 스프레드시트 파일 내에서 각 광고의 광고 유형 필드를 **[!UICONTROL Universal Video]**(으)로 지정합니다.

1. 새 광고마다 [광고 설정을 열고](/help/dsp/campaign-management/ads/ad-edit.md) 해당하는 비디오 형식을 선택합니다.

   * **[!UICONTROL VPAID]:** 보기는 항상 측정됩니다.
   * **[!UICONTROL VPAID & VAST (Default)]:** 조회 측정을 허용하지 않는 인벤토리를 포함합니다.
   * **[!UICONTROL VAST]** - 연결된 TV 인벤토리에 적합합니다.

   자세한 내용은 &quot;[범용 비디오 광고 설정](/help/dsp/campaign-management/ads/ad-settings-universal-video.md)&quot;을 참조하십시오.

1. [범용 비디오 배치에 새 범용 비디오 광고를 첨부합니다](/help/dsp/campaign-management/ads/ad-attach-to-placement.md).

## 범용 비디오 배치를 위해 연결된 TV 환경을 선택한 경우 일부 최적화 목표와 패키지를 사용할 수 없는 이유는 무엇입니까?

[클릭당 최저 비용]과 같이 표준 연결된 TV 배치와 호환되지 않는 목표는 범용 비디오 배치의 연결된 TV 환경에서 지원되지 않습니다. 마찬가지로 최적화 목표가 호환되지 않는 패키지도 선택할 수 없습니다.

## 범용 비디오 광고에는 언제 **[!UICONTROL VAST]** 비디오 형식을 사용해야 합니까?

다음 시나리오 중 하나에서 **[!UICONTROL VAST]**&#x200B;을(를) 사용합니다.

* 배치 대상이 TV 인벤토리를 연결했습니다.
* 이 배치는 Google Ad Manager, Appnexus, SpotX 또는 Freewheel의 비디오 인벤토리를 타깃팅합니다. 이러한 SSP는 VPAID 및 VAST 비디오 형식을 지원하지 않습니다.

## 여러 범용 비디오 광고를 동일한 범용 비디오 배치에 첨부할 수 있습니까?

예.
