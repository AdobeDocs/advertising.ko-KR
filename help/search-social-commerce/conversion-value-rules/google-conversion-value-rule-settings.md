---
title: '[!DNL Google Ads] 전환 값 규칙 설정'
description: ' [!DNL Google Ads] 전환 값 규칙에 대한 설정을 참조합니다.'
source-git-commit: efb4b80337b36b3b631898ca9ed66e99227468f1
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 0%

---

# [!DNL Google Ads] 전환 값 규칙 설정

<!-- Go through all -->

| 섹션 | 매개 변수 | 설명 |
|---|---|---|
| [!UICONTROL Select Campaign] | [!UICONTROL Network] | 광고 네트워크입니다. |
| | [!UICONTROL Account] | 광고 네트워크 계정입니다. |
| | [!UICONTROL Campaign] | 광고 캠페인. |
| [!UICONTROL Conditions] > [!UICONTROL Primary Condition] | \[조건 유형\] | (기존 규칙의 읽기 전용) 값 조정을 트리거하기 위해 충족해야 하는 조건 유형:<ul><li>**장치:** 모든 또는 특정 장치 형식을 대상으로 합니다.</li><li>**위치:** 모든 국가 및 지역을 대상으로 하거나 특정 위치를 대상으로 하고 제외합니다.</li><li>**대상:** 모든 또는 특정 대상을 타깃팅하려면</li></ul>**참고:** 계정의 모든 규칙은 같은 유형의 기본 및 (선택 사항) 보조 조건을 사용해야 합니다. 예를 들어 규칙 1에 기본 조건 &quot;대상&quot;과 보조 조건 &quot;위치&quot;가 포함되어 있으면 계정의 다른 모든 규칙에는 기본 조건 &quot;대상&quot;이 있어야 합니다. 다른 규칙에 보조 조건이 포함된 경우 &quot;위치&quot;여야 합니다. |
| | 조건 유형 > 장치 | (장치 조건만 해당) 타깃팅할 장치 유형:<ul><li>**모든 장치** — 모든 장치 유형을 대상으로 합니다.</li><li>**장치 선택** — 타깃팅할 장치 유형을 하나 이상 지정하려면: **데스크톱**, **모바일** 및 **태블릿**.</li></ul>조건 내에서 부울 연산자 OR를 사용하여 여러 대상을 연결하므로 값 조정을 시작하는 데 모든 옵션이 충족될 수 있습니다. 예: \[Device is Mobile OR Tablet\]인 경우 1.5를 추가합니다. |
| | Condition Type > 위치 | (위치 조건만 해당) 위치 대상 및 제외:<ul><li>**모든 국가 및 지역** — 모든 국가 및 지역을 대상으로 하거나 특정 위치를 대상으로 하고 제외합니다.</li><li>**위치 입력** — 특정 위치를 타깃팅하고 제외합니다.</li></ul><ul><li>위치나 하위 위치를 확장하려면 이름 뒤에 있는 > 를 클릭합니다.</li><li>대상을 추가하려면 대상을 한 번 선택하여 녹색 확인 표시를 표시합니다.</li><li>대상을 제외하려면 빨간색 **[!UICONTROL X]**&#x200B;을(를) 표시하도록 대상을 다시 선택하십시오.</li><li>대상 또는 제외를 제거하려면 다음 중 하나를 수행합니다.<ul><li>![&#x200B; 열의 항목 옆에 있는 &#x200B;](/help/search-social-commerce/assets/delete.png "삭제")삭제[!UICONTROL Selections]를 클릭합니다.</li><li>확인 표시 또는 [!UICONTROL X]이(가) 나타나지 않을 때까지 대상을 선택하십시오.</li></ul></li></ul>조건 내에서 부울 연산자 OR를 사용하여 여러 대상 또는 제외를 결합하므로 값 조정을 시작하는 데 모든 옵션이 충족될 수 있습니다. 예: \[위치가 알제리 또는 튀니지\]이면 1.5를 추가합니다. |
| | 조건 유형 > 대상 | (대상 조건만 해당) 대상은 다음과 같습니다.<ul><li>**모든 대상 세그먼트** — 모든 [!DNL Google Ads]개 대상 세그먼트를 타깃팅합니다.</li><li>**대상 세그먼트 입력** — 특정 [!DNL Google Ads]대상 세그먼트를 대상으로 합니다.</li></ul><ul><li>카테고리 또는 하위 카테고리를 해당 세그먼트로 확장하려면 이름 뒤에 있는 > 를 클릭합니다.</li><li>대상을 추가하려면 대상을 선택합니다.</li><li>대상을 제거하려면 대상을 선택 취소하거나 선택 열의 항목 옆에 있는 ![삭제](/help/search-social-commerce/assets/delete.png "삭제")를 클릭합니다.</li></ul>조건 내에서 부울 연산자 OR를 사용하여 여러 대상 또는 제외를 결합하므로 값 조정을 시작하는 데 모든 옵션이 충족될 수 있습니다. 예: \[대상이 할인 여행자 또는 가족 휴가객\]인 경우 1.5를 추가합니다.<br><br>**참고:** 대상 대상을 저장하면 대상을 추가할 수 있지만 [!DNL Google Ads] 편집기 외부에서 대상을 제거할 수 없습니다. 대상 대상을 제거해야 하는 경우 [!DNL Google Ads]에 직접 로그인한 다음 [!DNL Google Ads] 편집기를 사용하십시오. |
| Conditions > 보조 조건 | | (선택 사항, 기존 규칙의 경우 읽기 전용) 값 조정을 트리거하기 위해 충족해야 하는 조건 유형입니다. 보조 조건을 포함할 때 부울 연산자인 ALL을 사용하여 보조 조건이 기본 조건에 결합되므로 값 조정을 시작하려면 두 조건을 모두 충족해야 합니다. 예: \[위치가 알제리 또는 튀니지\]이고 \[장치가 모바일 또는 태블릿\]인 경우 1.5를 추가합니다.<br><br>설명은 기본 조건의 항목을 참조하십시오.<br><br>**참고:** 계정의 모든 규칙은 같은 유형의 기본 및 (선택 사항) 보조 조건을 사용해야 합니다. 예를 들어 규칙 1에 기본 조건 &quot;대상&quot;과 보조 조건 &quot;위치&quot;가 포함되어 있으면 계정의 다른 모든 규칙에는 기본 조건 &quot;대상&quot;이 있어야 합니다. 다른 규칙에 보조 조건이 포함된 경우 &quot;위치&quot;여야 합니다. |
| 값 조정 | 값 | 조정 유형을 지정한 다음 양수 값을 입력합니다.<ul><li>**추가** — 전달된 전환 값에 지정된 값을 추가합니다. 값은 0보다 커야 합니다.</li><li>**곱하기** — 전달된 전환 값에 지정된 값을 곱합니다. 값은 0.5에서 10 사이여야 합니다.</li></ul> |

>[!MORELIKETHIS]
>
>* [정보 [!DNL Google Ads] 전환 값 규칙](about-google-conversion-value-rules.md)
>* [전환 값 규칙 만들기 [!DNL Google Ads] 2&rbrace;](create-google-conversion-value-rule.md)
>* [전환 값 규칙 편집 [!DNL Google Ads] 2&rbrace;](edit-google-conversion-value-rule.md)
>* [전환 값 규칙의 상태 변경 [!DNL Google Ads] &#x200B;](change-the-status-of-google-conversion-value-rule.md)

