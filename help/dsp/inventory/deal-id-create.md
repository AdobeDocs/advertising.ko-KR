---
title: 거래 ID 세부 정보 수동으로 만들기
description: 거래 ID에 대한 세부 사항을 수동으로 입력하는 방법을 알아봅니다.
feature: DSP Private Inventory, DSP Deal IDs
exl-id: 20a57919-c68f-4c9d-a8e1-f49484f74655
source-git-commit: 4b9cc5956d573b346eacdf71a8ea490c162b4660
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# 거래 ID 세부 정보 수동으로 만들기

1. 메인 메뉴에서 **[!UICONTROL Inventory]** > **[!UICONTROL Deals].**

1. 데이터 테이블 위에서 **[!UICONTROL Create]**&#x200B;을 선택한 다음 을 선택합니다 **[!UICONTROL Deal ID]**.

1. 다음을 입력합니다. [거래 설정](deal-id-settings.md):

   1. 다음에서 [!UICONTROL Deal ID basics] 섹션에서 거래 세부 정보 및 거래에 액세스할 수 있는 광고주를 지정합니다. 보장된 거래의 경우, 추적 목적으로만 계획된 비행 날짜와 예상 노출 횟수를 지정해야 합니다.

      인벤토리 > 거래 보기에서 &quot;PG 노출 게재 간격&quot; 지출 열을 포함하여 보장된 거래의 게재 간격을 추적할 수 있습니다.

   1. (관리자 사용자만 해당, 선택 사항) [!UICONTROL Technical] 섹션에서 필요에 따라 기본 설정을 편집합니다.

   1. 클릭 **[!UICONTROL Save]**.

1. (보장된 거래만 해당) 거래에 사용할 광고(또는 게시자 관리 광고의 1x1 픽셀)를 선택하고 기본 프로그램 보증(PG) 배치를 만듭니다.

   기본 PG 배치를 사용하면 거래가 항상 각 입찰 요청에 대한 입찰을 반환하도록 할 수 있습니다. 기본 PG 배치를 만들지 않으면 거래를 타깃팅하는 배치는 올바르게 설정되지 않은 경우 입찰을 배치하지 않습니다. 항상 기본 PG 배치를 생성해야 합니다. 다음에서 [!UICONTROL Placements] 보기, 기본 PG 배치에는 [!UICONTROL Sub-type] 열 값 &quot;[!UICONTROL PG Default].&quot;

   선택적으로 추가 배치에서 거래를 재고 대상으로 사용할 수 있지만 입찰을 배치하도록 올바로 설정해야 합니다.

   1. 다음에서 [!UICONTROL Ad & Campaign Selection] 설정에서 거래에 사용할 광고를 선택합니다.

      1. 광고주, 캠페인 및 광고 유형을 선택합니다. 선택적으로 광고를 필터링할 광고 상태를 선택합니다.

      1. 사용 가능한 광고 목록에서 거래에 사용할 각 광고 옆에 있는 확인란을 선택합니다.

         각 게시자가 관리하는 광고에 대해 광고주와 캠페인을 선택한 후 1x1 추적 픽셀이 자동으로 적용됩니다.

      1. 클릭 **[!UICONTROL Apply]**.

   1. 배치 설정 화면에서

      1. 배치 이름을 입력합니다.

      1. (선택 사항) [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)( 거래의 CPM 값으로 자동으로 채워지는 기본 입찰의 덮어쓰기, 날짜 범위 변경 또는 더 많은 광고 첨부 포함).

      이 거래는 재고 목표 섹션에서 자동으로 타깃팅됩니다. 다른 모든 타깃팅 옵션은 적용할 수 없습니다.

      1. 클릭 **[!UICONTROL Create placement]**.

거래를 생성한 후에는 해당 거래를 여러 배치에 대한 재고 대상으로 사용할 수 있습니다.

>[!NOTE]
>
> 확인을 위해 거래 태그를 게시자에게 보내지 않아도 됩니다.

>[!TIP]
>
>* 다음에서 [!UICONTROL Inventory] > [!UICONTROL Deals] 보기, [!UICONTROL Pacing & Budget] 열은 거래가 지정된 플라이트 날짜 및 노출 목표에 어떻게 진행되고 있는지 보여줍니다.
>
>* 게재가 게재 간격 부족 또는 과대 게재 간격인 경우 게시자에게 문의하여 거래를 통해 보내는 볼륨을 조정하십시오.

>[!MORELIKETHIS]
>
>* [수동 거래 ID 설정](deal-id-settings.md)
>* [프로그램 보증 거래 설정](programmatic-guaranteed-set-up.md)
>* [프로그램 보증 거래의 경우 광고 제출 [!DNL FreeWheel]](freewheel-submit.md)
>* [프로그램 보증 거래 정보](programmatic-guaranteed-about.md)
<!-- >* [Specify Placements and Ads for a Private Deal](deal-id-attach-placements.md)-->
