---
title: Adobe 광고 ID를 사용하여 만들기 [!DNL Marketing Channels] 규칙
description: Adobe 광고 ID를 사용하여 다음에 대한 처리 규칙을 만드는 방법을 알아봅니다. [!DNL Analytics Marketing Channels].
feature: Integration with Adobe Analytics
exl-id: 525761b4-607f-4b03-9020-8051009a13c6
source-git-commit: 7e614ecb517515217d812926f61ca10437820efd
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 0%

---

# Adobe 광고 ID를 사용하여 만들기 [!DNL Marketing Channels] 처리 규칙

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

Adobe 광고 ID( 를 사용할 수 있습니다.[AMO ID 및 EF ID](../ids.md))을 클릭하여 구성합니다 [!DNL Marketing Channels] Adobe Analytics의 처리 규칙. Adobe 광고 캠페인과 관련된 규칙에 Adobe 광고 ID를 사용합니다.

## 처리 규칙의 AMO ID

AMO ID는 내에서 Adobe 광고 데이터를 보고하는 데 사용되는 기본 추적 코드입니다 [!DNL Analytics]. AMO ID는 내에서 세분화된 보고를 제공하기 위해 Adobe에서 관리하는 동적 값의 연결입니다 [!DNL Analytics]. It&#39;s stored저장 in an [!DNL Analytics] [eVar](https://experienceleague.adobe.com/docs/analytics/components/dimensions/evar.html) 또는 rVar 차원(AMO ID)입니다. AMO ID는에서 설정할 수 있습니다. [!DNL Analytics] 두 가지 방법으로:

* 클릭스루 추적: Adobe 광고는 `s_kwcid` 링크의 쿼리 문자열 매개 변수 및 [!DNL Analytics] 클릭스루가 발생할 때 랜딩 페이지 URL에서 매개 변수를 선택합니다.
* 뷰스루 추적([!DNL DSP] 만 해당): 마지막 이벤트 서비스는 서버측에서 뷰스루를 감지하고 AMO ID를 [!DNL Analytics]. 이 경우 URL에는 `s_kwcid` 매개 변수.

AMO ID 내의 동적 값은 추적된 마케팅 채널을 나타냅니다.

* AMO ID의 접두사를 사용하여 내에서 최상위 채널을 식별할 수 있습니다 [!DNL Marketing Channels].

* AMO ID 본문의 문자 구는 보다 구체적인 캠페인 유형을 나타냅니다.

* 접미사 &quot;vt&quot;는 다음에 대해 존재합니다. [!DNL DSP] 뷰스루 트래픽 및 를 사용하여 별도의 클릭스루와 뷰스루를 만들 수 있습니다 [!DNL DSP] 채널.

AMO ID의 나머지 부분은 무시할 수 있습니다.

| AMO ID | 채널 | 규칙 논리 |
|--------|---------|--------------------|
| 알! (접두사) | [!UICONTROL Paid Search] | 다음으로 시작 |
| ac! (접두사) | [!UICONTROL DSP] | 다음으로 시작 |
| ! (본문) | [!UICONTROL Google Search] | 다음 포함 |
| !s! (본문) | [!UICONTROL Search Partner] | 다음 포함 |
| !d! (본문) | [!UICONTROL Display Network] | 다음 포함 |
| ! (본문) | [!UICONTROL Smart Shopping Campaign] | 다음 포함 |
| ! (본문) | [!UICONTROL YouTube Video Ad] | 다음 포함 |
| ! (본문) | [!UICONTROL YouTube Search Ad] | 다음 포함 |
| !vp! (본문) | [!UICONTROL Google Video Partners] | 다음 포함 |
| !vt(접미어) | [!UICONTROL DSP View-through] | 종료 문자 |

### AMO ID를 사용하는 처리 규칙의 예

다음 [!DNL Marketing Channels] 에 대한 처리 규칙 [!UICONTROL Paid Search] 채널은 다음과 같을 수 있습니다.

![의 예 [!UICONTROL Paid Search] 규칙](/help/integrations/assets/a4adc-mc-rule-paidsearch.png)

다음 [!DNL Marketing Channels] 에 대한 처리 규칙 [!UICONTROL YouTube Video Ads] 채널은 다음과 같을 수 있습니다.

![의 예 [!UICONTROL YouTube Video Ads] 규칙](/help/integrations/assets/a4adc-mc-rule-youtube-video.png)

>[!IMPORTANT]
>
> 특정한 순서대로 규칙을 실행합니다. 위의 두 규칙이 순서대로 실행되면 [!DNL YouTube] 비디오 광고 트래픽은 모두 [!UICONTROL Paid Search] amo ID가 모두 &quot;AL!&quot;로 시작하므로 채널 포함 내용: &quot;!ytv!&quot;

## 처리 규칙의 EF ID

Amo EF ID(EF ID)는 [!DNL Analytics for Advertising] 통합. 주요 목적은 추적 및 전달하는 것입니다 [!DNL Analytics] 이벤트 데이터를 Adobe 광고로. 클릭스루 또는 뷰스루가 발생할 때마다, 동일한 방문자에 대해 정확히 동일한 광고라고 하더라도 고유한 EF ID가 생성됩니다. EF ID는에서 사용되지 않습니다 [!DNL Analytics] 일반적으로 의 변수 제한당 50만 개의 고유 값을 초과하므로 사용자 인터페이스를 보고하는 중 [!DNL Analytics]을 추가하여 보고할 수 없습니다. Adobe 광고 지표 및 메타데이터는 EF ID에 적용되지 않습니다. AMO ID에만 적용됩니다. Adobe 광고에서 캠페인 최적화를 위해 추가된 추적 세부 기간이 필요하므로 두 ID가 모두 필요합니다.

EF ID 차원은에서 직접 사용되지 않지만 [!DNL Analytics] 보고 시 EF ID는 마케팅 채널을 만드는 데 유용합니다. EF ID 접미사는 채널(디스플레이 또는 검색)과 방문이 클릭스루로 시작되었는지 뷰스루로 시작되었는지를 나타냅니다. EF ID의 구분 기호는 AMO ID의 느낌표가 아닌 콜론입니다.

| EF ID 접미사 | 채널 |
|-------|---------|
| :s | [!UICONTROL Paid Search] |
| :d | [!UICONTROL Display Click-through] |
| :i | [!UICONTROL Display View-through] |

### EF ID를 사용하는 처리 규칙의 예

#### 클릭스루 규칙 표시

클릭스루만 캡처하여 디스플레이 클릭스루 마케팅 채널을 만듭니다. AMO ID는 클릭스루와 뷰스루 모두에서 동일하기 때문에 이 규칙은 EF ID 변수와 `ef_id` 쿼리 문자열 매개 변수.

경우에 따라 클릭스루가 URL(기본값)을 통해 추적됩니다. 다른 경우에는 클릭스루가 서버측의 마지막 이벤트 서비스를 통해 추적되므로 URL에 `ef_id` 매개 변수. 따라서 규칙은 EF ID 변수 또는 `ef_id` 쿼리 문자열 매개 변수는 &quot;:d&quot;로 끝납니다. 사용`Any`&quot; 연산자 - 두 조건 중 하나에 대해 이 규칙을 트리거하려는 경우

![표시 클릭스루 규칙의 예](/help/integrations/assets/a4adc-mc-rule-display-ct.png)

#### 뷰스루 규칙 표시

디스플레이 뷰스루 채널을 만들려면 EF ID가 &quot;:i&quot;로 끝나는 규칙을 만듭니다. 방문자가 광고를 클릭하지 않았기 때문에 뷰스루 추적에 가 포함되지 않습니다. `ef_id` 또는 `s_kwcid` 규칙에 조건이 하나만 필요합니다.

![디스플레이 뷰스루 규칙의 예](/help/integrations/assets/a4adc-mc-rule-display-vt.png)

>[!MORELIKETHIS]
>
>* [의 기본 사항 [!DNL Analytics Marketing Channels]](mc-overview.md)
>* [Adobe 광고와 간에 채널 데이터가 다를 수 있는 이유 [!DNL Marketing Channels]](mc-data-variances.md)
>* [사용 [!DNL Analytics Marketing Channels] Adobe 광고 데이터 포함](mc-ac-data.md)
>* [비디오: 사용 [!DNL Marketing Channels] Adobe 광고 보고용](https://experienceleague.adobe.com/docs/advertising-learn/tutorials/analytics/analytics-reporting-a4adc.html)
>* [Adobe 광고 ID 사용됨 [!DNL Analytics]](/help/integrations/analytics/ids.md)

