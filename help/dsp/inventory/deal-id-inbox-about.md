---
title: 정보 [!UICONTROL Deal ID Inbox]
description: '에 대해 알아보기 [!UICONTROL Deal ID inbox] 이미 게시자와 협상한 비공개 거래를 수락할 수 있는 기능입니다. [!DNL FreeWheel], [!DNL Google Authorized Buyers] (이전 이름: [!DNL AdX]), and [!DNL Magnite DV+] (이전 [!DNL Rubicon]).'
feature: DSP Private Inventory, DSP Deal IDs
exl-id: a1ba7de0-d6b4-4e22-8615-3e62d2ffdf5c
source-git-commit: 14f78b89dea8cc680756232c6116975c652feee5
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# 정보 [!UICONTROL Deal ID Inbox]

Advertising DSP [!UICONTROL Deal ID inbox] 에서는 DSP이 SSP(공급측 플랫폼)를 통해 게시자로부터 가져온 거래를 신속하게 설정할 수 있으므로 각 거래를 수동으로 설정할 필요가 없습니다. 이미 게시자와 협상한 보장된 비공개 인벤토리 거래와 보장되지 않은 비공개 인벤토리 거래를 수락할 수 있습니다 [!DNL FreeWheel], [!DNL Google Authorized Buyers] (이전 이름: [!DNL AdX]), 및 [!DNL Magnite DV+] (이전 [!DNL Rubicon]의 ) [!UICONTROL Deal ID inbox].

>[!NOTE]
>
>Advertising DSP은 와 통합한 첫 번째 DSP입니다. [!DNL FreeWheel] API.

다음에서 [!UICONTROL Deal ID inbox]에서는 게시자가 거래 세부 정보를 볼 때 거래의 세부 정보를 볼 수 있고 거래 설정 속도를 높이고 수동 입력 오류를 방지할 수 있습니다.

<!-- 
Accepting a deal automatically pre-populates a new Deal ID record with details from the publisher, and you need to enter only the publisher [always? or just in some cases?], the media type, who can access the deal, and any attribute labels to apply to the deal so it's easy to find. [Are labels a dimension you can report on?]

For each available deal, you can review the deal details sent directly from the publisher. Some deals are grouped as proposals (packages), and you can see the individual deal details by reviewing the deal.

You can accept any available deal or move an incorrect deal to the Ignored Deals tab. You can also un-ignore deals, which moves them back to the New Deals tab so you can potentially accept them.

For each deal, you can select one publisher and one media type (Desktop Video, Mobile Video, Connected TV, Display, or Audio), and you can share the deal with specific advertisers and with all advertisers for a specific account.
 -->

DSP은 매일 오전 4:30(EST)에 모든 거래 세부 정보를 자동으로 새로 고칩니다. 또한 모든 항목이 새로 고쳐집니다 [!DNL FreeWheel] 에서 기존 거래 및 업데이트 [!DNL Google] 및 [!DNL Magnite DV+] 시간별. 거래 세부 사항을 수동으로 새로 고쳐 언제든지 새 거래를 채울 수도 있습니다.

<!-- MC: I'm not sure where I got the following. Is this currently true? -->
>[!NOTE]
>
>을 통한 프로그램 보증 거래 [!DNL Google Authorized Buyers], 예산의 90% 이상을 전달해야 합니다. 그렇지 않으면 계정에 대한 액세스 권한이 상실됩니다. [!DNL Google] 거래 [!UICONTROL Deal ID inbox].

## 구현 [!UICONTROL Deal ID Inbox]

을(를) 통해 거래를 받으려면 [!UICONTROL Deal ID inbox]: SSP 계정은 조직의 DSP 계정을 SSP 계정에 매핑해야 합니다. DSP은 관련 SSP와 조직의 계정 이름을 공유합니다. 자세한 내용은 Adobe 계정 팀에 문의하십시오.

거래 협상 중에 게시자에게 거래를 상위 DSP 계정 대신 구매자에게 보내도록 지시합니다. 거래 식별자는 SSP에 따라 이름 또는 ID일 수 있다.

## 거래에 대해 수행할 수 있는 작업

* **거래 검토** ssp에서 올바른 게시자, 비행 날짜, CPM 및 기타 거래 세부 사항을 보냈는지 확인합니다. 게시자가 실수를 한 경우 DSP 외부에서 연락하여 거래를 수정하고 다시 보낼 수 있도록 합니다.

* **거래 수락** 검토 후 에는 더 이상 표시되지 않습니다 [!UICONTROL Deal ID inbox]. 수락된 거래는에 나열됩니다. [!UICONTROL Inventory] > [!UICONTROL Deals] 광고주의 배치 내에서 타깃팅할 준비가 되었습니다.

* **거래 무시** 필요하지 않거나 원치 않는 것입니다. 무시된 거래는 다음으로 이동됨 [!UICONTROL Ignored Deals] 내의 탭 [!UICONTROL Deal ID inbox]- 아카이브 역할을 합니다. DSP은 사용자가 거래를 무시할 때 SSP 및 게시자에게 알리지 않습니다.

* **이미 수락된 거래의 세부 정보 수정** 출처: [!UICONTROL Inventory] > [!UICONTROL Deals] (다음에 없음) [!UICONTROL Deal ID inbox]). 마찬가지로 게시자가 거래에 변경 사항을 보낼 때에서 광고주가 해당 변경 사항을 구현할 책임이 있습니다. [!UICONTROL Inventory] > [!UICONTROL Deals] 이유: [!UICONTROL Deal ID inbox] 은 거래가 설정된 후 SSP의 변경 사항을 동기화하지 않습니다.

## 어떤 종류의 거래를 수락할 수 없습니까?

거래 목록에 이 포함되지 않은 경우 ![Accept](/help/dsp/assets/accept.png) 아이콘 또는 [!UICONTROL Accept] 단추이므로 다음에서 수락할 수 없습니다. [!UICONTROL Deal ID inbox]. 대신 [거래 ID 세부 사항 수동으로 만들기](/help/dsp/inventory/deal-id-create.md).

다음 유형의 거래는 수락할 수 없습니다.

* [!DNL Google] USD가 아닌 거래.

* [!DNL Magnite DV+] USD가 아닌 거래

* [!DNL FreeWheel] 계정 통화로 되어 있지 않은 거래.

* 오늘 이전에 종료 일자가 있는 거래입니다.

* 이전 [!DNL Magnite DV+] &quot;여러 미디어 유형&quot;으로 레이블이 지정된 거래.

거래 세부 사항에는 해당 거래를 수락할 수 없는 이유가 포함됩니다.

>[!MORELIKETHIS]
>
>* [Deal ID Inbox에서 거래 수락](deal-id-inbox-accept.md)
>* [재고 기능 개요](inventory-overview.md)

