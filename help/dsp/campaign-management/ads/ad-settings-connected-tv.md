---
title: 연결된 TV 광고 설정
description: 연결된 TV 광고에 사용할 수 있는 광고 설정에 대한 설명을 참조하십시오.
feature: DSP Ads
exl-id: d8e47f7e-7480-400f-8ffa-ecf41ce2ebfb
source-git-commit: f521cf26d9d3945bdf1abe4577bb37d732432c87
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# 연결된 TV 광고 설정

## [!UICONTROL Insert Ad Tag]

*새 광고만*

**[!UICONTROL URL]**: VAST 태그 URL.

**[!UICONTROL Title]**: 광고 보기 및 보고서에서 사용할 파일 이름입니다.

>[!TIP]
>
> VAST 태그의 유효성을 검사하려면 브라우저에 붙여 넣고 **[!UICONTROL Enter]** 키. 태그가 유효하면 다음을 포함하는 XML 파일이 표시됩니다 `<VAST>` 꼭대기 근처에 있습니다.

## [!UICONTROL Ad Options]

### [!UICONTROL Basic]

**[!UICONTROL Ad Type]:** (읽기 전용) 광고를 첨부할 수 있는 배치 유형에 해당하는 생성 중인 광고 유형입니다.

**[!UICONTROL Ad Name]:** 광고 이름. 에셋 제목은 기본적으로 사용되지만 이름을 변경할 수 있습니다.

>[!TIP]
>
> 에서 광고를 배치에 첨부할 때 쉽게 찾을 수 있는 이름을 사용합니다. [!UICONTROL Ads] 보고서에서 및 를 봅니다. 예를 들어 단위 유형 및 일부 주요 속성(예: Holiday Product Preview: 30sec CTV&quot;)을 설명합니다.

**[!UICONTROL Width | Ad Unit Width]:** 전체 광고 단위의 너비입니다. 이 옵션은 선택한 광고 단위 유형에 따라 잠길 수 있습니다.

**[!UICONTROL Height | Ad Unit Height]:** 전체 광고 단위의 높이입니다. 이 옵션은 선택한 광고 단위 유형에 따라 잠길 수 있습니다.

**[!UICONTROL Player X]:** 광고 단위에 대한 X 좌표입니다. 기본 설정을 유지합니다.

**[!UICONTROL Player Y]:** 광고 단위에 대한 Y 좌표입니다. 기본 설정을 유지합니다.

**[!UICONTROL Player Width]:** 전체 광고 단위의 너비입니다. 이 옵션은 선택한 광고 단위 유형에 따라 잠길 수 있습니다.

이는 과(와) 동일합니다 **[!UICONTROL Width]** 필드.

**[!UICONTROL Player Height]:** 전체 광고 단위의 높이입니다. 이 옵션은 선택한 광고 단위 유형에 따라 잠길 수 있습니다.

이는 과(와) 동일합니다 **[!UICONTROL Height]** 필드.

**[!UICONTROL Show Controls]:** 광고에 대한 비디오 컨트롤을 포함할 위치: *[!UICONTROL Under]*, *[!UICONTROL Over]*, *[!UICONTROL Bottom]*, 또는 *[!UICONTROL None]* (기본값).

**[!UICONTROL Preserve Aspect Ratio]:** 비디오의 폭 및 높이 비율을 유지할지 여부(*[!UICONTROL Yes]*) 또는 비디오를 늘려 사용 가능한 공간을 채웁니다(*[!UICONTROL No]*).

**[!UICONTROL VAST Tag]:** (VAST 태그를 사용하는 광고, 읽기 전용) 광고 소스로 입력한 타사 VAST 태그입니다.

**[!UICONTROL Final VAST Tag]:** (VAST 태그를 사용하는 광고, 읽기 전용) 필요한 와 함께 광고 소스로 입력한 타사 VAST 태그 [Advertising DSP 추적 매크로](/help/dsp/campaign-management/macros.md) 해당하는 경우 삽입됩니다.

**[!UICONTROL Clock Number]**: (영국에서만 사용되며, 권한이 있는 사용자만 사용할 수 있음) 올바른 광고가 브로드캐스트되도록 하는 데 사용되는 고유 식별자입니다. 이 설정을 적용할 수 없으면 비워 둡니다.

### [!UICONTROL Pixel]

배치에 대한 기존의 모든 이벤트 추적 픽셀은 자동으로 첨부됩니다. 개별 광고에 대한 추적 요구 사항을 기반으로 기존 픽셀을 분리하고 필요에 따라 새 픽셀을 만들 수 있습니다.

다음 설정은 사용자가 만들거나 편집하는 각 픽셀에 적용됩니다.

**[!UICONTROL Integration Event]:** 픽셀을 실행하도록 트리거하는 이벤트입니다. 이 광고 유형의 경우 *[!UICONTROL Impression]* 또는 *[!UICONTROL Click-through]*.

**[!UICONTROL Pixel Type]:** 픽셀이 *[!UICONTROL IMG URL]* (1x1 픽셀 이미지 파일), *[!UICONTROL HTML]*, 또는 *[!UICONTROL JavaScript URL]*.

**[!UICONTROL Pixel URL or Code]:** 지정된 픽셀 유형에 적절한 형식의 픽셀 이미지 URL입니다.

**[!UICONTROL Pixel Name]:** 픽셀 이름. 픽셀을 쉽게 식별하는 데 도움이 되는 이름을 사용합니다.

**[!UICONTROL Pixel Provider]:** 픽셀 공급자: *[!UICONTROL None]*, *[!UICONTROL Comscore]*, *[!UICONTROL WhiteOps]*, 또는 *[!UICONTROL IAS]*.

>[!MORELIKETHIS]
>
>* [광고 관리 기본 정보](ad-about.md)
>* [단일 광고 만들기](ad-create.md)
>* [광고와 연결된 배치 나열](/help/dsp/campaign-management/ads/ad-list-placements.md)
>* [광고 사양](ad-specs.md)
>* [DSP 매크로](/help/dsp/campaign-management/macros.md)
