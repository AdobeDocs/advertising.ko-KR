---
title: 배치 수준 사전 입찰 필터 및 사용 방법
description: 사용 가능한 배치 수준의 사전 입찰 필터를 참조하고 사용 방법을 확인하십시오.
feature: DSP Optimization
exl-id: 34a15666-7ca2-416d-9064-8638ca81e5b3
source-git-commit: e517dd5f5fa283ff8a2f57728612937148889732
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 0%

---

# 배치 수준 사전 입찰 필터 및 사용 방법

| 사전 입찰 필터 | 설명 | 이 필터 사용 시기 |
| ---------------| ----------- | ---------------------- |
| [!UICONTROL Click Through Rate] | 경매로 인해 클릭스루가 발생할 가능성에 대한 최소 예측 임계값을 설정합니다. 예를 들어 임계값을 0.1%로 설정하면 예측된 클릭 확률이 0.1%보다 크거나 같은 경우에만 경매에 입찰합니다.<br><br><b>참고:</b> 최적화 목표 전에 필터가 적용됩니다. 그 결과, 매우 엄격한 필터가 소비를 방지할 수 있습니다. | CTR(클릭스루 비율)에 대한 최소 KPI 목표가 있고 CTR이 임계값 이하일 때 예산을 지출하지 않으려는 경우 사용합니다. 이 필터는 상당히 제한적일 수 있으므로 현실적인 목표를 설정하는 것이 중요합니다. 배치에 대한 다른 제약에 따라, 일반적으로 0.03-.07%라는 목표는 좋은 시작점이다. 필요한 경우 사이트 수준에서 이를 최적화하여 지표를 개선할 수 있습니다.<br><br>최소 CTR과 최상의 CPM을 달성하는 것이 목표라면 [!UICONTROL Click Through Rate] 필터를 최적화 목표 &quot;[!UICONTROL Lowest CPM]&quot;과(와) 결합하는 것이 좋습니다. 목표가 초과 달성에 대한 실제 이점이 없는 최대 CPM이고 최소 CTR인 경우 [!UICONTROL Click Through Rate] 필터를 최적화 목표 &quot;[!UICONTROL Always Max Bid + Highest CTR]&quot;과(와) 연결하는 것이 더 적절할 수 있습니다. |
| [!UICONTROL 100% Completion Rate] | 노출에 입찰하기 전에 충족해야 하는 필수 최소 완료율을 설정합니다. | 캠페인의 주요 목표가 완료율일 때 이 필터를 사용합니다. 다른 타깃팅 매개 변수를 고려하지만 65%가 권장 시작 백분율입니다. |
| [!UICONTROL Player Size - Adobe] | DSP의 데이터를 사용하여 필요한 최소 플레이어 크기를 설정합니다. [!UICONTROL Player Size] 임계값이 충족되면 노출에 입찰할 수 있습니다. | DSP의 데이터를 사용하여 전체 에피소드 플레이어 인벤토리를 제공하고 있는지 확인하는 데 사용합니다. |
| [!UICONTROL Player Size 3rdParty (Moat/IAS)] | [!DNL Moat] 또는 [!DNL Integral Ad Science]([!DNL IAS])의 데이터를 사용하여 필요한 최소 플레이어 크기를 설정합니다. [!UICONTROL Player Size] 임계값이 충족되면 노출에 입찰할 수 있습니다. | 플랫폼 전체 [!DNL Moat] 또는 [!DNL IAS] 데이터를 사용하여 전체 에피소드 플레이어 인벤토리를 제공하는 데 사용합니다.<br><br><b>참고:</b> 캠페인이 [!DNL Moat] 또는 [!DNL IAS] 데이터를 사용하도록 구성된 경우에만 이 필터를 사용하십시오. |
| [!UICONTROL Viewability Adobe (MRC or [!DNL GroupM])] | DSP 조회 수 및 측정값을 사용하여 필요한 최소 조회 비율을 설정합니다. 지정된 임계값이 충족되면 노출에 입찰할 수 있습니다.<br><br><b>메모:</b><ul><li>캠페인의 [!UICONTROL Viewability Sensitivity] 설정이 &quot;[!UICONTROL Standard (50% of ad in view for 2 consecutive seconds)]&quot;이면 [!DNL Media Rating Council](MRC) 조회 측정 표준이 캠페인에 사용됩니다. [!UICONTROL Viewability Sensitivity] 설정이 &quot;[!UICONTROL Strict (100% of ad in view & audio on for 50% duration)]&quot;인 경우 [!DNL GroupM] 조회 측정 표준이 캠페인에 사용됩니다.</li><li>Adobe 측정 정의는 서드파티 정의와 다르므로 서드파티 데이터와 약간 일치하지 않을 수 있습니다.</li></ul> | 가장 좋은 방법은 최적화 목표와 사전 입찰 필터 설정을 캠페인의 [!UICONTROL Viewability Sensitivity] 설정과 일치시키는 것입니다. |

{style="table-layout:auto"}

>[!MORELIKETHIS]
>
>* [DSP이 캠페인을 최적화하는 방법](optimization-how-dsp-optimizes-campaigns.md)
>* [패키지 설정](/help/dsp/campaign-management/packages/package-settings.md)
>* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)
>* [캠페인 설정](/help/dsp/campaign-management/campaigns/campaign-settings.md)
>* [최적화 목표 및 사용 방법](optimization-goals.md)
