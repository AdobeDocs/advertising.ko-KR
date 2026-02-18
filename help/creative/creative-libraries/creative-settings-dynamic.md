---
title: 동적 크리에이티브 설정
description: 동적 크리에이티브에 대한 설정을 참조하십시오.
feature: Creative Dynamic Creatives
exl-id: 9dcd7245-fa02-4082-9abb-8c0792322a68
source-git-commit: 4e809ac18720f22f636b2df2ad4a5b1db355e729
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# 동적 크리에이티브 설정

<!-- add a description -->

## 동적 광고 설정<!-- for dynamic HTML5 ads {#dynamic-ad-settings-dynamic-html5}-->

<!-- add a description -->

### 기본 세부 정보

**[!UICONTROL Creative Type]:** 크리에이티브가 *[!UICONTROL Display]* 광고(HTML5)인지 *[!UICONTROL Video]* 광고인지 여부.

**[!UICONTROL Dynamic Display Ad Name]** 또는 **[!UICONTROL Dynamic Video Ad Name]:** 크리에이티브의 고유한 이름입니다.

**[!UICONTROL Advertiser]:** 광고를 만들 광고주입니다. [!UICONTROL Creatives] > [!UICONTROL Creative Libraries] 내에서 광고를 만드는 경우 광고주가 이미 선택되고 읽기 전용입니다.

**[!UICONTROL Library]:** 광고를 만들 크리에이티브 라이브러리입니다. [!UICONTROL Creatives] > [!UICONTROL Creative Libraries] 내에서 광고를 만드는 경우 라이브러리 이름이 이미 선택되고 읽기 전용입니다.

**[!UICONTROL Ad Template Size]:**(동적 디스플레이 광고 전용) 광고를 만들 광고 템플릿의 [광고 차원](/help/creative/creative-libraries/creative-sizes.md)입니다. 먼저 특정 [!UICONTROL Ad Template]을(를) 선택하면 이 값이 자동으로 선택됩니다.

## 광고 템플릿

**[!UICONTROL Ad Template]:** 광고를 만들 광고 템플릿입니다. 기존 광고 템플릿을 선택하거나 새 광고 템플릿을 업로드하고 템플릿 유형(*정적* 또는 *동적*)을 선택하십시오. 템플릿은 ZIP 형식이어야 하며 다음 항목을 포함해야 합니다. <!-- Need to add more specs for templates -->

* 광고 크리에이티브 표시: 원하는 광고 형식을 갖는 HTML5 파일과 (동적 HTML5 광고만 해당) 광고 속성(.tdf)이 있는 파일

* 비디오 크리에이티브: 원하는 광고 형식의 .scene 파일입니다. ZIP 파일은 최대 512MB일 수 있습니다.

계속하려면 **[!UICONTROL Select Ad Template]**&#x200B;을(를) 클릭하십시오.

**[!UICONTROL Card Count (Max 50)]:**(광고만 표시) 회전판에 표시할 제품 수입니다.

**[!UICONTROL Duration]:**(비디오 광고 전용, 읽기 전용) 선택한 광고 템플릿에서 파생된 비디오 기간입니다. 각 비디오의 재생 시간은 1~90초 사이여야 합니다.

## 카탈로그

**[!UICONTROL Template]:** 광고를 만드는 데 사용할 피드 템플릿입니다.

**\[Catalogs\]**: 광고를 생성할 하나 이상의 카탈로그. 기존 카탈로그를 선택하거나 기존 피드 템플릿을 다운로드하고 새 카탈로그를 만들어 업로드하여 새 카탈로그를 만드십시오. **[!UICONTROL Select Catalog]**&#x200B;을(를) 클릭합니다.

업로드된 카탈로그는 ZIP 형식이어야 하며, 다음과 같은 내용을 포함해야 합니다.

* (동적 디스플레이 및 비디오 광고) CSV, TSV 또는 Microsoft Excel 스프레드시트(XLSX) 형식의 피드 파일이 하나 이상 있습니다. 최대 파일 크기는 512MB입니다.<!-- Need to add more specs for the feed files -->

* (디스플레이 광고) GIF, JPEG, JPG 또는 PNG 형식의 이미지 자산

* (비디오 광고) MP4, MOV 또는 WEBM 형식의 비디오 자산. 지원되는 광고 템플릿에는 시작 카드, 끝 카드, 상단 오버레이, 하단 오버레이 또는 L자형 등이 있습니다. 각 비디오의 재생 시간은 1~90초 사이여야 합니다.

### [!UICONTROL Attributes Mapping]

**[!UICONTROL Enable targeting]**: <!-- "targeting options/filters," but I don't think this means user targeting since that is set in the experience/ad on DSP -->피드 파일에 광고를 만들려면 값이 있어야 하는 열 형식: *[!UICONTROL Profile data]*, *[!UICONTROL Geographic data], *[!UICONTROL Data pass], *[!UICONTROL Audience Segment]*.  **참고:** 이러한 설정은 광고 경험 설정의 고급 설정과 독립적으로 작동합니다.<!-- Clarify what qualifies for each, and explain more -->

**[!UICONTROL Dynamic Ad Fields]** / **[!UICONTROL Maps to Catalog Labels]:**

지정된 광고 템플릿의 각 속성(동적 광고 필드)을 지정된 카탈로그(카탈로그 레이블)의 열에 매핑하거나 정적 값을 입력합니다.

>[!MORELIKETHIS]
>
>* [Creative 라이브러리에 동적 크리에이티브 추가](creative-add-dynamic.md)
>* [Creative 라이브러리에서 동적 크리에이티브 편집](creative-edit-dynamic.md)
>* [동적 광고용 워크플로](/help/creative/introduction/workflow-dynamic-ads.md)
