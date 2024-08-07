---
source-git-commit: a59b477a6f8a616851d85bf89b58434d4d56cd83
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---
# Google 광고 엔티티에 대한 추적 템플릿 필드

<!-- Search CRUD and bulk edit of Google entity settings -->

**[!UICONTROL Tracking Template]:**(선택 사항) 모든 랜딩 외부 도메인 리디렉션 및 추적 매개 변수를 지정하고 [!DNL ValueTrack] 매개 변수에 최종/랜딩 페이지 URL을 임베드하는 추적 템플릿 또는 추적 URL입니다. 예: 리디렉션을 포함하는 `{lpurl}?source={network}&id=5` 또는 `http://www.trackingservice.example.com/?url={lpurl}?source={network}&id=5`.

캠페인 설정에 &quot;[!UICONTROL EF Redirect]&quot; 및 &quot;[!UICONTROL Auto Upload]&quot;이(가) 포함된 경우 적용되는 Adobe Advertising 전환 추적의 경우 레코드를 저장할 때 Search, Social 및 Commerce에서 자동으로 리디렉션 및 추적 코드 접두사를 추가합니다.

* 최종 URL을 포함하는 데 지원되는 매개 변수에 대해서는 [[!DNL Google Ads] 지원되는  [!DNL ValueTrack] 형식](https://support.google.com/google-ads/answer/6305348)에 대한 설명서를 참조하십시오. (&quot;사용 가능한 [!DNL ValueTrack] 매개 변수&quot;에 대한 섹션의 &quot;추적 템플릿 전용&quot; 매개 변수로 이동하십시오.)

* 필요에 따라 URL 매개 변수와 캠페인에 대해 정의된 사용자 지정 매개 변수를 앰퍼샌드(&amp;)로 구분하여 포함할 수 있습니다(예: {lpurl}?matchtype={matchtype}&amp;device={device}).

* 원할 경우 서드파티 리디렉션 및 추적을 추가할 수 있습니다.

>[!NOTE]
>
>* 병렬 추적을 활성화하는 소스의 클릭에 대체되지 않는 매크로를 사용하지 마십시오. 광고주가 매크로를 사용해야 하는 경우 Adobe 계정 팀은 고객 지원 팀 또는 구현 팀과 협력하여 매크로를 추가해야 합니다.
>* 가장 세분화된 수준의 추적 템플릿은 모든 상위 수준의 값을 재정의합니다. 예를 들어 계정 설정과 키워드 설정 모두에 값이 포함된 경우 키워드 값이 적용됩니다.
>* 광고, 사이트링크 또는 키워드 수준에서 추적 템플릿을 업데이트하는 경우 관련 광고가 다시 제출되어 검토됩니다. 승인을 위해 광고를 다시 제출하지 않고도 계정, 캠페인 또는 광고 그룹 수준에서 추적 템플릿을 업데이트할 수 있습니다.
