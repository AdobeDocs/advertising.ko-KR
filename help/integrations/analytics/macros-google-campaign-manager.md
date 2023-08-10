---
title: 추가 [!DNL Analytics for Advertising] 매크로 위치 [!DNL Google Campaign Manager 360] 광고 태그
description: 추가 이유 및 방법 알아보기 [!DNL Analytics for Advertising] 에 대한 매크로 [!DNL Google Campaign Manager 360] 광고 태그
feature: Integration with Adobe Analytics
exl-id: 89cd4e1d-277a-4a43-9c38-ae6641302e09
source-git-commit: 703cda43e96dfa9d80bbce2d64192fc461d5dbae
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# 추가 [!DNL Analytics for Advertising] 매크로 위치 [!DNL Google Campaign Manager 360] 광고 태그

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

*Advertising DSP에만 적용 가능*

에서 광고 태그를 사용하는 경우 [!DNL Google Campaign Manager 360] Advertising DSP 광고의 경우 다음을 추가합니다. [!DNL Analytics for Advertising] 를 사용하여 랜딩 페이지 URL에 대한 매개 변수 [`%p` 매크로](https://support.google.com/campaignmanager/table/6096962). 매개 변수는 AMO ID(`s_kwcid`) 및 `ef_id` Adobe Advertising이 Adobe Analytics에 광고에 대한 클릭 데이터를 전송할 수 있도록 랜딩 페이지 URL의 쿼리 문자열 매개 변수.

다음에 대한 매크로 사용 [!DNL Campaign Manager 360] 다음 유형의 디스플레이 및 비디오 광고 [!DNL Analytics for Advertising] 구현:

* **를 사용하는 광고주 [!DNL Adobe] [!DNL Analytics for Advertising] 웹 사이트에 구현된 JavaScript 코드**: JavaScript 코드가 이미 AMO ID( )를 기록합니다`s_kwcid`) 및 `ef_id` 쿼리 문자열 매개 변수. 그러나 매크로를 사용하면 서드파티 쿠키가 지원되지 않을 때 클릭 기반 전환을 포함하도록 추적이 확장됩니다. 가장 좋은 방법은 광고 태그에 다음 섹션의 매크로를 추가하여 JavaScript 코드를 통해 캡처되지 않은 추가 클릭스루 데이터를 캡처하는 것입니다.

>[!NOTE]
>
>JavaScript 코드는 쿠키를 계속 사용할 수 있는 동안에만 클릭 추적을 위한 솔루션입니다. 쿠키가 중단되면 다음 매크로를 구현해야 합니다.

* **웹 사이트에서 를 사용하지 않는 광고주 [!DNL Analytics for Advertising] JavaScript 코드 및 대신 [!DNL Analytics] 클릭스루 데이터에만 대한 서버측 전달** (뷰스루 데이터 없음): 다음 매크로는 Adobe Advertising을 통해 구입한 광고에서 비롯된 온사이트 클릭 활동을 보고하는 데 필요합니다.

## 매크로를 추가합니다. [!DNL Google Campaign Manager 360] 광고

다음 범위 내 [!DNL Google Campaign Manager 360]를 각 디스플레이 및 비디오 광고의 랜딩 페이지 URL에 다음 매개 변수에 추가합니다. `%pamo=!;`

여러 가지 방법으로 랜딩 페이지 URL을 지정할 수 있습니다. 각 옵션에 대한 지침은 다음 하위 섹션에 포함되어 있습니다.

다음은 접미사 형식의 랜딩 페이지 URL의 예입니다.

```
https://www.adobe.com/home?someparam1=somevalue1&%pamo=!;
```

>[!NOTE]
>
>>* 랜딩 페이지 URL에 일반적이지 않은 해시 기호(#)가 포함되어 있는 경우 `amo` 해시 기호 앞에 있는 매개 변수입니다.
>* 다음 항목 뒤에 다른 매개 변수가 포함되지 않는 경우 `amo` 매개 변수를 추가한 다음 그 뒤에 매개 변수(예: &amp;a=b)를 추가합니다. 예:`https://www.adobe.com/home?someparam1=somevalue1&%pamo=!;&a=b#login`

### 광고주 수준 랜딩 페이지 URL 접미사 구성

1. 다음을 참조하십시오. [광고주 속성을 여는 지침](https://support.google.com/campaignmanager/answer/2829344).
1. 다음에서 [!UICONTROL Landing page URL suffix] 설정, 포함 `%pamo!;` 다음에서 [!UICONTROL URL suffix] 필드.

### 캠페인 수준 랜딩 페이지 URL 접미사 구성

1. 다음을 참조하십시오. [캠페인 속성 열기 지침](https://support.google.com/campaignmanager/answer/2838056#set).
1. 다음에서 [!UICONTROL Landing page URL suffix] 설정, 포함 `%pamo!;` 다음에서 [!UICONTROL URL suffix] 필드.

### 크리에이티브 수준 랜딩 페이지 URL 접미사 구성

1. 크리에이티브 속성을 엽니다.
1. 다음에서 [!UICONTROL Click tags] 설정, 포함 `%pamo!;` 다음에서 [!UICONTROL Landing page] 클릭 태그에 대한 열입니다.

## 방법 [!DNL Analytics for Advertising] DSP에서 매크로가 확장됨

DSP에서 를 포함하는 광고를 만들 때 [!DNL Analytics for Advertising] 매개 변수(`amo`), `ef_id` 및 `s_kwcid` 매크로는 클릭 URL에 자동으로 추가됩니다. 가장 좋은 방법은 DSP에서 태그를 확인하여 `ef_id` 및 `s_kwcid` 매크로가 있습니다.

다음은 의 예입니다 [!DNL Google Campaign Manager 360] [태그](https://support.google.com/campaignmanager/answer/6080468) DSP에 표시되는 것과 같습니다.

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

사용자가 광고를 클릭하면 [!DNL Google Campaign Manager 360] 보기 `%pamo` 를 URL 접미사에 추가하고 동적으로 `amo` 매개 변수를 URL에 추가합니다.

>[!MORELIKETHIS]
>
>* [개요 [!DNL Analytics for Advertising]](overview.md)
>* [사용한 Adobe Advertising ID [!DNL Analytics]](/help/integrations/analytics/ids.md)
>* [추가 [!DNL Analytics for Advertising] 매크로 위치 [!DNL Flashtalking] 광고 태그](macros-flashtalking.md)
