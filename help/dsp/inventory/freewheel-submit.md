---
title: PG 거래에 대한 광고 제출 [!DNL FreeWheel]
description: 에서 게시자와 프로그래밍 방식으로 보장되는 거래에 대한 광고 승인을 요청하는 방법을 알아봅니다 [!DNL Freewheel].
feature: DSP Private Inventory, DSP Deal IDs
exl-id: 18d91f0c-4a27-4e40-b762-6c5e97e9a21a
source-git-commit: 14f78b89dea8cc680756232c6116975c652feee5
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 0%

---

# 프로그램 보증 거래에 대한 광고 제출 [!DNL Freewheel]

*이 있는 계정 [!DNL FreeWheel] 프로그램 보증 권한만*

한 번 [FreeWheel의 게시자와 프로그램 보증 거래 수락](#programmatic-guaranteed-set-up.md#pg-setup-deal-id-inbox), 광고 선택 및 거래에 사용할 프로그래밍 방식의 기본 배치 만들기가 포함된 경우 다음 위치에 광고를 제출해야 합니다. [!DNL Freewheel] 승인용.

>[!PREREQUISITES]
>
>Adobe 계정 팀과 협력하여 [!DNL DSP] 계정에는 다음 사용 권한이 있습니다. [!DNL FreeWheel] 프로그램 보증 워크플로우입니다.

1. 에 사용된 광고의 광고 키 복사 [!DNL Freewheel] 거래:

   1. 캠페인의 이름을 클릭합니다.

   1. 하위 메뉴에서 **[!UICONTROL Ads]**.

   1. 클릭  **[!UICONTROL ...]** > **[!UICONTROL Edit]** 광고 이름 옆에 있는 을 클릭합니다.

   1. 광고 설정이 열리면 브라우저의 주소 표시줄에 표시되는 URL의 영숫자 광고 키를 복사합니다.

      예를 들어 다음 URL에서 광고 키는 `3NtNC5ZbaGZtqbei8jD3`

      ```
      https://advertising.adobe.com/configurator/ad/3NtNC5ZbaGZtqbei8jD3?referrer=/playtime/ads
      ```

1. 다음 대상에게 광고 제출 [!DNL Freewheel]:

   1. 다음 중 하나를 수행합니다.

      * 광고 이름 옆에 있는 를 클릭합니다.  **[!UICONTROL ...]** > **[!UICONTROL submit to FreeWheel]**.

      * 메인 메뉴에서 **[!UICONTROL Inventory]** > **[!UICONTROL Deals]**. 거래 행에서 ![옵션 메뉴](/help/dsp/assets/options-menu.png) > **[!UICONTROL submit to FreeWheel]**.
   1. 거래 ID를 확인하고 **[!UICONTROL Ad Key]** 1단계에서 복사한 다음 **[!UICONTROL Submit]**.

   광고가 실행되기 전에 제출되고 승인되어야 합니다.

1. [광고 제출 상태 확인](freewheel-check-status.md).

>[!MORELIKETHIS]
>
>* [에서 프로그램 보증 거래 설정 개요 [!DNL Freewheel]](freewheel-overview.md)
>* [Deal ID Inbox에서 거래 수락](deal-id-inbox-accept.md)
>* [광고 상태 확인 [!DNL FreeWheel] 프로그램 보증 거래](freewheel-check-status.md)
>* [오류 코드 [!DNL Freewheel] 광고 제출](freewheel-error-codes.md)

