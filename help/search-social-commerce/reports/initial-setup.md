---
title: 보고서의 초기 설정 작업
description: 보고서에서 지표를 사용할 수 있도록 하는 방법과 보고서를 자동화하는 방법을 알아봅니다.
exl-id: c2e76c63-ddb8-4762-8628-30cf3f54b8fd
feature: Search Reports
source-git-commit: 724b4ff772fa7d6dc0640d35a968d664707ceae6
workflow-type: tm+mt
source-wordcount: '336'
ht-degree: 0%

---

# 보고서의 초기 설정 작업

신규 사용자는 다음과 같은 초기 설정 작업을 수행해야 합니다.

* Adobe Advertising이 광고주에 대해 추적하는 전환 지표를 [보고서와 다른 보기에 사용 가능하게 만들고](/help/search-social-commerce/admin/conversion-metrics/conversion-metric-edit-available.md), 선택적으로 [가독성을 위해 열 제목에 표시되는 전환 지표의 이름을 모두 바꾸고](/help/search-social-commerce/admin/conversion-metrics/conversion-metric-edit-display-name.md)있습니다.

  트랜잭션 속성은 특별히 사용 가능하게 만들지 않으면 보고서에 사용할 수 없습니다.

  나중에 새 전환 지표를 추적하기 시작하는 경우 이 작업을 반복해야 합니다.

* (선택 사항) 보고서 생성 자동화:

   * 지난 주 또는 지난 30일 동안의 [!UICONTROL Campaign Report]과(와) 같이 특정 시간 증분에 대한 보고서 데이터를 정기적으로 생성하려는 경우 [보고서 템플릿](/help/search-social-commerce/reports/automation/templates/template-about.md)을 설정하고 매일 또는 주나 월의 특정 날짜에 실행되도록 예약할 수 있습니다. 보고서 실행이 예약될 때마다 새 보고서가 생성됩니다. 보고서가 완료되면 [!UICONTROL Notification Center][&#128279;](/help/search-social-commerce/notifications/notification-about.md)에 구성된 알림 설정에 따라 특정 검색, 소셜 및 Commerce 사용자의 전자 메일 주소를 알릴 수 있습니다.

   * 피벗 테이블 및 추가 계산을 수행해야 하는 추가 열이 있거나 없는 사용자 지정 형식의 스프레드시트에서 최신 일일 보고서 데이터를 보려면 매일 [스프레드시트 피드](/help/search-social-commerce/reports/automation/spreadsheet-feeds/spreadsheet-feed-about.md)를 설정할 수 있습니다. 스프레드시트 피드는 최신 성능 데이터로 매일 새로 고침되며 이전 날짜에 대한 데이터는 계속 유지됩니다. 스프레드시트 피드를 구성하려면 먼저 [!DNL Microsoft Excel]에서 사용자 지정된 스프레드시트 템플릿을 만들어야 합니다. [!UICONTROL Notification Center][&#128279;](/help/search-social-commerce/notifications/notification-about.md)에 구성된 알림 설정을 기반으로 피드 파일을 사용할 수 있을 때 특정 검색, 소셜 및 Commerce 사용자의 전자 메일 주소를 알릴 수 있는 옵션이 있습니다.

   * FTP 위치에서 기본 및 고급 보고서를 받으려면 FTP 계정을 요청하고 특정 명명 규칙을 사용하여 보고서 템플릿을 설정하여 [기본 및 고급 보고서에 대한 FTP 액세스](/help/search-social-commerce/reports/automation/ftp-reports.md)를 설정할 수 있습니다.

>[!MORELIKETHIS]
>
>* [보고서 정보](report-about.md)
>* [보고서에 사용된 데이터](data-used-for-reports.md)
