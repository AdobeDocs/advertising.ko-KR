---
title: 인벤토리 피드에 대한 광고 템플릿 관리
description: 계정 구조를 관리하고 동적 광고를 게재하기 위해 인벤토리 데이터를 처리할 수 있는 광고 템플릿 관리에 대해 알아봅니다.
exl-id: b0e540cf-8735-4812-9df5-58f488a25ba5
feature: Search Inventory Feeds
source-git-commit: 67fe8581832dc0762d62908d01672e53cc95b847
workflow-type: tm+mt
source-wordcount: '1423'
ht-degree: 0%

---

# 인벤토리 피드에 대한 광고 템플릿 관리

*[!DNL Google Ads], [!DNL Microsoft Advertising], [!DNL Yahoo! Japan Ads] (삭제 작업만) 및 [!DNL Yandex] 계정만*

데이터를 업로드하기 전이나 후에 데이터를 처리할 수 있는 검색 엔진별 광고 템플릿을 만들 수 있습니다. 텍스트 광고 및 확장/확장 텍스트 광고, [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 반응형 검색 광고, [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 쇼핑 광고에 대한 템플릿을 만들 수 있습니다.

각 템플릿을 하나의 피드 파일, [!DNL Google Merchant Center] 계정 또는 [!DNL Microsoft Merchant Center] 계정과 연결할 수 있으며, 동일한 피드 파일 또는 계정에 여러 템플릿을 연결할 수 있습니다. 광고 템플릿에는 업로드된 파일 또는 계정의 실제 데이터 열로 대체되는 변수가 포함될 수 있습니다. 대부분의 경우 변수에는 데이터 파일의 각 적용 가능한 행에 대해 여러 광고, 키워드, 캠페인 또는 광고 그룹을 만들기 위해 검색, 소셜 및 Commerce에서 설정한 [수정자 그룹](/help/search-social-commerce/campaign-management/inventory-feeds/modifiers-manage.md)도 포함될 수 있습니다. 템플릿 옵션을 사용하면 광고에 대한 새 계정 구조(캠페인, 광고 그룹, 키워드)를 만들거나 광고를 기존 계정 구조에 매핑할 수 있습니다.

새 템플릿을 처음부터 새로 만드는 것 외에도 선택적으로 기존 템플릿을 복제하여 새 템플릿을 만들고 기존 템플릿을 편집할 수 있습니다.

템플릿을 만들고 이를 데이터 피드 파일 또는 머천트 센터 계정과 연결하면 파일 내의 데이터를 템플릿을 통해 전파하여 캠페인 데이터 및 계정 구조를 만들 수 있습니다. 원할 경우 광고 네트워크에 즉시 게시하거나 검토할 일괄 시트 파일을 만들 수 있습니다.

모든 템플릿은 활성화, 일시 중지 또는 삭제할 수 있습니다. 피드 데이터는 활성 템플릿을 통해서만 자동으로 전파될 수 있습니다. 그러나 일시 중지된 템플릿을 통해 데이터를 수동으로 전파할 수 있습니다.

## 피드 템플릿 만들기, 복제 또는 편집

텍스트 및 확장/확장 텍스트 광고, 반응형 검색 광고, [!DNL Google Ads]개 쇼핑 광고 및 [!DNL Microsoft Advertising]개 쇼핑 광고에 대한 별도의 템플릿을 만듭니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Advanced (ACM)]**&#x200B;을(를) 클릭합니다. 그러면 [!UICONTROL Templates] 탭이 열립니다.

1. 다음 중 하나를 수행합니다.

   * 템플릿을 처음부터 만들려면 데이터 테이블 위의 도구 모음에서 **[!UICONTROL Create/Clone]**&#x200B;을(를) 클릭한 다음 해당 광고 네트워크를 선택합니다.

   * 기존 템플릿을 복제하려면 다음 작업을 수행하십시오.

      1. 복사할 템플릿 옆에 있는 확인란을 선택합니다.

      1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL Create/Clone]**&#x200B;을(를) 클릭하고 적용 가능한 광고 네트워크를 선택합니다.

   * (기존 템플릿을 편집하려면) 템플릿 이름 옆에 있는 ![설정 보기/편집](/help/search-social-commerce/assets/settings.png "설정 보기/편집")을 클릭합니다.

1. [텍스트 광고 템플릿](/help/search-social-commerce/campaign-management/inventory-feeds/ad-templates/template-text-rsa.md), [[!DNL Google Ads] 쇼핑 광고 템플릿](/help/search-social-commerce/campaign-management/inventory-feeds/ad-templates/template-google-shopping.md) 또는 [[!DNL Microsoft Advertising] 쇼핑 광고 템플릿](/help/search-social-commerce/campaign-management/inventory-feeds/ad-templates/template-microsoft-shopping.md)에 대한 설정을 지정하십시오.

   1. 템플릿 설정 창의 맨 위에서 템플릿 이름과 적용 가능한 계정을 지정합니다.

      기존 템플릿을 복제하는 경우 새 템플릿에서 만든 광고가 소스 템플릿에서 만든 광고와 연결되지 않도록 새 템플릿의 이름을 변경합니다.

   1. (선택 사항) 왼쪽 열에서 템플릿을 통해 데이터를 전파할 제품 피드 파일 또는 머천트 센터 계정을 지정합니다.

      * (제품 피드 파일의 경우) 이전에 업로드한 파일을 선택하려면 ![아래쪽 화살표](/help/search-social-commerce/assets/arrow-down-dropdown.png "아래쪽 화살표")를 클릭하고 사용 가능한 피드 파일 목록에서 파일을 선택하십시오. 새 파일을 업로드하려면 전체 경로와 파일 이름을 입력하거나 **[!UICONTROL Browse]**&#x200B;을(를) 클릭하여 장치 또는 네트워크에서 파일을 찾은 다음 **[!UICONTROL Upload]**&#x200B;을(를) 클릭하여 파일을 지정하십시오.

      * (동기화된 머천트 센터 계정의 경우) 계정 이름을 선택합니다.

      선택한 파일 또는 계정에 대한 열이 표시됩니다.

   1. **[!UICONTROL Account Structure]** 탭에서 계정 구조 설정을 지정합니다.

   1. (텍스트 광고만 해당) **[!UICONTROL Keywords]** 탭을 클릭하고 키워드 설정을 지정합니다.

   1. (텍스트 및 반응형 검색 광고만 해당) **[!UICONTROL Ads]** 탭을 클릭하고 다음 중 하나를 수행합니다.

      >[!NOTE]
      >
      >* 표준 텍스트 광고 템플릿당 최대 4개의 광고 변형 템플릿, 확장/확장 텍스트 광고 템플릿당 5개의 광고 변형 템플릿, 반응형 검색 광고 템플릿당 3개의 광고 변형 템플릿을 포함할 수 있습니다.
      >* 각 광고 그룹에는 최대 3개의 활성화된 반응형 검색 광고가 포함될 수 있습니다.
      >* 기존 표준 텍스트 광고 변형을 편집할 수 없으며, 기존 템플릿은 더 이상 표준 텍스트 광고를 생성하지 않습니다.
      >* 광고 변형 템플릿을 변경하면 광고 유형 및 광고 네트워크에 따라 [템플릿을 통해 데이터를 전파할 때 기존 광고가 삭제되고 새 광고가 생성될 수 있습니다](/help/search-social-commerce/campaign-management/inventory-feeds/when-are-components-created-deleted.md).

      * 광고 변형을 추가하려면 다음 작업을 수행하십시오.

         1. 텍스트 광고를 만들려면 **[!UICONTROL Add Ad Variation]**&#x200B;을(를) 클릭하고, 확장/확장된 텍스트 광고를 만들려면 **[!UICONTROL Add ETA Variation]**&#x200B;을(를) 클릭하고, 반응형 텍스트 광고를 만들려면 **[!UICONTROL Add RSA Variation]**&#x200B;을(를) 클릭합니다.

            광고 유형을 지정하고 나면 템플릿으로 해당 광고 유형만 만들 수 있습니다.

         1. 광고 설정을 지정합니다.

            반응형 검색 광고의 경우 3-15개의 헤드라인과 2-4개의 설명을 포함할 수 있습니다.

         1. (선택 사항) 모든 대체 광고 복사 필드를 원본 광고 복사 필드의 텍스트로 미리 채우려면 **[!UICONTROL Prefill]** 옆에 있는 확인란을 선택합니다.

         1. (선택 사항) 다른 광고 복사본 집합을 광고에 추가하려면, 원본 광고 복사본의 줄 중 하나라도 전파 중에 동적 매개 변수가 데이터로 대체되면 최대 길이를 초과하는 경우 사용할 수 있습니다. **[!UICONTROL Add Alternate]**&#x200B;을(를) 클릭한 다음 대체 값을 추가하십시오.

            >[!NOTE]
            >
            >* [!UICONTROL Prefill] 옵션을 선택하면 대체 필드가 원본 필드로 미리 채워지며 필요에 따라 편집할 수 있습니다.
            >* 최대 길이를 초과하는 광고 복사 필드만 대체 값으로 바뀝니다. 예를 들어 원래 헤드라인이나 제목만 너무 긴 경우 생성된 광고 변형은 대체 헤드라인이나 제목과 원래 설명을 사용합니다. 따라서 대체 광고 사본을 원본 광고 사본과 결합할 때 적절한지 확인하십시오.
            >* 원본 광고 사본이 검색 엔진의 길이 요구 사항을 충족하면 대체 광고 사본은 무시됩니다.
            >* 각 광고 복사 필드에 대해 최대 4개의 대체를 지정할 수 있습니다.

         * 광고 변형을 편집하려면 다음 작업을 수행하십시오.

            1. 광고 설정을 편집합니다.

               반응형 검색 광고의 경우 3-15개의 헤드라인과 2-4개의 설명을 포함할 수 있습니다.

            1. (선택 사항) 모든 대체 광고 복사 필드를 원본 광고 복사 필드의 텍스트로 미리 채우려면 **[!UICONTROL Prefill]** 옆에 있는 확인란을 선택합니다.

            1. (선택 사항) 다른 광고 복사본 집합을 광고에 추가하려면, 원본 광고 복사본의 줄 중 하나라도 전파 중에 동적 매개 변수가 데이터로 대체되면 최대 길이를 초과하는 경우 사용할 수 있습니다. **[!UICONTROL Add Alternate]**&#x200B;을(를) 클릭한 다음 대체 값을 추가하십시오.

               >[!NOTE]
               >
               >* [!UICONTROL Prefill] 옵션을 선택하면 대체 필드가 원본 필드로 미리 채워지며 필요에 따라 편집할 수 있습니다.
               >* 최대 길이를 초과하는 광고 복사 필드만 대체 값으로 바뀝니다. 예를 들어 원래 헤드라인이나 제목만 너무 긴 경우 생성된 광고 변형은 대체 헤드라인이나 제목과 원래 설명을 사용합니다. 따라서 대체 광고 사본을 원본 광고 사본과 결합할 때 적절한지 확인하십시오.
               >* 원본 광고 사본이 검색 엔진의 길이 요구 사항을 충족하면 대체 광고 사본은 무시됩니다.
               >* 각 광고 복사 필드에 대해 최대 4개의 대체를 지정할 수 있습니다.

         * 광고 변형을 제거하려면 해당 광고 변형 옆에 있는 **[!UICONTROL Remove ETA Variation]**(확장/확장 텍스트 광고의 경우) 또는 **[!UICONTROL Remove RSA Variation]**(반응형 검색 광고의 경우)을 클릭합니다.

   1. (쇼핑 템플릿만 해당) **[!UICONTROL Product Groups]** 탭을 클릭한 다음 타깃팅할 제품 그룹에 대한 정보를 지정하십시오.

   1. (선택 사항) **[!UICONTROL Feed Filters]** 탭을 클릭한 다음 피드 파일에서 전파할 행을 지정합니다.

   1. (선택 사항) **[!UICONTROL Label Classifications tab]**&#x200B;을(를) 클릭한 다음, 만들 다른 캠페인 구성 요소에 지정할 레이블 분류 값을 지정합니다.

      1. **[!DNL \[Component\] Label Classifications]** 옆에 있는 확인란을 클릭합니다.

      1. 구성 요소에 지정할 각 레이블 분류에 대해 다음 작업을 수행하십시오.

         1. **[!UICONTROL Add Label Classification]**&#x200B;을(를) 클릭합니다.

         1. 레이블 분류를 선택한 다음 기존 값을 선택하거나 새 값을 입력합니다.

1. 템플릿을 저장합니다.

   * 템플릿을 저장하려면 **[!UICONTROL Save]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Save]**&#x200B;을(를) 다시 클릭합니다.

   * 템플릿을 저장하고 지정된 데이터 파일을 이 템플릿을 통해 전파하려면 **[!UICONTROL Save]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Save & Propagate]**&#x200B;을(를) 클릭합니다.

## 피드 템플릿 상태 변경

일시 중지된 데이터 피드 템플릿을 활성화하거나 활성 데이터 피드 템플릿을 일시 중지할 수 있습니다.

>[!NOTE]
>
>일시 중지된 템플릿을 통해 데이터를 수동으로 전파할 수는 있지만 데이터가 자동으로 전파되지는 않습니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Advanced (ACM)]**&#x200B;을(를) 클릭합니다. 그러면 [!UICONTROL Templates] 탭이 열립니다.

1. 상태를 변경할 각 템플릿 옆의 확인란을 선택합니다.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL Change Status]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Activate]** 또는 **[!UICONTROL Pause]**&#x200B;을(를) 클릭합니다.

## 피드 템플릿 삭제

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Advanced (ACM)]**&#x200B;을(를) 클릭합니다. 그러면 [!UICONTROL Templates] 탭이 열립니다.

1. 삭제할 각 템플릿 옆에 있는 확인란을 선택합니다.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Yes]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [인벤토리 피드를 사용하여 광고 관리 자동화 정보](../inventory-feeds-about.md)
>* [텍스트 광고 및 반응형 검색 광고 템플릿 설정](template-text-rsa.md)
>* [[!DNL Google Ads] 쇼핑 광고 템플릿 설정](template-google-shopping.md)
>* [[!DNL Microsoft Advertising] 쇼핑 광고 템플릿 설정](template-microsoft-shopping.md)
>* [템플릿을 통해 피드 데이터 전파](../feed-data-propagate.md)
