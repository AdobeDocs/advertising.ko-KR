---
source-git-commit: 029e406fbfb4217ce78364c2d1f1a6dae24ff588
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---
# 계정 및 캠페인 설정의 리디렉션 유형 필드

**[!UICONTROL Redirect Type]:** (대상 [!UICONTROL EF Redirect] 전용) 최종 URL 또는 대상 URL로 최종 사용자를 리디렉션하는 방법입니다. 선택한 옵션은 계정이나 캠페인의 모든 광고, 키워드 및 배치에 적용할 수 있습니다. 기본 계정 수준 설정은 광고주의 추적 설정에서 상속되고, 기본 캠페인 수준 설정은 계정 설정에서 상속됩니다.

* *[!UICONTROL Standard]:* 최종 사용자를 지정된 URL로 리디렉션하려면

* *[!UICONTROL Token]:* 최종 사용자를 URL로 리디렉션하고 클릭에 대한 검색, 소셜 및 상거래 ID도 기록하려면(`ef_id`) 토큰으로 사용되는 쿼리 문자열 매개 변수입니다. 오프라인 거래를 보고하거나, 검색, 소셜 및 상거래를 통해 Adobe Analytics과 데이터를 교환하거나, 내에서 발생하는 모든 전환을 추적하려는 경우 이 옵션을 선택합니다 [!DNL Apple Safari] 브라우저.

**참고:**

* 에서 전환하는 경우 [!UICONTROL Standard] 끝 [!UICONTROL Token]또는 그 반대로 계정에 대한 추적 URL을 다시 생성해야 합니다.
* 캠페인 수준에서 계정 수준 설정을 재정의할 수 있습니다.
