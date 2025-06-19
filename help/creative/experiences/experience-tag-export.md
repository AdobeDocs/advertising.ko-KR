---
title: 라이브 경험을 위한 광고 경험 태그 내보내기 및 구현
description: 광고 경험 태그를 내보내고 선택적으로 Advertising DSP 캠페인에 업로드하는 방법을 알아봅니다.
feature: Creative Experiences
exl-id: 4ae05142-8319-4329-96d7-f87d77f02745
source-git-commit: f2bf245c13244cbcb76cead8b37f149b9b9bc24f
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 0%

---

# 라이브 경험을 위한 광고 경험 태그 내보내기 및 구현

*베타가 닫힘*

특정 크리에이티브 크기의 광고 태그를 [live](experience-about.md#experience-statuses) 경험에 사용할 수 있게 되면, Advertising DSP 또는 기타 DSP에서 구현할 수 있도록 태그를 JavaScript 및 iframe 형식으로 생성하고 복사할 수 있습니다. DSP의 태그에는 DSP에 필요한 모든 매크로가 포함됩니다.

Advertising DSP을 사용하는 광고주는 선택적으로 광고 유형이 &quot;표준 디스플레이&quot;인 광고로 Advertising DSP 캠페인에 태그를 직접 업로드할 수 있습니다.

>[!NOTE]
>
>* 의사 결정 트리 타깃팅으로 경험을 만들면 [!DNL Creative]에서 적용 가능한 각 광고 크기에 대한 광고 태그를 자동으로 만듭니다.
>* 의사 결정 트리 타깃팅이 없는 경험을 만드는 경우 적용 가능한 각 광고 크기에 대해 [수동으로 광고 태그를 만들어야](experience-tag-create-manually.md) 합니다.
>* 경험 태그는 동적입니다. 경험을 편집하는 경우 태그를 업데이트할 필요가 없습니다.
>* 광고 경험을 구현할 캠페인에 경험과 호환되는 타겟팅이 포함되어 있는지 확인하십시오. 계층 타겟팅 동작은 DSP에 따라 다를 수 있습니다. Advertising DSP에서 광고 수준 타깃팅은 배치 수준 타깃팅 (대신 적용되지 않음) 위에 적용됩니다.

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Experiences]**&#x200B;을(를) 클릭합니다.

1. 다음 중 하나를 실행하십시오.<!-- I see multiselect, but it's not actually working for me as of 2/3 so I don't know how exporting multiple tags works.-->

   * 카드 보기에서 경험 이름 옆의 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Tag Manager]**&#x200B;을(를) 클릭합니다.

   * 테이블 보기에서 행 위에 커서를 놓고 **[!UICONTROL More]**&#x200B;을 클릭한 다음 **[!UICONTROL Tag Manager]**&#x200B;을(를) 클릭합니다

1. 적용 가능한 광고 태그의 행 위에 커서를 놓고 ![광고 태그 내보내기](/help/creative/assets/export.png "광고 태그 내보내기") **[!UICONTROL Export ad tags]** 또는 **[!UICONTROL ... More] > &#x200B;** [!UICONTROL Export ad tags]**&#x200B;를 클릭합니다.

<!-- Tag Manager has only a list view, but no card view, as of 2/2. -->

1. (선택 사항) [!UICONTROL Macros] 탭에서 태그에 포함할 사용자 지정 매크로를 최대 5개까지 지정합니다. 포함할 각 매크로에 대해:

   1. 확인란을 선택하십시오.<!-- Explain more -->

   1. 사용자 지정 매크로를 입력하십시오.<!-- Explain more -->

1. 오른쪽 상단의 **[!UICONTROL Next]**&#x200B;을(를) 클릭하거나 왼쪽 메뉴에서 **[!UICONTROL Generate ad tags]**&#x200B;을(를) 클릭합니다.

1. 태그 형식을 선택하십시오. ** *JavaScript<!-- sic -->* **&#x200B; 또는 &#x200B;** *IFRAME* ** <!-- sic -->.

1. [!UICONTROL Destinations] 목록에서 경험을 위한 광고를 만들 위치를 선택합니다.

   * *일반:* 다른 DSP에서 만들 광고의 경우. **참고:** 필요에 따라 [추가 매크로](/help/creative/creative-macros.md)를 수동으로 포함해야 할 수도 있습니다.

   * Advertising DSP에서 만들 광고의 경우 *Adobe AdCloud:*.

   * [!DNL Google Campaign Manager 360]에 만들 광고의 경우 *Google CM360:*. **참고:** 필요에 따라 [추가 매크로](/help/creative/creative-macros.md)를 수동으로 포함해야 할 수도 있습니다.

1. **[!UICONTROL Generate tags]**&#x200B;을(를) 클릭합니다.

1. 태그 복사 또는 다운로드:

   * 단일 광고 크기에 대한 태그를 복사하려면 태그 행을 확장하고 행 위에 커서를 놓은 다음 ![복사](/help/creative/assets/copy.png "복사") **[!UICONTROL Copy]**&#x200B;을 클릭합니다.<!-- why diff than "Copy to clipboard icon used to copy macros for creatives? -->

   * 생성된 모든 태그를 브라우저의 기본 다운로드 위치에 파일로 다운로드하려면 ![태그 다운로드](/help/creative/assets/download.png "태그 다운로드")를 클릭합니다.

   텍스트 편집기에서 파일을 열어 각 태그를 복사할 수 있습니다. JavaScript 태그의 경우 태그는 `<script></script>` 및 `<noscript></noscript>`개의 태그로 묶여 있습니다. iframe 태그의 경우 태그는 `<iframe></iframe>` 태그로 묶여 있습니다.

1. 관련 DSP에 대한 태그를 구현합니다.

   * Advertising DSP 이외의 DSP의 경우 DSP 내에서 광고를 만들 모든 사용자에게 태그를 제공합니다.

   * Advertising DSP의 경우

      1. 오른쪽 상단의 **[!UICONTROL Next]**&#x200B;을(를) 클릭하거나 왼쪽 메뉴에서 **[!UICONTROL DSP link]**&#x200B;을(를) 클릭합니다.

      1. 광고 태그를 업로드할 캠페인을 선택합니다.

      1. **[!UICONTROL Assign Tags]**&#x200B;을(를) 클릭합니다.

         DSP이 선택한 캠페인에 대한 [!UICONTROL Ads] 보기로 열립니다.

      1. [!UICONTROL Create ads] 보기에서 광고 태그를 검토하고 광고를 만들 각 태그를 선택한 다음 **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.


<!-- no way to get back to the Creative Tag Manager -- you have to click back through the main menu -->

<!-- Add this info, with descriptions:

## Ad tag formats

### JavaScript

### Iframe

-->

>[!MORELIKETHIS]
>
>* [적용 가능한 광고 크기에 대한 광고 태그를 수동으로 만듭니다](experience-tag-create-manually.md)
>* [타깃팅이 없는 경험에 대한 광고 태그에 크리에이티브를 할당](experience-tag-assign-creatives.md)
>* [광고 태그 이름 바꾸기](experience-tag-rename.md)
