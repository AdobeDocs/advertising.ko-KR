---
title: Creative Studio에서 표준 광고 관리
description: Creative Studio 광고 라이브러리에서 표준 디스플레이 광고를 생성, 편집, 복제, 다운로드 및 삭제하는 방법에 대해 알아봅니다.
exl-id: 01d3cdec-80d0-494c-94dd-d9d0ae8ca53c
product_v2: id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2: id: d0d9f2ed-c163-44e1-97a1-4ace121416b8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: a6ab21a588f5b069ea0783dee711f52d906a46f9
workflow-type: tm+mt
source-wordcount: 1181
ht-degree: 0%

---

# [!UICONTROL Creative Studio]에서 표준 광고 관리

*Beta 기능*

[!UICONTROL Creative Studio]의 **[!UICONTROL Creatives]** 탭은 템플릿에서 생성된 표준 디스플레이 광고 라이브러리입니다. 여기에서 [!UICONTROL Ad Variations Generator]을(를) 사용하여 광고를 만들고, 저장된 광고를 편집하고, 기존 광고에서 새 변형을 생성하고, 변경 로그를 보고, 복제, 다운로드 및 삭제할 수 있습니다.

## 표준 광고 만들기 {#create-standard-ads}

[!UICONTROL Ad Variations Generator]을(를) 사용하여 템플릿에서 디스플레이 광고 콘텐츠를 생성합니다. AI 어시스턴트는 헤드라인, CTA, 이미지, 색상 등을 생성 및 세분화하고, 단일 세션에서 새로운 크기 변형을 만들 수 있습니다.

>[!NOTE]
>
>표준 광고 생성은 현재 디스플레이 광고 템플릿만 지원합니다. 비디오 광고 템플릿은 **[!UICONTROL Creatives]** 탭 또는 **[!UICONTROL Templates]** 탭에서 시작점으로 사용할 수 없습니다.

### 사전 요구 사항

템플릿 라이브러리에 디스플레이 광고 템플릿이 하나 이상 있어야 합니다.

### 표준 광고 생성

1. 다음 방법 중 하나로 [!UICONTROL Ad Variations Generator]을(를) 엽니다.

   * [!UICONTROL Creatives] 탭의 **:**

      1. 주 메뉴에서 **[!UICONTROL Creative Studio]**&#x200B;을(를) 클릭합니다.

      1. **[!UICONTROL Creatives]** 탭의 **[!UICONTROL Generate standard ads from templates]** 빠른 작업 카드에서 **[!UICONTROL Generate]**&#x200B;을(를) 클릭합니다.

      1. 템플릿 선택 대화 상자에서 템플릿을 클릭하여 선택한 다음 **[!UICONTROL Use this template]**&#x200B;을(를) 클릭합니다.

   * (광고 표시 전용) **[!UICONTROL Templates] 탭에서:**

      1. 주 메뉴에서 **[!UICONTROL Creative Studio]**&#x200B;을(를) 클릭합니다.

      1. **[!UICONTROL Templates]** 탭을 클릭합니다.

      1. 템플릿 카드 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Generate ad variations]**&#x200B;을(를) 클릭합니다.

   [!UICONTROL Ad Variations Generator]이(가) 열립니다. 캔버스에는 템플릿의 사용 가능한 광고 형식이 포함된 **[!UICONTROL Template Sizes]** 섹션과 생성된 컨텐츠가 나타나는 **[!UICONTROL Ad Concepts]** 섹션이 표시됩니다.

1. (선택 사항) 브랜드 프로필을 광고에 적용하려면 캔버스 도구 모음에서 **[!UICONTROL Brand Profile]**&#x200B;을(를) 선택합니다.

   AI 비서는 콘텐츠를 생성할 때 브랜드의 로고, 색상 팔레트, 음성 지침, 이미지 표준 및 채널 지침을 사용합니다.

1. [!UICONTROL AI Assistant]을(를) 사용하여 광고 변형 작성:

   1. **[!UICONTROL Ask AI to generate ad variations…]** 필드에서 요청을 입력하고 **[!UICONTROL Enter]**&#x200B;을(를) 누르거나 추천 프롬프트 중 하나를 클릭합니다.

      * **[!UICONTROL Write 3 headline variations for this template]**
      * **[!UICONTROL Generate 3 versions of this ad that will help with performance]**
      * **[!UICONTROL Create a new size template]**

      AI는 캔버스에서 결과를 생성하여 *개념*(으)로 구성하며, 각각은 고유한 콘텐츠 변형을 나타냅니다. **[!UICONTROL Ad Concepts]** 섹션의 개념 카운터는 개념 수를 추적합니다(예: **(2/10)**). 세션당 최대 10개의 개념이 허용됩니다.

   1. 후속 메시지를 전송하여 세분화를 계속합니다. 예:

      * &quot;모든 사본을 더 재미있고 덜 조직적으로 만듭니다.&quot;
      * &quot;로고를 흰색 버전으로 변경하십시오.&quot;
      * &quot;모든 개념에서 CTA을 &#39;지금 쇼핑&#39;으로 설정합니다.&quot;
      * &quot;이 광고의 크기를 6개의 IAB 표준 표시 크기 모두로 조정하십시오.&quot;
      * &quot;각각에 대해 일치하는 배경 이미지와 함께 3개의 다른 헤드라인 개념을 주세요.&quot;

      >[!NOTE]
      >
      >AI 어시스턴트는 텍스트(헤드라인, 서브헤드라인, CTA, 본문 복사)를 생성 및 수정하고, 배경 이미지를 교체하고, 브랜드 색상을 적용하고, 로고 버전을 전환하고, 새 크기 템플릿을 만들 수 있습니다. 요소 위치, 레이아웃, 간격, 패딩, 글꼴 패밀리, 글꼴 크기 또는 테두리 등의 템플릿 구조를 변경할 수 없습니다. 세션을 시작하기 전에 템플릿 편집기에서 구조를 변경합니다. [템플릿 편집](creative-studio-manage-templates.md#edit-template)을 참조하세요.

   1. (선택 사항) 요청에 시각적 참조를 포함하려면 채팅 입력 영역에서 **[!UICONTROL +]** 단추를 클릭하십시오. **[!UICONTROL Select from Asset Library]** 대화 상자에서:

      * 에셋 라이브러리에서 에셋을 사용하려면 해당 에셋을 클릭한 다음 **[!UICONTROL Add to chat]**&#x200B;을(를) 클릭합니다. 자산을 컨텍스트로 포함하려면 메시지를 제출하십시오.

      * 하나 이상의 자산을 업로드하려면 **[!UICONTROL Upload Assets]**&#x200B;을(를) 클릭하고 장치나 네트워크에서 파일을 선택하십시오.

1. (선택 사항) 캔버스 도구 모음을 사용하여 생성된 광고를 검토합니다.

   * **[!UICONTROL Brand]:** 세션에 적용되는 브랜드 프로필을 선택하거나 변경합니다.
   * **[!UICONTROL Zoom in]** / **[!UICONTROL Zoom out]:** 캔버스 확대/축소 수준을 조정합니다.
   * **[!UICONTROL Fit to screen]:** 모든 크기를 표시하도록 보기를 재설정합니다.
   * **[!UICONTROL Replay animations]:** 템플릿 애니메이션을 재생합니다.

   AI가 새 크기를 만들면 **[!UICONTROL Adjust]**, **[!UICONTROL Keep]** 및 삭제 컨트롤이 새 크기 카드에 나타납니다. 크기를 그대로 사용하려면 **[!UICONTROL Keep]**&#x200B;을(를) 클릭하고, 구조적 변경을 수행할 수 있는 디스플레이 편집기에서 템플릿을 열려면 **[!UICONTROL Adjust]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Update Ad Format]**&#x200B;을(를) 클릭하여 저장하거나, 삭제 아이콘을 클릭하여 새 크기를 제거합니다.

1. (선택 사항) 개념 및 변형 관리:

   * 개념을 관리하려면 개념 레이블(예: **[!UICONTROL Concept 3]**) 위에 커서를 놓고 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 옵션을 선택합니다.

      * **[!UICONTROL Add to chat]:**&#x200B;이(가) 다음 프롬프트에서 개념을 참조합니다.
      * **[!UICONTROL Delete]:** 개념을 제거합니다.

   * 개별 변형을 관리하려면 변형 카드 위에 커서를 놓고 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 옵션을 선택하십시오.

      * **[!UICONTROL Add to Chat]:**&#x200B;이(가) 다음 프롬프트에서 변형을 참조합니다. 변형 카드 본문을 직접 클릭하여 언급을 전환할 수도 있습니다.
      * **[!UICONTROL Edit Data]:** 템플릿에 정의된 각 클릭 태그에 대한 클릭스루 URL과 변형 **[!UICONTROL Name]**&#x200B;을(를) 업데이트할 수 있는 대화 상자를 엽니다. 적용하려면 **[!UICONTROL Save]**&#x200B;을(를) 클릭하십시오.
      * **[!UICONTROL Delete]:** 변형을 제거합니다.

1. 생성된 개념에 만족하면 헤더에서 **[!UICONTROL Save Standard Ads]**&#x200B;을(를) 클릭합니다.

   적어도 하나의 개념이 존재할 때까지 버튼이 비활성화됩니다.

1. **[!UICONTROL Save Standard Ads]** 대화 상자에서 다음 설정을 지정한 다음 **[!UICONTROL Save Standard Ads]**&#x200B;을(를) 클릭합니다.

   **[!UICONTROL Advertiser]:**(필수) 광고주가 아래에 크리에이티브를 저장합니다.

   **[!UICONTROL Creative Library]:**(필수) 크리에이티브 라이브러리를 저장할 대상. 광고주를 선택하면 라이브러리 선택기가 활성화됩니다.

   **[!UICONTROL Attach to Bundles]:**(선택 사항) 활성화되면 저장된 크리에이티브가 하나 이상의 번들에 연결됩니다. 각 광고 변형에 대해 번들을 선택하거나 새 번들 이름을 입력합니다.

   **\[각 광고에 대한 설정\]:** 각 광고 변형에 대해 **[!UICONTROL Name],** **[!UICONTROL Language],** 및 **[!UICONTROL click URL]을(를) 보고 선택적으로 변경할 수 있습니다.**

## 표준 광고 편집 {#edit-standard-ad}

1. 주 메뉴에서 **[!UICONTROL Creative Studio]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 Creative 카드 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

   전체 화면 편집기가 열리고 왼쪽에는 라이브 광고 미리보기, 오른쪽에는 설정 패널이 표시됩니다.

1. **[!UICONTROL Details]** 및 **[!UICONTROL Attributes]** 탭을 사용하여 광고 설정을 편집합니다.

   **[!UICONTROL Details]** 탭:

   * **[!UICONTROL Creative Name]:**(필수) 크리에이티브의 표시 이름입니다.
   * **[!UICONTROL Language]:**(필수) 광고 콘텐츠의 언어입니다.
   * **[!UICONTROL Creative Size]:**(읽기 전용) 광고 차원입니다.
   * **클릭 태그:** 템플릿에서 클릭 태그를 정의하면 각 클릭 태그가 태그 이름으로 레이블이 지정된 필수 필드로 나타납니다. 각 태그에 대한 클릭스루 대상 URL을 입력합니다.
   * 광고 구성을 위한 **[!UICONTROL Label]:**(선택 사항) 레이블입니다. 기존 레이블을 선택하거나 새 태그를 입력하고 **[!UICONTROL Add tag].**&#x200B;을(를) 클릭합니다.

   **[!UICONTROL Attributes]** 탭:

   편집하면 실시간 미리보기가 실시간으로 업데이트됩니다. 미리 보기를 로드하는 동안에는 **[!UICONTROL Attributes]** 탭을 사용할 수 없습니다.

   * **텍스트 특성:** 템플릿에 정의된 편집 가능한 각 텍스트 레이어의 텍스트 값을 입력합니다.
   * **이미지 특성:** 현재 이미지의 축소판을 표시합니다. **[!UICONTROL Replace Image]**&#x200B;을(를) 클릭하여 대체 항목(PNG, JPEG, GIF, WebP 또는 SVG)을 업로드합니다.

1. **[!UICONTROL Update Creative]**&#x200B;을(를) 클릭합니다.

## 표준 광고에 대한 광고 변형 생성 {#generate-ad-variations}

1. 주 메뉴에서 **[!UICONTROL Creative Studio]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 Creative 카드 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Generate Ad Variations]**&#x200B;을(를) 클릭합니다.

   선택한 광고가 미리 로드된 상태로 [!UICONTROL Ad Variations Generator]이(가) 열립니다.

1. AI 채팅 인터페이스를 사용하여 추가 변형을 생성하고 구체화합니다. 전체 워크플로우에 대해서는 &quot;[표준 광고 만들기](#create-standard-ads)&quot;를 참조하십시오.

## 표준 광고 복제 {#duplicate-standard-ad}

표준 광고를 복제하여 라이브러리에 동일한 설정의 새 크리에이티브를 추가합니다. 나중에 새 크리에이티브의 이름을 바꾸고 필요에 따라 설정을 편집할 수 있습니다.

1. 주 메뉴에서 **[!UICONTROL Creative Studio]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 Creative 카드 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Duplicate]**&#x200B;을(를) 클릭합니다.

   새 크리에이티브의 이름은 `<original name> (copy)`입니다.

## 표준 광고에 대한 변경 로그 보기 {#view-change-log}

1. 주 메뉴에서 **[!UICONTROL Creative Studio]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 Creative 카드 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Change Log]**&#x200B;을(를) 클릭합니다.

   광고 변경 사항 테이블을 표시하는 대화 상자가 열립니다.

## 표준 광고 다운로드 {#download-standard-ad}

1. 주 메뉴에서 **[!UICONTROL Creative Studio]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 Creative 카드 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Download]**&#x200B;을(를) 클릭합니다.

   크리에이티브는 브라우저의 일반적인 절차에 따라 다운로드합니다.

## 표준 광고 삭제 {#delete-standard-ad}

>[!NOTE]
>
>이 작업은 취소할 수 없습니다.

1. 주 메뉴에서 **[!UICONTROL Creative Studio]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 Creative 카드 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [Advertising Creative의 Creative Studio 정보](creative-studio-about.md)
>* [Creative Studio에서 동적 크리에이티브 관리](creative-studio-manage-dynamic-ads.md)
>* [Creative Studio에서 템플릿 관리](creative-studio-manage-templates.md)
>* [Advertising Creative에서 브랜드 프로필 관리](/help/creative/brands/brand-manage.md)

