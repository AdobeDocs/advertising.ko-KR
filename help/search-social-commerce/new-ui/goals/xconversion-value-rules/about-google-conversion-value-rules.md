---
title: ' [!DNL Google Ads] 전환 값 규칙 정보'
description: 검색, 소셜 및 Commerce에서  [!DNL Google Ads] 전환 값 규칙을 보고 관리하는 방법을 알아봅니다.
source-git-commit: e15d34f3f32a8565735e53f1ce40e71008dbb4d9
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---

# [!DNL Google Ads]개 전환 값 규칙 정보

Search, Social 및 Commerce은 [ 계정의 ](https://support.google.com/google-ads/answer/10518330)전환 값 규칙[!DNL Google Ads]을 자동으로 동기화합니다. 전환 값 규칙을 사용하면 장치 유형, 위치 및 대상 세그먼트를 포함한 사용자 정보를 기반으로 전환 이벤트의 값을 조정할 수 있습니다. Google 스마트 입찰을 사용하여 검색, 디스플레이, 쇼핑 및 성과 최대 캠페인에서 가치 기반 입찰에 대한 규칙을 사용할 수 있습니다. 전환 최대화 및 Target ROAS 입찰 전략이 있는 캠페인의 경우 [!DNL Google Ads] 알고리즘이 더 높은 값으로 전환을 선호하기 시작합니다.

캠페인 수준 전환 값 규칙은 계정 수준 규칙을 재정의합니다. 전환이 여러 전환 값 규칙을 충족하면 규칙 중 하나만 적용됩니다. 일반적으로 가장 구체적인 규칙이 적용되지만, 다른 규칙 조건 유형의 우선 순위에 대해서는 [[!DNL Google Ads] 설명서를 참조하십시오](https://support.google.com/google-ads/answer/10520348).

## [!UICONTROL Conversion Value Rules] 보기 및 기능

[!DNL Google Ads] 인터페이스에서 만든 모든 규칙은 24시간 내에 동기화되며 [!UICONTROL Goals] > [!UICONTROL Conversion Value Rules] 보기에서 사용할 수 있습니다. 일부 계정은 전환 값 규칙을 관리할 수 있습니다.

* 개별 계정 또는 캠페인 수준에서 전환이 추적되는 계정에서 계정 수준 및 캠페인 수준 규칙을 만들고, 편집하고, 상태를 변경할 수 있습니다.

  계정은 [!DNL Google Ads] 관리자 계정에 연결할 수 있지만 계정 간 전환 추적을 사용할 수 없습니다(이 경우 관리자 계정의 모든 계정에서 전환이 추적됨).

* 계정 간 전환 추적을 사용하는 계정의 계정 수준 및 캠페인 수준 규칙은 관리자 계정에서 상속되며 읽기 전용입니다.

## 검색, 소셜 및 Commerce 포트폴리오가 있는 전환 값 규칙

광고주 계정이 검색, 소셜 및 Commerce 목표를 [!DNL Google Ads]에 업로드하도록 구성되어 있고 목표가 있는 포트폴리오에 전환 값 규칙을 사용하는 캠페인을 포함하면 [!DNL Google Ads]이(가) 목표에 지정된 원래 전환 값에 전환 값 규칙을 적용합니다. 따라서 Search, Social 및 Commerce의 전환 데이터가 [!DNL Google Ads]의 전환 데이터와 다릅니다.

예를 들어 목표가 단일 전환 지표 &quot;잠재 고객&quot;을 사용하고 모바일 장치에서 전환한 가중치를 10으로 제공하고 비모바일 장치에서 전환한 가중치를 10으로 제공한다고 가정해 보겠습니다. Search, Social 및 Commerce은 두 장치 유형의 이벤트를 1개의 전환으로 계산하고 전환 값을 10으로 크레딧합니다. 그러나 해당 포트폴리오의 캠페인이 전환 값 규칙 &quot;장치가 모바일인 경우 2를 곱하십시오.&quot;를 사용한다고 가정해 봅시다. 해당 캠페인에 대해 모바일 잠재 고객 이벤트가 추적되면 [!DNL Google Ads]도 전환 수를 1로 크레딧하지만 전환 값은 (10 x 2) = 20으로 크레딧합니다.

규칙이 적용되기 전의 원래 전환 값을 포함하여 규칙에 대한 자세한 내용은 [의 전환 값 규칙 보고서 [!DNL Google Ads]](https://support.google.com/google-ads/answer/10519848)를 참조하십시오.

>[!MORELIKETHIS]
>
>* [전환 값 규칙 만들기 [!DNL Google Ads] 2}](create-google-conversion-value-rule.md)
>* [전환 값 규칙 편집 [!DNL Google Ads] 2}](edit-google-conversion-value-rule.md)
>* [전환 값 규칙의 상태 변경 [!DNL Google Ads] ](change-the-status-of-google-conversion-value-rule.md)
>* [[!DNL Google Ads] 전환 값 규칙 설정](google-conversion-value-rule-settings.md)

