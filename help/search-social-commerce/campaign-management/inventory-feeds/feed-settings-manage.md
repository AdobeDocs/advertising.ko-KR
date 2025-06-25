---
title: 피드 데이터 설정 구성
description: 피드 데이터 처리 방법을 제어하는 설정을 구성하는 방법에 대해 알아봅니다.
exl-id: 7eaac751-ecdf-4e73-9eae-a961bd9b7360
feature: Search Inventory Feeds
source-git-commit: d0f1c413134a0868ddec79ded7672af316267edd
workflow-type: tm+mt
source-wordcount: '1155'
ht-degree: 0%

---

# 피드 데이터 설정 구성

*[!DNL Google Ads], [!DNL Microsoft Advertising], [!DNL Yahoo! Japan Ads]&#x200B;(삭제 작업만) 및 [!DNL Yandex] 계정만*

피드 데이터 파일에서 광고 그룹, 키워드 및 광고를 처리하는 방법과 피드 설정을 통해 특히 FTP 파일의 데이터를 처리하는 방법을 구성할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Search, Social, & Commerce]> [!UICONTROL Campaigns] >[!UICONTROL Advanced (ACM)]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL Settings]**&#x200B;을(를) 클릭합니다.

1. [피드 데이터 설정 지정](#feed-data-settings):

   1. [!UICONTROL Obsolete Item Auto-Processing] 섹션에서 필드에 있는 정보를 선택합니다.

   1. (FTP를 통해 또는 판매자 센터 계정에 대한 직접 링크를 통해 데이터를 업로드하는 광고주) [!UICONTROL FTP/GMC Account Auto-Processing] 섹션에서 필드에서 정보를 선택합니다.

   1. [!UICONTROL Miscellaneous Auto-Processing] 섹션에서 필드에 있는 정보를 선택합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 피드 데이터 설정 {#feed-data-settings}

**[!UICONTROL Enable obsolete item auto-processing for]:** 모든 [!UICONTROL Obsolete Item Auto-processing] 설정을 적용할 대상:

* *[!UICONTROL Ad Groups Only]:* 사용되지 않는 광고 그룹만.

* *[!UICONTROL Keywords Only]:* 사용되지 않는 키워드 및 제품 그룹만 해당됩니다.

* *[!UICONTROL Ad Variations Only]*(기본값): 사용되지 않는 광고만

* *[!UICONTROL Keywords and Ad Variations]:* 사용되지 않는 키워드/제품 타겟/제품 그룹 및 사용되지 않는 광고 둘 다.

>[!NOTE]
>
>* [!DNL Google Ads] 쇼핑 광고의 경우 가장 낮은 수준의 제품 그룹만 영향을 받습니다.
>* [!DNL Yandex] 계정의 경우 이 설정에 관계없이 광고 변형에 대해 사용되지 않는 항목 자동 처리 작업이 항상 수행됩니다.

**[!UICONTROL When the Scheduled End Date is reached]:**(수동으로 게시한 데이터만 해당) 지정한 종료 날짜 및 종료 시간이 되면 게시된 피드 파일의 라인 항목에 대한 작업:

* *[!UICONTROL Delete]*(기본값): 지정된 종료 시간이 되면 모든 관련 구성 요소를 삭제합니다. 이 작업을 되돌릴 수 없습니다.

* *[!UICONTROL Pause]:* 지정한 종료 시간이 되면 모든 관련 구성 요소를 일시 중지합니다. 필요한 경우 나중에 구성 요소를 다시 활성화할 수 있습니다.

* *[!UICONTROL None]:* 관련 구성 요소의 상태를 변경하지 마십시오.

**[!UICONTROL Missing line items in a manually uploaded feed]:** 기존 항목이 수동으로 업로드된 새 피드 파일에 포함되지 않았거나 템플릿의 맵 전용 설정에 따라 기존 캠페인 또는 광고 그룹에 매핑되지 않는 경우 수행할 작업:

* *[!UICONTROL Delete]:* 기존 구성 요소를 삭제합니다.

* *[!UICONTROL Pause]:* 기존 구성 요소를 일시 중지합니다. 새 피드 파일에 동일한 라인 항목이 포함되어 있는 경우 다시 활성화되며 기록 및 품질 점수가 유지됩니다. **참고:** 상위 제품 그룹의 모든 하위 제품 그룹이 누락된 경우 제품 그룹을 일시 중지할 수 없으므로 상위 제품 그룹이 삭제됩니다.

* *[!UICONTROL None]*(기본값): 기존 구성 요소를 변경하지 마십시오.

**[!UICONTROL Missing line items in an FTP feed/GMC account]:** 1) 항목이 포함되지 않은 경우(a) FTP 디렉터리에 업로드된 새 피드 파일의 항목 또는 b) 다음에 검색, 소셜 및 Commerce이 동기화되는 머천트 센터 계정의 항목 또는 2) 템플릿의 [!UICONTROL Map Only] 설정에 따라 기존 캠페인 또는 광고 그룹에 매핑되지 않은 경우 기존 항목을 어떻게 해야 합니까?

* *[!UICONTROL Delete]:* 기존 구성 요소를 삭제합니다.

* *[!UICONTROL Pause]:* 기존 구성 요소를 일시 중지합니다. 새 데이터에 동일한 라인 항목이 포함되어 있는 경우 다시 활성화되며 기록 및 품질 점수가 유지됩니다. **참고:** 상위 제품 그룹의 모든 하위 제품 그룹이 누락된 경우 제품 그룹을 일시 중지할 수 없으므로 상위 제품 그룹이 삭제됩니다.

* *[!UICONTROL None]*(기본값): 기존 구성 요소를 변경하지 마십시오.

**[!UICONTROL When a numeric stock level reaches N units, or where a text-based value is 'out of stock']:** 다음의 경우 재고 수준이 포함된 라인 항목으로 수행할 작업:

* (지정된 열에 숫자 전용 재고 값이 있는 피드의 경우) 재고 레벨은 지정된 수량보다 작거나 같습니다. 기본 수량은 영(0)입니다.

* (지정한 열에 텍스트 값이 있는 피드의 경우) [!UICONTROL Availability]의 값은 &quot;[!UICONTROL out of stock]&quot;입니다. 값은 대/소문자를 구분하지 않습니다. **참고:** **피드 템플릿에서 &quot;[!UICONTROL This column has non-numeric values]&quot;에 대한 확인란을 사용하여 텍스트 기반 재고 수준 열을 지정하십시오.&quot;

두 경우 모두에 대한 작업을 선택합니다.

* *[!UICONTROL Delete]*(기본값) 구성 요소를 삭제합니다.

* *[!UICONTROL Pause]:* 구성 요소를 일시 중지합니다. 데이터가 업데이트되면 숫자 재고 값이 지정된 수량을 초과하거나 [!UICONTROL Availability]이(가) &quot;[!UICONTROL in stock]&quot; 또는 &quot;[!UICONTROL preorder]&quot;인 경우 구성 요소가 다시 활성화됩니다. 구성 요소의 기록 및 품질 점수가 유지됩니다.

각 라인 항목의 재고 수준은 각 템플릿에 대한 &quot;[!UICONTROL Stock Level]&quot; 필드에 지정된 대로 피드 파일의 열에서 가져옵니다.

>[!TIP]
>
>* 재입고 또는 가용성 증가가 예상되는 제품 또는 서비스의 경우 광고 그룹, 키워드 및 광고를 삭제하고 다시 만드는 대신 일시 중지해야 합니다. 일시 정지를 하면 품질 점수를 유지할 수 있습니다.
>* 광고 그룹에 대해 더 이상 사용되지 않는 자동 처리를 활성화하고 새 데이터에 광고 그룹에 대한 재고 수준이 포함된 경우, 지정된 재고 수준이 브랜드/항목 수준이 아닌 범주 수준에 있는 경우에만 광고 그룹을 삭제하거나 일시 중지하는 것이 중요합니다. 예를 들어 광고 그룹 &quot;컨버터블&quot;이 있는 경우 광고 그룹에 대한 재고 수준은 광고 그룹에 표시된 모든 개별 컨버터블 모델에 대한 합계여야 합니다.

**[!UICONTROL Propagate feed data through all applicable templates]:**(FTP 또는 판매자 센터 계정을 통해 데이터 파일을 업로드하는 광고주) 적용 가능한 템플릿을 통해 새 데이터를 자동으로 전파합니다. 이 옵션은 기본적으로 선택되어 있습니다. 옵션을 비활성화해도 피드 파일, 계정 또는 템플릿에 대한 데이터를 수동으로 전파할 수 있습니다.

>[!NOTE]
>
>* FTP 파일의 경우 피드 서비스는 2시간마다(PST 시간대의 짝수 시간) FTP 디렉터리에서 업데이트를 확인합니다. 이 옵션은 마지막 확인 이후 업로드된 모든 파일을 처리합니다.
>* 판매자 센터 계정의 경우 검색, 소셜 및 Commerce이 광고주 시간대의 약 06:00에 매일 계정과 동기화됩니다. 이 옵션은 마지막 동기화 이후 업데이트된 모든 데이터를 처리합니다.
>* 전파된 데이터는 광고 네트워크나 [!UICONTROL Bulksheets] 보기에 게시될 때까지 [!UICONTROL Campaigns], [!UICONTROL Ad Groups], [!UICONTROL Keywords] 및 [!UICONTROL Ads] 탭에서 사용할 수 있습니다.

**[!UICONTROL Post to the SE]:**(FTP 또는 판매자 센터 계정을 통해 데이터 파일을 업로드하는 광고주) 새 데이터가 해당 템플릿을 통해 전파된 후 관련 광고 네트워크에 대한 올바른 형식으로 일괄 시트 파일을 자동으로 만듭니다. 하위 구성 요소에 오류가 없는 한 이 옵션은 [!UICONTROL Campaigns], [!UICONTROL Ad Groups], [!UICONTROL Keywords] 및 [!UICONTROL Ads] 탭에서도 데이터를 제거합니다.

이 옵션은 기본적으로 비활성화되어 있습니다. 이 옵션을 활성화하려면 확인란을 선택한 다음 일괄 시트 파일을 광고 네트워크에 게시할지 여부를 지정합니다.

* *[!UICONTROL Immediately]*(기본값): 데이터가 템플릿을 통해 전파된 후 대량 시트 파일을 관련 광고 네트워크에 게시합니다. 일괄 시트 파일은 30일 동안 [!UICONTROL Bulksheets] 보기에서 사용할 수 있습니다.

* *[!UICONTROL Preview in Bulksheet Management area only, post later]:** 일괄 시트 파일을 관련 광고 네트워크에 게시하지 않지만 나중에 게시할 수 있는 [!UICONTROL Bulksheets] 보기에 나열합니다. 일괄 시트 파일은 30일 동안 [!UICONTROL Bulksheets] 보기에서 사용할 수 있습니다. 일괄 시트 파일이 10MB보다 크지만 2GB보다 작은 경우 파일이 ZIP 형식이므로 게시하기 위해 파일의 압축을 풀 필요가 없습니다. **팁:** 이전에 랜딩 페이지의 유효성을 검사하지 않았다면 이 옵션을 사용하여 데이터를 광고 네트워크에 게시하기 전에 [!UICONTROL Bulksheets] 보기에서 유효성을 검사할 수 있습니다.

**[!UICONTROL Exclude keywords from posting when keyword length is greater than]:**&#x200B;은(는) 지정된 단어 수가 넘는 키워드 구문을 광고 네트워크에 게시하지 못하도록 합니다. 이 옵션을 선택하면 최대 단어 수를 초과하는 키워드 구문이 전파되어 [!UICONTROL Keywords] 탭에 나열되지만 데이터를 게시하려고 하면 게시되지 않습니다.

이 옵션은 구문에 포함된 단어 수에 관계없이 모든 키워드가 게시되도록 기본적으로 비활성화됩니다. 이 옵션을 선택하는 경우 게시할 최대 단어 수(3~10개)를 선택하십시오.

>[!MORELIKETHIS]
>
>* [인벤토리 피드 정보](/help/search-social-commerce/campaign-management/inventory-feeds/inventory-feeds-about.md)
>* [템플릿을 통해 피드 데이터 전파](/help/search-social-commerce/campaign-management/inventory-feeds/feed-data-propagate.md)
>* [피드에서 생성된 캠페인 데이터를 광고 네트워크에 게시](propagated-data-post.md)
