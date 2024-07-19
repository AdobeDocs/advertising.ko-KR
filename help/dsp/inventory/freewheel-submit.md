---
title: ' [!DNL FreeWheel]에게 PG 거래에 대한 광고 제출'
description: ' [!DNL Freewheel]의 게시자와 프로그래밍 방식으로 보장되는 거래에 대한 광고 승인을 요청하는 방법에 대해 알아봅니다.'
feature: DSP Private Inventory, DSP Deal IDs
exl-id: 18d91f0c-4a27-4e40-b762-6c5e97e9a21a
source-git-commit: 14f78b89dea8cc680756232c6116975c652feee5
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 0%

---

# 프로그램 보증 거래에 대한 광고를 [!DNL Freewheel]에 제출

*프로그래밍 방식으로 보장된 [!DNL FreeWheel] 권한이 있는 계정*

[FreeWheel](#programmatic-guaranteed-set-up.md#pg-setup-deal-id-inbox)에서 게시자와 함께 프로그램 방식으로 보장되는 거래를 수락하려면 광고를 선택하고 거래에 사용할 프로그램 방식으로 보장되는 기본 배치를 만들어야 합니다. 승인을 위해 광고를 [!DNL Freewheel]에 제출해야 합니다.

>[!PREREQUISITES]
>
>Adobe 계정 팀과 함께 [!DNL DSP] 계정에 [!DNL FreeWheel] 프로그래밍 방식으로 보장된 워크플로를 사용할 수 있는 권한이 있는지 확인하십시오.

1. [!DNL Freewheel] 거래에 사용된 광고의 광고 키를 복사합니다.

   1. 캠페인의 이름을 클릭합니다.

   1. 하위 메뉴에서 **[!UICONTROL Ads]**&#x200B;을(를) 클릭합니다.

   1. 광고 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

   1. 광고 설정이 열리면 브라우저의 주소 표시줄에 표시되는 URL의 영숫자 광고 키를 복사합니다.

      예를 들어 다음 URL에서 광고 키는 `3NtNC5ZbaGZtqbei8jD3`입니다

      ```
      https://advertising.adobe.com/configurator/ad/3NtNC5ZbaGZtqbei8jD3?referrer=/playtime/ads
      ```

1. [!DNL Freewheel]에 광고 제출:

   1. 다음 중 하나를 수행합니다.

      * 광고 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL submit to FreeWheel]**&#x200B;을(를) 클릭합니다.

      * 메인 메뉴에서 **[!UICONTROL Inventory]** > **[!UICONTROL Deals]**&#x200B;을(를) 클릭합니다. 거래 행에서 ![옵션 메뉴](/help/dsp/assets/options-menu.png) > **[!UICONTROL submit to FreeWheel]**&#x200B;을(를) 클릭합니다.

   1. 거래 ID를 확인하고 1단계에서 복사한 **[!UICONTROL Ad Key]**&#x200B;을(를) 입력한 다음 **[!UICONTROL Submit]**&#x200B;을(를) 클릭합니다.

   광고가 실행되기 전에 제출되고 승인되어야 합니다.

1. [광고 제출 상태를 확인](freewheel-check-status.md).

>[!MORELIKETHIS]
>
>* [프로그램 보증 거래 설정 개요 [!DNL Freewheel]](freewheel-overview.md)
>* [거래 ID 받은 편지함에서 거래 수락](deal-id-inbox-accept.md)
>* [광고 상태 확인 [!DNL FreeWheel] 프로그램 보증 거래](freewheel-check-status.md)
>* [광고 제출을 위한 오류 코드 [!DNL Freewheel] 오류 코드](freewheel-error-codes.md)
