---
title: ' [!DNL Flashtalking] 광고 태그에  [!DNL Analytics for Advertising] 매크로 추가'
description: ' [!DNL Flashtalking] 광고 태그에  [!DNL Analytics for Advertising] 매크로를 추가하는 이유와 방법을 알아봅니다.'
feature: Integration with Adobe Analytics
exl-id: ce81824c-60bf-487c-8358-d18fcb3cc95f
source-git-commit: a69bef9d249514f5c494cff8d706b9df792eaf23
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# [!DNL Analytics for Advertising] 매크로를 [!DNL Flashtalking] 광고 태그에 추가

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

*[!DNL Flashtalking]과(와) 직접 파트너 관계가 없는 조직*

*Advertising DSP에만 적용 가능*

Advertising DSP 광고에 [!DNL Flashtalking]의 광고 태그를 사용하는 경우 랜딩 페이지 URL에 추적 매개 변수를 추가해야 합니다. [!DNL Flashtalking]과(와) Advertising DSP 파트너 관계를 사용하려면 랜딩 페이지 URL에 Advertising 매개 변수에 대한 Analytics를 추가하십시오. 매개 변수는 랜딩 페이지 URL에 AMO ID(`s_kwcid`) 및 `ef_id` 쿼리 문자열 매개 변수를 기록하여 Adobe Advertising에서 광고에 대한 클릭 데이터를 Adobe Analytics으로 보낼 수 있도록 합니다.

>[!NOTE]
>
>조직에서 [!DNL Flashtalking]과(와) 직접 파트너 관계를 맺고 있는 경우 이 절차는 필요하지 않습니다. 대신 [!DNL Flashtalking] 계정에 로그인한 다음 [https://support.flashtalking.com/hc/en-us/articles/4409808166419-Accessing-Data-Pass-Macros](https://support.flashtalking.com/hc/en-us/articles/4409808166419-Accessing-Data-Pass-Macros)의 [!DNL Flashtalking] 지원 설명서에 따라 데이터 전달 매크로를 사용하여 `s_kwcid` 및 `ef_id` 추적 매개 변수를 추적하십시오.

다음 유형의 [!DNL Analytics for Advertising] 구현에 대해 [!DNL Flashtalking] 디스플레이 및 비디오 광고용 매크로를 사용합니다.

* **웹 사이트에 [!DNL Adobe] [!DNL Analytics for Advertising] JavaScript 코드가 구현된 광고주**: JavaScript 코드가 이미 AMO ID(`s_kwcid`) 및 `ef_id` 쿼리 문자열 매개 변수를 기록합니다. 그러나 매크로를 사용하면 서드파티 쿠키가 지원되지 않을 때 클릭 기반 전환을 포함하도록 추적이 확장됩니다. 가장 좋은 방법은 다음 섹션의 매크로를 광고 태그에 추가하여 JavaScript 코드를 통해 캡처되지 않은 추가 클릭스루 데이터를 캡처하는 것입니다.

  >[!NOTE]
  >
  >JavaScript 코드는 쿠키를 계속 사용할 수 있는 동안에만 클릭 추적을 위한 솔루션입니다. 쿠키가 중단되면 다음 매크로를 구현해야 합니다.

* **웹 사이트에서 [!DNL Analytics for Advertising] JavaScript 코드를 사용하지 않고 대신 [!DNL Analytics] 서버측 전달을 사용하여 클릭스루 데이터만**(뷰스루 데이터 없음)하는 광고주: 다음 매크로는 Adobe Advertising을 통해 구매하는 광고에서 시작된 온사이트 클릭 활동을 보고하는 데 필요합니다.

## 광고 태그 표시

[!DNL Flashtalking] 광고 태그 설정 내에서 다음 매크로를 `Clicktag` 필드의 클릭스루 URL 끝에 추가합니다.

```
[ftqs:[AdobeAMO]]
```

기본 URL 뒤에 있는 첫 번째 또는 유일한 쿼리 문자열인 경우 `?`을(를) 사용하여 기본 URL에서 구분합니다. 기본 URL에 여러 쿼리 문자열이 포함된 경우 첫 번째 문자열은 `?`로 시작하고 각 후속 문자열은 `&`로 시작합니다.

예:

`https://www.adobe.com/products/photoshop?[ftqs:[AdobeAMO]]`

`https://www.adobe.com/products/photoshop?cid=email&[ftqs:[AdobeAMO]]`

## 비디오 광고 태그

[!DNL Flashtalking] 광고 태그 설정 내에서 다음 매크로를 `Clicktag` 필드의 클릭스루 URL 끝에 추가합니다.

```
[%EL:param['AdobeAMO']%]&s_kwcid=[%EL:param['s_kwcid']%]
```

기본 URL 뒤에 있는 첫 번째 또는 유일한 쿼리 문자열인 경우 `?`을(를) 사용하여 기본 URL에서 구분합니다. 기본 URL에 여러 쿼리 문자열이 포함된 경우 첫 번째 문자열은 `?`로 시작하고 각 후속 문자열은 `&`로 시작합니다.

예:

`https://www.adobe.com/products/photoshop?[%EL:param['AdobeAMO']%]&s_kwcid=[%EL:param['s_kwcid']%]`

`https://www.adobe.com/products/photoshop?cid=email&[%EL:param['AdobeAMO']%]&s_kwcid=[%EL:param['s_kwcid']%]`

>[!MORELIKETHIS]
>
>* [개요 [!DNL Analytics for Advertising]](overview.md)
>* [사용한 Adobe Advertising ID [!DNL Analytics]](/help/integrations/analytics/ids.md)
>* [추가 [!DNL Analytics for Advertising] 매크로를  [!DNL Google Campaign Manager 360] 광고 태그](/help/integrations/analytics/macros-google-campaign-manager.md)에 추가

