---
title: 피드 템플릿 관리
description: 피드 템플릿을 관리하는 방법을 알아봅니다.
feature: Creative Dynamic Creatives
source-git-commit: 0d7a7ab23173a061961c4b5c66ace5b69a746e86
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# 피드 템플릿 관리

<!-- I have a "Retail" feed template that was created by rkarthik@adobe. Ask product if this is available to all clients or just internal.  -->

<!-- We have a finite set of supported fields on the backend. I need to include that info in an appendix. -->

피드 템플릿은 피드 파일/카탈로그의 필드를 Advertising Creative 백엔드의 필드와 매핑합니다. 정적 HTML5 광고가 아닌 동적 HTML5 광고에는 동적 광고를 만들기 위한 피드 템플릿이 필요합니다.

피드 템플릿은 여러 광고 템플릿과 함께 사용할 수 있습니다.

## 피드 템플릿 만들기

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Feeds]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Templates]** 탭을 클릭합니다.

1. 오른쪽 상단에서 **[!UICONTROL Create]** > **[!UICONTROL Template]**&#x200B;을(를) 클릭합니다.

1. [피드 템플릿 설정](#feed-template-settings)을 지정하십시오.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 피드 템플릿 편집

**참고:** 만든 피드 템플릿만 편집할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Feeds]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Templates]** 탭을 클릭합니다.

1. 템플릿 행 위에 커서를 놓고 **[!UICONTROL Duplicate]**&#x200B;을(를) 클릭합니다.

1. 필요에 따라 [피드 템플릿 설정](#feed-template-settings)을 편집합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 피드 템플릿 보기

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Feeds]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Templates]** 탭을 클릭합니다.

1. 템플릿 행 위에 커서를 놓고 **[!UICONTROL View]**&#x200B;을(를) 클릭합니다.

## 피드 템플릿 복제

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Feeds]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Templates]** 탭을 클릭합니다.

1. 템플릿 행 위에 커서를 놓고 **[!UICONTROL Duplicate]**&#x200B;을(를) 클릭합니다.

1. [!UICONTROL Duplicate Template] 화면에서 고유한 **[!UICONTROL Template Name]**&#x200B;을(를) 입력하십시오. 다른 사용자가 만든 템플릿을 복제하는 경우 **[!UICONTROL Advertiser]**&#x200B;을(를) 선택합니다. 필요에 따라 다른 [피드 템플릿 설정](#feed-template-settings)을(를) 편집하십시오.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 피드 템플릿 다운로드

다운로드한 피드 템플릿은 압축 Microsoft Excel 스프레드시트(XLSX) 형식입니다.

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Feeds]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Templates]** 탭을 클릭합니다.

1. 템플릿 행 위에 커서를 놓고 **[!UICONTROL Download]**&#x200B;을(를) 클릭합니다.

   브라우저의 일반적인 절차에 따라 파일이 다운로드됩니다.

## 피드 템플릿 설정 {#feed-template-settings}

### [!UICONTROL General] 설정

**[!UICONTROL Template Name]:** 지정한 광고주의 고유한 템플릿 이름입니다.

**[!UICONTROL Advertiser]:** 템플릿을 사용할 수 있는 광고주입니다.

**[!UICONTROL Description]:**(선택 사항) 피드 템플릿을 사용하는 모든 사용자에게 유용한 정보입니다.

### [!UICONTROL Field Mapping] 설정

피드 파일의 각 필드를 Advertising Creative 백엔드의 필드에 매핑합니다. 백엔드 필드 및 필수 특성 목록은 &quot;[동적 광고 피드 파일에 사용할 수 있는 필드](/help/creative/appendix-available-feed-fields.md)&quot;을(를) 참조하십시오.<!-- Check w/product: What is displayed where in the UI/reports and published ads? -->

적어도 하나의 피드 파일 필드는 &quot;[!UICONTROL Is Unique]&quot;(으)로 표시되어야 합니다. 필드 매핑을 추가하려면 **[!UICONTROL +]**&#x200B;을(를) 클릭합니다. 마지막 필드 매핑을 제거하려면 **[!UICONTROL +]**&#x200B;을(를) 클릭하십시오.

**[!UICONTROL Field Name]:** 피드 파일의 필드입니다.

**[!UICONTROL Description]:**(선택 사항) 피드 템플릿을 사용하는 모든 사용자에게 유용한 정보입니다.

**[!UICONTROL Is Unique]:** 필드가 고유 ID(키)임을 나타냅니다. 피드 템플릿당 하나 이상의 필드는 고유해야 합니다. 이 옵션을 선택하려면 단추를 클릭하여 오른쪽으로 이동합니다.<!-- **Note: The unique identifier is different from the feed "trigger" in experience settings. -->

**[!UICONTROL Backend Field]:** 피드 파일에서 지정된 [에 매핑되는 Advertising Creative 백 엔드의 ](/help/creative/appendix-available-feed-fields.md)필드[!UICONTROL Field Name]입니다.

>[!MORELIKETHIS]
>
>* [동적 광고용 워크플로](/help/creative/introduction/workflow-dynamic-ads.md)
>* [자산 파일 관리](/help/creative/feeds/asset-manage.md)
>* [카탈로그 관리](/help/creative/feeds/catalog-manage.md)
>* [카탈로그 처리 작업의 상태를 추적](/help/creative/feeds/job-status-track.md)
>* [동적 광고 템플릿 관리](/help/creative/ad-templates/ad-template-manage.md)
>* [Creative 라이브러리에 동적 크리에이티브 추가](/help/creative/creative-libraries/creative-add-dynamic.md)
