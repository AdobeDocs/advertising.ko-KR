---
source-git-commit: 029e406fbfb4217ce78364c2d1f1a6dae24ff588
workflow-type: tm+mt
source-wordcount: '144'
ht-degree: 0%

---
# RSA 광고 설정의 광고 설명 필드

**[!UICONTROL Ad Descriptions]:** 최소 2개, 최대 4개의 광고 설명(위치 고정 옵션 포함). 광고 네트워크에는 최대 2개의 설명과 함께 광고가 표시됩니다. 최소 2개를 입력하십시오. 각 설명의 최대 길이는 동적 텍스트(예: 키워드 및 광고 사용자 값)를 포함하여 90자입니다.

광고 사용자 정의자를 삽입하려면 다음 형식을 사용하십시오. `Default text` 는 피드 파일에 유효한 값이 포함되지 않았을 때 삽입할 선택적 값입니다.

* [!DNL Google Ads]: `{CUSTOMIZER.AdCustomizerName:Default text}, such as {CUSTOMIZER.Discount:10%}`

* [!DNL Microsoft Advertising]: `{CUSTOMIZER.Attribute name:Default text}, such as {CUSTOMIZER.Discount:10%}`

특정 위치에 설명을 고정하려면 고정 옵션(예: &quot;[!UICONTROL Pinned at position 1]&quot;). 각 위치에 대해 하나 이상의 설명을 사용할 수 있어야 합니다. 여러 설명을 동일한 위치에 고정하면 최종 광고는 항상 지정된 위치에 이러한 설명 중 하나를 포함합니다. 위치 2에 고정된 설명은 광고와 함께 표시되지 않을 수 있습니다.

설명을 추가하려면 **[!UICONTROL + Add]**.
