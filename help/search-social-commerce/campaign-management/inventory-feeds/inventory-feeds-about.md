---
title: 인벤토리 피드를 사용한 광고 관리 자동화 정보
description: 제품 또는 서비스 인벤토리에 대한 데이터를 기반으로 계정 구조를 자동으로 관리하고 동적 광고를 게재할 수 있는 고급 캠페인 관리에 대해 알아봅니다.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# 인벤토리 피드를 사용한 광고 관리 자동화 정보

*[!DNL Google Ads], [!DNL Microsoft® Advertising], [!DNL Yahoo! Japan Ads] (작업만 삭제) 및 [!DNL Yandex] 계정만*

다음 [!UICONTROL Campaigns] > [!UICONTROL Advanced (ACM)] 고급 캠페인 관리를 위한 보기를 사용하면 광고 네트워크 계정 구조를 자동으로 만들고 업데이트하고 제품 또는 서비스 인벤토리에 대한 데이터를 기반으로 동적 광고를 게재할 수 있습니다. 제품 데이터가 있는 새 파일을 매일 또는 원하는 만큼 자주 업로드하거나 [!DNL Google] 또는 [!DNL Microsoft®] 판매자 센터 계정입니다. 이 기능을 사용하여 다음을 수행할 수 있습니다.

* 순서가 지정된 데이터 소스에서 새 캠페인을 빌드합니다.

* 텍스트 및 반응형 검색 광고를 동적으로 업데이트, [!DNL Google Ads] 쇼핑 광고 또는 [!DNL Microsoft® Advertising] 변경 가능한 데이터 요소(예: 가격 또는 수량)에 대해 동적 변수를 사용하여 새 데이터가 처리될 때마다 광고를 봅니다. 데이터를 변경할 때마다 기존 광고가 삭제되고 새 광고가 만들어집니다.

* 지정된 종료 날짜에 따라 특정 수준 이하로 재고가 감소하거나 피드 데이터에서 기존 구성 요소를 생략하는 경우 광고 그룹, 키워드 및 광고를 자동으로 일시 중지하거나 제거합니다.

광고를 설정하려면 변수(자리 표시자)가 포함된 인벤토리 피드 템플릿을 만든 다음 이 변수를 업로드된 파일 또는 의 실제 데이터 열로 대체하십시오 [동기화된 Google 또는 Microsoft® 머천트 센터 계정](/help/search-social-commerce/campaign-management/accounts/merchant-account-manage.md). 변수에는 파일에 설정한 수정자 그룹 또는 파일의 개별 행을 포함하여 데이터 파일의 각 적용 가능한 행에 대해 여러 광고, 키워드, 캠페인 또는 광고 그룹을 생성할 수도 있습니다. 예를 들어, 광고 헤드라인에 수정자 그룹 변수를 사용하고 수정자 그룹에 두 개의 수정자(&quot;저렴한 경우&quot; 및 &quot;할인된 경우&quot;)가 포함된 경우 각 제품에 대해 두 개의 개별 광고(수정자마다 하나씩)가 만들어집니다. 대상 [!DNL Google Ads] 및 [!DNL Microsoft® Advertising] 동적 검색 광고에서 광고 사용자 지정 요소에 대한 값을 포함할 수도 있습니다.

| [!UICONTROL Ad Variation] 템플릿의 섹션 | 검색, 소셜 및 상거래의 수정자 | 피드 콘텐츠 | 결과 광고 |
|----|----|----|----|
| 제목: 하이엔드 구입 \{<i>제품 범주</i>\} &lt;<i>CheapList</i>>.<br><br>설명 1: 대량의 \{<i>제품 이름</i>\}.<br><br>설명 2: 다음에서 사용 가능: \{<i>할인율</i>\}% 할인. | 수정자 그룹 &quot;CheapList&quot;의 값:<br><br>&quot;싸게&quot;<br><br>&quot;할인된 가격으로&quot; | 제품 범주,제품명,할인율<br>전자 제품,iPod,10<br><br>의류,셔츠,15<br><br><b>참고:</b> 쉼표나 탭으로 값을 구분할 수 있습니다. | <u>값싸게 고급 전자제품을 구입하세요.</u><br>태블릿의 엄청난 재고입니다. 10% 할인가로 이용 가능합니다.<br><br><u>고급 전자제품을 할인가에 구입하세요.</u><br>태블릿의 엄청난 재고입니다. 10% 할인가로 이용 가능합니다.<br><br><u>고급 의류를 싸게 구입하세요.</u><br>엄청난 양의 셔츠. 15% 할인가로 이용 가능합니다.<br><br><u>고급 의류를 할인된 가격으로 구입하세요.</u><br>엄청난 양의 셔츠. 15% 할인가로 이용 가능합니다. |

광고를 생성하면 선택적으로 검토한 다음 광고 네트워크에 게시할 수 있습니다.

>[!NOTE]
>스프레드시트 파일을 사용하여 캠페인 데이터를 일괄적으로 생성하거나 편집하려면 &quot;[일괄 시트를 사용하여 캠페인 데이터 관리 기본 정보](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-about.md).&quot;

>[!MORELIKETHIS]
>
>* [재고 피드를 사용한 캠페인 데이터 관리 워크플로우](inventory-feeds-workflow.md)
>* [계정 구성 요소는 언제 재고 피드에서 생성되거나 삭제됩니까?](when-are-components-created-deleted.md)

