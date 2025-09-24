---
title: 동적 광고 템플릿 관리
description: xxxx에 대해 알아보십시오.
feature: Creative Templates
source-git-commit: 5828fada55ba9506589df6088ea58b896084700c
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 0%

---

# 동적 광고 템플릿 관리

원하는 광고 형식으로 zip HTML5 파일을 업로드하여 광고 유형(정적 HTML5 또는 동적 HTML5)과 광고 크기의 각 조합에 대한 별도의 광고 템플릿을 만듭니다. Dynamic HTML5 광고의 경우 광고 특성 <!-- more clarification? -->이 포함된 파일도 업로드합니다.

<!-- add this where/how?: You can use the same feed template for multiple ad templates. -->

<!-- EXPLAIN MORE:  Is this like repropagating a feed file through a template, or can you just change some things? Is generating an ad template a one-time thing, using the existing feed file, but you might later update the file and re-propagation doesn't happen automatically? Clarify the use cases for each.-->

## 동적 광고 템플릿 만들기

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Ad Templates]**&#x200B;을(를) 클릭합니다.

1. 오른쪽 상단에서 **[!UICONTROL Create Ad Template]** 클릭

1. [광고 템플릿 설정 지정](#ad-template-settings)

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

## 동적 광고 템플릿 편집

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Ad Templates]**&#x200B;을(를) 클릭합니다.

1. 광고 템플릿 행 위에 커서를 놓고 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. [광고 템플릿 설정](#ad-template-settings)을(를) 편집합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 동적 광고 템플릿 다운로드

<!-- Explain more about what this contains and the format:  Downloaded ad templates are compressed (zipped) files that include XXX as TDF files and the uploaded HTML5 (and attributes?) data. You can open the TDF file in a text editor. -->

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Ad Templates]**&#x200B;을(를) 클릭합니다.

1. 광고 템플릿 행 위에 커서를 놓고 **[!UICONTROL Download]**&#x200B;을(를) 클릭합니다.

   브라우저의 일반적인 절차에 따라 파일이 다운로드됩니다.

## 동적 광고 템플릿 삭제

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Ad Templates]**&#x200B;을(를) 클릭합니다.

1. 광고 템플릿 행 위에 커서를 놓고 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Delete]**.<!-- Confirm -->을(를) 클릭합니다

## 광고 템플릿에서 동적 광고 만들기

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Ad Templates]**&#x200B;을(를) 클릭합니다.

1. 광고 템플릿 행 위에 커서를 놓고 **[!UICONTROL Create Dynamic Ad]**&#x200B;을(를) 클릭합니다.

   [!UICONTROL New Dynamic Ad] 화면에서 [!UICONTROL Ad Template Size], [!UICONTROL Ad Template Type] 및 [!UICONTROL Ad Template] 필드가 자동으로 선택되고 읽기 전용입니다.

1. [동적 광고를 만들](/help/creative/creative-libraries/creative-add-dynamic.md)동적 광고 설정을 지정하십시오.

## 광고 템플릿 설정 {#ad-template-settings}

### 광고 템플릿 세부 정보

**[!UICONTROL Advertiser]**: (기존 템플릿의 경우 읽기 전용) 광고가 생성되는 광고주입니다.

**[!UICONTROL Ad Template Name]**: 광고주의 고유한 광고 템플릿 이름입니다.

**[!UICONTROL Ad Template Type]**: (기존 템플릿의 경우 읽기 전용) 광고 템플릿 형식: *정적 HTML5* 또는 *동적 HTML5*.

**[!UICONTROL Ad Template Size]**: (기존 템플릿의 경우 읽기 전용) 템플릿으로 만든 광고의 차원입니다.

**[!UICONTROL Description]**: (선택 사항) 광고 템플릿을 사용하는 모든 사용자에게 유용한 정보입니다.

<!-- I don't see this on 9/24:

### (Static HTML5 ad templates) Click Tags

**\[Click Tag Parameter\]**: The click tag parameters to allow click-tracking redirects from ads created using the ad template. To add a parameter, click **[!UICONTROL + Add More]** and enter an additional parameter. You can include up to five parameters.

-->

### HTML zip

원하는 광고 형식으로 압축한 HTML5 파일입니다. 파일을 이미 업로드한 경우에는 파일 이름이 나열됩니다.

[HTML5 광고 사양](/help/creative/creative-libraries/html5-creative-specification.md)을 참조하세요.

파일을 업로드하려면:

1. **[!UICONTROL Upload HTML5 zip]**&#x200B;을(를) 클릭합니다.

1. 장치 또는 네트워크에서 파일을 찾습니다.

### (동적 HTML5 광고 템플릿) 특성 파일

<!-- EXPLAIN -->광고 템플릿에 대한 속성을 포함하는 파일입니다. 파일을 이미 업로드한 경우에는 파일 이름이 나열됩니다.

<!-- Add specs for this file type -->

파일을 업로드하려면:

1. **[!UICONTROL Upload Attributes File]**&#x200B;을(를) 클릭합니다.

1. 장치 또는 네트워크에서 파일을 찾습니다.

>[!MORELIKETHIS]
>
>* [동적 광고에 대한 워크플로](/help/creative/introduction/workflow-dynamic-ads.md)
>* [자산 파일 관리](/help/creative/feeds/asset-manage.md)
>* [피드 템플릿 관리](/help/creative/feeds/feed-template-manage.md)
>* [카탈로그 관리](/help/creative/feeds/catalog-manage.md)
>* [Creative 라이브러리에 동적 크리에이티브 추가](/help/creative/creative-libraries/creative-add-dynamic.md)

