---
title: 연결된 TV 광고 설정
description: 연결된 TV 광고에 사용할 수 있는 광고 설정에 대한 설명을 참조하십시오.
feature: DSP Ads
exl-id: d8e47f7e-7480-400f-8ffa-ecf41ce2ebfb
source-git-commit: 863bf7a4d8304e42b7004742de59b9e1a09f81b7
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# 연결된 TV 광고 설정

## [!UICONTROL Insert Ad Tag]

*새 광고만*

**[!UICONTROL URL]**: VAST 태그 URL.

**[!UICONTROL Title]**: 광고 보기 및 보고서에 사용되는 파일의 이름입니다.

>[!TIP]
>
> VAST 태그의 유효성을 검사하려면 브라우저에 붙여 넣고 **[!UICONTROL Enter]** 키를 누르십시오. 태그가 올바른 경우 `<VAST>`을(를) 포함하는 XML 파일이 맨 위에 표시됩니다.

## [!UICONTROL Ad Options]

### [!UICONTROL Basic]

**[!UICONTROL Ad Type]:**(읽기 전용) 만들고 있는 광고 유형으로, 광고를 연결할 수 있는 배치 유형에 해당합니다.

**[!UICONTROL Ad Name]:** 광고 이름입니다. 에셋 제목은 기본적으로 사용되지만 이름을 변경할 수 있습니다.

>[!TIP]
>
> 광고를 게재에 첨부할 때, [!UICONTROL Ads] 보기 및 보고서에서 쉽게 찾을 수 있는 이름을 사용합니다. 예를 들어 단위 유형 및 일부 주요 속성(예: Holiday Product Preview: 30sec CTV&quot;)을 설명합니다.

**[!UICONTROL Width | Ad Unit Width]:** 전체 광고 단위의 너비입니다. 이 옵션은 선택한 광고 단위 유형에 따라 잠길 수 있습니다.

**[!UICONTROL Height | Ad Unit Height]:** 전체 광고 단위의 높이입니다. 이 옵션은 선택한 광고 단위 유형에 따라 잠길 수 있습니다.

**[!UICONTROL Player X]:** 광고 단위에 대한 X 좌표입니다. 기본 설정을 유지합니다.

**[!UICONTROL Player Y]:** 광고 단위에 대한 Y 좌표입니다. 기본 설정을 유지합니다.

**[!UICONTROL Player Width]:** 전체 광고 단위의 너비입니다. 이 옵션은 선택한 광고 단위 유형에 따라 잠길 수 있습니다.

**[!UICONTROL Width]** 필드와 동일합니다.

**[!UICONTROL Player Height]:** 전체 광고 단위의 높이입니다. 이 옵션은 선택한 광고 단위 유형에 따라 잠길 수 있습니다.

**[!UICONTROL Height]** 필드와 동일합니다.

**[!UICONTROL Show Controls]:** 광고에 대한 비디오 컨트롤을 포함할 위치: *[!UICONTROL Under]*, *[!UICONTROL Over]*, *[!UICONTROL Bottom]* 또는 *[!UICONTROL None]*(기본값).

**[!UICONTROL Preserve Aspect Ratio]:** 비디오의 너비 및 높이 비율(*[!UICONTROL Yes]*)을 유지할지, 사용 가능한 공간(*[!UICONTROL No]*)을 채우도록 비디오를 늘릴지 여부를 지정합니다.

**[!UICONTROL VAST Tag]:**(VAST 태그만 사용하는 광고, 읽기 전용) 광고 소스로 입력한 타사 VAST 태그입니다.

**[!UICONTROL Final VAST Tag]:**(VAST 태그만 사용하는 광고, 읽기 전용) 필요한 [Advertising DSP 추적 매크로](/help/dsp/campaign-management/macros.md)가 삽입된 서드파티 VAST 태그입니다(해당하는 경우).

**[!UICONTROL Clock Number]**: (영국에서만 사용되며 권한이 있는 사용자만 사용할 수 있음) 올바른 광고가 브로드캐스트되도록 하는 데 사용되는 고유 식별자입니다. 이 설정을 적용할 수 없으면 비워 둡니다.

### [!UICONTROL Pixel]

<!-- **[!UICONTROL Pixel]:** -->

{{$include /help/_includes/dsp-ad-pixel.md}}

>[!MORELIKETHIS]
>
>* [광고 관리 정보](ad-about.md)
>* [단일 광고 만들기](ad-create.md)
>* [광고에 연결된 배치 나열](/help/dsp/campaign-management/ads/ad-list-placements.md)
>* [광고 사양](ad-specs.md)
>* [DSP 매크로](/help/dsp/campaign-management/macros.md)
