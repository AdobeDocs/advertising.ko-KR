---
title: ' [!DNL Google Ads] 전환 값 규칙 만들기'
description: ' [!DNL Google Ads] 전환 값 규칙을 만드는 방법을 알아봅니다.'
source-git-commit: e15d34f3f32a8565735e53f1ce40e71008dbb4d9
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 0%

---

# [!DNL Google Ads] 전환 값 규칙 만들기

[!DNL Google Ads] 계정에 계정 수준 및 캠페인 수준 전환 값 규칙을 만들 수 있으며, 이 규칙을 통해 전환은 개별 계정 수준 또는 하위 계정 수준에서 추적됩니다. 마스터 계정 수준에서 추적되는 계정 간 전환이 있는 계정에 대한 규칙을 만들 수 없습니다.

각 규칙에는 최대 2개의 조건과 해당 조건이 충족될 때 적용할 전환값 조정이 포함됩니다. 계정의 모든 규칙은 동일한 유형의 기본 및 (선택 사항) 보조 조건을 사용해야 합니다. 예를 들어 규칙 1에 기본 조건 &quot;대상&quot;과 보조 조건 &quot;위치&quot;가 포함되어 있으면 계정의 다른 모든 규칙에는 기본 조건 &quot;대상&quot;이 있어야 합니다. 다른 규칙에 보조 조건이 포함된 경우 &quot;위치&quot;여야 합니다.

각 캠페인에 대해 여러 캠페인 수준 규칙을 만들 수 있습니다. 그러나 [!DNL Google Ads]은(는) 계정 수준 규칙이 이미 있는 경우 [!DNL Google Ads] 편집기 외부에서 새 계정 수준 규칙을 만들 수 있는 기능을 아직 제공하지 않습니다. 추가 계정 수준 규칙을 만들려면 [!DNL Google Ads]에 직접 로그인한 다음 [!DNL Google Ads] 편집기를 사용하십시오.

**참고:** 캠페인 수준 전환 값 규칙은 계정 수준 규칙을 재정의하며 전환에는 하나의 규칙만 적용할 수 있습니다. 자세한 내용은 [방법 [!DNL Google Ads] 전환이 여러 규칙에 대한 조건을 충족할 때 전환에 적용되는 규칙을 결정합니다](https://support.google.com/google-ads/answer/10520348).

1. 메인 메뉴에서 **[!UICONTROL Goals]>[!UICONTROL Conversion Value Rules]**&#x200B;을(를) 클릭합니다.

   기본적으로 **[!UICONTROL Campaign]** 탭이 선택되어 모든 캠페인 수준 규칙을 표시합니다.

1. (선택 사항) 계정 수준 규칙을 대신 만들려면 **[!UICONTROL Account]** 탭을 클릭합니다.

1. 도구 모음에서 ![만들기](/help/search-social-commerce/assets/add.png "만들기").<!-- Upload newer icon -->를 클릭합니다.

1. 광고 네트워크 및 계정을 선택합니다. 캠페인 수준 규칙의 경우 캠페인도 선택합니다. **[!UICONTROL Next]**&#x200B;을(를) 클릭합니다.

1. [전환 규칙 설정](google-conversion-value-rule-settings.md)을 구성하십시오.

   기본 조건 및 값 조정을 구성해야 합니다. 선택적으로 보조 조건을 구성할 수 있습니다.

   조건 내에서 부울 연산자 OR를 사용하여 여러 대상 또는 제외를 결합하므로 값 조정을 시작하는 데 모든 옵션이 충족될 수 있습니다. 보조 조건을 포함할 때 부울 연산자인 ALL을 사용하여 보조 조건이 기본 조건에 결합되므로 값 조정을 시작하려면 두 조건을 모두 충족해야 합니다. 예: \[위치가 알제리 또는 튀니지\]이고 \[장치가 모바일 또는 태블릿\]인 경우 1.5를 추가합니다.

   **참고:** 계정의 모든 규칙은 같은 유형의 기본 및 (선택 사항) 보조 조건을 사용해야 합니다. 예를 들어 규칙 1에 기본 조건 &quot;대상&quot;과 보조 조건 &quot;위치&quot;가 포함되어 있으면 계정의 다른 모든 규칙에는 기본 조건 &quot;대상&quot;이 있어야 합니다. 다른 규칙에 보조 조건이 포함된 경우 &quot;위치&quot;여야 합니다.

1. 설정을 검토하려면 **[!UICONTROL Review and Save]**&#x200B;을(를) 클릭하십시오.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [정보 [!DNL Google Ads] 전환 값 규칙](about-google-conversion-value-rules.md)
>* [전환 값 규칙 편집 [!DNL Google Ads] 2}](edit-google-conversion-value-rule.md)
>* [전환 값 규칙의 상태 변경 [!DNL Google Ads] ](change-the-status-of-google-conversion-value-rule.md)
>* [[!DNL Google Ads] 전환 값 규칙 설정](google-conversion-value-rule-settings.md)

