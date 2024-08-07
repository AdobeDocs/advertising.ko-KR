---
title: '[!UICONTROL Simple Ad Serving] 거래 만들기'
description: '[!UICONTROL Simple Ad Serving] 거래의 추적 픽셀을 만드는 방법을 알아봅니다.'
feature: DSP Simple Ad Serving
exl-id: 77d5dabd-1a0d-4dce-8a9a-8d54a637e15d
source-git-commit: 443f8907644bf3e480626e14713e8abb9bfca284
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# [!UICONTROL Simple Ad Serving] 거래 만들기

1. 메인 메뉴에서 **[!UICONTROL Inventory]** > **[!UICONTROL Deals].**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위에서 **[!UICONTROL Create]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Simple Ad Serving]**&#x200B;을(를) 선택합니다.

1. [거래 설정](simple-deal-settings.md) 입력:

   1. [!UICONTROL Select Ad Source] 섹션에서 게시자, 광고주 및 캠페인, 광고 유형에 대한 정보를 지정한 다음 **[!UICONTROL Next]**&#x200B;을(를) 클릭합니다.

   1. [!UICONTROL Select Ad(s)] 섹션에서 DSP에서 프록시로 사용할 광고를 지정합니다.

      1. 다음 중 하나를 수행합니다.

         * 기존 광고의 경우 사용할 광고를 선택합니다.

         * 새 광고의 경우 프록시 [타사 광고](/help/dsp/campaign-management/ads/ad-create-multiple.md)를 만드십시오.

      >[!NOTE]
      > DSP은 지정한 광고를 제공하지 않습니다. 게시자가 광고를 게재합니다.

      1. **[!UICONTROL Next]**&#x200B;을(를) 클릭합니다.

   1. 피드 세부 정보에서 피드 세부 사항을 편집한 다음 **[!UICONTROL Next]**&#x200B;을(를) 클릭합니다.

      DSP은 광고에 대해 &quot;SAS 배치 - &lt;*거래 이름*>&quot;이라는 배치를 자동으로 생성합니다. 배치에서 거래는 [!UICONTROL Inventory Targets] 섹션에서 자동으로 타깃팅됩니다. 다른 모든 타깃팅 옵션은 적용할 수 없습니다.

1. 다음 방법 중 하나로 구현을 위해 이벤트 추적 픽셀을 게시자에게 보냅니다.

   * (선택 사항) [!UICONTROL Activate Tag with Publisher] 화면에서 거래 태그를 게시자에게 보냅니다.

     이전 단계를 완료하면 DSP에서 게시자에게 보낼 수 있는 이메일 메시지를 생성합니다. 이 메시지에는 거래 세부 사항, 거래 태그를 검색할 링크 및 링크에 대한 인증 코드가 포함됩니다.

      1. 거래 세부 사항을 검토하고 다음 중 하나를 수행합니다.

         * 장치의 전자 메일 응용 프로그램에 정보를 전자 메일 메시지에 붙여 넣으려면 **[!UICONTROL Email & Done]**&#x200B;을(를) 클릭하고 전자 메일 응용 프로그램을 선택하십시오. [!UICONTROL CC:] 필드가 [!DNL Adobe] 지원 주소로 미리 채워져 있습니다. 그런 다음 메시지를 게시자에게 적절한 연락처로 보낼 수 있습니다.

         * 클립보드에 정보를 복사하려면 **[!UICONTROL Copy Email]을(를) 클릭합니다.** 전자 메일 메시지에 내용을 수동으로 붙여 넣고 게시자의 해당 연락처로 보낼 수 있습니다. `publisher-support-global@adobe.com`에 대한 복사본(참조:)을 포함해야 합니다. 메시지 복사가 끝나면 **[!UICONTROL Email & Done]**&#x200B;을(를) 클릭합니다.

      1. (필요한 경우) 게시자의 후속 작업을 통해 태그가 적절한 매크로를 포함하여 게시자의 광고 서버에서 태그가 작동하는지 확인합니다.

   * (선택 사항) 이벤트 추적 픽셀을 수동으로 게시자에게 보냅니다.

      1. [!UICONTROL Deals] 보기의 거래 행에서 ![옵션 메뉴](/help/dsp/assets/options-menu.png) **>[!UICONTROL show pixel]**&#x200B;을(를) 클릭합니다.

         이벤트 픽셀에는 [!UICONTROL Clickthrough] 픽셀과 [!UICONTROL Impression] 픽셀이 포함됩니다. 비디오 및 오디오 광고에는 완료된 사분위별 이벤트 픽셀도 포함됩니다([!UICONTROL 25% Complete]부터 [!UICONTROL 100% Complete]까지).

      1. 이벤트 추적 픽셀을 복사하여 게시자에게 제공합니다.

>[!MORELIKETHIS]
>
>* [정보 [!UICONTROL Simple Ad Serving]](simple-deal-about.md)
>* [[!UICONTROL Simple Ad Serving] 설정](simple-deal-settings.md)
>* [거래에 대한 자세한 보고서 보기](/help/dsp/inventory/deal-view-report.md)

<!-- add back when reimplemented:
>* [View Event-Tracking Pixels for a [!UICONTROL Simple Ad Serving] Deal](simple-deal-show-pixels.md)
-->
