---
title: 광고에서 픽셀 첨부 및 제거
description: 광고에서 서드파티 추적 픽셀을 첨부 및 제거하는 방법을 알아봅니다.
feature: DSP Ads
source-git-commit: a3bd04da6c6f428fdb6e1f05187ea3de0174c9d7
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# 광고에서 픽셀 첨부 및 제거

광고에서 서드파티 추적 픽셀을 연결 및 분리할 수 있습니다.

## [!UICONTROL Ad Tools] 보기 열기 {#ad-tools-open}

1. 주 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 캠페인의 이름을 클릭합니다.

1. 다음 방법 중 하나로 [!UICONTROL Ad Tools] 보기를 엽니다.

   * ([!UICONTROL Campaigns] 보기에서) 캠페인 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Ad Tools].**&#x200B;을(를) 클릭합니다.

   * ([!UICONTROL Packages] , [!UICONTROL Placements] 또는 [!UICONTROL Ads] 보기에서) 오른쪽 상단에서 **[!UICONTROL ...]** > **[!UICONTROL Ad Tools]**&#x200B;을(를) 클릭합니다.

## 배치에 있는 광고에 서드파티 추적 픽셀 첨부 {#attach-pixels-ads}

1. [[!UICONTROL Ad Tools] 보기를 엽니다](#ad-tools-open).

   **[!UICONTROL Attach Pixels]** 탭이 열립니다.

1. [!UICONTROL Edit] 하위 보기에서:

   1. (선택 사항) 다음 방법 중 하나로 광고와 서드파티 픽셀을 찾습니다.

      * 왼쪽 표 위에 있는 ![필터](/help/dsp/assets/filter.png)를 클릭하고 광고 상태, 광고 유형, 픽셀 통합 이벤트 또는 픽셀 유형별로 목록을 필터링합니다.

      * 오른쪽 및 왼쪽 표 위에서 광고 이름 및 픽셀 이름에서 특정 텍스트 문자열을 검색합니다.

   1. (캠페인에 대한 서드파티 추적 픽셀이 없는 경우) 픽셀을 만듭니다.

      1. 오른쪽 테이블에서 **[!UICONTROL Create pixel]**&#x200B;을(를) 클릭합니다.

      1. 설정을 지정합니다.

         **[!UICONTROL Integration Event]:** 픽셀을 실행하도록 트리거하는 이벤트(예: *[!UICONTROL Impression]* 또는 *[!UICONTROL Click-through]*).

         **[!UICONTROL Pixel Type]:** 픽셀이 *[!UICONTROL IMG URL]*(1x1 픽셀 이미지 파일), *[!UICONTROL HTML]* 또는 *[!UICONTROL JavaScript URL]*&#x200B;인지 여부.

         **[!UICONTROL Pixel URL or Code]:** 지정된 픽셀 유형에 적절한 형식의 픽셀 이미지 URL입니다.

         **[!UICONTROL Pixel Name]:** 픽셀 이름입니다. 픽셀을 쉽게 식별하는 데 도움이 되는 이름을 사용합니다.

         **[!UICONTROL Pixel Provider]:** 픽셀 공급자: *[!UICONTROL None]*, *[!UICONTROL Comscore]*, *[!UICONTROL WhiteOps]* 또는 *[!UICONTROL IAS]*.

      1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

   1. 왼쪽 표에서 서드파티 추적 픽셀을 첨부할 각 광고 옆에 있는 확인란을 선택합니다.

   1. 오른쪽 표에서 선택한 광고에 첨부할 각 서드파티 추적 픽셀 옆의 확인란을 선택합니다.

      선택한 광고에 아직 첨부되지 않은 픽셀만 선택할 수 있습니다.

   1. 오른쪽 하단에서 **[!UICONTROL Attach]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 캠페인 세부 정보 보기로 돌아가려면 ![ 왼쪽에 있는 ](/help/dsp/assets/breadcrumb-return.png "폴더로 돌아가기")폴더로 돌아가기[!UICONTROL Ad Tools]를 클릭하고 캠페인 이름을 선택합니다.

## 배치의 광고에서 서드파티 추적 픽셀 분리 {#detach-pixels-ads}

1. [[!UICONTROL Ad Tools] 보기를 엽니다](#ad-tools-open).

   **[!UICONTROL Attach Pixels]** 탭이 열립니다.

1. [!UICONTROL Edit] 하위 보기에서:

   1. (선택 사항) 다음 방법 중 하나로 광고와 서드파티 픽셀을 찾습니다.

      * 왼쪽 표 위에 있는 ![필터](/help/dsp/assets/filter.png)를 클릭하고 광고 상태, 광고 유형, 픽셀 통합 이벤트 또는 픽셀 유형별로 목록을 필터링합니다.

      * 오른쪽 및 왼쪽 표 위에서 광고 이름 및 픽셀 이름에서 특정 텍스트 문자열을 검색합니다.

   1. 왼쪽 표에서 서드파티 추적 픽셀을 분리할 각 광고 옆에 있는 확인란을 선택합니다.

   1. 오른쪽 표에서 선택한 광고에서 분리할 각 타사 추적 픽셀 옆의 확인란을 선택합니다.

      선택한 모든 광고에 첨부된 픽셀만 선택할 수 있습니다.

   1. 오른쪽 하단에서 **[!UICONTROL Detach]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 캠페인 세부 정보 보기로 돌아가려면 ![ 왼쪽에 있는 ](/help/dsp/assets/breadcrumb-return.png "폴더로 돌아가기")폴더로 돌아가기[!UICONTROL Ad Tools]를 클릭하고 캠페인 이름을 선택합니다.

## 광고에 첨부된 픽셀 보기 {#view-pixels-ads}

1. [[!UICONTROL Ad Tools] 보기를 엽니다](#ad-tools-open).

   **[!UICONTROL Attach Pixels]** 탭이 열립니다.

1. 오른쪽 상단의 **[!UICONTROL View]** 옵션으로 전환합니다.

1. (선택 사항) 필요에 따라 광고 및 서드파티 픽셀을 찾습니다.

   * 왼쪽 표 위에 있는 ![필터](/help/dsp/assets/filter.png)를 클릭하고 광고 상태, 광고 유형, 픽셀 통합 이벤트 또는 픽셀 유형별로 목록을 필터링합니다.

   * 오른쪽 및 왼쪽 표 위에서 광고 이름 및 픽셀 이름에서 특정 텍스트 문자열을 검색합니다.

1. 왼쪽 테이블의 광고 행을 클릭하면 오른쪽 테이블에 첨부된 픽셀이 표시됩니다.

1. (선택 사항) 광고에 더 많은 픽셀을 첨부하려면 오른쪽 상단의 **[!UICONTROL Edit]** 보기로 전환합니다. 지침은 이전 절차의 3단계, &quot;[배치에 서드파티 추적 픽셀 첨부](#attach-pixels-ads)&quot;를 참조하십시오.

>[!MORELIKETHIS]
>
>* [광고 관리 정보](ad-about.md)
>* [배치에 광고 첨부](/help/dsp/campaign-management/ads/ad-attach-to-placement.md)
>* [단일 광고 만들기](ad-create.md)
>* [여러 타사 광고 만들기](ad-create-multiple.md)
>* [광고 편집](ad-edit.md)
>* [광고에 연결된 배치 나열](ad-list-placements.md)
>* [배치에 대한 광고 일정 편집](/help/dsp/campaign-management/placements/placement-edit-ad-schedule.md)
>* 범용 비디오에 대한 [FAQ](/help/dsp/campaign-management/faq-universal-video.md)

