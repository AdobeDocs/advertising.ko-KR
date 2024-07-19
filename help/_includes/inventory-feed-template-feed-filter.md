---
source-git-commit: 029e406fbfb4217ce78364c2d1f1a6dae24ff588
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---
# 텍스트 광고 템플릿 - 피드 필터

**\[피드 필터\]:** 피드 파일에서 전파할 행:

* *[!UICONTROL Propagate all rows found in feed:]*(기본값): 모든 행의 데이터를 전파합니다.

* *[!UICONTROL Propagate rows that meet certain conditions:]* 지정한 조건을 충족하는 행에만 데이터를 전파합니다. 적용할 필터 지정:

   1. 모든 필터에 사용할 부울 작업을 선택하십시오. **[!UICONTROL AND]** 또는 **[!UICONTROL OR]**.

   1. 첫 번째 메뉴에서 열 이름을 선택하고 두 번째 메뉴에서 연산자를 선택한 다음 해당 값을 입력하거나 입력 필드를 비워 두어 조건 없이 행에 대한 데이터를 전파합니다.

  열 목록에는 피드에서 사용 가능한 모든 열이 포함됩니다.

  사용 가능한 연산자에는 *[!UICONTROL contains]*, *[!UICONTROL does not contain]*, *[!UICONTROL =]*, *[!UICONTROL <>]*(같지 않음), *[!UICONTROL in]*, *[!UICONTROL not in]*, *[!UICONTROL less than]* 및 *[!UICONTROL greater than]*&#x200B;이(가) 포함됩니다. 연산자 &quot;[!UICONTROL in]&quot;을(를) 선택하면 쉼표로 구분된 값 목록을 입력할 수 있습니다. 레코드가 지정된 값과 일치하면 해당 행에 대한 데이터가 전파됩니다. 다른 모든 연산자의 경우 값을 하나만 입력합니다. 값은 대/소문자를 구분하지 않습니다.

  예를 들어 &quot;product_type&quot; 열을 선택하고 &quot;shoes&quot;를 포함하는 제품 이름에 대한 행만 반환하려면 &quot;**[!UICONTROL contains]**&quot;을(를) 선택하고 입력 필드에 `shoes`을(를) 입력합니다.

   1. (최대 9개의 추가 필터를 적용하려면) 각 추가 필터에 대해 **[!UICONTROL Add Condition]**&#x200B;을(를) 클릭한 다음 2단계별로 추가 필터를 지정하십시오.
