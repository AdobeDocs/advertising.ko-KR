---
source-git-commit: 38d6d70d03c12aab1a7caee6e589a2fdeaf78ad4
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---
# Microsoft 광고 엔티티에 대한 추적 템플릿 필드

<!-- Search CRUD and bulk edit of Microsoft entity settings -->

**[!UICONTROL Tracking Template]:** (선택 사항, 모든 엔티티에 사용할 수 없음) 모든 오프랜딩 도메인 리디렉션 및 추적 매개 변수를 지정하고 또한 최종/랜딩 페이지 URL을 매개 변수에 임베드하는 추적 템플릿 또는 추적 URL입니다. 예: `{lpurl}?source={network}&id=5` 또는 `http://www.trackingservice.example.com/?url={lpurl}?source={network}&id=5` 리디렉션을 포함합니다.

Adobe Advertising 전환 추적의 경우, 캠페인 설정에 이 포함되어 있을 때 적용됩니다.[!UICONTROL EF Redirect]&quot; 및 &quot;[!UICONTROL Auto Upload],&quot; Search, Social 및 Commerce는 레코드를 저장할 때 자체 리디렉션 및 추적 코드 접두사를 자동으로 추가합니다.

* 최종 URL을 포함하도록 지원되는 매개 변수에 대해 다음을 참조하십시오. [[!DNL Microsoft Advertising] 최종 URL을 나타내는 매개 변수에 대한 설명서](https://help.ads.microsoft.com/#apex/3/en/56799).

* 필요에 따라 URL 매개 변수와 캠페인에 대해 정의된 사용자 지정 매개 변수를 앰퍼샌드(&amp;)로 구분하여 포함할 수 있습니다. {lpurl}?matchtype={matchtype}장치(&amp;d)={device}.

* 원할 경우 서드파티 리디렉션 및 추적을 추가할 수 있습니다.

<!-- Some entities may need additional/different notes. Try to keep this applicable to all MS entities. -->

>[!NOTE]
>
>* 가장 세분화된 수준의 추적 템플릿은 모든 상위 수준의 값을 재정의합니다. 예를 들어 계정 설정과 키워드 설정 모두에 값이 포함된 경우 키워드 값이 적용됩니다.
>* 승인을 위해 광고를 다시 제출하지 않고도 원하는 수준에서 추적 템플릿을 업데이트할 수 있습니다.
