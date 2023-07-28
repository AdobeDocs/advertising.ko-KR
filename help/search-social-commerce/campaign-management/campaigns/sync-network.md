---
title: 수동으로 광고 네트워크 데이터 동기화
description: 지원되는 광고 네트워크에 대한 캠페인 구조 및 캠페인 엔티티의 동기화를 수동으로 트리거하는 방법에 대해 알아봅니다.
exl-id: da437f37-800a-4c56-b5c1-7c985ddd45c8
feature: Search Campaign Management
source-git-commit: 052574217d7ddafb8895c74094da5997b5ff83db
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# 수동으로 광고 네트워크 데이터 동기화

*[!DNL Baidu], [!DNL Google Ads], [!DNL Microsoft® Advertising] (이전 [!DNL Bing Ads]), [!DNL Yahoo! Japan Ads], 및 [!DNL Yandex] 계정만*

동기화는 검색, 소셜 및 상거래가 각 광고주의 광고 네트워크 계정에 대한 업데이트된 정보를 수집하는 프로세스입니다. [지원되는 광고 네트워크](/help/search-social-commerce/introduction/supported-inventory.md). 이 데이터에는 검색, 소셜 및 상거래에서 관리되거나 보고되는 대부분의 속성을 포함하여 광고주의 캠페인 구조 및 캠페인 엔티티가 포함됩니다. 여기에는 클릭 데이터나 검색, 소셜 및 커머스 외부에서 입력한 입찰 및 입찰 수정자가 포함되지 않으며, 이는 별도로 수집됩니다.

Search, Social 및 Commerce는 하루에 한 번 광고 네트워크 계정과 자동으로 동기화(동기화)되며, 광고 네트워크 중 하나에서 새 캠페인이 검색될 때마다 동기화됩니다. 또한 검색, 소셜 및 상거래 내에서 수행한 캠페인 데이터에 대한 모든 변경 사항을 광고 네트워크로 즉시 전송합니다.

지정된 계정 또는 특정 활성 및 일시 중지된 캠페인에서 모든 활성 및 일시 중지된 캠페인의 동기화를 수동으로 요청할 수 있습니다. 이 작업은 광고 네트워크에서 새로 추가되거나 변경된 엔티티를 수집합니다.

&quot;가 있는 캠페인의 경우[!UICONTROL Auto Upload]&quot; 옵션을 사용하면 동기화 작업은 추적 템플릿 또는 대상 URL에서 누락되었거나 변경되어야 하는 추적 코드를 생성하고 게시합니다. URL은 계정 설정 또는 캠페인에 대한 추적 설정의 매개 변수에 따라 생성됩니다. 관련 항목에 대한 추적 URL이 있는 경우, 새 URL이 필요하지 않으면 다시 생성되지 않습니다(예: 키워드 일치 유형, 크리에이티브 텍스트 또는 계정의 추적 매개 변수가 변경된 경우).

>[!NOTE]
>
>언제든지 [일괄 시트 만들기](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-download.md), 일괄 시트가 생성되기 전에 광고 네트워크와 선택적으로 동기화할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Search]>[!UICONTROL Campaigns]**. 하위 메뉴에서 다음 중 하나를 선택합니다 **[!UICONTROL Accounts]** 특정 계정의 모든 캠페인을 동기화하거나 **[!UICONTROL Campaigns]** 특정 캠페인을 동기화할 수 있습니다.

1. (선택 사항) 특정 계정 또는 캠페인을 포함하도록 목록을 필터링합니다.

1. 동기화할 각 계정 또는 캠페인 옆에 있는 확인란을 선택합니다. 한 번에 최대 50개의 캠페인을 동기화할 수 있습니다. 한 번에 5개 이상의 계정을 동기화하는 경우 작업은 최대 5개의 계정으로 분할됩니다.

1. 클릭 **![자세히](/help/search-social-commerce/assets/more.png "자세히")** 도구 모음에서 를 선택하고 **[!UICONTROL Sync]**.

에서 동기화 작업의 상태를 추적할 수 있습니다. [!UICONTROL Workspace] 보기. 작업을 표시하는 데 한 시간 이상 걸릴 수 있습니다.

>[!MORELIKETHIS]
>
>* [일괄 시트 파일 다운로드/만들기](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-download.md)
