---
title: (새 UI)  [!DNL Google Ads] 향상된 잠재 고객 전환에 대한 전환 작업 만들기
description: 잠재 고객에 대한 향상된 전환을 위해  [!DNL Google Ads] 전환 작업을 만드는 방법을 알아봅니다.
feature: Conversions
feature_v2: id: aed5e38a-3e62-42fa-8d16-cd080729b2a0id: e6916c1b-e939-4e0b-99f5-768e83e1e99f
subfeature_v2: id: d068b149-b9d1-421c-9033-a51495366ddc
source-git-commit: 0bfee2b52410b5cab8e9b3dfba35effc36fc40e1
workflow-type: tm+mt
source-wordcount: 510
ht-degree: 0%

---

# (새 UI) [!DNL Google Ads] 향상된 잠재 고객 전환에 대한 전환 작업 만들기

*Beta 기능*

*[!DNL Google Ads]개의 계정만*

관리자 계정 수준에서 추적되는 전환이 아니라 개별 [!DNL Google Ads] 계정에 대해 추적할 잠재 고객에 대한 [!DNL Google Ads] 향상된 전환에 대한 전환 작업을 만들 수 있습니다.

전환 작업을 만들고 전환 추적 태그를 구현하면 [조직에서 캡처한 오프라인 전환 데이터를 업로드](conversions-upload-offline-enhanced-conversions.md)하고 전환 작업에 연결할 수 있습니다.

[!DNL Microsoft Advertising] 계정에 대한 지원을 사용할 수 없습니다.

## 전환 작업 만들기

1. 메인 메뉴에서 **[!UICONTROL Goals]>[!UICONTROL Conversions]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위에서 **[!UICONTROL Set up Conversion]**&#x200B;을(를) 클릭합니다.

1. [전환 작업 설정](#conversion-action-settings-google)을 지정하십시오.

   1. [!UICONTROL Setup Method] *[!UICONTROL Create Conversion]*&#x200B;을(를) 선택하십시오.

   1. 계정을 선택한 다음 전환 유형을 선택합니다. *[!UICONTROL Import conversion]*.

   1. **[!UICONTROL Next]**&#x200B;을(를) 클릭합니다.

   1. 전환 작업 옵션을 지정합니다.

   1. 설정을 검토하려면 **[!UICONTROL Review and Save]**&#x200B;을(를) 클릭하십시오.

   1. **[!UICONTROL Generate]**&#x200B;을(를) 클릭합니다.

1. 잠재 고객에 대한 향상된 전환을 위해 추적 태그를 만드는 방법에 대한 정보를 읽은 다음 **[!UICONTROL Next]**&#x200B;을(를) 클릭합니다.

   전환 지표를 추적하려는 웹 사이트에서 필요할 경우 전환 태그를 만들어 구현해야 합니다. 또한 잠재 고객에 대해 향상된 전환을 활성화하고 고객 데이터 이용 약관에 동의해야 합니다. 지침은 [!DNL Google Ads]의 &quot;[잠재 고객에 대한 향상된 전환을 위해  [!DNL Google] 태그를 구성](https://support.google.com/google-ads/answer/11021502)&quot;하는 지침을 참조하십시오.

   트랜잭션별 전환 값을 추적하려면 [이벤트 코드 조각을 사용자 지정](https://support.google.com/google-ads/answer/6095947)하세요.

1. **[!UICONTROL Close].** 클릭

## 전환 작업 설정 {#conversion-action-settings-google}

### 경로 설정 섹션

**[!UICONTROL Setup Method]:** 동작 유형: *[!UICONTROL Create Conversion]*

**[!UICONTROL Platform]:** 광고 네트워크: *[!UICONTROL Google]*.

### 전환 세부 정보 섹션

**[!UICONTROL Select Account]:** 적용 가능한 [!DNL Google Ads] 계정입니다.

**[!UICONTROL Type of conversions]:** 추적할 변환 유형: *[!UICONTROL Import conversion]*&#x200B;을(를) 선택합니다. 다른 모든 유형은 다른 유형의 전환에 대한 전환 추적 태그(전환 작업 아님)를 만드는 데 사용됩니다.

### 전환 설정 섹션

**[!UICONTROL Conversion Name]:** 변환 작업의 고유한 이름입니다.

**[!UICONTROL Goal Category]:** 전환 범주(예: *적격 잠재 고객* 또는 *등록*).

**[!UICONTROL Preferred Action optimization]:** 목표가 *[!UICONTROL Primary action used for bidding optimization]*&#x200B;인지 *[!UICONTROL Secondary action not used for bidding optimization]*&#x200B;인지 여부.

**[!UICONTROL Conversion Value]:** 각 전환의 [값을 측정하는 방법](https://support.google.com/google-ads/answer/13064207):

* 통화를 선택하고 각 전환에 대한 값을 입력해야 하는 *[!UICONTROL Use the same value for each conversion],*.

* 통화를 선택하고 각 전환에 대한 기본값을 입력해야 하는 *[!UICONTROL Use different values for each conversion],*. 특정 웹 페이지에서 태그를 구현할 때 태그에서 기본값을 트랜잭션 특정 값으로 변경할 수 있습니다.

* *[!UICONTROL Don't use a value for this conversion action (Not recommended)]*

**[!UICONTROL Count]:** [클릭당 또는 상호 작용당 카운트할 전환 수](https://support.google.com/google-ads/answer/3438531): *[!UICONTROL Every (Recommended for every purchases because every purchase is valuable)]* 또는 *[!UICONTROL One (Recommended for leads, sign-ups and other conversions for which only the first interaction is valuable)]*.

**[!UICONTROL Click-Through Conversion Window]:** 전환이 기록된 광고 상호 작용 후 최대 일 수입니다. 검색, 표시 및 쇼핑 캠페인의 경우 기간은 1~90일 사이일 수 있습니다. 숫자를 선택하거나 **[!UICONTROL Custom]**&#x200B;을(를) 선택하고 숫자를 입력하세요.

**[!UICONTROL View-Through Conversion Window]:** 사용자가 광고를 본 후 뷰스루 전환이 기록된 최대 일 수입니다. 검색, 표시 및 쇼핑 캠페인의 경우 기간은 1~90일 사이일 수 있습니다. 숫자를 선택하거나 **[!UICONTROL Custom]**&#x200B;을(를) 선택하고 숫자를 입력하세요.

**[!UICONTROL Attribution Model]:** [각 광고 상호 작용의 크레딧을 결정하는 속성 모델](https://support.google.com/google-ads/answer/6259715?sjid=8211249329930775138): *[!UICONTROL Data driven]* 또는 *[!UICONTROL Last click]*.

>[!MORELIKETHIS]
>
>* [(새 UI) 향상된 전환을 위해 오프라인 전환 데이터 업로드](/help/search-social-commerce/admin/conversion-metrics/upload-data-offline-conversions.md)
>* [향상된 전환을 위해 오프라인 전환 데이터 업로드](/help/search-social-commerce/admin/conversion-metrics/upload-data-offline-conversions.md)
>* [잠재 고객에 대한  [!DNL Google Ads] 향상된 전환 구현](/help/search-social-commerce/campaign-management/special-workflows/google-enhanced-conversions-leads.md)
