---
title: 프리롤 광고 설정
description: 프리롤 광고에 사용할 수 있는 광고 설정에 대한 설명을 참조하십시오.
feature: DSP Ads
exl-id: d0ba4346-13ae-405c-92b6-a0c32dd09d0a
source-git-commit: 2f137b17deea4cd02ae19494a306ff37c7002423
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 0%

---

# 프리롤 광고 설정

## [!UICONTROL Insert Ad Tag]

*새 광고만*

**[!UICONTROL URL]:** VAST 태그 URL입니다.

**[!UICONTROL Title]:** [!UICONTROL Ads] 보기 및 보고서에 있는 파일의 제목입니다.

>[!TIP]
>
> VAST 태그의 유효성을 검사하려면 브라우저에 붙여 넣고 **[!UICONTROL Enter]** 키를 누르십시오. 태그가 올바른 경우 `<VAST>`을(를) 포함하는 XML 파일이 맨 위에 표시됩니다.

## [!UICONTROL Ad Options]

### [!UICONTROL Basic]

**[!UICONTROL Ad Type]:**(읽기 전용) 만들고 있는 광고 유형으로, 광고를 연결할 수 있는 배치 유형에 해당합니다.

**[!UICONTROL Ad Name]:** 광고 이름입니다. 에셋 제목은 기본적으로 사용되지만 이름을 변경할 수 있습니다.

>[!TIP]
>
> 광고를 게재에 첨부할 때, [!UICONTROL Ads] 보기 및 보고서에서 쉽게 찾을 수 있는 이름을 사용합니다. 예를 들어 단위 유형 및 일부 주요 속성(예: Holiday Product Preview: 30sec Preroll)에 대해 설명합니다.

**[!UICONTROL Width]| [!UICONTROL Ad Unit Width]:**(표준 및 스킵할 수 있는 프리롤 광고만 해당) 전체 광고 단위의 너비입니다. 이 옵션은 선택한 광고 단위 유형에 따라 잠길 수 있습니다.

**[!UICONTROL Height]| [!UICONTROL Ad Unit Height]:**(표준 및 스킵할 수 있는 프리롤 광고만 해당) 전체 광고 단위의 높이입니다. 이 옵션은 선택한 광고 단위 유형에 따라 잠길 수 있습니다.

**[!UICONTROL Player X]:** 광고 단위에 대한 X 좌표입니다. 기본 설정을 유지합니다.

**[!UICONTROL Player Y]:** 광고 단위에 대한 Y 좌표입니다. 기본 설정을 유지합니다.

**[!UICONTROL Player Width]:** 전체 광고 단위의 너비입니다. 이 옵션은 선택한 광고 단위 유형에 따라 잠길 수 있습니다.

이 필드는 **[!UICONTROL Width]** 필드와 동일합니다.

**[!UICONTROL Player Height]:** 전체 광고 단위의 높이입니다. 이 옵션은 선택한 광고 단위 유형에 따라 잠길 수 있습니다.

**[!UICONTROL Height]** 필드와 동일합니다.

**[!UICONTROL Show Controls]:** 광고에 대한 비디오 컨트롤을 포함할 위치: *[!UICONTROL Under]*, *[!UICONTROL Over]*, *[!UICONTROL Bottom]* 또는 *[!UICONTROL None]*(기본값).

**[!UICONTROL Preserve Aspect Ratio]:** 비디오의 너비 및 높이 비율(*[!UICONTROL Yes]*)을 유지할지 또는 비디오를 늘려 사용 가능한 공간(*[!UICONTROL No]*)을 채울지 여부를 지정합니다.

**[!UICONTROL VAST Tag]:**(VAST 태그만 사용하는 광고, 읽기 전용) 광고 소스로 입력한 타사 VAST 태그입니다.

**[!UICONTROL Final VAST Tag]:**(VAST 태그만 사용하는 광고, 읽기 전용) 필요한 [Advertising DSP 추적 매크로](/help/dsp/campaign-management/macros.md)가 삽입된 서드파티 VAST 태그입니다(해당하는 경우).

**[!UICONTROL Wmode]:**(대화형 프리롤 전용) 창 모드: *[!UICONTROL window]*, *[!UICONTROL transparent]* 또는 *[!UICONTROL opaque]*.

**[!UICONTROL Video Format]:**(대화형 프리롤만 해당) 잠재적인 인벤토리에 대한 광고 플레이어의 형식: *[!UICONTROL VPAID]* 또는 *[!UICONTROL VPAID & VAST]*. 항상 VPAID에 대해 가시성이 측정되지만, VPAID 및 VAST에는 가시성 측정을 허용하지 않는 재고가 포함됩니다. 조회 지표가 캠페인에 중요한 경우 이 구분을 고려하십시오.

**[!UICONTROL Clock Number]**: (대화형 프리롤 전용, 영국에서만 사용, 권한이 있는 사용자만 사용) 올바른 광고가 브로드캐스트되도록 하는 데 사용되는 고유 식별자입니다. 이 설정을 적용할 수 없으면 비워 둡니다.

### [!UICONTROL Pixel]

배치에 대한 기존의 모든 이벤트 추적 픽셀은 자동으로 첨부됩니다. 개별 광고에 대한 추적 요구 사항을 기반으로 기존 픽셀을 분리하고 필요에 따라 새 픽셀을 만들 수 있습니다. **팁:** [!UICONTROL Ad Tools] 보기를 사용하여 한 번에 배치의 여러 광고에 대한 타사 추적 픽셀을 편집하려면 &quot;[배치에 타사 추적 픽셀 첨부](/help/dsp/campaign-management/ads/ad-attach-to-placement.md#attach-pixels-ads)&quot;를 참조하십시오.

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
>* [광고에 연결된 배치 나열](/help/dsp/campaign-management/ads/ad-list-placements.md)
>* [광고 사양](ad-specs.md)
>* [DSP 매크로](/help/dsp/campaign-management/macros.md)
