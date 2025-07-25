---
title: 타깃팅된 경험 설정
description: 타겟팅된 광고 경험에 대한 모든 설정 설명을 참조하십시오.
feature: Creative Experiences
exl-id: cb6fd855-6534-4eac-b34b-323073d186be
source-git-commit: 4b780760e5a7a0c3d370054fce8b1c15fbc6802d
workflow-type: tm+mt
source-wordcount: '1133'
ht-degree: 0%

---

# 타깃팅된 광고 경험 설정

*베타가 닫힘*

## [!UICONTROL Experience basics] 섹션

**[!UICONTROL Ad Type]:**(기존 경험의 경우 읽기 전용) 경험에 포함된 광고 유형: *[!UICONTROL Standard Display]*, *[!UICONTROL Dynamic Display]* 또는 *[!UICONTROL Video]*. 경험을 저장하면 광고 유형을 변경할 수 없습니다.

**[!UICONTROL Advertiser]:**(기존 경험의 경우 읽기 전용) 경험에 포함된 광고 및 타겟 조합에 입찰할 광고주입니다. 경험을 저장하면 광고주를 변경할 수 없습니다.

**[!UICONTROL Experience Name]:** 경험의 고유한 이름입니다. **팁:** Advertising DSP 또는 다른 DSP에서 환경을 광고로 사용할 때 쉽게 찾을 수 있는 이름을 사용하십시오.

**[!UICONTROL Creative Library]:**(기존 경험의 경우 읽기 전용) 경험에 사용할 단일 Creative 라이브러리입니다. 경험을 저장하면 라이브러리를 변경할 수 없습니다.

## [!UICONTROL Default creatives] 섹션

**\[기본 크리에이티브 지정\]:** 브라우저에 JavaScript이 사용되지 않거나 지연으로 인해 광고 서버가 광고를 개인화할 수 없는 경우와 같이 경험에 할당된 크리에이티브를 표시할 수 없는 경우 사용할 기본 크리에이티브입니다. 표준 디스플레이 경험의 경우 경험이 적용되는 광고 크기당 하나의 이미지 크리에이티브를 포함합니다. 표준 비디오 경험의 경우 경험이 적용되는 광고 크기당 하나의 비디오 크리에이티브를 포함합니다. 선택에 따라 경험에 사용할 수 있는 창의적인 크기가 결정됩니다.

의사 결정 트리 타깃팅이 있는 경험의 경우 의사 결정 트리 내에서 동일한 크기의 크리에이티브가 포함된 크리에이티브 번들로 기본 크리에이티브를 재정의할 수 있습니다.<!-- verify -->

* 다른 차원의 기본 크리에이티브를 추가하려면 **[!UICONTROL + Add Sizes]**&#x200B;을(를) 클릭하고 오른쪽 창에서 추가할 각 크리에이티브 옆의 확인란을 선택한 다음 **[!UICONTROL Add Creatives]**&#x200B;을(를) 클릭합니다.

* 기본 크리에이티브를 삭제하려면 크리에이티브 썸네일 위에 커서를 놓고 ![삭제](/help/creative/assets/delete.png "삭제")를 클릭합니다.

* 모든 기본 크리에이티브를 삭제하려면 ![삭제](/help/creative/assets/delete.png "삭제") **[!UICONTROL Delete all]**&#x200B;을(를) 클릭합니다.

* 오른쪽의 [크리에이티브] 창을 표시하거나 숨기려면 오른쪽 창의 오른쪽 상단에 있는 ![표시/숨기기](/help/creative/assets/hide-show-creatives.png "표시/숨기기")를 클릭합니다.

## [!UICONTROL Targeting] 섹션

**[!UICONTROL Targeting]:**(기존 경험의 경우 읽기 전용) 의사 결정 트리 및 자동 태그 생성을 사용하여 크리에이티브 타깃팅을 활성화합니다. 경험을 저장하면 이 설정을 변경할 수 없습니다.

**[!UICONTROL Language Targeting]:**(표준 광고만 있는 경험, 선택 사항, 기존 경험의 경우 읽기 전용) 사용자의 브라우저 언어 설정을 확인하고 해당 언어의 크리에이티브를 사용할 수 있는 경우 지정된 언어의 크리에이티브를 표시합니다. 브라우저 지정 언어의 크리에이티브를 사용할 수 없는 경우 대신 [!UICONTROL Preferred language] 설정이 사용됩니다.

경험을 저장하면 이 설정을 변경할 수 없습니다.

**[!UICONTROL Preferred language]:**(표준 광고만 있는 경험, 기존 경험의 경우 읽기 전용) [!UICONTROL Language Targeting]이(가) 활성화된 경우를 제외하고 경험에서 만든 모든 광고의 언어입니다. 경험을 저장하면 이 설정을 변경할 수 없습니다.

## [!UICONTROL Advanced] 섹션

**데이터 전달:**(기존 경험의 경우 읽기 전용, 선택 사항) DSP, 게시자 또는 파트너가 노출 시 실시간으로 전달하는 특정 키-값 쌍(예: SKU=01234567890123 또는 Cart=empty)을 기준으로 사용자를 타깃팅합니다. 최대 5개의 기본 데이터 전달 키(매개 변수)를 지정할 수 있습니다. 의사 결정 트리 내에서 타깃팅을 설정할 때 한 수준의 데이터 전달 대상 노드를 포함하고, 선택적으로 키를 사용자 지정하고, 각 노드에 대해 타깃팅할 값을 지정할 수 있습니다. 경험을 만들 때 이 필드에 키를 지정하지 않은 경우에도 결정 트리 내에서 키를 지정할 수 있습니다.

각 키는 광고 경험 태그에 매크로로 추가되며, 이를 통해 DSP에서 광고로 구현하도록 생성할 수 있습니다.

**반경:**(동적 광고만 있는 경험, 선택 사항) 피드 파일에 지정된 미국 우편 번호에서 타깃팅할 반경입니다. 0마일에서 200마일 사이의 반경을 선택하십시오. 경험에 대한 동적 광고를 만드는 데 사용되는 피드 파일에는 파일의 각 제품 행에 대한 값이 있는 [!UICONTROL ZIP] 열<!-- or a user-named column mapped to a ZIP column -->이(가) 포함되어야 합니다. 예를 들어 반경 10마일의 경우, 95110에서 사용할 수 있는 제품에 대한 광고를 95110 10마일(사용자의 IP 주소로 결정됨) 내의 사용자에게 표시할 수 있습니다.

**RT 픽셀:**(기존 경험의 경우 읽기 전용, 선택 사항) 잠재적으로 타깃팅할 [!UICONTROL Creative] 리타겟팅 픽셀입니다. 의사 결정 트리 내에서 타깃팅을 설정할 때 한 수준의 RT 픽셀 대상 노드를 포함할 수 있습니다. 각 노드에 대해 타겟팅할 픽셀과 할당된 크리에이티브 번들에서 크리에이티브를 표시하는 데 필요한 픽셀 속성 값을 지정합니다. 경험을 만들 때 이 필드에 픽셀을 지정하지 않으면 결정 트리 내에서 픽셀을 지정할 수 있습니다.<!-- May move this to just within the decision tree. -->

**레이블:**<!-- should be "Labels" --> (선택 사항) 경험에 적용할 [!DNL Creative]별 레이블입니다. 경험 보기에서 레이블을 기준으로 경험을 필터링하고 [!UICONTROL Experience Label]에 [!UICONTROL Custom Creative Report] 차원을 포함할 수 있습니다.

* 기존 레이블을 선택하려면 ![아래로](/help/creative/assets/chevron-down.png "아래로")를 클릭하고 적용할 각 레이블 옆에 있는 확인란을 선택하십시오.

* 기존 레이블을 검색하려면 레이블 이름 내에 텍스트 문자열 입력을 시작합니다.

* 적용할 새 레이블을 만들려면 목록을 열고 **+ 레이블 추가**&#x200B;를 클릭하고 [!UICONTROL Label] 필드에 새 레이블 이름을 입력한 다음 **만들기**&#x200B;를 클릭합니다.

* 레이블을 제거하려면 레이블 이름 옆에 있는 확인란을 선택 취소합니다.

**노출 추적 URL:** (선택 사항) 경험에서 만든 모든 광고의 랜딩 페이지 URL에 추가할 타사 노출 추적 URL입니다. 최대 5개의 URL을 포함할 수 있습니다. URL을 추가하려면 ![아이콘](/help/creative/assets/create.png) **[!UICONTROL Add More]을(를) 클릭하고 URL을 입력하십시오.

URL을 입력하면 [사용 가능한 모든 매크로](/help/creative/creative-macros.md)와 이 매크로가 대체되는 데이터가 페이지 아래쪽에 나열됩니다. URL에 매크로 중 하나를 삽입하려면 매크로 설명 위에 커서를 놓고 ![클립보드에 복사](/help/creative/assets/copy-to-clipboard.png "클립보드에 복사")를 클릭한 다음 URL 필드에 매크로를 원하는 위치에 붙여넣습니다.

>[!NOTE]
>
>* [!DNL Creative]은(는) 자신의 노출 추적 태그를 랜딩 페이지 URL에 자동으로 접두사로 추가합니다.
>* [경험의 모든 크리에이티브에 대해 이 URL을 재정의할 수 있습니다](experience-tracking-urls-targeting.md).
>* [!UICONTROL Client JS] 필드에 타사 JavaScript 노출 추적 코드를 입력할 수도 있습니다

**클릭 추적 URL:** (선택 사항) 랜딩 페이지 URL에 추가할 타사 클릭 추적 URL입니다. 최대 5개의 URL을 포함할 수 있습니다. URL을 추가하려면 ![아이콘](/help/creative/assets/create.png) **[!UICONTROL Add More]을(를) 클릭하고 URL을 입력하십시오.

URL을 입력하면 [사용 가능한 모든 매크로](/help/creative/creative-macros.md)와 이 매크로가 대체되는 데이터가 페이지 아래쪽에 나열됩니다. URL에 매크로 중 하나를 삽입하려면 매크로 설명 위에 커서를 놓고 ![클립보드에 복사](/help/creative/assets/copy-to-clipboard.png "클립보드에 복사")를 클릭한 다음 URL 필드에 매크로를 원하는 위치에 붙여넣습니다.

>[!NOTE]
>
>* [!DNL Creative]은(는) 자신의 노출 추적 태그를 랜딩 페이지 URL에 자동으로 접두사로 추가합니다.
>* [경험의 모든 크리에이티브에 대해 이 URL을 재정의할 수 있습니다](experience-tracking-urls-targeting.md).

**클라이언트 JS:**(선택 사항) 다음 중 하나:

* (광고주가 광고에 OBA 준수 공급업체를 사용하는 경우) JavaScript 코드는 사용자가 OBA(온라인 행동 타깃팅)를 옵트아웃할 수 있도록 하는 광고 오버레이를 가리킵니다.

* 랜딩 페이지에 추가할 타사 JavaScript 노출 추적 코드. **참고:** [!UICONTROL Impression Tracking URL] 필드에 타사 노출 추적 URL을 입력할 수도 있습니다.

>[!MORELIKETHIS]
>
>* [의사 결정 트리 타깃팅으로 경험 만들기](experience-create-targeting.md)
>* [의사 결정 트리 타깃팅으로 경험 편집](experience-edit-targeting.md)
>* [추적 URL에 사용할 수 있는 매크로](/help/creative/creative-macros.md)
