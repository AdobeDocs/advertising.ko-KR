---
source-git-commit: 029e406fbfb4217ce78364c2d1f1a6dae24ff588
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---
# RSA 광고 설정의 광고 제목 필드

**[!UICONTROL Ad Titles]:** 최소 3개, 최대 15개의 광고 제목(헤드라인)에 선택적 위치 핀을 포함합니다. 광고 네트워크에는 최대 3개의 헤드라인이 있는 광고가 표시됩니다. 최소 3개를 입력하십시오. 각 제목의 최대 길이는 동적 문자를 포함하여 30자입니다
텍스트(예: 키워드 및 광고 사용자 값).

광고 사용자 지정기를 삽입하려면 다음 형식을 사용하십시오. 여기서 `Default text`은(는) 피드 파일에 유효한 값이 없을 때 삽입할 선택적 값입니다.

* [!DNL Google Ads]: `{CUSTOMIZER.AdCustomizerName:Default text}, such as {CUSTOMIZER.Discount:10%}`

* [!DNL Microsoft Advertising]: `{CUSTOMIZER.Attribute name:Default text}, such as {CUSTOMIZER.Discount:10%}`

제목을 특정 위치에 고정하려면 고정 옵션(예: &quot;[!UICONTROL Pinned at position 1]&quot;)을 선택하십시오. 각 직책에 대해 하나 이상의 제목을 사용할 수 있어야 합니다. 여러 제목을 동일한 위치에 고정하면 최종 광고에는 항상 지정된 위치의 해당 제목 중 하나가 포함됩니다. 위치 3에 고정된 제목은 광고와 함께 표시되지 않을 수 있습니다.

제목을 추가하려면 **[!UICONTROL + Add]**&#x200B;을(를) 클릭합니다.
