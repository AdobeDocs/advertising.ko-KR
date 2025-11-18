---
title: 사용자 정의 보고서 관리
description: 교차 경험 [!UICONTROL Custom Creative Report]을(를) 생성하고 관리하는 방법을 알아봅니다.
feature: Creative Reporting
source-git-commit: 41b8d295436bdbe6cea402e5bb234caa7a36f4df
workflow-type: tm+mt
source-wordcount: '1477'
ht-degree: 0%

---

# [!UICONTROL Manage custom reports]

사용자 지정 보고서를 작성, 복제, 편집, 실행, 다운로드 및 삭제할 수 있습니다.

## 사용자 지정 보고서 만들기 {#report-create}

1. 메인 메뉴에서 **[!UICONTROL Reports]** > **[!UICONTROL Custom Reports]**&#x200B;을(를) 클릭합니다.

1. 오른쪽 상단에서 **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

1. [보고서 설정](#report-settings)을 지정하십시오.

1. **[!UICONTROL Create Custom Report]**&#x200B;을(를) 클릭합니다.

## 사용자 지정 보고서 복제

사용자 지정 보고서를 복제하여 유사한 설정으로 새 보고서를 만듭니다.

1. 메인 메뉴에서 **[!UICONTROL Reports]** > **[!UICONTROL Custom Reports]**&#x200B;을(를) 클릭합니다.

1. 보고서 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Copy]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 필요에 따라 [보고서 설정](#report-settings.md)을 편집합니다.

   보고서 이름은 기본적으로 &quot;\&lt;*기존 보고서 이름*\> \#2&quot;(또는 시퀀스의 다음 번호)입니다.

## 사용자 지정 보고서 편집 {#report-edit}

1. 메인 메뉴에서 **[!UICONTROL Reports]** > **[!UICONTROL Custom Reports]**&#x200B;을(를) 클릭합니다.

1. 보고서 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. [보고서 설정](#report-settings.md)을(를) 편집합니다.

1. **[!UICONTROL Edit Custom Report]**&#x200B;을(를) 클릭합니다.

## 사용자 지정 보고서 실행 {#report-run-now}

만료되지 않았고 현재 실행 중이 아닌 모든 보고서를 실행할 수 있습니다.

>[!NOTE]
>
>사용자 지정 보고서는 [만들기](#report-create) 또는 [편집](#report-edit)할 때 실행할 수도 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Reports]** > **[!UICONTROL Custom Reports]**&#x200B;을(를) 클릭합니다.

1. 보고서 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Run Now]**&#x200B;을(를) 클릭합니다.

   보고서가 완료되면 보고서 설정에 지정된 대상으로 전송됩니다.

## 사용자 정의 보고서 다운로드

상태가 &quot;[!UICONTROL Ready to Download]&quot; 또는 &quot;[!UICONTROL Completed]&quot;인 지난 4개월 동안의 완료된 보고서 인스턴스를 다운로드할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Reports]** > **[!UICONTROL Custom Reports]**&#x200B;을(를) 클릭합니다.

1. 보고서 행의 [!UICONTROL Download Report] 열에서 다음을 수행합니다.

   * 보고서의 최신 인스턴스를 다운로드하려면 **[!UICONTROL Download]**&#x200B;을(를) 클릭하십시오.

   * (여러 인스턴스가 있는 보고서) ![&#x200B; 옆에 있는 &#x200B;](/help/dsp/assets/chevron-down.png "아래쪽 화살표")아래쪽 화살표[!UICONTROL Download]를 클릭한 다음 다운로드할 보고서의 완료 날짜를 클릭합니다. 다운로드 가능한 보고서 인스턴스는 다운로드 아이콘(![다운로드 아이콘](/help/dsp/assets/indicator-downloadable.png "다운로드 아이콘"))으로 표시됩니다.

     사용 가능한 인스턴스가 많으면 필요한 경우 목록 맨 아래의 **[!UICONTROL Load More]**&#x200B;을(를) 클릭합니다.

     보고서가 같은 날에 여러 번 실행되면 해당 날짜의 보고서 인스턴스가 시간 순서대로 나열되며 가장 최근 인스턴스가 맨 위에 표시됩니다.

     실패한 보고서 작업은 오류 아이콘(![오류 표시기](/help/dsp/assets/indicator-critical.png "오류 표시기"))으로 표시되어 다운로드할 수 없습니다. 오류 설명을 보려면 커서를 오류 아이콘 위에 놓습니다.

## 사용자 지정 보고서 삭제

1. 메인 메뉴에서 **[!UICONTROL Reports]** > **[!UICONTROL Custom Reports]**&#x200B;을(를) 클릭합니다.

1. 보고서 이름 옆에 있는 **[!UICONTROL ...]** > **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

## 보고서 설정 {#report-settings}

**[!UICONTROL Name]:** 보고서 이름입니다. 최대 길이는 180자입니다.

**[!UICONTROL Report Type]:** 보고서 유형입니다.

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
  >[&#x200B; 보기에서 &#x200B;](#report-run-now)언제든지 사용자 지정 보고서를 실행[!UICONTROL Reports]할 수도 있습니다.

* *[!UICONTROL On]\&lt;날짜\>:* 계정의 시간대에서 09:00까지 완료되도록 지정된 날짜에 보고서를 실행합니다.

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

**[!UICONTROL Select To Add As Report Headers]:** 보고서에 포함할 데이터 열 또는 헤더입니다. 열을 추가하려면 범주를 확장하고 열 이름 옆에 있는 확인란을 선택합니다. 사용 가능한 열은 보고서에 따라 다르며 사용할 수 없는 모든 지표가 비활성화됩니다.<!-- Add back once I have this completed, and reconsider wording of link/anchor:  See "[Available Report Columns](#report-custom-creative-columns)" for descriptions of all options. -->

**[!UICONTROL Drag to Re-Order Report Headers Below]:** 열 머리글 순서입니다. 열을 끌어다 놓아 순서를 사용자 지정할 수 있습니다.

**[!UICONTROL Format]:** *[!UICONTROL CSV]*(쉼표로 구분된 값) 또는 *[!UICONTROL Tab]*(탭으로 구분된 값) 형식으로 보고서를 생성할지 여부입니다.

**[!UICONTROL Headers]:** 열 머리글을 *[!UICONTROL Include]* 또는 *[!UICONTROL Do Not Include]*&#x200B;할지 여부입니다.

### [!UICONTROL Multi-Touch Conversion Options] 섹션

**[!UICONTROL Attribution Rule Settings]:** 설정은 보고서 유형에 따라 다릅니다.

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


<!-- This needs a lot of updating for new report:

## Available Report Columns {#report-custom-creative-columns}

|Metric Type|Subtype|Column Name|Description|
|-----------|-------|-----------|-----------|
|\[Dimension\]|[!UICONTROL Ad]|[!UICONTROL Ad Size]|The dimensions of the published ad.|
|\[Dimension\]|[!UICONTROL Ad]|[!UICONTROL Is Default]|Whether the served ad was a default image ad or video ad for the experience.|
|\[Dimension\]|[!UICONTROL Ad]|[!UICONTROL Rotation Type]| Whether ads were rotated algorithmically (*Algorithmic*), in a specified sequence (*Sequenced*), or according to relative weights (*Weighted*).|
|\[Dimension\]|[!UICONTROL Creative]|[!UICONTROL Creative ID]| The ID that [!UICONTROL Creative] assigned to the creative.|
|\[Dimension\]|[!UICONTROL Creative]|[!UICONTROL Creative Name]| The name of the creative.|
|\[Dimension\]|[!UICONTROL Creative]|[!UICONTROL Creative Type]| The type of creative (such as [!UICONTROL HTML5]).|
|\[Dimension\]|[!UICONTROL Creative]|[!UICONTROL Parent Creative ID]| The ID that [!UICONTROL Creative] assigned to the parent creative.|
|\[Dimension\]|[!UICONTROL Creative]|[!UICONTROL Parent Creative Name]| The name of the parent creative.|
|\[Dimension\]|[!UICONTROL Creative]|[!UICONTROL Parent Creative Type]| The type of parent creative (such as [!UICONTROL HTML5]).|
|\[Dimension\]|[!UICONTROL Click Events]|[!UICONTROL Ad Link]| The landing page URL.|
|\[Dimension\]|[!UICONTROL Click Events]|[!UICONTROL Click Type]| The specific type of user interaction.|
|\[Dimension\]|[!UICONTROL Click Events]|[!UICONTROL Direction]| The directional flow or navigation path of the user's click interaction within the creative experience. |
|\[Dimension\]|[!UICONTROL Custom Attributes]|[!UICONTROL Custom Attribute 1]| The value of Attribute 1 in the pixel tag, when it was included.|
|\[Dimension\]|[!UICONTROL Custom Attributes]|[!UICONTROL Custom Attribute 2]| The value of Attribute 2 in the pixel tag, when it was included.|
|\[Dimension\]|[!UICONTROL Custom Attributes]|[!UICONTROL Custom Attribute 3]| The value of Attribute 3 in the pixel tag, when it was included.|
|\[Dimension\]|[!UICONTROL Custom Attributes]|[!UICONTROL Custom Attribute 4]| The value of Attribute 3 in the pixel tag, when it was included.|
|\[Dimension\]|[!UICONTROL Custom Attributes]|[!UICONTROL Custom Attribute 5]| The value of Attribute 5 in the pixel tag, when it was included.|
|\[Dimension\]|[!UICONTROL Device]|[!UICONTROL Device Browser]|The browser in which the ad was shown (such as [!UICONTROL Chrome] or [!UICONTROL Firefox]).|
|\[Dimension\]|[!UICONTROL Device]|[!UICONTROL Device OS]|The operating system on which the ad was shown (such as [!UICONTROL Windows]).|
|\[Dimension\]|[!UICONTROL Device]|[!UICONTROL Device Type]|The type of device on which the ad was shown (such as [!UICONTROL Desktop]).|
|\[Dimension\]|[!UICONTROL DSP]|[!UICONTROL DSP Name]| The name of the DSP on which ads were run. |
|\[Dimension\]|[!UICONTROL DSP]|[!UICONTROL DSP Placement ID]| The ID of the placement for which ads were run. |
|\[Dimension\]|[!UICONTROL DSP]|[!UICONTROL DSP Placement Name]| The name of the placement for which ads were run. |
|\[Dimension\]|[!UICONTROL DSP]|[!UICONTROL DSP Site ID]| The ID of the site on which ads were run.|
|\[Dimension\]|[!UICONTROL DSP]|[!UICONTROL DSP Site Name]| The name of the site on which ads were run. |
|\[Dimension\]|[!UICONTROL Experiences]|[!UICONTROL Ad Tag Id]|The ID that [!UICONTROL Creative] assigned to the ad experience tag.|
|\[Dimension\]|[!UICONTROL Experiences]|[!UICONTROL Advertiser Name]| The name of the advertiser.|
|\[Dimension\]|[!UICONTROL Experiences]|[!UICONTROL Date/Time]|The date and time of the event.|
|\[Dimension\]|[!UICONTROL Experiences]|[!UICONTROL Experience ID]| The ID that [!UICONTROL Creative] assigned to the experience.|
|\[Dimension\]|[!UICONTROL Experiences]|[!UICONTROL Experience Name]| The name of the experience.|
|\[Dimension\]|[!UICONTROL Experiences]|[!UICONTROL Targeting Branch Value]| The specific path through the targeting decision tree that determined which creative experience variant was served to the user.|
|\[Dimension\]|[!UICONTROL Experiences]|[!UICONTROL Trafficking Line]| The name of the ad tag. |
|\[Dimension\]|[!UICONTROL Geo]|[!UICONTROL City]|The city to which the reported data is attributed.|
|\[Dimension\]|[!UICONTROL Geo]|[!UICONTROL Country Code]|The country code for the country to which the reported data is attributed.|
|\[Dimension\]|[!UICONTROL Geo]|[!UICONTROL DMA]|The Designated Market Area (DMA) to which the reported data is attributed.|
|\[Dimension\]|[!UICONTROL Geo]|[!UICONTROL State Code]|The state code for the state to which the reported data is attributed.|
|\[Dimension\]|[!UICONTROL Geo]|[!UICONTROL Zip Code]|The zip code to which the reported data is attributed.|
|\[Dimension\]|[!UICONTROL Product]|[!UICONTROL Category ID]|(Dynamic ads) The target product category ID.|
|\[Dimension\]|[!UICONTROL Product]|[!UICONTROL Category Name]|(Dynamic ads) The target product category name.|
|\[Dimension\]|[!UICONTROL Product]|[!UICONTROL Creative Attribute 1]|(Dynamic ads) The first creative attribute.|
|\[Dimension\]|[!UICONTROL Product]|[!UICONTROL Creative Attribute 2]|(Dynamic ads) The second creative attribute.|
|\[Dimension\]|[!UICONTROL Product]|[!UICONTROL Creative Attribute 3]|(Dynamic ads) The third creative attribute.|
|\[Dimension\]|[!UICONTROL Product]|[!UICONTROL Creative Attribute 4]|(Dynamic ads) The fourth creative attribute.|
|\[Dimension\]|[!UICONTROL Product]|[!UICONTROL Creative Attribute 5]|(Dynamic ads) The fifth creative attribute.|
|\[Dimension\]|[!UICONTROL Product]|[!UICONTROL Product ID]|(Dynamic ads) The target product ID.|
|\[Dimension\]|[!UICONTROL Product]|[!UICONTROL Product Name]|(Dynamic ads) The target product name.|
|\[Dimension\]|[!UICONTROL Segment]|[!UICONTROL Matched Audience Segment ID]|The IDs for up to five user segments that matched the ad theme.|
|\[Dimension\]|[!UICONTROL Segment]|[!UICONTROL Pixel Segment ID]|The ID for a retargeting pixel to which the reported data is attributed.|
|\[Dimension\]|[!UICONTROL Segment]|[!UICONTROL Pixel Segment Name]|The name of a retargeting pixel to which the reported data is attributed.|
|\[Dimension\]|[!UICONTROL Segment]|[!UICONTROL Segment Values]|The attributes for an audience segment to which the reported data is attributed.|
|[!UICONTROL Metrics]|[!UICONTROL Standard]|[!UICONTROL Clicks]|The sum of all clicks on an ad.|
|[!UICONTROL Metrics]|[!UICONTROL Standard]|[!UICONTROL CTR]|The click-through rate, which is the percentage of clicks divided by ad impressions.|
|[!UICONTROL Metrics]|[!UICONTROL Standard]|[!UICONTROL Engagement Rate]|The percentage of impressions served that resulted in user engagements.|
|[!UICONTROL Metrics]|[!UICONTROL Standard]|[!UICONTROL Engagements]|The number of interactions on a served ad.|
|[!UICONTROL Metrics]|[!UICONTROL Standard]|[!UICONTROL Impressions]|The total number of ad impressions.|
|[!UICONTROL Metrics]|[!UICONTROL Standard]|[!UICONTROL Media Match Rate]| The percentage of impressions with a retargeted cookie. |
|[!UICONTROL Metrics]|[!UICONTROL Standard]|[!UICONTROL Product Clicks]|(Dynamic ads only) The sum of all clicks on ads for a product. When the product is null, this value is zero (0).|
|[!UICONTROL Metrics]|[!UICONTROL Standard]|[!UICONTROL Product Conversion]|(Dynamic ads only) The sum of all conversions on ads for a product. When the product is null, this value is zero (0).|
|[!UICONTROL Metrics]|[!UICONTROL Standard]|[!UICONTROL Product Conversion Rate]|(Dynamic ads only) The percentage of ads for a product that resulted in conversions. When the product is null, this value is zero (0).|
|[!UICONTROL Metrics]|[!UICONTROL Standard]|[!UICONTROL Product CTR]|(Dynamic ads only) The click-through rate for ads for a product, which is the percentage of clicks divided by ad impressions. When the product is null, this value is zero (0).|
|[!UICONTROL Metrics]|[!UICONTROL Standard]|[!UICONTROL Product Impressions]|(Dynamic ads only) The total number of impressions for a product. When the product is null, this value is zero (0).|
|[!UICONTROL Metrics]|[!UICONTROL Standard]|[!UICONTROL Product Revenue]|(Dynamic ads only) The total revenue on served ads for a product. When the product is null, this value is zero (0).|
|[!UICONTROL Metrics]|[!UICONTROL Standard]|[!UICONTROL Revenue]|The total revenue on served ads.|
|[!UICONTROL Metrics]|[!UICONTROL Video]|[!UICONTROL 100% Completion Rate]|The percentage of views that watched the ad in its entirety.|
|[!UICONTROL Metrics]|[!UICONTROL Video]|[!UICONTROL 25% Completion Rate]|The percentage of views that watched at least one quartile of the ad.|
|[!UICONTROL Metrics]|[!UICONTROL Video]|[!UICONTROL 50% Completion Rate]|The percentage of views that watched at least two quartiles of the ad.|
|[!UICONTROL Metrics]|[!UICONTROL Video]|[!UICONTROL 75% Completion Rate]|The percentage of views that watched at least three quartiles of the ad.|
|[!UICONTROL Metrics]|[!UICONTROL Video]|[!UICONTROL 100% Completions]|The number of views that watched the ad in its entirety.|
|[!UICONTROL Metrics]|[!UICONTROL Video]|[!UICONTROL 25% Completions]|The number of views that watched at least one quartile of the ad.|
|[!UICONTROL Metrics]|[!UICONTROL Video]|[!UICONTROL 50% Completions]|The number of views that watched at least two quartiles of the ad.|
|[!UICONTROL Metrics]|[!UICONTROL Video]|[!UICONTROL 75% Completions]|The number of views that watched at least three quartiles of the ad.|
|[!UICONTROL Metrics]|[!UICONTROL Video]|[!UICONTROL Avg Percent Viewed]|The average percentage an ad was watched to completion, accounting for all views.|
|[!UICONTROL Metrics]|[!UICONTROL Video]|[!UICONTROL Play Rate]|The percentage of impressions served that resulted in video views.|
|[!UICONTROL Metrics]|[!UICONTROL Video]|[!UICONTROL Playtime per View]|The average duration of a video view, measured in seconds.|
|[!UICONTROL Metrics]|[!UICONTROL Video]|[!UICONTROL Viewed Minutes]|The total number of minutes a video ad was viewed.|
|[!UICONTROL Metrics]|[!UICONTROL Video]|[!UICONTROL Views]|The total number of video ad views.




|[!UICONTROL Metrics]|[!UICONTROL Viewability]|[!UICONTROL 100% Viewable Completion (%)]| .|
|[!UICONTROL Metrics]|[!UICONTROL Viewability]|[!UICONTROL 50% Viewable Completion (%)]| .|
|[!UICONTROL Metrics]|[!UICONTROL Viewability]|[!UICONTROL Viewability Rate (%)]|The percentage of viewable impressions out of all measurable impressions, calculated as <code>[!UICONTROL Viewable Impressions] / [!UICONTROL Measurable Impressions]</code>.|
|[!UICONTROL Metrics]|[!UICONTROL Viewability]|[!UICONTROL Viewable Impressions]|The number of ad impressions considered viewable.|
|[!UICONTROL Conversion Metrics]|[Grouped by advertiser in report settings]|[Advertiser-specific conversion]| The total for a specified advertiser-specific conversion metric or Adobe Analytics event.|
|[!UICONTROL Custom Goals]|[Grouped by advertiser in report settings]|[Advertiser-specific custom goal]|(Advertisers with Advertising DSP) The weighted sum of all conversions that are included in the specified [Advertising DSP custom goal](/help/dsp/optimization/custom-goal.md).|

{style="table-layout:auto"}

-->

>[!MORELIKETHIS]
>
>* [경험 수준 성과 보고서](/help/creative/experiences/experience-performance-details.md)
>* [DSP 사용자 지정 보고서 정보](/help/dsp/reports/report-about.md){target="_blank"}
>* [정보 [!UICONTROL report destinations]](/help/dsp/reports/report-destinations/report-destination-about.md){target="_blank"}
