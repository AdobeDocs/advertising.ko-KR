---
title: 사용자 지정 보고서 설정
description: 사용자 지정 보고서 설정에 대한 설명을 참조하십시오.
feature: DSP Custom Reports
exl-id: 0e9e4332-3c10-44b0-b315-691b22dfb3c7
source-git-commit: e517dd5f5fa283ff8a2f57728612937148889732
workflow-type: tm+mt
source-wordcount: '1261'
ht-degree: 0%

---

# 사용자 지정 보고서 설정

**[!UICONTROL Name]** 보고서 이름입니다. 최대 길이는 180자입니다.

**[!UICONTROL Report Type]** 보고서 유형: *[!UICONTROL Custom]*(사용 가능한 옵션 포함), *[!UICONTROL Billing]*, *[!UICONTROL Conversion]*, *[!UICONTROL Device]*, *[!UICONTROL Frequency (by Impression)]*, *[!UICONTROL Frequency (by App/Site)]*, *[!UICONTROL Geo]*, *[!UICONTROL Margin]*, *[!UICONTROL Media Performance]*, *[!UICONTROL Segment]*, *[!UICONTROL Site]*, *[!UICONTROL Household Reach & Frequency]* 또는 *[!UICONTROL Household Conversions]*.

## [!UICONTROL Apply Filters] 섹션

**[!UICONTROL Timezone]:** 보고를 위한 시간대입니다.

**[!UICONTROL Observe Daylight Savings Time]:**&#x200B;은(는) 보고된 시간에 일광 절약 시간을 고려합니다.

**\[Date Range\]:** 데이터를 생성할 날짜 범위입니다. 사용 가능한 일 수는 보고서 및 선택한 차원에 따라 다릅니다. 다음 중 하나를 선택합니다.

* **[!UICONTROL Previous N days]:** 오늘 이전 특정 일수의 데이터를 포함합니다.

* **[!UICONTROL Custom]:** 특정 시작 날짜와 종료 날짜 사이의 데이터를 포함합니다. 전날까지 데이터를 보고하려면 **[!UICONTROL Present]**&#x200B;을(를) 선택하십시오.

* **[!UICONTROL Last Calendar Month]:** 이전 달력의 데이터를 포함합니다.

**[!UICONTROL Add Filters]:**(선택 사항) 차원을 보고서에 열로 포함할지 여부에 관계없이 데이터를 필터링할 추가 차원입니다. 사용 가능한 필터는 보고서 유형에 따라 다르며 *[!UICONTROL Account]*\*, *[!UICONTROL Ad Type]*, *[!UICONTROL Ads]*, *[!UICONTROL Advertiser]*, *[!UICONTROL Campaign]*, *[!UICONTROL Country]*, * *[!UICONTROL Package]*, *[!UICONTROL Placement]*, *[!UICONTROL Video]* 및 *[!UICONTROL Video Duration]*&#x200B;을(를) 포함할 수 있습니다.

\* *[!UICONTROL Account]*&#x200B;은(는) 조직이 [교차 계정 보고](report-about.md#cross-account-reporting)에 대해 구성된 경우에만 다음 보고서 유형에 사용할 수 있습니다. [!UICONTROL Custom], [!UICONTROL Site], [!UICONTROL Segment], [!UICONTROL Geo], [!UICONTROL Device], [!UICONTROL Frequency (by Impression)] 및 [!UICONTROL Conversion]. 교차 계정 보고에 대한 자세한 내용은 Adobe 계정 팀에 문의하십시오.

하나 이상의 필터를 적용하려면 다음을 수행합니다.

* 차원을 선택하고 연산자(*같음* 또는 *같지 않음*)를 선택한 다음 적용 가능한 값을 선택하십시오. 예를 들어 프리롤 광고에 대해서만 데이터를 반환하려면 &quot;[!UICONTROL Ad Type equals Preroll]&quot;을(를) 지정합니다.
* (선택 사항) 필터에 추가 기준을 추가합니다.
* (선택 사항) 각각 하나 이상의 기준을 사용하여 필터를 추가합니다.

## [!UICONTROL Build Your Report] 섹션

**[!UICONTROL Select To Add As Report Headers]:** 보고서에 포함할 데이터 열 또는 헤더입니다. 열을 추가하려면 범주를 확장하고 열 이름 옆에 있는 확인란을 선택합니다. 사용 가능한 열은 보고서에 따라 다르며 사용할 수 없는 모든 지표가 비활성화됩니다. 사용 가능한 데이터 범주는 다음과 같습니다.

* [!UICONTROL Dimensions]

  >[!NOTE]
  >
  > [!UICONTROL Household Reach & Frequency] 보고서에는 하나의 차원만 포함될 수 있습니다.

* [!UICONTROL Metrics]

  >[!NOTE]
  >
  >[!UICONTROL Household Reach & Frequency] 보고서에는 겹치는 지표 또는 겹치지 않는 지표가 포함될 수 있지만 둘 다 포함할 수는 없습니다.

* [!UICONTROL Conversion Metrics](광고주별로 정렬됨)

* [!UICONTROL Custom Goals](광고주별로 정렬됨)

모든 옵션에 대한 설명은 &quot;[사용 가능한 보고서 열](report-columns.md)&quot;을 참조하십시오.

**[!UICONTROL Drag to Re-Order Report Headers Below]:** 열 머리글 순서입니다. 열을 끌어다 놓아 순서를 사용자 지정할 수 있습니다.

**[!UICONTROL Format]:** *[!UICONTROL CSV]*(쉼표로 구분된 값) 또는 *[!UICONTROL Tab]*(탭으로 구분된 값) 형식으로 보고서를 생성할지 여부입니다.

**[!UICONTROL Headers]:** 열 머리글을 *[!UICONTROL Include]* 또는 *[!UICONTROL Do Not Include]*&#x200B;할지 여부입니다.

## [!UICONTROL Multi-Touch Conversion Options] 섹션

**[!UICONTROL Attribution Rule Settings]:** 설정은 보고서 유형에 따라 다릅니다.

* **\[속성 유형\]:**([!UICONTROL Conversion Metrics] 또는 [!UICONTROL Custom Goals] 열이 있는 [!UICONTROL Household Conversion] 보고서, Adobe Advertising 전환 추적만 있는 광고주) 보고서 내에서 전환을 유도하는 일련의 이벤트에서 전환 데이터를 특성화하는 방법:

   * *[!UICONTROL Unique]:*(기본값) 전환 경로에 있는 차원 값(예: 장치 또는 배치)의 횟수를 카운트합니다.

   * *[!UICONTROL Multi-Touch Attribution (MTA)]:* 전환 경로에 있는 차원 값(예: 장치 또는 배치)의 발생 빈도에 따라 각 전환의 크레딧을 배포합니다. 예를 들어 전환 전에 CTV에 8개, 모바일에 2개로 총 10개의 노출이 있었다면 크레딧의 80%(0.8)는 CTV 화면에, 0.2는 모바일에 제공됩니다.

* **\[규칙 유형\]:**(모든 [!UICONTROL Custom], [!UICONTROL Conversion], [!UICONTROL Device], [!UICONTROL Geo], [!UICONTROL Segment] 및 [!UICONTROL Site] 보고서에 [!UICONTROL Conversion Metrics] 또는 [!UICONTROL Custom Goals] 열이 있음, Adobe Advertising 전환 추적 전용 광고주) 보고서 내에서 전환으로 이어지는 일련의 이벤트에서 전환 데이터를 특성화하는 방법을 알아봅니다. 규칙 간의 차이를 비교하려면 두 개 이상의 규칙을 선택할 수 있습니다.

  >[!NOTE]
  >
  >전환 경로에는 [!DNL Advertising Search, Social, & Commerce]에 구성된 광고주의 노출 또는 클릭 전환 확인 기간 내의 노출 횟수 및 클릭 수가 포함됩니다. 전환 속성 중에 클릭이 노출보다 선호됩니다. 전환 경로에서 모든 클릭은 속성 규칙에 따라 전체 크레딧을 받습니다. 전환 경로에서 클릭이 추적되지 않는 경우에만 노출이 크레딧을 받습니다.

   * *[!UICONTROL Last Event]:* 특성은 전환 경로의 마지막 클릭 또는 노출로 전환됩니다.

   * *[!UICONTROL Weight Last More]:* 특성은 전환 경로의 모든 이벤트로 전환되지만 마지막 이벤트에는 가장 많은 가중치를 주고 이전 이벤트에는 순차적으로 더 적은 가중치를 제공합니다.

   * *[!UICONTROL Even Distribution]:* 특성은 전환 경로의 각 이벤트에 동일하게 전환됩니다.

   * *[!UICONTROL Weight First More]:* 특성은 전환 경로의 모든 이벤트로 전환되지만 첫 번째 이벤트에 가장 많은 가중치를 제공하고 다음 이벤트에 순차적으로 더 적은 가중치를 제공합니다.

   * *[!UICONTROL First Event]:* 특성은 전환 경로의 첫 번째 클릭 또는 노출로 전환됩니다.

   * *[!UICONTROL U-shaped]:* 전환 경로의 모든 이벤트에 대한 전환의 특성을 지정하지만 첫 번째 이벤트와 마지막 이벤트에 가장 많은 가중치를 제공하고 전환 경로 중간에 있는 이벤트에는 순차적으로 더 적은 가중치를 제공합니다.

   * *[!UICONTROL Display Only]:* 특성 변환이 변환 경로의 마지막 DSP 클릭 또는 노출로 변경되었습니다. 여기에는 비디오 및 연결된 TV 광고가 포함되며 [!DNL Advertising Search, Social, & Commerce]개 광고에 대한 클릭은 제외됩니다.

   * *[!UICONTROL Social Only]:* 사용되지 않음

  <!-- See also [How Attribution Rules Are Calculated for Adobe Advertising](). -->

* **전환 확인:**([!UICONTROL Conversion Metrics] 또는 [!UICONTROL Custom Goals] 열이 있는 [!UICONTROL Household Conversion] 보고서, Adobe Advertising 전환 추적만 있는 광고주) 보고서 내에서 전환 이벤트가 해당 이벤트에 귀속될 수 있는 노출 이벤트 후 최대 일 수입니다. 기본값은 *[!UICONTROL 30 days]*&#x200B;이고 최대값은 92일입니다.

**[!UICONTROL Paths as Columns]:**(모든 [!UICONTROL Custom], [!UICONTROL Conversion], [!UICONTROL Device], [!UICONTROL Geo], [!UICONTROL Segment] 및 [!UICONTROL Site] 보고서에 [!UICONTROL Conversion Metrics] 또는 [!UICONTROL Custom Goals] 열이 있음) 이전 이벤트가 동일한 장치에서 발생한 경우 보고할 전환 유형. 최대 세 가지 유형을 포함할 수 있습니다. 선택한 각 유형에 대해 각 전환 지표에 대해 별도의 열이 포함되며 지정된 접미사([!UICONTROL (tl)], [!UICONTROL (ct)] 또는 [!UICONTROL (vt)])가 추가됩니다.

* *[!UICONTROL Total (TL) = CT + VT \* VT weight]:* 클릭수(클릭스루의 경우 CT) 및 노출수(뷰스루의 경우 VT)에 속하는 전환을 포함합니다. 노출로 인한 전환에는 지정된 뷰스루 가중치가 곱해집니다. 기본 뷰스루 가중치는 100%입니다. 즉, 노출에 의한 전환은 클릭에 의한 전환 값의 100%로 계산됩니다.

* *[!UICONTROL With Clicks (CT)]:* 클릭에 속하는 전환만 포함합니다.

* *[!UICONTROL Impressions Only (VT)]:* 전환 경로에서 추적된 클릭이 없기 때문에 노출에 기인한 전환만 포함합니다.

**[!UICONTROL Conversion Reporting Based On]:** 전환 데이터를 보고하는 방법:

* *[!UICONTROL Conversion Timestamp]:*(기본값) 전환은 전환 날짜와 연결됩니다.

* *[!UICONTROL Event Timestamp]:* 전환은 지정된 [!UICONTROL Attribution Rule Settings]에 의해 결정된 대로 전환을 초래한 노출 또는 클릭의 날짜를 기준으로 보고됩니다.

## [!UICONTROL Add Report Destinations] 섹션

**[!UICONTROL Destination Type]:** 다음 대상 유형 중 하나를 선택하십시오.

* *[!UICONTROL S3]:* 완료된 보고서를 하나 이상의 [!DNL Amazon Simple Storage Service]([!DNL Amazon S3]) 위치로 보내려면 **[!UICONTROL Destination Name]** 필드에 지정해야 합니다.
* *[!UICONTROL sFTP]:* 완료된 보고서를 하나 이상의 SFTP 위치로 보내려면 **[!UICONTROL Destination Name]** 필드에 지정해야 합니다.
* *[!UICONTROL FTP]:* 완료된 보고서를 하나 이상의 FTP 위치로 보내려면 **[!UICONTROL Destination Name]** 필드에 지정해야 합니다.
* *[!UICONTROL FTP SSL](현재 Beta):* 완료된 보고서를 하나 이상의 FTP SSL 위치로 보내려면 **[!UICONTROL Destination Name]** 필드에 지정해야 합니다.
* *[!UICONTROL Email]:* 오류로 인해 보고서가 취소된 경우 완료된 보고서나 알림을 보낼 전자 메일 주소를 지정합니다.

>[!NOTE]
>
> 보고서를 저장하면 대상 유형을 변경할 수 없습니다.

**[!UICONTROL Email]:**(전자 메일 대상 유형만 해당) 각 주소에 주소를 입력하고 **+**&#x200B;을(를) 클릭합니다.

**[!UICONTROL Destination Name]:**(S3, FTP, sFTP 및 FTP SSL 대상 유형만 해당) 사용자 지정 보고서가 전송되는 보고서 대상의 이름입니다.

* 기존 대상을 지정하려면 목록에서 대상 이름을 선택합니다. 여러 대상 이름을 별도로 선택할 수 있습니다.

* 새 대상을 만들려면 다음 작업을 수행하십시오.

   1. **새 대상 추가**&#x200B;를 클릭합니다.

   1. [보고서 대상 설정](/help/dsp/reports/report-destinations/report-destination-settings.md)을 입력하고 **저장**&#x200B;을 클릭합니다.

   1. 보고서 설정으로 돌아가서 **대상 이름 새로 고침을 클릭합니다.**

      이제 기존 대상 목록에서 새 대상을 사용할 수 있으며, 원할 경우 보고서에 추가할 수 있습니다.

**[!UICONTROL Frequency]:**(각 [!UICONTROL Destination Name]에 대해) 보고서를 대상으로 보내는 빈도: *[!UICONTROL Once]*, *[!UICONTROL Daily]*, *[!UICONTROL Weekly]* 또는 *[!UICONTROL Monthly]*.

보고서를 생성할 **[!UICONTROL Start Day]:**(*[!UICONTROL Weekly]* 또는 *[!UICONTROL Monthly]*&#x200B;의 [!UICONTROL Frequency]을(를) 가진 각 [!UICONTROL Destination Name]에 대해). 주별 보고서의 경우 요일을 선택합니다. 월별 보고서의 경우 해당 월의 숫자 일을 선택합니다.

## [!UICONTROL Save Report] 섹션

**[!UICONTROL When to Generate]:** 보고서 생성 시기: *[!UICONTROL On Schedule]* 또는 *[!UICONTROL Run Now]*. 예약된 보고서는 계정의 시간대에서 09:00까지 제공됩니다.

**[!UICONTROL End Date]:** 최대 4개월 후의 보고서 만료일입니다. 보고서가 만료되기 전에 지정된 모든 이메일 수신자는 만료 날짜로부터 7일 1일 전에 이메일 경고를 수신하게 됩니다. 보고서를 더 오래 유지하려면 보고서 설정에서 만료 날짜를 변경합니다.

>[!NOTE]
>
>[!UICONTROL Reports] 보기에서 [언제든지 사용자 지정 보고서를 실행](report-run-now.md)할 수 있습니다.

>[!MORELIKETHIS]
>
>* [사용자 지정 보고서 정보](/help/dsp/reports/report-about.md)
>* [사용자 지정 보고서 만들기](/help/dsp/reports/report-create.md)
>* [사용자 지정 보고서 복제](/help/dsp/reports/report-copy.md)
>* [사용자 지정 보고서 편집](/help/dsp/reports/report-edit.md)
>* [사용자 지정 보고서 실행](/help/dsp/reports/report-run-now.md)
>* [사용자 지정 보고서 설정](/help/dsp/reports/report-settings.md)
>* [보고서 대상 정보](/help/dsp/reports/report-destinations/report-destination-about.md)
>* [사용 가능한 보고서 열](/help/dsp/reports/report-columns.md)
