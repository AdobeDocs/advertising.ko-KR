---
source-git-commit: 029e406fbfb4217ce78364c2d1f1a6dae24ff588
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---
# 코드 조각

## Google 광고 엔티티에 대한 추적 템플릿 필드 {#tracking-template-google}

<!-- Duplicated from include file because one file has multiple occurrences, which ExL doesn't support. -->

**[!UICONTROL Tracking Template]:** (선택 사항) 모든 오프랜딩 도메인 리디렉션 및 추적 매개 변수를 지정하고 또한 최종/랜딩 페이지 URL을 임베드하는 추적 템플릿 또는 추적 URL [!DNL ValueTrack] 매개 변수. 예: `{lpurl}?source={network}&id=5` 또는 `http://www.trackingservice.example.com/?url={lpurl}?source={network}&id=5` 리디렉션을 포함합니다.

캠페인 설정에 &quot;&quot;가 포함된 경우 적용되는 Adobe 광고 전환 추적의 경우[!UICONTROL EF Redirect]&quot; 및 &quot;[!UICONTROL Auto Upload],&quot; Search, Social 및 Commerce는 레코드를 저장할 때 자체 리디렉션 및 추적 코드 접두사를 자동으로 추가합니다.

* 최종 URL을 포함하도록 지원되는 매개 변수에 대해 다음을 참조하십시오. [[!DNL Google Ads] documentation for the supported [!DNL ValueTrack] 형식](https://support.google.com/google-ads/answer/6305348). (&quot;사용 가능한 ValueTrack 매개 변수&quot; 섹션의 &quot;추적 템플릿만&quot; 매개 변수로 이동합니다.)

* URL 매개 변수와 캠페인에 대해 정의된 모든 사용자 지정 매개 변수를 앰퍼샌드(&amp;)로 구분하여 선택적으로 포함할 수 있습니다(예: {lpurl}?matchtype={matchtype}&amp;device={device}).

* 원할 경우 서드파티 리디렉션 및 추적을 추가할 수 있습니다.

>[!NOTE]
>
>* 병렬 추적을 활성화하는 소스의 클릭에 대체되지 않는 매크로를 사용하지 마십시오. 광고주가 매크로를 사용해야 하는 경우 Adobe 계정 팀은 고객 지원 팀 또는 구현 팀과 협력하여 매크로를 추가해야 합니다.
>* 가장 세분화된 수준의 추적 템플릿은 모든 상위 수준의 값을 재정의합니다. 예를 들어 계정 설정과 키워드 설정 모두에 값이 포함된 경우 키워드 값이 적용됩니다.
>* 광고, 사이트링크 또는 키워드 수준에서 추적 템플릿을 업데이트하는 경우 관련 광고가 다시 제출되어 검토됩니다. 승인을 위해 광고를 다시 제출하지 않고도 계정, 캠페인 또는 광고 그룹 수준에서 추적 템플릿을 업데이트할 수 있습니다.


## Microsoft 광고 엔티티에 대한 추적 템플릿 필드 {#tracking-template-microsoft}

<!-- Search CRUD and bulk edit of Microsoft entity settings -->

**[!UICONTROL Tracking Template]:** (선택 사항) 모든 오프랜딩 도메인 리디렉션 및 추적 매개 변수를 지정하고 또한 최종/랜딩 페이지 URL을 매개 변수에 임베드하는 추적 템플릿 또는 추적 URL. 예: `{lpurl}?source={network}&id=5` 또는 `http://www.trackingservice.example.com/?url={lpurl}?source={network}&id=5` 리디렉션을 포함합니다.

캠페인 설정에 &quot;&quot;가 포함된 경우 적용되는 Adobe 광고 전환 추적의 경우[!UICONTROL EF Redirect]&quot; 및 &quot;[!UICONTROL Auto Upload],&quot; Search, Social 및 Commerce는 레코드를 저장할 때 자체 리디렉션 및 추적 코드 접두사를 자동으로 추가합니다.

* 최종 URL을 포함하도록 지원되는 매개 변수에 대해 다음을 참조하십시오. [[!DNL Microsoft Advertising] 최종 URL을 나타내는 매개 변수에 대한 설명서](https://help.ads.microsoft.com/#apex/3/en/56799).

* URL 매개 변수와 캠페인에 대해 정의된 모든 사용자 지정 매개 변수를 앰퍼샌드(&amp;)로 구분하여 선택적으로 포함할 수 있습니다(예: {lpurl}?matchtype={matchtype}&amp;device={device}).

* 원할 경우 서드파티 리디렉션 및 추적을 추가할 수 있습니다.

<!-- Some entities may need additional/different notes. Try to keep this applicable to all MS entities. -->

>[!NOTE]
>
>* 가장 세분화된 수준의 추적 템플릿은 모든 상위 수준의 값을 재정의합니다. 예를 들어 계정 설정과 키워드 설정 모두에 값이 포함된 경우 키워드 값이 적용됩니다.
>* 승인을 위해 광고를 다시 제출하지 않고도 원하는 수준에서 추적 템플릿을 업데이트할 수 있습니다.


## 텍스트 광고 템플릿 - 동적 매개 변수를 삽입하는 방법을 설명하는 참고 사항 {#inventory-feed-template-insert-dynamic-parameter}

열 이름이나 수정자 그룹을 동적 매개 변수로 삽입하려면 입력 필드를 클릭한 다음 열 목록 또는 [수정자 이름](/help/search-social-commerce/campaign-management/inventory-feeds/modifiers-manage.md) 을 클릭합니다. 을(를) 삽입하려면 [!DNL Param1] 또는 [!DNL Param2] 변수에 값을 입력합니다. `{param1:default text}` 또는 `{param2:default text}`여기서 &quot;기본 텍스트&quot;는 피드 파일의 매개 변수 열이 광고 행에 대해 비어 있는 경우 사용되는 텍스트입니다.

## 텍스트 광고 템플릿 - 광고 사용자 정의자를 삽입하는 방법을 설명하는 참고 사항 {#inventory-feed-template-insert-ad-customizer}

광고 사용자 정의자를 삽입하려면 다음 형식을 사용하십시오. `Default text` 는 피드 파일에 유효한 값이 포함되지 않았을 때 삽입할 선택적 값입니다.

* [!DNL Google Ads]: `{CUSTOMIZER.AdCustomizerName:Default text}`, 예: `{CUSTOMIZER.Discount:10%}`

* [!DNL Microsoft Advertising]: `{CUSTOMIZER.Attribute name:Default text}`, 예: `{CUSTOMIZER.Discount:10%}`
