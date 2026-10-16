---
title: Creative Studio에서 광고 템플릿 관리
description: Adobe Advertising Creative에서 광고 템플릿을 만들고, 가져오고, 구성하고, 관리하는 방법을 알아봅니다.
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: d0d9f2ed-c163-44e1-97a1-4ace121416b8
    internal-label: Creative
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 8fa8d6c66228d3a0af1de2514dd016d8f50262e8
workflow-type: tm+mt
source-wordcount: '3702'
ht-degree: 1%
---
# [!UICONTROL Creative Studio]에서 광고 템플릿 관리

광고 생성 세션에서 사용할 디스플레이 및 비디오 광고 템플릿을 만들고 가져오고 관리합니다.

## [!UICONTROL Creative Studio] > [!UICONTROL Templates] 보기

**[!UICONTROL Templates]** 탭은 새 광고 템플릿을 만들거나 가져오는 빠른 작업을 제공합니다.

[!UICONTROL Templates] 탭에는 <!-- Only in the Templates tab --> 페이지 하단에 기존 광고 템플릿이 [개별 카드(기본값) 또는 테이블/목록](/help/creative/introduction/customize-data-views.md) 형식으로 나열됩니다. 광고 템플릿 목록에는 [!UICONTROL All], [!UICONTROL System Templates]&#x200B;(Adobe 계정 팀이 계정에 업로드하는 항목) 및 [!UICONTROL User Templates]에 대한 탭이 포함되어 있습니다. 기본적으로 모든 광고주에 대한 광고 템플릿이 표시됩니다. 특정 광고주에 대한 광고 템플릿만 보려면 페이지 상단의 광고주 목록에서 를 선택합니다.

<!--
Probably not necessary:

* **[!UICONTROL Card view]** &mdash; Displays templates as cards. Each card shows a preview thumbnail and the ad dimensions. Hovering a card reveals action controls.

* **[!UICONTROL Table view]** &mdash; Displays templates in a table with columns for **[!UICONTROL Name]**, **[!UICONTROL Type]**, **[!UICONTROL Status]**, **[!UICONTROL Size/Duration]**, **[!UICONTROL Advertiser]**, and **[!UICONTROL Updated]**. Click the **[!UICONTROL Name]** or **[!UICONTROL Updated]** column header to sort ascending or descending. Pagination controls appear at the bottom of the list.
-->

### 사용 가능한 작업

<!--  Figure out how to handle these, which relate to the template list at the bottom of the page: * [Browse and search templates](#browse-search) -->

생성:

* [AI를 사용하여 광고 템플릿 생성](#template-generate)

* [광고 템플릿 수동으로 만들기](#template-create)

* [HTML5 광고 템플릿 가져오기](#templates-import)

기존 템플릿에 대한 작업:

* [디스플레이 광고 템플릿에서 광고 변형 생성](#ad-variations-generate)

* [광고 템플릿 편집](#template-edit)

* [광고 템플릿에 대한 레이블 추가 또는 제거](#template-labels)

* [광고 템플릿 미리 보기](#template-preview)

* [광고 템플릿 다운로드](#template-download)

* [즐겨찾기로 광고 템플릿 추가 또는 제거](#template-favorite)

* [광고 템플릿 삭제](#template-delete)

<!--

Move to a Common Tasks chapter:

## Browse and search templates {#browse-search}

### Search

Type in the **[!UICONTROL Search templates]** field and press **[!UICONTROL Enter]** to find templates by name. Click the **[!UICONTROL Clear search]** button to reset.

### Filter by source

Use the filter pills in the toolbar to show a subset of templates:

* **[!UICONTROL All]** &mdash; Shows all templates.
* **[!UICONTROL System Templates]** &mdash; Shows Adobe-provided templates only.
* **[!UICONTROL User Templates]** &mdash; Shows templates you or your team have created or imported.

### Filter by status or format

1. In the main menu, click **[!UICONTROL Creative Studio].**

1. Click the **[!UICONTROL Templates]** tab.

1. Click **[!UICONTROL Filter]** in the toolbar.

1. In the **[!UICONTROL Filters]** dialog, select a filter category:

   * **[!UICONTROL Status]:** Filter by **[!UICONTROL Live]** or **[!UICONTROL Draft]**.
   * **[!UICONTROL Ad Format]:** Filter by **[!UICONTROL Display]** or **[!UICONTROL Video]**.

1. Select one or more options in the category, then click **[!UICONTROL Apply]**.

Applied filters appear as chips below the toolbar. To refine or remove an active filter, click its chip to open a popover where you can toggle options, then click **[!UICONTROL Apply]** or **[!UICONTROL Delete]** to remove the filter. To remove all active filters at once, click **[!UICONTROL Clear All]**.

-->

## AI를 사용하여 광고 템플릿 생성 {#template-generate}

*Beta 기능*

[!UICONTROL Creative Studio]의 AI를 사용하여 기존 정적 디스플레이 광고 이미지를 편집 가능한 디스플레이 광고 템플릿으로 변환합니다. 3단계 마법사를 사용하면 템플릿을 생성 및 검토하고 자연어를 사용하여 변경 사항을 요청하고 템플릿 편집기를 열어 수동으로 변경하고 템플릿을 저장할 수 있습니다.

### 사전 요구 사항

Creative 라이브러리에 정적 이미지 광고가 필요합니다. 이 워크플로는 라이브러리에서 광고를 선택합니다. 생성 대화 상자에서 직접 새 이미지를 업로드하지 않습니다.

<!--

Publish this when prompt-based generation becomes available:

To generate a template from an existing image, you need a static image ad in a Creative Library. This option selects ads from your libraries; it doesn't upload a new image directly in the generation dialog. You don't need an existing ad image to generate a template from a prompt.

-->

### 1단계: 템플릿 생성 및 검토

1. 주 메뉴에서 **[!UICONTROL Creative Studio]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Templates]** 탭을 클릭합니다.

1. (선택 사항) 페이지 상단의 광고주 목록에서 광고주를 선택하여 해당 광고주의 라이브러리를 확인합니다.

1. **[!UICONTROL Use AI to Generate a New Display Ad Template]** 상자에서 **[!UICONTROL Generate]**&#x200B;을(를) 클릭합니다.

1. 아직 선택하지 않은 경우 **[!UICONTROL Generate New Ad Template]** 대화 상자에서 **[!UICONTROL Generate from Existing Standard Ad Image]**&#x200B;을(를) 선택합니다.

1. **[!UICONTROL Ad Library]** 목록에서 이미지 광고가 포함된 라이브러리를 선택합니다.

1. 이미지 광고 카드 위에 커서를 놓고 **[!UICONTROL Use this Standard Ad]**&#x200B;을(를) 클릭합니다.

   선택한 광고의 폭과 높이를 사용하여 자동으로 생성이 시작됩니다.

<!--

Switch to this when prompt-based generation becomes available:

1. In the **[!UICONTROL Generate New Ad Template]** dialog, choose how to generate the template:

   * **[!UICONTROL Generate from Prompt]:** Describe the ad template you want to create using a text prompt.

   * **[!UICONTROL Generate from Existing Standard Ad Image]:** Convert an existing static image ad into an editable template.

1. Follow the steps for your selected option:

   * From a prompt:

      1. Enter a description of the template you want to create. Include details such as the layout, headline, call to action, and visual style.

      1. Follow the on-screen instructions to generate the template.

   * From an existing standard ad image:

      1. Select the library containing the image ad from the **[!UICONTROL Ad Library]** list.

      1. Hold the cursor over the image ad card and click **[!UICONTROL Use this Standard Ad]**.

         Generation begins automatically, using the selected ad's width and height.

-->

1. [생성된 템플릿을 검토하고 세분화합니다](#template-review).

### 2단계: 템플릿 검토 및 세분화 {#template-review}

1. 생성이 완료될 때까지 기다린 다음 템플릿 미리 보기 및 **[!UICONTROL Layers]** 패널을 검토합니다(사용 가능한 경우).

   템플릿을 사용하기 전에 텍스트, 이미지 및 레이아웃을 확인하십시오. 여기에 표시된 레이어는 검토용입니다. 템플릿 편집기에서 수동으로 변경하십시오.

1. (선택 사항) 생성된 템플릿에 대한 요청 변경 사항:

   1. **[!UICONTROL Ask the AI for any changes]** 필드에서 원하는 변경 내용을 설명합니다. 예를 들어 `Change the headline to "Limited Time Offer" and the button text to "Shop Now"`을(를) 입력합니다.

   1. **[!UICONTROL Regenerate]**&#x200B;을(를) 클릭합니다.

   1. 업데이트된 미리보기를 검토합니다. 필요에 따라 반복합니다.

1. 계속할 준비가 되면 **[!UICONTROL Use this Ad Template]**&#x200B;을(를) 클릭합니다.

   생성된 템플릿이 디스플레이 템플릿 편집기에서 열립니다.

### 3단계: 템플릿 편집 및 저장 {#template-save}

>[!TIP]
>
> AI 어시스턴트는 오픈 소스 글꼴 라이브러리를 사용하여 광고에서 글꼴과 일치하는 항목을 찾습니다. 사용자 고유의 글꼴을 사용하려면 [!UICONTROL Assets] 탭이나 템플릿 편집기에서 업로드한 다음 편집기에서 생성된 글꼴을 바꾸십시오.
>
> 최상의 결과를 얻으려면 AI가 생성한 로고를 템플릿 편집기에서 원본 픽셀 단위 완벽한 로고로 바꾸십시오.

1. 템플릿 편집기에서 생성된 요소를 검토하고 [템플릿 편집기 컨트롤](#template-controls)을 사용하여 나머지 변경 작업을 수행합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Update Template]** 대화 상자에서 **[!UICONTROL Template name]**&#x200B;을(를) 입력하거나 업데이트하고 **[!UICONTROL Advertiser]**&#x200B;을(를) 선택한 다음 선택적으로 태그를 추가합니다.

1. 템플릿을 저장하고 **[!UICONTROL Templates]** 보기로 돌아가려면 **[!UICONTROL Update]**&#x200B;을(를) 클릭합니다.

   대신 별도의 복사본을 저장하려면 **[!UICONTROL Save As New]**&#x200B;을(를) 클릭합니다.

그런 다음 템플릿을 사용하여 [광고 변형을 생성](#ad-variations-generate)할 수 있습니다.

### 템플릿을 생성할 수 없는 경우 {#troubleshooting}

| 문제 | 할 일 |
| --- | --- |
| 이미지에서 생성할 때 라이브러리 또는 이미지 광고가 나열되지 않음 | 선택한 광고주와 **[!UICONTROL Ad Library]**&#x200B;을(를) 확인하십시오. 라이브러리에 표준 광고 이미지가 없는 경우 기존 정적 이미지 광고가 포함된 다른 라이브러리를 선택합니다. |
| 이미지 기반 생성에 실패하거나 이미지를 변환할 수 없음 | 표시된 메시지를 검토하고 **[!UICONTROL Back to library]**&#x200B;을(를) 클릭한 다음 이미지 광고를 선택하여 다시 시도하십시오. |

<!--

Add when prompt-based generation is available:

| Prompt-based generation fails | Review the displayed message and revise your prompt before trying again. |

-->

## 광고 템플릿 수동으로 만들기 {#template-create}

템플릿 편집기를 사용하여 빈 디스플레이 또는 비디오 템플릿을 만듭니다.

1. 주 메뉴에서 **[!UICONTROL Creative Studio].**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Templates]** 탭을 클릭합니다.

1. **[!UICONTROL Create New Ad Template]** 상자에서 **[!UICONTROL Create]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Display Ad Template]** 또는 **[!UICONTROL Video Ad Template]**&#x200B;을(를) 선택합니다.

1. (광고 표시) 광고 템플릿 크기를 선택한 다음 **[!UICONTROL Continue]**&#x200B;을(를) 클릭합니다.

1. 템플릿 편집기의 [컨트롤을 사용하여 템플릿 설정을 구성합니다](#template-controls).

1. (선택 사항) 정의된 대로 템플릿 복사본을 다운로드하려면 **[!UICONTROL ...]** > **[!UICONTROL Download]**&#x200B;을(를) 클릭합니다.

   브라우저의 일반적인 절차에 따라 파일이 다운로드됩니다.

1. 템플릿을 저장합니다.

   1. 다음 중 하나를 수행합니다.

      * **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

      * 템플릿을 초안으로 저장하려면 **[!UICONTROL ...]** > **[!UICONTROL Save as Draft]**&#x200B;을(를) 클릭합니다.

   1. **[!UICONTROL Template name]**&#x200B;을(를) 입력하고 **[!UICONTROL Advertiser]**&#x200B;을(를) 선택한 다음 선택적으로 기존 태그를 선택하거나 템플릿에 새 태그를 추가한 다음 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## HTML5 광고 템플릿 가져오기 {#templates-import}

ZIP 파일로 패키지된 사전 빌드된 HTML5 템플릿을 하나 이상 업로드합니다. 템플릿은 가져올 때 유효성이 검사됩니다. HTML이 200,000자를 초과하거나, CSS가 60,000자를 초과하거나, 템플릿에 5,000개 이상의 DOM 요소가 있거나, 템플릿에 지원되지 않는 스크립트 태그가 포함된 경우 가져오기가 실패합니다.

1. 주 메뉴에서 **[!UICONTROL Creative Studio].**&#x200B;을(를) 클릭합니다.

1. 페이지 맨 위에서 광고주를 선택합니다.

1. **[!UICONTROL Templates]** 탭을 클릭합니다.

1. **[!UICONTROL Upload HTML5 Templates]** 상자에서 **[!UICONTROL Upload]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Display Ad Template]** 또는 **[!UICONTROL Video Ad Template]**&#x200B;을(를) 선택합니다.

1. 장치 또는 네트워크에서 ZIP 파일을 하나 이상 선택합니다.

1. **[!UICONTROL Import Templates]** 대화 상자에서:

   1. **[!UICONTROL Advertiser]** 선택.

      페이지 맨 위에서 특정 광고주를 이미 선택한 경우 해당 광고주가 미리 선택됩니다.

   1. (선택 사항) 각 파일에 대해 **[!UICONTROL Template Name]**&#x200B;을(를) 편집합니다.

      기본적으로 파일 이름이 사용됩니다.

   1. (선택 사항) 파일을 더 추가하려면 **[!UICONTROL Add more]**&#x200B;을(를) 클릭하고 추가 ZIP 파일을 선택하십시오. 각 추가 파일에 대해 **[!UICONTROL Template Name]**&#x200B;을(를) 지정하십시오.

1. **[!UICONTROL Import Templates]**&#x200B;을(를) 클릭합니다.

>[!NOTE]
>
>가져오기에 실패한 경우 템플릿을 단순화하거나 Adobe 계정 팀에 문의하십시오.

## 광고 템플릿 편집 {#template-edit}

*광고 템플릿만 표시합니다.*

>[!IMPORTANT]
>
>AI 에이전트는 템플릿 레이아웃, 요소 위치, 간격 또는 타이포그래피를 변경할 수 없습니다. 콘텐츠를 생성하기 전에 템플릿 편집기에서 구조를 변경합니다.

1. 주 메뉴에서 **[!UICONTROL Creative Studio].**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Templates]** 탭을 클릭합니다.

1. 템플릿 카드 또는 테이블 행 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Edit Template]**&#x200B;을(를) 클릭합니다.

1. 템플릿 편집기의 [컨트롤을 사용하여 템플릿 레이아웃 또는 요소를 편집합니다](#template-controls).

1. (선택 사항) 정의된 대로 템플릿 복사본을 다운로드하려면 **[!UICONTROL ...]** > **[!UICONTROL Download]**&#x200B;을(를) 클릭합니다.

   브라우저의 일반적인 절차에 따라 파일이 다운로드됩니다.

1. 템플릿을 저장합니다.

   * **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

   * 템플릿을 초안으로 저장하려면 **[!UICONTROL ...]** > **[!UICONTROL Save as Draft]**&#x200B;을(를) 클릭합니다. **[!UICONTROL Template name]**&#x200B;을(를) 입력하고 **[!UICONTROL Advertiser]**&#x200B;을(를) 선택한 다음 선택적으로 기존 태그를 선택하거나 템플릿에 새 태그를 추가한 다음 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

<!--

I don't see this anywhere:

1. Click **[!UICONTROL Generate Ad Variations]** to proceed to content generation, or navigate away to save your changes.

-->

## 디스플레이 광고 템플릿에서 광고 변형 생성 {#ad-variations-generate}

*광고 템플릿만 표시합니다.*

1. 주 메뉴에서 **[!UICONTROL Creative Studio].**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Templates]** 탭을 클릭합니다.

1. 템플릿 카드 또는 테이블 행 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Generate Ad Variations]**&#x200B;을(를) 클릭합니다.

   템플릿이 미리 로드된 상태로 [!UICONTROL Ad Variations Generator]이(가) 열립니다.

1. AI 채팅 인터페이스를 사용하여 광고 콘텐츠를 생성하고 구체화합니다. 전체 워크플로를 보려면 &quot;[Creative Studio에서 표준 광고 관리](creative-studio-manage-standard-ads.md)&quot;를 참조하십시오.

## 광고 템플릿에 대한 레이블 추가 또는 제거 {#template-labels}

*광고 템플릿만 표시합니다.*

레이블은 사용자 템플릿을 구성하고 필터링하는 데 도움이 됩니다. 시스템 템플릿에 레이블을 추가할 수 없습니다.

1. 주 메뉴에서 **[!UICONTROL Creative Studio].**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Templates]** 탭을 클릭합니다.

1. 템플릿 카드 또는 테이블 행 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Edit Labels]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Edit Labels]** 대화 상자에서:

   * 레이블을 추가하려면 기존 레이블을 선택하거나 입력 필드에 이름을 입력하고 **[!UICONTROL Add Tag]**&#x200B;을(를) 클릭합니다.

   * 레이블을 제거하려면 레이블 태그 옆에 있는 **[!UICONTROL X]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 광고 템플릿 미리 보기 {#template-preview}

1. 주 메뉴에서 **[!UICONTROL Creative Studio].**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Templates]** 탭을 클릭합니다.

1. 템플릿 카드 위에 커서를 놓습니다.

1. 다음 중 하나를 수행합니다.

   * (카드 보기) **[!UICONTROL Preview template]** 아이콘을 클릭하거나 **[!UICONTROL ...]** > **[!UICONTROL Preview]**&#x200B;을(를) 클릭합니다.

   * (표 보기) **[!UICONTROL ...]** > **[!UICONTROL Preview]**&#x200B;을(를) 클릭합니다.

1. 비디오 템플릿의 경우 ![재생](/help/creative/assets/play.png "재생")을 클릭하세요.

## 광고 템플릿 다운로드 {#template-download}

1. 주 메뉴에서 **[!UICONTROL Creative Studio].**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Templates]** 탭을 클릭합니다.

1. 템플릿 카드 또는 테이블 행 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Download]**&#x200B;을(를) 클릭합니다.

   브라우저의 일반 절차에 따라 템플릿은 ZIP 파일로 다운로드됩니다.

## 즐겨찾기로 광고 템플릿 추가 또는 제거 {#template-favorite}

*카드 보기 전용*

1. 주 메뉴에서 **[!UICONTROL Creative Studio].**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Templates]** 탭을 클릭합니다.

1. 템플릿 카드 위에 커서를 놓습니다.

1. 다음 중 하나를 수행합니다.

   * 템플릿을 즐겨찾기로 추가하려면 ![즐겨찾기](/help/creative/assets/favorite-null.png "즐겨찾기")를 클릭하십시오.

   * 즐겨찾기로 템플릿을 제거하려면 ![즐겨찾기](/help/creative/assets/favorite.png "즐겨찾기")를 클릭하십시오.

## 광고 템플릿 삭제 {#template-delete}

1. 주 메뉴에서 **[!UICONTROL Creative Studio].**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Templates]** 탭을 클릭합니다.

1. 템플릿 카드 또는 테이블 행 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

## 템플릿 편집기 컨트롤 {#template-controls}

디스플레이 및 비디오 템플릿 편집기 모두 변경 내용을 실행 취소하고 보기를 조정할 수 있는 도구 모음을 캔버스 위에 제공하고, 에셋 및 요소를 추가할 수 있는 왼쪽 패널을 제공하며, 레이어를 관리할 수 있는 오른쪽에 [!UICONTROL Layers] 패널을 제공합니다. 선택한 요소를 편집하고 시간 및 재생을 제어하는 도구는 디스플레이 템플릿과 비디오 템플릿 간에 다릅니다.

<!--

Removing -- these are actions that are used within specific procedures:

### Top toolbar

The top toolbar above the canvas is the same for both display and video templates.

| Control | Description |
| --- | --- |
| Template name | The current template name, shown at the top of the editor. Click the **[!UICONTROL Edit name]** icon next to the name to rename it inline. |
| **[!UICONTROL Save]** | Saves and publishes the template. |
| **[!UICONTROL ...]** > **[!UICONTROL Save As Draft]** | Saves the template as a draft without publishing. Enter or update the name, select the advertiser, optionally add tags, and click **[!UICONTROL Save]**. |
| **[!UICONTROL ...]** > **[!UICONTROL Download]** | Downloads the current template as a ZIP file. |
| **[!UICONTROL Cancel]** | Discards unsaved changes and returns to the Templates list. |

-->

### 변경 내용을 실행 취소하고 캔버스 보기 조정

일반 작업 도구 모음은 광고 템플릿 편집기의 편집 캔버스 위에 있으며 두 부분으로 분할됩니다(왼쪽 및 오른쪽).

#### 광고 템플릿 표시

| 제어 | 설명 |
| --- | --- |
| **[!UICONTROL Undo]** | 마지막 작업을 취소합니다. |
| ![다시 실행](/help/creative/assets/cs-icon-redo.png "다시 실행") **[!UICONTROL Redo]** | 마지막으로 실행 취소된 작업을 다시 실행합니다. |
| **[!UICONTROL Links]** | 템플릿의 요소에 첨부된 클릭스루 URL을 관리할 패널을 엽니다. |
| 확대/축소 컨트롤 | 캔버스 확대율을 조정하려면 **[!UICONTROL Zoom out]** 또는 **[!UICONTROL Zoom in]**&#x200B;을(를) 클릭합니다(10%-150%, 10% 증가). 확대/축소 수준 레이블(캔버스가 자동으로 맞춰진 경우 **[!UICONTROL Auto]** 또는 수동으로 설정된 경우 백분율 표시)을 클릭하여 옵션이 있는 메뉴를 엽니다. **[!UICONTROL Auto-Fit Page]**, **[!UICONTROL 100% Zoom]**, **[!UICONTROL 50% Zoom]**, **[!UICONTROL Zoom In]** 및 **[!UICONTROL Zoom Out]**. |
| 광고 크기 | 현재 광고 차원을 표시합니다(예: 300 × 250). 를 클릭하여 일반적으로 사용되는 6개의 IAB 표준 크기를 카드로 제공하는 크기 선택기와 19개의 표준 IAB 디스플레이 광고 크기가 모두 포함된 드롭다운을 엽니다. 새 템플릿의 기본 크기는 300 × 250(Medium 사각형)입니다. |
| ![레이어 패널 열기](/help/creative/assets/layers-panel-open.png "레이어 패널 열기") | [!UICONTROL Layers] 패널을 엽니다. [!UICONTROL Layers] 패널을 닫은 경우에만 나타납니다. |

#### 비디오 광고 템플릿

| 제어 | 설명 |
| --- | --- |
| **[!UICONTROL Undo]** / ![다시 실행](/help/creative/assets/cs-icon-redo.png "다시 실행") **[!UICONTROL Redo]** | 마지막 작업을 실행 취소하거나 다시 실행합니다. |
| 확대/축소 컨트롤 | 캔버스 확대율을 조정하려면 **[!UICONTROL Zoom out]** 또는 **[!UICONTROL Zoom in]**&#x200B;을(를) 클릭합니다. 확대/축소 수준을 클릭하여 **[!UICONTROL Auto-Fit Page]**, **[!UICONTROL 100% Zoom]**, **[!UICONTROL 50% Zoom]**, **[!UICONTROL Zoom In]** 및 **[!UICONTROL Zoom Out]** 옵션이 있는 메뉴를 엽니다. |
| ![레이어 패널 열기](/help/creative/assets/layers-panel-open.png "레이어 패널 열기") | [!UICONTROL Layers] 패널을 엽니다. [!UICONTROL Layers] 패널을 닫은 경우에만 나타납니다. |

<!--

Not there as of 10/15:

| Page resize | Opens the page-size controls to change the video template dimensions. |
| **[!UICONTROL Preview]** | Opens a preview of the video template. |

   -->

### 에셋 및 요소 추가

왼쪽 패널에서 템플릿에 광고 에셋 및 요소를 추가할 수 있습니다. 아이콘을 클릭하여 콘텐츠 패널을 열고 동일한 아이콘을 다시 클릭하여 닫습니다.

#### 광고 템플릿 표시

| 아이콘 | 설명 |
| --- | --- |
| **[!UICONTROL Search]** | 라이브러리의 모든 자산 유형을 검색합니다. |
| **[!UICONTROL Upload]** | 현재 템플릿에서 사용할 이미지 또는 글꼴 파일을 편집기에 업로드합니다. 한 번에 최대 20개의 파일을 업로드할 수 있습니다. |
| **[!UICONTROL Templates]** | Creative Studio 라이브러리에서 광고 템플릿을 검색하여 기본 레이어 또는 참조 요소로 사용합니다. |
| **[!UICONTROL My Assets]** | Creative Studio [!UICONTROL Assets] 탭에서 업로드한 모든 자산을 찾아봅니다. |
| **[!UICONTROL Images]** | Creative Studio [!UICONTROL Assets] 탭에서 업로드한 이미지 자산만 찾아봅니다. |
| **[!UICONTROL Text]** | 업로드한 사용자 정의 글꼴을 포함한 텍스트 요소를 캔버스에 추가합니다. |
| **[!UICONTROL Elements]** | 모양 및 레이아웃 요소(예: 단추 및 사각형)를 추가합니다. |

패널의 항목을 캔버스로 직접 드래그하거나 클릭하여 기본 위치에 배치할 수 있습니다.

#### 비디오 광고 템플릿

| 아이콘 | 설명 |
| --- | --- |
| **[!UICONTROL Search]** | 라이브러리의 모든 자산 유형을 검색합니다. |
| **[!UICONTROL Upload]** | 현재 템플릿에서 사용할 이미지, 비디오, 오디오 또는 글꼴 파일(TTF, OTF, WOFF, WOFF2)을 편집기에 업로드합니다. 한 번에 최대 20개의 파일을 업로드할 수 있습니다. |
| **[!UICONTROL Templates]** | Creative Studio 라이브러리에서 광고 템플릿을 찾아봅니다. |
| **[!UICONTROL My Assets]** | Creative Studio [!UICONTROL Assets] 탭에서 업로드한 모든 자산을 찾아봅니다. |
| **[!UICONTROL Images]** | Creative Studio [!UICONTROL Assets] 탭에서 업로드한 이미지 자산만 찾아봅니다. |
| **[!UICONTROL Video]** | Creative Studio [!UICONTROL Assets] 탭에서 업로드한 비디오 자산만 찾아봅니다. |
| **[!UICONTROL Audio]** | Creative Studio [!UICONTROL Assets] 탭에서 업로드한 오디오 에셋만 찾아봅니다. |
| **[!UICONTROL Text]** | 업로드한 사용자 정의 글꼴을 포함한 텍스트 요소를 캔버스에 추가합니다. |
| **[!UICONTROL Elements]** | 도형 및 벡터 요소를 추가합니다. |

패널의 항목을 캔버스로 직접 드래그하거나 클릭하여 기본 위치에 배치할 수 있습니다.

### 선택한 요소 편집

편집 캔버스에서 요소를 클릭하여 선택합니다. 템플릿 유형에 따라 하나 이상의 도구 모음이 해당 요소에 대한 컨트롤과 함께 나타납니다.

컨트롤은 요소 유형에 따라 다릅니다.

<!-- From inspectorbar.ts -->

#### 템플릿 편집 도구 모음 표시

| 제어 | 요소 유형 | 설명 |
| --- | --- | --- |
| **[!UICONTROL Properties]** | 모두 | 패널을 열어 레이어 이름을 편집하고, 레이어를 동적(광고 생성 중 스왑 가능)으로 표시하고, 클릭스루 URL(링크만)을 설정합니다. 그 아래에 **[!UICONTROL Default]**, **[!UICONTROL Hover]**, **[!UICONTROL Click]** 또는 **[!UICONTROL Focus]** 상태를 선택하여 해당 상호 작용 상태에 대한 요소의 스타일을 지정한 다음, 요소 유형에 따라 스타일 — 타이포그래피(텍스트와 링크만 해당), 장식(채우기, 테두리, 모서리 반경), 차원, 위치 — 을 조정합니다. |
| **[!UICONTROL Effects]** | 모두 | **[!UICONTROL Default]**, **[!UICONTROL Hover]**, **[!UICONTROL Click]** 또는 **[!UICONTROL Focus]** 상태를 선택하여 해당 상호 작용 상태에 대한 효과를 적용한 다음 **[!UICONTROL Transform]**, **[!UICONTROL Transition]**, **[!UICONTROL Box Shadow]**, **[!UICONTROL Filter]**, **[!UICONTROL Blend Mode]** 및 **[!UICONTROL Cursor]** 섹션을 조정하는 패널을 엽니다. 텍스트 요소에 **[!UICONTROL Text Shadow]** 섹션도 포함됩니다. |
| **[!UICONTROL Animations]** | 모두 | 타임라인에서 레이어의 시작 및 종료 시간을 설정하고 지속 시간과 완화를 사용하여 **[!UICONTROL Entrance Animation]**, **[!UICONTROL Loop Animation]** 및 **[!UICONTROL Exit Animation]** 사전 설정을 구성할 수 있는 패널을 엽니다. **[!UICONTROL Copy]**, **[!UICONTROL Paste]** 및 **[!UICONTROL Reset]** 작업을 포함합니다. |
| **[!UICONTROL Crop]** | 이미지 | 이미지를 자를 수 있는 도구 모음을 엽니다. **[!UICONTROL Aspect Ratio]** 사전 설정(또는 **[!UICONTROL Free]**)을 선택한 다음 **[!UICONTROL Apply]** 또는 **[!UICONTROL Cancel]**&#x200B;을(를) 클릭합니다. |
| **[!UICONTROL Position]** | 모두 | **[!UICONTROL Move]** 옵션(**[!UICONTROL Forward]**, **[!UICONTROL Backward]**, **[!UICONTROL To front]**, **[!UICONTROL To back]**), **[!UICONTROL Align to Page]** 옵션(**[!UICONTROL Top]**, **[!UICONTROL Left]**, **[!UICONTROL Middle]**, **[!UICONTROL Center]**, **[!UICONTROL Bottom]**, **[!UICONTROL Right]**, **[!UICONTROL Fit Vertically]**, **[!UICONTROL Fit Horizontally]**, **[!UICONTROL Fit to Page]**) 및 이미지가 아닌 요소의 경우 **[!UICONTROL Layer Level Alignment]** 옵션(**[!UICONTROL Fit to Content]**&#x200B;과 같은 6개의 정렬 옵션 포함)으로 메뉴를 엽니다. |

#### 비디오 템플릿 편집 도구 모음

| 제어 | 요소 유형 | 설명 |
| --- | --- | --- |
| **[!UICONTROL Shape]** | 모양 | 모양별 옵션을 설정합니다. |
| 오려내기 컨트롤 | 이미지 | 컷아웃 유형, 오프셋 및 매끄럽게 하기 를 조정합니다. |
| **[!UICONTROL Group]** / **[!UICONTROL Ungroup]** | 여러 개의 선택한 요소 또는 그룹 | 선택한 요소를 함께 그룹화하거나 선택한 그룹의 그룹을 해제합니다. |
| **[!UICONTROL Combine]** | 호환 가능한 도형 | 선택한 모양을 단일 모양으로 결합합니다. |
| **[!UICONTROL Audio replace]** | 오디오 및 비디오 | 오디오 트랙을 자산 라이브러리의 파일로 대체합니다. |
| **[!UICONTROL Typeface]**, **[!UICONTROL Bold]**, **[!UICONTROL Italic]**, **[!UICONTROL Font size]**, **[!UICONTROL Align horizontal]**, **[!UICONTROL Advanced]** | 텍스트 | 글꼴 모음, 두께, 크기, 가로 맞춤 및 기타 고급 타이포그래피 설정을 조정합니다. |
| **[!UICONTROL Image]** / **[!UICONTROL Video]** | 이미지 및 비디오 | 요소의 채우기 이미지 또는 비디오 소스를 설정합니다. |
| **[!UICONTROL Trim]** | 비디오 및 오디오 | 트리밍 모드를 열어 클립의 시작점과 끝점을 설정합니다. |
| ![볼륨](/help/creative/assets/volume.png "볼륨")([!UICONTROL Volume]) | 비디오 및 오디오 | 오디오 레벨을 조정합니다. |
| ![재생 속도](/help/creative/assets/speed.png "재생 속도")([!UICONTROL Playback speed]) | 비디오 및 오디오 | 재생 속도를 조정합니다. |
| ![자르기](/help/creative/assets/crop.png "자르기")([!UICONTROL Crop]) | 모두 | 요소를 사용자 지정 영역으로 자릅니다. |
| 회전 및 뒤집기 컨트롤 | 모두 | 선택한 요소를 회전하거나 대칭 이동합니다. |
| ![뇌졸중](/help/creative/assets/stroke.png "뇌졸중")([!UICONTROL Stroke]) | 모두 | 테두리 색상과 너비를 설정합니다. |
| **[!UICONTROL Text Background]** | 텍스트 | 텍스트 뒤에 배경색을 추가합니다. |
| **[!UICONTROL Animations]** | 모두 | 시작, 종료 또는 루프 애니메이션을 추가하거나 편집합니다. |
| **[!UICONTROL Style]** | 모두 | **[!UICONTROL Adjustments]**, **[!UICONTROL Filter]**, **[!UICONTROL Effect]** 및 **[!UICONTROL Blur]** 옵션이 있는 메뉴를 엽니다. |
| **[!UICONTROL Shadow]** | 모두 | 그림자 효과를 추가하거나 편집합니다. |
| **[!UICONTROL Opacity]** | 모두 | 요소의 투명도 수준을 설정합니다. |
| **[!UICONTROL Position]** | 모두 | 요소의 크기, 위치 및 회전을 숫자로 조정합니다. |
| ![편집 패널](/help/creative/assets/cs-template-video-editing-panel.png "편집 패널") | 모두 | 더 많은 편집 기능이 있는 선택한 요소의 [편집 패널](#detailed-element-properties-for-video-templates)을 열거나 닫습니다. |

#### 비디오 템플릿에 대한 자세한 요소 속성

비디오 템플릿 편집기에서 도구 모음의 ![편집 패널](/help/creative/assets/cs-template-video-editing-panel.png "편집 패널")을 클릭하여 더 많은 편집 기능이 있는 선택한 요소의 편집 패널을 엽니다. 편집 패널은 캔버스 왼쪽에 나타나며 템플릿의 레이어를 나열하는 [!UICONTROL Layers] 패널과 별개입니다.

##### 개별 요소

단일 이미지, 비디오, 모양 또는 텍스트 요소를 선택하면 편집 패널에 아래의 해당 섹션이 표시됩니다.

| 패널 섹션 | 도구 | 컨트롤 |
| --- | --- | --- |
| [!UICONTROL Layer] | 정렬 및 레이어 위치 | 선택한 레이어를 왼쪽, 가로 가운데, 오른쪽, 위쪽, 세로 가운데 또는 아래쪽으로 맞춥니다. 정렬 메뉴는 앞뒤 스택 순서를 변경합니다. 이러한 컨트롤은 레이어 자체의 위치를 지정하므로 레이어 내의 텍스트를 양쪽 정렬하지 않습니다. |
| | [!UICONTROL Rotate & Flip] | 회전 각도를 도 단위로 입력합니다. 레이어를 가로로 미러링하려면 ![가로 뒤집기](/help/creative/assets/cs-template-video-flip.png "가로 뒤집기")를 사용하고, 세로로 미러링하려면 ![세로 뒤집기](/help/creative/assets/cs-template-video-flip-vertical.png "세로 뒤집기")를 사용하십시오. |
| | ![불투명도](/help/creative/assets/cs-template-video-opacity.png "불투명도") [!UICONTROL Opacity] | 선택한 레이어를 투명도가 높아지거나 낮아집니다. |
| | ![혼합 모드](/help/creative/assets/cs-template-video-blend-mode.png "혼합 모드") [!UICONTROL Blend Mode] | 선택한 레이어의 색상이 그 뒤에 있는 레이어와 결합하는 방식을 변경합니다. |
| | [!UICONTROL Transform]: [!UICONTROL Position & Size] | 레이어의 위치 및 치수에 대한 추가 컨트롤을 엽니다. 사용 가능 여부는 선택한 레이어의 변형 권한에 따라 다릅니다. |
| [!UICONTROL Shape] | ![모양 옵션](/help/creative/assets/cs-template-video-shape-options.png "모양 옵션") [!UICONTROL Shape] 및 모양별 속성 | 형태와 점, 면, 내경, 선 폭 또는 모서리 반지름과 같은 사용 가능한 특성을 변경합니다. 컨트롤은 선택한 도형에 따라 다릅니다. |
| | [!UICONTROL Vector]: [!UICONTROL Edit Path] | 가능한 경우 벡터 편집 모드로 전환하여 모양의 패스를 편집합니다. |
| [!UICONTROL Character] | ![서체](/help/creative/assets/cs-template-video-typeface.png "서체") 서체, ![텍스트 스타일](/help/creative/assets/cs-template-video-text-style.png "텍스트 스타일") 텍스트 스타일, ![굵게](/help/creative/assets/cs-template-video-text-bold.png "굵게") 굵게, ![기울임꼴](/help/creative/assets/cs-template-video-text-italic.png "기울임꼴") 기울임꼴 및 ![글꼴 크기](/help/creative/assets/cs-template-video-font-size.png "글꼴 크기") 글꼴 크기 | (텍스트 레이어) 선택한 텍스트의 글꼴 모음, 글꼴 스타일 및 크기를 변경합니다. |
| | ![왼쪽 정렬](/help/creative/assets/cs-template-video-text-align-l.png "왼쪽 정렬") / ![가운데 정렬](/help/creative/assets/cs-template-video-text-align-c.png "가운데 정렬") / ![오른쪽 정렬](/help/creative/assets/cs-template-video-text-align-r.png "오른쪽 정렬") 텍스트 정렬 | (텍스트 레이어) 프레임 내의 텍스트를 왼쪽, 가운데 또는 오른쪽으로 정렬하거나 정렬을 자동으로 감지합니다. |
| | ![고급 텍스트 설정](/help/creative/assets/cs-template-video-advanced-text.png "고급 텍스트 설정") 고급 텍스트 설정 | (텍스트 레이어) 추가 타이포그래피 설정을 엽니다. |
| [!UICONTROL Fill] | ![채우기](/help/creative/assets/cs-template-video-fill.png "채우기") 채우기 컨트롤 | 선택한 레이어의 색상, 이미지 또는 비디오 채우기를 변경합니다. 컨트롤은 현재 채우기 유형을 반영하고 해당 설정을 엽니다. 텍스트의 경우 텍스트 색상을 변경합니다. |
| [!UICONTROL Stroke] | ![획](/help/creative/assets/cs-template-video-stroke.png "획") 획 컨트롤 | 윤곽선을 활성화하거나 비활성화하고 색상, 너비, 스타일 및 배치를 변경합니다. 스트로크가 활성화되면 추가 컨트롤이 나타납니다. |
| [!UICONTROL Text Background] | ![텍스트 배경](/help/creative/assets/cs-template-video-text-bg.png "텍스트 배경") 배경 컨트롤 | (텍스트 레이어) 텍스트 뒤에 배경을 추가하거나 변경합니다. |
| [!UICONTROL Animations] | ![애니메이션](/help/creative/assets/cs-template-video-animation.png "애니메이션") [!UICONTROL Presets] | 시작, 종료 및 루프 애니메이션을 포함하여 선택한 레이어에 대한 애니메이션 사전 설정을 엽니다. |
| [!UICONTROL Appearance] | ![조정](/help/creative/assets/cs-template-video-adjustments.png "조정") [!UICONTROL Adjustments] | 선택한 레이어의 시각적 속성을 변경합니다. |
| | ![필터](/help/creative/assets/cs-template-video-filter.png "필터") [!UICONTROL Filter] | 선택한 레이어에 시각적 필터를 적용합니다. |
| | ![효과](/help/creative/assets/cs-template-video-effects.png "효과") [!UICONTROL Effect] | 선택한 레이어에 효과를 적용합니다. |
| | ![흐림 효과](/help/creative/assets/cs-template-video-blur.png "흐림 효과") [!UICONTROL Blur] | 선택한 레이어에 흐림 효과를 적용합니다. |
| | ![그림자](/help/creative/assets/cs-template-video-shadow.png "그림자") [!UICONTROL Shadow] | 선택한 레이어의 그림자를 추가하거나 변경합니다. |

##### 다중 선택 및 특수 요소

여러 요소, 그룹, 컷아웃 요소 또는 오디오 클립을 선택하면 편집 패널에 아래의 선택 영역별 섹션이 표시됩니다. 여러 요소, 그룹 및 컷아웃에도 [!UICONTROL Layer] 섹션이 유지됩니다.

| 패널 섹션 | 도구 | 컨트롤 |
| --- | --- | --- |
| [!UICONTROL Layer] | 정렬 및 레이어 위치 | 선택한 여러 요소 또는 그룹을 정렬합니다. 정렬 메뉴는 앞뒤 스택 순서를 변경합니다. |
| | [!UICONTROL Rotate & Flip] | 선택한 요소 또는 그룹을 회전하거나 대칭 이동합니다. |
| | ![불투명도](/help/creative/assets/cs-template-video-opacity.png "불투명도") [!UICONTROL Opacity] | 선택한 요소 또는 그룹을 더 투명하게 하거나 덜 투명하게 합니다. |
| | ![혼합 모드](/help/creative/assets/cs-template-video-blend-mode.png "혼합 모드") [!UICONTROL Blend Mode] | 선택한 요소 또는 그룹의 색상이 그 뒤에 있는 레이어와 결합하는 방식을 변경합니다. |
| | [!UICONTROL Transform]: [!UICONTROL Position & Size] | 선택한 요소 또는 그룹의 위치 및 차원에 대한 컨트롤을 엽니다. 사용 가능한 컨트롤은 선택한 요소에 따라 다릅니다. |
| [!UICONTROL Selection] | ![그룹](/help/creative/assets/cs-template-video-group.png "그룹") 그룹 / ![그룹 해제](/help/creative/assets/cs-template-video-ungroup.png "그룹 해제") 그룹 해제 | 선택한 여러 레이어 또는 선택한 그룹의 [!UICONTROL Layer] 아래에 나타납니다. 선택한 레이어를 함께 관리할 수 있도록 그룹화하거나 그룹을 개별 레이어로 구분합니다. |
| [!UICONTROL Settings] | ![Cutout clip](/help/creative/assets/cs-template-video-cutout-clip.png "Cutout clip") / ![Cutout overlay](/help/creative/assets/cs-template-video-cutout-overlay.png "Cutout overlay") Cutout 컨트롤 | (오려내기 레이어)는 [!UICONTROL Layer] 아래에 나타납니다. 컷아웃 유형을 선택하고 오프셋과 모서리 매끄럽게 하기를 조정합니다. |
| [!UICONTROL Audio Properties] | ![트리밍](/help/creative/assets/cs-template-video-trim.png "트리밍") 트리밍, ![볼륨](/help/creative/assets/cs-template-video-volume.png "볼륨") 볼륨 및 ![재생 속도](/help/creative/assets/cs-template-video-playback-speed.png "재생 속도") 재생 속도 | (오디오 레이어) 클립의 시작 및 종료 지점, 오디오 레벨 및 재생 속도를 설정합니다. |

#### 캔버스에서 직접 요소 편집

##### 광고 템플릿 표시

| 액션 | 설명 |
| --- | --- |
| **[!UICONTROL Replace]** | (이미지 요소만 해당) 이미지를 자산 라이브러리의 이미지로 바꿀 수 있도록 이미지 패널을 엽니다. |
| ![앞으로 이동](/help/creative/assets/cs-icon-move-forward.png "앞으로 이동") **[!UICONTROL Move forward]** | 요소를 겹침 순서에서 한 단계 앞으로(앞쪽으로) 이동합니다. |
| ![뒤로 이동](/help/creative/assets/cs-icon-move-backward.png "뒤로 이동") **[!UICONTROL Move backward]** | 요소를 겹침 순서에서 한 단계 뒤로 이동합니다(뒤로). |
| ![복제](/help/creative/assets/cs-icon-duplicate.png "복제") **[!UICONTROL Duplicate]** | 요소의 복사본을 만듭니다. |
| ![삭제](/help/creative/assets/cs-icon-delete.png "삭제") **[!UICONTROL Delete]** | 캔버스에서 요소를 제거합니다. |
| 회전 핸들 | 선택한 요소 위에 있는 핸들을 클릭하고 드래그하여 회전합니다. 회전을 15도 단위로 스냅하려면 드래그하면서 **[!UICONTROL Shift]**&#x200B;을(를) 유지하십시오. |

선택한 요소를 클릭하여 드래그하여 위치를 변경하고, 그 주변의 핸들을 클릭하여 드래그하여 크기를 조정할 수도 있습니다.

##### 비디오 광고 템플릿

| 액션 | 설명 |
| --- | --- |
| **[!UICONTROL Edit text]** | (텍스트 요소만 해당) 캔버스에서 직접 텍스트를 입력하고 서식을 지정할 수 있도록 텍스트 편집 모드로 전환합니다. 텍스트 편집 모드에서 보조 메뉴는 **[!UICONTROL Text color]**, **[!UICONTROL Bold]**, **[!UICONTROL Italic]** 및 **[!UICONTROL Text variables]**(템플릿 자리 표시자)을 제공합니다. |
| **[!UICONTROL Replace]** | (이미지 요소만 해당) 이미지를 교체할 수 있도록 에셋 라이브러리를 엽니다. |
| **[!UICONTROL Bring forward]** | 요소를 겹침 순서에서 한 단계 앞으로 이동합니다. |
| **[!UICONTROL Send backward]** | 요소를 겹침 순서에서 한 단계 뒤로 이동합니다. |
| **[!UICONTROL Duplicate]** | 요소의 복사본을 만듭니다. |
| **[!UICONTROL Delete]** | 캔버스에서 요소를 제거합니다. |
| **... >[!UICONTROL Flip horizontal]** | 요소를 수평으로 180도 뒤집습니다. |
| **... >[!UICONTROL Flip vertical]** | 요소를 수직으로 180도 뒤집습니다. |
| **... >[!UICONTROL Copy Element]** | 요소를 캔버스 클립보드에 복사합니다. |
| **... >[!UICONTROL Pastes Element]** | 복사된 요소를 붙여넣습니다. |

선택한 요소를 클릭하여 드래그하여 위치를 변경하고, 그 주변의 핸들을 클릭하여 드래그하여 크기를 조정할 수도 있습니다.

### 시간 및 재생 제어

디스플레이 편집기와 비디오 편집기는 모두 캔버스 하단에 타임라인 패널을 표시합니다.

#### 광고 템플릿 표시

타임라인에는 캔버스의 각 레이어에 대한 트랙이 표시되며, 시간 범위에는 레이어가 시작 및 종료 애니메이션 타이밍을 기준으로 표시됩니다. 트랙의 시작 또는 끝 핸들을 드래그하여 시작 또는 종료 시간을 조정하거나 트랙을 드래그하여 레이어 순서를 변경합니다. 눈금자를 클릭하거나 재생 헤드를 드래그하여 특정 시점으로 이동합니다.

타임라인 도구 모음에는 **[!UICONTROL Duration]** 필드(0~60초), **[!UICONTROL Play]**/**[!UICONTROL Pause]**, 현재 시간/총 기간 표시, 루프 전환, **[!UICONTROL Timeline Scale]** 확대/축소 컨트롤, **[!UICONTROL Fit View]** 단추 및 축소/확장 전환이 포함됩니다.

#### 비디오 광고 템플릿

타임라인에 템플릿의 모든 비디오 및 오디오 클립이 표시됩니다. 타임라인을 사용하여 클립이 제시간에 정렬되는 방식을 검토하고 시작 및 끝 핸들을 드래그하여 클립을 트리밍합니다. 타임라인에서 새 클립을 바로 추가할 수는 없습니다. 대신 왼쪽 패널 또는 캔버스에서 추가한 다음 타임라인에서 클립으로 나타납니다.

### 레이어 관리

캔버스 오른쪽의 [!UICONTROL Layers] 패널에는 템플릿의 모든 요소가 나열되며, 이를 통해 해당 요소의 순서, 가시성 및 속성을 관리할 수 있습니다. 표시 서식 파일의 경우 캔버스 도구 모음에서 **[!UICONTROL Open Layers]**&#x200B;을(를) 클릭하여 엽니다. 비디오 템플릿의 경우 기본적으로 패널이 열립니다.

레이어를 클릭하여 캔버스에서 해당 요소를 선택합니다.

**탭(광고 템플릿만 표시)**

표시 템플릿에는 [!UICONTROL Layers] 패널 위쪽에 두 개의 탭이 있습니다.

* **[!UICONTROL Dynamic]** — AI 에이전트가 대체할 수 있는 이미지 및 텍스트와 같이 광고 생성 중에 교환할 수 있는 레이어만 나열합니다. 광고 변형을 생성하기 위한 기본 보기입니다.
* **[!UICONTROL All]** — 구조적 컨테이너를 포함하여 템플릿에 대한 전체 레이어 계층 구조를 표시합니다. 이 보기를 사용하여 요소의 중첩 방법을 검사하거나 다시 구성합니다.

비디오 템플릿은 탭이 없는 단일 목록의 모든 레이어를 표시합니다.

**레이어별 작업**

레이어 위에 커서를 놓으면 다음 작업이 표시됩니다.

| 액션 | 설명 |
| --- | --- |
| ![레이어 이름 바꾸기](/help/creative/assets/edit.png "레이어 이름 바꾸기") **[!UICONTROL Rename layer]** | 패널에 새 레이어 이름을 입력할 수 있습니다. |
| ![레이어 잠금](/help/creative/assets/cs-icon-lock.png "레이어 잠금") **[!UICONTROL Lock layer]** / ![레이어 잠금 해제](/help/creative/assets/cs-icon-unlock.png "레이어 잠금 해제") **[!UICONTROL Unlock layer]** | 레이어를 이동, 편집 또는 재정렬하지 못하도록 합니다. |
| ![레이어 숨기기](/help/creative/assets/cs-icon-hidden.png "레이어 숨기기") **[!UICONTROL Hide layer]** / ![레이어 표시](/help/creative/assets/cs-icon-visible.png "레이어 표시") **[!UICONTROL Show layer]** | 캔버스에서 레이어를 숨기거나 표시합니다. 숨겨진 레이어는 템플릿에서 유지되지만 템플릿을 렌더링할 때는 표시되지 않습니다. |
| ![순서를 바꾸려면 드래그](/help/creative/assets/cs-icon-drag.png "순서를 바꾸려면 드래그") 순서를 바꾸려면 드래그 | (광고 템플릿만 표시) 순서 조정 아이콘을 드래그하여 겹침 순서에서 레이어의 위치를 변경합니다. 순서를 변경하려면 레이어 잠금을 해제해야 합니다. |

**패널 바닥글**

| 액션 | 설명 |
| --- | --- |
| ![선택한 레이어 복제](/help/creative/assets/cs-icon-duplicate.png "선택한 레이어 복제") **[!UICONTROL Duplicate selected layer]** | 선택한 레이어의 복사본을 만듭니다. |
| ![선택한 레이어 삭제](/help/creative/assets/cs-icon-delete.png "선택한 레이어 삭제") **[!UICONTROL Delete selected layer]** | 선택한 레이어를 삭제합니다. |
| **[!UICONTROL Group selected layers]**(비디오 템플릿 전용) | 둘 이상의 선택한 레이어를 단일 그룹으로 그룹화합니다. 두 개 이상의 레이어를 선택한 경우에만 나타납니다. 그룹화된 레이어의 그룹을 해제하거나 그룹 행의 컨트롤을 사용하여 그룹에서 개별 레이어를 제거할 수 있습니다. |

<!--

These are all saved with the template, but they aren't what you see, as-is, in the template settings per se. Rethink if I should include this, and how to frame it:

## Template settings {#template-settings}

### Display ad template settings

| Setting | Description |
| --- | --- |
| **[!UICONTROL Advertiser]** | (Required) The advertiser this template belongs to. |
| **[!UICONTROL Ad Template Name]** | (Required) A unique name for the template. |
| **[!UICONTROL Type]** | (Required) The HTML5 template type: **[!UICONTROL Static HTML5]** or **[!UICONTROL Dynamic HTML]**. |
| **[!UICONTROL Size]** | (Required) The ad dimensions. |
| **[!UICONTROL Description]** | (Optional) A description of the template. |
| **[!UICONTROL Tags]** | (Optional) One or more labels. Click **[!UICONTROL Add More]** to add additional tags. |
| **ZIP file** | The HTML5 creative ZIP file. For **[!UICONTROL Dynamic HTML]** templates, also upload the template data file (TDF). |

### Video ad template settings

| Setting | Description |
| --- | --- |
| **[!UICONTROL Advertiser]** | (Required) The advertiser this template belongs to. |
| **[!UICONTROL Ad Template Name]** | (Required) A unique name for the template. |
| **[!UICONTROL Description]** | (Optional) A description of the template. |
| **ZIP file** | The video ad template ZIP file. |

-->

>[!MORELIKETHIS]
>
>* [Advertising Creative의 Creative Studio 정보](creative-studio-about.md)
>* [Creative Studio에서 자산 관리](creative-studio-manage-assets.md)
>* [Creative Studio에서 표준 광고 관리](creative-studio-manage-standard-ads.md)
>* [Creative Studio에서 동적 크리에이티브 관리](creative-studio-manage-dynamic-ads.md)
