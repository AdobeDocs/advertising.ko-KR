---
title: 사용자 지정 경고 템플릿 설정
description: 사용자 지정 경고 템플릿 설정에 대해 알아봅니다.
exl-id: c9cff26b-e6be-4dad-ac3a-b5a53387c4e6
feature: Search Alerts
source-git-commit: 3ab2e38f6a2f70c03504363575b13dc0dc730282
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 0%

---

# 사용자 지정 경고 템플릿 설정

| 탭 | 매개 변수 | 설명 |
|--- |--- |--- |
| [!UICONTROL Date Range] | [!UICONTROL Date] | 경고 조건을 평가할 날짜 범위입니다. 지표는 날짜 범위에서 집계하여 평가됩니다. 옵션 범위는 *[!UICONTROL Yesterday]*&#x200B;에서 *[!UICONTROL Last 180 Days]*&#x200B;까지입니다. |
| [!UICONTROL Filters] |  | [!UICONTROL Scheduling and Delivery] 탭에 지정된 시간에 경고를 트리거하는 조건입니다. 사용 가능한 열은 엔티티 유형(예: 캠페인 또는 키워드)에 따라 다릅니다. 모든 필터는 부울 함수 AND를 사용하여 결합됩니다. 즉, 지정된 모든 조건이 충족되어야 합니다.<ul><li><p>필터를 추가하려면 ![추가](/help/search-social-commerce/assets/arrow-down-expand.png "추가") ![&#x200B; 옆에 있는 &#x200B;](/help/search-social-commerce/assets/add.png "아래쪽 화살표")아래쪽 화살표&#x200B;**[!UICONTROL ADD FILTER]**&#x200B;를 클릭하고 다음을 수행합니다.</p></li><ol><li><p>(선택 사항) 텍스트 문자열로 열 이름을 필터링하려면 **[!UICONTROL ADD FILTER]** 입력 필드에 검색 문자열을 입력합니다.</p></li><li><p>열 메뉴에서 열 이름을 선택합니다.</p></li><li><p>열에서 필터를 정의합니다.</p></li><ul><li><p>(입력 필드가 없는 필터) 두 번째 메뉴 옆의 ![아래쪽 화살표](/help/search-social-commerce/assets/arrow-down-expand.png "아래쪽 화살표")를 클릭한 다음 포함할 각 값 옆의 확인란을 선택합니다.</p></li><li><p>(지정된 날짜 범위와 이전 기간 사이의 값 증가 또는 감소를 추적할 지표 열) 연산자의 경우 *증가* 또는 *감소*&#x200B;를 선택한 다음 임계값을 입력합니다.</p><p>예를 들어, &quot;[!UICONTROL Cost]&quot; 열을 선택했으며 캠페인 비용이 21% 증가할 때 알림을 받으려면 &quot;[!UICONTROL increases by]&quot;을(를) 선택하고 입력 필드에 21을 입력합니다. [!UICONTROL Date Comparison Format] 필드에 통화 단위의 변경보다 백분율의 변경에 관심이 있음을 나타냅니다.</p><p>이 옵션을 선택하면 각 일반 데이터 열에 대해 두 개의 열이 더 추가됩니다. 예를 들어, 보고서에는 &quot;클릭 수&quot;에 대해 하나의 열만 포함하는 대신 &quot;클릭 수 R1&quot;(범위 1의 경우) &quot;클릭 수 R2&quot;(범위 2의 경우) 및 &quot;클릭 수 차이&quot; 또는 &quot;클릭 수 차이(%)&quot;에 대한 열이 지정된 [!UICONTROL Date Comparison Format]에 따라 포함됩니다(아래 참조).</p><p>**메모:**</p><ul><li><p>차이 열은 파생 지표에 대해 채워지지 않습니다.<p></li><li><p>이 기능은 전환 지표, ID 또는 레이블 분류 열에 사용할 수 없습니다.</p></li><li><p>큰 날짜 범위를 비교하는 보고서를 생성하는 데 시간이 더 걸릴 수 있습니다.</p></li></ul></ul><li><p>(입력 필드가 있는 다른 모든 필터) 두 번째 메뉴에서 연산자를 선택한 다음 해당 값을 입력합니다.</p><p>예를 들어 &quot;클릭 수&quot; 열을 선택하고 클릭 수가 100개를 초과하는 행만 반환하려는 경우 &quot;보다 큼&quot;을 선택하고 입력 필드에 100을 입력합니다.</p><p>데이터 유형에 따라 사용 가능한 연산자에는 <i>보다 큼</i>, <i>보다 작음</i>, <i>같음</i>, <i>포함</i>, <i>포함하지 않음</i>, <i>다음으로 시작</i>, <i>다음으로 끝남</i>, <i>값 없음</i>, <i>값 있음</i>, <i>이전</i>, <i>다음</i> 또는 <i>날짜 없음</i>이 포함될 수 있습니다.</p><p>**참고:** 텍스트 값은 대/소문자를 구분하지 않습니다. 예를 들어 이름에 &quot;대출&quot;이 있는 캠페인으로 필터링하면 결과에 &quot;소비자 대출&quot; 및 &quot;대출 신청&quot;이 포함될 수 있습니다.</p></li></ol><li><p>필터를 제거하려면 필터 정의 옆에 있는 ![삭제](/help/search-social-commerce/assets/delete.png "삭제")를 클릭합니다.</p></li></ul> |
|  | [!UICONTROL Comparing] | (하나 이상의 지표 열에서 경고 트랙이 증가 또는 감소하는 경우 사용 가능; 읽기 전용) 데이터가 비교되는 두 날짜 범위입니다. |
|  | [!UICONTROL Date Comparison Format] | (하나 이상의 지표 열에서 경고 트랙이 증가 또는 감소하는 경우 사용 가능) 두 날짜 범위의 데이터 차이를 표시하는 방법:<ul><li><p><i>[!UICONTROL Variance]</i>(기본값) — 차이를 숫자 값으로 표시합니다.</p></li><li><p><i>[!UICONTROL % Change]</i> — 차이를 백분율로 표시합니다.</p></li></ul> |
| [!UICONTROL Scheduling and Delivery] | [!UICONTROL Name] | 경고 이름. 5자 이상이어야 합니다. |
|  | [!UICONTROL Trigger this Alert] [when] | 경고가 지정된 조건 필터를 확인하고 모든 조건이 충족되면 이메일 알림을 보내는 빈도:<ul><li><p>[!UICONTROL Daily at <*NN*> `[AM\|PM]`]</p></li><li><p>[!UICONTROL Weekly on <*요일*>, &lt;*NN*> `[AM\|PM]`]</p></li><li><p>[!UICONTROL Every month on <*일 NN*>, &lt;*NN*> `[AM\|PM]`]</p></li></ul>**참고:** 이 값은 평가 기간에 영향을 주지 않습니다. |
|  | [!UICONTROL Email Recipients] | (경고 템플릿 작성자만 편집 가능, 기타 사용자의 경우 읽기 전용) 경고가 생성될 때 알림을 보낼 이메일 주소. 기본적으로 템플릿 작성자의 주소가 입력됩니다.<br><br>주소를 추가하려면 주소를 입력한 다음 **[!UICONTROL Add]**&#x200B;을(를) 클릭합니다. 여러 주소를 지정하려면 쉼표나 공백으로 구분하거나 별도로 추가합니다.<br><br>경고에 최대 1000개의 레코드가 포함된 경우 경고의 CSV 버전이 전자 메일 메시지에 첨부됩니다. |

>[!MORELIKETHIS]
>
>* [사용자 지정 경고 정보](alert-about.md)
>* [사용자 지정 경고 템플릿 만들기](alert-template-create.md)
>* [사용자 지정 경고 템플릿 편집](alert-template-edit.md)
>* [사용자 지정 경고 템플릿 일시 중지](alert-template-pause.md)
>* [사용자 지정 경고 템플릿 활성화](alert-template-activate.md)
>* [사용자 지정 경고 템플릿을 삭제](alert-template-delete.md)
>* [사용자 지정 경고 보기](alert-view.md)
>* [사용자 지정 경고에 대한 데이터 내보내기](alert-export-data.md)
