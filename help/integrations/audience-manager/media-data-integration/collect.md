---
title: Advertising DSP 캠페인에서 클릭 및 노출 데이터 수집
description: Audience Manager 픽셀을 사용하여 Advertising DSP 광고에서 쿠키 기반 노출과 클릭 이벤트를 캡처하는 방법에 대해 알아봅니다
feature: Integration with Adobe Audience Manager
exl-id: d827fbb8-b61a-4601-a42a-1ea60e4f36b7
source-git-commit: e517dd5f5fa283ff8a2f57728612937148889732
workflow-type: tm+mt
source-wordcount: '997'
ht-degree: 0%

---

# Advertising DSP 캠페인에서 미디어 노출 데이터 수집

*Advertising DSP만 있는 광고주*

*Adobe Advertising-Adobe Audience Manager 통합만 있는 광고주*

이 문서에서는 Audience Manager 픽셀을 사용하여 쿠키 기반 노출 및 클릭 이벤트를 캡처하는 Advertising DSP 광고에 태그를 지정하는 방법과 데이터 사용에 필요한 추가 작업에 대해 설명합니다.

이벤트 픽셀은 모바일 앱 및 연결된 TV(CTV)와 같은 쿠키가 없는 환경에서 발생하는 이벤트를 캡처하지 않습니다.

## 1단계: Audience Manager에서 데이터 Source 설정 {#set-up-data-source}

Audience Manager에서 DSP 노출에 대한 [데이터 원본](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/data-sources/datasources-list-and-settings.html)을(를) 만들고 데이터를 클릭합니다. 추적된 모든 이벤트가 데이터 원본에 속하도록 각 이벤트 태그에 데이터 원본 ID [을(를) 포함합니다](#implement-dsp-pixels).

>[!NOTE]
> 단일 데이터 소스 내에서 여러 DSP에서 실행되는 광고 캠페인에 대한 모든 노출 횟수 및 클릭 데이터를 수집할 수 있습니다.

## 2단계: 웹 페이지에서 노출 및 클릭 이벤트 픽셀 구현 {#implement-dsp-pixels}

광고주는 자체 브랜드에 대한 이벤트 태그를 만들고 구현할 수 있습니다. 필요한 경우 Adobe Audience Manager 컨설턴트 또는 Adobe 계정 팀에 문의하여 지원을 받으십시오.

>[!NOTE]
>
>조직에서 [!DNL Analytics] 추적을 사용하는 경우 Audience Manager 클릭 추적이 필요하지 않을 수 있습니다. Adobe Analytics은 클릭 신호를 캡처하여 [서버측 전달](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/server-side-forwarding/ssf.html)을 통해 Audience Manager으로 보낼 수 있습니다.

### 픽셀 구문

이벤트 픽셀에는 다음 매개 변수가 포함되어야 합니다.

**노출 추적 픽셀:**

`[Audience Manager customer domain].demdex.net/event?d_event=imp&d_src=[source id]&d_campaign=${TM_CAMPAIGN_ID_NUM}`

`&` 접두사가 있는 [선택적 추가 매개 변수](#parameters) 사용

**클릭 추적 픽셀:**

`[Audience Manager customer domain].demdex.net/event?d_event=click&d_src=[source id]&d_rd=[redirect URL]&d_campaign=${TM_CAMPAIGN_ID_NUM}`

`&` 접두사가 있는 [선택적 추가 매개 변수](#parameters) 사용

위치:

* `[Audience Manager customer domain]`은(는) 노출 또는 클릭 이벤트를 [!DNL Adobe]에 보낼 도메인 이름입니다.

* `[source id]`은(는) DSP 노출을 추적하고 데이터를 클릭하는 [데이터 원본](#set-up-data-source)의 ID입니다.

* `[redirect URL]`은(는) 이중 인코딩 리디렉션 URL입니다. www.urlencoder.org과 같은 온라인 인코딩 도구를 사용하는 경우 인코더를 통해 문자열을 실행하고 결과를 다시 인코딩하십시오.

* `${TM_CAMPAIGN_ID_NUM}`은(는) DSP의 숫자 캠페인 ID입니다. DSP 매크로를 사용하는 대신 개별 캠페인 ID를 하드코딩하려면 캠페인 설정에서 ID를 찾습니다.

* 각 [매개 변수](#key-value-pairs)에는 `&`이(가) 접두사로 사용되고 `d_parameter=parameter_id` 형식입니다. 여기서 `parameter`은(는) 새 필드의 키-값 쌍으로 대체됩니다. 예: `&d_placement=${TM_PLACEMENT_ID_NUM}`

### 키-값 쌍으로서의 매개변수 {#parameters}

**형식:** `d_parameter=parameter_id`

    위치:
    
    * 매개 변수 접두사가 &#39;&amp;&#39;인 경우
    
    * &#39;매개 변수&#39;는 새 필드의 키-값 쌍으로 대체됩니다
    
    예: &#39;&amp;d_placement=${TM_PLACEMENT_ID_NUM}&#39;

두 픽셀 유형 모두 특성을 수집하거나 다른 보고서에 캠페인 메타데이터(예: 배치 이름 또는 캠페인 이름)를 제공하기 위해 *키-값 쌍*(으)로 추가 매개 변수를 포함할 수 있습니다. 키-값 쌍은 데이터 집합을 정의하는 상수인 *key*&#x200B;과(와) 집합에 속하는 변수인 *value*&#x200B;의 두 가지 관련 요소로 구성됩니다.

키-값 쌍에서 값 변수는 하드 코딩된 ID이거나, 캠페인 및 사용자 추적을 위해 광고 태그가 로드될 때 해당 값으로 동적으로 대체되는 작은 자체 포함 코드 단위인 *macro*&#x200B;일 수 있습니다. 캠페인 관련 매개 변수의 경우 Audience Manager 매크로 대신 [DSP 매크로](/help/dsp/campaign-management/macros.md)를 사용하여 해당 노출과 함께 캠페인 특성을 보내거나 모든 Audience Manager에서 단일 픽셀을 사용하여 데이터를 클릭하여 광고를 표시할 수 있습니다. 이벤트 픽셀에 삽입하는 DSP 매크로는 픽셀 내에 포함하는 키-값 쌍에 적합한 값이어야 합니다. 예를 들어 `d_placement` 키의 경우 DSP 매크로 `${TM_PLACEMENT_ID_NUM}`을(를) 값으로 사용하여 Adobe Advertising 매크로에서 생성한 배치 ID를 캡처합니다.

Audience Manager에서 노출 이벤트 픽셀에 대해 지원하는 매크로 목록을 보려면 &quot;[픽셀 호출을 통해 캠페인 노출 데이터 캡처](https://experienceleague.adobe.com/docs/audience-manager/user-guide/implementation-integration-guides/media-data-integration/impression-data-pixels.html#supported-key-value-pairs)&quot;를 참조하십시오.

클릭 이벤트 픽셀에 대해 Audience Manager이 지원하는 매크로 목록을 보려면 &quot;[픽셀 호출을 통해 캠페인 클릭 데이터 캡처](https://experienceleague.adobe.com/docs/audience-manager/user-guide/implementation-integration-guides/media-data-integration/click-data-pixels.html)&quot;를 참조하십시오.

>[!TIP]
>
>* 가장 좋은 방법은 캠페인 속성을 사용하여 Audience Manager 트레이트를 만들 수 있도록 캠페인, 배치, 광고(광고) 및 사이트 ID를 포함하는 것입니다.
>* Audience Optimization 보고서를 만들려면 추가 매개 변수가 필요합니다.
>* 키-값 쌍에서 관련 [DSP 매크로](/help/dsp/campaign-management/macros.md)(으)로 값을 바꾸면 모든 캠페인의 모든 광고에서 단일 픽셀을 사용할 수 있습니다. 예를 들어 Adobe Advertising 매크로에서 생성된 캠페인 ID를 캡처하려면 `d_campaign=[%campaignID%]`을(를) `d_campaign=${TM_CAMPAIGN_ID_NUM}`(으)로 변경하십시오.
>* 필요한 경우 하드코딩된 값으로 자신만의 매개 변수를 만들 수 있습니다. 예: `d_DSP=AdCloud`

노출 이벤트 픽셀의 예:

`http://acme.demdex.net/event?d_event=imp&d_src=1052880&d_site=${TM_SITE_ID_NUM}&d_creative=${TM_AD_ID_NUM}&d_placement=${TM_FEED_ID_NUM}&d_campaign=${TM_CAMPAIGN_ID_NUM}&d_DSP=AdCloud&d_bust=${TM_RANDOM}`

### 픽셀 추가 위치

#### 노출 추적 픽셀

[!DNL DSP] 캠페인의 모든 광고에 노출 이벤트 추적 픽셀을 첨부합니다. 다음 위치에서 그렇게 할 수 있습니다.

* 배치 수준에서 - 기본적으로 배치의 모든 광고에 픽셀을 적용합니다. 배치 설정의 [추적] 섹션에서 [[!UICONTROL Event pixels] 필드](/help/dsp/campaign-management/placements/placement-settings.md)에 픽셀을 추가합니다.

* 광고 수준에서, 배치 수준 이벤트 픽셀을 무시합니다. 광고 설정에서 [[!UICONTROL Pixel] 탭에서 이벤트 픽셀을 만듭니다](/help/dsp/campaign-management/ads/ad-edit.md).

* (서드파티 광고 서버의 광고) 광고 서버 내의 광고 수준에서.

#### 클릭 추적 픽셀

광고 서버 내에서 일반적으로 광고의 클릭스루 URL을 삽입하는 위치에 관계없이 클릭 이벤트 픽셀(인코딩된 URL이 추가됨)을 삽입합니다.

## 3단계: 구현 후 작업

이벤트 태그가 구현되면 데이터가 Audience Manager 데이터 수집 서버로 전송됩니다. 보고서에서 데이터를 사용하려면 먼저 다음 작업을 완료하십시오.

### [!DNL Amazon S3] 버킷 및 Data Source 만들기

데이터가 Audience Manager 서버에 있으면 [!DNL Amazon Simple Storage Service] ([!DNL Amazon S3]) 버킷을 만든 다음 모든 픽셀 데이터가 전송되는 데이터 소스를 만들어야 합니다. 지원이 필요한 경우 Audience Manager 컨설턴트나 [고객 지원 센터](https://experienceleague.adobe.com/docs/audience-manager/user-guide/help-and-legal/help-legal-contact.html)에 문의하십시오.

### Audience Manager 트레이트 및 세그먼트 만들기

이벤트 데이터가 [사용되지 않은 신호](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reporting/interactive-and-overlap-reports/unused-signals.html)(으)로 Audience Manager에 전송됩니다. 보고서에 데이터를 사용하기 전에 수집된 데이터에서 [규칙 기반 특성](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/traits/trait-builder/create-onboarded-rule-based-traits.html)을 수동으로 만든 다음 이러한 특성을 사용하여 [세그먼트](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/segments/segments-purpose.html)을(를) 만드십시오.

DSP의 특정 크리에이티브에 노출된 사용자에 대해 사용자 수준 데이터를 채우는 예제 트레이트:

1. 이벤트를 `d_event = imp`(으)로 식별합니다.
1. DSP 캠페인 내에서 Creative ID를 식별한 다음 트레이트에 `d_creative=[Creative ID]`(으)로 매핑합니다.

![특성 만들기 화면](/help/dsp/assets/aa-trait.png)

>[!MORELIKETHIS]
>
>* [DSP 매크로](/help/dsp/campaign-management/macros.md)
>* [Adobe Audience Manager에 DSP Media 노출 데이터 전송 개요](overview.md)
>* [사용 사례](use-cases.md)
