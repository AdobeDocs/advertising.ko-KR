---
title: ' [!DNL Naver] 추적 전용 계정 구현'
description: 광고 네트워크에서 직접 구매하는 광고의 성과를 추적하고 보고하고 시각화할 수 있도록  [!DNL Naver] 계정에 대한 추적 캠페인을 설정하는 방법에 대해 알아봅니다.
exl-id: acbaf4f0-eb55-4788-bc84-c3181d635f1d
feature: Search Campaign Management
source-git-commit: e16bc62127a708de8f4deb1eddfa53a14405cbc2
workflow-type: tm+mt
source-wordcount: '687'
ht-degree: 0%

---

# [!DNL Naver] 추적 전용 계정 구현

*[!DNL Naver]개의 계정만*

광고 네트워크에서 직접 구매하는 광고의 성과를 추적, 보고 및 시각화할 수 있도록 [!DNL Naver] 계정에 대한 추적 캠페인을 만들 수 있습니다. Search, Social 및 Commerce은 데이터를 광고 네트워크와 동기화하지 않고 추적을 자동으로 업로드하며 계정에 대한 입찰도 하지 않습니다.

추적 캠페인은 기존 캠페인, 광고 그룹 및 키워드를 복제합니다. 검색, 소셜 및 Commerce에서 계정 구조를 만들고 광고 네트워크 내의 원래 캠페인에 추적을 추가한 후에는 키워드 또는 광고에 대한 일일 네트워크 트래픽 지표를 업로드할 수 있습니다. 그런 다음 Search, Social 및 Commerce은 전환을 광고와 키워드로 연결할 수 있습니다.

모든 캠페인과 개별 캠페인, 광고 그룹 또는 키워드/광고에 대한 성능 지표를 추적할 수 있습니다. 다른 광고 네트워크에 대한 데이터와 함께 가장 기본, 고급 및 지원 보고서에 이러한 보고서에 대한 정보를 포함할 수도 있습니다. 지표를 Adobe Analytics으로 내보내는 기능은 지원되지 않지만, Search, Social 및 Commerce은 추적 중인 [지표 [!DNL Analytics]](/help/integrations/analytics/analytics-data-in-advertising.md)를 Search, Social 및 Commerce에 동기화할 수 있습니다.

>[!NOTE]
>
>최적화를 위해 포트폴리오에 추적 캠페인을 추가할 수 없습니다.

1. 검색, 소셜 및 Commerce에서 추적 캠페인 만들기:

   1. [더미 네트워크 계정 세부 정보](/help/search-social-commerce/campaign-management/accounts/ad-network-account-manage.md)를 만듭니다. 단일 광고 네트워크 내에 여러 개의 계정이 있는 경우 [!UICONTROL Accounts] 보기에서 하나의 계정으로 통합합니다.

      [!DNL Naver]은(는) 추적 매개 변수를 광고 네트워크에 업로드하는 데 API를 지원하지 않습니다. 그러나 일괄 시트를 사용하여 추적 매개 변수를 생성하고 광고 네트워크 내에 수동으로 추가할 수 있습니다(단계 2에 따라). 추적 매개 변수를 생성하려면 &quot;[!UICONTROL EF Redirect]&quot; 추적 메서드를 사용해야 합니다. 원하는 추가 매개변수를 선택적으로 추가할 수 있습니다.

      Search, Social 및 Commerce은 계정의 일괄 시트 내에서 생성되는 모든 추적 URL에 `ev_cl={ef_uniqueid}` 매개 변수를 자동으로 포함합니다. 이 고유 ID는 캠페인 데이터와 임의 비용을 일치시키고 업로드한 데이터를 클릭하는 데 사용됩니다.

   1. 추적할 캠페인을 설정합니다.

      1. 광고 네트워크 내에서 Search, Social 및 Commerce에서 계정을 추적하려는 모든 엔티티와 필요한 상위 엔티티를 포함하는 일괄 시트 파일을 만듭니다.

         상위 캠페인 및 광고 그룹을 포함하여 키워드에 대한 데이터를 포함할 수 있습니다.

      1. 필요한 경우 일괄 시트 파일을 편집하여 검색, 소셜 및 Commerce [계정에 필요한 일괄 시트 형식 [!DNL Naver] 계정](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-naver.md)을 따르도록 하십시오.

      1. 검색, 소셜 및 Commerce에서 [일괄 시트 파일을 업로드](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-upload.md)합니다.

         >[!NOTE]
         >
         >참고: Search, Social 및 Commerce은 데이터를 광고 네트워크 계정에 게시하지 않습니다.

1. 캠페인에 대한 추적을 설정합니다.

   1. 검색, 소셜 및 Commerce에서 &quot;[!UICONTROL Generate Tracking URLs]&quot;에 대한 옵션을 사용하여 [새 일괄 시트 파일을 다운로드](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-download.md)하십시오.

   &quot;[!UICONTROL Generate Tracking URLs]&quot; 옵션을 사용하면 각 키워드에 대한 [!UICONTROL Destination URL] 필드가 [!UICONTROL Base URL] 값 접두사가 있는 Search, Social 및 Commerce 추적 코드로 채워집니다.

   다음은 추적이 있는 대상 URL의 예입니다.

   ```http://pixel.everesttech.net/1234/cq?ev_sid=87&ev_cl=258e27dcec70156a667f2229020e488&url=http%3A//www.example.com```

   1. 다운로드한 일괄 시트 파일의 [!UICONTROL Destination URL] 값을 네트워크의 관련 키워드 설정에 복사합니다.

      광고 네트워크의 편집기 내에서 네트워크에 파일을 업로드하여 관련 엔티티에 URL을 추가할 수 있습니다. 이 경우 네트워크의 데이터 요구 사항에 따라 일부 열을 제거해야 할 수 있습니다. 그렇지 않으면 네트워크에서 수동으로 URL을 입력해야 합니다.

1. 추적 중인 키워드 또는 광고 그룹 수준의 브랜드 광고에 대해 광고 네트워크에서 매일 집계되는 클릭 및 비용 데이터를 정기적으로 다운로드한 다음 [클릭 및 비용 데이터를 업로드](/help/search-social-commerce/tools/metrics-upload-tracking-campaigns/naver-tracking-campaigns-upload-metrics.md)하여 [필요한 형식](/help/search-social-commerce/tools/metrics-upload-tracking-campaigns/naver-tracking-campaigns-data-requirements.md)의 검색, 소셜 및 Commerce으로 업로드합니다.

   전체 계정 계층 구조 및 포함하려는 지표를 포함합니다. Search, Social 및 Commerce은 업로드한 데이터를 기존 캠페인의 데이터와 일치시킵니다.

1. (선택 사항) 웹 페이지에서 Adobe Advertising 전환 추적 서비스 태그를 사용하여 광고 네트워크에서 추적되지 않는 전환을 추적하는 경우, 일별로 집계된 전환 데이터가 포함된 피드 파일을 전송하여 추적 캠페인에 추가합니다.

   자세한 내용은 Adobe 계정 팀에 문의하십시오.

업로드된 모든 추적 데이터는 [!UICONTROL Accounts], [!UICONTROL Campaigns], [!UICONTROL Ad Groups] 및 [!UICONTROL Keywords] 보기 내에서 [!UICONTROL Search] > [!UICONTROL Campaigns] > [!UICONTROL Campaigns]에서 사용할 수 있습니다. [!UICONTROL Insights & Reports] 보기의 보고서에도 사용할 수 있습니다.

>[!MORELIKETHIS]
>
>* [부록 - [!DNL Naver] 계정](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-data-formats/bulksheet-data-naver.md)에 필요한 일괄 시트 데이터
>* [추적 전용 계정에 대한 트래픽 및 전환 지표 업로드 [!DNL Naver] 2&rbrace;](/help/search-social-commerce/tools/metrics-upload-tracking-campaigns/naver-tracking-campaigns-upload-metrics.md)
>* [추적 전용 계정에 대한 지표 데이터 요구 사항 [!DNL Naver] 2&rbrace;](/help/search-social-commerce/tools/metrics-upload-tracking-campaigns/naver-tracking-campaigns-data-requirements.md)
>*  [!DNL Naver][&#128279;](/help/search-social-commerce/tracking/formats-click-tracking-naver.md)에 대한 클릭 추적 형식
