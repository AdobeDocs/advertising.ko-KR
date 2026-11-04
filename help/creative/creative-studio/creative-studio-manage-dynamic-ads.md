---
title: Creative Studio에서 동적 크리에이티브 관리
description: Adobe Advertising Creative Studio에서 카탈로그 기반의 동적 크리에이티브를 빌드, 품질 검사, 편집, 복제 및 삭제하는 방법에 대해 알아봅니다.
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: d0d9f2ed-c163-44e1-97a1-4ace121416b8
    internal-label: Creative
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: b9a68528b3c622aae44a46bca9b3bb747019bc95
workflow-type: tm+mt
source-wordcount: '1421'
ht-degree: 0%
---
# [!UICONTROL Creative Studio]에서 동적 크리에이티브 관리

[!UICONTROL Creative Studio]의 **[!UICONTROL Creatives]** 탭에는 라이브러리별로 동적 크리에이티브가 나열됩니다. 여기에서 새로운 카탈로그 기반의 동적 크리에이티브를 구축하고, AI를 통한 품질 점검 크리에이티브를 구축하고, 기존 크리에이티브의 세부 정보 및 속성 매핑을 편집하고, 변경 로그를 보고, 중복된 크리에이티브를 확인하고, 크리에이티브를 삭제할 수 있습니다.

## 동적 크리에이티브 구축 {#build-dynamic-creative}

이 워크플로우를 사용하여 카탈로그 기반의 동적 크리에이티브를 만듭니다. 4단계 안내식 마법사는 템플릿 선택, 카탈로그 연결, 카탈로그 필드를 템플릿 요소에 매핑하는 과정을 안내합니다. 설정 후 [!UICONTROL AI Assistant]을(를) 사용하면 카탈로그 데이터에서 생성된 각 광고 조합을 미리 보고 품질을 확인할 수 있습니다.

동적 크리에이티브는 주요 방식에서 표준 광고와 다릅니다. AI 에이전트는 카탈로그 소스 콘텐츠를 수정할 수 없습니다. 문제를 필터링, 분석 및 플래그를 지정할 수 있지만 광고 콘텐츠를 변경하려면 QA 화면이나 소스 카탈로그에서 카탈로그 값을 수동으로 업데이트해야 합니다.

### 사전 요구 사항

* 사용자가 만든 디스플레이 광고 템플릿(시스템 템플릿이 아님)이 템플릿 라이브러리에 하나 이상 있어야 합니다.
* 계정에서 제품 또는 콘텐츠 카탈로그(피드)를 사용할 수 있습니다.

### 1단계: [!UICONTROL Build Dynamic Creative] 마법사 열기 {#open-wizard}

1. 주 메뉴에서 **[!UICONTROL Creative Studio]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Creatives]** 탭의 **[!UICONTROL Build dynamic creatives from catalog data]** 빠른 작업 카드에서 **[!UICONTROL Build]**&#x200B;을(를) 클릭합니다.

   4단계 **[!UICONTROL Build Dynamic Creative]** 대화 상자가 열립니다.

### 2단계: 템플릿 선택 {#select-template}

>[!NOTE]
>
>템플릿 갤러리 목록에는 사용자가 만든 광고 템플릿만 표시됩니다. 시스템 템플릿 및 비디오 광고 템플릿은 동적 크리에이티브의 시작점으로 사용할 수 없습니다.

1. 템플릿 갤러리에서 템플릿을 클릭하여 선택합니다.

   템플릿을 선택할 때까지 **[!UICONTROL Next]** 단추를 사용할 수 없습니다.

1. **[!UICONTROL Use this template]**&#x200B;을(를) 클릭합니다.

### 3단계: 카탈로그 선택 {#select-catalog}

1. 크리에이티브 설정을 구성합니다.

   * **[!UICONTROL Ad Library]:** 크리에이티브를 저장할 크리에이티브 라이브러리를 선택합니다.
   * **[!UICONTROL Dynamic creative name]:** 동적 크리에이티브의 이름을 입력하십시오.
   * **[!UICONTROL Number of cards]:** 각 광고 조합에 포함할 카탈로그 오퍼 수를 입력합니다(1-50).
   * **[!UICONTROL Assign dynamic creative to a bundle]:**(선택 사항) 활성화되면 저장된 크리에이티브가 번들에 연결됩니다. 라이브러리에서 번들을 선택합니다.

1. 하나 이상의 카탈로그 선택:

   1. (선택 사항) **[!UICONTROL Catalog template]**&#x200B;을(를) 사용하여 카탈로그 목록을 특정 템플릿 계열로 필터링합니다. 선택적으로 템플릿 파일을 다운로드하여 검토하려면 **[!UICONTROL Download feed template]**&#x200B;을(를) 클릭하십시오.

   1. 목록에서 카탈로그를 검색하고 선택합니다. 선택한 모든 카탈로그는 동일한 카탈로그 템플릿 제품군에 속해야 합니다. 제품군을 혼합하려고 하면 경고가 표시됩니다.

   1. (선택 사항) 새 카탈로그 파일을 업로드하려면 파일을 업로드 영역으로 끌어다 놓거나 **[!UICONTROL Browse Files]**&#x200B;을(를) 클릭합니다. 지원되는 형식: JPG, PNG, JPEG, XLS, XLSX, CSV, TSV, ZIP 및 MP4. 최대 파일 크기: 25MB 한 번에 하나의 파일을 업로드할 수 있습니다. 업로드된 카탈로그가 칩 목록에 **(업로드됨)**(으)로 표시됩니다.

1. **[!UICONTROL Continue]**&#x200B;을(를) 클릭합니다.

### 4단계: 카탈로그 필드를 템플릿 요소에 매핑 {#attribute-mapping}

각 카탈로그 필드를 템플릿의 해당 요소에 매핑합니다. 예를 들어, 카탈로그의 제품 이름 필드를 템플릿의 헤드라인 요소에 매핑하고 제품 이미지 필드를 배경 이미지 요소에 매핑합니다.

1. **[!UICONTROL Targeting]**&#x200B;에서 Creative를 개인화할 데이터 원본을 하나 이상 선택하십시오. **[!UICONTROL Profile data]**, **[!UICONTROL Geographic data]**, **[!UICONTROL Data pass]** 또는 **[!UICONTROL Audience Segment]**.

1. 각 템플릿 요소에 대해 드롭다운에서 일치하는 카탈로그 필드를 선택합니다.

1. **[!UICONTROL Continue]**&#x200B;을(를) 클릭합니다.

### 5단계: AI를 통한 미리보기 및 QA {#qa}

1. *[!UICONTROL Save Dynamic Creative & Skip QA]*&#x200B;을(를) 사용할지 *[!UICONTROL Continue to QA]*&#x200B;을(를) 사용할지 선택합니다.

   QA를 계속하면 미리 보기 캔버스와 **[!UICONTROL AI Assistant]** 채팅 패널이 있는 **[!UICONTROL Dynamic Creative QA]** 화면이 열립니다.

1. QA를 계속하는 경우 &quot;[동적 크리에이티브의 품질 확인](#qa-dynamic-creative)&quot;의 절차를 따라 [광고 분석 및 필터링](#analyze-ads), [미리 보기 및 경고 검토](#review-previews), 선택적으로 [카탈로그 값 수정](#correct-catalog-values)합니다. 완료되면 [동적 크리에이티브를 저장](#save-or-exit)합니다.

## 다이내믹 크리에이티브 편집 {#edit-dynamic-creative}

1. 주 메뉴에서 **[!UICONTROL Creative Studio]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 Creative 카드 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

   전체 화면 편집기가 열리고 왼쪽에는 광고 미리 보기가 있고 오른쪽에는 설정 패널이 있습니다.

1. **[!UICONTROL Details]** 및 **[!UICONTROL Attribute Mapping]** 탭을 사용하여 크리에이티브 설정을 편집합니다.

   **[!UICONTROL Details]** 탭:

   * **[!UICONTROL Advertiser]**, **[!UICONTROL Ad Library]** 및 **[!UICONTROL Ad template]**&#x200B;은(는) 읽기 전용입니다.
   * **[!UICONTROL Dynamic creative name]:** 크리에이티브의 표시 이름입니다.
   * **[!UICONTROL Number of cards]:** 각 광고 조합에 포함된 카탈로그 오퍼 수입니다(1-50).
   * (선택 사항) **[!UICONTROL Catalogs]**&#x200B;에서 카탈로그 선택을 업데이트합니다.
     * **[!UICONTROL Catalog template]**&#x200B;을(를) 사용하여 사용 가능한 카탈로그를 필터링하십시오. 필요한 경우 템플릿 파일을 다운로드하려면 **[!UICONTROL Download feed template]**&#x200B;을(를) 클릭합니다.
     * 목록에서 카탈로그를 검색 및 선택하거나 업로드 영역으로 드래그하거나 **[!UICONTROL Browse Files]**&#x200B;을(를) 클릭하여 새 카탈로그 파일을 업로드하십시오(지원되는 형식: JPG, PNG, JPEG, XLS, XLSX, CSV, TSV, ZIP, MP4; 최대 25MB; 한 번에 한 파일). 업로드된 카탈로그의 칩 목록에 **(업로드됨)** 레이블이 지정되었습니다.

     모든 카탈로그는 동일한 카탈로그 템플릿 제품군에 속해야 합니다.

   **[!UICONTROL Attribute Mapping]** 탭:

   * **[!UICONTROL Targeting]**&#x200B;에서 **[!UICONTROL Profile data]**, **[!UICONTROL Geographic data]**, **[!UICONTROL Data pass]** 또는 **[!UICONTROL Audience Segment]** 데이터 원본을 하나 이상 선택하십시오.
   * **[!UICONTROL Attribute Mapping]**&#x200B;에서 각 템플릿 레이어 이름의 매핑을 해당 카탈로그 열 레이블로 업데이트합니다.

1. **[!UICONTROL Update Creative]**&#x200B;을(를) 클릭합니다.

## 다이내믹 크리에이티브 품질 검사 {#qa-dynamic-creative}

QA 도우미를 사용하여 동적 크리에이티브의 템플릿에 대해 카탈로그 행을 분석하고, 결과 광고를 미리 보고, 잠재적인 콘텐츠 문제를 식별할 수 있습니다. **[!UICONTROL AI Assistant]**&#x200B;을(를) 사용하여 광고를 필터링 및 그룹화하고, 카탈로그 경고를 검토하고, 변경 내용을 게시하기 전에 카탈로그 값을 수동으로 수정할 수 있습니다.

>[!NOTE]
>
>[!UICONTROL Creative Studio] 또는 [!UICONTROL Creative Libraries]에서 동적 크리에이티브의 품질을 확인할 수 있습니다. 메뉴 레이블은 다르지만 두 진입점은 동일한 기능을 사용하여 동일한 **[!UICONTROL Dynamic Creative QA]** 화면을 엽니다. 분석은 선택한 크리에이티브, 카탈로그 및 요청에 따라 다릅니다. 다른 진입점에 대해서는 &quot;[Creative 라이브러리에서 동적 크리에이티브 품질 검사](/help/creative/creative-libraries/creative-edit-dynamic.md#qa-dynamic-creative)&quot;를 참조하십시오.

QA 도우미는 표준 크리에이티브나 동적 비디오 크리에이티브가 아닌 동적 디스플레이 크리에이티브에 사용할 수 있습니다.

### QA 길잡이 열기 {#open-qa-agent}

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Studio]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 [!UICONTROL Generate or Build Creatives] 섹션 아래의 Creative 라이브러리에서 동적 Creative를 찾습니다.

1. Creative 카드 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL QA Assistant]**&#x200B;을(를) 클릭합니다.

   미리 보기 캔버스와 **[!UICONTROL AI Assistant]** 채팅 패널이 있는 **[!UICONTROL Dynamic Creative QA]** 화면이 열립니다.

1. 크리에이티브가 여러 카탈로그를 사용하는 경우 헤더의 **[!UICONTROL Catalog]**&#x200B;에서 검토할 카탈로그를 선택하십시오.

   도우미가 선택한 카탈로그를 분석합니다. 크리에이티브가 하나의 카탈로그만 사용하는 경우에는 카탈로그 선택기가 비활성화됩니다.

### AI로 광고 분석 및 필터링 {#analyze-ads}

1. **[!UICONTROL AI Assistant]** 패널에서 **[!UICONTROL Ask anything]**&#x200B;에 요청을 입력하고 **[!UICONTROL Enter]**&#x200B;을(를) 누르거나 제안 프롬프트 중 하나를 클릭합니다.

   * **[!UICONTROL Run a comprehensive QA pass on this dynamic creative]**
   * **[!UICONTROL Group ads by product]**
   * **[!UICONTROL Filter ads by geography]**
   * **[!UICONTROL Show all ads with headlines over 80 characters]**

   도우미가 채팅 패널에서 응답하고 일치하는 카탈로그 행을 캔버스에서 광고 미리 보기로 표시합니다. 요청을 제출할 때까지 캔버스는 도우미에게 카탈로그를 분석하도록 요청하라는 메시지를 표시합니다.

1. 후속 요청을 통해 검토를 계속 구체화합니다. 도우미는 다음 작업을 도와 드릴 수 있습니다.

   * 대상자 세그먼트, 언어, 지역 또는 우편 번호별로 광고를 필터링합니다.
   * 지정한 임계값을 사용하여 문자 길이를 확인합니다.
   * 피드 오류, 누락된 콘텐츠 및 의심스러운 콘텐츠가 있는지 확인합니다.
   * 번역 상태를 검토합니다.
   * A/B 테스트 변형 비교
   * 제품 또는 문제별 등 검토용 그룹 광고.

   보조자의 응답을 확인하고 변경 사항을 저장하기 전에 미리보기를 검사합니다.

### 미리 보기 및 경고 검토 {#review-previews}

* 캔버스 도구 모음을 사용하여 다음을 수행할 수 있습니다.

  * 확대/축소를 조정합니다.
  * **[!UICONTROL Thumbnail view]**&#x200B;과(와) **[!UICONTROL Actual size]** 간 전환.
  * 미리 보기를 재생하려면 **[!UICONTROL Replay animations]**&#x200B;을(를) 클릭합니다.
  * 페이지당 행 수를 선택하거나 페이지 번호를 선택하거나 **[!UICONTROL Previous page]** 및 **[!UICONTROL Next page]**&#x200B;을(를) 사용합니다.

* 어시스턴트 그룹 결과가 나오면 해당 링크를 클릭하여 그룹의 모든 크리에이티브를 조회합니다. **[!UICONTROL Back to groups]**&#x200B;을(를) 사용하여 그룹화된 결과로 돌아가거나 **[!UICONTROL Catalog Rows]**&#x200B;을(를) 사용하여 그룹화된 보기에서 나가십시오.

* 미리 보기에 **[!UICONTROL Issues detected]**&#x200B;이(가) 표시되면 표시기 위에 커서를 놓으면 문제 세부 정보를 볼 수 있습니다.

* 카탈로그 경고를 사용할 수 있으면 **[!UICONTROL View Alerts]**&#x200B;을(를) 클릭합니다. **[!UICONTROL Alerts]** 대화 상자에 각 문제에 대한 카탈로그, 행 번호, 열 및 오류 메시지가 나열됩니다. 캔버스로 돌아가려면 **[!UICONTROL Close]**&#x200B;을(를) 클릭하십시오.

### 올바른 카탈로그 값 {#correct-catalog-values}

QA 화면을 종료하지 않고 광고 미리 보기에서 카탈로그 값을 수동으로 편집할 수 있습니다.

1. 수정하려는 미리 보기에서 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. 편집 대화 상자에서 **[!UICONTROL Catalog columns to edit]**&#x200B;에서 변경할 열을 선택합니다. 열을 찾으려면 **[!UICONTROL Search columns]**&#x200B;을(를) 사용합니다.

1. **[!UICONTROL Columns content]**&#x200B;에서 선택한 필드 값을 업데이트합니다.

1. **[!UICONTROL Update]**&#x200B;을(를) 클릭합니다.

   미리보기가 새로 고침되어 업데이트된 값이 반영됩니다. 동적 크리에이티브를 저장할 때까지 카탈로그 변경 사항이 게시되지 않습니다.

>[!IMPORTANT]
>
>이러한 편집은 광고 미리 보기뿐만 아니라 카탈로그 데이터를 업데이트합니다. 값을 게시하기 전에 검토하십시오.

### 변경 내용 저장 또는 종료 {#save-or-exit}

* 동적 크리에이티브를 저장하고 카탈로그 편집 내용을 게시하려면 다음 작업을 수행하십시오.

  1. 헤더에서 **[!UICONTROL Save Dynamic Creative]**&#x200B;을(를) 클릭합니다.

  1. 저장 확인:

     * 새 크리에이티브를 보려면 **[!UICONTROL Create Dynamic Creative]** 확인 대화 상자에서 **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.
     * 기존 크리에이티브의 경우 **[!UICONTROL Update Dynamic Creative]** 확인 대화 상자에서 **[!UICONTROL Update]**&#x200B;을(를) 클릭합니다.

     [!UICONTROL Creative Studio]&#x200B;(으)로 돌아갑니다.

* 보류 중인 카탈로그 편집 내용을 게시하지 않고 나가려면 페이지 머리글에서 **[!UICONTROL Cancel]**&#x200B;을(를) 클릭합니다.

## 동적 크리에이티브에 대한 변경 로그 보기 {#view-change-log}

1. 주 메뉴에서 **[!UICONTROL Creative Studio]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 Creative 카드 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Change Log]**&#x200B;을(를) 클릭합니다.

## 다이내믹 크리에이티브 복제 {#duplicate-dynamic-creative}

동적 크리에이티브를 복제하여 동일한 설정을 사용하는 새 크리에이티브를 라이브러리에 추가합니다. 나중에 새 크리에이티브의 이름을 바꾸고 필요에 따라 설정을 편집할 수 있습니다.

1. 주 메뉴에서 **[!UICONTROL Creative Studio]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 Creative 카드 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Duplicate]**&#x200B;을(를) 클릭합니다.

   새 크리에이티브의 이름은 `<original name> (copy)`입니다.

## 동적 크리에이티브 삭제 {#delete-dynamic-creative}

1. 주 메뉴에서 **[!UICONTROL Creative Studio]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 Creative 카드 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [Advertising Creative의 Creative Studio 정보](creative-studio-about.md)
>* [Creative Studio에서 표준 광고 관리](creative-studio-manage-standard-ads.md)
>* [Creative Studio에서 템플릿 관리](creative-studio-manage-templates.md)
