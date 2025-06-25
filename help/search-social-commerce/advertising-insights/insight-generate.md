---
title: ' [!DNL Advertising Insight] 생성'
description: ' [!DNL Advertising Insight]을(를) 만드는 방법을 알아봅니다.'
exl-id: e6b692be-189e-4c6c-a536-e6c78801853d
feature: Search Advertising Insights
source-git-commit: d0f1c413134a0868ddec79ded7672af316267edd
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# [!DNL Advertising Insight] 생성

1. 메인 메뉴에서 **[!UICONTROL Search, Social, & Commerce]> [!UICONTROL Insights & Reports] >[!UICONTROL Advertising Insights]**&#x200B;을(를) 클릭합니다.

2. 생성하려는 insight을 클릭합니다.

3. insight 설정을 지정합니다.

   1. (일부 보고서, 선택 사항) insight의 날짜 범위를 지정합니다.

   2. (가장 통찰력 있음) 분석할 포트폴리오를 선택합니다.

      일반적으로 활성 캠페인이 포함된 모든 최적화 및 활성 포트폴리오를 사용할 수 있습니다. 일부 인사이트의 경우 **[!UICONTROL Only Optimized Portfolios]**&#x200B;을(를) 포함하도록 포트폴리오 목록을 필터링할 수 있습니다.

      [!UICONTROL Day of Week] 인사이트의 경우 지출이 충분한 포트폴리오와 지난 2일 동안 타깃팅에 사용한 포트폴리오만 사용할 수 있습니다.

   3. ([!UICONTROL Event Path Beta] insight만 해당) 다음을 수행합니다.

      1. **[!UICONTROL Operation]**: *[!UICONTROL Extract events]*(분석을 위해 [!UICONTROL Channel Assist Report] 또는 [!UICONTROL Campaign Assist Report]을(를) 업로드하고 사용자 이벤트를 개별 그룹으로 분류하려면) 또는 *[!UICONTROL Analyze classified events]*(이벤트 그룹을 업로드하고 이를 사용하여 insight을 생성하려면)을 선택합니다.

      1. **[!UICONTROL Select]**&#x200B;을(를) 클릭하여 XLSX 및 ZIP(압축된 XLSX) 형식의 파일을 찾은 다음 **[!UICONTROL Upload]**&#x200B;을(를) 클릭합니다.

   4. ([!UICONTROL Google Account Audit] insight만 해당) 다음을 수행합니다.

      1. **[!UICONTROL Advertiser Name]** 및 **[!UICONTROL Account Name]**&#x200B;을(를) 입력하십시오.

      1. **[!UICONTROL Account Currency]**, **[!UICONTROL File Format Region]**(*[!UICONTROL United States]* 또는 *[!UICONTROL United Kingdom]*) 및 **[!UICONTROL Output Language]**(*[!UICONTROL English (USA)]*, *[!UICONTROL French]* 또는 *[!UICONTROL German]*)을(를) 선택하십시오.

      1. **[!UICONTROL Select]**&#x200B;을(를) 클릭하여 [!DNL Google Ads] 웹 사용자 인터페이스에서 계정에 대해 다운로드한 캠페인, 키워드 및 변경 기록 보고서와 [!DNL Google Ads Editor] 애플리케이션에서 계정에 대해 다운로드한 일괄 시트 파일을 찾습니다. **[!UICONTROL Upload]**&#x200B;을(를) 클릭합니다.

         모든 파일은 CSV, TSV, TXT 또는 ZIP(압축된 CSV, TSV 또는 TXT) 형식이어야 합니다.

   5. ([!UICONTROL Location Target Performance] insight 전용, 선택 사항) 데이터를 요약이 아닌 매일 집계하려면 *[!UICONTROL Daily]*&#x200B;의 **[!UICONTROL Time Aggregation]**&#x200B;을(를) 선택하십시오.

   6. ([!UICONTROL Normalized Sim (Combined)] insight만 해당) 다음을 수행합니다.

      1. **[!UICONTROL Step]** 필드에서 insight에 포함할 대상 지출 수준 또는 단계 수를 지정합니다. 값은 3~100 사이일 수 있습니다.

      1. **[!UICONTROL Type]** 필드에서 시뮬레이션 유형을 선택합니다.

         * *[!UICONTROL Optimized Multi-portfolio]*: 동일한 목표와 통화를 사용하는 여러 포트폴리오에서 단일 시뮬레이션을 생성합니다.

         * *[!UICONTROL Individual Normalized]*: 선택한 각 포트폴리오에 대해 개별 시뮬레이션을 생성합니다. 포트폴리오의 목표와 통화는 다를 수 있습니다.

   7. ([!UICONTROL Portfolio Launch] insight 전용, 선택 사항) 실행 날짜를 미래의 날짜로 지정하려면 **[!UICONTROL Optional Date]** 필드에 날짜를 지정합니다.

   8. ([!UICONTROL Quality Score] insight만 해당) 해당 광고 네트워크를 선택합니다.

   9. ([!UICONTROL Query Cross Matching] insight 전용) **[!UICONTROL Google Accounts]** 메뉴에서 계정을 선택합니다.

4. **[!UICONTROL Generate Insight]**&#x200B;을(를) 클릭합니다.

   [!UICONTROL Advertising Insights]에 대해 [구성된 알림 설정](/help/search-social-commerce/notifications/notification-edit.md)을 기반으로 작업이 완료되거나 실패하면 알림을 받습니다.

>[!MORELIKETHIS]
>
>* [정보 [!UICONTROL Advertising Insights]](insight-about.md)
>* [보기 또는 저장 [!DNL Advertising Insight]](insight-view-save.md)
>* [삭제 [!DNL Advertising Insight]](insight-delete.md)
