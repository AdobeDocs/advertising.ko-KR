---
source-git-commit: 6e5d79eb9c04a12813c42e33a2228c69f2adbaae
workflow-type: tm+mt
source-wordcount: '151'
ht-degree: 0%

---
# 최종 URL 접미사 정의

<!-- Used in many places; in inventory feed templates, it's actually called "Campaign Final URL Suffix," but leaving this generic anyway since it's a paragraph-level include file -->

**[!UICONTROL Final URL Suffix]:** ([!DNL Google Ads] 및 [!DNL Microsoft Advertising] accounts only; 선택 사항) 정보를 추적하기 위해 최종 URL 끝에 추가하는 모든 매개 변수. 비즈니스에서 추적해야 하는 모든 매개 변수를 포함합니다. 예:`param1=value1&param2=value2`

Adobe Advertising 전환 추적을 사용하는 계정에서 접미사에 광고 네트워크의 클릭 식별자(`msclkid` 대상 [!DNL Microsoft Advertising]; `gclid` 대상 [!DNL Google Ads]).

Adobe Analytics 통합이 있는 계정은 [AMO ID](/help/integrations/analytics/ids.md) 매개 변수. 계정에 서버측 AMO ID 구현이 있는 경우 사용자가 광고를 클릭하면 매개 변수가 자동으로 추가됩니다. 그렇지 않으면 여기에 매개 변수를 수동으로 추가해야 합니다. 다음을 참조하십시오. [필수 접미어 형식 [!DNL Google Ads]](/help/search-social-commerce/tracking/formats-click-tracking-google.md) 및 [필수 접미어 형식 [!DNL Microsoft Advertising]](/help/search-social-commerce/tracking/formats-click-tracking-microsoft.md).

>[!NOTE]
>
>* 이 필드는 다음에 의해 업데이트되지 않습니다. [!UICONTROL Auto Upload] 추적 설정입니다.
>* 하위 수준의 최종 URL 접미사는 계정 수준 접미사를 덮어씁니다. 간편하게 유지 관리할 수 있도록 개별 계정 구성 요소에 대해 다른 추적이 필요하지 않은 경우 계정 수준 접미사만 사용하십시오. 광고 그룹 수준 또는 하위 수준에서 접미사를 구성하려면 광고 네트워크의 편집기를 사용합니다.
