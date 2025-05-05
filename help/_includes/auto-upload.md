---
source-git-commit: bef353542ee73d32b8ac53e6abd3265528be154f
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---
# 계정 및 캠페인 설정의 자동 업로드 필드

**[!UICONTROL Auto Upload]:**([!UICONTROL EF Redirect]이(가) 있는 동기화된 캠페인의 경우에만) 다음에 검색, 소셜 및 Commerce이 이 템플릿과 동기화할 때 광고 네트워크에 자동으로 다음 항목을 업로드합니다. (a) 추적 템플릿에 대한 검색, 소셜 및 Commerce 추적 매개 변수와 최종 URL에 추가된 동일한 매개 변수 또는 (b) 검색, 소셜 및 Commerce 추적 코드에 포함된 새 대상 URL. [Adobe Advertising-Adobe Analytics 통합](https://experienceleague.adobe.com/docs/advertising/integrations/analytics/overview.html?lang=ko)과 서버측 AMO ID(s_kwcid) 구성이 있는 광고주의 경우 업로드에는 [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 계정에 대한 [AMO ID 매개 변수](/help/integrations/analytics/ids.md#amo-id)도 포함됩니다. 기본 계정 수준 설정은 광고주의 추적 설정에서 상속됩니다. 캠페인 수준에서 계정 수준 설정을 재정의할 수 있습니다.

**참고:** 추적 URL은 동기화되지 않은 엔터티(즉, 추가된 새 엔터티 및 속성이 변경된 기존 엔터티)에 대해서만 매일 업데이트됩니다. 따라서 기존 광고주/계정/캠페인에 대해 이 설정을 비활성화에서 활성화로 변경하면 이미 동기화 중인 기존 엔티티에 대한 추적 URL이 업데이트되지 않습니다. 동기화 중인 기존 엔터티의 URL에 추적을 추가하려면 Adobe 계정 팀에 연락하여 1회 수동 동기화 프로세스를 요청하십시오. 자동 업로드 프로세스는 향후 변경 사항을 처리합니다.
