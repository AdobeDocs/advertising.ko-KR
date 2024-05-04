---
title: 광고 설정 표시
description: 디스플레이 광고에 사용할 수 있는 광고 설정에 대한 설명을 참조하십시오.
feature: DSP Ads
exl-id: cff65a48-486f-401e-9759-2bb63871448f
source-git-commit: 2f137b17deea4cd02ae19494a306ff37c7002423
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# 광고 설정 표시

다음 설정은 표준 디스플레이 광고에 사용됩니다.

## [!UICONTROL Ad Options]

### 기본

**[!UICONTROL Ad Type]:** (읽기 전용) 광고를 첨부할 수 있는 배치 유형에 해당하는 생성 중인 광고 유형입니다. 기본값은 입니다 *[!UICONTROL Display]*.

**[!UICONTROL Ad Name]:** 광고 이름. 에셋 제목은 기본적으로 사용되지만 이름을 변경할 수 있습니다.

>[!TIP]
>
> 에서 광고를 배치에 첨부할 때 쉽게 찾을 수 있는 이름을 사용합니다. [!UICONTROL Ads] 보고서에서 및 를 봅니다. 예를 들어 단위 유형 및 일부 주요 속성(예: Holiday Product Preview: 300x250 Gamer&quot;)을 설명합니다.

**\[광고 소스\]**: (읽기 전용) *[!UICONTROL 3rd party]*.

**[!UICONTROL This is an expandable Banner]:** (타사 광고만 해당) 광고가 확장 가능한 배너 광고임을 나타냅니다. 관련 확장 설정에 따라 구매할 재고가 결정되므로 광고 비헤이비어가 반영되었는지 확인합니다.

**[!UICONTROL Expansion Method]:** (타사 확장 가능한 배너 광고만 해당) 배너가 *[!UICONTROL Click]* 또는 *[!UICONTROL Rollover]*.

**[!UICONTROL Expansion Directions]:** (타사 확장 가능 배너 광고만 해당) 광고가 확장되는 방향. *[!UICONTROL Up]*, *[!UICONTROL Down]*, *[!UICONTROL Left]*, 또는 *[!UICONTROL Right]*.

**[!UICONTROL Certified Vendors]:** (확장 가능한 타사 배너 광고만 해당) 광고를 사용할 수 있는 인증된 공급업체: *[!UICONTROL DCM]* ([!DNL Google DoubleClick for Advertisers]), *[!UICONTROL Flashtalking]*, *[!UICONTROL Sizmek]*, 또는 *[!UICONTROL Jivox]*.

**[!UICONTROL Display Code]:** (타사 광고만 해당) 타사 광고 자산의 URL입니다. 임의 [timestamp] 및 [[timestamp]] 매개 변수가 실제 값으로 대체됩니다.

**[!UICONTROL Final Display Code]:** (타사 광고만 해당) 타사 크리에이티브 에셋의 URL로서 필요한 경우 [Advertising DSP 추적 매크로](/help/dsp/campaign-management/macros.md) 해당하는 경우 삽입됩니다.

**[!UICONTROL Ad Size]:** 광고의 너비 및 높이입니다. 다음이어야 합니다. [지원되는 표준 디스플레이 광고 크기](ad-specs.md). 광고를 업로드하거나 입력하기 전에 광고 크기를 수동으로 입력할 수 있습니다. [!UICONTROL Display Code]. 광고 크기를 입력하지 않으면 업로드된 광고 또는 광고 태그의 차원이 자동으로 읽기 전용으로 입력됩니다. 크기가 표준 디스플레이 크기(예: 300x250 광고 크기 대신 301x250)에 없는 경우 디스플레이 광고가 저장되지 않습니다.

>[!IMPORTANT]
>
> 너비 및 높이 필드에서 선언된 광고 크기는 수신 입찰 요청과 일치합니다. 광고의 차원이 선언된 광고 크기와 일치하지 않으면 게재 문제가 발생할 수 있습니다.

### [!UICONTROL Pixel]

배치에 대한 기존의 모든 이벤트 추적 픽셀은 자동으로 첨부됩니다. 개별 광고에 대한 추적 요구 사항을 기반으로 기존 픽셀을 분리하고 필요에 따라 새 픽셀을 만들 수 있습니다. **팁:** 를 사용하여 한 번에 배치의 여러 광고에 대한 서드파티 추적 픽셀을 편집하려면 다음과 같이 하십시오. [!UICONTROL Ad Tools] 보기, 참조 &quot;[배치에 있는 광고에 서드파티 추적 픽셀 첨부](/help/dsp/campaign-management/ads/ad-attach-to-placement.md#attach-pixels-ads).&quot;

다음 설정은 사용자가 만들거나 편집하는 각 픽셀에 적용됩니다.

**[!UICONTROL Integration Event]:** 픽셀을 실행하도록 트리거하는 이벤트입니다. 이 광고 유형의 경우 *[!UICONTROL Impression]* 또는 *[!UICONTROL Click-through]*.

**[!UICONTROL Pixel Type]:** 픽셀이 *[!UICONTROL IMG URL]* (1x1 픽셀 이미지 파일), *[!UICONTROL HTML]*, 또는 *[!UICONTROL JavaScript URL]*.

**[!UICONTROL Pixel URL or Code]:** 지정된 내용에 적합한 형식의 픽셀 이미지 URL [!UICONTROL Pixel Type].

**[!UICONTROL Pixel Name]:** 픽셀 이름. 픽셀을 쉽게 식별하는 데 도움이 되는 이름을 사용합니다.

**[!UICONTROL Pixel Provider]:** 픽셀 공급자: *[!UICONTROL None]*, *[!UICONTROL Comscore]*, *[!UICONTROL WhiteOps]*, 또는 *[!UICONTROL IAS]*.

>[!MORELIKETHIS]
>
>* [광고 관리 기본 정보](ad-about.md)
>* [단일 광고 만들기](ad-create.md)
>* [광고와 연결된 배치 나열](ad-list-placements.md)
>* [광고 사양](ad-specs.md)
>* [DSP 매크로](/help/dsp/campaign-management/macros.md)
