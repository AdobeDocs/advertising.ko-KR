---
title: AI를 사용하여 이미지에서 광고 템플릿 생성
description: Creative Studio에서 AI를 사용하여 기존 정적 디스플레이 광고 이미지를 편집 가능한 광고 템플릿으로 변환하는 방법에 대해 알아봅니다.
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: d0d9f2ed-c163-44e1-97a1-4ace121416b8
    internal-label: Creative
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: adc2fdc93f06b5459c19b08306d1e30ce00e7028
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%
---
# AI를 사용하여 이미지에서 광고 템플릿 생성

*Beta 기능*

[!UICONTROL Creative Studio]의 AI를 사용하여 기존 정적 디스플레이 광고 이미지를 편집 가능한 디스플레이 광고 템플릿으로 변환합니다. 생성된 템플릿을 검토하고 자연어를 사용하여 변경 사항을 요청한 다음 템플릿 편집기를 열어 수동으로 변경하고 템플릿을 저장합니다.

## 시작하기 전에

Creative 라이브러리에 기존 정적 이미지 광고가 필요합니다. 이 워크플로는 라이브러리에서 광고를 선택합니다. 생성 대화 상자에서 직접 새 이미지를 업로드하지 않습니다.

## 템플릿 생성 및 검토 {#template-generate}

1. 주 메뉴에서 **[!UICONTROL Creative Studio]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Templates]** 탭을 클릭합니다.

1. (선택 사항) 페이지 상단의 광고주 목록에서 광고주를 선택하여 해당 광고주의 라이브러리를 확인합니다.

1. **[!UICONTROL Use AI to Generate a New Display Ad Template]** 상자에서 **[!UICONTROL Generate]**&#x200B;을(를) 클릭합니다.

1. 아직 선택하지 않은 경우 **[!UICONTROL Generate New Ad Template]** 대화 상자에서 **[!UICONTROL Generate from Existing Standard Ad Image]**&#x200B;을(를) 선택합니다.

1. **[!UICONTROL Ad Library]** 목록에서 이미지 광고가 포함된 라이브러리를 선택합니다.

1. 이미지 광고 카드 위에 커서를 놓고 **[!UICONTROL Use this Standard Ad]**&#x200B;을(를) 클릭합니다.

   선택한 광고의 폭과 높이를 사용하여 자동으로 생성이 시작됩니다.

1. 생성이 완료될 때까지 기다린 다음 템플릿 미리 보기 및 **[!UICONTROL Layers]** 패널을 검토합니다(사용 가능한 경우).

   템플릿을 사용하기 전에 텍스트, 이미지 및 레이아웃을 확인하십시오. 여기에 표시된 레이어는 검토용입니다. 템플릿 편집기에서 수동으로 변경하십시오.

1. (선택 사항) 생성된 템플릿에 대한 요청 변경 사항:

   1. **[!UICONTROL Ask the AI for any changes]** 필드에서 원하는 변경 내용을 설명합니다. 예를 들어 `Change the headline to "Limited Time Offer" and the button text to "Shop Now"`을(를) 입력합니다.

   1. **[!UICONTROL Regenerate]**&#x200B;을(를) 클릭합니다.

   1. 업데이트된 미리보기를 검토합니다. 필요에 따라 반복합니다.

1. 계속할 준비가 되면 **[!UICONTROL Use this Ad Template]**&#x200B;을(를) 클릭합니다.

   생성된 템플릿이 디스플레이 템플릿 편집기에서 열립니다.

## 템플릿 편집 및 저장 {#template-save}

1. 템플릿 편집기에서 생성된 요소를 검토하고 [템플릿 편집기 컨트롤](creative-studio-manage-templates.md#template-controls)을 사용하여 나머지 변경 작업을 수행합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Update Template]** 대화 상자에서 **[!UICONTROL Template name]**&#x200B;을(를) 입력하거나 업데이트하고 **[!UICONTROL Advertiser]**&#x200B;을(를) 선택한 다음 선택적으로 태그를 추가합니다.

1. 템플릿을 저장하고 **[!UICONTROL Templates]** 보기로 돌아가려면 **[!UICONTROL Update]**&#x200B;을(를) 클릭합니다.

   대신 별도의 복사본을 저장하려면 **[!UICONTROL Save As New]**&#x200B;을(를) 클릭합니다.

그런 다음 템플릿을 사용하여 [광고 변형을 생성](creative-studio-manage-templates.md#ad-variations-generate)할 수 있습니다.

## 템플릿을 생성할 수 없는 경우 {#troubleshooting}

* **나열된 라이브러리 또는 이미지 광고가 없습니다.** 선택한 광고주와 **[!UICONTROL Ad Library]**&#x200B;을(를) 확인하십시오. 라이브러리에 표준 광고 이미지가 없는 경우 기존 정적 이미지 광고가 포함된 다른 라이브러리를 선택합니다.

* **생성에 실패하거나 이미지를 변환할 수 없습니다.** 표시된 메시지를 검토하고 **[!UICONTROL Back to library]**&#x200B;을(를) 클릭한 다음 이미지 광고를 선택하여 다시 시도하십시오.

>[!MORELIKETHIS]
>
>* [Creative Studio에서 광고 템플릿 관리](creative-studio-manage-templates.md)
>* [Creative Studio에서 표준 광고 관리](creative-studio-manage-standard-ads.md)