---
source-git-commit: 029e406fbfb4217ce78364c2d1f1a6dae24ff588
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---
# 계정 및 캠페인 설정의 리디렉션 유형 필드

**[!UICONTROL Redirect Type]:**([!UICONTROL EF Redirect]에만 해당) 최종 사용자를 최종 URL 또는 대상 URL로 리디렉션하는 메서드입니다. 선택한 옵션은 계정이나 캠페인의 모든 광고, 키워드 및 배치에 적용할 수 있습니다. 기본 계정 수준 설정은 광고주의 추적 설정에서 상속되고, 기본 캠페인 수준 설정은 계정 설정에서 상속됩니다.

* *[!UICONTROL Standard]:* 최종 사용자를 지정된 URL로 리디렉션합니다.

* *[!UICONTROL Token]:* 최종 사용자를 URL로 리디렉션하고 클릭(`ef_id`)에 대한 Search, Social 및 Commerce ID도 토큰으로 사용되는 쿼리 문자열 매개 변수로 기록합니다. 오프라인 트랜잭션을 보고하거나, 검색, 소셜 및 Commerce에서 Adobe Analytics과 데이터를 교환하거나, [!DNL Apple Safari] 브라우저 내에서 발생하는 모든 전환을 추적하려는 경우 이 옵션을 선택하십시오.

**메모:**

* [!UICONTROL Standard]에서 [!UICONTROL Token](으)로 전환하거나 그 반대로 전환하는 경우 계정에 대한 추적 URL을 다시 생성해야 합니다.
* 캠페인 수준에서 계정 수준 설정을 재정의할 수 있습니다.
