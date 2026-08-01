---
title: 광고 관리
description: 사용 가능한 광고 유형을 포함하여 광고를 만들고 관리하는 방법을 알아봅니다.
feature: Search Campaign Management
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2:
  - id: aed5e38a-3e62-42fa-8d16-cd080729b2a0
subfeature_v2:
  - id: f3d33161-c519-436e-bbbd-730ba428736b
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 6a479ae0bb30d609b16a343efcec296137b9ab43
workflow-type: tm+mt
source-wordcount: 1733
ht-degree: 0%

---

# 광고 관리

*Beta 기능*

*[!DNL Google Ads], [!DNL LY Ads], [!DNL Microsoft Advertising], [!DNL Yandex] 및 기존 [!DNL Baidu] 계정만*

광고는 광고 그룹에 속하며, 광고 네트워크 및 광고 유형에 따라 헤드라인, 설명, 이미지 또는 기타 크리에이티브 요소 등 사용자에게 표시되는 콘텐츠를 포함합니다.

[API 연결을 통해 광고 네트워크 계정에 액세스할 수 있도록 설정](/help/search-social-commerce/new-ui/set-up/accounts/api-accounts/api-account-manage.md) 및 검색, 소셜 및 Commerce이 계정 데이터를 광고 네트워크와 동기화하면 [지원되는 캠페인 유형](/help/search-social-commerce/introduction/supported-inventory.md)에 대한 광고를 만들 수 있습니다. 광고의 상태를 편집하고 변경할 수도 있습니다.

각 광고 네트워크에서 사용할 수 있는 기능에 대한 자세한 내용은 &quot;[지원되는 인벤토리](/help/search-social-commerce/introduction/supported-inventory.md)&quot;를 참조하십시오.

## [!UICONTROL Ads] 보기 정보 {#ad-view-about}

[!UICONTROL Manage] > [!UICONTROL Ads] 보기는 선택한 광고주 계정에 대해 필터링된 보기의 모든 광고를 나열합니다.

### 사용 가능한 작업

* [광고 만들기](#ad-create)

* [행 내에서 광고 이름 바꾸기](#ad-rename)

* [광고 설정 편집](#ad-edit)

* [광고 상태 변경 또는 삭제](#ad-status)

* [[!UICONTROL Ads] 보기에서 데이터 보기 보고서 관리](#ad-reports)

## 사용 가능한 광고 유형 {#ad-types}

동기화된 광고 네트워크 계정 내에서 광고 그룹에 대해 지원되는 광고 유형을 만들고 관리할 수 있습니다.

* 검색 네트워크를 대상으로 하는 캠페인의 광고 그룹에 대한 **텍스트 광고 또는 확장된 텍스트 광고**. 텍스트 광고에는 광고 그룹 또는 캠페인 수준 매개 변수를 오버라이드하는 선택적 추적 매개 변수가 포함될 수 있습니다. 광고 네트워크에 따라 확장/확장 텍스트 광고 또는 표준 텍스트 광고를 만들 수 있습니다.

* [!DNL Microsoft Audience Network]의 [!DNL Microsoft Advertising] 캠페인에 대한 교차 장치, 기본 **대상 광고**. 캠페인 설정에 따라 대상 광고에 대한 두 가지 옵션이 있습니다.

  * 캠페인이 판매자 센터 상점에 연결된 경우 광고 네트워크에서 상점의 제품 정보를 사용하여 캠페인에 대한 피드 기반 광고를 자동으로 생성하도록 합니다. 캠페인에 대한 피드 기반 광고를 만들 필요는 없지만 사용자 타겟팅을 사용하여 광고 그룹을 만들어야 합니다.

  * 캠페인이 판매자 센터 계정에 연결되어 있지 않은 경우, 여러 텍스트 및 이미지 에셋이 포함된 반응형 광고 형식을 사용하여 이미지 기반 대상 광고를 만드십시오. 광고 네트워크는 가장 효과적인 광고 요소 조합을 사용하여 광고를 조합하고 [!DNL MSN], [!DNL Outlook.com] 및 [!DNL Microsoft Edge]과(와) 같은 사이트에 표시합니다.

* 검색 네트워크에서 [!DNL Google Ads] 캠페인에 대한 **통화 전용 광고**. 호출 전용 광고는 전화 번호를 포함하는 텍스트 광고입니다. 필요에 따라 고급 호출 보고를 위해 [!DNL Google Ads]이(가) 할당한 전달 번호를 사용할 수 있습니다.

  >[!NOTE]
  >
  >현재는 호출 전용 광고를 만들거나 편집할 수 없습니다. 기존 호출 전용 광고를 보거나, 상태를 변경하거나, 삭제할 수 있습니다.

* 검색 캠페인의 [!DNL Google Ads] 및 [!DNL Microsoft Advertising]개 동적 검색 광고 그룹에 대해 **확장된 동적 검색 광고**(이제 광고 네트워크에서 &quot;동적 검색 광고&quot;라고 함). 동적 검색 광고는 키워드 대신 웹 사이트의 콘텐츠를 사용하여 광고를 표시할 시기를 결정합니다. 광고 네트워크는 동적으로 헤드라인을 생성하고, 랜딩 페이지 URL과 디스플레이 URL을 선택하며, 최종 URL을 자동으로 생성합니다.

  동적 검색 광고에 대한 자세한 내용은 [[!DNL Google Ads] 설명서](https://support.google.com/google-ads/answer/2471185) 및 [[!DNL Microsoft Advertising] 설명서](https://help.ads.microsoft.com/#apex/ads/en/56794)를 참조하세요.

* [!DNL Microsoft Advertising] 검색 캠페인에 대한 **멀티미디어 광고**. 멀티미디어 광고는 눈에 띄는 메인 라인과 사이드바 위치에 표시되는 대형 이미지 광고이며, 페이지당 하나의 멀티미디어 광고만 표시됩니다. 여기에는 반응형 광고와 같은 여러 텍스트 및 이미지 자산이 포함될 수 있으며 광고 네트워크는 광고 요소의 가장 효과적인 조합을 사용하여 광고를 어셈블합니다. 멀티미디어 광고는 텍스트 광고 배치를 대체하지 않습니다.

* 쇼핑 네트워크의 **[!DNL Microsoft Advertising]개 제품(쇼핑) 광고**&#x200B;에 대한 프로모션 라인입니다. 쇼핑 광고는 키워드 대신 기존 [!DNL Microsoft Merchant Center] 제품 피드의 제품을 사용하여 광고를 표시할 방법과 위치를 결정합니다. 광고 복사 및 랜딩 페이지 URL은 피드의 제품 정보에서 자동으로 생성되지만 선택적으로 광고 그룹에 포함할 프로모션 라인을 설정할 수 있습니다.

  제품 광고에 대한 자세한 내용은 [Microsoft Advertising 설명서](https://help.ads.microsoft.com/#apex/3/en/51082)를 참조하세요.

* 검색 네트워크의 [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 캠페인에 대해 **반응형 검색 광고**. 광고 네트워크는 광고 제목 및 설명 세트에서 텍스트 기반 반응형 검색 광고를 동적으로 어셈블하며, 함께 잘 작동하는 조합을 선호합니다. 이 광고에는 최대 3개의 헤드라인, 2개의 설명 및 기본 URL과 선택적 경로1 및 경로2 필드의 사용자 지정 가능한 URL이 포함되어 있습니다. 광고 제목과 설명을 특정 위치에 선택적으로 고정할 수 있습니다.

  >[!NOTE]
  >
  >[!DNL Google Ads]은(는) 기본 편집기 외부에서 광고로 표시된 텍스트 조합에 대한 데이터를 제공하지 않습니다. 각 텍스트 조합에 대한 보고에 대한 자세한 내용은 [Google 광고 설명서](https://support.google.com/google-ads/answer/7684791)를 참조하세요.

### 광고 수준 성능 데이터

광고 수준 데이터는 대부분의 광고 유형에 사용할 수 있습니다.

그러나 [!DNL Google Ads] 동적 검색 광고(DSA), 성능 최대, 스마트 쇼핑 및 [!DNL YouTube] 캠페인에는 사용할 수 없습니다. 캠페인에 대한 총 광고 수준 데이터와 캠페인에 대한 총 데이터 간의 불일치를 예상합니다.

| 광고 네트워크/캠페인/광고 유형 | 데이터 가용성 |
|---|---|
| [!DNL Google Ads] 동적 검색 광고(DSA) | 캠페인, 광고 그룹 |
| 최대 [!DNL Google Ads] 성능 | 캠페인 |
| [!DNL Google Ads] 쇼핑, 스마트 쇼핑 | 캠페인, 광고 그룹 |
| [!DNL Google Ads] [!DNL YouTube] | 캠페인, 광고 그룹 |

## 광고 만들기 {#ad-create}

<!-- Verify that this note is still applicable -->

>[!NOTE]
>
>* 쇼핑 캠페인을 위해 제품 광고를 만들 필요가 없습니다. 광고 네트워크에서 자동으로 만듭니다. 그러나 [!DNL Microsoft Advertising] 쇼핑 캠페인의 경우 선택적으로 광고에 포함할 프로모션 라인을 정의할 수 있습니다.
>* [!DNL Google Ads] 통화 전용 광고를 만들 수 없습니다.

>[!TIP]
>
>한 번에 많은 광고를 만들려면 [캠페인 일괄 시트](/help/search-social-commerce/new-ui/set-up/bulksheets/about.md)를 사용하십시오.

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Ads]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Create Ads]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Basic Settings]** 단계에서 네트워크, 계정, 캠페인, 광고 그룹 및 광고 유형을 선택합니다.

   사용 가능한 광고 유형에 대한 자세한 내용은 &quot;[사용 가능한 광고 유형](#ad-types)&quot;을 참조하십시오.

1. [Baidu 텍스트 광고](ad-settings-baidu-text.md), [Google 광고 확장 동적 검색 광고](ad-settings-google-dsa.md)(Google 광고에서 &quot;동적 검색 광고&quot;라고 함), [Google 광고 반응형 검색 광고](ad-settings-google-rsa.md), [Microsoft Advertising 확장 동적 검색 광고](ad-settings-microsoft-dsa.md), [Microsoft Advertising 멀티미디어 광고](ad-settings-microsoft-multimedia.md), [Microsoft Advertising 제품 광고](ad-settings-microsoft-product.md), [Microsoft 반응형(대상) 광고](ad-settings-microsoft-responsive.md), [Advertising 반응형 검색 광고](ad-settings-microsoft-rsa.md) 또는 [Yandex 텍스트 광고](ad-settings-yandex-text.md) 설정에 대한 나머지 설정을 지정합니다.

   >[!NOTE]
   >
   >(Adobe Advertising 전환 추적이 있는 캠페인) 계정 또는 캠페인 설정에서 키워드 수준에서만 추적을 지정하는 경우 검색, 소셜 및 Commerce에서 광고에 대한 추적을 생성하지 않습니다.

1. **[!UICONTROL Review and Save]**&#x200B;을(를) 클릭합니다.

1. 필요한 경우 ![편집](/help/search-social-commerce/assets/edit-new.png "편집") **[!UICONTROL Edit]**&#x200B;을(를) 클릭하고 광고 설정을 변경합니다.

1. **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

1. &#x200B;<!-- Add link to where to generate this once available to users-->(Adobe Advertising 전환 추적을 사용하는 캠페인의 쇼핑 광고, 선택 사항) 광고 클릭을 추적하려면 계정, 캠페인 또는 제품 그룹 설정에 추적 URL을 수동으로 추가하십시오.

## 광고 이름 바꾸기 {#ad-rename}

전체 광고 설정을 열지 않고 광고의 이름을 빠르게 변경합니다.

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Ads]**&#x200B;을(를) 클릭합니다.

1. 광고 행 위에 커서를 놓고 **[!UICONTROL ...]>[!UICONTROL Rename]**&#x200B;을(를) 클릭합니다.

1. 이름을 편집한 다음 **[!UICONTROL Apply]**&#x200B;을(를) 클릭합니다.

## 광고 설정 편집 {#ad-edit}

>[!NOTE]
>
>* 다음 광고 유형은 *변경 가능*&#x200B;입니다. 즉, 광고 사본 또는 이미지를 변경하고 동일한 광고 ID를 유지할 수 있습니다. 동적 검색 광고를 제외한 모든 [!DNL Google Ads] 광고 유형 및 [!DNL Microsoft Advertising] 확장된 텍스트 광고.
>* 기타 지원되는 모든 광고는 *변경할 수 없음*&#x200B;입니다. 즉, 광고 복사본 또는 이미지를 변경하면 기존 광고가 삭제되고 새 광고가 만들어집니다. 검색, 소셜 및 Commerce이 최적화를 위해 충분한 데이터를 수집하는 동안 새 광고의 성능은 2주 동안 불안정할 수 있습니다.
>* [!DNL Microsoft Advertising] 제품 광고의 프로모션 라인을 제외하고 제품 광고의 콘텐츠를 편집할 수 없습니다. 그러나 광고를 일시 중지하거나 삭제할 수 있습니다.
>* [!DNL Google Ads] 통화 전용 광고를 편집할 수 없습니다. 그러나 일시 중지하거나 삭제할 수 있습니다.
>* 한 번에 하나의 광고만 편집할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Ads]**&#x200B;을(를) 클릭합니다.

1. 광고 옆에 있는 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. [Baidu 텍스트 광고](ad-settings-baidu-text.md), [Google 광고에서 확장된 동적 검색 광고](ad-settings-google-dsa.md)(이제 Google 광고에서 &quot;동적 검색 광고&quot;라고 함), [Google 광고 반응형 검색 광고](ad-settings-google-rsa.md), [Microsoft Advertising 확장된 동적 검색 광고](ad-settings-microsoft-dsa.md), [Microsoft Advertising 멀티미디어 광고](ad-settings-microsoft-multimedia.md), [Microsoft Advertising 제품 광고](ad-settings-microsoft-product.md), [Microsoft 반응형(대상) 광고](ad-settings-microsoft-responsive.md), [Advertising Microsoft 반응형 검색 광고](ad-settings-microsoft-rsa.md) 또는 [Yandex 텍스트 광고](ad-settings-yandex-text.md) 설정의 나머지 설정을 편집합니다.

1. **[!UICONTROL Review and Save]**&#x200B;을(를) 클릭합니다.

1. 필요한 경우 ![편집](/help/search-social-commerce/assets/edit-new.png "편집") **[!UICONTROL Edit]**&#x200B;을(를) 클릭하고 광고 설정을 변경합니다.

1. **[!UICONTROL Update]**&#x200B;을(를) 클릭합니다.

## 광고 상태 변경 {#ad-status}

전체 광고 설정을 열지 않고도 광고의 상태를 빠르게 변경할 수 있습니다.

지원되는 광고 네트워크에서 활성 광고를 일시 중지하여 입찰을 비활성화할 수 있습니다. 나중에 상태를 다시 활성으로 변경하여 입찰을 다시 시작할 수 있습니다.

활성 광고나 일시 중지된 광고를 삭제할 수도 있습니다. 삭제된 광고는 광고 네트워크에서 삭제됩니다. 이러한 데이터는 데이터 필터에 포함할 때 계속 표시되지만 변경할 수는 없습니다.

### 광고 활성화 또는 일시 중지

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Ads]**&#x200B;을(를) 클릭합니다.

1. 광고 행의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 상태를 변경합니다.

   * 일시 중지된 광고를 활성화하려면 **[!UICONTROL Activate]**&#x200B;을(를) 클릭합니다.

   * 활성 광고를 일시 중지하려면 **[!UICONTROL Pause]**&#x200B;을(를) 클릭합니다.

### 광고 삭제

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Ads]**&#x200B;을(를) 클릭합니다.

1. 광고 행의 확인란을 선택합니다.

1. 일괄 작업 도구 모음에서 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Confirm]**&#x200B;을(를) 클릭합니다.

## [!UICONTROL Ads] 보기에서 데이터 보기 보고서 관리 {#ad-reports}

[!UICONTROL Ads] 보기에서 하나 이상의 광고에 대한 데이터 행을 포함하는 보고서를 생성한 다음 보고서를 Microsoft Excel 워크시트 파일(XLXS 형식)로 다운로드합니다. 이 보고서에는 보기에 표시된 모든 열이 포함됩니다.

생성된 보고서는 삭제할 수 있습니다.

또한 &quot;[(기존 UI) 캠페인 관리 보기에서 데이터 다운로드](/help/search-social-commerce/common-tasks/navigation-editing-selection/download.md)&quot; 및 &quot;[(기존 UI) [!UICONTROL Downloads] 메뉴에서 성능 데이터 보고서 또는 일괄 시트 파일 삭제](/help/search-social-commerce/common-tasks/navigation-editing-selection/download-delete-data.md)&quot;를 참조하십시오.

### 필터링된 데이터 행으로 보고서 생성

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Ads]**&#x200B;을(를) 클릭합니다.

1. 다운로드할 데이터의 광고를 지정합니다.

   * 특정 광고에 대한 데이터를 다운로드하려면 광고 옆에 있는 확인란을 선택합니다.

   * 모든 광고의 데이터를 다운로드하려면 확인란을 선택할 필요가 없습니다. 기본적으로 모든 광고가 포함됩니다.

1. 데이터 테이블 위의 도구 모음에서 ![보고서 다운로드](/help/search-social-commerce/assets/download.png "보고서 다운로드") **[!UICONTROL Reports]**&#x200B;를 클릭합니다.

1. [!UICONTROL Grid Reports] 설정에서 고유한 보고서 이름을 입력한 다음 **[!UICONTROL Generate]**&#x200B;을(를) 클릭합니다.

   기본적으로 파일 이름은 &quot;ad_YYYYMMDD_NNNN&quot;으로 지정됩니다. 여기서 &quot;NNNN&quot;은 순차적 작업 번호입니다(예: &quot;ad_20250402_1326).

   파일이 [!UICONTROL Recently Generated] 목록에 추가됩니다.

1. (선택 사항) 파일이 완료되면 다운로드하려면 파일 이름 옆에 있는 ![다운로드](/help/search-social-commerce/assets/download.png "다운로드")를 클릭합니다.

   브라우저의 일반적인 절차에 따라 파일이 다운로드됩니다.

### 완료된 보고서 다운로드

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Ads]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위의 도구 모음에서 ![보고서 다운로드](/help/search-social-commerce/assets/download.png "보고서 다운로드") **[!UICONTROL Reports]**&#x200B;를 클릭합니다.

1. [!UICONTROL Grid Reports] 대화 상자의 [!UICONTROL Recently Generated] 목록에서 파일 이름 옆에 있는 ![다운로드](/help/search-social-commerce/assets/download.png "다운로드")를 클릭합니다.

   브라우저의 일반적인 절차에 따라 파일이 다운로드됩니다.

### 완료된 보고서 삭제

1. 메인 메뉴에서 **[!UICONTROL Manage]>[!UICONTROL Ads]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위의 도구 모음에서 ![보고서 다운로드](/help/search-social-commerce/assets/download.png "보고서 다운로드") **[!UICONTROL Reports]**&#x200B;를 클릭합니다.

1. [!UICONTROL Grid Reports] 대화 상자의 [!UICONTROL Recently Generated] 목록에서 파일 이름 옆에 있는 ![삭제](/help/search-social-commerce/assets/delete-new.png "삭제")를 클릭합니다.

>[!MORELIKETHIS]
>
>* [[!DNL Baidu] 텍스트 광고 설정](ad-settings-baidu-text.md)
>* [[!DNL Google Ads] 확장된 동적 검색 광고 설정](ad-settings-google-dsa.md)
>* [[!DNL Google Ads] 반응형 검색 광고 설정](ad-settings-google-rsa.md)
>* [[!DNL Microsoft Advertising] 확장된 동적 검색 광고 설정](ad-settings-microsoft-dsa.md)
>* [[!DNL Microsoft Advertising] 멀티미디어 광고 설정](ad-settings-microsoft-multimedia.md)
>* [[!DNL Microsoft Advertising] 제품 광고 설정](ad-settings-microsoft-product.md)
>* [[!DNL Microsoft Advertising] 응답형(대상) 광고 설정](ad-settings-microsoft-responsive.md)
>* [[!DNL Microsoft Advertising] 반응형 검색 광고 설정](ad-settings-microsoft-rsa.md)
>* [[!DNL Yandex] 텍스트 광고 설정](ad-settings-yandex-text.md)
