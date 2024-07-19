---
source-git-commit: 029e406fbfb4217ce78364c2d1f1a6dae24ff588
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---
# 텍스트 광고 템플릿 - 광고 그룹 맵 메서드

**[!UICONTROL Map Method]:**(광고 그룹에 대해 [!UICONTROL Map Only]을(를) 사용하는 경우, [!DNL Yandex]을(를) 제외한 모든 광고 네트워크) 새 키워드 및 광고가 기존 광고 그룹에 매핑되는 방법:

* *[!UICONTROL Contains Anywhere]:* 이름이 지정된 문자열을 포함하는 기존 광고 그룹(있는 경우)에 데이터를 추가합니다.

* *[!UICONTROL Contains Exactly]:* 이름이 지정된 문자열을 포함하는 기존 광고 그룹(있는 경우)에 데이터를 추가합니다.

* *[!UICONTROL Exactly Matches]*(기본값): 같은 이름의 기존 광고 그룹(있는 경우)에 데이터를 추가합니다.

일치하는 항목이 없으면 광고 그룹에 대한 모든 데이터가 무시됩니다. 피드의 광고 그룹 데이터에 캠페인 데이터가 포함되지 않은 경우, 광고 그룹은 캠페인에 있는 동일한 이름의 광고 그룹(있는 경우)에 매핑됩니다. 여러 광고 그룹 일치 항목이 발견되면 키워드 및 광고가 해당 항목 모두에 매핑됩니다.
