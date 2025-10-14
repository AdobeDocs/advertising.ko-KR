---
title: Adobe Analytics [!DNL eVars]  및 prop에서 전환 지표 만들기
description: ' [!DNL eVar] 및  [!DNL prop] 수준 데이터를 사용하여 사용자 지정 성공 이벤트 지표를 구성합니다.'
feature: Integration with Adobe Analytics, Conversions
exl-id: 7717d10c-76ca-4ba9-9fbb-e34ad006619c
source-git-commit: be78460b42e1d9622cb781a0a32b01a34464a76d
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# Adobe Analytics [!DNL eVars] 및 [!DNL props]에서 전환 지표 만들기

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

성공 이벤트 지표를 사용하여 브랜드 목표에 가장 적합한 DSP 사이트 데이터를 기반으로 Commerce 패키지 및 검색, 소셜 및 Adobe Analytics 캠페인을 최적화할 수 있습니다. [[!DNL Analytics] [!DNL eVars] 및 &#x200B;](https://experienceleague.adobe.com/docs/analytics/components/dimensions/evar.html?lang=ko) 수준 데이터를 이벤트에 통합하여 기존 [[!DNL props]](https://experienceleague.adobe.com/docs/analytics/components/dimensions/prop.html?lang=ko) 및 [!DNL eVar][!DNL prop]을(를) 기반으로 사용자 지정 성공 이벤트 지표를 구성할 수 있습니다. 표준, 사용자 지정 및 예약 전환 지표와 트래픽 지표를 포함한 다른 [!DNL Analytics] 지표는 DSP과 검색, 소셜 및 Commerce에서 자동으로 사용할 수 있습니다.

![사용 예](/help/integrations/assets/a4adc-conversion-evar-example.jpg "사용 예")

[!DNL Analytics] 관리자 또는 다른 사용자가 다음 작업 대부분을 수행해야 합니다. 지원이 필요한 경우 Adobe 계정 팀에 문의하십시오.

1. [!DNL Analytics]에서 [자리 표시자 성공 이벤트를 만듭니다](https://experienceleague.adobe.com/ko/docs/analytics/admin/admin-tools/manage-report-suites/edit-report-suite/conversion-variables/success-event).

   다음 추가 매개 변수를 사용하십시오.

   **유형:** `Counter`

   **극성:** `Up is Good` 또는 `Up is Bad`

   **가시성:** `Visible Everywhere`

   **고유 이벤트 기록:** `Always Record Event`

   **기여도:** `Enabled`

   이미 캡처한 기존 데이터를 사용하므로 브랜드 웹 사이트에서 새 이벤트를 구현할 필요가 없습니다.

1. [!DNL Analytics]에서 처리 규칙을 만들고 유효성을 검사합니다.

   >[!NOTE]
   >
   >관리자가 아닌 사용자에게 권한을 부여하지 않은 경우 [!DNL Analytics] 계정 관리자만 처리 규칙을 만들 수 있습니다.

   1. 다음 구성을 사용하여 [처리 규칙을 만듭니다](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/manage-report-suites/edit-report-suite/report-suite-general/c-processing-rules/c-processing-rules-configuration/t-processing-rules.html?lang=ko).

      * 충족해야 하는 조건에 대해 필요한 [!DNL eVars] 또는 [!DNL props]을(를) 지정하십시오.

        가장 정확한 이벤트가 생성되도록 필요에 따라 세부 기간을 추가로 구성할 수 있습니다.

        >[!TIP]
        >
        >가장 좋은 방법은 [!DNL eVar] 또는 [!DNL prop] 중 하나만 사용하는 것입니다.

      * 작업에 대해 **이벤트 설정**&#x200B;을 선택하고 자리 표시자 이벤트를 선택합니다.

   1. [!DNL Analytics] [!DNL Analysis Workspace]에서 [프로젝트를 만들고](https://experienceleague.adobe.com/docs/analytics/analyze/analysis-workspace/home.html?lang=ko) 새 이벤트를 자유 형식 테이블로 가져와 데이터가 [!DNL eVar] 또는 [!DNL prop] 지표에 대해 채워지고 있는지 확인하십시오.

1. Adobe 계정 팀에 문의하여 새 지표를 Adobe Advertising에 동기화하십시오.

지표를 사용할 수 있게 되면 이를 사용하여 목표를 만든 다음 검색, 소셜 및 Commerce 포트폴리오에 할당하거나 DSP 패키지에 대한 [사용자 지정 목표](/help/dsp/optimization/custom-goal.md)(으)로 사용할 수 있습니다.

목표 작성에 대한 자세한 내용은 Search, Social 및 Commerce 내에서 사용할 수 있는 &quot;목표&quot;에 대한 최적화 안내서 장을 참조하십시오

>[!MORELIKETHIS]
>
>* [[!DNL Analytics] Adobe Advertising의 데이터](/help/integrations/analytics/analytics-data-in-advertising.md)
>* [광고주에 대해 추적된 전환 지표를 봅니다](/help/search-social-commerce/admin/conversion-metrics/conversion-metric-view-tracked.md)
