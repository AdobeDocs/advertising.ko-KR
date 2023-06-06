---
source-git-commit: 029e406fbfb4217ce78364c2d1f1a6dae24ff588
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 0%

---
# 텍스트 광고 템플릿 - 광고 그룹 수준 음성 키워드 설정

**[!UICONTROL Delete negative keywords when omitted from list]:** (Yandex를 제외한 모든 광고 네트워크, 선택 사항) 아래 목록에 지정되지 않은 템플릿을 사용하여 이전에 만든 기존 광고 그룹 수준의 부정적인 키워드를 삭제합니다. **참고:** 다른 수단을 사용하여 생성된 부정적 키워드(예: 일반 일괄 시트에서는 [!UICONTROL Campaigns] 템플릿을 사용하여 보기 또는 광고 네트워크의 광고 편집기에서 를 제거할 수 없습니다.

**[!UICONTROL Apply these negatives]:** (를 제외한 모든 광고 네트워크 [!DNL Yandex]; 선택 사항) 추가할 정적 광고 그룹 수준의 부정적인 키워드입니다. 동일한 키워드에 대해 여러 키워드 또는 여러 일치 유형을 지정하려면 별도의 행에 입력합니다. 빼기 기호 없이 다음 구문을 사용합니다.

* 부정 브로드 일치: `keyword` (지원되지 않음 [!DNL Microsoft Advertising])
* 음수 구문 일치: `"keyword"`
* 음수 완전 일치: `[keyword]`

구문과 정확한 일치 유형에 대한 일반적인 구문은 템플릿을 통해 피드 데이터를 전파할 때 생성되는 일괄 시트에서 사용됩니다. **참고:** 에 음수 키워드가 표시되지 않습니다. [!UICONTROL Keywords] 탭 또는 [!UICONTROL Search] > [!UICONTROL Campaigns] > [!UICONTROL Campaigns] 보기.
