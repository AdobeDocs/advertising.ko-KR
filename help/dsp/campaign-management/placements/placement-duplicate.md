---
title: 중복 배치
description: 하나 이상의 배치를 복제하는 방법을 알아봅니다.
feature: DSP Placements
exl-id: 41021f5b-13d1-419f-af03-c5507f9fed4d
source-git-commit: 051658d822253e5d0cac56e3d59e99386c68fb71
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# 중복 배치

<!-- Some placements don't have this option. Clarify which placement types aren't eligible -- is it PG placements, or all placements using private inventory? And anything else? -->

하나 이상의 배치를 복제하여 유사한 설정의 배치를 만듭니다. 다음을 수행할 수 있습니다.

* 여러 개의 배치 중복 만들기
* 원래 광고주 및 캠페인 내 또는 다른 광고주 및 캠페인 내에 중복 배치
* (원본 캠페인 내의 중복 배치의 경우) 선택적으로 원본 광고를 복제합니다
* 새 배치의 상태 및 플라이트 날짜 수정

중복되지 않은 배치 설정 목록은 &quot;[중복되지 않은 항목](#placement-not-duplicated)&quot;을 참조하십시오.

1. 주 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 캠페인의 이름을 클릭합니다.

1. 하위 메뉴에서 **[!UICONTROL Placements]**&#x200B;을(를) 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * 한 배치를 복제하려면 패키지 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Duplicate]**&#x200B;을(를) 클릭합니다.

   * 여러 배치를 복제하려면 다음을 수행합니다.

      1. 복제할 각 배치 옆의 확인란을 선택합니다.

      1. 일괄 작업 도구 모음에서 **[!UICONTROL Duplicate]**&#x200B;을(를) 클릭합니다.

1. 새 배치 설정을 지정합니다.

   1. (단일 배치) 새 배치 이름을 입력합니다.

   1. **[!UICONTROL Choose Package (Required)]** 메뉴에서 부모 패키지 또는 &lbrace;1*** 중 하나를 선택합니다.[!UICONTROL No package]

   1. (선택 사항) 기본 설정을 변경합니다.

   설정은 선택한 모든 배치에 적용됩니다.

   기본적으로 새 배치는 원래 광고 유형에 대한 것이고, 원래 광고주 및 캠페인에 지정되고, 현재 날짜에 시작되는 비행 일정이 있으며, 일시 중지되고, 원래 광고를 포함하지 않습니다.

   여러 배치를 만들 때 새 배치 이름은 규칙 &lt;*original_placement_name #N*>(예: &quot;내 배치 #2&quot;)을 사용하여 차례로 숫자로 추가됩니다.

1. **[!UICONTROL Submit]**&#x200B;을(를) 클릭합니다.

## 복제되지 않은 항목 {#placement-not-duplicated}

원래 배치의 모든 설정은 다음을 제외하고 복제됩니다.

* 실험 설정
* (플라이트 날짜를 변경하는 경우) 사용자 지정 광고 예약
* (광고를 첨부하지 않는 경우) 사용자 지정 광고 가중치 및 예약
* 프로그래밍 방식 보장(PG) 거래의 기본 배치 및 [!UICONTROL Simple Ad Serving] 거래의 배치
* (배치를 다른 캠페인에 복사하는 경우):
   * 지역 대상
   * 이벤트 픽셀
   * 광고
   * 배치 수준 [!DNL DoubleVerify Authentic Brand Safety] 세그먼트(광고주 수준 세그먼트를 재정의함)

## 새 배치 구성 모범 사례

>[!TIP]
>
>* 일괄 시트를 사용하여 [한 번에 여러 캠페인 구성 요소를 변경](/help/dsp/campaign-management/campaign-components-review-edit.md)할 수 있습니다.
>* 광고 태그 시트를 사용하여 [여러 타사 광고를 업로드](/help/dsp/campaign-management/ads/ad-create-multiple.md)합니다.

* 새 배치를 활성화할 준비가 될 때까지 일시 중지합니다.

* 다음 사항을 고려하고 필요에 따라 새 배치 설정을 편집합니다.

   * 그 계좌는 새로운 배치 예산을 수용할 충분한 자금이 있습니까?

   * 새 배치에 이전 배치와 다른 예산이 필요합니까?

   * 필요한 사용자 지정 광고 가중치 및 일정을 포함하여 크리에이티브를 업로드하고 배치에 첨부합니다.

   * 필요에 따라 배치 및 광고에 이벤트 픽셀을 첨부합니다.

   * 필요에 따라 지리적 대상과 배치 수준 [!DNL DoubleVerify Authentic Brand Safety] 세그먼트를 배치에 포함하십시오.

   * 프로그램 보증 거래의 경우 새 거래 ID를 사용하고 기본 배치를 만듭니다.

   * 필요에 따라 [!UICONTROL Simple Ad Serving] 거래에 대한 새 배치를 만듭니다.

>[!MORELIKETHIS]
>
>* [배치 관리 정보](placement-about.md)
>* [배치 만들기](placement-create.md)
>* [배치 편집](placement-edit.md)
>* [배치에 대한 변경 로그 보기](placement-change-log.md)
>* [배치 설정](placement-settings.md)
