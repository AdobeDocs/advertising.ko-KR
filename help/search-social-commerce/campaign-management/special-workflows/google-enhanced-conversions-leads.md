---
title: 리드에 대해  [!DNL Google Ads] 향상된 전환 구현
description: 리드에 대해  [!DNL Google Ads] 향상된 전환을 설정하는 워크플로에 대해 알아봅니다.
feature: Search Campaign Management, Conversions
exl-id: b708c9f2-2962-45d9-8780-4e96ef2ae8f7
source-git-commit: 56161ece4ba9c01cddb86e16796150c391f1a811
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# 리드에 대해 [!DNL Google Ads] 향상된 전환 구현

*[!DNL Google Ads]개의 계정만*

[[!DNL Google Ads] 잠재 고객에 대한 향상된 전환](https://support.google.com/google-ads/answer/9888656)을 통해 자사 전환 데이터를 사용하여 사용자를 오프라인 전환에 매핑할 수 있습니다. 웹 사이트 잠재 고객의 결과로 발생하는 전화 또는 이메일 판매 추적과 같이 클릭 ID를 사용할 수 없는 환경에서 잠재 고객에 대해 향상된 전환 기능을 사용합니다.

검색, 소셜 및 Commerce 내에서 다음 작업을 수행할 수 있습니다.

* 잠재 고객에 대한 기존 향상된 전환 보기

  검색, 소셜 및 Commerce은 광고주 시간대의 05:00에 매일 리드에 대한 기존 강화 전환을 동기화합니다.

* 잠재 고객에 대한 향상된 전환 만들기

* 자사 오프라인 전환 데이터를 업로드하여 리드에 대한 향상된 전환에 매핑합니다.

* 보고서 내의 지표와 최적화 목표 내의 가중 지표로 잠재 고객에 대한 향상된 전환을 포함합니다.

이 기능을 사용하려면 다음 단계를 완료하십시오. 전환 추적 태그를 만드는 단계와 전환 작업을 만드는 단계는 선택적으로 되돌릴 수 있습니다.

1. [!DNL Google Ads] 내에서 잠재 고객에 대한 향상된 전환을 옵트인합니다.

   1. 계정의 전환 설정을 엽니다.

   1. 잠재 고객에 대한 향상된 전환 옵션을 선택하고 서비스 약관에 동의합니다.

   1. [!DNL Google] 태그를 사용할지 [!DNL Google Tag Manager]을(를) 사용하여 변환 태그를 만들지 선택합니다.


1. 전환 작업에 대한 [!DNL Google] 태그를 구성하고 구현합니다.

   지침은 [a [!DNL Google] tag](https://support.google.com/google-ads/answer/11021502) 또는 [using [!DNL Google Tag Manager]](https://support.google.com/google-ads/answer/11347292) 리드에 대한 향상된 전환을 위한 태그를 만드는 [!DNL Google Ads] 도움말을 참조하세요.

1. [검색, 소셜 및 Commerce](/help/search-social-commerce/admin/conversion-metrics/conversion-action-google.md) 또는 [Google 광고](https://support.google.com/google-ads/answer/12216226) 내에서 잠재 고객에 대한 향상된 전환에 대한 전환 작업을 만듭니다.

   **전환 유형에 대해** *전환 가져오기* 또는 *가져오기를 선택합니다.*

1. 필요한 경우 해시된 이메일 주소 또는 전화 번호를 포함한 자사 데이터를 업로드하여 지정된 계정에 대한 전환에 기여합니다. [검색, 소셜 및 Commerce](/help/search-social-commerce/admin/conversion-metrics/upload-data-offline-conversions.md) 내에서 또는 [!DNL Google Data Manager]을(를) 사용하여 이 단계를 완료할 수 있습니다.

   * 검색, 소셜 및 Commerce 내에서 [!DNL Microsoft Excel] 형식으로 템플릿을 다운로드하고, 변환 데이터를 입력하고 로컬에 파일을 저장한 다음 편집된 파일을 업로드할 수 있습니다. 템플릿에는 광고 및 개인화 목적으로 [!DNL Google]에 데이터를 업로드하는 데 동의했는지 여부를 나타내는 열이 포함되어 있습니다.

     업로드된 모든 데이터는 실시간으로 [!DNL Google Ads]에 동기화됩니다.

   * [!DNL Google Data Manager]을(를) 사용하여 데이터를 업로드하는 방법에 대한 자세한 내용은 &quot;[데이터 관리자 정보](https://support.google.com/google-ads/answer/14639041)&quot;를 참조하십시오.

>[!MORELIKETHIS]
>
>* [잠재 고객에 대한 전환 작업 만들기 [!DNL Google Ads] 향상된 전환](/help/search-social-commerce/admin/conversion-metrics/conversion-action-google.md)
>* [향상된 전환을 위해 오프라인 전환 데이터 업로드](/help/search-social-commerce/admin/conversion-metrics/upload-data-offline-conversions.md)
