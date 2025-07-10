---
title: 크리에이티브 라이브러리에 표준 크리에이티브 추가
description: 크리에이티브 라이브러리에 표준(비동적) 크리에이티브를 추가하는 방법을 알아봅니다.
feature: Creative Standard Creatives
exl-id: e6f1265b-9d05-4b3d-9dc6-300dbd9eb52d
source-git-commit: bc3309523572656362cebebab9b735530003a81c
workflow-type: tm+mt
source-wordcount: '1001'
ht-degree: 0%

---

# 크리에이티브 라이브러리에 표준 크리에이티브 추가

*베타가 닫힘*

[광고 경험](creative-library-manage.md)에서 사용할 크리에이티브 라이브러리를 [추가](/help/creative/experiences/experience-about.md)합니다.

>[!NOTE]
>
> 사용자 타겟이 정의되지 않은 광고 경험 내에 개별 크리에이티브를 직접 포함할 수 있습니다. 광고 타겟팅 경험에 포함할 수 있는 [번들](bundle-manage.md)에서 광고 크리에이티브를 그룹화할 수도 있습니다.

## 크리에이티브 라이브러리에 유연한 HTML 광고 추가 {#flexible-creative-add}

다음 중 하나를 수행할 수 있습니다.

* ZIP 파일에 자신의 유연한 크리에이티브를 업로드하십시오.

* 계정에 업로드된 사전 정의된 유연한 크리에이티브 템플릿을 자신의 유연한 크리에이티브를 위한 시작점으로 사용합니다.

### 자신만의 유연한 크리에이티브 업로드 {#flexible-creative-upload}

여러 개의 유연한 크리에이티브 단위를 업로드할 수 있습니다. 유연한 크리에이티브는 ZIP 형식이어야 하며, 최대 2MB일 수 있습니다. 파일 요구 사항은 [HTML5 Creative 사양](html5-creative-specification.md)을 참조하십시오.

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

1. 라이브러리 이름을 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 **[!UICONTROL Standard Ads]** 하위 탭을 클릭합니다.

1. **[!UICONTROL Create]** > **[!UICONTROL Creative]** > **[!UICONTROL Flexible]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Upload New]**&#x200B;을(를) 클릭합니다.

1. 다음 방법 중 하나로 ZIP 파일을 지정합니다.

   * 장치나 네트워크의 파일을 상자로 끌어서 놓습니다.

   * 장치 또는 네트워크에서 파일을 찾으려면 **[!UICONTROL Select a file]**&#x200B;을(를) 클릭하십시오.

   [유연한 광고 사양](#flexible-ad-spec)을 참조하세요.

1. 유연한 크리에이티브 파일 추가 또는 제거:

   * 파일을 추가하려면 왼쪽 상단의 ![추가](/help/creative/assets/create.png "추가")를 클릭하고 장치나 네트워크에서 파일을 찾습니다.

   * 파일을 제거하려면 해당 파일 옆에 있는 확인란을 선택 취소합니다.

1. [유연한 HTML5 광고 설정](/help/creative/creative-libraries/creative-settings-standard.md#creative-settings-flexible-html5)을 지정하십시오.

   기본적으로 방금 업로드한 모든 크리에이티브가 선택됩니다. 값이 하나만 있는 설정은 선택한 모든 크리에이티브에 적용됩니다. 일부 설정의 경우 개별 값을 지정할 수 있습니다. 특정 크리에이티브에 대한 설정을 입력하려면 적용할 수 없는 각 크리에이티브 옆의 확인란을 선택 취소합니다.

1. **[!UICONTROL Create]** 클릭

### 템플릿을 사용하여 유연한 크리에이티브 추가 {#flexible-creative-use-template}

계정에 업로드된 유연한 크리에이티브 템플릿을 사용하여 사전 정의 크기의 광고를 작성할 수 있습니다. 사용할 템플릿을 선택하면 클릭 태그 및 속성이 편집됩니다.&lt;!— 템플릿 다운로드 기능을 다시 추가하는 경우 마지막 문장을 다음으로 바꾸기: a\) 사용할 템플릿을 선택한 다음 클릭 태그 및 특성을 편집할 수 있습니다. 또는 b\) [템플릿을 ZIP 파일로 다운로드](#download-flexible-creative-template), 콘텐츠를 오프라인으로 편집하여 자체 크리에이티브를 만든 다음 [편집된 파일을 새 크리에이티브로 업로드](flexible-creative-upload)할 수 있습니다.>

<!-- Not currently an option:
You can use any of the [predefined flexible creative templates](flexible-html5-templates.md) included with [!DNL Creative] to build 160x600, 300x250, 300x600, or 728x90 ads.

For information about the attributes available in predefined templates, see "[Available flexible creative templates](#flexible-creative-templates-available)."
-->

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

1. 라이브러리 이름을 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 **[!UICONTROL Standard Ads]** 하위 탭을 클릭합니다.

1. **[!UICONTROL Create]** > **[!UICONTROL Creative]** > **[!UICONTROL Flexible]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Browse System Flexible Templates]**&#x200B;을(를) 클릭합니다.

<!-- Not options as of 5/22/25:

1. In the left panel, select the creative size to see all available templates for that size.

1. Select the template:

   * In card view, click **[!UICONTROL ...]** next to the template name, and then click **[!UICONTROL Use Selected]**.
     
   * In table view, hold the cursor over the row and click **[!UICONTROL Use Selected]**.
-->

1. (선택 사항) 템플릿을 미리 보려면 템플릿 이름 옆에 있는 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Preview]**&#x200B;을(를) 클릭합니다.

   템플릿을 선택적으로 다운로드할 수 있습니다

1. 템플릿 이름 옆에 있는 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Use Selected]**&#x200B;을(를) 클릭합니다.

1. 언어를 지정하고 자신의 클릭 태그, 이미지 및 기타 특성을 포함하도록 [유연한 HTML5 Creative 설정](/help/creative/creative-libraries/creative-settings-standard.md#creative-settings-flexible-html5)을 편집합니다.

   크리에이티브가 압축되면 최대 파일 크기는 2MB입니다.<!-- Still true? -->

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

## 크리에이티브 라이브러리에 HTML5 크리에이티브 추가

단일 유형(단순 또는 정적)의 여러 HTML5 크리에이티브를 한 번에 추가할 수 있습니다.

<!-- Add in when we add this feature back:
You can optionally download a sample HTML5 creative as a ZIP file, edit the contents to build your own creative, and then add the edited file as a new creative.
-->

>[!NOTE]
>
>[ 내에서 직접 편집할 수 있는 표준 HTML 태그로 모든 특성을 가진 HTML5 크리에이티브인 ](#flexible-creative-add)유연한 HTML5 크리에이티브를 추가[!DNL Creative]할 수도 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

1. 라이브러리 이름을 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 **[!UICONTROL Standard Ads]** 하위 탭을 클릭합니다.

1. **[!UICONTROL Create]** > **[!UICONTROL Creative]** > **[!UICONTROL HTML5]**&#x200B;을(를) 클릭합니다.

<!-- Not an option as of 3/4:

1. (Optional) To download a sample HTML5 creative as a ZIP file, click **Sample HTML5 Creatives**.

   The ZIP file is downloaded according to your browser's normal procedure, usually to the folder that is specified for downloads. 
   
   To create your own HTML5 creative using the sample, unzip the file and edit the contents to include your own ad images and attributes. Then, rename the folder and zip it, and continue below.

-->

1. 다음 방법 중 하나로 파일을 지정합니다.

   * 장치나 네트워크의 파일을 상자로 끌어서 놓습니다.

   * 장치 또는 네트워크에서 파일을 찾으려면 **[!UICONTROL Select a file]**&#x200B;을(를) 클릭하십시오.

   [HTML5 광고 사양](/help/creative/creative-libraries/html5-creative-specification.md)을 참조하세요.

1. [HTML5 광고 설정](/help/creative/creative-libraries/creative-settings-standard.md#creative-settings-html5)을 지정하십시오.

기본적으로 방금 업로드한 모든 크리에이티브가 선택됩니다. 값이 하나만 있는 설정은 선택한 모든 크리에이티브에 적용됩니다. 일부 설정의 경우 개별 값을 지정할 수 있습니다. 특정 크리에이티브에 대한 설정을 입력하려면 적용할 수 없는 각 크리에이티브 옆의 확인란을 선택 취소합니다.

1. **[!UICONTROL Create]** 클릭

## 광고 라이브러리에 이미지 광고 추가

GIF, JPEG, JPG 또는 PNG 형식의 이미지를 만들 수 있습니다. 최대 파일 크기는 2MB입니다. [지원되는 크리에이티브 크기](/help/creative/creative-libraries/creative-sizes.md)를 참조하세요.

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

1. 라이브러리 이름을 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 **[!UICONTROL Standard Ads]** 하위 탭을 클릭합니다.

1. **[!UICONTROL Create]** > **[!UICONTROL Creative]** > **[!UICONTROL Image]**&#x200B;을(를) 클릭합니다.

1. 이미지를 지정합니다.

   * 로컬 이미지 에셋의 경우 다음 중 하나를 수행합니다.

      * 장치나 네트워크의 파일을 상자로 끌어서 놓습니다.

      * 장치 또는 네트워크에서 파일을 찾으려면 **[!UICONTROL Select a file]**&#x200B;을(를) 클릭하십시오.

   * DSP 계정에 연결된 [Adobe Experience Manager 라이브러리](/help/creative/creative-libraries/aem-assets-configure.md)에서 승인된 이미지의 경우 다음을 수행하십시오.

      1. **[!UICONTROL AEM Asset Library]**&#x200B;을(를) 클릭합니다.

      1. Experience Manager 계정에 로그인합니다.

      1. [!UICONTROL Assets] 또는 [!UICONTROL Collections] 보기에서 파일을 찾아 선택한 다음 오른쪽 상단의 **[!UICONTROL Select]**&#x200B;을(를) 클릭합니다.

         <!-- If the existing asset has multiple quality options, [!DNL Creative] downloads the primary asset, or the asset with the highest resolution within some upper limit [verify what it is and how this works]. [If an asset is part of an image set, ... primary asset in the image set. -->

1. 이미지 추가 또는 제거:

   * 이미지를 추가하려면 왼쪽 상단의 ![추가](/help/creative/assets/create.png "추가")를 클릭하고 장치나 네트워크에서 파일을 찾습니다.

   * 이미지를 제거하려면 이미지 옆에 있는 확인란을 선택 취소합니다.

1. [이미지 크리에이티브 설정](/help/creative/creative-libraries/creative-settings-standard.md#creative-settings-image)을 지정하십시오.

   기본적으로 방금 업로드한 모든 크리에이티브가 선택되고 지정한 설정이 선택한 모든 크리에이티브에 적용됩니다. 하나의 값만 있는 모든 설정은 선택한 모든 크리에이티브에 적용됩니다. 특정 크리에이티브에 대한 설정을 입력하려면 적용할 수 없는 각 크리에이티브의 선택을 해제합니다.

1. **[!UICONTROL Create]** 클릭

## 크리에이티브 라이브러리에 서드파티 크리에이티브 추가 {#creative-add-third-party}

[!DNL Creative]은(는) 대부분의 타사 광고 서버에서 호스팅되는 크리에이티브에 대해 JavaScript 추적 태그를 지원합니다.

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

1. 라이브러리 이름을 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 **[!UICONTROL Standard Ads]** 하위 탭을 클릭합니다.

1. **[!UICONTROL Create]** > **[!UICONTROL Creative]** > **[!UICONTROL 3rd Party]**&#x200B;을(를) 클릭합니다.

1. [타사 크리에이티브 설정](#creative-settings-third-party)에서 크리에이티브에 대한 JavaScript 태그 및 기타 설정을 지정합니다.

   [사용 가능한 매크로](/help/creative/creative-macros.md)를 복사하여 JavaScript 태그에 붙여넣을 수 있습니다.

1. **[!UICONTROL Create]** 클릭

## 광고 라이브러리에 비디오 광고 추가

[비디오 크리에이티브 사양](/help/creative/creative-libraries/creative-libraries-about.md#creative-video-specs) 및 [지원되는 크리에이티브 크기](/help/creative/creative-libraries/creative-sizes.md)를 참조하세요.

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

1. 라이브러리 이름을 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 **[!UICONTROL Standard Ads]** 하위 탭을 클릭합니다.

1. **[!UICONTROL Create]** > **[!UICONTROL Creative]** > **[!UICONTROL Video]**&#x200B;을(를) 클릭합니다.

1. 다음 방법 중 하나로 비디오 파일을 지정합니다.

   * 장치나 네트워크의 파일을 상자로 끌어서 놓습니다.

   * 장치 또는 네트워크에서 파일을 찾으려면 **[!UICONTROL Select a file]**&#x200B;을(를) 클릭하십시오.

1. [비디오 크리에이티브 설정](/help/creative/creative-libraries/creative-settings-standard.md#creative-settings-video)을 지정하십시오.

   기본적으로 방금 업로드한 크리에이티브가 선택되고 지정한 설정이 선택한 크리에이티브에 적용됩니다.<!-- By default, all creatives you just uploaded are selected, and any settings you specify apply to all selected creatives. Any settings with only one value apply to all selected creatives. To enter settings for specific creatives, deselect each inapplicable creative. -->

1. **[!UICONTROL Create]** 클릭

>[!MORELIKETHIS]
>
>* [표준 광고 편집](/help/creative/creative-libraries/creative-edit-standard.md)
>* [표준 크리에이티브 설정](/help/creative/creative-libraries/creative-settings-standard.md)
>* [추적 URL에 사용할 수 있는 매크로](/help/creative/creative-macros.md)
>* [지원되는 크리에이티브 크기](/help/creative/creative-libraries/creative-sizes.md)
>* [크리에이티브 미리 보기](/help/creative/creative-libraries/creative-preview.md)
>* [번들에서 광고 연결 및 분리](/help/creative/creative-libraries/creative-attach-detach-bundles.md)
>* [크리에이티브 라이브러리 정보](/help/creative/creative-libraries/creative-libraries-about.md)
>* [Creative 라이브러리 관리](/help/creative/creative-libraries/creative-library-manage.md)
