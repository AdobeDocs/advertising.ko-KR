---
title: (새 UI) 알림 관리
description: 푸시 알림 및 알림 센터 웹 애플리케이션을 비롯한 검색, 소셜 및 Commerce 알림을 보고, 구성하고, 관리하는 방법을 알아봅니다.
feature: Search Notifications
source-git-commit: 000ed245b2ea3381e4ca8fcbdd2d6075d50f4b09
workflow-type: tm+mt
source-wordcount: '1710'
ht-degree: 0%

---

# (새 UI) 알림 관리

*Beta 기능*

다양한 유형의 경고를 구독하거나 구독 취소하도록 알림 설정을 구성할 수 있습니다. 다음 방법 중 하나로 알림을 볼 수 있습니다.

* ![알림](/help/search-social-commerce/assets/notifications.png "알림")의 오른쪽 상단에서 사용할 수 있는 [!UICONTROL Notifications] 패널에서. 패널에서 목록을 필터링하거나 알림 설정을 편집하거나 [!UICONTROL Notification Center]을(를) 열 수 있습니다.

* 검색, 소셜 및 Commerce 외부의 별도의 창에서 열리는 [!UICONTROL Notification Center]에서. [!UICONTROL Notifications] 패널에서 [!UICONTROL Notification Center]을(를) 열려면 **[!UICONTROL View All]**&#x200B;을(를) 클릭합니다.

* Search, Social 및 Commerce 외부의 별도의 창에서 [!UICONTROL Notification Center]을(를) 여는 [!UICONTROL Notification Center] 웹 응용 프로그램에서

  애플리케이션이 일반 브라우저 버전보다 빠르게 로드되고 자동으로 업데이트됩니다. 응용 프로그램을 설치하고 브라우저의 앱 관리자를 사용하여 관리할 수 있습니다.

* 을(를) 푸시 알림에서 브라우저로 설정합니다.

  푸시 알림을 활성화하면 브라우저의 알림 규칙에 따라 표시됩니다.

알림을 보고, 알림을 읽음 또는 읽지 않음으로 표시하고, 알림을 삭제할 수 있습니다.

## 알림 유형

* **[!UICONTROL Notices]**: 릴리스, 가동 중지 시간 및 기타 변경 관리 알림.

* **[!UICONTROL Recommendations]**: 성능 향상, 모범 사례 구현 등을 위해 확인된 영업 기회입니다.

* **[!UICONTROL Warnings]**: 주의가 필요하지만 최적화 또는 관리에 중요하지 않은 문제입니다.

* **[!UICONTROL Issues]**: 즉각적인 주의가 필요한 심각한 문제입니다. 계정 인증 오류 알림이 포함됩니다.

## 알림 범주

<!-- Update info, and update links to files for new UI once they're available-->

* [!UICONTROL Campaign Management]

   * **[!UICONTROL Bulksheets]**: [일괄 시트 작업](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-about.md)이 완료되었거나 실패했다는 알림입니다.<!-- Update link once file for new UI available-->

   * **[!UICONTROL Manager Account Missing]**: Search, Social 및 Commerce에 [ad 네트워크 관리자 계정](/help/search-social-commerce/admin/manager-accounts.md)에 대한 자격 증명이 누락되었다는 알림으로, 중요한 기능을 올바르게 설정하는 데 필요합니다.<!-- Moving to Campaign Management > Setup Errors at some point -->

   * **[!UICONTROL UI Actions]**: 백그라운드에서 수행되는 작업이 완료되었거나 실패했음을 알립니다. 작업 유형에는 [일괄 시트 작업](/help/search-social-commerce/campaign-management/bulksheets/bulksheet-about.md)<!-- Update link once file for new UI available-->, 데이터 테이블 내의 일괄 편집 작업 또는 도구 모음 사용, 엔티티 할당 작업 또는 사용자 인터페이스 내의 기타 작업(예: 광고 네트워크와의 동기화, 행 붙여넣기 또는 엔티티 이름 바꾸기)이 포함됩니다. 엔터티 할당에는 엔터티에 [레이블 분류 값](/help/search-social-commerce/new-ui/reports/label-classifications-manage.md)을(를) 할당하거나 할당 해제하는 것, 포트폴리오에 캠페인을 할당하는 것, 포트폴리오에 제약 조건을 할당하거나 할당 해제하는 것이 포함됩니다.

   * [!UICONTROL Data Upload]

      * **[!UICONTROL Direct File Upload]**: [수동 계정 데이터 업로드](/help/search-social-commerce/new-ui/set-up/accounts/data-upload-accounts/upload-account-data.md)를 통해 계정 데이터 파일이 업로드되었거나 계정 데이터 업로드가 실패했음을 알립니다. <!-- Verify description-->

      * **[!UICONTROL File Upload to Cloud Storage]**: [계정 데이터를  [!DNL Amazon] [!DNL S3] 버킷에 업로드](/help/search-social-commerce/new-ui/set-up/accounts/data-upload-accounts/upload-account-data.md)하여 계정 데이터 파일이 업로드되었거나 계정 데이터 업로드가 실패했음을 알립니다. <!-- Verify description-->

   * [!UICONTROL Network Errors]

      * **[!UICONTROL Account Auth Error]**: 자격 증명이 잘못되었거나 인증 토큰이 잘못되었거나 만료되어 Search, Social 및 Commerce에서 [ad 네트워크 계정](/help/search-social-commerce/new-ui/set-up/accounts/api-accounts/api-account-manage.md)에 액세스할 수 없다는 알림입니다.

      * **[!UICONTROL Account Missing]**: Search, Social 및 Commerce에 [광고 네트워크 계정](/help/search-social-commerce/new-ui/set-up/accounts/api-accounts/api-account-manage.md)에 대한 자격 증명이 없다는 알림입니다.

      * **[!UICONTROL Manager Account Auth Error]**: 자격 증명이 잘못되었거나 인증 토큰이 잘못되었거나 만료되어 Search, Social 및 Commerce이 [ad 네트워크 관리자 계정](/help/search-social-commerce/admin/manager-accounts.md)과(와) 동기화할 수 없다는 알림입니다.<!-- Update link once file for new UI available-->

* [!UICONTROL Insights & Reports]

   * **[!UICONTROL Advertising Insights]**: [an [!DNL Advertising Insight]](/help/search-social-commerce/advertising-insights/insight-about.md)에 대한 알림이 완료되었거나 실패했습니다.

   * **[!UICONTROL Custom Alerts]**: 경고 템플릿에 대해 [경고 인스턴스](/help/search-social-commerce/new-ui/alerts-manage.md)가 트리거된 알림입니다.

   * **[!UICONTROL Spreadsheet Feeds]**: [스프레드시트 피드](/help/search-social-commerce/new-ui/reports/spreadsheet-feeds-manage.md)가 완료되었거나 실패했다는 알림입니다.

   * [!UICONTROL Reports]

      * **[!UICONTROL Grid Reports]**: 특정 보기의 데이터 보기 보고서(예: [!UICONTROL Camapigns] 보기의 데이터 테이블 내용)가 완료되었거나 실패했음을 알립니다.

      * **[!UICONTROL Reports]**: [사용자 지정 또는 예약된 보고서](/help/search-social-commerce/new-ui/reports/management/report-manage.md)가 완료되었거나 실패했다는 알림입니다.

   * [!UICONTROL Portfolio Management]

      * **[!UICONTROL Intraday Optimization]**: 실시간 최적화를 사용하지 않도록 설정할 때의 알림입니다.

      * **[!UICONTROL Simulation Report]**: [시뮬레이션 작업](/help/search-social-commerce/new-ui/plan/simulations/simulation-about.md)에 대한 알림입니다.

      * [!UICONTROL Objective & Conversion Configuration]

         * **[!UICONTROL Auto Assign Campaign Conversion Goal - Advertiser Level]**: 캠페인 전환 목표의 자동 할당 성공 및 실패에 대한 광고주 수준의 알림입니다.

         * **[!UICONTROL Auto Assign Campaign Conversion Goal - Portfolio Level]**: 캠페인 전환 목표의 자동 할당 성공 및 실패에 대한 포트폴리오 수준의 알림입니다.

      * [!UICONTROL Portfolios]

         * **[!UICONTROL Portfolio Bulksheet Diagnostic Report]**: 일괄 시트를 통한 [포트폴리오 일괄 편집 작업에 대한 알림](/help/search-social-commerce/new-ui/manage/portfolios/portfolio-bulksheets.md).

         * **[!UICONTROL Portfolio Settings]**: [포트폴리오 설정 변경](/help/search-social-commerce/new-ui/manage/portfolios/portfolio-settings.md)에 대한 알림입니다.

<!--

In Campaign Management:

  * [!UICONTROL Setup Errors]

    * **[!UICONTROL Adobe Analytics Tracking Setup Error]**: Notifications that an account-level landing page suffix is incorrect due to missing or incorrect [AMO ID (`s_kwcid` parameter)](/help/integrations/analytics/ids.md).
  
    * **[!UICONTROL Manager Account Missing]**: Notifications that Search, Social, & Commerce is missing the credentials for an [ad network manager account](/help/search-social-commerce/admin/manager-accounts.md), which are required for the correct setup of critical functions.

-->

<!--
* [!UICONTROL Optimization]

  * **[!UICONTROL Accuracy]**: Notifications when a portfolio's model accuracy deviates [by how much?] from expectations.
-->


## 사용 가능한 작업

* [알림 보기](#notification-view)

* [알림 설정 편집](#notification-edit)

* [알림을 읽음 또는 읽지 않음으로 표시](#notification-mark-read-unread)

* [알림 삭제](#notification-delete)

* [푸시 알림 활성화 및 비활성화](#notification-push-enable-disable)

* [[!UICONTROL Notification Center] 웹 응용 프로그램 설치 및 제거](#notification-app-install-uninstall)

## 알림 보기 {#notification-view}

계정 인증 오류, 트리거된 사용자 지정 경고 및 생성된 [!UICONTROL Advertising Insights]에 대한 [알림을 구독](#notification-edit)할 때 [!UICONTROL Notifications] 패널 또는 [!UICONTROL Notification Center]에서 알림을 볼 수 있습니다.

### [!UICONTROL Notifications] 패널 내에서 알림 보기

1. 페이지의 오른쪽 상단에서 ![알림](/help/search-social-commerce/assets/notifications.png "알림")을 클릭합니다.

1. (선택 사항) 다음 중 하나를 수행합니다.

   * 통지의 상세내역을 조회하려면 통지 이름을 누릅니다.

     일부 알림에서 [!UICONTROL Action Recommended] 섹션에는 영향을 받거나 책임 있는 엔터티의 필터링된 보기를 여는 링크가 포함될 수 있습니다.

   * 알림을 *읽음* 또는 *읽지 않음*(으)로 표시하려면 경고 이름 위에 커서를 놓고 ![읽음 또는 읽지 않음으로 표시](/help/search-social-commerce/assets/notifications-read-unread.png "읽음 또는 읽지 않음으로 표시")를 클릭합니다.

     *읽음*(으)로 표시된 알림이 밝은 색의 텍스트로 표시되지만 삭제할 때까지 사용 가능합니다.

     ![읽은 알림 및 읽지 않은 알림](/help/search-social-commerce/assets/notifications-read-vs-unread.png "읽은 알림 및 읽지 않은 알림")

   * 알림 유형에 대한 구독 환경 설정을 변경하려면 알림 옆에 있는 ![설정](/help/search-social-commerce/assets/settings-nc.png "설정")을 클릭하고 설정을 변경한 다음 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

   * 알림을 삭제하려면 알림 옆에 있는 ![삭제](/help/search-social-commerce/assets/delete.png "삭제")를 클릭합니다.

   * [!UICONTROL Notification Center]을(를) 열려면 **[!UICONTROL View All]**&#x200B;을(를) 클릭합니다.

### [!UICONTROL Notification Center] 내의 알림 보기

1. 페이지의 오른쪽 상단에서 ![알림](/help/search-social-commerce/assets/notifications.png "알림")을 클릭합니다.

1. **[!UICONTROL View All]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 유형별로 알림을 필터링하려면 *[!UICONTROL Notices], [!UICONTROL Recommendations], [!UICONTROL Warnings] 또는[!UICONTROL Issues]*&#x200B;을(를) 클릭합니다.

1. (선택 사항) 다음 중 하나를 수행합니다.

   * 통지의 상세내역을 조회하려면 통지 이름을 누릅니다.

     일부 알림에서 [!UICONTROL Action Recommended] 섹션에는 영향을 받거나 책임 있는 엔터티의 필터링된 보기를 여는 링크가 포함될 수 있습니다.

   * 알림을 *읽음* 또는 *읽지 않음*(으)로 표시하려면 경고 이름 위에 커서를 놓고 ![읽음 또는 읽지 않음으로 표시](/help/search-social-commerce/assets/notifications-read-unread.png "읽음 또는 읽지 않음으로 표시")를 클릭합니다.

     *읽음*(으)로 표시된 알림이 밝은 색의 텍스트로 표시되지만 삭제할 때까지 사용 가능합니다.

   * 알림 유형에 대한 구독 환경 설정을 변경하려면 알림 옆에 있는 ![설정](/help/search-social-commerce/assets/settings-nc.png "설정")을 클릭하고 설정을 변경한 다음 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

   * 알림을 삭제하려면 알림 옆에 있는 ![삭제](/help/search-social-commerce/assets/delete.png "삭제")를 클릭합니다.

## 알림 설정 편집 {#notification-edit}

계정 인증 오류, 트리거된 모든 사용자 지정 경고 및 생성한 [!UICONTROL Advertising Insights] 완료에 대한 전자 메일 및 웹 알림을 선택적으로 구독하거나 구독 취소할 수 있습니다.

1. 다음 방법 중 하나로 알림 설정을 엽니다.

   * 페이지의 오른쪽 상단에서 ![알림](/help/search-social-commerce/assets/notifications.png "알림")을 클릭하여 [!UICONTROL Notifications] 패널을 엽니다. 오른쪽 상단에서 ![설정](/help/search-social-commerce/assets/settings-nc.png "설정")을(를) 클릭합니다.

   * 페이지의 오른쪽 상단에서 ![알림](/help/search-social-commerce/assets/notifications.png "알림")을 클릭하고 **[!UICONTROL View All]**&#x200B;을(를) 클릭하여 [!UICONTROL Notification Center]을(를) 연 다음 왼쪽 메뉴에서 ![설정](/help/search-social-commerce/assets/settings-nc.png "설정")을(를) 클릭합니다.

1. 위에 나열된 알림 범주에 대한 설정을 변경합니다.

   * 알림을 구독하거나 구독을 취소하려면 [!UICONTROL Subscribe] 열에서 슬라이더를 이동합니다.

      * 모든 알림 유형에서 가입을 해지하려면 슬라이더를 왼쪽(비활성화)으로 이동합니다.

      * 하나 이상의 알림 유형에 가입하려면 슬라이더를 오른쪽으로 이동합니다(활성화됨).

   * ([!UICONTROL Subscribe]을(를) 사용하도록 설정한 경우) 전자 메일 알림을 구독하려면 **[!UICONTROL Email]** 열의 확인란을 선택하십시오.

   * [!UICONTROL Subscribe]이(가) 비활성화된 경우 검색, 소셜 및 Commerce 내에서 웹 알림을 구독하고 브라우저에 활성화된 경우 푸시 알림을 구독하려면 **[!UICONTROL Web]** 열의 확인란을 선택하십시오.

     웹 알림은 브라우저에 [푸시 알림을 활성화](#notification-push-enable-disable)하는 경우에만 전달됩니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 알림을 읽음 또는 읽지 않음으로 표시 {#notification-mark-read-unread}

알림을 *읽음* 또는 *읽지 않음*&#x200B;으로 표시하면 각 페이지 맨 위에 있는 [!UICONTROL Notifications] 링크에 표시된 읽지 않은 알림 수가 변경됩니다(예: ![읽지 않은 알림 카운터가 있는 알림 아이콘](/help/search-social-commerce/assets/notifications-unread.png "읽지 않은 알림 카운터가 있는 알림 아이콘")).

*읽음*(으)로 표시된 알림이 밝은 색의 텍스트로 표시되지만 삭제할 때까지 사용 가능합니다.

![읽은 알림 및 읽지 않은 알림](/help/search-social-commerce/assets/notifications-read-vs-unread.png "읽은 알림 및 읽지 않은 알림")

1. [알림 패널 또는 알림 센터를 엽니다](#notification-view).

1. 경고 이름 위에 커서를 놓고 ![읽음 또는 읽지 않음으로 표시](/help/search-social-commerce/assets/notifications-read-unread.png "읽음 또는 읽지 않음으로 표시")를 클릭합니다.

## 알림 삭제 {#notification-delete}

### [!UICONTROL Notifications] 패널 내에서 알림 삭제

1. 페이지의 오른쪽 상단에서 ![알림](/help/search-social-commerce/assets/notifications.png "알림")을 클릭합니다.

1. 알림 옆에 있는 ![삭제](/help/search-social-commerce/assets/delete.png "삭제")를 클릭합니다.

### [!UICONTROL Notification Center] 내에서 알림 삭제

1. 페이지의 오른쪽 상단에서 ![알림](/help/search-social-commerce/assets/notifications.png "알림")을 클릭합니다.

1. **[!UICONTROL View All]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 유형별로 알림을 필터링하려면 *[!UICONTROL Notices]*, *[!UICONTROL Recommendations]*, *[!UICONTROL Warnings]* 또는 *[!UICONTROL Issues]*&#x200B;을(를) 클릭합니다.

1. 알림 옆에 있는 ![삭제](/help/search-social-commerce/assets/delete.png "삭제")를 클릭합니다.

## 푸시 알림 활성화 및 비활성화 {#notification-push-enable-disable}

브라우저의 알림 규칙에 따라 표시되는 검색, 소셜 및 Commerce 내에서 알림을 활성화할 수 있습니다. [!DNL Microsoft Windows]을(를) 사용하는 장치에서 화면 오른쪽 아래(시스템 트레이)에 알림이 표시됩니다. [!DNL Apple Mac]개 장치에서 알림이 오른쪽 메뉴에 표시됩니다.

푸시 알림은 다음 브라우저에서 사용할 수 있습니다.

* [!DNL Google Chrome] 40 이상

* [!DNL Microsoft Edge] 17 이상

* [!DNL Mozilla Firefox] 44 이상

브라우저의 표준 절차에 따라 푸시 알림을 비활성화할 수 있습니다.

### 푸시 알림 활성화

1. 페이지의 오른쪽 상단에서 ![알림](/help/search-social-commerce/assets/notifications.png "알림")을 클릭합니다.

1. **[!UICONTROL View All]**&#x200B;을(를) 클릭합니다.

1. 오른쪽 하단에서 ![푸시 알림 사용](/help/search-social-commerce/assets/notifications-push.png "푸시 알림 사용")을 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Enable]**&#x200B;을(를) 클릭합니다.

1. `https://alert-center-ui-na.efrontier.com`에서 [!UICONTROL Notification Center]의 알림을 허용하도록 브라우저를 구성하십시오.

   기본 알림 설정은 브라우저마다 다르며, a) [!UICONTROL Notification Center]에서 알림을 허용하는 옵션이 자동으로 표시되거나 b) 알림 설정을 수동으로 관리해야 할 수 있습니다. 예를 들어 [!DNL Microsoft Edge]에서 브라우저 도구 모음에서 [!UICONTROL Notification Center]의 알림을 허용할 수 있습니다. 브라우저 도움말의 지침을 참조하십시오.

   ![Microsoft Edge에서 알림 설정을 관리할 위치](/help/search-social-commerce/assets/notifications-blocked-dialog.png "Microsoft Edge에서 알림 설정을 관리할 위치")

1. [알림 설정](#notification-edit)에서 푸시할 경고 유형에 대해 [!UICONTROL Web] 알림을 사용하도록 설정하십시오.

### 푸시 알림 비활성화

브라우저의 알림 관리자 내에서 `https://alert-center-ui-na.efrontier.com`에서 알림을 제거합니다. 예를 들어 [!DNL Google Chrome]에서 `chrome://settings/content/notifications`의 지정된 사이트에서 알림을 제거하거나 차단할 수 있습니다.

브라우저 도움말의 지침을 참조하십시오.

## [!UICONTROL Notification Center] 웹 응용 프로그램 설치 및 제거 {#notification-app-install-uninstall}

[!UICONTROL Notification Center] 웹 응용 프로그램을 설치하여 브라우저 외부에서 알림을 받고 관리할 수 있습니다. 응용 프로그램은 Search, Social 및 Commerce 내의 [!UICONTROL Notification Center]과(와) 같은 모양이며 같은 기능을 가지고 있습니다. 응용 프로그램은 [!DNL Google Chrome] 40 이상 또는 [!DNL Microsoft Edge] 17 이상에서 사용할 수 있습니다.

[!UICONTROL Notification Center] 응용 프로그램을 설치하면 브라우저의 응용 프로그램 관리자에서 자동으로 활성화되어 레이아웃이 창 크기에 따라 동적으로 정렬되는 별도의 창으로 로드됩니다. 브라우저의 응용 프로그램 관리자에서 응용 프로그램을 열고 닫거나 운영 체제의 작업 표시줄이나 도크에 고정할 수 있습니다. 응용 프로그램이 자동으로 업데이트됩니다.

![Microsoft Windows 작업 표시줄의 알림 센터 아이콘](/help/search-social-commerce/assets/windows-taskbar.png "Microsoft Windows 작업 표시줄의 알림 센터 아이콘")

브라우저의 응용 프로그램 관리자에서 응용 프로그램을 비활성화하거나 제거할 수 있습니다. 웹 응용 프로그램 관리에 대한 자세한 내용은 브라우저의 도움말을 참조하십시오.

### [!DNL Google Chrome]용 [!UICONTROL Notification Center] 웹 응용 프로그램 설치

1. 페이지의 오른쪽 상단에서 ![알림](/help/search-social-commerce/assets/notifications.png "알림")을 클릭합니다.

1. **[!UICONTROL View All]**&#x200B;을(를) 클릭합니다.

1. 오른쪽 하단에서 ![알림 센터 웹 앱 설치](/help/search-social-commerce/assets/notifications-install-app.png "알림 센터 웹 앱 설치")를 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Add]**&#x200B;을(를) 클릭합니다.

1. 설치 앱에서? 메시지를 보려면 **[!UICONTROL Install]**&#x200B;을(를) 클릭하십시오.

### [!DNL Microsoft Edge]용 [!UICONTROL Notification Center] 웹 응용 프로그램 설치

* 검색, 소셜 및 Commerce 내에서:

   1. 페이지의 오른쪽 상단에서 ![알림](/help/search-social-commerce/assets/notifications.png "알림")을 클릭합니다.

   1. **[!UICONTROL View All]**&#x200B;을(를) 클릭합니다.

   1. 오른쪽 하단에서 ![알림 센터 웹 앱 설치](/help/search-social-commerce/assets/notifications-install-app.png "알림 센터 웹 앱 설치")를 클릭합니다.

   1. 확인 메시지에서 **[!UICONTROL Add]**&#x200B;을(를) 클릭합니다.

   1. [!UICONTROL Install Notification Center] 앱 메시지에서 **[!UICONTROL Install]**&#x200B;을(를) 클릭합니다.

* [!DNL Edge] 주 메뉴에서:

   1. 브라우저 도구 모음에서 **..** > **[!UICONTROL Apps]** > **[!UICONTROL Install Notification Center]**&#x200B;을(를) 클릭합니다.

   1. [!UICONTROL Install Notification Center] 앱 메시지에서 **[!UICONTROL Install]**&#x200B;을(를) 클릭합니다.

### [!DNL Google Chrome]에 대한 [!UICONTROL Notification Center] 웹 응용 프로그램 제거

* [!DNL Chrome]에서 `chrome://apps`(으)로 이동하여 **[!UICONTROL notification-center]**&#x200B;을(를) 마우스 오른쪽 단추로 클릭한 다음 **[!UICONTROL Remove from Chrome]**&#x200B;을(를) 클릭합니다.

### [!DNL Microsoft Edge]에 대한 [!UICONTROL Notification Center] 웹 응용 프로그램 제거

1. [!DNL Edge] 브라우저 도구 모음에서 **..** > **[!UICONTROL Apps]** > **[!UICONTROL Manage apps]**&#x200B;을(를) 클릭합니다. 또는 `edge://apps`(으)로 이동합니다.

1. **[!UICONTROL Notification Center]**&#x200B;을(를) 마우스 오른쪽 단추로 클릭하고 **[!UICONTROL Uninstall]**&#x200B;을(를) 클릭합니다.
