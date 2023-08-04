---
title: 프로그램 보증 거래 정보
description: 프로그램 보증 거래(PG) 및 이를 제공하는 인증 SSP에 대해 알아봅니다.
feature: DSP Private Inventory, DSP Deal IDs, DSP Programmatic Guaranteed Deals
exl-id: 47c89d8a-f45f-4fcb-84a6-031f7d7f580f
source-git-commit: 700a38baba3e9abc871e23e95faba6715d661eb9
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 0%

---

# 프로그램 보증 거래 정보

프로그램 보증 거래(PG)는 광고 서버 태그가 아닌 거래 ID를 통해 게시자와 직접 체결할 수 있는 보증된 구매입니다. PG는 사용자와 게시자가 보다 유연하게 관리할 수 있으며, 일반 태그 구입보다 더 투명합니다. 청구 및 보고는 DSP을 통해 통합되므로 시간을 절약할 수 있습니다.

## PG 거래의 특징

* 거래는 항상 DSP을 통해 청구됩니다.
* 그 거래에는 정가와 수량이 있다.
* 게시자 또는 SSP(공급측 플랫폼)는 모든 예산 게재 간격, 예산 한도 및 모든 타겟팅을 처리합니다.
* 일반적으로 이 거래는 게시자의 광고 서버에서 우선 순위가 높습니다.
* 입찰 요청은 단일 거래나 구매자에게만 국한되지 않습니다.
* 단일 거래 ID에서 여러 유형의 비디오가 지원됩니다.
* 게시자가 관리하는 광고는 Google Authorized Bureers SSP를 통해 수락됩니다.
* SSP 및 게시자에게는 배달 SLA가 있습니다.

DSP이 각 입찰 요청에 대한 요청을 반환하고 SSP로 배달 SLA를 이행할 수 있도록 PG 거래에는 PG 기본 배치 및 광고(또는 게시자 관리 광고의 경우 1x1 픽셀)가 필요합니다. 필수 PG 기본 배치를 설정하면 다른 배치에서 PG 거래를 타깃팅할 수도 있습니다.

## DSP의 PG 거래에 대해 인증된 SSP

* [!DNL Ambient Digital]
* [!DNL FreeWheel]
* [!DNL Google Authorized Buyers]
* [!DNL Magnite CTV] (이전 [!DNL Telaria])
* [!DNL Magnite DV+] (이전 [!DNL Rubicon])
* [!DNL OpenX]
* [!DNL SpotX]

>[!MORELIKETHIS]
>
>* [프로그램 보증 거래 협상을 위한 팁](/help/dsp/inventory/programmatic-guaranteed-tips.md)
>* [프로그램 보증 거래 설정](programmatic-guaranteed-set-up.md)
>* [SSP 파트너](ssp-partners.md)
>* [재고 기능 개요](inventory-overview.md)
