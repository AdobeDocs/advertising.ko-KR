---
title: '[!UICONTROL Custom Creative Report]'
description: 교차 경험 [!UICONTROL Custom Creative Report]을(를) 생성하는 방법을 알아봅니다.
feature: Creative Reporting
exl-id: 13687d9d-6283-40ac-86a2-bb88b9fdfcc3
source-git-commit: 4b780760e5a7a0c3d370054fce8b1c15fbc6802d
workflow-type: tm+mt
source-wordcount: '2019'
ht-degree: 0%

---

# [!UICONTROL Custom Creative Report]

*베타가 닫힘*

[!UICONTROL Custom Creative Report]을(를) 사용하면 모든 광고 경험에 대한 보고서 데이터의 콘텐츠와 배달을 사용자 지정할 수 있습니다.

보고서를 한 번 생성하거나 지정된 기준(예: 15일마다 또는 매월 1일)에 따라 지정된 시간대의 03:00에 매일, 매주 또는 매월 예약할 수 있습니다. 보고서가 생성되면 [!UICONTROL Reports] > [!UICONTROL Custom Reports] 또는 다음 유형의 연결된 [보고서 대상](/help/dsp/reports/report-destinations/report-destination-about.md)에서 다운로드할 수 있습니다.

* [!DNL Amazon Simple Storage Service]&#x200B;([!DNL S3])
* FTP
* FTP SSL <!-- (in beta) -->
* SFTP

## [!UICONTROL Custom Creative Report] 만들기

1. 메인 메뉴에서 **[!UICONTROL Reports]** > **[!UICONTROL Custom Reports]**&#x200B;을(를) 클릭합니다.

1. 오른쪽 상단에서 **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

1. [보고서 설정](#report-settings)을 지정하십시오.

1. **[!UICONTROL Create Custom Report]**&#x200B;을(를) 클릭합니다.

## 보고서 설정 {#report-settings}

**[!UICONTROL Name]:** 보고서 이름입니다. 최대 길이는 180자입니다.

**[!UICONTROL Report Type]:** 보고서 유형: *[!UICONTROL Custom Creative Beta]*.

### [!UICONTROL Report Range] 섹션

이 섹션은 보고서에 포함되는 데이터를 결정합니다. 보고서 일정에 대한 날짜를 설정하려면 &quot;[!UICONTROL Report run schedule]&quot; 섹션을 참조하십시오.

**[!UICONTROL Timezone]:** 보고를 위한 시간대입니다.

**[!UICONTROL Observe Daylight Savings Time]:**&#x200B;은(는) 보고된 시간에 일광 절약 시간을 고려합니다.

**범위:** 데이터를 생성할 날짜 범위입니다. 사용 가능한 일 수는 보고서 및 선택한 차원에 따라 다릅니다. 다음 중 하나를 선택합니다.

* **[!UICONTROL Previous Calendar Week]:** 이전 일정 주에 대한 데이터를 포함합니다.

* **[!UICONTROL Previous Calendar Month]:** 이전 달력의 데이터를 포함합니다.

* **[!UICONTROL Custom Range]:** 특정 시작 날짜와 종료 날짜 사이의 데이터를 포함합니다. 전날까지 데이터를 보고하려면 **[!UICONTROL Present]**&#x200B;을(를) 선택하십시오.

### [!UICONTROL Report Run schedule] 섹션

이 섹션은 보고서가 실행되는 날짜를 결정합니다. 보고서 데이터를 포함할 날짜를 설정하려면 &quot;[!UICONTROL Report range]&quot; 섹션을 참조하십시오.

**\[Schedule\]:** 보고서 생성 시기:

* *[!UICONTROL Immediately]*: 보고서를 보고서 큐에 즉시 추가합니다.

  >[!NOTE]
  >
  >[ 보기에서 ](/help/dsp/reports/report-run-now.md)언제든지 사용자 지정 보고서를 실행[!UICONTROL Reports]할 수도 있습니다.

* *[!UICONTROL On]\&lt;날짜\>:* 계정의 시간대에서 09:00까지 완료하도록 지정된 날짜에 보고서를 실행합니다.

* *[!UICONTROL Recurring]:* 지정한 기간 동안 일정에 따라 보고서를 실행합니다.

   * **\[Schedule\]:** 보고서 실행 빈도:

      * *매일* - N일마다 보고서를 실행합니다. 예를 들어 보고서를 2주(14일)마다 실행하려면 이 옵션을 선택하고 **14**&#x200B;을(를) 입력하십시오.

      * *주별* 보고서를 지정된 요일에 실행합니다. 예를 들어 매주 월요일과 금요일에 보고서를 실행하려면 이 옵션을 선택하고 **월요일**&#x200B;과 **금요일** 옆에 있는 확인란을 선택하십시오.

      * *월별* - 해당 월의 특정 숫자(1일 ~ 30일)에 보고서를 실행합니다. 예를들어 매월 첫째 날에 보고서를 실행하고 이 옵션을 선택한 다음 **1**&#x200B;을(를) 입력합니다.

   * **시작**: 보고서를 실행할 수 있는 첫 번째 날짜입니다. 지정된 일정에 따라 첫 번째 보고서 인스턴스가 이 날짜 이후에 발생할 수 있습니다.

   * **까지**: 보고서 만료일로, 최대 4개월 후에 만료될 수 있습니다. 보고서가 만료되기 전에 지정된 모든 이메일 대상은 만료일 7일 1일 전에 이메일 알림을 받습니다. 보고서를 더 오래 유지하려면 이 날짜를 변경하십시오.

### [!UICONTROL Apply Filters] 섹션

**[!UICONTROL Filter by]:**(선택 사항) 차원을 보고서에 열로 포함할지 여부에 관계없이 데이터를 필터링할 추가 차원입니다. 사용 가능한 필터는 보고서 유형에 따라 다르며 *[!UICONTROL Advertiser]*, *[!UICONTROL Experience]*, *[!UICONTROL Creative Library]* 및 *[!UICONTROL DSP]*<!-- Clarify what this is for, Advertising DSP or whatever DSP the ads were run from? -->을(를) 포함할 수 있습니다.

하나 이상의 필터를 적용하려면 다음을 수행합니다.

* 차원을 선택하고 연산자(*같음* 또는 *같지 않음*)를 선택한 다음 적용 가능한 값을 선택하십시오. 예를 들어 프리롤 광고에 대해서만 데이터를 반환하려면 &quot;[!UICONTROL Ad Type equals Preroll]&quot;을(를) 지정합니다.
* (선택 사항) 필터에 추가 기준을 추가합니다.
* (선택 사항) 각각 하나 이상의 기준을 사용하여 필터를 추가합니다.

### [!UICONTROL Build Your Report] 섹션

**[!UICONTROL Select To Add As Report Headers]:** 보고서에 포함할 데이터 열 또는 헤더입니다. 열을 추가하려면 범주를 확장하고 열 이름 옆에 있는 확인란을 선택합니다. 사용 가능한 열은 보고서에 따라 다르며 사용할 수 없는 모든 지표가 비활성화됩니다. 모든 옵션에 대한 설명은 &quot;[사용 가능한 보고서 열](#report-custom-creative-columns)&quot;을 참조하십시오.

**[!UICONTROL Drag to Re-Order Report Headers Below]:** 열 머리글 순서입니다. 열을 끌어다 놓아 순서를 사용자 지정할 수 있습니다.

**[!UICONTROL Format]:** *[!UICONTROL CSV]*(쉼표로 구분된 값) 또는 *[!UICONTROL Tab]*(탭으로 구분된 값) 형식으로 보고서를 생성할지 여부입니다.

**[!UICONTROL Headers]:** 열 머리글을 *[!UICONTROL Include]* 또는 *[!UICONTROL Do Not Include]*&#x200B;할지 여부입니다.

### [!UICONTROL Multi-Touch Conversion Options] 섹션

**[!UICONTROL Attribution Rule Settings]:** 설정은 보고서 유형에 따라 다릅니다.

* **\[Attribution Type\]:**(Adobe Advertising 전환 추적만 있는 광고주) 보고서 내에서 전환으로 이어지는 일련의 이벤트에서 전환 데이터를 특성화하는 방법:

   * *[!UICONTROL Unique]:*(기본값) 전환 경로에 있는 차원 값(예: 장치 또는 배치)의 횟수를 카운트합니다.

   * *[!UICONTROL Multi-Touch Attribution (MTA)]:* 전환 경로에 있는 차원 값(예: 장치 또는 배치)의 발생 빈도에 따라 각 전환의 크레딧을 배포합니다. 예를 들어 전환 전에 CTV에 8개, 모바일에 2개로 총 10개의 노출이 있었다면 크레딧의 80%(0.8)는 CTV 화면에, 0.2는 모바일에 제공됩니다.

* **\[규칙 유형\]:**(Adobe Advertising 전환 추적 전용 광고주) 보고서 내에서 전환으로 이어지는 일련의 이벤트에서 전환 데이터를 특성화하는 방법. 규칙 간의 차이를 비교하려면 두 개 이상의 규칙을 선택할 수 있습니다.

  >[!NOTE]
  >
  >전환 경로에는 [!DNL Advertising Search, Social, & Commerce]에 구성된 광고주의 노출 또는 클릭 전환 확인 기간 내의 노출 횟수 및 클릭 수가 포함됩니다. 전환 속성 중에 클릭이 노출보다 선호됩니다. 전환 경로에서 모든 클릭은 속성 규칙에 따라 전체 크레딧을 받습니다. 전환 경로에서 클릭이 추적되지 않는 경우에만 노출이 크레딧을 받습니다.

   * *[!UICONTROL Last Event]:* 특성은 전환 경로의 마지막 클릭 또는 노출로 전환됩니다.

   * *[!UICONTROL Weight Last More]:* 특성은 전환 경로의 모든 이벤트로 전환되지만 마지막 이벤트에는 가장 많은 가중치를 주고 이전 이벤트에는 순차적으로 더 적은 가중치를 제공합니다.

   * *[!UICONTROL Even Distribution]:* 특성은 전환 경로의 각 이벤트에 동일하게 전환됩니다.

   * *[!UICONTROL Weight First More]:* 특성은 전환 경로의 모든 이벤트로 전환되지만 첫 번째 이벤트에 가장 많은 가중치를 제공하고 다음 이벤트에 순차적으로 더 적은 가중치를 제공합니다.

   * *[!UICONTROL First Event]:* 특성은 전환 경로의 첫 번째 클릭 또는 노출로 전환됩니다.

   * *[!UICONTROL U-shaped]:* 전환 경로의 모든 이벤트에 대한 전환의 특성을 지정하지만 첫 번째 이벤트와 마지막 이벤트에 가장 많은 가중치를 제공하고 전환 경로 중간에 있는 이벤트에는 순차적으로 더 적은 가중치를 제공합니다.

   * *[!UICONTROL Display Only]:* 특성을 전환 경로에서 마지막 DSP 클릭 또는 노출로 전환했습니다. 여기에는 비디오 및 연결된 TV 광고가 포함되며 [!DNL Advertising Search, Social, & Commerce]개 광고에 대한 클릭은 제외됩니다.

   * *[!UICONTROL Social Only]:* 사용되지 않음

또한 &quot;[Adobe Advertising에 대한 속성 규칙을 계산하는 방법](/help/search-social-commerce/reports/attribution-rules.md)&quot;을 참조하십시오.

**[!UICONTROL Paths as Columns]:** 동일한 장치에서 이전 이벤트가 발생한 경우 보고할 전환 유형입니다. 최대 세 가지 유형을 포함할 수 있습니다. 선택한 각 유형에 대해 각 전환 지표에 대해 별도의 열이 포함되며 지정된 접미사([!UICONTROL (tl)], [!UICONTROL (ct)] 또는 [!UICONTROL (vt)])가 추가됩니다.

* *[!UICONTROL Total (TL) = CT + VT \* VT weight]:* 클릭수(클릭스루의 경우 CT) 및 노출수(뷰스루의 경우 VT)에 속하는 전환을 포함합니다. 노출로 인한 전환에는 지정된 뷰스루 가중치가 곱해집니다. 기본 뷰스루 가중치는 100%입니다. 즉, 노출에 의한 전환은 클릭에 의한 전환 값의 100%로 계산됩니다.

* *[!UICONTROL With Clicks (CT)]:* 클릭에 속하는 전환만 포함합니다.

* *[!UICONTROL Impressions Only (VT)]:* 전환 경로에서 추적된 클릭이 없기 때문에 노출에 기인한 전환만 포함합니다.

### [!UICONTROL Add Report Destinations] 섹션

**[!UICONTROL Destination Type]:** 완료된 보고서 및 오류 알림을 전달할 위치입니다. 보고서를 저장하면 대상 유형을 변경할 수 없습니다.

>[!NOTE]
>
>완료된 보고서는 항상 [!UICONTROL Reports] > [!UICONTROL Custom Reports] 보기에서 다운로드할 수 있습니다.

* *[!UICONTROL None]:* 보고서나 알림을 배달하지 않습니다.

* *[!UICONTROL S3]:* 완료된 보고서를 하나 이상의 [!DNL Amazon Simple Storage Service]&#x200B;([!DNL Amazon S3]) 위치로 보내려면 **[!UICONTROL Destination Name]** 필드에서 선택해야 합니다.

* *[!UICONTROL sFTP]:* 완료된 보고서를 하나 이상의 SFTP 위치로 보내려면 **[!UICONTROL Destination Name]** 필드에서 선택해야 합니다.

* *[!UICONTROL FTP]:* 완료된 보고서를 하나 이상의 FTP 위치로 보내려면 **[!UICONTROL Destination Name]** 필드에서 선택해야 합니다.

* *[!UICONTROL FTP SSL] (현재 Beta):* 완료된 보고서를 하나 이상의 FTP SSL 위치로 보내려면 **[!UICONTROL Destination Name]** 필드에서 선택해야 합니다.

* *[!UICONTROL Email]:* 오류로 인해 보고서가 취소된 경우 완료된 보고서나 알림을 보낼 전자 메일 주소를 지정합니다.

**[!UICONTROL Email]:**(전자 메일 대상 유형만 해당) 각 주소에 주소를 입력하고 **+**&#x200B;을(를) 클릭합니다.

**[!UICONTROL Destination Name]:**(S3, FTP, sFTP 및 FTP SSL 대상 유형만 해당) 사용자 지정 보고서가 전송되는 [보고서 대상](/help/dsp/reports/report-destinations/report-destination-about.md){target="_blank"}의 이름입니다.

* 기존 대상을 지정하려면 목록에서 대상 이름을 선택합니다. 여러 대상 이름을 별도로 선택할 수 있습니다.

* 새 대상을 만들려면 다음 작업을 수행하십시오.

   1. **새 대상 추가**&#x200B;를 클릭합니다.

   1. [보고서 대상 설정](/help/dsp/reports/report-destinations/report-destination-settings.md){target="_blank"}을 입력하고 **저장**&#x200B;을 클릭합니다.

   1. 보고서 설정으로 돌아가서 **대상 이름 새로 고침을 클릭합니다.**

      이제 기존 대상 목록에서 새 대상을 사용할 수 있으며, 원할 경우 보고서에 추가할 수 있습니다.

## 사용 가능한 보고서 열 {#report-custom-creative-columns}

| 지표 유형 | 하위 유형 | 열 이름 | 설명 |
|-----------|-------|-----------|-----------|
| [!UICONTROL Dimension] | [!UICONTROL Ad] | [!UICONTROL Ad Size] | 게시된 광고의 차원입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Ad] | [!UICONTROL Is Default] | 제공된 광고가 경험에 대한 기본 이미지 광고인지 비디오 광고인지 여부. |
| [!UICONTROL Dimension] | [!UICONTROL Ad] | [!UICONTROL Rotation Type] | 광고가 상대적 가중치(*가중*)에 따라 회전되었는지 또는 알고리즘 방식으로 회전되었는지(*알고리즘*) 여부. |
| [!UICONTROL Dimension] | [!UICONTROL Creative] | [!UICONTROL Creative ID] | [!UICONTROL Creative]이(가) 크리에이티브에 할당한 ID입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Creative] | [!UICONTROL Creative Name] | 크리에이티브 이름. |
| [!UICONTROL Dimension] | [!UICONTROL Creative] | [!UICONTROL Creative Type] | 크리에이티브 유형(예: [!UICONTROL HTML5]). |
| [!UICONTROL Dimension] | [!UICONTROL Creative] | [!UICONTROL Parent Creative ID] | [!UICONTROL Creative]이(가) 상위 Creative에 할당한 ID입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Creative] | [!UICONTROL Parent Creative Name] | 상위 문안의 이름입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Creative] | [!UICONTROL Parent Creative Type] | 상위 크리에이티브 유형(예: [!UICONTROL HTML5]). |
| [!UICONTROL Dimension] | [!UICONTROL Click Events] | [!UICONTROL Ad Link] | 랜딩 페이지 URL. |
| [!UICONTROL Dimension] | [!UICONTROL Click Events] | [!UICONTROL Click Type] | 사용자 인터랙션의 특정 유형. |
| [!UICONTROL Dimension] | [!UICONTROL Click Events] | [!UICONTROL Direction] | 크리에이티브 경험 내에서 사용자의 클릭 인터랙션에 대한 방향 흐름 또는 탐색 경로. |
| [!UICONTROL Dimension] | [!UICONTROL Device] | [!UICONTROL Device Browser] | 광고가 표시된 브라우저(예: [!UICONTROL Chrome] 또는 [!UICONTROL Firefox]). |
| [!UICONTROL Dimension] | [!UICONTROL Device] | [!UICONTROL Device OS] | 광고가 표시된 운영 체제(예: [!UICONTROL Windows]). |
| [!UICONTROL Dimension] | [!UICONTROL Device] | [!UICONTROL Device Type] | 광고가 표시된 장치의 유형입니다(예: [!UICONTROL Desktop]). |
| [!UICONTROL Dimension] | [!UICONTROL DSP] | [!UICONTROL DSP Name] | 광고가 실행된 DSP의 이름입니다. |
| [!UICONTROL Dimension] | [!UICONTROL DSP] | [!UICONTROL DSP Placement ID] | 광고가 실행된 배치 ID입니다. |
| [!UICONTROL Dimension] | [!UICONTROL DSP] | [!UICONTROL DSP Placement Name] | 광고가 실행된 배치의 이름입니다. |
| [!UICONTROL Dimension] | [!UICONTROL DSP] | [!UICONTROL DSP Site ID] | 광고가 실행된 사이트의 ID. |
| [!UICONTROL Dimension] | [!UICONTROL DSP] | [!UICONTROL DSP Site Name] | 광고가 실행된 사이트의 이름입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Experiences] | [!UICONTROL Ad Tag Id] | [!UICONTROL Creative]이(가) 광고 경험 태그에 할당한 ID입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Experiences] | [!UICONTROL Advertiser Name] | 광고주의 이름입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Experiences] | [!UICONTROL Date/Time] | 이벤트 날짜 및 시간입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Experiences] | [!UICONTROL Experience ID] | [!UICONTROL Creative]이(가) 경험에 할당한 ID입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Experiences] | [!UICONTROL Experience Name] | 경험의 이름입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Experiences] | [!UICONTROL Targeting Branch Value] | 사용자에게 제공된 크리에이티브 경험 변형을 결정하는 타겟팅 결정 트리를 통한 특정 경로. |
| [!UICONTROL Dimension] | [!UICONTROL Experiences] | [!UICONTROL Trafficking Line] | 광고 태그의 이름입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Geo] | [!UICONTROL City] | 보고된 데이터가 속하는 도시입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Geo] | [!UICONTROL Country Code] | 보고된 데이터가 속하는 국가의 국가 코드입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Geo] | [!UICONTROL DMA] | 보고된 데이터가 속하는 DMA(Designated Market Area). |
| [!UICONTROL Dimension] | [!UICONTROL Geo] | [!UICONTROL State Code] | 보고된 데이터가 속하는 상태의 상태 코드입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Geo] | [!UICONTROL Zip Code] | 보고된 데이터가 속하는 우편 번호입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Product] | [!UICONTROL Category ID] | (동적 광고) 대상 제품 범주 ID입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Product] | [!UICONTROL Category Name] | (동적 광고) 대상 제품 범주 이름입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Product] | [!UICONTROL Creative Attribute 1] | (Dynamic ads) 첫 번째 크리에이티브 속성입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Product] | [!UICONTROL Creative Attribute 2] | (Dynamic ads) 두 번째 크리에이티브 속성입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Product] | [!UICONTROL Creative Attribute 3] | (Dynamic ads) 세 번째 크리에이티브 속성입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Product] | [!UICONTROL Creative Attribute 4] | (Dynamic ads) 네 번째 크리에이티브 속성입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Product] | [!UICONTROL Creative Attribute 5] | (Dynamic ads) 다섯 번째 크리에이티브 속성입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Product] | [!UICONTROL Product ID] | (동적 광고) 대상 제품 ID입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Product] | [!UICONTROL Product Name] | (Dynamic ads) 대상 제품 이름입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Segment] | [!UICONTROL Matched Audience Segment ID] | 광고 테마와 일치하는 최대 5개의 사용자 세그먼트에 대한 ID입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Segment] | [!UICONTROL Pixel Segment ID] | 보고된 데이터가 속하는 리타겟팅 픽셀의 ID입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Segment] | [!UICONTROL Pixel Segment Name] | 보고된 데이터가 속하는 재타겟팅 픽셀의 이름입니다. |
| [!UICONTROL Dimension] | [!UICONTROL Segment] | [!UICONTROL Segment Values] | 보고된 데이터가 속하는 대상 세그먼트의 속성입니다. |
| [!UICONTROL Metric] | [!UICONTROL Standard Metrics] | [!UICONTROL Clicks] | 광고의 모든 클릭 수 합계입니다. |
| [!UICONTROL Metric] | [!UICONTROL Standard Metrics] | [!UICONTROL CTR] | 클릭스루 비율(광고 노출 횟수로 나눈 클릭 수의 백분율)입니다. |
| [!UICONTROL Metric] | [!UICONTROL Standard Metrics] | [!UICONTROL Engagement Rate] | 사용자 참여를 유도한 제공된 노출 횟수의 비율입니다. |
| [!UICONTROL Metric] | [!UICONTROL Standard Metrics] | [!UICONTROL Engagements] | 제공된 광고의 상호 작용 수입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL Impressions] | 총 광고 노출 횟수. |
| [!UICONTROL Metric] | [!UICONTROL Standard Metrics] | [!UICONTROL Media Match Rate] | 재타겟팅된 쿠키가 있는 노출 비율입니다. |
| [!UICONTROL Metric] | [!UICONTROL Standard Metrics] | [!UICONTROL Product Clicks] | (동적 광고만 해당) 제품 광고에 대한 모든 클릭의 합계입니다. 제품이 null이면 이 값은 0(영)입니다. |
| [!UICONTROL Metric] | [!UICONTROL Standard Metrics] | [!UICONTROL Product Conversion] | (동적 광고만 해당) 제품 광고에 대한 모든 전환의 합계입니다. 제품이 null이면 이 값은 0(영)입니다. |
| [!UICONTROL Metric] | [!UICONTROL Standard Metrics] | [!UICONTROL Product Conversion Rate] | (동적 광고만 해당) 전환을 초래한 제품에 대한 광고의 비율입니다. 제품이 null이면 이 값은 0(영)입니다. |
| [!UICONTROL Metric] | [!UICONTROL Standard Metrics] | [!UICONTROL Product CTR] | (동적 광고만 해당) 제품 광고에 대한 클릭스루 비율(광고 노출 횟수로 나눈 클릭 수) 제품이 null이면 이 값은 0(영)입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL Product Impressions] | (동적 광고만 해당) 제품에 대한 총 노출 횟수입니다. 제품이 null이면 이 값은 0(영)입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL Product Revenue] | (동적 광고만 해당) 제품에 대해 제공된 광고의 총 매출액. 제품이 null이면 이 값은 0(영)입니다. |
| [!UICONTROL Metrics] | [!UICONTROL Standard Metrics] | [!UICONTROL Revenue] | 제공된 광고의 총 매출액. |
| [!UICONTROL Conversion Metrics] | [보고서 설정에서 광고주별로 그룹화됨] | [광고주별 전환] | 지정된 광고주별 전환 지표 또는 Adobe Analytics 이벤트에 대한 합계입니다. |
| [!UICONTROL Custom Goals] | [보고서 설정에서 광고주별로 그룹화됨] | [광고주별 사용자 지정 목표] | (Advertising DSP을 사용하는 광고주) 지정된 [Advertising DSP 사용자 지정 목표](/help/dsp/optimization/custom-goal.md)에 포함된 모든 전환의 가중 합계입니다. |

{style="table-layout:auto"}

>[!MORELIKETHIS]
>
>* [경험 수준 성과 보고서](/help/creative/experiences/experience-performance-details.md)
>* [DSP 사용자 지정 보고서 정보](/help/dsp/reports/report-about.md){target="_blank"}
>* [정보 [!UICONTROL report destinations]](/help/dsp/reports/report-destinations/report-destination-about.md){target="_blank"}
