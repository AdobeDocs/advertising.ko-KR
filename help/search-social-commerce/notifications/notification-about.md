---
title: 알림 기본 정보
description: 다양한 유형 및 범주를 포함하여 알림에 대해 알아봅니다.
exl-id: 79495e1c-72ce-476f-83df-c4d95391f51c
feature: Search Notifications
source-git-commit: 955f19647d49c31f70b8ec574734b44a9b490d52
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# 알림 기본 정보

*Beta 기능*

다양한 유형의 경고를 구독하거나 구독 취소하도록 알림 설정을 구성할 수 있습니다. 다음 방법 중 하나로 알림을 볼 수 있습니다.

* 다음에서 [!UICONTROL Notifications] 패널: 의 기본 메뉴에서 사용할 수 있습니다. ![알림](/help/search-social-commerce/assets/notifications-panel.png "알림").

* 출처: [!UICONTROL Insights & Reports] > [!UICONTROL Notification Center Beta].

* 다음에서: [!UICONTROL Notification Center] 웹 애플리케이션: [!UICONTROL Notification Center] 검색, 소셜 및 커머스 외부의 별도의 창에서.

  애플리케이션이 일반 브라우저 버전보다 빠르게 로드되고 자동으로 업데이트됩니다. 응용 프로그램을 설치하고 브라우저의 앱 관리자를 사용하여 관리할 수 있습니다.

* 을(를) 푸시 알림에서 브라우저로 설정합니다.

  푸시 알림을 활성화하면 브라우저의 알림 규칙에 따라 표시됩니다.

알림을 보고, 알림을 읽음 또는 읽지 않음으로 표시하고, 알림을 삭제할 수 있습니다.

## 알림 유형

* **[!UICONTROL Notices]**: 릴리스, 다운타임 및 기타 변경 관리 공지.

* **[!UICONTROL Recommendations]**: 성능 향상, 모범 사례 구현 등을 위해 확인된 영업 기회입니다.

* **[!UICONTROL Warnings]**: 주의가 필요하지만 최적화 또는 관리에 중요하지 않은 문제입니다.

* **[!UICONTROL Issues]**: 즉각적인 주의가 필요한 심각한 문제. 계정 인증 오류 알림이 포함됩니다.

## 알림 범주

* [!UICONTROL Campaign Management]

   * **[!UICONTROL Bulksheets]**: 다음에 대한 알림: [일괄 시트 작업](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-about.md) 이(가) 완료되었거나 실패했습니다.

   * **[!UICONTROL Manager Account Missing]**: 검색, 소셜 및 상거래에 대한 자격 증명이 누락되었다는 알림 [광고 네트워크 관리자 계정](/help/search-social-commerce/admin/manager-accounts.md)중요 기능을 올바르게 설정하는 데 필요합니다.

   * **[!UICONTROL UI Actions]**: 백그라운드에서 수행되는 작업이 완료되었거나 실패했음을 알립니다. 작업 유형은 다음과 같습니다 [일괄 시트 작업](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-about.md), 데이터 테이블 내에서 또는 도구 모음, 엔티티 할당 작업 또는 사용자 인터페이스 내에서 기타 작업(예: 광고 네트워크와의 동기화, 행 붙여넣기 또는 엔티티 이름 바꾸기)을 사용하여 작업을 일괄 편집합니다. 엔티티 할당에는 할당 또는 할당 취소가 포함됩니다. [레이블 분류 값](/help/search-social-commerce/campaign-management/label-classifications/classification-about.md) 모든 엔티티에 대해, 포트폴리오에 캠페인을 할당하고, 포트폴리오에 제한 사항을 할당하거나 할당 취소합니다.<!--Link "constraint" to constraint-about.md if that file is ever public -->

   * [!UICONTROL Data Upload]

      * **[!UICONTROL Direct File Upload]**: 닫힌 베타에 사용됩니다

      * **[!UICONTROL File Upload to Cloud Storage]**: 닫힌 베타에 사용됩니다

   * [!UICONTROL Network Errors]

      * **[!UICONTROL Account Auth Error]**: 검색, 소셜 및 상거래에 액세스할 수 없는 알림 [광고 네트워크 계정](/help/search-social-commerce/campaign-management/accounts/ad-network-account-about.md) 잘못된 자격 증명 또는 유효하지 않거나 만료된 인증 토큰으로 인해.

      * **[!UICONTROL Account Missing]**: 검색, 소셜 및 상거래에 대한 자격 증명이 누락되었다는 알림 [광고 네트워크 계정](/help/search-social-commerce/campaign-management/accounts/ad-network-account-about.md).

      * **[!UICONTROL Manager Account Auth Error]**: Search, Social 및 Commerce가 와 동기화할 수 없는 알림입니다. [광고 네트워크 관리자 계정](/help/search-social-commerce/admin/manager-accounts.md) 잘못된 자격 증명 또는 유효하지 않거나 만료된 인증 토큰으로 인해.

  <!--
  * [!UICONTROL Setup Errors]
  
    * **[!UICONTROL Adobe Analytics Tracking Setup Error]**: : Notifications that the [!UICONTROL Landing Page Suffix] value is incorrect, missing, or contains an incorrect [AMO ID template](/help/integrations/analytics/ids.md#amo-id-formats); or it's overridden at a lower level by an incorrect value.
    
    * **[!UICONTROL Manager Account Missing]**: Notifications that Search, Social, & Commerce is missing the credentials for an [ad network manager account](/help/search-social-commerce/admin/manager-accounts.md), which are required for the correct setup of critical functions.
  -->

* [!UICONTROL Insights & Reports]

   * **[!UICONTROL Advertising Insights]**: 다음과 같은 알림 [an [!DNL Advertising Insight]](/help/search-social-commerce/advertising-insights/insight-about.md) 이(가) 완료되었거나 실패했습니다.

   * **[!UICONTROL Custom Alerts]**: 다음과 같은 알림 [경고 인스턴스](/help/search-social-commerce/alerts/alert-about.md) 경고 템플릿에 대해 트리거되었습니다.

   * **[!UICONTROL Reports]**: 다음에 대한 알림: [사용자 지정 또는 예약된 보고서](/help/search-social-commerce/reports/report-about.md) 이(가) 완료되었거나 실패했습니다.

   * **[!UICONTROL Spreadsheet Feeds]**: 다음에 대한 알림: [스프레드시트 피드](/help/search-social-commerce/reports/automation/spreadsheet-feeds/spreadsheet-feed-about.md) 이(가) 완료되었거나 실패했습니다.

<!--
* [!UICONTROL Optimization]

  * **[!UICONTROL Accuracy]**: 

-->

<!--
* [!UICONTROL Portfolio Management]

  * **[!UICONTROL Simulation Report]**: 

-->

<!--
* [!UICONTROL System]

  * **[!UICONTROL Change Management]**: 

-->

>[!MORELIKETHIS]
>
>* [알림 보기](notification-view.md)
>* [알림을 읽음 또는 읽지 않음으로 표시](notification-mark-read-unread.md)
>* [알림 삭제](notification-delete.md)
>* [알림 설정 편집](notification-edit.md)
>* [푸시 알림 활성화 및 비활성화 위치 [!UICONTROL Notification Center]](notifications-push-enable-disable.md)
>* [설치 및 제거 [!UICONTROL Notification Center] 웹 애플리케이션](notification-app-install-uninstall.md)
