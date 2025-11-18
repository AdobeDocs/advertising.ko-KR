---
title: 사용자 정의 보고서 정보
description: 사용자 지정 보고서를 수동으로 만들거나 사전 구성된 보고서 템플릿을 사용하는 옵션에 대해 알아봅니다.
feature: DSP Custom Reports
exl-id: 321062f3-754b-4379-9587-003862c4221b
source-git-commit: a643a2d255431c5ce93f2df092d92932d4cccc02
workflow-type: tm+mt
source-wordcount: '1623'
ht-degree: 0%

---

# 사용자 정의 보고서 정보

사용자 지정 보고서를 사용하면 캠페인 차원(광고주, 배치, 사이트 또는 지역 등)과 사용자에게 가장 중요한 지표를 사용하여 보고서 데이터의 콘텐츠와 게재를 사용자 지정할 수 있습니다. 다음 중 하나를 수행할 수 있습니다.

* 세분화된 수준에서 캠페인 성과 보고서를 완전히 구성합니다.

* 사전 구성된 보고서 템플릿 중에서 선택하고 선택적으로 추가로 사용자 지정합니다.

보고서를 한 번 생성하거나 지정된 기준(예: 15일마다 또는 매월 1일)에 따라 지정된 시간대의 03:00에서 매일, 매주 또는 매월 예약할 수 있습니다. 보고서가 생성되면 [!UICONTROL Reports] > [!UICONTROL Custom Reports] 또는 다음 유형의 연결된 [보고서 대상](/help/dsp/reports/report-destinations/report-destination-about.md)에서 다운로드할 수 있습니다.

* [!DNL Amazon Simple Storage Service]&#x200B;([!DNL S3])
* FTP
* FTP SSL <!-- (in beta) -->
* SFTP

>[!NOTE]
>
>캠페인(캠페인, 패키지, 배치 또는 광고)의 모든 수준에서 온디맨드 데이터를 볼 수도 있습니다. [관련 캠페인 관리 보기](/help/dsp/campaign-management/reports/campaign-reports-about.md).

## 사용 가능한 보고서 유형

* **[!UICONTROL Custom]:** 이 보고서는 대부분의 차원과 지표를 사용하여 사용자 지정 보고서를 만드는 데 사용할 수 있는 빈 템플릿입니다. [!UICONTROL Conversion], [!UICONTROL Device], [!UICONTROL Geo] 및 [!UICONTROL Site] 보고서는 각 사용 사례에 대해 미리 선택된 열과 차원이 있는 이 템플릿의 변형입니다.

* 사전 구성된 보고서 템플릿

   * **[!UICONTROL All-in Cost BETA]**: (Advertising Creative과 Advertising DSP을 모두 사용하는 광고주, Beta 기능) 이 보고서를 사용하여 Advertising DSP 지출이 Adobe Creative의 광고 제공으로 인한 것인지 확인하십시오. 캠페인, 패키지, 배치 및 광고 수준에서 크리에이티브, 속성, 타겟 및 기타 데이터를 볼 수 있습니다.

   * **[!UICONTROL Billing]:** 이 보고서를 사용하여 캠페인별 미디어 청구에 대한 지출 지표와 같은 주요 청구 지표를 이해할 수 있습니다. 범용 ID를 대상으로 하는 배치에는 데이터를 사용할 수 없습니다.

     >[!NOTE]
     >
     >이 보고서에는 청구 세그먼트에 대한 데이터가 포함됩니다. 사용자 또는 장치에 여러 세그먼트에 속하는 노출이 제공되는 경우 청구 가능한 세그먼트는 하나만 노출로 크레딧됩니다.

   * **[!UICONTROL Content]:** 이 보고서를 사용하여 지정된 콘텐츠 차원(예: 장르, 프로덕션 품질 및 콘텐츠 등급)별로 노출 전달 및 기타 지표를 이해함으로써 타깃팅을 최적화하고 브랜드 안전을 보장할 수 있습니다. 보고서는 콘텐츠 차원 외에도 대부분의 표준 차원, 지표 및 필터를 포함합니다. 콘텐츠 차원별 데이터는 [!DNL Freewheel], [!DNL Index], [!DNL Magnite], [!DNL Microsoft], [!DNL Nexxen], [!DNL Pubmatic], [!DNL Sharethrough] 및 [!DNL Triplelift]에 사용할 수 있습니다. 콘텐츠 신호는 비트스트림 중에 게시자에 의해 전달되고 가용성의 영향을 받습니다.

   * **[!UICONTROL Conversion]:** 이 보고서를 사용하여 Adobe Advertising 전환 추적을 사용하여 캡처된 전환 지표에 따라 캠페인이 수행되는 방식을 이해합니다. 이 보고서에는 멀티 터치 속성이 포함됩니다.

   * **[!UICONTROL Custom Creative]:**(Advertising Creative을 사용하는 광고주만 해당) 이 보고서를 사용하여 Advertising Creative 광고 경험 전반에서 성과를 모니터링합니다.

   * **[!UICONTROL Device]:** 미리 채워진 이 템플릿을 사용하여 장치 관련 차원별 주요 지표를 확인합니다.

   * **[!UICONTROL Frequency (by Impression)]:** 이 보고서를 사용하여 고유 뷰어에 표시된 노출 분포(예: 한 노출, 두 노출, 세 노출 등을 본 고유 뷰어의 수)를 파악합니다. 배치 또는 캠페인으로 데이터를 사용할 수 있습니다.

     >[!NOTE]
     >
     >* 데이터는 2019년 3월 1일 이후에 사용할 수 있습니다.
     >* 빈도는 데이터 샘플링을 기반으로 계산됩니다.
     >* 일부 인벤토리의 경우 게시자는 장치 식별자를 전달하지 않으므로 빈도를 추적할 수 없습니다. 이 보고서에는 장치 식별자를 사용할 수 있었던 노출만 포함됩니다.

   * **[!UICONTROL Frequency (by App/Site)]:** 이 보고서를 사용하여 앱별 또는 사이트별로 광고에 도달한 고유 사용자 수를 파악합니다. 또한 특정 앱 또는 사이트를 통해서만 광고에 도달한 고유 사용자 수(&quot;고유 사용자&quot;)를 확인할 수 있습니다.

     >[!NOTE]
     >
     >* 데이터는 2018년 11월 15일 이후에 사용할 수 있습니다.
     >* 일부 개인 인벤토리의 경우 게시자는 장치 식별자를 전달하지 않으므로 빈도를 추적할 수 없습니다.

   * **[!UICONTROL Geo]**: 미리 채워진 이 템플릿을 사용하여 지리적 차원별 주요 지표를 확인하십시오.

   * **[!UICONTROL Household Conversions]:** 이 보고서를 사용하여 장치/쿠키 수준이 아닌 IP 주소를 기반으로 하는 가구 수준에서 뷰스루 전환을 볼 수 있습니다. 이 인사이트를 사용하여 캠페인 성과를 측정하고 최적화할 수 있습니다. 자세한 내용은 &quot;[가구 보고서에 대한 FAQ](/help/dsp/reports/faq-reports.md)&quot;를 참조하십시오. 범용 ID를 대상으로 하는 배치에는 데이터를 사용할 수 없습니다.

   * **[!UICONTROL Household Reach & Frequency]:** 이 보고서를 사용하여 장치/쿠키 수준이 아닌 IP 주소를 기반으로 하는 가구 수준에서 단일 차원에 대한 노출 횟수, 도달 범위 및 빈도를 확인할 수 있습니다. 인사이트를 사용하여 미디어 믹스를 최적화하고, 성능을 개선하고, 증분 도달 기회를 식별합니다. 자세한 내용은 &quot;[가구 보고서에 대한 FAQ](/help/dsp/reports/faq-reports.md)&quot;를 참조하십시오. 범용 ID를 대상으로 하는 배치에는 데이터를 사용할 수 없습니다.

   * **[!UICONTROL Margin]:** 이 보고서를 사용하여 캠페인이나 배치별 이익, 이익 및 기타 지출 지표와 같은 주요 지표를 볼 수 있습니다. 범용 ID를 대상으로 하는 배치에는 데이터를 사용할 수 없습니다.

   * **[!UICONTROL Path to Conversion]:** 이 보고서를 사용하여 성과가 가장 좋은 광고 상호 작용 시퀀스를 기반으로 예산을 최적화하고 광고를 개인화하는 방법을 확인하십시오. 이 보고서는 지정된 데이터 범위에서 선택한 각 전환 지표를 유도하는 동일한 가구의 상호 작용 포인트 시퀀스를 보여 줍니다. 보고서는 첫 번째 상호 작용과 전환 사이에 지정된 전환 확인 기간을 사용하며 다음 차원 하나를 포함할 수 있습니다.

      * [!UICONTROL Channel Assist Type]: [!UICONTROL Audio Impression], [!UICONTROL CTV Impression], [!UICONTROL Display Click], [!UICONTROL Display Impression], [!UICONTROL Native Click], [!UICONTROL Native Impression], [!UICONTROL Search Click], [!UICONTROL Video Click] 또는 [!UICONTROL Video Impression] 마케팅 채널이 전환 프로세스를 어떻게 지원했는지 표시합니다.

      * [!UICONTROL Campaign ID] 또는 [!UICONTROL Campaign Name]: 전환 프로세스를 지원한 캠페인을 표시합니다.

      * [!UICONTROL Ad ID] 또는 [!UICONTROL Ad Name]은(는) 전환된 DSP 광고를 표시합니다.

      * [!UICONTROL Ad ID & Paid Keyword (SSC)] 또는 [!UICONTROL Ad Name & Paid Keyword (SSC)]은(는) 전환된 Search, Social 및 Commerce 키워드를 표시합니다.

     보고서의 열에는 &quot;[!UICONTROL Event #1]&quot; - &quot;[!UICONTROL Event #10]&quot;,&quot;[!UICONTROL Path Length]&quot;, &quot;% \&lt;전환 지표 이름 1\>&quot;, &quot;% \&lt;전환 지표 이름 2\>&quot; 등이 포함됩니다.

     최대 10개의 최신 상호 작용 지점이 포함됩니다. 경로 행은 전환 횟수별로 정렬됩니다.

     이 보고서를 [!DNL Advanced Measurement Services] 및 Adobe 분석에서 만든 보고서와 비교하려면 &quot;[사용자 지정 보고서에 대한 FAQ](/help/dsp/reports/faq-reports.md)&quot;를 참조하십시오.

   * **[!UICONTROL Path Length]:** 최적의 광고 빈도를 선택할 수 있도록 이 보고서를 사용하여 시간에 따른 전환에 필요한 사용자 상호 작용 지점 수를 추적합니다. 이 보고서는 사용자가 광고 상호 작용을 한 번, 광고 상호 작용을 두 번 한 후 발생한 전환 수와 같이 경로 길이(상호 작용 지점)별 전환 수를 보여줍니다. 보고서는 여러 전환 지표에 대한 데이터를 포함할 수 있으며 첫 번째 상호 작용과 전환 간에 지정된 전환 확인 기간을 사용합니다. 보고서의 열에는 &quot;[!UICONTROL Path Length]&quot;, &quot;[!UICONTROL Number of] \&lt;전환 지표 이름 1\>,&quot;% \&lt;전환 지표 이름 1\>,&quot; \&lt;전환 지표 이름 2\>,&quot;% \&lt;전환 지표 이름 2\> 등이 있습니다.

     데이터는 최대 10의 각 경로 길이에 대해 표시되며, 10보다 큰 경로 길이에 대한 데이터는 함께 그룹화됩니다.

   * **[!UICONTROL Segment]:** 미리 채워진 이 템플릿을 사용하여 세그먼트별로 주요 지표를 확인합니다.

     >[!NOTE]
     >
     >* 이 보고서는 다양한 타겟팅된 세그먼트의 성과를 보여 주기 위한 것입니다. 세그먼트 멤버십 데이터를 사용합니다. 노출이 두 개 이상의 타겟팅된 세그먼트에 속하는 개인 또는 디바이스에 제공되면 이 보고서에는 각 세그먼트에 대한 행이 한 개 포함됩니다. 이러한 이유로 이 보고서의 합계는 실제 게재와 일치하지 않을 수 있습니다.
     >* 세그먼트에 대한 전환 지표 및 사용자 지정 목표 데이터는 2019년 8월 2일 이후에 사용할 수 있습니다. 세그먼트에 대한 다른 모든 데이터는 2018년 6월 1일 이후부터 사용할 수 있습니다.

   * **[!UICONTROL Site]:** 기본적으로 표준 지표, 사이트별 총 미디어 순 지출 및 총 청구 가능 순 지출을 포함합니다.

   * **[!UICONTROL Time to Conversion]:** 이 보고서를 사용하여 최적의 속성 전환 확인 기간을 결정하고 전환 시간이 더 긴 캠페인을 식별하십시오. 전환 시간이 더 길어질 수 있으며, 이는 재타겟팅의 이점을 얻을 수 있습니다. 이 보고서는 마지막 상호 작용(광고 노출 또는 클릭)에서 전환까지의 시간(일)별 전환 수를 보여줍니다. 보고서는 여러 전환 지표에 대한 데이터를 포함할 수 있으며 첫 번째 상호 작용과 전환 간에 지정된 전환 확인 기간을 사용합니다. 보고서의 열에는 &quot;[!UICONTROL Time Taken (in days)]&quot;, &quot;[!UICONTROL Number of] \&lt;전환 지표 이름 1\>,&quot;% \&lt;전환 지표 이름 1\>,&quot; \&lt;전환 지표 이름 2\>,&quot;% \&lt;전환 지표 이름 2\> 등이 있습니다. 전환 확인 기간보다 오래 걸리는 전환은 한 행으로 그룹화됩니다(예: 보고서에서 30일 전환 확인 기간을 사용하는 경우, 발생하는 데 30일 이상 걸리는 모든 전환은 &quot;[!UICONTROL Time Taken (in days)]&quot; 값이 &quot;30+&quot;인 행으로 그룹화됨).

## 교차 계정 보고 {#cross-account-reporting}

여러 DSP 계정이 있는 조직은 조직의 필요에 따라 선택적으로 사용자 지정 보고서에서 교차 계정 데이터를 활성화할 수 있습니다. 예를 들어 계정 A에게 계정 B의 데이터에 대한 액세스 권한을 부여하고 계정 B에게 계정 C의 (계정 A의 데이터는 아님) 데이터에 대한 액세스 권한을 부여할 수 있습니다. 이 기능을 활성화하고 구성하려면 Adobe 계정 팀에 문의하십시오.

조직에 대해 기능이 활성화되면 [, &#x200B;](report-settings.md), [!UICONTROL Custom], [!UICONTROL Site], [!UICONTROL Segment], [!UICONTROL Geo] 및 [!UICONTROL Device] 보고서 유형을 계정별로 [!UICONTROL Frequency (by Impression)]필터링[!UICONTROL Conversion]할 수 있습니다.

[!UICONTROL Settings] > [!UICONTROL Account]의 계정 설정은 a) 계정에 데이터를 사용할 수 있는 다른 계정과 b) 계정의 데이터에 액세스할 수 있는 다른 계정을 나타냅니다.

## [!UICONTROL Custom Reports] 보기

[!UICONTROL Reports] > [!UICONTROL Custom Reports]에는 생성된 보고서, 향후 생성이 예약된 보고서 및 실패한 보고서를 포함하여 기존 보고서가 나열됩니다. &quot;[!UICONTROL Report Run]&quot; 열은 2024년 8월 22일부터 보고서가 트리거된 날짜를 표시합니다. 기본적으로 사용자가 만든 보관되지 않은 모든 보고서가 나열되며 가장 최근의 보고서가 맨 위에 표시됩니다. 보고서가 반복인지 일회인지 여부, 보고서 유형, 대상 유형 및 보고서 작성자 상태 별로 목록을 추가로 필터링할 수 있습니다.

새 사용자 지정 보고서를 만들거나, 기존 보고서를 편집하거나, 복제하여 새 보고서를 만들거나, 보고서를 즉시 실행하고, 지난 4개월 동안의 보고서 인스턴스를 다운로드하고, 보고서를 삭제할 수 있습니다.

## 보고서 상태 {#custom-report-status}

* **[!UICONTROL Yet to start]:** 보고서가 실행된 적이 없습니다.

* **[!UICONTROL Report generating]:** 보고서를 만드는 중입니다.

* **[!UICONTROL Ready to download]:**(반복 보고서만 해당) 하나 이상의 보고서 인스턴스를 다운로드할 수 있으며 더 많은 보고서 인스턴스가 예약되어 있습니다.

* **[!UICONTROL Failed]:** 보고서 작업이 실패했습니다. 보고서 견인에 대해 개별 보고서 인스턴스가 실패한 이유를 보려면 ![&#x200B; 옆에 있는 &#x200B;](/help/dsp/assets/chevron-down.png "아래쪽 화살표")아래쪽 화살표[!UICONTROL Download]를 클릭하십시오. 실패한 보고서 작업은 오류 아이콘(![오류 표시기](/help/dsp/assets/indicator-critical.png "오류 표시기"))으로 표시됩니다. 오류 설명을 보려면 커서를 오류 아이콘 위에 놓습니다.

* **[!UICONTROL Completed]:** 반복되지 않는 보고서의 경우 보고서가 완료됩니다. 반복 보고서의 경우 모든 보고서 인스턴스가 완료되었습니다. 지난 4개월 동안 완료된 모든 보고서를 다운로드할 수 있습니다.

* **[!UICONTROL Archived]:** 보고서가 보관되어 있으므로 실행할 수 없습니다. 이 상태는 보고서에 대해 보고서 생성에 여러 번 실패하는 경우 설정됩니다. 현재 사용자 인터페이스에서는 이 상태를 설정할 수 없습니다.

>[!MORELIKETHIS]
>
>* [사용자 지정 보고서 만들기](/help/dsp/reports/report-create.md)
>* [사용자 지정 보고서 다운로드](/help/dsp/reports/report-download.md)
>* [사용자 지정 보고서 설정](/help/dsp/reports/report-settings.md)
>* 가족 보고서 관련 [FAQ](/help/dsp/reports/faq-reports.md)
>* [캠페인 관리 보기의 성능 보고서 유형](/help/dsp/campaign-management/reports/campaign-reports-about.md)
>* [사용 가능한 보고서 열](/help/dsp/reports/report-columns.md)
>* [정보 [!UICONTROL Report Destinations]](/help/dsp/reports/report-destinations/report-destination-about.md)
