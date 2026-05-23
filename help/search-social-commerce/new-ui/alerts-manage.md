---
title: (새 UI) 사용자 지정 경고 관리
description: 사용자 지정 경고 및 경고 템플릿을 생성, 구성, 일시 중지, 활성화, 삭제, 보기 및 내보내는 방법을 알아봅니다.
feature: Search Alerts
source-git-commit: 0fddeb8f01bd7c310544973ae2aff78339eb2144
workflow-type: tm+mt
source-wordcount: '1065'
ht-degree: 0%

---

# (새 UI) 사용자 지정 경고 관리

경고 템플릿을 만들어 포트폴리오, 캠페인 또는 광고 그룹이 지정된 기간 동안 성능 지표와 같은 특정 조건을 충족하는 시점을 식별한 다음 경고를 생성합니다. 경고는 단일 광고주에 대해 사용할 수 있습니다. 경고는 관련 기본 보기의 모든 열을 포함합니다. 예를 들어 캠페인 수준 경고에는 기본 [!UICONTROL Campaigns] 보기의 모든 열이 포함됩니다.

[!UICONTROL Custom Alerts] 패널의 [!UICONTROL Alert Templates] 탭이나 페이지의 맨 위에서 경고 템플릿을 만들 수 있습니다.

경고 템플릿에 대해 경고 인스턴스가 트리거되는 경우:

* 지정된 수신자는 이메일 알림을 받습니다. 경고에 최대 1000개의 레코드가 포함된 경우 전자 메일 알림에 경고를 트리거한 모든 엔터티에 대한 데이터를 포함하여 경고 데이터가 포함된 [CSV](/help/search-social-commerce/glossary.md#c-d) 파일이 포함됩니다.

* 경고가 [!UICONTROL Custom Alert Templates] 패널의 [!UICONTROL Triggered Alerts] 탭에 나열됩니다.<!-- Not available as of 5/22 for alerts triggered the day before:  A downloadable report is available for ten days after the alert is triggered. -->

<!-- This doesn't seem to be true as of 5/22 -- check on this behavior:    * The alert is listed in the [!UICONTROL Notifications] center in the applicable entity view, which is available from the right toolbar. Notifications remain in the [!UICONTROL Notifications] center unless you delete them or mark them as read. -->

## [!UICONTROL Custom Alerts] 보기

[!UICONTROL Custom Alerts] 패널을 열려면 오른쪽 상단의 ![사용자 지정 경고](/help/search-social-commerce/assets/custom-alert.png "사용자 지정 경고")를 클릭합니다.

[!UICONTROL Custom Alerts] 패널에는 계정에 대해 만들어진 모든 경고 템플릿을 나열하며 경고 템플릿을 만들고, 편집하고, 일시 중지하고, 다시 활성화하고, 삭제할 수 있는 [!UICONTROL Alert Templates] 보기가 포함되어 있습니다. [!UICONTROL Triggered Alerts] 보기는 생성된 경고 인스턴스를 나열합니다.

## 사용 가능한 작업

* [트리거된 경고 보기](#alert-view)

* [사용자 지정 경고 템플릿 보기](#alert-template-view)

* [사용자 지정 경고 템플릿 만들기](#alert-template-create)

* [사용자 지정 경고 템플릿 편집](#alert-template-edit)

* [사용자 지정 경고 템플릿 일시 중지](#alert-template-pause)

* [사용자 지정 경고 템플릿 활성화](#alert-template-activate)

* [사용자 지정 경고 템플릿 삭제](#alert-template-delete)

<!-- Not available as of 5/22:  * [Export data for triggered alerts](#alert-export-data) -->

## 트리거된 경고 보기 {#alert-view}

1. 페이지의 오른쪽 상단에서 ![사용자 지정 경고](/help/search-social-commerce/assets/custom-alert.png "사용자 지정 경고")를 클릭합니다.

1. **[!UICONTROL Triggered Alerts]** 탭을 클릭합니다.

1. (선택 사항) 특정 엔티티 유형에 대한 경고를 포함하도록 목록을 필터링하거나 템플릿 이름 내에서 텍스트 문자열을 검색합니다. 검색 쿼리는 대/소문자를 구분하지 않습니다.

## 사용자 지정 경고 템플릿 보기 {#alert-template-view}

1. 페이지의 오른쪽 상단에서 ![사용자 지정 경고](/help/search-social-commerce/assets/custom-alert.png "사용자 지정 경고")를 클릭하면 [!UICONTROL Alert Templates] 탭이 열립니다.

1. (선택 사항) 특정 엔티티 유형에 대한 경고를 포함하도록 목록을 필터링하거나 템플릿 이름 내에서 텍스트 문자열을 검색합니다. 검색 쿼리는 대/소문자를 구분하지 않습니다.

1. (선택 사항) 경고 템플릿에 대한 모든 기준을 보려면 기준 수를 클릭합니다(예: ![사용자 지정 경고 기준 예 단추](/help/search-social-commerce/assets/custom-alert-criteria.png "사용자 지정 경고 기준 예 단추")).

## 사용자 지정 경고 템플릿 만들기 {#alert-template-create}

새 경고 템플릿의 상태는 &quot;[!UICONTROL Active]&quot;입니다.

1. 다음 중 하나를 수행합니다.

   * 페이지의 오른쪽 상단에서 ![사용자 지정 경고](/help/search-social-commerce/assets/custom-alert.png "사용자 지정 경고") > **[!UICONTROL Create Custom Alert]**&#x200B;을(를) 클릭합니다.

   페이지의 오른쪽 상단에서 ![사용자 지정 경고](/help/search-social-commerce/assets/custom-alert.png "사용자 지정 경고") > **[!UICONTROL View Custom Alerts]**&#x200B;을(를) 클릭합니다. 그러면 [!UICONTROL Alert Templates] 탭이 열립니다. **[!UICONTROL Create Alert]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Entity]**, **[!UICONTROL Date Range]**, **[!UICONTROL Filters]** 및 **[!UICONTROL Scheduling and Delivery]** 탭에서 [경고 설정](#alert-template-settings)을(를) 지정하십시오.

   탭 이름(예: &quot;필터&quot;)을 클릭하거나 오른쪽 하단의 **[!UICONTROL Next]**&#x200B;을 클릭하여 탭 사이를 이동할 수 있습니다.

1. [!UICONTROL Summary] 탭에서 **[!UICONTROL Create Alert]**&#x200B;을(를) 클릭합니다.

## 사용자 지정 경고 템플릿 편집 {#alert-template-edit}

1. 오른쪽 상단에서 ![사용자 지정 경고](/help/search-social-commerce/assets/custom-alert.png "사용자 지정 경고") > **[!UICONTROL View Custom Alerts]**&#x200B;을(를) 클릭합니다. 그러면 [!UICONTROL Alert Templates] 탭이 열립니다.

1. (선택 사항) 특정 엔티티 유형에 대한 경고를 포함하도록 목록을 필터링하거나 템플릿 이름 내에서 텍스트 문자열을 검색합니다. 검색 쿼리는 대/소문자를 구분하지 않습니다.

1. 템플릿 이름 옆에 있는 ![편집](/help/search-social-commerce/assets/edit-new.png "편집")을 클릭합니다.

1. [!UICONTROL Edit Custom Alert] 창에서 **[!UICONTROL Date Range]**, **[!UICONTROL Filters]** 및 **[!UICONTROL Scheduling and Delivery]** 탭의 [경고 설정](#alert-template-settings)을(를) 편집합니다.

   탭 이름(예: &quot;필터&quot;)을 클릭하거나 오른쪽 하단의 **[!UICONTROL Next]**&#x200B;을 클릭하여 탭 사이를 이동할 수 있습니다.

1. [!UICONTROL Summary] 탭에서 **[!UICONTROL Update Alert]**&#x200B;을(를) 클릭합니다.

## 사용자 지정 경고 템플릿 일시 중지 {#alert-template-pause}

1. 오른쪽 상단에서 ![사용자 지정 경고](/help/search-social-commerce/assets/custom-alert.png "사용자 지정 경고") > **[!UICONTROL View Custom Alerts]**&#x200B;을(를) 클릭합니다. 그러면 [!UICONTROL Alert Templates] 탭이 열립니다.

1. (선택 사항) 특정 엔티티 유형에 대한 경고를 포함하도록 목록을 필터링하거나 템플릿 이름 내에서 텍스트 문자열을 검색합니다. 검색 쿼리는 대/소문자를 구분하지 않습니다.

1. 템플릿 행에서 *[!UICONTROL Paused]*&#x200B;을(를) 선택합니다.

## 사용자 지정 경고 템플릿 활성화 {#alert-template-activate}

1. 오른쪽 상단에서 ![사용자 지정 경고](/help/search-social-commerce/assets/custom-alert.png "사용자 지정 경고") > **[!UICONTROL View Custom Alerts]**&#x200B;을(를) 클릭합니다. 그러면 [!UICONTROL Alert Templates] 탭이 열립니다.

1. (선택 사항) 특정 엔티티 유형에 대한 경고를 포함하도록 목록을 필터링하거나 템플릿 이름 내에서 텍스트 문자열을 검색합니다. 검색 쿼리는 대/소문자를 구분하지 않습니다.

1. 템플릿 행에서 *[!UICONTROL Active]*&#x200B;을(를) 선택합니다.

## 사용자 지정 경고 템플릿 삭제 {#alert-template-delete}

생성한 경고 템플릿만 삭제할 수 있습니다.

1. 오른쪽 상단에서 ![사용자 지정 경고](/help/search-social-commerce/assets/custom-alert.png "사용자 지정 경고") > **[!UICONTROL View Custom Alerts]**&#x200B;을(를) 클릭합니다. 그러면 [!UICONTROL Alert Templates] 탭이 열립니다.

1. (선택 사항) 특정 엔티티 유형에 대한 경고를 포함하도록 목록을 필터링하거나 템플릿 이름 내에서 텍스트 문자열을 검색합니다. 검색 쿼리는 대/소문자를 구분하지 않습니다.

1. 템플릿 행에서 ![삭제](/help/search-social-commerce/assets/delete-new.png "삭제")를 클릭합니다.

1. 확인 메시지 상자에서 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

## 사용자 지정 경고 템플릿 설정 {#alert-template-settings}

| 탭 | 매개 변수 | 설명 |
|--- |--- |--- |
|  | [!UICONTROL Name] | 경고 이름. 5자 이상이어야 합니다. |
| [!UICONTROL Date Range] | [!UICONTROL Select Entity] | 평가할 엔터티 형식: <i>[!UICONTROL Portfolio]</i>, <i>[!UICONTROL Campaign]</i> 또는 <i>[!UICONTROL Ad Group]</i>. |
| [!UICONTROL Date Range] | [!UICONTROL Period] | 경고 조건을 평가할 날짜 범위입니다. 지표는 날짜 범위에서 집계하여 평가됩니다. 옵션 범위는 *[!UICONTROL Yesterday]*&#x200B;에서 *[!UICONTROL Last 180 Days]*&#x200B;까지입니다. |
| [!UICONTROL Filters] | \[정의된 필터\] | [!UICONTROL Scheduling and Delivery] 탭에 지정된 시간에 경고를 트리거하는 조건입니다. 사용 가능한 열은 엔티티 유형에 따라 다릅니다. 모든 필터는 부울 함수 AND를 사용하여 결합됩니다. 즉, 지정된 모든 조건이 충족되어야 합니다.<ul><li><p>필터를 추가하려면 다음 작업을 수행하십시오.<p><ol><li><p>(선택 사항) 텍스트 문자열로 열 이름을 필터링하려면 [!UICONTROL ADD FILTER] 입력 필드에 검색 문자열을 입력합니다.</p></li><li><p>열 목록에서 열 이름을 선택합니다.</p></li><li><p>열에서 필터를 정의합니다.</p></li><ul><li><p>(입력 필드가 없는 필터) 두 번째 메뉴 옆의 ![아래쪽 화살표](/help/search-social-commerce/assets/arrow-down-expand.png "아래쪽 화살표")를 클릭한 다음 포함할 각 값 옆의 확인란을 선택합니다.</p></li><li><p>(입력 필드가 있는 다른 모든 필터) 두 번째 메뉴에서 연산자를 선택한 다음 해당 값을 입력합니다.</p><p>예를 들어 &quot;클릭 수&quot; 열을 선택하고 클릭 수가 100개를 초과하는 행만 반환하려는 경우 &quot;보다 큼&quot;을 선택하고 입력 필드에 100을 입력합니다.</p><p>데이터 유형에 따라 사용 가능한 연산자에는 <i>보다 큼</i>, <i>보다 작음</i>, <i>같음</i>, <i>포함</i>, <i>포함하지 않음</i>, <i>다음으로 시작</i>, <i>다음으로 끝남</i>, <i>값 없음</i>, <i>값 있음</i>, <i>이전</i>, <i>다음</i> 또는 <i>날짜 없음</i>이 포함될 수 있습니다.</p><p>**참고:** 텍스트 값은 대/소문자를 구분하지 않습니다. 예를 들어 이름에 &quot;대출&quot;이 있는 캠페인으로 필터링하면 결과에 &quot;소비자 대출&quot; 및 &quot;대출 신청&quot;이 포함될 수 있습니다.</p></li></ol><li><p>필터를 제거하려면 필터 정의 옆에 있는 ![삭제](/help/search-social-commerce/assets/delete.png "삭제")를 클릭합니다.</p></li></ul> |
| [!UICONTROL Scheduling and Delivery] | [!UICONTROL Trigger this Alert] \[when\] | 경고가 지정된 조건 필터를 확인하고 모든 조건이 충족되면 이메일 알림을 보내는 빈도:<ul><li><p>[!UICONTROL Daily at <*NN*> `[AM\|PM]`]</p></li><li><p>[!UICONTROL Weekly on <*요일*>, &lt;*NN*> `[AM\|PM]`]</p></li><li><p>[!UICONTROL Every month on <*일 NN*>, &lt;*NN*> `[AM\|PM]`]</p></li></ul>**참고:** 이 값은 평가 기간에 영향을 주지 않습니다. |
|  | [!UICONTROL Email Recipients] | (경고 템플릿의 작성자만 편집할 수 있으며 기타 사용자는 읽기 전용) 경고가 트리거될 때 알림을 전송할 등록된 검색, 소셜 및 Commerce 사용자. 기본적으로 사용자 계정의 이름이 선택됩니다. 선택적으로 광고주의 데이터에 액세스할 수 있는 사용자를 추가하거나 제거합니다.<br><br>경고에 최대 1000개의 레코드가 포함된 경우 경고의 CSV 버전이 전자 메일 메시지에 첨부됩니다. |

<!--

Not available as of 5/22:

## Export data for triggered alerts {#alert-export-data}

You can export data for a triggered alert or data for the most recently triggered alert for an alert template as a [!DNL Microsoft Excel] workbook ([XLS](/help/search-social-commerce/glossary.md#w-x) file), a tab-separated values ([TSV](/help/search-social-commerce/glossary.md#s-t)) file, or a comma-separated values ([CSV](/help/search-social-commerce/glossary.md#c-d)) file. Downloadable reports are available for ten days after the alert is triggered and are then automatically deleted.

1. Do either of the following:

   * (To export data for the most recently triggered alert for an alert template) In the upper right, click ![Custom Alert](/help/search-social-commerce/assets/custom-alert.png "Custom Alert") > **[!UICONTROL View Custom Alerts]**, which opens to the [!UICONTROL Alert Templates] tab.

   * (To export data for a specific triggered alert) In the upper right, click ![Custom Alert](/help/search-social-commerce/assets/custom-alert.png "Custom Alert"). Click **[!UICONTROL Triggered Alerts]**.

1. In the [!UICONTROL Export] column next to the template or report name, click the name of a format, and then open or save the file according to your browser's normal procedure:

   * **[!UICONTROL XLS]:** For an [!DNL Excel] workbook with a single worksheet (XLS). The report includes one worksheet, labeled at the top with the parameters, with one row for each included component when data for the component is available. Rows with no data are omitted. Basic reports include a total for each numeric column.

   * **[!UICONTROL TSV]:** For a TSV file. The report includes the parameters and one row for each included component.

   * **[!UICONTROL CSV]:** For a CSV file. The report includes the parameters and one row for each included component.

-->
