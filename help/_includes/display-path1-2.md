---
source-git-commit: a59b477a6f8a616851d85bf89b58434d4d56cd83
workflow-type: tm+mt
source-wordcount: '104'
ht-degree: 0%

---
# 일부 광고 설정에서 경로 1 표시 및 경로 2 표시 필드

**[!UICONTROL Display Path 1]**, **[!UICONTROL Display Path 2]:**(선택 사항) 최종 URL에서 자동으로 추출되는 표시 URL에 추가되는 텍스트입니다. 각 경로는 URL 앞에 슬래시(`/`)가 붙습니다. 경로에는 슬래시(`/`) 또는 줄바꿈(`\n`) 문자를 사용할 수 없습니다. 각 경로의 최대 길이는 15자 또는 7개의 더블바이트 문자입니다.

광고 사용자 지정기를 삽입하려면 다음 형식을 사용하십시오. 여기서 `Default text`은(는) 피드 파일에 유효한 값이 없을 때 삽입할 선택적 값입니다.

* [!DNL Google Ads]: `{CUSTOMIZER.AdCustomizerName:Default text}, such as {CUSTOMIZER.Discount:10%}`

* [!DNL Microsoft Advertising]: `{CUSTOMIZER.Attribute name:Default text}, such as {CUSTOMIZER.Discount:10%}`

예를 들어 [!UICONTROL Display Path 1]이(가) &quot;거래&quot;이고 [!UICONTROL Display Path 2]이(가) &quot;로컬&quot;이면 디스플레이 URL은 `<display URL>/deals/local`(예: www.example.com/deals/local)이 됩니다.
