---
title: 생성 [!DNL Advertising Insight]
description: 을(를) 만드는 방법 알아보기 [!DNL Advertising Insight].
exl-id: e6b692be-189e-4c6c-a536-e6c78801853d
feature: Search Advertising Insights
source-git-commit: e517dd5f5fa283ff8a2f57728612937148889732
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# 생성 [!DNL Advertising Insight]

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Insights & Reports] >[!UICONTROL Advertising Insights]**.

2. 생성하려는 인사이트를 클릭합니다.

3. 인사이트 설정 지정:

   1. (일부 보고서, 선택 사항) 인사이트에 대한 날짜 범위를 지정합니다.

   2. (가장 통찰력 있음) 분석할 포트폴리오를 선택합니다.

      일반적으로 활성 캠페인이 포함된 모든 최적화 및 활성 포트폴리오를 사용할 수 있습니다. 일부 통찰력의 경우 포함할 포트폴리오 목록을 필터링할 수 있습니다 **[!UICONTROL Only Optimized Portfolios]**.

      대상 [!UICONTROL Day of Week] 충분한 지출이 있고 지난 2일 동안 타깃팅에 지출한 포트폴리오만 사용할 수 있는 통찰력을 제공합니다.

   3. ([!UICONTROL Event Path Beta] insight만 해당) 다음을 수행합니다.

      1. 다음 항목 선택 **[!UICONTROL Operation]**: *[!UICONTROL Extract events]* (업로드: [!UICONTROL Channel Assist Report] 또는 [!UICONTROL Campaign Assist Report] 및 분석을 위해 사용자 이벤트를 개별 그룹으로 분류) 또는 *[!UICONTROL Analyze classified events]* (이벤트 그룹을 업로드하고 이를 사용하여 인사이트를 생성합니다.)

      1. 클릭 **[!UICONTROL Select]** XLSX 및 ZIP(압축된 XLSX) 형식으로 파일을 찾은 다음 **[!UICONTROL Upload]**.

   4. ([!UICONTROL Google Account Audit] insight만 해당) 다음을 수행합니다.

      1. 다음을 입력합니다. **[!UICONTROL Advertiser Name]** 및 **[!UICONTROL Account Name]**.

      1. 다음 항목 선택 **[!UICONTROL Account Currency]**, **[!UICONTROL File Format Region]** (*[!UICONTROL United States]* 또는 *[!UICONTROL United Kingdom]*) 및 **[!UICONTROL Output Language]** (*[!UICONTROL English (USA)]*, *[!UICONTROL French]*, 또는 *[!UICONTROL German]*).

      1. 클릭 **[!UICONTROL Select]** 에서 계정에 대해 다운로드한 캠페인, 키워드 및 변경 내역 보고서를 찾으려면 [!DNL Google Ads] 웹 사용자 인터페이스 및 에서 계정에 대해 다운로드한 일괄 시트 파일 [!DNL Google Ads Editor] 응용 프로그램. 그런 다음 **[!UICONTROL Upload]**.

         모든 파일은 CSV, TSV, TXT 또는 ZIP(압축된 CSV, TSV 또는 TXT) 형식이어야 합니다.

   5. ([!UICONTROL Location Target Performance] insight만 해당, 선택 사항) 요약이 아닌 매일 데이터를 집계하려면 다음을 선택합니다. **[!UICONTROL Time Aggregation]** / *[!UICONTROL Daily]*.

   6. ([!UICONTROL Normalized Sim (Combined)] insight만 해당) 다음을 수행합니다.

      1. 다음에서 **[!UICONTROL Step]** 필드에 인사이트에 포함할 타겟 지출 레벨 수 또는 단계를 지정합니다. 값은 3~100 사이일 수 있습니다.

      1. 다음에서 **[!UICONTROL Type]** 필드에서 시뮬레이션 유형을 선택합니다.

         * *[!UICONTROL Optimized Multi-portfolio]*: 동일한 목표와 통화를 사용하는 여러 포트폴리오에 대해 단일 시뮬레이션을 생성합니다.

         * *[!UICONTROL Individual Normalized]*: 선택한 각 포트폴리오에 대해 개별 시뮬레이션을 생성합니다. 포트폴리오의 목표와 통화는 다를 수 있습니다.

   7. ([!UICONTROL Portfolio Launch] insight만 해당, 선택 사항) 미래의 시작 날짜를 지정하려면 **[!UICONTROL Optional Date]** 필드.

   8. ([!UICONTROL Quality Score] insight만 해당) 해당 광고 네트워크를 선택합니다.

   9. ([!UICONTROL Query Cross Matching] insight만 해당) **[!UICONTROL Google Accounts]** 메뉴에서 계정을 선택합니다.

4. 클릭 **[!UICONTROL Generate Insight]**.

   에 따라 작업이 완료되거나 실패하면 알림을 받습니다. [구성된 알림 설정](/help/search-social-commerce/notifications/notification-edit.md) 대상 [!UICONTROL Advertising Insights].

>[!MORELIKETHIS]
>
>* [정보 [!UICONTROL Advertising Insights]](insight-about.md)
>* [보기 또는 저장 [!DNL Advertising Insight]](insight-view-save.md)
>* [삭제 [!DNL Advertising Insight]](insight-delete.md)
