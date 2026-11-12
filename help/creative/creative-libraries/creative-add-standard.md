---
title: 크리에이티브 라이브러리에 표준 크리에이티브 추가
description: 크리에이티브 라이브러리에 표준(비동적) 크리에이티브를 추가하는 방법을 알아봅니다.
feature: Creative Standard Creatives
exl-id: e6f1265b-9d05-4b3d-9dc6-300dbd9eb52d
TQID: 'https://experienceleague.adobe.com/mgUcE-E6LAIFFU8S5WrUceCQ6ZMSGF9tFkqEfnuKKSQ'
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
    internal-label: Demand Side Platform
  - id: d0d9f2ed-c163-44e1-97a1-4ace121416b8
    internal-label: Creative
subfeature_v2:
  - id: d06c1576-7039-4934-b256-7366e138fbb6
    internal-label: Creative Standard Creatives
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: a2a6d94329df17c332a140de428bb44fb892c97a
workflow-type: tm+mt
source-wordcount: '2018'
ht-degree: 0%
---
# 크리에이티브 라이브러리에 표준 크리에이티브 추가

표준 [광고 경험](/help/creative/experiences/experience-about.md)에서 사용할 표준 크리에이티브를 [크리에이티브 라이브러리](creative-library-manage.md)에 추가하십시오.

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

1. **[!UICONTROL Creatives]** 탭에서 **[!UICONTROL Create]** > **[!UICONTROL Creatives]** > **[!UICONTROL Flexible]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Upload New]**&#x200B;을(를) 클릭합니다.

1. 다음 방법 중 하나로 ZIP 파일을 지정합니다.

   * 장치나 네트워크의 파일을 상자로 끌어서 놓습니다.

   * 장치 또는 네트워크에서 파일을 찾으려면 **[!UICONTROL Select a file]**&#x200B;을(를) 클릭하십시오.

   [유연한 광고 사양](#flexible-ad-spec)을 참조하세요.

1. 유연한 크리에이티브 파일 추가 또는 제거:

   * 파일을 추가하려면 왼쪽 상단의 ![추가](/help/creative/assets/create.png "추가")를 클릭하고 장치나 네트워크에서 파일을 찾습니다.

   * 파일을 제거하려면 해당 파일 옆에 있는 확인란을 선택 취소합니다.

1. (선택 사항) 크리에이티브를 미리 보려면 이미지 위에서 ![미리 보기](/help/creative/assets/preview.png "미리 보기")를 클릭합니다.

1. [유연한 HTML5 광고 설정](/help/creative/creative-libraries/creative-settings-standard.md#creative-settings-flexible-html5)을 지정하십시오.

   기본적으로 방금 업로드한 모든 크리에이티브가 선택됩니다. 값이 하나만 있는 설정은 선택한 모든 크리에이티브에 적용됩니다. 일부 설정의 경우 개별 값을 지정할 수 있습니다. 특정 크리에이티브에 대한 설정을 입력하려면 적용할 수 없는 각 크리에이티브 옆의 확인란을 선택 취소합니다.

1. **[!UICONTROL Create]** 클릭

### 템플릿을 사용하여 유연한 크리에이티브 추가 {#flexible-creative-use-template}

계정에 업로드된 유연한 크리에이티브 템플릿을 사용하여 사전 정의된 크기의 광고를 작성할 수 있습니다. 사용할 템플릿을 선택하면 클릭 태그 및 속성이 편집됩니다.

<!--
Replace last sentence with this if we add the template download feature back:  You can either a\) select a template to use, and then edit the click tags and attributes; or b\) [download a template as a ZIP file](#download-flexible-creative-template), edit the contents offline to build your own creative, and then [upload the edited file as a new creative](flexible-creative-upload).
-->

<!--
 Not currently an option:
You can use any of the [predefined flexible creative templates](flexible-html5-templates.md) included with [!DNL Creative] to build 160x600, 300x250, 300x600, or 728x90 ads.

For information about the attributes available in predefined templates, see "[Available flexible creative templates](#flexible-creative-templates-available)."
-->

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

1. 라이브러리 이름을 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 **[!UICONTROL Create]** > **[!UICONTROL Creatives]** > **[!UICONTROL Flexible]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Browse System Flexible Templates]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 템플릿을 미리 보려면 템플릿 이름 옆에 있는 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Preview]**&#x200B;을(를) 클릭합니다.

   필요한 경우 템플릿을 다운로드할 수 있습니다. 템플릿 이름 옆에 있는 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Download]**&#x200B;을(를) 클릭합니다.

1. 템플릿 이름 옆에 있는 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Use Selected]**&#x200B;을(를) 클릭합니다.

1. 언어를 지정하고 자신의 클릭 태그, 이미지 및 기타 특성을 포함하도록 [유연한 HTML5 Creative 설정](/help/creative/creative-libraries/creative-settings-standard.md#creative-settings-flexible-html5)을 편집합니다.

   크리에이티브가 압축되면 최대 파일 크기는 2MB입니다.<!-- Still true? -->

1. 유연한 크리에이티브 파일 추가 또는 제거:

   * 장치나 네트워크에서 파일을 추가하려면 왼쪽 상단의 ![추가](/help/creative/assets/create.png "추가")를 클릭하고 파일을 찾습니다. 크리에이티브 옆에 있는 확인란을 선택하고 다른 크리에이티브 옆에 있는 확인란을 선택 취소한 다음 [유연한 HTML5 크리에이티브 설정](/help/creative/creative-libraries/creative-settings-standard.md#creative-settings-flexible-html5)을(를) 편집하여 언어를 지정하고 자신의 클릭 태그, 이미지 및 기타 특성을 포함하십시오.

   * 파일을 제거하려면 해당 파일 옆에 있는 확인란을 선택 취소합니다.

1. (선택 사항) 크리에이티브를 미리 보려면 이미지 위에서 ![미리 보기](/help/creative/assets/preview.png "미리 보기")를 클릭합니다.

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

## 크리에이티브 라이브러리에 표준 디스플레이 크리에이티브 추가

표준 디스플레이 크리에이티브에는 Adobe Experience Manager 및 HTML에서 가져온 크리에이티브를 포함하여 이미지 및 Adobe GenStudio for Performance Marketing5 크리에이티브가 포함됩니다.

* GIF, JPEG, JPG 또는 PNG 형식의 이미지를 만들 수 있습니다. 최대 파일 크기는 2MB입니다. [지원되는 크리에이티브 크기](/help/creative/creative-libraries/creative-sizes.md)를 참조하세요.

* 한 번에 여러 Experience Manager 에셋, 여러 GenStudio 경험 또는 단일 유형(단순 또는 정적)의 여러 로컬 HTML5 크리에이티브를 추가할 수 있습니다. HTML5 광고 제품의 경우 [HTML5 광고 사양](/help/creative/creative-libraries/html5-creative-specification.md)을 참조하세요.

<!--
 Add in when we add this feature back:
You can optionally download a sample HTML5 creative as a ZIP file, edit the contents to build your own creative, and then add the edited file as a new creative.
-->

>[!NOTE]
>
>[!DNL Creative] 내에서 직접 편집할 수 있는 표준 HTML 태그로 모든 특성을 가진 HTML5 크리에이티브인 [유연한 HTML5 크리에이티브를 추가](#flexible-creative-add)할 수도 있습니다.

### 새 UI에서

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 특정 라이브러리를 포함하도록 [보기를 사용자 지정](/help/creative/introduction/customize-data-views.md)합니다.

1. 다음 방법 중 하나로 라이브러리를 엽니다.

   * 라이브러리 이름을 클릭합니다.

   * 라이브러리 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Open]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 **[!UICONTROL Create]** > **[!UICONTROL Upload]** > **[!UICONTROL Display]**&#x200B;을(를) 클릭합니다.

1. 크리에이티브 지정:

   * 로컬 이미지 또는 HTML5 에셋의 경우 다음 중 하나를 수행하십시오.

     * 장치나 네트워크의 파일을 상자로 끌어서 놓습니다.

     * 장치 또는 네트워크에서 파일을 찾으려면 **[!UICONTROL Select a file]**&#x200B;을(를) 클릭하십시오.

   * DSP 계정에 연결된 [Experience Manager 라이브러리](/help/creative/creative-libraries/aem-assets-configure.md)에서 승인된 이미지의 경우 다음을 수행하십시오.

     1. **[!UICONTROL AEM Asset Library]**&#x200B;을(를) 클릭합니다.

     1. (Experience Manager 계정에 아직 로그인하지 않은 경우) Experience Manager 계정에 로그인합니다.

     1. [!UICONTROL Assets] 또는 [!UICONTROL Collections] 보기에서 파일을 찾아 선택한 다음 오른쪽 상단의 **[!UICONTROL Select]**&#x200B;을(를) 클릭합니다.

        <!-- If the existing asset has multiple quality options, [!DNL Creative] downloads the primary asset, or the asset with the highest resolution within some upper limit [verify what it is and how this works]. [If an asset is part of an image set, ... primary asset in the image set. -->

   * GenStudio 경험의 경우 다음을 수행합니다.

     1. **[!UICONTROL GenStudio Library]**&#x200B;을(를) 클릭합니다.

     1. (GenStudio 계정에 아직 로그인하지 않은 경우) GenStudio 계정에 로그인합니다.

        기본적으로 디스플레이 광고 경험이 표시됩니다. 필요에 따라 캠페인 또는 기타 속성으로 경험을 필터링할 수 있습니다.

     1. 디스플레이 광고 경험을 찾아 선택한 다음 오른쪽 상단의 **[!UICONTROL Select]**&#x200B;을(를) 클릭합니다.

     선택한 경험의 각 크리에이티브 변형을 별도의 HTML5 크리에이티브로 가져옵니다.

1. 광고 추가 또는 제거:

   * 이미지를 추가하려면 왼쪽 상단의 ![추가](/help/creative/assets/create.png "추가")를 클릭하고 장치나 네트워크에서 파일을 찾습니다.

   * 이미지를 제거하려면 이미지 옆에 있는 확인란을 선택 취소합니다.

1. [HTML5 광고 설정](/help/creative/creative-libraries/creative-settings-standard.md#creative-settings-html5) 또는 [이미지 광고 설정](/help/creative/creative-libraries/creative-settings-standard.md#creative-settings-image)을 지정하십시오.

   기본적으로 방금 업로드한 모든 크리에이티브 또는 GenStudio 경험이 선택되고 지정한 설정이 선택한 모든 항목에 적용됩니다. 값이 하나만 있는 설정은 선택한 모든 항목에 적용됩니다. 특정 크리에이티브 또는 GenStudio 경험에 대한 설정을 입력하려면 적용할 수 없는 각 크리에이티브 또는 경험의 선택을 해제합니다.

1. **[!UICONTROL Save Creative]**&#x200B;을(를) 클릭합니다.

### 기존 UI에서

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Switch to classic UI]**&#x200B;을(를) 클릭합니다.

1. 라이브러리 이름을 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 **[!UICONTROL Create]** > **[!UICONTROL Creatives]** > **[!UICONTROL Standard Display]**&#x200B;을(를) 클릭합니다.

1. 크리에이티브 지정:

   * 로컬 이미지 또는 HTML5 에셋의 경우 다음 중 하나를 수행하십시오.

     * 장치나 네트워크의 파일을 상자로 끌어서 놓습니다.

     * 장치 또는 네트워크에서 파일을 찾으려면 **[!UICONTROL Select a file]**&#x200B;을(를) 클릭하십시오.

   * DSP 계정에 연결된 [Experience Manager 라이브러리](/help/creative/creative-libraries/aem-assets-configure.md)에서 승인된 이미지의 경우 다음을 수행하십시오.

     1. **[!UICONTROL AEM Asset Library]**&#x200B;을(를) 클릭합니다.

     1. (Experience Manager 계정에 아직 로그인하지 않은 경우) Experience Manager 계정에 로그인합니다.

     1. [!UICONTROL Assets] 또는 [!UICONTROL Collections] 보기에서 파일을 찾아 선택한 다음 오른쪽 상단의 **[!UICONTROL Select]**&#x200B;을(를) 클릭합니다.

        <!-- If the existing asset has multiple quality options, [!DNL Creative] downloads the primary asset, or the asset with the highest resolution within some upper limit [verify what it is and how this works]. [If an asset is part of an image set, ... primary asset in the image set. -->

   * GenStudio 경험의 경우 다음을 수행합니다.

     1. **[!UICONTROL GenStudio Library]**&#x200B;을(를) 클릭합니다.

     1. (GenStudio 계정에 아직 로그인하지 않은 경우) GenStudio 계정에 로그인합니다.

        기본적으로 디스플레이 광고 경험이 표시됩니다. 필요에 따라 캠페인 또는 기타 속성으로 경험을 필터링할 수 있습니다.

     1. 디스플레이 광고 경험을 찾아 선택한 다음 오른쪽 상단의 **[!UICONTROL Select]**&#x200B;을(를) 클릭합니다.

     선택한 경험의 각 크리에이티브 변형을 별도의 HTML5 크리에이티브로 가져옵니다.

1. 광고 추가 또는 제거:

   * 이미지를 추가하려면 왼쪽 상단의 ![추가](/help/creative/assets/create.png "추가")를 클릭하고 장치나 네트워크에서 파일을 찾습니다.

   * 이미지를 제거하려면 이미지 옆에 있는 확인란을 선택 취소합니다.

1. [HTML5 광고 설정](/help/creative/creative-libraries/creative-settings-standard.md#creative-settings-html5) 또는 [이미지 광고 설정](/help/creative/creative-libraries/creative-settings-standard.md#creative-settings-image)을 지정하십시오.

   기본적으로 방금 업로드한 모든 크리에이티브 또는 GenStudio 경험이 선택되고 지정한 설정이 선택한 모든 항목에 적용됩니다. 값이 하나만 있는 설정은 선택한 모든 항목에 적용됩니다. 특정 크리에이티브 또는 GenStudio 경험에 대한 설정을 입력하려면 적용할 수 없는 각 크리에이티브 또는 경험의 선택을 해제합니다.

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

## Creative Library에 타사 크리에이티브 추가 {#creative-add-third-party}

[!DNL Creative]은(는) 서드파티 광고 서버에서 호스팅되는 디스플레이 크리에이티브에 대한 광고 태그를 지원합니다. 새 UI에서 트래픽 시트에서 하나 이상의 크리에이티브를 가져올 수 있습니다. 기존 UI는 단일 크리에이티브에 대한 태그 입력을 지원합니다.

### 새 UI에서

#### 트래픽 시트 준비 {#third-party-sheet-requirements}

* Excel(`.xlsx` 또는 `.xls`), CSV 또는 TSV 파일(10MB 이하, 광고 크리에이티브 수 500개 이하)을 사용합니다.

* Excel 파일의 경우 첫 번째 워크시트에 크리에이티브를 추가합니다. 첫 번째 워크시트만 가져옵니다. 암호로 보호된 파일은 지원되지 않습니다.

* [!DNL Flashtalking] 또는 [!DNL Google Campaign Manager 360] 내보내기를 사용하거나 일반 시트를 준비하십시오. 시트는 업로드할 때 선택하는 광고 서버 레이아웃과 일치해야 합니다.

* 각 크리에이티브에 대한 크리에이티브 이름, 크기 및 광고 태그를 포함합니다. 이름에는 최대 255자를 사용할 수 있습니다. 단일 크기 열(예: `300x250`) 또는 공급업체 내보내기의 개별 너비 및 높이 열에 차원을 지정하십시오. [지원되는 크리에이티브 크기](creative-sizes.md)를 사용하십시오.

* 제네릭 시트의 경우 열 머리글 `Creative Name`, `Size` 및 `Ad Tag`을(를) 사용합니다. 업로드 대화 상자에서 CSV 템플릿을 다운로드할 수 있습니다. 예제 행을 자체 크리에이티브 데이터로 대체합니다.

>[!IMPORTANT]
>
>* 일괄 업로드는 표시 태그만 지원합니다. 비디오 및 VAST 태그는 지원되지 않습니다.
>* 일괄 업로드는 제공된 대로 광고 태그를 저장합니다. 가져오는 동안 추적 매크로를 삽입하거나 추적 URL을 다시 작성하지 않습니다. 시트를 업로드하기 전에 태그에 필요한 [추적 매크로](/help/creative/creative-macros.md)를 포함하십시오.

#### 크리에이티브 업로드 및 검토 {#third-party-bulk-upload}

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

1. 다음 방법 중 하나로 라이브러리를 엽니다.

   * 라이브러리 이름을 클릭합니다.

   * 라이브러리 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Open]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 **[!UICONTROL Add new]** > **[!UICONTROL Upload]** > **[!UICONTROL 3rd Party]**&#x200B;을(를) 클릭합니다.

   **[!UICONTROL Bulk upload third-party tags]** 대화 상자가 열립니다.

1. 시트와 일치하는 **[!UICONTROL Ad server]**&#x200B;을(를) 선택하십시오.

   * **[!UICONTROL Flashtalking]**

   * **[!UICONTROL Google CM360]**

   * **[!UICONTROL Generic]**

   파일을 업로드하려면 먼저 광고 서버를 선택해야 합니다. 선택한 광고 서버는 시트의 모든 크리에이티브에 적용됩니다. 개별 태그에서는 감지되지 않습니다.

1. (선택 사항) 제네릭 시트를 준비하려면 **[!UICONTROL Download CSV template]**&#x200B;을(를) 클릭하고 예제 데이터를 독창적인 데이터로 바꾼 다음 파일을 저장합니다.

1. 다음 방법 중 하나로 시트를 지정합니다.

   * 파일을 업로드 상자에 끌어다 놓습니다.

   * 장치 또는 네트워크에서 파일을 찾으려면 **[!UICONTROL select a file]**&#x200B;을(를) 클릭하십시오.

   시트가 업로드되고 분석됩니다. 레이아웃이 선택한 광고 서버와 일치하지 않으면 시트를 수정하거나 일치하는 광고 서버를 선택하고 파일을 다시 업로드하십시오.

1. **[!UICONTROL Review third-party creatives]**&#x200B;에서 각 행에 대한 **[!UICONTROL Creative name]**, **[!UICONTROL Size]**, **[!UICONTROL Type]**, **[!UICONTROL Language]** 및 **[!UICONTROL Status]**&#x200B;을(를) 검토하십시오.

   * 시트에 여러 태그 형식이 포함되어 있는 경우 가져올 태그 열의 탭을 선택합니다. 선택한 형식이 모든 행에 적용되고 해당 열에 태그가 없는 행은 표시되지 않습니다. 탭을 변경하면 해당 형식에 대해 가져올 수 있는 모든 행으로 선택이 재설정됩니다.

   * 기본적으로 가져올 수 있는 모든 행이 선택됩니다. 가져오지 않을 크리에이티브 옆의 확인란을 선택 취소합니다.

   * (선택 사항) 개별 광고 **[!UICONTROL Language]**&#x200B;을(를) 변경합니다. 기본값은 영어입니다.

   * **[!UICONTROL Error]** 상태의 행을 선택하거나 가져올 수 없습니다. 올바른 행을 가져오거나 **[!UICONTROL Cancel]**&#x200B;을(를) 클릭하여 원본 시트를 수정하고 다시 업로드할 수 있습니다. 누락된 이름, 차원 또는 태그를 수정하고 비디오 태그나 지원되지 않는 것으로 플래그가 지정된 문자를 제거합니다.

1. **[!UICONTROL 가져오기 클릭 <N> 광고 ]**. 여기서 `<N>`은(는) 선택한 광고 수입니다. 한 번 창작하려면&#x200B;**[!UICONTROL Import 1 creative]**을(를) 클릭하십시오.

   대화 상자가 닫히고 가져오기가 시작되었음을 알리는 알림이 표시됩니다. 처리가 완료되면 라이브러리에 크리에이티브가 표시됩니다.

가져오기를 추적하려면 맨 위 메뉴 모음의 오른쪽에 있는 ![작업 관리자](/help/creative/assets/job-manager.png "작업 관리자")(**[!UICONTROL Job Manager]**)를 클릭합니다. 처리 중 실패한 행이 있으면 가져오기 작업에 대해 **[!UICONTROL Download failed rows]**&#x200B;을(를) 클릭하고 다운로드한 시트를 수정한 후 다시 업로드하십시오.

### 기존 UI에서

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Switch to classic UI]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 특정 라이브러리를 포함하도록 [보기를 사용자 지정](/help/creative/introduction/customize-data-views.md)합니다.

1. 라이브러리 이름을 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 **[!UICONTROL Create]** > **[!UICONTROL Creatives]** > **[!UICONTROL 3rd Party]**&#x200B;을(를) 클릭합니다.

1. [타사 크리에이티브 설정](#creative-settings-third-party)에서 크리에이티브에 대한 JavaScript 태그 및 기타 설정을 지정합니다.

   [사용 가능한 매크로](/help/creative/creative-macros.md)를 복사하여 JavaScript 태그에 붙여넣을 수 있습니다.

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

## 크리에이티브 라이브러리에 비디오 크리에이티브 업로드

[비디오 크리에이티브 사양](/help/creative/creative-libraries/creative-libraries-about.md#creative-video-specs) 및 [지원되는 크리에이티브 크기](/help/creative/creative-libraries/creative-sizes.md)를 참조하세요.

### 새 UI에서

한 번에 하나의 비디오를 업로드할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 특정 라이브러리를 포함하도록 [보기를 사용자 지정](/help/creative/introduction/customize-data-views.md)합니다.

1. 다음 방법 중 하나로 라이브러리를 엽니다.

   * 라이브러리 이름을 클릭합니다.

   * 라이브러리 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Open]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 **[!UICONTROL Create]** > **[!UICONTROL Upload]** > **[!UICONTROL Video]**&#x200B;을(를) 클릭합니다.

1. 다음 방법 중 하나로 비디오 파일을 지정합니다.

   * 장치 또는 네트워크에 있는 파일을 상자로 끌어서 놓습니다.

   * 장치 또는 네트워크에서 파일을 찾으려면 **[!UICONTROL Select a file]**&#x200B;을(를) 클릭하십시오.

1. [비디오 크리에이티브 설정](/help/creative/creative-libraries/creative-settings-standard.md#creative-settings-video)을 지정하십시오.

1. **[!UICONTROL Save Creative]**&#x200B;을(를) 클릭합니다.

### 기존 UI에서

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Libraries]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Switch to classic UI]**&#x200B;을(를) 클릭합니다.

1. 라이브러리 이름을 클릭합니다.

1. **[!UICONTROL Creatives]** 탭에서 **[!UICONTROL Create]** > **[!UICONTROL Creatives]** > **[!UICONTROL Video]**&#x200B;을(를) 클릭합니다.

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
>* [크리에이티브에 대한 변경 로그 보기](/help/creative/creative-libraries/creative-view-change-log.md)
>* [추적 URL에 사용할 수 있는 매크로](/help/creative/creative-macros.md)
>* [지원되는 크리에이티브 크기](/help/creative/creative-libraries/creative-sizes.md)
>* [크리에이티브 미리 보기](/help/creative/creative-libraries/creative-preview.md)
>* [번들에서 광고 연결 및 분리](/help/creative/creative-libraries/creative-attach-detach-bundles.md)
>* [크리에이티브 라이브러리 정보](/help/creative/creative-libraries/creative-libraries-about.md)
>* [Creative 라이브러리 관리](/help/creative/creative-libraries/creative-library-manage.md)
