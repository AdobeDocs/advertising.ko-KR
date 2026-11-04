---
title: 동적 크리에이티브 편집 및 품질 점검
description: Creative Library에서 동적 크리에이티브 설정을 편집하고 카탈로그 콘텐츠를 품질 검사하는 방법을 알아봅니다.
feature: Creative Dynamic Creatives
exl-id: b75b9aeb-ffd0-4b86-aa7a-bd6a22e7a8e4
TQID: 'https://experienceleague.adobe.com/QoQ5p4sFV-ARIMNDbPkp7axfqkVEC3sxJ6MTlPIG22Y'
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: d0d9f2ed-c163-44e1-97a1-4ace121416b8
    internal-label: Creative
subfeature_v2:
  - id: d70c54b0-f069-4a3c-8056-7069a25e110c
    internal-label: Creative Dynamic Creatives
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: ed1682eff9ce28df30a5314de90f6f67c10f338a
workflow-type: tm+mt
source-wordcount: '1118'
ht-degree: 0%
---
# 동적 크리에이티브 편집 및 품질 점검

크리에이티브 설정을 편집하여 이름, 카탈로그 및 속성 매핑과 같은 크리에이티브의 구성을 변경합니다. QA 에이전트를 사용하여 결과 광고를 검토하고 카탈로그 값을 수정합니다.

## 크리에이티브 설정 편집 {#edit-creative-settings}

### 새 UI에서 {#from-the-new-ui}

1. 크리에이티브 설정을 엽니다.

   * 크리에이티브 라이브러리에서:

     1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

     1. 다음 방법 중 하나로 라이브러리를 엽니다.

        * 라이브러리 이름을 클릭합니다.

        * 라이브러리 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Open]**&#x200B;을(를) 클릭합니다.

     1. **[!UICONTROL Creatives]** 탭에서 크리에이티브 이름 옆에 있는 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

   * [!UICONTROL Creative Studio]부터:

     1. 메인 메뉴에서 **[!UICONTROL Creative]>[!UICONTROL Creative Studio]**&#x200B;을(를) 클릭합니다.

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

### 기존 UI에서 {#from-the-legacy-ui}

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Switch to classic UI]**&#x200B;을(를) 클릭합니다.

1. 라이브러리 이름을 클릭합니다.

1. Creative 행 위에 커서를 놓고 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. [동적 광고 설정](creative-settings-dynamic.md)을(를) 편집합니다.

1. 생성할 크리에이티브를 미리 보려면 **[!UICONTROL Continue]**&#x200B;을(를) 클릭하십시오. 미리보기 내에서 다음 중 하나를 수행할 수 있습니다.

   * 카탈로그, 필터 값 <!-- explain more--> 및 광고 크기별로 광고 크리에이티브를 필터링하려면 미리 보기 영역 위의 필터를 사용하십시오.

   * 미리 보기 영역 아래의 검색 필드에서 고유 ID로 제품을 검색합니다.

   * 표시되는 열을 변경하려면 미리 보기 영역 아래의 ![열 필터](/help/creative/assets/custom-columns.png "열 필터")를 클릭하십시오.

   * 특정 크리에이티브를 미리 보려면 행의 확인란을 선택합니다.

   * 콘텐츠 변경:

     * (광고만 표시) 표 내에서 셀의 값을 편집하려면 셀 내부를 클릭하고 값을 편집합니다. 셀 외부를 클릭하거나 **[!DNL Enter]** 키를 눌러 변경 내용을 저장합니다.

     * 단일 제품을 기본값 <!--Explain what this means. -->(으)로 표시하려면 행 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Set as Default]**&#x200B;을(를) 클릭합니다.

     * (광고에 두 개 이상의 오퍼가 포함된 경우) 여러 제품을 기본값으로 표시하려면 행(최대 오퍼 수)을 선택하고 일괄 작업 도구 모음에서 **[!UICONTROL Set as Default]**&#x200B;을(를) 클릭합니다.

     * 카탈로그에서 제품을 삭제하려면 행 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Delete Row]**&#x200B;을(를) 클릭합니다.

     * (광고에 두 개 이상의 오퍼가 포함된 경우) 카탈로그에서 여러 제품을 삭제하려면 행(최대 오퍼 수)을 선택하고 일괄 작업 도구 모음에서 **[!UICONTROL Delete Row]**&#x200B;을(를) 클릭합니다.

1. 크리에이티브를 저장합니다.

   * 광고를 저장하고 라이브러리의 [크리에이티브 번들](bundle-manage.md)에 추가하려면:

     1. **[!UICONTROL Save and Attach to Bundle]**&#x200B;을(를) 클릭합니다.

     1. **[!UICONTROL Save]**&#x200B;을(를) 클릭하여 광고를 저장합니다.

     1. 번들을 선택한 다음 **[!UICONTROL Attach Creative to Bundles]**&#x200B;을(를) 클릭합니다.

   * 광고를 저장하고 설치를 종료하려면 **[!UICONTROL Save]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Save]**&#x200B;을(를) 다시 클릭합니다.

## 다이내믹 크리에이티브 품질 확인(새 UI만 해당) {#qa-dynamic-creative}

새 UI에서 QA 에이전트를 사용하여 동적 크리에이티브의 템플릿에 대해 카탈로그 행을 분석하고, 결과 광고를 미리 보고, 잠재적인 콘텐츠 문제를 식별할 수 있습니다. **[!UICONTROL AI Assistant]**&#x200B;을(를) 사용하여 광고를 필터링 및 그룹화하고, 카탈로그 경고를 검토하고, 변경 내용을 게시하기 전에 카탈로그 값을 수동으로 수정할 수 있습니다.

>[!NOTE]
>
>[!UICONTROL Creative Libraries] 또는 [!UICONTROL Creative Studio]에서 동적 크리에이티브의 품질을 확인할 수 있습니다. 다른 진입점에 대해서는 &quot;[Creative Studio에서 동적 크리에이티브 품질 검사](/help/creative/creative-studio/creative-studio-manage-dynamic-ads.md#qa-dynamic-creative)&quot;를 참조하십시오.

QA 에이전트는 표준 크리에이티브나 동적 비디오 크리에이티브가 아닌 동적 템플릿을 기반으로 한 동적 디스플레이 크리에이티브에 대해서만 사용할 수 있습니다.

### QA 에이전트 열기 {#open-qa-agent}

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

1. 다음 방법 중 하나로 라이브러리를 엽니다.

   * 라이브러리 이름을 클릭합니다.
   * 라이브러리 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Open]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 동적 Creative 이름 옆의 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL QA Agent]**&#x200B;을(를) 클릭합니다.

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

* 기존 동적 크리에이티브를 저장하고 카탈로그 편집 내용을 게시하려면 다음 작업을 수행하십시오.

  1. 헤더에서 **[!UICONTROL Save Dynamic Creative]**&#x200B;을(를) 클릭합니다.

  1. **[!UICONTROL Update Dynamic Creative]** 확인 대화 상자에서 **[!UICONTROL Update]**&#x200B;을(를) 클릭합니다.

     크리에이티브 라이브러리로 돌아갑니다.

* 보류 중인 카탈로그 편집 내용을 게시하지 않고 나가려면 페이지 머리글에서 **[!UICONTROL Cancel]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [동적 크리에이티브 설정](creative-settings-dynamic.md)
>* [Creative 라이브러리에 동적 크리에이티브 추가](creative-add-dynamic.md)
>* [크리에이티브에 대한 변경 로그 보기](/help/creative/creative-libraries/creative-view-change-log.md)
>* [동적 광고용 워크플로](/help/creative/introduction/workflow-dynamic-ads.md)
