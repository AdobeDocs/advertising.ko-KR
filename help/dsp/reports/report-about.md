---
title: 사용자 정의 보고서 정보
description: 사용자 지정 보고서를 수동으로 만들거나 사전 구성된 보고서 템플릿을 사용하는 옵션에 대해 알아봅니다.
feature: DSP Custom Reports
exl-id: 321062f3-754b-4379-9587-003862c4221b
source-git-commit: 1d8f7c8a365b53a0345ef4155802802acbf3f027
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# 사용자 정의 보고서 정보

사용자 지정 보고서를 사용하면 캠페인 차원(광고주, 배치, 사이트 또는 지역 등)과 사용자에게 가장 중요한 지표를 사용하여 보고서 데이터의 콘텐츠와 게재를 사용자 지정할 수 있습니다. 다음 중 하나를 수행할 수 있습니다.

* 세분화된 수준에서 캠페인 성과 보고서를 완전히 구성합니다.
* 사전 구성된 보고서 템플릿 중에서 선택하고 선택적으로 추가로 사용자 지정합니다.

보고서를 한 번 생성하거나 지정된 시간대의 03:00에 일별, 주별 또는 월별 생성되도록 예약할 수 있습니다. 보고서가 생성되면 지정된 각 이메일 수신자에게 전달되거나 연결됩니다 [보고서 대상](/help/dsp/reports/report-destinations/report-destination-about.md) 다음 유형 중 하나:

* [!DNL Amazon Simple Storage Service] ([!DNL S3])
* FTP
* SFTP
* FTP SSL (Beta)

>[!NOTE]
>
>캠페인(캠페인, 패키지, 배치 또는 광고)의 모든 수준에서 온디맨드 데이터를 볼 수도 있습니다 [관련 캠페인 관리 보기 내](/help/dsp/campaign-management/reports/campaign-reports-about.md).

## 사용 가능한 보고서 유형

* **[!UICONTROL Custom]:** 이 보고서는 대부분의 차원과 지표를 사용하여 사용자 지정 보고서를 만드는 데 사용할 수 있는 빈 템플릿입니다. [!UICONTROL Conversion], [!UICONTROL Device], [!UICONTROL Geo], 및 [!UICONTROL Site] 보고서는 각 사용 사례에 대해 미리 선택된 열과 차원이 있는 이 템플릿의 변형입니다.

* 사전 구성된 보고서 템플릿

   * **[!UICONTROL Billing]:** 이 보고서를 사용하여 캠페인별 미디어 청구에 대한 지출 지표와 같은 주요 청구 지표를 이해할 수 있습니다. 범용 ID를 대상으로 하는 배치에는 데이터를 사용할 수 없습니다.

     >[!NOTE]
     >
     >이 보고서에는 청구 세그먼트에 대한 데이터가 포함됩니다. 사용자 또는 장치에 여러 세그먼트에 속하는 노출이 제공되는 경우 청구 가능한 세그먼트는 하나만 노출로 크레딧됩니다.

   * **[!UICONTROL Conversion]:** 이 보고서를 사용하여 Adobe Advertising 전환 추적을 사용하여 캡처된 전환 지표를 기반으로 캠페인이 수행되는 방식을 이해합니다. 이 보고서에는 멀티 터치 속성이 포함됩니다.

   * **[!UICONTROL Device]:** 사전 채워진 이 템플릿을 사용하여 디바이스 관련 차원별 주요 지표를 볼 수 있습니다.

   * **[!UICONTROL Frequency (by Impression)]:** 이 보고서를 사용하여 고유 뷰어에 표시된 노출 횟수 분포(예: 한 노출, 두 노출, 세 노출 등을 본 고유 뷰어 수)를 파악할 수 있습니다. 배치 또는 캠페인으로 데이터를 사용할 수 있습니다.

     >[!NOTE]
     >
     >* 데이터는 2019년 3월 1일 이후에 사용할 수 있습니다.
     >* 빈도는 데이터 샘플링을 기반으로 계산됩니다.
     >* 일부 인벤토리의 경우 게시자는 장치 식별자를 전달하지 않으므로 빈도를 추적할 수 없습니다. 이 보고서에는 장치 식별자를 사용할 수 있었던 노출만 포함됩니다.

   * **[!UICONTROL Frequency (by App/Site)]:** 이 보고서를 사용하여 앱 또는 사이트별로 도달한 고유 사용자 수를 파악합니다. 특정 앱 또는 사이트만 통해 도달한 고유 사용자 수(&quot;고유 사용자&quot;)를 확인할 수도 있습니다.

     >[!NOTE]
     >
     >* 데이터는 2018년 11월 15일 이후에 사용할 수 있습니다.
     >* 일부 개인 인벤토리의 경우 게시자는 장치 식별자를 전달하지 않으므로 빈도를 추적할 수 없습니다.

   * **[!UICONTROL Geo]**: 이 미리 채워진 템플릿을 사용하여 지리적 차원별 주요 지표를 볼 수 있습니다.

   * **[!UICONTROL Margin]:** 이 보고서를 사용하여 캠페인이나 배치별 이익, 이익 및 기타 지출 지표와 같은 주요 지표를 볼 수 있습니다. 범용 ID를 대상으로 하는 배치에는 데이터를 사용할 수 없습니다.

   * **[!UICONTROL Segment]:** 미리 채워진 이 템플릿을 사용하여 세그먼트별 주요 지표를 볼 수 있습니다.

     >[!NOTE]
     >
     >* 이 보고서는 다양한 타겟팅된 세그먼트의 성과를 보여 주기 위한 것입니다. 세그먼트 멤버십 데이터를 사용합니다. 노출이 두 개 이상의 타겟팅된 세그먼트에 속하는 개인 또는 디바이스에 제공되면 이 보고서에는 각 세그먼트에 대한 행이 한 개 포함됩니다. 이러한 이유로 이 보고서의 합계는 실제 게재와 일치하지 않을 수 있습니다.
     >* 세그먼트에 대한 전환 지표 및 사용자 지정 목표 데이터는 2019년 8월 2일 이후에 사용할 수 있습니다. 세그먼트에 대한 다른 모든 데이터는 2018년 6월 1일 이후부터 사용할 수 있습니다.

   * **[!UICONTROL Site]:** 기본적으로 에는 사이트별 표준 지표, 총 미디어 순 지출 및 총 청구 가능 순 지출이 포함됩니다.

   * **[!UICONTROL Household Reach & Frequency]:** 이 보고서를 사용하여 장치/쿠키 수준이 아닌 IP 주소를 기반으로 하는 가구 수준에서 단일 차원에 대한 노출 횟수, 도달 범위 및 빈도를 확인할 수 있습니다. 인사이트를 사용하여 미디어 믹스를 최적화하고, 성능을 개선하고, 증분 도달 기회를 식별합니다. 를 참조하십시오.[세대 보고서에 대한 FAQ](/help/dsp/reports/faq-household-report.md)&quot; 을 참조하십시오. 범용 ID를 대상으로 하는 배치에는 데이터를 사용할 수 없습니다.

   * **[!UICONTROL Household Conversions]:** 이 보고서를 사용하여 장치/쿠키 수준이 아닌 IP 주소를 기반으로 가구 수준에서 뷰스루 전환을 볼 수 있습니다. 이 인사이트를 사용하여 캠페인 성과를 측정하고 최적화할 수 있습니다. 를 참조하십시오.[세대 보고서에 대한 FAQ](/help/dsp/reports/faq-household-report.md)&quot; 을 참조하십시오. 범용 ID를 대상으로 하는 배치에는 데이터를 사용할 수 없습니다.

## 교차 계정 보고 {#cross-account-reporting}

여러 DSP 계정이 있는 조직은 조직의 필요에 따라 선택적으로 사용자 지정 보고서에서 교차 계정 데이터를 활성화할 수 있습니다. 예를 들어 계정 A에게 계정 B의 데이터에 대한 액세스 권한을 부여하고 계정 B에게 계정 C의 (계정 A의 데이터는 아님) 데이터에 대한 액세스 권한을 부여할 수 있습니다. 이 기능을 활성화하고 구성하려면 Adobe 계정 팀에 문의하십시오.

조직에 대해 기능이 활성화되면 다음을 수행할 수 있습니다. [필터](report-settings.md) 계정별 보고서 유형:  [!UICONTROL Custom], [!UICONTROL Site], [!UICONTROL Segment], [!UICONTROL Geo], [!UICONTROL Device], [!UICONTROL Frequency (by Impression)], 및 [!UICONTROL Conversion].

의 계정 설정 [!UICONTROL Settings] > [!UICONTROL Account] a) 계정에 데이터를 사용할 수 있는 다른 계정과 b) 계정의 데이터에 액세스할 수 있는 다른 계정을 나타냅니다.

>[!MORELIKETHIS]
>
>* [사용자 지정 보고서 만들기](/help/dsp/reports/report-create.md)
>* [사용자 지정 보고서 설정](/help/dsp/reports/report-settings.md)
>* [세대 보고서에 대한 FAQ](/help/dsp/reports/faq-household-report.md)
>* [Campaign Management 보기의 성능 보고서 유형](/help/dsp/campaign-management/reports/campaign-reports-about.md)
>* [사용 가능한 보고서 열](/help/dsp/reports/report-columns.md)
>* [정보 [!UICONTROL Report Destinations]](/help/dsp/reports/report-destinations/report-destination-about.md)
