---
title: 에셋 파일 관리
description: 광고주를 위한 에셋 파일을 업로드하고 관리하는 방법을 알아봅니다.
feature: Creative Dynamic Creatives
exl-id: 2fe2d778-8456-490a-bf44-234dbc08649f
source-git-commit: 4e809ac18720f22f636b2df2ad4a5b1db355e729
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 0%

---

# 에셋 파일 관리

* Dynamic HTML5 광고에는 Microsoft Excel 스프레드시트(XLSX) 형식의 피드 파일과 스프레드시트에서 참조되는 실제 이미지 자산이 필요합니다.

* 정적 HTML5 광고에는 광고당 하나의 이미지 자산만 필요합니다.

* 비디오 광고에는 Microsoft Excel 스프레드시트(XLSX) 형식의 피드 파일과 스프레드시트에서 참조되는 실제 비디오 자산이 필요합니다.

>[!NOTE]
>
> 각 피드 파일은 하나의 카탈로그에 대해서만 사용할 수 있습니다.

## 파일 요구 사항

* Dynamic HTML5 광고:

   * CSV, TSV 또는 Microsoft Excel 스프레드시트(XLSX) 형식의 피드 파일로, 각 광고 변형에 대해 하나의 머리글 행과 하나의 데이터 행이 있습니다. `images/image_name` 형식(예: `images/300x250_acme_logo.png`)을 사용하여 각 행에 이미지 이름을 포함하십시오.

     광고주별 필드 이름은 [동적 광고 피드 파일에 사용 가능한 필드](/help/creative/appendix-available-feed-fields.md)에 매핑해야 합니다.

   * GIF, JPEG, JPG 또는 PNG 형식의 연결된 이미지 자산입니다.<!-- Is this true: The maximum file size is two (2) MB. --> [지원되는 크리에이티브 크기](/help/creative/creative-libraries/creative-sizes.md)를 참조하십시오.

  하나의 XLSX 파일, 하나의 이미지 파일 또는 XLSX와 이미지 파일의 조합이 포함된 하나의 ZIP 파일을 업로드할 수 있습니다.<!-- Check w/eng re any limitations or best practices WRT number of files and filesize allowed -->

* 정적 HTML5 광고:

   * GIF, JPG, JPEG 또는 PNG 형식의 광고당 하나의 이미지 에셋.

     ZIP 파일에 단일 이미지 또는 여러 이미지를 업로드할 수 있습니다.<!-- Check w/eng re any limitations or best practices WRT number of files and filesize allowed -->

* 동적 비디오 광고:

   * CSV, TSV 또는 Microsoft Excel 스프레드시트(XLSX) 형식의 피드 파일로, 각 광고 변형에 대해 하나의 머리글 행과 하나의 데이터 행이 있습니다. `videos/image_name` 형식(예: `videos/300x250_acme_logo.png`)을 사용하여 각 행에 비디오 이름을 포함하십시오. ZIP 파일은 최대 500개의 행에서 최대 512MB일 수 있습니다.

     광고주별 필드 이름은 [동적 광고 피드 파일에 사용 가능한 필드](/help/creative/appendix-available-feed-fields.md)에 매핑해야 합니다.

     다이내믹 비디오가 있는 모든 계정의 경우 가장 좋은 방법은 자산 파일의 각 필드를 Advertising Creative 백엔드의 필드에 매핑하는 [마스터 피드 템플릿 &#x200B;](catalog-manage.md)의 복사본과 함께 자산 파일을 사용하여 [카탈로그를 만들기[!UICONTROL Adobe Creative Template]](feed-template-manage.md)하는 것입니다.

   * MP4, MOV 또는 WEBM 형식의 연결된 비디오 자산입니다. 지원되는 광고 템플릿에는 시작 카드, 끝 카드, 상단 오버레이, 하단 오버레이 또는 L자형 등이 있습니다. 각 비디오의 재생 시간은 1~90초 사이여야 합니다. [지원되는 크리에이티브 크기](/help/creative/creative-libraries/creative-sizes.md)를 참조하세요.

  하나의 XLSX 파일, 하나의 이미지 파일 또는 XLSX와 비디오 파일의 조합이 포함된 하나의 ZIP 파일을 업로드할 수 있습니다.<!-- Check w/eng re any limitations or best practices WRT number of files and filesize allowed -->

## 에셋 파일 업로드

>[!NOTE]
>
>에셋 파일을 업로드하는 대신 [Creative 라이브러리에 동적 크리에이티브를 추가](/help/creative/creative-libraries/creative-add-dynamic.md)할 때 카탈로그를 직접 업로드할 수도 있습니다. 만든 모든 카탈로그는 나중에 사용할 수 있도록 [!UICONTROL Catalogs] 보기 내에서 사용할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Feeds]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Assets]** 탭을 클릭합니다.

1. 오른쪽 상단에서 **[!UICONTROL Create]** > **[!UICONTROL Asset]**&#x200B;을(를) 클릭합니다.

1. 에셋 파일을 구성합니다.

   1. 자산 파일에 액세스할 수 있는 광고주를 선택합니다.

   1. 다음 방법 중 하나로 에셋 파일을 지정합니다.

      * 장치 또는 네트워크에 있는 파일을 상자로 끌어서 놓습니다.

      * 장치 또는 네트워크에서 파일을 찾으려면 **[!UICONTROL Select a file]**&#x200B;을(를) 클릭하십시오.

   1. **[!UICONTROL Upload]**&#x200B;을(를) 클릭합니다.

모든 ZIP 파일은 자동으로 압축 해제됩니다. 스프레드시트 파일을 업로드하면 파일이 [!UICONTROL Feeds] 하위 탭에 나열됩니다. 이미지 파일을 업로드하면 이미지 파일이 [!UICONTROL Images] 하위 탭에 나열됩니다.

## 에셋 파일 다운로드

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Feeds]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Assets]** 탭을 클릭합니다.

1. 자산 행 위에 커서를 놓고 **[!UICONTROL Download]**&#x200B;을(를) 클릭합니다.

   브라우저의 일반적인 절차에 따라 파일이 다운로드됩니다.

## 에셋 파일 삭제

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Feeds]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Assets]** 탭을 클릭합니다.

1. 자산 행 위에 커서를 놓고 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [동적 광고 피드 파일에 사용할 수 있는 필드](/help/creative/appendix-available-feed-fields.md)
>* [동적 광고용 워크플로](/help/creative/introduction/workflow-dynamic-ads.md)
>* [피드 템플릿 관리](/help/creative/feeds/feed-template-manage.md)
>* [카탈로그 관리](/help/creative/feeds/catalog-manage.md)
>* [동적 광고 템플릿 관리](/help/creative/ad-templates/ad-template-manage.md)
>* [Creative 라이브러리에 동적 크리에이티브 추가](/help/creative/creative-libraries/creative-add-dynamic.md)
