---
title: 오디오 광고 설정
description: 오디오 광고에 사용할 수 있는 광고 설정에 대한 설명을 참조하십시오.
feature: DSP Ads
exl-id: 2fa1143b-6e83-4729-91cd-7a5da357509e
source-git-commit: 4b9cc5956d573b346eacdf71a8ea490c162b4660
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# 오디오 광고 설정

## [!UICONTROL Insert Ad Tag]

*새 광고만*

**[!UICONTROL URL]**: VAST 태그 URL.

**[!UICONTROL Title]**: [!UICONTROL Ads] 보기 및 보고서에 사용되는 파일 이름입니다.

>[!TIP]
>
> VAST 태그의 유효성을 검사하려면 브라우저에 붙여 넣고 **[!UICONTROL Enter]** 키를 누르십시오. 태그가 올바른 경우 `<VAST>`을(를) 포함하는 XML 파일이 맨 위에 표시됩니다.

## [!UICONTROL Ad Options]

### [!UICONTROL Basic]

**[!UICONTROL Ad Type]:**(읽기 전용) 만들고 있는 광고 유형으로, 광고를 연결할 수 있는 배치 유형에 해당합니다. 기본값은 *[!UICONTROL Audio]*&#x200B;입니다.

**[!UICONTROL Ad Name]:** 광고 이름입니다. 에셋 제목은 기본적으로 사용되지만 이름을 변경할 수 있습니다.

>[!TIP]
>
> 광고를 게재에 첨부할 때, [!UICONTROL Ads] 보기 및 보고서에서 쉽게 찾을 수 있는 이름을 사용합니다. 예를 들어 단위 유형 및 일부 주요 속성(예: Holiday Product Preview: 30sec Audio&quot;)을 설명합니다.

**[!UICONTROL Ad Duration]:** 오디오 파일의 길이입니다. 선택한 광고 단위에 따라 [!UICONTROL 15] 또는 [!UICONTROL 30] 중 하나로 자동 설정됩니다.

이 필드는 계정 권한에 따라 표시될 수도 있고 표시되지 않을 수도 있습니다.

**[!UICONTROL VAST Tag]:**(VAST 태그를 사용하는 광고 전용) 타사 광고 소스에 대한 URL입니다. VAST 태그에 오디오 미디어 파일만 포함되어 있는지 확인합니다.

**[!UICONTROL Final VAST Tag]:**(VAST 태그를 사용하는 광고 전용) 필요한 [Advertising DSP 추적 매크로](/help/dsp/campaign-management/macros.md)가 삽입된 타사 광고 소스의 URL입니다(해당하는 경우).

**[!UICONTROL Select Rate]:**(사용 권한만 있는 사용자) Adobe을 통해 청구된 사전 협상된 요금이거나 공급업체를 통해 협상되고 청구된 요금 중 하나입니다. 요금을 추가하려면 Adobe 계정 팀에 문의하십시오.

### [!UICONTROL Pixel]

배치에 대한 기존의 모든 이벤트 추적 픽셀은 자동으로 첨부됩니다. 개별 광고에 대한 추적 요구 사항을 기반으로 기존 픽셀을 분리하고 필요에 따라 새 픽셀을 만들 수 있습니다. **팁:** [!UICONTROL Ad Tools] 보기를 사용하여 한 번에 배치의 여러 광고에 대한 타사 추적 픽셀을 편집하려면 &quot;[배치에 타사 추적 픽셀 첨부](/help/dsp/campaign-management/ads/ad-attach-to-placement.md#attach-pixels-ads)&quot;를 참조하십시오.

다음 설정은 사용자가 만들거나 편집하는 각 픽셀에 적용됩니다.

**[!UICONTROL Integration Event]:** 픽셀을 실행하도록 트리거하는 이벤트입니다. 이 광고 유형의 경우 *[!UICONTROL Impression]* 또는 *[!UICONTROL Click-through]*&#x200B;에서 실행되는 픽셀을 사용하십시오.

**[!UICONTROL Pixel Type]:** 픽셀이 *[!UICONTROL IMG URL]*(1x1 픽셀 이미지 파일), *[!UICONTROL HTML]* 또는 *[!UICONTROL JavaScript URL]*&#x200B;인지 여부.

**[!UICONTROL Pixel URL or Code]:** 지정된 픽셀 유형에 적절한 형식의 픽셀 이미지 URL입니다.

**[!UICONTROL Pixel Name]:** 픽셀 이름입니다. 픽셀을 쉽게 식별하는 데 도움이 되는 이름을 사용합니다.

**[!UICONTROL Pixel Provider]:** 픽셀 공급자:*[!UICONTROL None]*, *[!UICONTROL Comscore]*, *[!UICONTROL WhiteOps]* 또는 *[!UICONTROL IAS]*.

>[!MORELIKETHIS]
>
>* [광고 관리 정보](ad-about.md)
>* [단일 광고 만들기](ad-create.md)
>* [광고에 연결된 배치 나열](/help/dsp/campaign-management/ads/ad-list-placements.md)
>* [광고 사양](ad-specs.md)
>* [DSP 매크로](/help/dsp/campaign-management/macros.md)
