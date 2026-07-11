---
title: Creative Studio에서 에셋 관리
description: Adobe Advertising Creative의 Creative Studio Assets 탭에서 에셋을 업로드, 검색 및 관리하는 방법을 알아봅니다.
product_v2: id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2: id: d0d9f2ed-c163-44e1-97a1-4ace121416b8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 24e27656edda50f29292cb75823ef6cacdb685fe
workflow-type: tm+mt
source-wordcount: 292
ht-degree: 0%

---

# [!UICONTROL Creative Studio]에서 자산 관리

*Beta 기능*

광고 템플릿에서 참조할 이미지, 비디오, 오디오 및 글꼴 자산을 업로드하고 광고 생성 세션 중에 AI 에이전트 채팅 메시지에 첨부합니다.

## [!UICONTROL Creative Studio] > [!UICONTROL Assets] 보기

**[!UICONTROL Assets]** 탭에는 카드 보기에 있는 기존 자산이 나열됩니다.

### 사용 가능한 작업

<!--  * [Browse and search assets](#assets-search) -->

* [에셋 업로드](#assets-upload)

* [에셋 이름 바꾸기](#assets-rename)

* [에셋 다운로드](#assets-download)

* [에셋 삭제](#assets-delete)

<!--

Should be in "Common Tasks" chapter

## Browse and search assets {#assets-search}

* Use the **[!UICONTROL Search assets]** field to find assets by name. Enter at least three characters to trigger a search; shorter queries don't filter results.
* Click **[!UICONTROL Filter]** to filter the asset library by type or other attributes.

-->

## 에셋 업로드 {#assets-upload}

1. 주 메뉴에서 **[!UICONTROL Creative Studio].**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Assets]** 탭을 클릭합니다.

1. **[!UICONTROL Upload Assets]**&#x200B;을(를) 클릭합니다.

1. 컴퓨터 또는 네트워크에서 하나 이상의 파일을 선택합니다.

   지원되는 파일 유형은 다음과 같습니다.

   <!-- Verified 2026-07-09 against creative-api TemplateMediaValidator.java (IMAGE_EXTENSIONS, VIDEO_EXTENSIONS, AUDIO_EXTENSIONS), which backs the /v1/creative/template-medias upload/initiate endpoint used by this tab. The Assets tab file input has no client-side accept restriction (TemplateBrowser.tsx) and relies entirely on this backend validator, so it is authoritative. -->

   | 유형 | 지원되는 형식 | 최대 파일 크기 |
   | --- | --- | --- |
   | 이미지 | JPG/JPEG, PNG, GIF, WebP, SVG | 10MB |
   | 비디오 | MP4, MOV, AVI, WebM | 512메가바이트 |
   | 오디오 | MP3, WAV, AAC, OGG | 50MB |

   오류 알림과 함께 빈 파일 및 지원되지 않는 파일 유형이 거부됩니다.

   자산 이름은 확장명 없이 업로드된 파일 이름으로 저장됩니다. 파일 이름의 공백 및 비 ASCII 문자는 밑줄로 대체됩니다. 예를 들어 `My Logo.png`을(를) 업로드하면 이름이 `My_Logo`인 자산이 만들어집니다. 에셋의 이름은 나중에 변경할 수 있습니다.

<!--

maybe later:

   | Fonts | TTF, OTF, WOFF, WOFF2 | 5 MB |
   
-->

## 에셋 이름 편집 {#asset-rename}

1. 주 메뉴에서 **[!UICONTROL Creative Studio].**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Assets]** 탭을 클릭합니다.

1. 자산 카드 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Edit name]**&#x200B;을(를) 클릭합니다.

1. 에셋 이름을 업데이트합니다.

   에셋 이름은 최대 512자까지 가능합니다.

1. **[!UICONTROL Update]**&#x200B;을(를) 클릭합니다.

## 에셋 다운로드 {#asset-download}

1. 주 메뉴에서 **[!UICONTROL Creative Studio].**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Assets]** 탭을 클릭합니다.

1. 자산 카드 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Download]**&#x200B;을(를) 클릭합니다.

   브라우저의 일반 절차에 따라 에셋이 다운로드됩니다.

## 에셋 삭제 {#asset-delete}

>[!NOTE]
>
>삭제된 에셋은 다시 활성화할 수 없습니다.

1. 주 메뉴에서 **[!UICONTROL Creative Studio].**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Assets]** 탭을 클릭합니다.

1. 자산 카드 위에 커서를 놓고 **[!UICONTROL ...]** > **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [Advertising Creative의 Creative Studio 정보](creative-studio-about.md)
>* [Creative Studio에서 템플릿 관리](creative-studio-manage-templates.md)
>* [Creative Studio에서 표준 광고 생성](creative-studio-manage-standard-ads.md)
