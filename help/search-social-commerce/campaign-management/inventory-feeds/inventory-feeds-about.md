---
title: 인벤토리 피드를 사용한 광고 관리 자동화 정보
description: 제품 또는 서비스 인벤토리에 대한 데이터를 기반으로 계정 구조를 자동으로 관리하고 동적 광고를 게재할 수 있는 고급 캠페인 관리에 대해 알아봅니다.
exl-id: 46e78f32-96ef-4a23-bbe3-f18b84309463
feature: Search Inventory Feeds
source-git-commit: 67fe8581832dc0762d62908d01672e53cc95b847
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 0%

---

# 인벤토리 피드를 사용한 광고 관리 자동화 정보

*[!DNL Google Ads], [!DNL Microsoft Advertising], [!DNL Yahoo! Japan Ads](삭제 작업만) 및 [!DNL Yandex] 계정만*

고급 캠페인 관리를 위한 [!UICONTROL Campaigns] > [!UICONTROL Advanced (ACM)] 보기를 사용하면 광고 네트워크 계정 구조를 자동으로 만들고 업데이트하며 제품 또는 서비스 인벤토리에 대한 데이터를 기반으로 동적 광고를 게재할 수 있습니다. 매일 또는 원하는 횟수만큼 제품 데이터가 포함된 새 파일을 업로드하거나 [!DNL Google] 또는 [!DNL Microsoft] 가맹점 센터 계정에 직접 연결할 수 있습니다. 이 기능을 사용하여 다음을 수행할 수 있습니다.

* 순서가 지정된 데이터 소스에서 새 캠페인을 빌드합니다.

* 변경 가능한 데이터 요소(예: 가격 또는 수량)에 대해 동적 변수를 사용하여 새 데이터가 처리될 때마다 텍스트 및 반응형 검색 광고, [!DNL Google Ads]개 쇼핑 광고 또는 [!DNL Microsoft Advertising]개 쇼핑 광고를 동적으로 업데이트합니다. 데이터를 변경할 때마다 기존 광고가 삭제되고 새 광고가 만들어집니다.

* 지정된 종료 날짜에 따라 특정 수준 이하로 재고가 감소하거나 피드 데이터에서 기존 구성 요소를 생략하는 경우 광고 그룹, 키워드 및 광고를 자동으로 일시 중지하거나 제거합니다.

광고를 설정하려면 변수(자리 표시자)가 포함된 인벤토리 피드 템플릿을 만든 다음 이 변수를 업로드된 파일 또는 [동기화된 Google 또는 Microsoft 판매자 센터 계정의 실제 데이터 열로 대체](/help/search-social-commerce/campaign-management/accounts/merchant-account-manage.md)하십시오. 변수에는 파일에 설정한 수정자 그룹 또는 파일의 개별 행을 포함하여 데이터 파일의 각 적용 가능한 행에 대해 여러 광고, 키워드, 캠페인 또는 광고 그룹을 생성할 수도 있습니다. 예를 들어, 광고 헤드라인에 수정자 그룹 변수를 사용하고 수정자 그룹에 두 개의 수정자(&quot;저렴한 경우&quot; 및 &quot;할인된 경우&quot;)가 포함된 경우 각 제품에 대해 두 개의 개별 광고(수정자마다 하나씩)가 만들어집니다. [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 동적 검색 광고의 경우 광고 사용자 지정자에 대한 값도 포함할 수 있습니다.

| 템플릿의 [!UICONTROL Ad Variation] 섹션 | 검색, 소셜 및 Commerce의 수정자 | 피드 콘텐츠 | 결과 광고 |
|----|----|----|----|
| 제목: 고급 \{<i>제품 범주</i>\} &lt;<i>CheapList</i>> 구매<br><br>설명 1: \{<i>제품 이름</i>\}의 큰 인벤토리.<br><br>설명 2: \{<i>할인율</i>\}%에서 사용할 수 있습니다. | 수정자 그룹 &quot;CheapList&quot;의 값:<br><br>&quot;저렴한 값&quot;<br><br>&quot;할인&quot; | 제품 범주,제품 이름,할인율<br>전자 제품,iPod,10<br><br>의류,셔츠,15<br><br><b>참고:</b> 쉼표나 탭으로 값을 구분할 수 있습니다. | <u>저렴한 가격으로 고급 전자 제품을 구입하십시오.</u><br>태블릿의 많은 인벤토리. 10% 할인가로 이용 가능합니다.<br><br><u>할인된 가격으로 고급 전자 제품을 구입하십시오.</u><br>태블릿의 많은 인벤토리. 10% 할인가로 이용 가능합니다.<br><br><u>저렴한 가격으로 고급 의류를 구입하십시오.</u><br>많은 수의 셔츠가 있습니다. 15% 할인가로 이용 가능합니다.<br><br><u>할인된 가격으로 고급 의류를 구입하세요.</u><br>많은 수의 셔츠가 있습니다. 15% 할인가로 이용 가능합니다. |

광고를 생성하면 선택적으로 검토한 다음 광고 네트워크에 게시할 수 있습니다.

>[!NOTE]
>스프레드시트 파일을 사용하여 캠페인 데이터를 대량으로 만들거나 편집하려면 &quot;[일괄 시트를 사용한 캠페인 데이터 관리 정보](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-about.md)&quot;를 참조하십시오.

## 재고 피드를 사용한 캠페인 데이터 관리 워크플로우

*[!DNL Google Ads], [!DNL Microsoft Advertising], [!DNL Yahoo! Japan Ads](삭제 작업만) 및 [!DNL Yandex] 계정만*

처음에는 적어도 한 개의 피드 파일 또는 계정을 테스트한 다음 프로세스를 완전히 자동화하거나 각 단계에서 계속 제어할 수 있습니다.

1. (선택 사항) 데이터 파일을 저장하기 위한 FTP 디렉터리를 설정하려면 Adobe 계정 팀에 문의하십시오.

   FTP 디렉터리를 사용하는 경우 피드 서비스는 2시간마다 새 파일을 확인합니다.

   그렇지 않으면 [!UICONTROL Advanced (ACM)] 보기에서 파일을 수동으로 업로드할 수 있습니다.

1. 피드 데이터를 처리하기 위한 [매개 변수를 설정합니다](feed-settings-manage.md#feed-data-settings).

   FTP를 사용하는 경우 처음에 데이터를 광고 네트워크에 자동으로 게시하지 마십시오. 첫 번째 파일의 출력을 확인하고 결과에 만족하면 설정을 변경할 수 있습니다.

1. FTP 디렉터리에 데이터 파일을 업로드하거나, [데이터 파일을 수동으로 업로드](feed-files-manage.md)하거나, [Google 또는 Microsoft 판매자 센터 계정에 대한 액세스 사용](/help/search-social-commerce/campaign-management/accounts/merchant-account-manage.md)하십시오.[!UICONTROL Advanced (ACM) view]

파일을 수동으로 업로드하려면 데이터 파일을 사용하는 템플릿을 만들 때까지 기다릴 수 있습니다.

1. (선택 사항) 피드 데이터 템플릿의 다양한 데이터 필드에 변수로 사용할 [수정자](modifiers-manage.md) 그룹을 만듭니다.

1. 데이터 열을 사용하여 특정 광고 네트워크 계정에 대한 캠페인, 광고 그룹, 키워드 및/또는 광고 복사본을 만드는 [하나 이상의 템플릿을 만듭니다](ad-templates/ad-template-manage.md).

1. [템플릿을 통해 피드 데이터를 전파합니다](feed-data-propagate.md). 템플릿의 열 이름을 파일 또는 계정의 데이터로 대체합니다. 템플릿 옵션에 따라 검색, 소셜 및 Commerce은 기본 설정을 사용하여 광고에 대한 새 계정 구조(캠페인, 광고 그룹, 키워드)를 만들거나 광고를 기존 계정 구조에 매핑합니다.

1. (선택 사항) [출력을 미리 봅니다](propagated-data-view.md). [!UICONTROL Advanced (ACM)] 보기에서 선택적으로 [!UICONTROL Propagations] 탭에서 데이터 변경 사항에 대한 요약을 봅니다.

1. 관련 광고 네트워크 계정에 [데이터를 게시](propagated-data-post.md)합니다.

1. (FTP 또는 판매자 센터 계정을 사용하여 데이터를 업로드하는 경우, 선택 사항) 첫 번째 피드 파일의 출력을 확인한 후 [매개 변수를 편집](feed-settings-manage.md#feed-data-settings)하여 후속 데이터를 관련 템플릿을 통해 자동으로 전파하고 관련 광고 네트워크에 게시합니다.

1. (새 데이터 파일이 있는 경우) 필요한 경우 새 파일을 업로드하고, 템플릿을 통해 데이터를 전파하고, 관련 광고 네트워크에 데이터를 게시합니다. 선택적으로 한 단계로 데이터를 전파하고 게시할 수 있습니다.

>[!MORELIKETHIS]
>
>* [재고 피드에서 계정 구성 요소를 만들거나 삭제하는 경우는 언제입니까?](when-are-components-created-deleted.md)
