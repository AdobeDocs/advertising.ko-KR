---
title: 배치 만들기
description: 배치를 만드는 방법을 알아봅니다.
feature: DSP Placements
exl-id: 28a328b1-0839-442e-a245-f586a7042f41
source-git-commit: 9b3d6893e004b16714bf50f1334424d50fac7c91
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# 배치 만들기

>[!TIP]
>
>특정 캠페인 목표 또는 보고 요구 사항을 기반으로 배치를 만듭니다.

1. 메인 메뉴에서 **[!UICONTROL Campaigns]**.

1. 배치를 포함할 캠페인의 이름을 클릭합니다.

1. 데이터 테이블 위에서 **[!UICONTROL Create]**. 다음에서 [!UICONTROL Placement Types] 메뉴의 섹션에서 배치 유형을 클릭합니다.

   배치 유형은 배치가 포함할 수 있는 광고 유형을 결정합니다.

1. 다음을 입력합니다. [배치 설정](placement-settings.md):

   1. 다음을 지정합니다. [!UICONTROL Placement Basics] 설정.

   1. 다음에서 [!UICONTROL Goals] 섹션에서 다음을 지정합니다. [!UICONTROL Gross Budget] 또한 선택적으로 추가 배치 목표를 지정합니다.

      일부 필드에는 재정의할 수 있는 기본값이 있습니다.

      배치가 할당된 패키지에 패키지 수준 간격 지정이 있는 경우 목표 및 간격 지정 설정은 패키지 설정을 반영합니다.

   1. (선택 사항) [!UICONTROL Geo-Targeting] 섹션, 포함되거나 제외되는 위치의 범위를 좁힙니다.

      특정 위치를 식별하지 않으면 모든 위치가 타깃팅됩니다.

      >[!NOTE]
      >
      >Roku 배치에 도시 및 DMA 위치를 사용할 수 없습니다.

   1. 다음에서 [!UICONTROL Inventory Targeting] 섹션, 포함 또는 제외할 재고 소스 범위를 좁힙니다.

      대부분의 배치 유형에는 기본적으로 모든 재고 유형과 각 유형의 모든 소스가 포함됩니다. 대상 [!DNL Roku] 배치, 재고 유형 및 소스를 지정해야 합니다.

   1. (선택 사항) [!UICONTROL Site Targeting] 섹션을 통해 타겟팅할 사이트 범위를 좁히고 제외할 사이트를 지정합니다.

   1. (선택 사항) [!UICONTROL Audience Targeting] 섹션:

      1. 대상자 범위를 좁힙니다. 여기에는 배치 내에서 타깃팅할 대상 세그먼트 선택이 포함됩니다.

         대상 [!DNL Roku] 배치, 다음을 활용할 수 있습니다. [와 일치하는 DSP의 고유 대상자 [!DNL Roku]](/help/dsp/inventory/roku-inventory.md) 에 대해 일치시킬 수 있는 하나 이상의 대상 세그먼트를 포함하여 [!DNL Roku] (옵트인) 결정론적 데이터 세트입니다.

      1. (사람 수준 크로스 디바이스 타깃팅이 있는 캠페인의 경우, 선택 사항) 배치가 하나 이상의 특정 대상을 타겟팅하는 경우 배치에 대해 사람 기반 크로스 디바이스 타깃팅을 활성화합니다.

         사용자 기반 크로스 디바이스 타깃팅은에서 제공합니다. [!DNL LiveRamp] 미국 데이터만 사용. 이 서비스는 모든 광고주가 $0.35 CPM으로 다음을 사용하여 게재하는 노출물에 사용할 수 있습니다. [!DNL LiveRamp] 장치 그래프(타겟팅된 대상 세그먼트 내에서 찾을 수 없는 장치의 경우).

   1. (선택 사항) [!DNL Brand Safety and Media Targeting] 섹션에서 배치에 대해 브랜드 안전 제한을 적용합니다.

   1. (선택 사항) [!DNL Tracking] 섹션에서 배치에 있는 광고에 대한 서드파티 이벤트 픽셀 또는 전환 픽셀을 입력합니다.

      >[!NOTE]
      >
      >([!DNL Roku] 배치) 서드파티 픽셀 공급업체 승인됨 [!DNL Roku] include [!DNL Acxiom], [!DNL Comscore], [!DNL Data Plus Math], [!DNL Experian], [!DNL Factual], [!DNL Kantar], [!DNL Marketing Evolution], [!DNL Neustar], [!DNL Nielsen], [!DNL Nielsen Catalina Solutions], [!DNL NinthDecimal], [!DNL Oracle], [!DNL Placed], [!DNL Polk], 및 [!DNL Research Now].

1. 클릭 **[!UICONTROL Create Placement]**.

1. (선택 사항) 배치에 광고 첨부:

   1. 클릭 **[!UICONTROL Attach an ad]**.

   1. 다음 중 하나를 수행합니다.

      * 새 광고를 만들려면 다음 작업을 수행하십시오.

         1. 클릭 **[!UICONTROL Create a New Ad].**

         1. 광고 설정 지정 [오디오 광고](/help/dsp/campaign-management/ads/ad-settings-audio.md), [연결된 TV](/help/dsp/campaign-management/ads/ad-settings-connected-tv.md), [디스플레이 광고](/help/dsp/campaign-management/ads/ad-settings-display.md), [모바일 광고](/help/dsp/campaign-management/ads/ad-settings-mobile.md), [기본 광고](/help/dsp/campaign-management/ads/ad-settings-native.md), [프리롤 광고](/help/dsp/campaign-management/ads/ad-settings-pre-roll.md), 또는 [범용 비디오 광고](/help/dsp/campaign-management/ads/ad-settings-universal-video.md).

        >[!NOTE]
        >
        >범용 비디오 배치에는 범용 비디오 광고만 포함될 수 있습니다.

         1. 클릭 **[!UICONTROL Save & Submit for Review]**.

         1. (선택 사항) 배치에 대해 만들려는 각 추가 광고에 대해 **[!UICONTROL Attach Another Ad]**&#x200B;을 클릭한 다음 1~3단계를 반복합니다.

         1. 기존 광고를 첨부하지 않으려면 **[!UICONTROL I'm done for now]**.

      * 캠페인에 기존 광고를 첨부하려면:

      1. 클릭 **[!UICONTROL Select an Ad]**.

      1. 다음 중 하나를 수행합니다.

         * 한 번에 광고를 하나씩 추가하려면:

            1. 광고 이름 옆에 있는 를 클릭합니다. **[!UICONTROL Select].**

            1. (선택 사항) 첨부할 각 추가 광고에 대해 **[!UICONTROL Attach Another Ad]**&#x200B;을 클릭하고 프로세스를 반복합니다.

         * 한 번에 최대 20개의 광고를 추가하려면:

            1. 광고 목록 위에 있는 확인란을 선택합니다.

            1. 추가할 각 광고 옆에 있는 확인란을 선택합니다.

            1. 클릭 **[!UICONTROL Attach]**.

            1. 광고 이름 옆에 있는 를 클릭합니다. **[!UICONTROL Select]**.

      1. (선택 사항) 배치의 특정 광고에 대한 기본 비행 기간 및 광고 회전을 무시하려면 다음을 수행하십시오.

         1. 클릭 **[!UICONTROL Custom Schedule Ads]**.

         1. 다음 중 하나를 수행합니다.

            * 항공편을 추가하려면 **[!UICONTROL Add Flight]**&#x200B;를 클릭한 다음 시작 날짜와 종료 날짜를 지정합니다.

            * 기존 비행을 광고에 추가하려면 **[!UICONTROL +]** (비행 열의 광고 행).

            * 광고에서 기존 항공편을 제거하려면 **[!UICONTROL x]** (비행 열의 광고 행).

            * (여러 광고의 비행 시간이 동일한 경우) 광고를 불균일하게 회전하려면 다음을 클릭하십시오. **[!UICONTROL Even Rotation]** 그런 다음 각 광고를 회전할 상대적 가중치를 백분율로 입력합니다.

              총 가중치는 100이어야 합니다.

         1. 오른쪽 상단에서 **[!UICONTROL Continue]**.

         1. 비행 세부 사항을 검토한 다음 **[!UICONTROL Save & Finish]**.

>[!MORELIKETHIS]
>
>* [배치 관리 정보](placement-about.md)
>* [배치 편집](placement-edit.md)
>* [배치에 대한 입찰 승수 관리](placement-manage-bid-multipliers.md)
>* [배치에 대한 광고 일정 편집](placement-edit-ad-schedule.md)
>* [배치 일시 중지 또는 활성화](placement-pause-activate.md)
>* [배치에 대한 변경 로그 보기](placement-change-log.md)
>* [배치 설정](placement-settings.md)
>* [배치 예측 보고서 보기](/help/dsp/campaign-management/reports/placement-forecast.md)
>* [범용 비디오에 대한 FAQ](/help/dsp/campaign-management/faq-universal-video.md)
>* [키보드 단축키](/help/dsp/campaign-management/reports/keyboard-shortcuts.md)
>* [문제 해결 성능](/help/dsp/optimization/troubleshooting-performance.md)
>* [비디오: 표준 디스플레이 배치를 만드는 방법](https://video.tv.adobe.com/v/340454)
