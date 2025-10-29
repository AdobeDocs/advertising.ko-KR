---
title: 배치 만들기
description: 배치를 만드는 방법을 알아봅니다.
feature: DSP Placements
exl-id: 28a328b1-0839-442e-a245-f586a7042f41
source-git-commit: d1be9ab441fd8abdc21491afb57763ec6eb2bec0
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 0%

---

# 배치 만들기

>[!TIP]
>
>특정 캠페인 목표 또는 보고 요구 사항을 기반으로 배치를 만듭니다.

1. 주 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 배치를 포함할 캠페인의 이름을 클릭합니다.

1. 데이터 테이블 위에서 **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다. 메뉴의 [!UICONTROL Placement Types] 섹션에서 배치 유형을 클릭합니다.

   배치 유형은 배치가 포함할 수 있는 광고 유형을 결정합니다.

1. [배치 설정](placement-settings.md) 입력:

   1. [!UICONTROL Placement Basics] 설정을 지정하십시오.

   1. [!UICONTROL Goals] 섹션에서 [!UICONTROL Gross Budget]을(를) 지정하고 선택적으로 추가 배치 목표를 지정합니다.

      일부 필드에는 재정의할 수 있는 기본값이 있습니다.

      배치가 할당된 패키지에 패키지 수준 간격 지정이 있는 경우 목표 및 간격 지정 설정은 패키지 설정을 반영합니다.

   1. (선택 사항) [!UICONTROL Geo-Targeting] 섹션에서 포함 또는 제외된 위치를 좁힙니다.

      특정 위치를 식별하지 않으면 모든 위치가 타깃팅됩니다.

      >[!NOTE]
      >
      >Roku 배치에 도시 및 DMA 위치를 사용할 수 없습니다.

   1. [!UICONTROL Inventory Targeting] 섹션에서 포함 또는 제외할 인벤토리 원본 범위를 좁힙니다.

      대부분의 배치 유형에는 기본적으로 모든 재고 유형과 각 유형의 모든 소스가 포함됩니다. [!DNL Roku] 배치의 경우 인벤토리 유형 및 소스를 지정해야 합니다.

   1. (선택 사항) [!UICONTROL Site or app And Keyword Targeting] 섹션에서 대상 및 제외할 사이트 및 앱의 범위를 좁힙니다.

   1. (선택 사항) [!UICONTROL Audience Targeting] 섹션에서:

      1. 대상자 범위를 좁힙니다. 여기에는 배치 내에서 타깃팅할 대상 세그먼트 선택이 포함됩니다.

         [!DNL Roku] 배치의 경우 [(옵트인) 결정적 데이터 세트에 대해 일치시킬 수 있는 하나 이상의 대상 세그먼트를 포함하여  [!DNL Roku]](/help/dsp/inventory/roku-inventory.md)과(와) 일치하는 [!DNL Roku]DSP의 고유한 대상 세그먼트를 활용할 수 있습니다.

         활성, 예약됨 또는 일시 중지됨 배치에 첨부되지 않은 자사 RampID 세그먼트는 일시 중지됩니다. 세그먼트는 세그먼트 목록에 &quot;자동 일시 중지됨&quot;으로 표시됩니다.

      1. (사람 수준 크로스 디바이스 타깃팅이 있는 캠페인의 경우, 선택 사항) 배치가 하나 이상의 특정 대상을 타겟팅하는 경우 배치에 대해 사람 기반 크로스 디바이스 타깃팅을 활성화합니다.

         사용자 기반 장치 간 타깃팅은 [!DNL LiveRamp]에서 미국 데이터만 사용하여 제공합니다. [!DNL LiveRamp] 장치 그래프(즉, 타깃팅된 대상 세그먼트 내에서 찾을 수 없는 장치의 경우)를 사용하여 제공된 노출 횟수에 대해 $0.35 CPM의 모든 광고주가 이 서비스를 사용할 수 있습니다.

   1. (선택 사항) [!DNL Brand Safety and Media Targeting] 섹션에서 배치에 대한 브랜드 안전 제한을 적용합니다.

   1. (선택 사항) [!DNL Tracking] 섹션에서 배치에 있는 광고의 서드파티 이벤트 픽셀 또는 전환 픽셀을 입력합니다.

      >[!NOTE]
      >
      >([!DNL Roku]개 배치) [!DNL Roku]이(가) 승인한 타사 픽셀 공급업체는 [!DNL Acxiom], [!DNL Comscore], [!DNL Data Plus Math], [!DNL Experian], [!DNL Factual], [!DNL Kantar], [!DNL Marketing Evolution], [!DNL Neustar], [!DNL Nielsen], [!DNL Nielsen Catalina Solutions], [!DNL NinthDecimal], [!DNL Oracle], [!DNL Placed], [!DNL Polk] 및 [!DNL Research Now]입니다.

1. **[!UICONTROL Create Placement]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 배치에 광고 첨부:

   1. **[!UICONTROL Attach an ad]**&#x200B;을(를) 클릭합니다.

   1. 다음 중 하나를 수행합니다.

      * 새 광고를 만들려면 다음 작업을 수행하십시오.

         1. **[!UICONTROL Create a New Ad].** 클릭

         1. [오디오 광고](/help/dsp/campaign-management/ads/ad-settings-audio.md), [연결된 TV](/help/dsp/campaign-management/ads/ad-settings-connected-tv.md), [디스플레이 광고](/help/dsp/campaign-management/ads/ad-settings-display.md), [모바일 광고](/help/dsp/campaign-management/ads/ad-settings-mobile.md), [기본 광고](/help/dsp/campaign-management/ads/ad-settings-native.md), [프리롤 광고](/help/dsp/campaign-management/ads/ad-settings-pre-roll.md) 또는 [범용 비디오 광고](/help/dsp/campaign-management/ads/ad-settings-universal-video.md)에 대한 광고 설정을 지정하십시오.

        >[!NOTE]
        >
        >범용 비디오 배치에는 범용 비디오 광고만 포함될 수 있습니다.

         1. **[!UICONTROL Save & Submit for Review]**&#x200B;을(를) 클릭합니다.

         1. (선택 사항) 배치에 대해 만들려는 각 추가 광고에 대해 **[!UICONTROL Attach Another Ad]**&#x200B;을(를) 클릭한 다음 1-3단계를 반복합니다.

         1. 기존 광고를 첨부하지 않으려면 **[!UICONTROL I'm done for now]**&#x200B;을(를) 클릭합니다.

      * 캠페인에 기존 광고를 첨부하려면:

         1. **[!UICONTROL Select an Ad]**&#x200B;을(를) 클릭합니다.

         1. 다음 중 하나를 수행합니다.

            * 한 번에 광고를 하나씩 추가하려면:

               1. 광고 이름 옆에 있는 **[!UICONTROL Select].**&#x200B;을(를) 클릭합니다

               1. (선택 사항) 첨부할 각 추가 광고에 대해 **[!UICONTROL Attach Another Ad]**&#x200B;을(를) 클릭한 다음 이 프로세스를 반복합니다.

            * 한 번에 최대 20개의 광고를 추가하려면:

               1. 광고 목록 위에 있는 확인란을 선택합니다.

               1. 추가할 각 광고 옆에 있는 확인란을 선택합니다.

               1. **[!UICONTROL Attach]**&#x200B;을(를) 클릭합니다.

               1. 광고 이름 옆에 있는 **[!UICONTROL Select]**&#x200B;을(를) 클릭합니다.

         1. (선택 사항) 배치의 특정 광고에 대한 기본 비행 기간 및 광고 회전을 무시하려면 다음을 수행하십시오.

            1. **[!UICONTROL Custom Schedule Ads]**&#x200B;을(를) 클릭합니다.

            1. 다음 중 하나를 수행합니다.

               * 항공편을 추가하려면 **[!UICONTROL Add Flight]**&#x200B;을(를) 클릭한 다음 시작 날짜와 종료 날짜를 지정하십시오.

               * 광고에 기존 비행을 추가하려면 비행 열의 광고 행에서 **[!UICONTROL +]**&#x200B;을(를) 클릭합니다.

               * 광고에서 기존 플라이트 제거를 수행하려면 플라이트 열의 광고 행에서 **[!UICONTROL x]**&#x200B;을(를) 클릭합니다.

               * (여러 광고의 비행 시간이 동일한 경우) 광고를 불균일하게 회전하려면 비행 정보에서 **[!UICONTROL Even Rotation]**&#x200B;을(를) 클릭한 다음 각 광고를 회전하는 상대 가중치를 백분율로 입력하십시오.

                 총 가중치는 100이어야 합니다.

            1. 오른쪽 상단에서 **[!UICONTROL Continue]**&#x200B;을(를) 클릭합니다.

            1. 비행 세부 정보를 검토한 다음 **[!UICONTROL Save & Finish]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [배치 관리 정보](placement-about.md)
>* [배치 편집](placement-edit.md)
>* [배치에 대한 입찰 승수 관리](placement-manage-bid-multipliers.md)
>* [배치에 대한 광고 일정 편집](placement-edit-ad-schedule.md)
>* [배치 비활성화 또는 활성화](placement-pause-activate.md)
>* [배치에 대한 변경 로그 보기](placement-change-log.md)
>* [배치 설정](placement-settings.md)
>* [배치 예측 보고서 보기](/help/dsp/campaign-management/reports/placement-forecast.md)
>* 범용 비디오에 대한 [FAQ](/help/dsp/campaign-management/faq-universal-video.md)
>* [키보드 단축키](/help/dsp/campaign-management/reports/keyboard-shortcuts.md)
>* [성능 문제 해결](/help/dsp/optimization/troubleshooting-performance.md)
>* [비디오: 표준 디스플레이 배치를 만드는 방법](https://video.tv.adobe.com/v/340454)
