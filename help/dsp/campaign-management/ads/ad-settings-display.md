---
title: 광고 설정 표시
description: 디스플레이 광고에 사용할 수 있는 광고 설정에 대한 설명을 참조하십시오.
feature: DSP Ads
exl-id: cff65a48-486f-401e-9759-2bb63871448f
source-git-commit: 9d9330847c9356180928337a4a452f35e7024545
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---

# 광고 설정 표시

다음 설정은 표준 디스플레이 광고에 사용됩니다.

## [!UICONTROL Ad Options]

### 기본

**[!UICONTROL Ad Type]:**(읽기 전용) 만들고 있는 광고 유형으로, 광고를 연결할 수 있는 배치 유형에 해당합니다. 기본값은 *[!UICONTROL Display]*&#x200B;입니다.

**[!UICONTROL Ad Name]:** 광고 이름입니다. 에셋 제목은 기본적으로 사용되지만 이름을 변경할 수 있습니다.

>[!TIP]
>
> 광고를 게재에 첨부할 때, [!UICONTROL Ads] 보기 및 보고서에서 쉽게 찾을 수 있는 이름을 사용합니다. 예를 들어 단위 유형 및 일부 주요 속성(예: Holiday Product Preview: 300x250 Gamer&quot;)을 설명합니다.

**\[Ad Source\]**: (읽기 전용) *[!UICONTROL 3rd party]*.

**[!UICONTROL This is an expandable Banner]:**(타사 광고만 해당) 확장 가능한 배너 광고임을 나타냅니다. 관련 확장 설정에 따라 구매할 재고가 결정되므로 광고 비헤이비어가 반영되었는지 확인합니다.

**[!UICONTROL Expansion Method]:**(타사 확장 가능한 배너 광고만 해당) 배너가 *[!UICONTROL Click]* 또는 *[!UICONTROL Rollover]*&#x200B;에서 확장되는지 여부.

**[!UICONTROL Expansion Directions]:**(타사 확장 가능 배너 광고만 해당) 광고가 확장되는 방향: *[!UICONTROL Up]*, *[!UICONTROL Down]*, *[!UICONTROL Left]* 또는 *[!UICONTROL Right]*.

**[!UICONTROL Certified Vendors]:**(타사 확장 가능한 배너 광고만 해당) 광고를 사용할 수 있는 인증된 공급업체입니다. *[!UICONTROL DCM]*([!DNL Google DoubleClick for Advertisers]), *[!UICONTROL Flashtalking]*, *[!UICONTROL Sizmek]* 또는 *[!UICONTROL Jivox]*.

**[!UICONTROL Display Code]:**(타사 광고 전용) 타사 광고 자산의 URL입니다. [timestamp] 및 [[timestamp]] 매개 변수가 실제 값으로 대체됩니다.

**[!UICONTROL Final Display Code]:**(타사 광고만 해당) 필요한 [Advertising DSP 추적 매크로](/help/dsp/campaign-management/macros.md)가 삽입된 타사 크리에이티브 에셋의 URL입니다(해당하는 경우).

**[!UICONTROL Ad Size]:** 광고의 너비와 높이입니다. [지원되는 표준 디스플레이 광고 크기](ad-specs.md)여야 합니다. 광고를 업로드하거나 [!UICONTROL Display Code]을(를) 입력하기 전에 광고 크기를 수동으로 입력할 수 있습니다. 광고 크기를 입력하지 않으면 업로드된 광고 또는 광고 태그의 차원이 자동으로 읽기 전용으로 입력됩니다.

>[!IMPORTANT]
>
> 너비 및 높이 필드에서 선언된 광고 크기는 수신 입찰 요청과 일치합니다. 광고의 차원이 선언된 광고 크기와 일치하지 않으면 게재 문제가 발생할 수 있습니다.

### [!UICONTROL Pixel]

배치에 대한 기존의 모든 이벤트 추적 픽셀은 자동으로 첨부됩니다. 개별 광고에 대한 추적 요구 사항을 기반으로 기존 픽셀을 분리하고 필요에 따라 새 픽셀을 만들 수 있습니다. **팁:** [!UICONTROL Ad Tools] 보기를 사용하여 한 번에 배치의 여러 광고에 대한 타사 추적 픽셀을 편집하려면 &quot;[배치에 타사 추적 픽셀 첨부](/help/dsp/campaign-management/ads/ad-pixel-attach-detach.md#attach-pixels-ads)&quot;를 참조하십시오.

다음 설정은 사용자가 만들거나 편집하는 각 픽셀에 적용됩니다.

**[!UICONTROL Integration Event]:** 픽셀을 실행하도록 트리거하는 이벤트입니다. 이 광고 유형의 경우 *[!UICONTROL Impression]* 또는 *[!UICONTROL Click-through]*&#x200B;에서 실행되는 픽셀을 사용하십시오.

**[!UICONTROL Pixel Type]:** 픽셀이 *[!UICONTROL IMG URL]*(1x1 픽셀 이미지 파일), *[!UICONTROL HTML]* 또는 *[!UICONTROL JavaScript URL]*&#x200B;인지 여부.

**[!UICONTROL Pixel URL or Code]:** 지정된 [!UICONTROL Pixel Type]에 적절한 형식의 픽셀 이미지의 URL입니다.

**[!UICONTROL Pixel Name]:** 픽셀 이름입니다. 픽셀을 쉽게 식별하는 데 도움이 되는 이름을 사용합니다.

**[!UICONTROL Pixel Provider]:** 픽셀 공급자: *[!UICONTROL None]*, *[!UICONTROL Comscore]*, *[!UICONTROL WhiteOps]* 또는 *[!UICONTROL IAS]*.

>[!MORELIKETHIS]
>
>* [광고 관리 정보](ad-about.md)
>* [단일 광고 만들기](ad-create.md)
>* [광고에 연결된 배치 나열](ad-list-placements.md)
>* [광고 사양](ad-specs.md)
>* [DSP 매크로](/help/dsp/campaign-management/macros.md)
