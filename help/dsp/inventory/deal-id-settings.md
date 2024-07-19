---
title: 수동 거래 ID 설정
description: 수동으로 입력한 거래 ID에 대한 설정 설명을 참조하십시오.
feature: DSP Private Inventory, DSP Deal IDs
exl-id: 9d3417cb-8b44-4f1c-afc4-eea6a2e5b9d7
source-git-commit: badf6a1d7059b9e7e261165b19e00f09573b9e53
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# 수동 거래 ID 설정

| 섹션 | 매개 변수 | 설명 | 필수 | 편집 가능 |
|---------|-----------|-------------|----------|----------|
| [거래 세부 정보] | [!UICONTROL Deal name] | Advertising DSP에서 [!UICONTROL Deal ID]을(를) 식별하는 이름입니다. 이름을 입력하거나 **[!UICONTROL Auto-name]**&#x200B;을(를) 선택하여 DSP이 거래 세부 정보를 기반으로 이름을 생성하도록 합니다.<br><br>자동 생성된 이름의 예: `[!DNL 24159708 - Deal ID - Guaranteed Fixed - USD - 5 - 24Kitchen - Private]` | 예 | 예 |
| | [!UICONTROL External deal ID] | 이 거래를 식별하기 위해 게시자 및 SSP에서 사용하는 ID입니다. | 예 | 아니요 |
| | [!UICONTROL Publisher] | 이 재고를 판매하는 게시자의 이름입니다. | 예 | 아니요 |
| | [!UICONTROL SSP] | 이 거래가 실행되는 SSP(공급측 플랫폼)입니다. | 예 | 아니요 |
| | [!UICONTROL Media type] | 이 거래를 통해 구입한 미디어 유형: *[!UICONTROL Desktop video]*, *[!UICONTROL Mobile video]*, *[!UICONTROL Connected TV]*, *[!UICONTROL Display]*, *[!UICONTROL Audio]* 또는 *[!UICONTROL Publisher Managed]*. 옵션은 SSP마다 다릅니다.<br><br> 거래가 여러 미디어 유형을 허용하는 경우 거래를 만들 때 기본 배치에 대한 미디어 유형을 선택하십시오. 나중에 값을 변경하거나 [추가 미디어 유형으로 새 배치를 첨부](deal-id-attach-placements.md)하면 됩니다.<!-- It would be ideal if this field was multi-select rather than a radio button, so you don't have to "change" the value later. --> | 예 | 아니요 |
| | [!UICONTROL Deal type] | 거래 약정 및 가격 구조:<br><ul><li>*[!UICONTROL Non guaranteed (floor)]*: 귀하와 게시자가 고정된 노출 횟수 게재를 하지 않았습니다. 거래에는 재고에 대한 최소 가격이 명시되어 있지만, CPM은 시장 상황에 따라 변동하고 증가할 수 있습니다.</li><li>*[!UICONTROL Non guaranteed (fixed)]*: 귀하와 게시자가 고정된 노출 횟수 게재를 하지 않았습니다. 가격은 협상된 고정 비율로 책정됩니다.</li><li>*[!UICONTROL Guaranteed (fixed)]*: 귀하와 게시자가 미리 정의된 노출 횟수, 타기팅 횟수, 비행 날짜 및 고정 가격에 동의했습니다.<br><br><b>참고:</b> 보장된 거래에는 [!UICONTROL Tracking] 섹션에서 비행 날짜 및 지정된 노출 횟수가 필요합니다. 또한 거래에 대한 기본 프로그램 보증(PG) 배치를 만들어야 하며 선택적으로 다른 배치에 이 거래를 사용할 수 있습니다.</li></ul> | 예 | 아니요 |
| | [!UICONTROL CPM] | CPM(1000회 노출당 협상된 비용) | 예 | 예 |
| | [통화] | 거래의 통화입니다.<br><br>모든 SSP에서 USD로 거래를 수락합니다. SSP가 DSP 계정에 대한 통화를 수락하면 해당 통화도 사용할 수 있습니다. | 예 | 아니요 |
| | [!UICONTROL Billing method] | 모든 거래 ID는 [!DNL Adobe] 자금 조달 및 인보이스 발행 상태입니다. DSP은 사용량을 기준으로 사용 가능한 모든 미디어 공급업체에 비용을 지불하고 공급업체와의 불일치를 관리하며 하나의 통합 송장을 계정에 보냅니다. 이 옵션은 계정의 요금 카드에 설명된 대로 추가 요금을 발생시킵니다. | 예 | 아니요 |
| [!UICONTROL Advertisers] | [!UICONTROL Account email] | 거래에 액세스할 수 있는 사용자 계정의 이메일 주소입니다. | 아니요 | 예 |
| | [!UICONTROL Advertisers that can access this deal] | 이 거래에 액세스할 수 있는 계정의 특정 광고주.<br><br><b>참고:</b> [!UICONTROL Deals] 보기에서 추가 계정의 광고주와 거래를 공유할 수 있습니다. 거래 행에서 **[!UICONTROL #]**&#x200B;을(를) 클릭하고 **[!UICONTROL share]**&#x200B;을(를) 클릭한 다음 전자 메일 주소로 거래를 공유합니다. | 예 | 예 |
| [!UICONTROL Tracking] | [!UICONTROL Flight Dates] | 이 거래를 사용하는 트래픽의 시작 날짜와 종료 날짜입니다. 이러한 날짜는 추적 목적으로만 사용되며 광고 게재에는 영향을 주지 않습니다.<br><br><b>팁:</b> [!UICONTROL Inventory] > [!UICONTROL Deals] 보기에서 [!UICONTROL Pacing & Budget] 열은 거래가 지정된 플라이트 날짜 및 노출 목표에 어떻게 진행되고 있는지 보여 줍니다. 게재가 게재 간격 부족 또는 과대 게재 간격인 경우 게시자에게 문의하여 거래를 통해 보내는 볼륨을 조정하십시오. | 보장된 거래: 예<br>보장되지 않은 거래: 아니요 | 예 |
| | [!UICONTROL Impressions] | (보장되지 않는 거래의 경우 선택 사항) 이 거래를 사용하여 실행할 것으로 예상되는 예상 노출 횟수입니다. 이 값은 추적 목적으로만 사용되며 게시자는 광고 게재를 제어합니다. | 보장된 거래: 예<br>보장되지 않은 거래: 아니요 | 예 |

{style="table-layout:auto"}

>[!MORELIKETHIS]
>
>* [거래 ID 세부 정보 수동으로 만들기](deal-id-create.md)
>* [SSP 파트너](ssp-partners.md)
>* [개인 인벤토리 정보](private-inventory-about.md)
