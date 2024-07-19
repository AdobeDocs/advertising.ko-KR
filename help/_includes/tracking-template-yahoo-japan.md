---
source-git-commit: 029e406fbfb4217ce78364c2d1f1a6dae24ff588
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 0%

---
# Yahoo!에 대한 추적 템플릿 필드 일본 광고 엔티티

<!-- Search CRUD and bulk edit of Yahoo! Japan Ads entity settings -->

**[!UICONTROL Tracking Template]:**(선택 사항) 모든 랜딩 외부 도메인 리디렉션 및 추적 매개 변수를 지정하고 매개 변수에 최종/랜딩 페이지 URL을 임베드하는 추적 템플릿 또는 추적 URL입니다. `!{lpurl}` 매개 변수를 사용하여 랜딩 페이지 URL을 지정하십시오. 예: 리디렉션을 포함하는 `{lpurl}?source={network}&id=5` 또는 `http://www.trackingservice.example.com/?url={lpurl}?source={network}&id=5`.

원할 경우 서드파티 리디렉션 및 추적을 추가할 수 있습니다.

캠페인 설정에 &quot;[!UICONTROL EF Redirect]&quot; 및 &quot;[!UICONTROL Auto Upload]&quot;이(가) 포함된 경우 적용되는 Adobe Advertising 전환 추적의 경우 레코드를 저장할 때 Search, Social 및 Commerce에서 자동으로 리디렉션 및 추적 코드 접두사를 추가합니다.

>[!NOTE]
>
>* 가장 세분화된 수준의 추적 템플릿은 모든 상위 수준의 값을 재정의합니다. 예를 들어 계정 설정과 키워드 설정 모두에 값이 포함된 경우 키워드 값이 적용됩니다.
>* 승인을 위해 광고를 다시 제출하지 않고도 원하는 수준에서 추적 템플릿을 업데이트할 수 있습니다.
