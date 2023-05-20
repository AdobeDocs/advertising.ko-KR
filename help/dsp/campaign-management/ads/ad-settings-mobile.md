---
title: 모바일 광고 설정
description: 모바일 광고에 사용할 수 있는 광고 설정에 대한 설명을 참조하십시오.
feature: DSP Ads
exl-id: 45e8da8c-d6a2-4c42-8932-4cf551f6f899
source-git-commit: 7e614ecb517515217d812926f61ca10437820efd
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# 모바일 광고 설정

## [!UICONTROL Insert Ad Tag]

*새로운 모바일 비디오 광고 형식만*

**[!UICONTROL URL]** 또는 **[!UICONTROL Ad Tag]**: 크리에이티브 에셋 및 추적 픽셀을 포함하는 서드파티 VAST 광고 태그 또는 광고 태그

**[!UICONTROL Ad Title]** 또는 **[!UICONTROL Title]**: 다음에 사용되는 광고 이름 [!UICONTROL Ads] 및 보고서를 봅니다.

>[!TIP]
>
> VAST 태그의 유효성을 검사하려면 브라우저에 붙여 넣고 **[!UICONTROL Enter]** 키. 태그가 유효하면 다음을 포함하는 XML 파일이 표시됩니다 `<VAST>` 꼭대기 근처에 있습니다.

## [!UICONTROL Ad Options]

### [!UICONTROL Basic]: 모바일 디스플레이 광고

**[!UICONTROL Ad Type]:** (읽기 전용) 광고를 첨부할 수 있는 배치 유형에 해당하는 생성 중인 광고 유형입니다.

**[!UICONTROL Ad Name]:** 광고 이름. 에셋 제목은 기본적으로 사용되지만 이름을 변경할 수 있습니다.

>[!TIP]
>
> 광고를 배치에 첨부할 때, 광고 보기에서, 그리고 보고서에서 쉽게 찾을 수 있는 이름을 사용합니다. 예를 들어 단위 유형 및 일부 주요 속성(예: Holiday Product Preview: 300x250 Gamer&quot;)을 설명합니다.

**\[광고 소스\]**: (읽기 전용) *[!UICONTROL 3rd party]*.

**[!UICONTROL Display Code]:** 서드파티 크리에이티브 에셋의 URL. 임의 [timestamp] 및 [[timestamp]] 매개 변수가 실제 값으로 대체됩니다.

**[!UICONTROL Final Display Code]:** 필요한 타사 크리에이티브 에셋의 URL [Advertising DSP 추적 매크로](/help/dsp/campaign-management/macros.md) 해당하는 경우 삽입됩니다.

### [!UICONTROL Basic]: 비디오 광고

**[!UICONTROL Ad Type]:** (읽기 전용) 광고를 첨부할 수 있는 배치 유형에 해당하는 생성 중인 광고 유형입니다.

**[!UICONTROL Ad Name]:** 광고 이름. 에셋 제목은 기본적으로 사용되지만 이름을 변경할 수 있습니다.

>[!TIP]
>
> 광고를 배치에 첨부할 때, 광고 보기에서, 그리고 보고서에서 쉽게 찾을 수 있는 이름을 사용합니다. 예를 들어 장치 유형과 몇 가지 주요 특성(예: Holiday Product Preview: 30sec Phone Preroll)에 대해 설명합니다.

**[!UICONTROL Width]| [!UICONTROL Ad Unit Width]:** 전체 광고 단위의 너비입니다. 이 옵션은 선택한 광고 단위 유형에 따라 잠길 수 있습니다.

**[!UICONTROL Height]| [!UICONTROL Ad Unit Height]:** 전체 광고 단위의 높이입니다. 이 옵션은 선택한 광고 단위 유형에 따라 잠길 수 있습니다.

**[!UICONTROL Player X]:** 광고 단위에 대한 X 좌표입니다. 기본 설정을 유지합니다.

**[!UICONTROL Player Y]:** 광고 단위에 대한 Y 좌표입니다. 기본 설정을 유지합니다.

**[!UICONTROL Player Width]:** 전체 광고 단위의 너비입니다. 이 옵션은 선택한 광고 단위 유형에 따라 잠길 수 있습니다.

이는 과(와) 동일합니다 **[!UICONTROL Width]** 필드.

**[!UICONTROL Player Height]:** 전체 광고 단위의 높이입니다. 이 옵션은 선택한 광고 단위 유형에 따라 잠길 수 있습니다.

이는 과(와) 동일합니다 **[!UICONTROL Height]** 필드.

**[!UICONTROL Show Controls]:** 광고에 대한 비디오 컨트롤을 포함할 위치: *[!UICONTROL Under]*, *[!UICONTROL Over]*, *[!UICONTROL Bottom]*, 또는 *[!UICONTROL None]* (기본값).

**[!UICONTROL Preserve Aspect Ratio]:** 비디오의 폭 및 높이 비율을 유지할지 여부(*[!UICONTROL Yes]*) 또는 비디오를 늘려 사용 가능한 공간을 채웁니다(*[!UICONTROL No]*).

**[!UICONTROL Close Button Delay]:** (일부 광고 유형) 닫기 버튼의 모양을 지연하는 초 수입니다.

**[!UICONTROL VAST Tag]:** (VAST 태그를 사용하는 광고, 읽기 전용) 크리에이티브 자산으로 입력한 타사 VAST 태그입니다.

**[!UICONTROL Final VAST Tag]:** (VAST 태그를 사용하는 광고, 읽기 전용) 필요한 경우 크리에이티브 자산으로 입력한 타사 VAST 태그 [Advertising DSP 추적 매크로](/help/dsp/campaign-management/macros.md) 해당하는 경우 삽입됩니다.

**[!UICONTROL Wmode]:** (일부 광고 유형) 창 모드: *[!UICONTROL window]*, *[!UICONTROL transparent]*, 또는 *[!UICONTROL opaque]*.

### [!UICONTROL Pixel]

배치에 대한 기존의 모든 이벤트 추적 픽셀은 자동으로 첨부됩니다. 개별 광고에 대한 추적 요구 사항을 기반으로 기존 픽셀을 분리하고 필요에 따라 새 픽셀을 만들 수 있습니다.

다음 설정은 사용자가 만들거나 편집하는 각 픽셀에 적용됩니다.

**[!UICONTROL Integration Event]:** 픽셀을 실행하도록 트리거하는 이벤트입니다. 이 광고 유형의 경우 *[!UICONTROL Impression]* 또는 *[!UICONTROL Click-through]*.

**[!UICONTROL Pixel Type]:** 픽셀이 *[!UICONTROL IMG URL]* (1x1 픽셀 이미지 파일), *[!UICONTROL HTML]*, 또는 *[!UICONTROL JavaScript URL]*.

**[!UICONTROL Pixel URL or Code]:** 지정된 내용에 적합한 형식의 픽셀 이미지 URL [!UICONTROL Pixel Type].

**[!UICONTROL Pixel Name]:** 픽셀 이름. 픽셀을 쉽게 식별하는 데 도움이 되는 이름을 사용합니다.

**[!UICONTROL Pixel Provider]:** 픽셀 공급자: *[!UICONTROL None]*, *[!UICONTROL Nielsen]*, 또는 *[!UICONTROL Comscore]*.

### [!UICONTROL Sharing]

더 이상 사용되지 않음

>[!MORELIKETHIS]
>
>* [광고 관리 기본 정보](ad-about.md)
>* [단일 광고 만들기](ad-create.md)
>* [광고와 연결된 배치 나열](/help/dsp/campaign-management/ads/ad-list-placements.md)
>* [광고 사양](ad-specs.md)
>* [DSP 매크로](/help/dsp/campaign-management/macros.md)

