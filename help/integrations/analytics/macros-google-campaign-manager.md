---
title: ' [!DNL Google Campaign Manager 360] 광고 태그에  [!DNL Analytics for Advertising] 매크로 추가'
description: ' [!DNL Google Campaign Manager 360] 광고 태그에  [!DNL Analytics for Advertising] 매크로를 추가하는 이유와 방법을 알아봅니다.'
feature: Integration with Adobe Analytics
exl-id: 89cd4e1d-277a-4a43-9c38-ae6641302e09
source-git-commit: aa41ba08ba83bfacbc2541c0f0d90336b3c36305
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# [!DNL Analytics for Advertising] 매크로를 [!DNL Google Campaign Manager 360] 광고 태그에 추가

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

*Advertising DSP에만 적용 가능*

Advertising DSP 광고에 [!DNL Google Campaign Manager 360]의 광고 태그를 사용하는 경우 [`%p` 매크로를 사용하여 [!DNL Analytics for Advertising] 매개 변수를 랜딩 페이지 URL에 추가하십시오](https://support.google.com/campaignmanager/table/6096962). 매개 변수는 랜딩 페이지 URL에 AMO ID(`s_kwcid`) 및 `ef_id` 쿼리 문자열 매개 변수를 기록하여 Adobe Advertising이 광고에 대한 클릭 데이터를 Adobe Analytics으로 보낼 수 있도록 합니다.

다음 유형의 [!DNL Analytics for Advertising] 구현에 대해 [!DNL Campaign Manager 360] 디스플레이 및 비디오 광고용 매크로를 사용합니다.

* **웹 사이트에 [!DNL Adobe] [!DNL Analytics for Advertising] JavaScript 코드가 구현된 광고주**: JavaScript 코드가 이미 AMO ID(`s_kwcid`) 및 `ef_id` 쿼리 문자열 매개 변수를 기록합니다. 그러나 매크로를 사용하면 서드파티 쿠키가 지원되지 않을 때 클릭 기반 전환을 포함하도록 추적이 확장됩니다. 가장 좋은 방법은 다음 섹션의 매크로를 광고 태그에 추가하여 JavaScript 코드를 통해 캡처되지 않은 추가 클릭스루 데이터를 캡처하는 것입니다.

>[!NOTE]
>
>JavaScript 코드는 쿠키를 계속 사용할 수 있는 동안에만 클릭 추적을 위한 솔루션입니다. 쿠키가 중단되면 다음 매크로를 구현해야 합니다.

* **웹 사이트에서 [!DNL Analytics for Advertising] JavaScript 코드를 사용하지 않고 대신 [!DNL Analytics] 서버측 전달을 사용하여 클릭스루 데이터만**(뷰스루 데이터 없음)하는 광고주: 다음 매크로는 Adobe Advertising을 통해 구매하는 광고에서 시작된 온사이트 클릭 활동을 보고하는 데 필요합니다.

## [!DNL Google Campaign Manager 360] 광고에 매크로 추가

[!DNL Google Campaign Manager 360]에서 각 디스플레이 및 비디오 광고의 랜딩 페이지 URL에 다음 매개 변수를 추가합니다. `%pamo=!;`

여러 가지 방법으로 랜딩 페이지 URL을 지정할 수 있습니다. 각 옵션에 대한 지침은 다음 하위 섹션에 포함되어 있습니다.

다음은 접미사 형식의 랜딩 페이지 URL의 예입니다.

```
https://www.adobe.com/home?someparam1=somevalue1&%pamo=!;
```

>[!NOTE]
>
>&#x200B;>* 랜딩 페이지 URL에 일반적이지 않은 해시 기호(#)가 포함되어 있으면 해시 기호 앞에 `amo` 매개 변수를 배치합니다.
>* `amo` 매개 변수 뒤에 다른 매개 변수가 포함되지 않은 경우 그 뒤에 매개 변수(예: &amp;a=b)를 추가합니다. 예: `https://www.adobe.com/home?someparam1=somevalue1&%pamo=!;&a=b#login`

### 광고주 수준 랜딩 페이지 URL 접미사 구성

1. [광고주 속성을 여는 지침](https://support.google.com/campaignmanager/answer/2829344)을 참조하세요.
1. [!UICONTROL Landing page URL suffix] 설정에서 [!UICONTROL URL suffix] 필드에 `%pamo!;`을(를) 포함합니다.

### 캠페인 수준 랜딩 페이지 URL 접미사 구성

1. [캠페인 속성을 여는 지침](https://support.google.com/campaignmanager/answer/2838056#set)을 참조하세요.
1. [!UICONTROL Landing page URL suffix] 설정에서 [!UICONTROL URL suffix] 필드에 `%pamo!;`을(를) 포함합니다.

### 크리에이티브 수준 랜딩 페이지 URL 접미사 구성

1. 크리에이티브 속성을 엽니다.
1. [!UICONTROL Click tags] 설정에서 클릭 태그의 [!UICONTROL Landing page] 열에 `%pamo!;`을(를) 포함합니다.

## DSP에서 [!DNL Analytics for Advertising] 매크로를 확장하는 방법

DSP에서 [!DNL Analytics for Advertising] 매개 변수(`amo`)를 포함하는 광고를 만들면 `ef_id` 및 `s_kwcid` 매크로가 클릭 URL에 자동으로 추가됩니다. 가장 좋은 방법은 DSP에서 태그를 확인하여 `ef_id` 및 `s_kwcid` 매크로가 있는지 확인하는 것입니다.

다음은 DSP에 나타나는 [!DNL Google Campaign Manager 360] [ins 태그](https://support.google.com/campaignmanager/answer/6080468)의 예입니다.

```
<ins class='dcmads' style='display:inline-block;width:160px;height:600px'
data-dcm-placement='N6482.2155306TUBEMOGUL/B23486129.261313631'
data-dcm-rendering-mode='iframe'
data-dcm-https-only
data-dcm-resettable-device-id=''
data-dcm-app-id='' data-dcm-click-tracker='${TM_CLICK_URL}'
data-dcm-param-amo='ef_id=${TM_USER_ID}:${TM_DATETIME}:d&s_kwcid=AC!${TM_AD_ID}!${TM_PLACEMENT_ID}'>
<script src='https://www.googletagservices.com/dcm/dcmads.js'></script>
</ins>
```

사용자가 광고를 클릭하면 [!DNL Google Campaign Manager 360]에 URL 접미사에 `%pamo`이(가) 표시되고 `amo` 매개 변수의 값이 URL에 동적으로 삽입됩니다.

>[!MORELIKETHIS]
>
>* [개요 [!DNL Analytics for Advertising]](overview.md)
>*  [!DNL Analytics][&#128279;](/help/integrations/analytics/ids.md)에서 사용하는 Adobe Advertising ID
>* [추가 [!DNL Analytics for Advertising] 매크로를  [!DNL Flashtalking] 광고 태그](macros-flashtalking.md)에 추가
