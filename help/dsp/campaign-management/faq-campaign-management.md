---
title: Campaign Management에 대한 FAQ
description: 변경 사항에 대한 지연 기간 및 비행 중 예산을 변경할 때 발생하는 상황 등 캠페인 관리에 대해 자세히 알아보십시오.
feature: DSP Packages, DSP Placements
exl-id: 8a443543-ebb1-4273-a007-afef07d32d8c
source-git-commit: e517dd5f5fa283ff8a2f57728612937148889732
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# Campaign Management에 대한 FAQ

<!-- Most of this information should be moved into the relevant topics (especially editing topics). -->

## 설정 변경 지연

* 배치나 패키지 설정을 변경할 때 변경 사항은 언제 적용됩니까?

  설정 변경 사항은 일반적으로 즉시 적용되지만 최대 12시간이 소요될 수 있습니다.

  배송 마지막 날인 경우 당일 일찍 변경 작업을 수행하여 DSP에서 변경 사항을 기반으로 패키지를 재수정할 시간이 충분합니다. 예를 들어 짝수 게재 간격 방식에서 프론트로드 게재 간격 방식으로 변경하는 경우 DSP은 나머지 비행 시간 동안 지출을 배분하는 방법을 재평가해야 합니다. 비행 마지막 날에 배달할 시간이 1시간밖에 남지 않았다면 그런 변화는 하지 마세요.

## 비행 중 예산 업데이트

* 배치를 변경하면 DSP에서 패키지 예산을 재할당하는 데 얼마나 걸립니까?

  예산 할당은 배치 성과를 기준으로 하며, 이 점수는 14일 평균을 사용하여 평가됩니다. 배치를 변경하면 14일 평균 동안 성능이 변경되는 경우에만 예산 할당이 변경됩니다.

  성능 변경이 발생하면 DSP은 그에 따라 다음 예산 최적화 주기 동안 배치 간에 패키지 예산을 재할당합니다. 이 최적화는 캠페인 시간대의 자정(00:00)에 발생합니다.

* 배치가 패키지에서 제거되고 다른 패키지에 추가될 때 예산은 어떻게 재할당됩니까?

  배치의 전체 지출 내역이 배치에 첨부되고 패키지에서 패키지로 이동합니다.

  패키지에서 배치를 제거하면 패키지에 더 이상 배치 지출 내역이 없습니다. 패키지 예산은 (패키지 예산 - 제거된 배치 예산) / 남은 비행 시간 간격이 됩니다. 그런 다음 패키지 예산이 패키지에 남아 있는 배치에 할당됩니다.

  마찬가지로 동일한 배치를 다른 패키지에 추가하는 경우 DSP은 새 패키지의 모든 배치에 대한 예산을 할당할 때 배치의 지출 내역을 고려합니다.

* 패키지 게재 간격 변경 비행 마지막 날

  비행기 마지막 날에는 패키지 예산이 초과되지 않도록 하루 24시간에서 23시간으로 단축된다. 또한 패키지의 게재 간격 채우기 전략은 자동으로 &quot;&quot;로 변경됩니다[!UICONTROL Frontload],&quot;로 설정되어 있더라도[!UICONTROL even].&quot; 즉, 일일 예산의 65%가 EST 오전 11:30까지 전달되어야 합니다.

>[!MORELIKETHIS]
>
>* [패키지 설정](/help/dsp/campaign-management/packages/package-settings.md)
>* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)
>* [성과 캠페인 설정에 대한 우수 사례](/help/dsp/optimization/campaign-best-practices-performance.md)
