---
title: 동적 크리에이티브 설정
description: 동적 크리에이티브에 대한 설정을 참조하십시오.
feature: Creative Dynamic Creatives
source-git-commit: 31651c4e30d22b4d1639ef3fc05d5ff9e02dd040
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# 동적 크리에이티브 설정

<!-- add a description -->

<!-- This looks the same for me for either HTML5 type as of 9/24:

## Dynamic ad settings for static HTML5 ads {#dynamic-ad-settings-static-html5}

### Basic Details

**[!UICONTROL Advertiser]:** The advertiser for which to create the ads.

**[!UICONTROL Library]:** The creative library in which to create the ads.

**[!UICONTROL Dynamic Ad Name]:** A unique name for the creative.

**[!UICONTROL Ad Template Size]:** The ad dimensions for the ad template from which to create the ad. If you first select a specific [!UICONTROL Ad Template], then this value is automatically selected.

**[!UICONTROL Ad Template Type]:** The type of ad template from which to create the ad: *[!UICONTROL Static HTML5]* or *[!UICONTROL Dynamic HTML5]*.  If you first select a specific [!UICONTROL Ad Template], then this value is automatically selected.

**[!UICONTROL Ad Template]:** The ad template from which to create the ad.

**[!UICONTROL clickURL]:** A valid landing page URL to which users are redirected when they click the ad.

### [!UICONTROL Attributes Details]

-->

## 동적 광고 설정<!-- for dynamic HTML5 ads {#dynamic-ad-settings-dynamic-html5}-->

<!-- add a description -->

### 기본 세부 정보

**[!UICONTROL Dynamic Ad Name]:** 크리에이티브의 고유한 이름입니다.

**[!UICONTROL Advertiser]:** 광고를 만들 광고주입니다.

**[!UICONTROL Library]:** 광고를 만들 크리에이티브 라이브러리입니다. [!UICONTROL Creatives] > [!UICONTROL Creative Libraries] 내에서 광고를 만드는 경우 라이브러리 이름이 이미 선택되고 읽기 전용입니다.

**[!UICONTROL Ad Template Size]:** 광고를 만들 광고 템플릿에 대한 [광고 차원](/help/creative/creative-libraries/creative-sizes.md)입니다. 먼저 특정 [!UICONTROL Ad Template]을(를) 선택하면 이 값이 자동으로 선택됩니다.

## 광고 템플릿

**[!UICONTROL Ad Template]:** 광고를 만들 광고 템플릿입니다. 기존 광고 템플릿을 선택하거나 새 광고 템플릿을 업로드하고 템플릿 유형(*정적* 또는 *동적*)을 선택하십시오. 업로드된 템플릿은 ZIP 형식이어야 하며 HTML5 파일과 템플릿 정의 파일(template.TDF)을 포함해야 합니다. <!-- Need to add more specs for that -->

**[!UICONTROL Number of offers (Max 50)]:** 회전판에 표시할 제품 수입니다.

## 카탈로그

**[!UICONTROL Template]:** 광고를 만드는 데 사용할 피드 템플릿입니다.

**\[Catalogs\]**: 광고를 생성할 하나 이상의 카탈로그. 기존 카탈로그를 선택하거나 기존 피드 템플릿을 다운로드하고 새 카탈로그를 만들어 업로드하여 새 카탈로그를 만드십시오.

업로드된 카탈로그는 ZIP 형식이어야 하며, 다음과 같은 내용을 포함해야 합니다.

* CSV, TSV 또는 Microsoft Excel 스프레드시트(XLSX) 형식의 피드 파일이 하나 이상 있습니다.<!-- Need to add more specs for that -->

* GIF, JPEG, JPG 또는 PNG 형식의 이미지 자산

* (선택 사항) MP4 또는 WEBM 형식의 비디오 자산

### [!UICONTROL Attributes Mapping]

**[!UICONTROL Enable targeting]**: <!-- "targeting options/filters," but I don't think this means user targeting since that is set in the experience/ad on DSP -->피드 파일에 광고를 만들려면 값이 있어야 하는 열 형식: *[!UICONTROL Profile data]*, *[!UICONTROL Geographic data], *[!UICONTROL Data pass], *[!UICONTROL Audience Segment]*.  **참고:** 이러한 설정은 광고 경험 설정의 고급 설정과 독립적으로 작동합니다.<!-- Clarify what qualifies for each, and explain more -->

**[!UICONTROL Dynamic Ad Fields]** / **[!UICONTROL Maps to Catalog Labels]:**

지정된 광고 템플릿의 각 속성(동적 광고 필드)을 지정된 카탈로그(카탈로그 레이블)의 열에 매핑하거나 정적 값을 입력합니다.

>[!MORELIKETHIS]
>
>* [Creative 라이브러리에 동적 크리에이티브 추가](creative-add-dynamic.md)
>* [Creative 라이브러리에서 동적 크리에이티브 편집](creative-edit-dynamic.md)
>* [동적 광고용 워크플로](/help/creative/introduction/workflow-dynamic-ads.md)
