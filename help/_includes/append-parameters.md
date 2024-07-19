---
source-git-commit: 05b9a55e19c9f76060eedb35c41cdd2e11753c24
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---
# 계정 및 캠페인 설정의 매개 변수 필드 추가

**[!UICONTROL Append Parameters]:**(선택 사항) 기본 URL에 추가할 추가 추적 매개 변수입니다.<!-- When account uses setting append_param_to_tt_fus, then we add append parameters to the tracking templates OR the landing page suffixes instead (not sure how we determine which) -->. 광고주 수준 추가 매개 변수는 계정 수준 및 캠페인 수준에서 기본적으로 포함되지만, 어느 것이든 재정의할 수 있습니다.

타사 추적 매개 변수를 비롯한 모든 정적 텍스트 문자열 또는 기본 URL에 적절한 데이터 값을 삽입하는 [지원되는 추적 매개 변수](/help/search-social-commerce/tracking/click-tracking-urls-optional-parameters.md)를 사용할 수 있습니다.

여러 매개 변수는 쉼표 또는 앰퍼샌드(&amp;)로 구분하십시오. 중첩된 대괄호는 지원되지 않습니다.

**메모:**

* 매개 변수를 추가하는 변경 내용은 [!UICONTROL Auto Upload] 옵션에 의해 제어되지 않습니다. 기존 기본 URL에 대한 추가 매개 변수를 변경하면 새 URL이 자동으로 생성되지 않습니다. 계정 또는 캠페인에 대한 일괄 시트 파일을 다운로드하고 [!UICONTROL Base URL/Final URL] 필드를 업데이트한 다음 일괄 시트를 업로드하고 게시하여 새 매개 변수를 추가합니다.

* (병렬 추적을 사용하는 광고 네트워크) 병렬 추적을 활성화하는 소스의 클릭에 대체되지 않는 매크로를 사용하지 마십시오. 광고주가 매크로를 사용해야 하는 경우 Adobe 계정 팀은 고객 지원 팀 또는 구현 팀과 협력하여 매크로를 추가해야 합니다.

* (Adobe Advertising-Adobe Analytics 통합을 사용하는 광고주) 검색, 소셜 및 Commerce 데이터를 [!DNL Analytics]에 보낼 AMO ID 매개 변수를 포함하려면 [광고 네트워크별 형식](/help/integrations/analytics/ids.md#amo-id-formats)을 참조하세요. 서버측 AMO ID 구현으로 [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 계정에 대한 매개 변수를 수동으로 추가할 필요는 없습니다.
