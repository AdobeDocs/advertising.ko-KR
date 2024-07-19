---
title: 프로그램 보증 거래 설정
description: 게시자와 협상한 프로그램 보증 거래(PG)를 설정하는 방법을 알아봅니다.
feature: DSP Private Inventory, DSP Deal IDs, DSP Programmatic Guaranteed Deals
exl-id: d962942f-c248-4b48-97bd-baa2df3a519e
source-git-commit: 4b9cc5956d573b346eacdf71a8ea490c162b4660
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 0%

---

# 프로그램 보증 거래 설정

*[지원되는 공급측 플랫폼만](programmatic-guaranteed-about.md)*

지원되는 게시자와 프로그램 보증(PG) 거래를 협상한 후 [!DNL Deal ID inbox]을(를) 사용하거나 거래 세부 정보를 수동으로 입력하여 DSP 내에서 거래를 설정할 수 있습니다.

>[!NOTE]
>
> PG 거래의 경우 게시자는 모든 예산 게재 간격, 예산 한도 및 타겟팅을 처리합니다. DSP을 통한 PG를 허용하는 모든 SSP는 게시자가 예산 상한을 설정할 수 있음을 확인합니다.
>
> [!DNL FreeWheel]에서 게시자와 프로그래밍 방식으로 보장되는 거래를 설정하려면 추가 권한과 단계가 필요합니다. 자세한 내용은 &quot;[프로그램 보증 거래 설정 개요 [!DNL FreeWheel]](freewheel-overview.md)&quot;를 참조하십시오.

## [!DNL Deal ID Inbox]을(를) 사용하여 프로그램 보증 거래 설정 {#pg-setup-deal-id-inbox}

다음 메서드는 [!DNL FreeWheel], [!DNL Google Authorized Buyers] 및 [!DNL Magnite DV+]의 기본 프로시저입니다.

1. [거래 수락](deal-id-inbox-accept.md).

1. 거래를 저장한 후 거래에 사용할 광고(또는 게시자 관리 광고의 1x1 추적 픽셀)를 선택하고 메시지가 표시되면 프로그램 보증 기본 배치(PG)를 만듭니다.

   구매의 100%를 게재하려면 거래에 대한 기본 PG 배치를 생성해야 합니다. 이 배치 유형에는 타깃팅이 없으므로 DSP은 게시자의 모든 입찰 요청에 입찰을 반환할 수 있습니다.

   * 단일 거래를 수락하는 경우 자동으로 PG 기본 배치 생성 워크플로우로 리디렉션됩니다.

     모든 [!DNL FreeWheel] 거래는 단일 거래로 제안됩니다.

   * 여러 PG 거래 ID가 있는 제안을 수락하는 경우 생성해야 하는 각 PG 기본 배치를 식별합니다. 필요한 배치를 모두 만들면 계속 버튼이 활성화됩니다.

1. (선택 사항) ![옵션 메뉴](/help/dsp/assets/options-menu.png) **>[!UICONTROL Attach new placement]**&#x200B;을(를) 클릭하여 추가 PG 또는 비 PG 배치에서 PG 거래를 타깃팅합니다.

   거래는 미디어 유형(예: 연결된 TV, 데스크탑 및 오디오)의 조합을 지원하는 여러 배치를 타깃팅할 수 있습니다.

## 수동으로 프로그램 보증 거래 설정

다른 모든 SSP에 이 방법을 사용하십시오.

1. [거래 ID 세부 정보를 수동으로 설정](deal-id-create.md).

1. 거래를 저장한 후 거래에 사용할 광고(또는 게시자 관리 광고의 경우 1x1 추적 픽셀)를 선택하고 메시지가 표시되면 PG 기본 배치를 만듭니다.

   구매의 100%를 게재하려면 거래에 대한 PG 기본 배치를 생성해야 합니다. 이 배치 유형에는 타깃팅이 없으므로 DSP은 게시자의 모든 입찰 요청에 입찰을 반환할 수 있습니다.

1. (선택 사항) ![옵션 메뉴](/help/dsp/assets/options-menu.png) **>[!UICONTROL Attach new placement]**&#x200B;을(를) 클릭하여 추가 PG 또는 비 PG 배치에서 PG 거래를 타깃팅합니다.

   거래는 미디어 유형(예: 연결된 TV, 데스크탑 및 오디오)의 조합을 지원하는 여러 배치를 타깃팅할 수 있습니다.

>[!MORELIKETHIS]
>
>* [프로그램 보증 거래 정보](programmatic-guaranteed-about.md)
>* [프로그램 보증 거래를 협상하기 위한 팁](/help/dsp/inventory/programmatic-guaranteed-tips.md)
>* [프로그램 보증 거래에 대한 광고 제출 [!DNL FreeWheel]](freewheel-submit.md)
>* [거래 ID 받은 편지함에서 거래 수락](deal-id-inbox-accept.md)
>* [거래 ID 세부 정보 수동으로 만들기](deal-id-create.md)
>* [SSP 파트너](ssp-partners.md)
>* [인벤토리 기능 개요](inventory-overview.md)
