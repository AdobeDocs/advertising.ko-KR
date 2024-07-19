---
source-git-commit: 029e406fbfb4217ce78364c2d1f1a6dae24ff588
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 0%

---
# 텍스트 광고 템플릿 - 광고 그룹 수준 음성 키워드 설정

**[!UICONTROL Delete negative keywords when omitted from list]:**(Yandex를 제외한 모든 광고 네트워크, 선택 사항) 아래 목록에 지정되지 않은 템플릿을 사용하여 이전에 만든 기존 광고 그룹 수준의 부정적인 키워드를 삭제합니다. **참고:** 다른 방법(예: 일반 일괄 시트, [!UICONTROL Campaigns] 보기 또는 광고 네트워크의 광고 편집기에서)을 사용하여 만든 부정적 키워드는 템플릿을 사용하여 제거되지 않습니다.

**[!UICONTROL Apply these negatives]:**([!DNL Yandex]을(를) 제외한 모든 광고 네트워크; 선택 사항) 추가할 정적 광고 그룹 수준의 부정적인 키워드. 동일한 키워드에 대해 여러 키워드 또는 여러 일치 유형을 지정하려면 별도의 행에 입력합니다. 빼기 기호 없이 다음 구문을 사용합니다.

* 음수 브로드 일치: `keyword`([!DNL Microsoft Advertising]에서 지원되지 않음)
* 음수 구 일치: `"keyword"`
* 정확히 일치하는 음수: `[keyword]`

구문과 정확한 일치 유형에 대한 일반적인 구문은 템플릿을 통해 피드 데이터를 전파할 때 생성되는 일괄 시트에서 사용됩니다. **참고:** [!UICONTROL Keywords] 탭이나 [!UICONTROL Search] > [!UICONTROL Campaigns] > [!UICONTROL Campaigns] 보기에서 음수 키워드를 볼 수 없습니다.
