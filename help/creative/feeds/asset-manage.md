---
title: 에셋 파일 관리
description: 광고주를 위한 에셋 파일을 업로드하고 관리하는 방법을 알아봅니다.
feature: Creative Dynamic Creatives
source-git-commit: 6f2f6580e8d4fc11f52a97b086ce453e423ab4e6
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---

# 에셋 파일 관리

Dynamic HTML5 광고에는 XLSX(Microsoft Excel 스프레드시트) 형식의 피드 파일과 스프레드시트에서 참조되는 이미지 자산이 모두 필요합니다(Adobe Experience Manager 자산 참조 제외). 정적 HTML5 광고에는 광고당 하나의 이미지 자산만 필요합니다.

>[!NOTE]
>
> 각 피드 파일은 하나의 카탈로그에 대해서만 사용할 수 있습니다.

## 파일 요구 사항

* Dynamic HTML5 광고:

   * 각 광고 변형에 대해 하나의 헤더 행과 하나의 데이터 행이 있는 Microsoft Excel 스프레드시트(XLSX) 형식의 피드 파일입니다. 각 행에 이미지 이름 또는 Adobe Experience Manager에 대한 참조를 포함하십시오.<!-- need spec of available column names that the user-created header names must map to; need to reference it in feed template topic too, so make it a separate file/appendix. -->

     업로드할 이미지의 경우 `images/image_name` 형식(예: `images/300x250_acme_logo.png`)을 사용하여 이미지를 참조합니다.<!-- Verify.  Also need to include the spec for how to reference images in AEM -->

   * GIF, JPEG, JPG 또는 PNG 형식의 연결된 이미지 자산입니다.<!-- NOT GIF still? And is this true: The maximum file size is two (2) MB. --> [지원되는 크리에이티브 크기](/help/creative/creative-libraries/creative-sizes.md)를 참조하십시오.

  하나의 XLSX 파일, 하나의 이미지 파일 또는 XLSX와 이미지 파일의 조합이 포함된 하나의 ZIP 파일을 업로드할 수 있습니다.<!-- Check w/eng re any limitations or best practices WRT number of files and filesize allowed -->

* 정적 HTML5 광고:

   * GIF, JPG, JPEG 또는 PNG 형식의 광고당 하나의 이미지 에셋.

     ZIP 파일에 단일 이미지 또는 여러 이미지를 업로드할 수 있습니다.<!-- Check w/eng re any limitations or best practices WRT number of files and filesize allowed -->

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
>* [동적 광고용 워크플로](/help/creative/introduction/workflow-dynamic-ads.md)
>* [피드 템플릿 관리](/help/creative/feeds/feed-template-manage.md)
>* [카탈로그 관리](/help/creative/feeds/catalog-manage.md)
>* [동적 광고 템플릿 관리](/help/creative/ad-templates/ad-template-manage.md)
>* [Creative 라이브러리에 동적 크리에이티브 추가](/help/creative/creative-libraries/creative-add-dynamic.md)
