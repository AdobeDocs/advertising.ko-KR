---
title: Creative 라이브러리에 동적 크리에이티브 추가
description: Creative Library에 동적 크리에이티브를 추가하는 방법을 알아봅니다.
feature: Creative Dynamic Creatives
source-git-commit: 9aeb35ec5aba1c6c4c7683487ed3c0a0e22accb8
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---

# Creative 라이브러리에 동적 크리에이티브 추가

동적 [광고 경험](creative-library-manage.md)에서 사용할 동적 크리에이티브를 [크리에이티브 라이브러리](/help/creative/experiences/experience-about.md)에 추가하십시오. 단일 광고 템플릿에서 하나의 정적 HTML5 광고 또는 동적 HTML5 광고를 만들 수 있습니다. 동적 HTML5 광고의 경우 피드 파일에서 생성된 지정된 카탈로그의 에셋을 사용합니다.

>[!PREREQUISITES]
>
>크리에이티브 라이브러리에 동적 크리에이티브를 추가하려면 먼저 광고 템플릿 만들기, 에셋 업로드 및 피드 템플릿 및 카탈로그 만들기(동적 HTML5 광고) 등의 다른 단계를 완료해야 합니다. &quot;[동적 광고용 워크플로우](/help/creative/introduction/workflow-dynamic-ads.md)&quot;를 참조하십시오.

<!-- This does't work for me 9/24 -- I still have to select a catalog:

## Add dynamic creatives using a static HTML5 ad template

1. In the main menu, click **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**.

1. Click the library name.

1. On the **[!UICONTROL Creatives]** tab, click **[!UICONTROL Create]** > **[!UICONTROL Creatives]** > **[!UICONTROL Dynamic Ad]**.

1. Specify the [dynamic ad settings](/help/creative/creative-libraries/creative-settings-dynamic.md#dynamic-ad-settings-static-html5):

   1. On the [!UICONTROL Basic Details] tab, specify the ad details and the clickURL.

   1. Click **[!UICONTROL Process]**.

   1. On the [!UICONTROL Attributes Details] tab, specify the dynamic ad attributes.

1. Click **[!UICONTROL Save]**.

-->

## 동적 HTML5 광고 템플릿을 사용하여 동적 크리에이티브 추가

1. 다음 중 하나를 수행합니다.

   * 크리에이티브 라이브러리에서:

      1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

      1. 라이브러리 이름을 클릭합니다.

      1. **[!UICONTROL Creatives]** 탭에서 **[!UICONTROL Create]** > **[!UICONTROL Creatives]** > **[!UICONTROL Dynamic Ad]**&#x200B;을(를) 클릭합니다.

   * 광고 템플릿에서:

      1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Ad Templates]**&#x200B;을(를) 클릭합니다.

      1. 광고 템플릿 행 위에 커서를 놓고 **[!UICONTROL Create Dynamic Ad]**&#x200B;을(를) 클릭합니다.

1. [동적 광고 설정 지정](/help/creative/creative-libraries/creative-settings-dynamic.md):

   1. 기본 광고 세부 정보를 지정합니다.

   1. 광고 크리에이티브에 사용할 광고 템플릿을 선택합니다.

   1. 광고를 제작할 카탈로그를 선택하십시오.

   1. 광고를 만드는 데 사용할 카탈로그 행의 기준을 선택하십시오.

   1. 지정된 광고 템플릿의 각 속성(동적 광고 필드)을 지정된 피드 파일(카탈로그 레이블)의 열에 매핑합니다.

   1. 생성할 크리에이티브를 미리 보려면 **[!UICONTROL Continue]**&#x200B;을(를) 클릭하십시오. 미리보기 내에서 다음 중 하나를 수행할 수 있습니다.

      * 카탈로그, 필터 값 <!-- explain more--> 및 광고 크기별로 광고 크리에이티브를 필터링하려면 미리 보기 영역 위의 필터를 사용하십시오.

      * 미리 보기 영역 아래의 검색 필드에서 고유 ID로 제품을 검색합니다.

      * 표시되는 열을 변경하려면 미리 보기 영역 아래의 ![열 필터](/help/creative/assets/custom-columns. "열 필터")를 클릭하십시오.

      * 특정 크리에이티브를 미리 보려면 행의 확인란을 선택합니다.

      * 콘텐츠 변경:

         * 테이블 내에서 셀 값을 편집하려면 셀 내부를 누르고 값을 편집합니다. 셀 외부를 클릭하거나 **[!DNL Enter]** 키를 눌러 변경 내용을 저장합니다.

         * 단일 제품을 기본값 <!--Explain what this means. -->(으)로 표시하려면 행 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Set as Default]**&#x200B;을(를) 클릭합니다.

         * (광고에 두 개 이상의 오퍼가 포함된 경우) 여러 제품을 기본값으로 표시하려면 행(최대 오퍼 수)을 선택하고 일괄 작업 도구 모음에서 **[!UICONTROL Set as Default]**&#x200B;을(를) 클릭합니다.

      * 카탈로그에서 제품을 삭제하려면 행 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Delete Row]**&#x200B;을(를) 클릭합니다.

      * (광고에 두 개 이상의 오퍼가 포함된 경우) 카탈로그에서 여러 제품을 삭제하려면 행(최대 오퍼 수)을 선택하고 일괄 작업 도구 모음에서 **[!UICONTROL Delete Row]**&#x200B;을(를) 클릭합니다.

1. 크리에이티브를 저장합니다.

   * 광고를 저장하고 라이브러리의 [크리에이티브 번들](/help/creative/creative-libraries/bundle-manage.md)에 추가하려면:

      1. **[!UICONTROL Save and Attach to Bundle]**&#x200B;을(를) 클릭합니다.

      1. **[!UICONTROL Save]**&#x200B;을(를) 클릭하여 광고를 저장합니다.

      1. 번들을 선택한 다음 **[!UICONTROL Attach Creative to Bundles]**&#x200B;을(를) 클릭합니다.

   * 광고를 저장하고 설치를 종료하려면 **[!UICONTROL Save]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Save]**&#x200B;을(를) 다시 클릭합니다.

>[!MORELIKETHIS]
>
>* [동적 크리에이티브 설정](creative-settings-dynamic.md)
>* [Creative 라이브러리에서 동적 크리에이티브 편집](creative-edit-dynamic.md)
>* [동적 광고용 워크플로](/help/creative/introduction/workflow-dynamic-ads.md)
