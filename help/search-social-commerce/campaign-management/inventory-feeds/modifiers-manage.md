---
title: 수정자 관리
description: 인벤토리 데이터 피드에 대한 광고 템플릿에 대한 수정자를 구성하고 관리하는 방법에 대해 알아봅니다.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '375'
ht-degree: 0%

---

# 수정자 관리

*[!DNL Google Ads], [!DNL Microsoft® Advertising], [!DNL Yahoo! Japan Ads] (작업만 삭제) 및 [!DNL Yandex] 계정만*

수정자는 형용사 또는 부사로서 기본적인 문장 구조를 바꾸지 않고 문장에 추가하거나 문장에서 제거할 수 있다. 피드 데이터 템플릿의 다양한 데이터 필드에 변수로 사용할 수정자 그룹을 만들 수 있습니다. 계정 구조(캠페인 및 광고 그룹) 필드, 키워드, 기본 URL 및 광고에 수정자를 포함시켜 연결된 각 수정자 값에 대해 하나의 값을 만듭니다. 예를 들어 광고 헤드라인에서 수정자 그룹 변수를 사용하고 수정자 그룹에 3개의 수정자(&quot;저렴한&quot;, &quot;할인&quot; 및 &quot;경제적인&quot;)가 포함된 경우 데이터 피드의 각 데이터 행에 대해 3개의 개별 광고(수정자마다 하나씩)가 만들어집니다. 마찬가지로, 광고 그룹의 기본 URL에 여러 값이 있는 수정자 그룹을 포함하면 결과 기본 URL마다 하나의 키워드 세트가 만들어집니다.

각 수정자 그룹에는 원하는 수만큼 수정자가 포함될 수 있습니다. 각 템플릿은 하나의 수정자 그룹만 사용할 수 있습니다.

## 수정자 그룹 만들기

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Advanced (ACM)]**.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL Modifiers]**.

1. 수정자 그룹 목록 위에서 **[!UICONTROL Create]**.

1. 수정자 그룹 설정을 지정합니다.

   **[!UICONTROL Name]:** 수정자 그룹의 이름입니다.

   **[!UICONTROL Modifiers]:** 그룹의 수정자 값(라인당 하나)입니다.

1. 클릭 **[!UICONTROL Save]**.

## 수정자 그룹 편집

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Advanced (ACM)]**.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL Modifiers]**.

1. 수정자 그룹 목록에서 수정자 그룹명을 누릅니다.

1. 수정자 그룹 설정을 편집합니다.

   **[!UICONTROL Name]:** 수정자 그룹의 이름입니다.

   **[!UICONTROL Modifiers]:** 그룹의 수정자 값(라인당 하나)입니다.

1. 클릭 **[!UICONTROL Save]**.

## 수정자 그룹 삭제

>[!IMPORTANT]
>
>수정자 그룹을 삭제하면 해당 수정자 그룹에 대한 모든 변수를 제거합니다(로 표시). `<modifier_group_name>`기존 템플릿의 필드에서 가져온 참조)를 참조하십시오. 존재하지 않는 수정자에 대한 변수를 사용하여 템플릿을 통해 데이터를 전파하려고 하면 작업이 실패합니다1.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Advanced (ACM)]**.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL Modifiers]**.

1. 삭제할 각 수정자 그룹 옆의 확인란을 선택합니다.

1. 수정자 그룹 목록 위에서 **[!UICONTROL Delete]**.

1. 확인 메시지에서 다음을 클릭합니다. **[!UICONTROL Yes]**.

1. (필요한 경우) [수정자에 대한 참조 제거](/help/search-social-commerce/campaign-management/inventory-feeds/ad-templates/ad-template-manage.md) 모든 적용 가능한 템플릿에서.

>[!MORELIKETHIS]
>
>* [인벤토리 피드 기본 정보](/help/search-social-commerce/campaign-management/inventory-feeds/inventory-feeds-about.md)
>* [광고 템플릿 관리](/help/search-social-commerce/campaign-management/inventory-feeds/ad-templates/ad-template-manage.md)

