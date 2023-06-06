---
source-git-commit: 029e406fbfb4217ce78364c2d1f1a6dae24ff588
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---
# GGL 및 MS 캠페인 설정, MS 광고 그룹 설정, MS 멀티미디어 및 반응형 광고 설정의 사용자 지정 매개 변수 필드

**[!UICONTROL Custom Parameters]:** (선택 사항, 대상 캠페인에만 적용 가능 [!DNL Microsoft Advertising]) 최대 3개의 사용자 지정 매개 변수에 대한 이름 및 값 쌍입니다. 이름의 최대 길이는 영숫자 16자이고, 값의 최대 길이는 임베드된 매개 변수를 포함하여 200자입니다.

엔티티 및 해당 하위 엔티티에 대한 추적 템플릿에 사용자 지정 매개 변수 이름을 포함할 수 있습니다. 사용자가 관련 광고를 클릭하면 광고 네트워크가 매개 변수 이름을 정의된 매개 변수 값으로 바꿉니다. 예를 들어 고객 매개 변수를 만드는 경우 `{_color}=red` 및 추적 템플릿에는 `http://tracker.example.com/?color={_color}&u={lpurl}`: 사용자가 광고를 클릭하면 &quot;빨간색&quot;이 color 매개 변수에 삽입됩니다.

광고 그룹의 사용자 지정 매개 변수 또는 ([!DNL Microsoft Advertising] 광고 수준 은 동일한 이름으로 캠페인 수준 사용자 지정 매개 변수를 재정의합니다.
