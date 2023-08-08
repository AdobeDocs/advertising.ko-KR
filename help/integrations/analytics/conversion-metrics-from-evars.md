---
title: "Adobe Analytics에서 전환 지표 만들기 [!DNL eVars] 및 prop"
description: "다음을 사용하여 사용자 정의 성공 이벤트 지표 구성 [!DNL eVar]- 및 [!DNL prop]-level data."
feature: Integration with Adobe Analytics, Conversions
source-git-commit: 73cdb171523b55f48b5ae5c5b2b4843f542336a6
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---

# Adobe Analytics에서 전환 지표 만들기 [!DNL eVars] 및 [!DNL props]

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

성공 이벤트 지표를 사용하여 브랜드 목표에 가장 적합한 Adobe Analytics 사이트 데이터를 기반으로 DSP 패키지 및 검색, 소셜 및 상거래 캠페인을 최적화할 수 있습니다. 다음을 기반으로 사용자 정의 성공 이벤트 지표를 구성할 수 있습니다. [기존 항목 [!DNL Analytics] [!DNL eVars]](https://experienceleague.adobe.com/docs/analytics/components/dimensions/evar.html) 및 [본인 [!DNL props]](https://experienceleague.adobe.com/docs/analytics/components/dimensions/prop.html) 벼락치기로 [!DNL eVar]- 및 [!DNL prop]-level 데이터를 이벤트에 추가합니다. 기타 [!DNL Analytics] 표준, 사용자 지정 및 예약 전환 지표와 트래픽 지표를 포함한 지표는 DSP 및 Search, Social, Commerce에서 자동으로 사용할 수 있습니다.

![사용 예](/help/integrations/assets/a4adc-conversion-evar-example.jpg "사용 예")

다음 작업의 대부분은 [!DNL Analytics] 관리자 또는 다른 사용자. 지원이 필요한 경우 (DSP 사용자) DSP 기술 지원 팀( )에 문의하십시오. `adcloud_support@adobe.com` 또는 (검색, 소셜 및 상거래 사용자) Adobe 계정 팀에 문의하십시오.

1. 위치 [!DNL Analytics], [자리 표시자 성공 이벤트 만들기](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/manage-report-suites/edit-report-suite/conversion-variables/success-events/success-event.html?lang=en).

   다음 추가 매개 변수를 사용하십시오.

   **유형:** `Counter`

   **극성:**  다음 중 하나 `Up is Good` 또는 `Up is Bad`

   **가시성:** `Visible Everywhere`

   **고유 이벤트 기록:** `Always Record Event`

   **기여도:** `Enabled`

   이미 캡처한 기존 데이터를 사용하므로 브랜드 웹 사이트에서 새 이벤트를 구현할 필요가 없습니다.

1. 에서 처리 규칙 만들기 [!DNL Analytics]:

   >[!NOTE]
   >
   >전용 [!DNL Analytics] 관리자가 아닌 사용자에게 권한을 부여하지 않은 경우 계정 관리자는 처리 규칙을 만들 수 있습니다.

   1. [처리 규칙 만들기](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/manage-report-suites/edit-report-suite/report-suite-general/c-processing-rules/c-processing-rules-configuration/t-processing-rules.html?lang=en), 다음 구성 사용:

      * 충족해야 하는 조건에 대해 필요한 을 지정합니다 [!DNL eVars] 또는 [!DNL props].

        가장 정확한 이벤트가 생성되도록 필요에 따라 세부 기간을 추가로 구성할 수 있습니다.

        >[!TIP]
        >
        >가장 좋은 방법은 하나만 사용하는 것입니다 [!DNL eVar] 또는 [!DNL prop].

      * 작업에 대해 을(를) 선택합니다 **이벤트 설정** 자리 표시자 이벤트를 선택합니다.

   1. 위치 [!DNL Analytics] [!DNL Analysis Workspace], [프로젝트 만들기](https://experienceleague.adobe.com/docs/analytics/analyze/analysis-workspace/home.html) 및에 대해 데이터가 채워지고 있는지 확인하기 위해 새 이벤트를 자유 형식 테이블로 가져옵니다. [!DNL eVar] 또는 [!DNL prop] 지표.

1. 새 지표를 Adobe에 동기화하려면 Adobe Advertising 계정 팀에 문의하십시오.

지표를 사용할 수 있으면에서 이 지표를 사용하여 목표를 만든 다음, 이를 검색, 소셜 및 상거래 포트폴리오에 지정하거나 로 사용할 수 있습니다. [사용자 정의 목표](/help/dsp/optimization/custom-goal-about.md) DSP 패키지의 경우.

목표 작성에 대한 자세한 내용은 Search, Social 및 Commerce에서 제공되는 &quot;목표&quot;에 대한 최적화 안내서 장을 참조하십시오.

>[!MORELIKETHIS]
>
>* [[!DNL Analytics] Adobe Advertising의 데이터](/help/integrations/analytics/analytics-data-in-advertising.md)
<!--
>* [](/help/search-social-commerce/admin/conversion-metrics/ ????????)
-->