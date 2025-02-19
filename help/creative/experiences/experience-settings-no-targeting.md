---
title: 타깃팅되지 않은 경험에 대한 설정
description: 의사 결정 트리 타깃팅이 없는 광고 경험에 대한 모든 설정 설명을 참조하십시오.
feature: Creative Experiences
exl-id: aeeca035-8ae2-4173-827a-b8690d228549
source-git-commit: 4d362e7321433cb3c4ef34790f8ae26f817cd9d9
workflow-type: tm+mt
source-wordcount: '1129'
ht-degree: 0%

---

# 타깃팅되지 않은 경험에 대한 설정

*베타가 닫힘*

## [!UICONTROL Experience basics] 섹션

**[!UICONTROL Advertiser]:**(기존 경험의 경우 읽기 전용) 경험에 포함된 크리에이티브에 입찰할 광고주입니다. 경험을 저장하면 광고주를 변경할 수 없습니다.

**[!UICONTROL Experience Name]:** 경험의 고유한 이름입니다. **팁:** Advertising DSP 또는 다른 DSP에서 환경을 광고로 사용할 때 쉽게 찾을 수 있는 이름을 사용하십시오.

**[!UICONTROL Creative Library]:**(기존 경험의 경우 읽기 전용) 경험에 사용할 단일 Creative 라이브러리입니다. 경험을 저장하면 라이브러리를 변경할 수 없습니다.

## [!UICONTROL Default creatives] 섹션

**\[기본 크리에이티브 지정\]:** 브라우저가 JavaScript을 사용할 수 없거나 광고 서버가 지연으로 인해 광고를 개인화할 수 없는 경우와 같이 브라우저에 경험에 할당된 크리에이티브를 표시할 수 없는 경우 사용할 기본 이미지 크리에이티브입니다. 경험이 적용되는 광고 크기당 하나의 이미지 크리에이티브를 포함합니다. 선택에 따라 경험에 사용할 수 있는 창의적인 크기가 결정됩니다. <!-- In the legacy product, you selected the ad sizes for the experience, and then selected default images for each of those ad sizes. -->

의사 결정 트리 타깃팅이 없는 경험의 경우 [!UICONTROL Tag Manager].<!-- verify --> 내에서 크기가 같은 크리에이티브로 기본 크리에이티브를 재정의할 수 있습니다.

* 다른 차원의 기본 크리에이티브를 추가하려면 **[!UICONTROL + Add Sizes]**&#x200B;을(를) 클릭하고 오른쪽 창에서 추가할 각 크리에이티브 옆의 확인란을 선택한 다음 **[!UICONTROL Add Creatives]**&#x200B;을(를) 클릭합니다.

* 기본 크리에이티브를 삭제하려면 크리에이티브 썸네일 위에 커서를 놓고 ![삭제](/help/creative/assets/delete.png "삭제")를 클릭합니다.

* 모든 기본 크리에이티브를 삭제하려면 ![삭제](/help/creative/assets/delete.png "삭제") **[!UICONTROL Delete all]**&#x200B;을(를) 클릭합니다.

* 오른쪽의 [크리에이티브] 창을 표시하거나 숨기려면 오른쪽 창의 오른쪽 상단에 있는 ![표시/숨기기](/help/creative/assets/hide-show-creatives.png "표시/숨기기")를 클릭합니다.

## [!UICONTROL Targeting] 섹션

**[!UICONTROL Targeting]:**(기존 경험의 경우 읽기 전용) 의사 결정 트리를 사용하여 타깃팅을 사용하지 않으려는 경우에는 적용할 수 없습니다. 이 옵션은 사용하지 않도록 설정하십시오.

**[!UICONTROL Dynamic ads]:**(기존 경험의 경우 읽기 전용) 경험에 동적 광고가 포함되어 있음을 나타냅니다. **참고:** 경험에는 모든 표준 광고 또는 모든 동적 광고가 포함될 수 있습니다.

**[!UICONTROL Language Targeting]:**(표준 광고만 있는 경험, 선택 사항, 기존 경험의 경우 읽기 전용) 사용자의 브라우저 언어 설정을 확인하고 해당 언어의 크리에이티브를 사용할 수 있는 경우 지정된 언어의 크리에이티브를 표시합니다. 브라우저 지정 언어의 크리에이티브를 사용할 수 없는 경우 대신 [!UICONTROL Preferred language] 설정이 사용됩니다. 경험을 저장하면 이 설정을 변경할 수 없습니다.

**[!UICONTROL Preferred language]:**(표준 광고만 있는 경험, 기존 경험의 경우 읽기 전용) [!UICONTROL Language Targeting]이(가) 활성화된 경우를 제외하고 경험에서 만든 모든 광고의 언어입니다. 경험을 저장하면 이 설정을 변경할 수 없습니다.

## [!UICONTROL Advanced] 섹션

**데이터 패스:**(동적 광고만 있는 경험, 선택 사항) DSP, 게시자 또는 파트너가 노출 시 실시간으로 전달하는 특정 키-값 쌍을 기준으로 사용자를 타깃팅합니다. 최대 5개의 데이터 패스 키(매개 변수)를 지정할 수 있습니다.<!-- May move this to just within the decision tree. -->

나중에 특정 크리에이티브 크기에 대한 광고 경험 태그를 만들면 이 필드에 지정된 각 키가 태그에 매크로로 추가됩니다. 태그를 DSP에 광고로 구현하기 전에 태그 내의 각 키-값 쌍에 대한 값을 입력해야 합니다.

**반경:**(동적 광고만 있는 경험, 선택 사항) 피드 파일에 지정된 미국 우편 번호에서 타깃팅할 반경입니다. 0마일에서 200마일 사이의 반경을 선택하십시오. 경험에 대한 동적 광고를 만드는 데 사용되는 피드 파일에는 파일의 각 제품 행에 대한 값이 있는 [!UICONTROL ZIP] 열<!-- or a user-named column mapped to a ZIP column -->이(가) 포함되어야 합니다. 예를 들어 반경 10마일의 경우, 95110에서 사용 가능한 제품에 대한 광고를 반경 10마일 내의 사용자에게 표시할 수 95110.

**RT 픽셀:**(동적 광고만 있는 경험, 선택 사항) 잠재적으로 타깃팅할 [!UICONTROL Creative] 리타겟팅 픽셀입니다. 의사 결정 트리 내에서 타깃팅을 설정할 때 한 수준의 RT 픽셀 대상 노드를 포함하고 각 노드에 대해 타깃팅할 픽셀과, 할당된 크리에이티브 번들에서 크리에이티브를 표시하기 위해 존재해야 하는 픽셀 속성에 대한 필수 값을 지정할 수 있습니다. 이 필드에 픽셀을 지정하지 않으면 결정 트리 내에서 픽셀을 지정할 수 있습니다.&lt;!— R부터: &quot;RT 픽셀은 동적 광고 설정에서 콘텐츠 선택을 통해 이루어져야 합니다.&quot; — 명확화. 동적 광고 설정에 &quot;Datapass&quot;(한 단어)가 표시되지만 해당 설정과 이 경험 수준 설정이 어떻게 함께 작동하는지 확실하지 않습니다. —>

**[!UICONTROL Label]:** <!-- should be "Labels" -->(선택 사항) 경험에 적용할 모든 [!DNL Creative]별 레이블. 경험<!-- sic --> 보기에서 레이블을 기준으로 경험을 필터링할 수 있습니다.

* 기존 레이블을 선택하려면 ![아래로](/help/creative/assets/chevron-down.png "아래로")를 클릭하고 적용할 각 레이블 옆에 있는 확인란을 선택하십시오.

* 기존 레이블을 검색하려면 레이블 이름 내에 텍스트 문자열 입력을 시작합니다.

* 적용할 새 레이블을 만들려면 목록을 열고 **+ 레이블 추가**&#x200B;를 클릭하고 [!UICONTROL Label] 필드에 새 레이블 이름을 입력한 다음 **만들기**&#x200B;를 클릭합니다.

* 레이블을 제거하려면 레이블 이름 옆에 있는 확인란을 선택 취소합니다.

**[!UICONTROL Impression Tracking URL]:**(선택 사항) 경험에서 만든 모든 광고의 랜딩 페이지 URL에 추가할 타사 노출 추적 URL입니다. 최대 5개의 URL을 포함할 수 있습니다. URL을 추가하려면 ![아이콘](/help/creative/assets/create.png) **[!UICONTROL Add More]을(를) 클릭하고 URL을 입력하십시오.

URL을 입력하면 [사용 가능한 모든 매크로](/help/creative/creative-macros.md)와 이 매크로가 대체되는 데이터가 페이지 아래쪽에 나열됩니다. URL에 매크로 중 하나를 삽입하려면 매크로 설명 위에 커서를 놓고 ![클립보드에 복사](/help/creative/assets/copy-to-clipboard.png "클립보드에 복사")를 클릭한 다음 URL 필드에 매크로를 원하는 위치에 붙여넣습니다.

>[!NOTE]
>
>* [!DNL Creative]은(는) 자신의 노출 추적 태그를 랜딩 페이지 URL에 자동으로 접두사로 추가합니다.
>* 이 URL은 경험의 모든 크리에이티브에 대해 재정의할 수 있습니다.
>* [!UICONTROL Client JS] 필드에 타사 JavaScript 노출 추적 코드를 입력할 수도 있습니다

**[!UICONTROL Click Tracking URL]:** (선택 사항) 랜딩 페이지 URL에 추가할 타사 클릭 추적 URL입니다. 최대 5개의 URL을 포함할 수 있습니다. URL을 추가하려면 ![아이콘](/help/creative/assets/create.png) **[!UICONTROL Add More]**&#x200B;을(를) 클릭하고 URL을 입력하십시오.

URL을 입력하면 [사용 가능한 모든 매크로](/help/creative/creative-macros.md)와 이 매크로가 대체되는 데이터가 페이지 아래쪽에 나열됩니다. URL에 매크로 중 하나를 삽입하려면 매크로 설명 위에 커서를 놓고 ![클립보드에 복사](/help/creative/assets/copy-to-clipboard.png "클립보드에 복사")를 클릭한 다음 URL 필드에 매크로를 원하는 위치에 붙여넣습니다.

>[!NOTE]
>
>* [!DNL Creative]은(는) 자신의 노출 추적 태그를 랜딩 페이지 URL에 자동으로 접두사로 추가합니다.
>* 환경의 모든 Creative <!-- creative bundle for targeted experiences -->에 대해 이 URL을 재정의할 수 있습니다.

**[!UICONTROL Client JS]:**(선택 사항) 다음 중 하나:

* (광고주가 광고에 OBA 준수 공급업체를 사용하는 경우) JavaScript 코드는 사용자가 OBA(온라인 행동 타깃팅)를 옵트아웃할 수 있도록 하는 광고 오버레이를 가리킵니다.

* 랜딩 페이지에 추가할 타사 JavaScript 노출 추적 코드. **참고:** [!UICONTROL Impression Tracking URL] 필드에 타사 노출 추적 URL을 입력할 수도 있습니다.

>[!MORELIKETHIS]
>
>* [의사 결정 트리 타깃팅 없이 경험 만들기](experience-create-no-targeting.md)
>* [의사 결정 트리 타깃팅 없이 경험 편집](experience-edit-no-targeting.md)
>* [추적 URL에 사용할 수 있는 매크로](/help/creative/creative-macros.md)
>* [적용 가능한 광고 크기에 대한 광고 태그를 수동으로 만듭니다](experience-tag-create-manually.md)
>* [타깃팅이 없는 경험에 대한 광고 태그에 크리에이티브를 할당](experience-tag-assign-creatives.md)
>* [타깃팅하지 않고 경험에 대한 추적 URL 사용자 지정](experience-tracking-urls-no-targeting.md)
>* [타깃팅하지 않고 경험에 대한 크리에이티브 최적화 및 일정 사용자 지정](experience-optimization-scheduling-no-targeting.md)
