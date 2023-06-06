---
source-git-commit: 029e406fbfb4217ce78364c2d1f1a6dae24ff588
workflow-type: tm+mt
source-wordcount: '104'
ht-degree: 0%

---
# 일부 광고 설정에서 경로 1 표시 및 경로 2 표시 필드

**[!UICONTROL Display Path 1]**, **[!UICONTROL Display Path 2]:** (선택 사항) 최종 URL에서 자동으로 추출되는 표시 URL에 추가되는 텍스트입니다. 각 경로는 URL 앞에 슬래시(`/`). 경로에는 슬래시()를 사용할 수 없습니다.`/`) 또는 줄바꿈(`\n`)자. 각 경로의 최대 길이는 15자 또는 7개의 더블바이트 문자입니다.

광고 사용자 정의자를 삽입하려면 다음 형식을 사용하십시오. `Default text` 는 피드 파일에 유효한 값이 포함되지 않았을 때 삽입할 선택적 값입니다.

* [!DNL Google Ads]: `{CUSTOMIZER.AdCustomizerName:Default text}, such as {CUSTOMIZER.Discount:10%}`

* [!DNL Microsoft Advertising]: `{CUSTOMIZER.Attribute name:Default text}, such as {CUSTOMIZER.Discount:10%}`

예를 들어 표시 경로 1이 &quot;거래&quot;이고 표시 경로 2가 &quot;로컬&quot;인 경우 표시 URL은 다음과 같습니다. `<display URL>/deals/local`예: www.example.com/deals/local
