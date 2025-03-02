---
title: '[!UICONTROL Deal ID Inbox] 정보'
description: ' [!DNL FreeWheel], [!DNL Google Authorized Buyers] (이전 이름:  [!DNL AdX]), and [!DNL Magnite DV+] (이전 이름:  [!DNL Rubicon])에 게시자와 이미 협상한 비공개 거래를 수락할 수 있는 [!UICONTROL Deal ID inbox] 기능에 대해 알아봅니다.'
feature: DSP Private Inventory, DSP Deal IDs
exl-id: a1ba7de0-d6b4-4e22-8615-3e62d2ffdf5c
source-git-commit: 394a281c9b9d7eeab939f4c58508ec1f34eba67c
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# [!UICONTROL Deal ID Inbox] 정보

Advertising DSP [!UICONTROL Deal ID inbox]을(를) 사용하면 DSP이 SSP(공급측 플랫폼)를 통해 게시자로부터 가져온 거래를 빠르게 설정할 수 있으므로 각 거래를 수동으로 설정할 필요가 없습니다. [!UICONTROL Deal ID inbox]에서 [!DNL FreeWheel], [!DNL Google Authorized Buyers]&#x200B;(이전 [!DNL AdX]) 및 [!DNL Magnite DV+]&#x200B;(이전 [!DNL Rubicon])의 게시자와 이미 협상한 비공개 인벤토리 거래와 보장되지 않는 비공개 인벤토리 거래를 수락할 수 있습니다.

>[!NOTE]
>
>Advertising DSP은 [!DNL FreeWheel] API와 통합한 첫 번째 DSP입니다.

[!UICONTROL Deal ID inbox]에서 게시자에게 표시되는 거래의 세부 정보를 확인하고 거래 설정 속도를 높이고 수동 입력 오류를 방지할 수 있습니다.

<!-- 
Accepting a deal automatically pre-populates a new Deal ID record with details from the publisher, and you need to enter only the publisher [always? or just in some cases?], the media type, who can access the deal, and any attribute labels to apply to the deal so it's easy to find. [Are labels a dimension you can report on?]

For each available deal, you can review the deal details sent directly from the publisher. Some deals are grouped as proposals (packages), and you can see the individual deal details by reviewing the deal.

You can accept any available deal or move an incorrect deal to the Ignored Deals tab. You can also un-ignore deals, which moves them back to the New Deals tab so you can potentially accept them.

For each deal, you can select one publisher and one media type (Desktop Video, Mobile Video, Connected TV, Display, or Audio), and you can share the deal with specific advertisers and with all advertisers for a specific account.
 -->

DSP은 매일 오전 4:30(EST)에 모든 거래 세부 정보를 자동으로 새로 고칩니다. 또한 모든 [!DNL FreeWheel] 거래가 새로 고침되고 [!DNL Google] 및 [!DNL Magnite DV+]에서 시간별로 기존 거래가 업데이트됩니다. 거래 세부 사항을 수동으로 새로 고쳐 언제든지 새 거래를 채울 수도 있습니다.

<!-- MC: I'm not sure where I got the following. Is this currently true? -->

>[!NOTE]
>
>[!DNL Google Authorized Buyers]을(를) 통해 프로그램 방식으로 보장되는 거래의 경우 예산의 90% 이상을 제공해야 합니다. 그렇지 않으면 계정에서 [!UICONTROL Deal ID inbox]의 [!DNL Google] 거래에 액세스할 수 없습니다.

## [!UICONTROL Deal ID Inbox] 구현

[!UICONTROL Deal ID inbox]에서 거래를 받으려면 SSP 계정이 조직의 DSP 계정을 SSP 계정에 매핑해야 합니다. DSP은 관련 SSP와 조직의 계정 이름을 공유할 수 있습니다. 자세한 내용은 Adobe 계정 팀에 문의하십시오.

거래 협상 중에 게시자에게 거래를 상위 DSP 계정 대신 구매자에게 보내도록 지시합니다. 거래 식별자는 SSP에 따라 이름 또는 ID일 수 있다.

## 거래에 대해 수행할 수 있는 작업

* **거래 검토** SSP에서 올바른 게시자, 비행 날짜, CPM 및 기타 거래 세부 정보를 보냈는지 확인합니다. 게시자가 실수를 한 경우 DSP 외부에서 연락하여 거래를 수정하고 다시 보낼 수 있도록 합니다.

* 검토 후 **거래를 승인**&#x200B;하면 [!UICONTROL Deal ID inbox]에 더 이상 나타나지 않습니다. 수락된 거래는 [!UICONTROL Inventory] > [!UICONTROL Deals]에 나열되며 광고주의 배치 내에서 타깃팅할 준비가 되었습니다.

* 필요하지 않거나 원치 않는 거래는 **무시합니다**. 무시된 거래는 [!UICONTROL Deal ID inbox] 내의 [!UICONTROL Ignored Deals] 탭으로 이동되며 보관 역할을 합니다. DSP은 사용자가 거래를 무시할 때 SSP 및 게시자에게 알리지 않습니다.

* **이미 수락된 거래의 세부 정보를 수정**([!UICONTROL Inventory] > [!UICONTROL Deals]&#x200B;([!UICONTROL Deal ID inbox]에 없음). 마찬가지로, 게시자가 거래에 대한 변경 사항을 보낼 때 [!UICONTROL Deal ID inbox]이(가) 거래가 설정된 후 SSP의 변경 사항을 동기화하지 않으므로 광고주가 [!UICONTROL Inventory] > [!UICONTROL Deals]에서 해당 변경 사항을 구현해야 합니다.

## 어떤 종류의 거래를 수락할 수 없습니까?

거래 목록에 ![승인](/help/dsp/assets/accept.png) 아이콘 또는 [!UICONTROL Accept] 단추가 없으면 [!UICONTROL Deal ID inbox]에서 승인할 수 없습니다. 대신 [거래 ID 세부 정보를 수동으로 만들 수 있습니다](/help/dsp/inventory/deal-id-create.md).

다음 유형의 거래는 수락할 수 없습니다.

* USD가 아닌 거래 [!DNL Google]개.

* USD가 아닌 거래 [!DNL Magnite DV+]개

* [!DNL FreeWheel] 거래에서 계정 통화로 표시되지 않습니다.

* 오늘 이전에 종료 일자가 있는 거래입니다.

* 여러 미디어 유형으로 레이블이 지정된 이전 [!DNL Magnite DV+] 거래입니다.

거래 세부 사항에는 해당 거래를 수락할 수 없는 이유가 포함됩니다.

>[!MORELIKETHIS]
>
>* [거래 ID 받은 편지함에서 거래 수락](deal-id-inbox-accept.md)
>* [인벤토리 기능 개요](inventory-overview.md)
