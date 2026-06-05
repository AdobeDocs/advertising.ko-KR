---
title: 광고주의 전환 지표 관리
description: Adobe Advertising이 광고주를 위해 추적하는 전환 지표를 사용하는 방법을 알아봅니다.
feature: Conversions
feature_v2:
  - id: aed5e38a-3e62-42fa-8d16-cd080729b2a0
  - id: e6916c1b-e939-4e0b-99f5-768e83e1e99f
subfeature_v2:
  - id: d068b149-b9d1-421c-9033-a51495366ddc
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: b9388f691c8e804cece8d9f1eeb1bdc4f352dd11
workflow-type: tm+mt
source-wordcount: 932
ht-degree: 0%

---

# (새 UI) 광고주의 전환 지표를 관리합니다

*Beta 기능*

광고주의 [전환](/help/search-social-commerce/glossary.md#c-d) 지표가 Adobe Advertising 전체에서 사용됩니다.

* 검색, 소셜 및 Commerce에서 전환 지표에 대한 데이터를 캠페인, 포트폴리오 및 목표 관리 보기의 열과 보고서에 표시할 수 있습니다. 충분한 액세스 권한이 있는 사용자는 전환 지표를 사용하여 목표를 만들 수도 있습니다. 목표는 포트폴리오를 최적화하는 데 사용됩니다.

* (Advertising DSP을 사용하는 광고주) DSP에서 캠페인 관리 보기, 사용자 지정 목표 및 사용자 지정 보고서에 전환 지표를 포함할 수 있습니다. 전환 지표를 사용하여 패키지를 최적화하는 데 사용되는 [사용자 지정 목표](/help/dsp/admin/custom-objectives-manage.md)를 만들 수도 있습니다.

사용 가능한 지표는 다음과 같습니다.

* Adobe Advertising이 광고주를 위해 추적하는 전환 지표입니다.

* [전환 및 사이트 참여 지표가 Adobe Analytics에서 동기화됨](/help/integrations/analytics/analytics-data-in-advertising.md).

* [사이트 이벤트가 Adobe Customer Journey Analytics에서 동기화됨](/help/integrations/customer-journey-analytics/overview.md).

* [!DNL Google Ads]에서 추적한 전환과 [!DNL Microsoft Advertising] 유니버설 이벤트 추적 태그에서 추적한 전환입니다.

* [특정 [!DNL Google Analytics] 계정, 속성 및 보기 조합을 검색, 소셜 및 Commerce에 대한 데이터 소스로 구성](/help/search-social-commerce/admin/data-sources/data-source-about.md)한 경우) [!DNL Google Analytics]에 의해 추적된 전환.

* 사용자 지정 피드의 전환.

사용 가능한 전환 지표 목록에서 광고주의 데이터에 대한 액세스 권한이 있는 각 사용자는 특정 지표를 선택하거나 생략하는 등 관리 보기 및 보고서에 사용할 수 있는 지표를 사용자 지정할 수 있습니다. 검색된 데이터의 맞춤법과 정확히 동일한 지표 이름을 사용하거나 가독성을 위해 열 제목에 표시되는 이름을 변경할 수 있습니다.

>[!IMPORTANT]
>
>기본적으로 [!DNL Google Ads], [!DNL Google Analytics] 및 [!DNL Microsoft Advertising] 유니버설 이벤트 추적 태그에 의해 추적된 전환을 제외한 광고주의 전환 지표는 캠페인 및 포트폴리오 관리 보기, 목표 및 보고서에 포함할 수 없습니다. 전환 지표를 사용할 수 있도록 하려면 전환 지표를 명시적으로 사용할 수 있도록 해야 합니다.
>
>[!DNL Google Ads], [!DNL Google Analytics] 및 [!DNL Microsoft Advertising] 유니버설 이벤트 추적 태그가 추적하는 새 전환은 항상 자동으로 사용할 수 있습니다.

>[!TIP]
>
>광고주(또는 광고 네트워크)가 전환 지표의 수집을 중지하면 내역 데이터를 보는 데 사용하지 않으려면 [관리 보기 및 보고서에서 해당 지표를 숨기십시오](#conversion-metrics-change-available).

## 광고주에 대해 추적된 전환 지표 보기

* 메인 메뉴에서 **[!UICONTROL Goals]>[!UICONTROL Conversions]**&#x200B;을(를) 클릭합니다.

광고주를 위해 수집된 모든 전환 지표와 여기에 지정된 다른 표시 이름이 나열됩니다. 각 지표 행에는 지표의 소스가 포함됩니다.

## 전환 지표에 대한 표시 이름 변경

예를 들어, 이름이 *reg*&#x200B;인 전환 지표를 사용하여 등록 데이터를 수집하는 경우 선택적으로 표시 이름을 변경하여 &quot;등록&quot;으로 표시되도록 할 수 있습니다.

기존 표시 이름은 삭제할 수 없습니다.

>[!NOTE]
>
>[&#x200B; [!DNL Google Analytics]](/help/search-social-commerce/admin/data-sources/data-source-about.md)의 지표에 대해 통합을 업데이트하거나 다시 인증하면 표시 이름에 대한 수동 변경 내용을 덮어씁니다. 마찬가지로, 통합을 [업데이트](/help/search-social-commerce/admin/data-sources/data-source-edit.md) 또는 [재인증](/help/search-social-commerce/admin/data-sources/data-source-reauthenticate.md)하지 않는 한 [!DNL Google Analytics] 내의 이름 변경 내용은 무시됩니다.

1. 메인 메뉴에서 **[!UICONTROL Goals]>[!UICONTROL Conversions]**&#x200B;을(를) 클릭합니다.

1. 도구 모음[&#128279;](/help/search-social-commerce/common-tasks/data-views/ad-hoc-settings/column-filter-apply-from-toolbar.md) 또는 [열 제목](/help/search-social-commerce/common-tasks/data-views/ad-hoc-settings/column-filter-apply-from-column-heading.md)에서  목록을 필터링합니다.

1. 지표의 **[!UICONTROL Conversion Display Name]** 열에서 지표 이름 위에 커서를 놓고 **..** > **[!UICONTROL Rename]**&#x200B;을(를) 클릭합니다.

1. 표시할 이름을 입력한 다음 **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

   표시 이름은 고유해야 하며 다음 특수 문자를 포함할 수 없습니다. `\"<'>&`

## 관리 뷰, 목표 및 보고서에서 사용할 수 있는 전환 지표 변경 {#conversion-metrics-change-available}

>[!NOTE]
>
>이전에 사용할 수 있었던 전환 지표를 숨기면 전환 지표가 포함된 파생 지표에서 제거됩니다.

1. 메인 메뉴에서 **[!UICONTROL Goals]>[!UICONTROL Conversions]**&#x200B;을(를) 클릭합니다.

   광고주를 위해 수집된 모든 전환 지표와 표시를 위해 지정된 다른 이름이 나열됩니다.

1. (선택 사항) 도구 모음[&#128279;](/help/search-social-commerce/common-tasks/data-views/ad-hoc-settings/column-filter-apply-from-toolbar.md) 또는 [열 제목](/help/search-social-commerce/common-tasks/data-views/ad-hoc-settings/column-filter-apply-from-column-heading.md)에서  목록을 필터링합니다.

1. 관리 보기 및 보고서에 사용할 수 있는 전환 지표를 변경합니다.

   * 단일 지표를 표시하거나 숨기려면 **[!UICONTROL Visibility]** 열에서 스위치를 클릭하여 설정을 변경합니다.

   * 여러 지표를 표시하거나 숨기려면 다음을 수행합니다.

      1. 각 전환 지표 옆에 있는 확인란을 선택합니다.

         여러 행 선택에 대한 팁은 &quot;[여러 행 선택](/help/search-social-commerce/common-tasks/navigation-editing-selection/multiple-rows-select.md)&quot;을 참조하십시오.

      1. 일괄 작업 도구 모음에서 ![가시성](/help/search-social-commerce/assets/visible.png "가시성")을 클릭하여 지표를 표시하거나 ![가시성 해제](/help/search-social-commerce/assets/visibility-off.png "가시성 해제")을(를) 클릭하여 지표를 숨깁니다.

      1. (지표를 숨기려면) 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭하여 지표가 포함된 파생 지표에서 지표를 제거하는 등 지표를 숨깁니다.

## 전환 가시성 및 소스 보고서 관리

추적된 전환에 대한 다음 정보를 다운로드할 수 있습니다. 동기화된 지표 이름, 검색, 소셜 및 Commerce 관리 보기 및 보고서 내 지표의 표시 이름, 관리 보기 및 보고서에 지표가 표시되는지 여부, 전환 ID 및 지표 소스. 데이터를 [!DNL Microsoft Excel] 통합 문서(XLSX 파일) 형식의 파일로 다운로드합니다.

### 필터링된 데이터 행으로 보고서 생성

1. 메인 메뉴에서 **[!UICONTROL Goals]>[!UICONTROL Conversions]**&#x200B;을(를) 클릭합니다.

1. 다운로드하려는 데이터의 전환을 지정합니다.

   * 특정 행에 대한 데이터를 다운로드하려면 행 옆에 있는 확인란을 선택합니다.

   * 모든 행의 데이터를 다운로드하려면 확인란을 선택할 필요가 없습니다. 기본적으로 모든 행이 포함됩니다.

1. 데이터 테이블 위의 도구 모음에서 ![보고서 다운로드](/help/search-social-commerce/assets/download.png "보고서 다운로드") **[!UICONTROL Reports]**&#x200B;를 클릭합니다.

1. [!UICONTROL Grid Reports] 설정에서 고유한 보고서 이름을 입력한 다음 **[!UICONTROL Generate]**&#x200B;을(를) 클릭합니다.

   기본적으로 파일 이름은 &quot;conversionsReport_YYYYMMDD_NNNN&quot;으로 지정됩니다. 여기서 &quot;NNNN&quot;은 순차적 작업 번호입니다(예: &quot;conversionsReport_20260402_1326).

   파일이 [!UICONTROL Recently Generated] 목록에 추가됩니다.

1. (선택 사항) 파일이 완료되면 다운로드하려면 파일 이름 옆에 있는 ![다운로드](/help/search-social-commerce/assets/download.png "다운로드")를 클릭합니다.

   브라우저의 일반적인 절차에 따라 파일이 다운로드됩니다.

### 완료된 보고서 다운로드

1. 메인 메뉴에서 **[!UICONTROL Goals]>[!UICONTROL Conversions]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위의 도구 모음에서 ![보고서 다운로드](/help/search-social-commerce/assets/download.png "보고서 다운로드") **[!UICONTROL Reports]**&#x200B;를 클릭합니다.

1. [!UICONTROL Grid Reports] 대화 상자의 [!UICONTROL Recently Generated] 목록에서 파일 이름 옆에 있는 ![다운로드](/help/search-social-commerce/assets/download.png "다운로드")를 클릭합니다.

   브라우저의 일반적인 절차에 따라 파일이 다운로드됩니다.

### 완료된 보고서 삭제

1. 메인 메뉴에서 **[!UICONTROL Goals]>[!UICONTROL Conversions]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위의 도구 모음에서 ![다운로드](/help/search-social-commerce/assets/download.png "다운로드") **[!UICONTROL Reports]**&#x200B;을(를) 클릭합니다.

1. [!UICONTROL Grid Reports] 대화 상자의 [!UICONTROL Recently Generated] 목록에서 파일 이름 옆에 있는 ![삭제](/help/search-social-commerce/assets/delete-new.png "삭제")를 클릭합니다.

<!--
>[!MORELIKETHIS]
>
>* 
-->
