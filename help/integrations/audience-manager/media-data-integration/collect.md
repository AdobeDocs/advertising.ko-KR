---
title: Advertising DSP 캠페인에서 클릭 및 노출 데이터 수집
description: Audience Manager 픽셀을 사용하여 Advertising DSP 광고에서 쿠키 기반 노출 및 클릭 이벤트를 캡처하는 방법에 대해 알아봅니다
feature: Integration with Adobe Audience Manager
exl-id: d827fbb8-b61a-4601-a42a-1ea60e4f36b7
source-git-commit: 4b9cc5956d573b346eacdf71a8ea490c162b4660
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 0%

---

# Advertising DSP 캠페인에서 미디어 노출 데이터 수집

*Advertising DSP만 있는 광고주*

*Adobe Advertising-Adobe Audience Manager 통합만 있는 광고주*

이 문서에서는 Audience Manager 픽셀을 사용하여 쿠키 기반 노출 및 클릭 이벤트를 캡처하는 Advertising DSP 광고에 태그를 추가하는 방법과 데이터를 사용하는 데 필요한 추가 작업에 대해 설명합니다.

이벤트 픽셀은 모바일 앱 및 연결된 TV(CTV)와 같은 쿠키가 없는 환경에서 발생하는 이벤트를 캡처하지 않습니다.

## 1단계: Audience Manager에서 데이터 소스 설정 {#set-up-data-source}

Audience Manager에서 [데이터 소스](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/data-sources/datasources-list-and-settings.html) DSP 를 클릭하고 데이터를 클릭합니다. 데이터 소스 ID 포함 [각 이벤트 태그에서](#implement-dsp-pixels) 추적된 모든 이벤트가 데이터 소스에 귀속되도록 하는 것입니다.

>[!NOTE]
> 단일 데이터 소스 내에서 여러 DSP에서 실행되는 광고 캠페인에 대한 모든 노출 횟수 및 클릭 데이터를 수집할 수 있습니다.

## 2단계: 웹 페이지에서 노출 및 클릭 이벤트 픽셀 구현 {#implement-dsp-pixels}

광고주는 자체 브랜드에 대한 이벤트 태그를 만들고 구현할 수 있습니다. 필요한 경우 Adobe Audience Manager 컨설턴트 또는 Adobe 계정 팀에 문의하여 지원을 받으십시오.

>[!NOTE]
>
>조직에서 를 사용하는 경우 [!DNL Analytics] 추적하면 Audience Manager 클릭 추적이 필요하지 않을 수 있습니다. Adobe Analytics은 클릭 신호를 캡처하여 다음을 통해 Audience Manager으로 보낼 수 있습니다. [서버측 전달](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/server-side-forwarding/ssf.html).

### 픽셀 구문

이벤트 픽셀에는 다음 매개 변수가 포함되어야 합니다.

**노출 추적 픽셀:**

`[Audience Manager customer domain].demdex.net/event?d_event=imp&d_src=[source id]&d_campaign=${TM_CAMPAIGN_ID_NUM}`

포함 [선택적 추가 매개 변수](#parameters) 접두사 `&`

**클릭 추적 픽셀:**

`[Audience Manager customer domain].demdex.net/event?d_event=click&d_src=[source id]&d_rd=[redirect URL]&d_campaign=${TM_CAMPAIGN_ID_NUM}`

포함 [선택적 추가 매개 변수](#parameters) 접두사 `&`

위치:

* `[Audience Manager customer domain]` 는 노출 또는 클릭 이벤트를 보낼 도메인 이름입니다. [!DNL Adobe].

* `[source id]` 는 의 ID입니다. [데이터 소스](#set-up-data-source) 를 사용하여 DSP 노출을 추적하고 데이터를 클릭합니다.

* `[redirect URL]` 는 이중으로 인코딩된 리디렉션 URL입니다. www.urlencoder.org과 같은 온라인 인코딩 도구를 사용하는 경우 인코더를 통해 문자열을 실행하고 결과를 다시 인코딩하십시오.

* `${TM_CAMPAIGN_ID_NUM}` 는 DSP의 숫자 캠페인 ID입니다. DSP 매크로를 사용하는 대신 개별 캠페인 ID를 하드코딩하려면 캠페인 설정에서 ID를 찾습니다.

* 각 [매개 변수](#key-value-pairs) 접두사가 붙음 `&` 다음 형식을 갖습니다. `d_parameter=parameter_id`, 여기서 `parameter` 는 새 필드의 키-값 쌍으로 대체됩니다. 예: `&d_placement=${TM_PLACEMENT_ID_NUM}`

### 키-값 쌍으로서의 매개변수 {#parameters}

**형식:**  `d_parameter=parameter_id`

    여기서:
    
    * 매개 변수 접두사가 &#39;&amp;&#39;입니다.
    
    * &#39;parameter&#39;가 새 필드의 키-값 쌍으로 대체됩니다.
    
    예: `&amp;d_placement=${TM_PLACEMENT_ID_NUM}`

두 픽셀 유형 모두 다음과 같이 추가 매개변수를 포함할 수 있습니다. *키-값 쌍* 트레이트를 수집하거나 다른 보고서에 대한 캠페인 메타데이터(예: 배치 이름 또는 캠페인 이름)를 제공할 수 있습니다. 키-값 쌍은 두 개의 관련 요소인 a *key*: 데이터 세트를 정의하는 상수입니다. *값*: 집합에 속하는 변수입니다.

키-값 쌍에서 값 변수는 하드 코딩된 ID이거나 *매크로*: 캠페인 및 사용자 추적을 위해 광고 태그가 로드될 때 해당 값으로 동적으로 대체되는 자체 포함된 코드의 작은 단위입니다. 캠페인 관련 매개 변수의 경우 [DSP 매크로](/help/dsp/campaign-management/macros.md) Audience Manager 매크로를 사용하여 캠페인 속성을 해당 노출과 함께 보내거나 모든 Audience Manager에서 단일 픽셀을 사용하여 광고로 데이터를 클릭하는 방법. 이벤트 픽셀에 삽입하는 DSP 매크로는 픽셀 내에 포함하는 키-값 쌍에 적합한 값이어야 합니다. 예: `d_placement` 키, DSP 매크로를 사용해야 합니다. `${TM_PLACEMENT_ID_NUM}` Adobe Advertising 매크로에서 생성한 배치 ID를 캡처할 값으로 사용됩니다.

노출 이벤트 픽셀에 대해 Audience Manager이 지원하는 매크로 목록은 &quot;[픽셀 호출을 통해 캠페인 노출 횟수 데이터 캡처](https://experienceleague.adobe.com/docs/audience-manager/user-guide/implementation-integration-guides/media-data-integration/impression-data-pixels.html#supported-key-value-pairs).&quot;

클릭 이벤트 픽셀에 대해 Audience Manager이 지원하는 매크로 목록은 &quot;[픽셀 호출을 통해 캠페인 클릭 데이터 캡처](https://experienceleague.adobe.com/docs/audience-manager/user-guide/implementation-integration-guides/media-data-integration/click-data-pixels.html).&quot;

>[!TIP]
>
>* 가장 좋은 방법은 캠페인 속성을 사용하여 Audience Manager 트레이트를 만들 수 있도록 캠페인, 배치, 광고(광고) 및 사이트 ID를 포함하는 것입니다.
>* Audience Optimization 보고서를 만들려면 추가 매개 변수가 필요합니다.
>* 키-값 쌍에서 값을 관련 값으로 바꿉니다 [DSP 매크로](/help/dsp/campaign-management/macros.md) 따라서 모든 캠페인의 모든 광고에서 단일 픽셀을 사용할 수 있습니다. 예: 변경 `d_campaign=[%campaignID%]`끝 `d_campaign=${TM_CAMPAIGN_ID_NUM}` Adobe Advertising 매크로에서 생성된 캠페인 ID를 캡처합니다.
>* 필요한 경우 하드코딩된 값으로 자신만의 매개 변수를 만들 수 있습니다. 예: `d_DSP=AdCloud`

노출 이벤트 픽셀의 예:

`http://acme.demdex.net/event?d_event=imp&d_src=1052880&d_site=${TM_SITE_ID_NUM}&d_creative=${TM_AD_ID_NUM}&d_placement=${TM_FEED_ID_NUM}&d_campaign=${TM_CAMPAIGN_ID_NUM}&d_DSP=AdCloud&d_bust=${TM_RANDOM}`

### 픽셀 추가 위치

#### 노출 추적 픽셀

의 모든 광고에 노출 이벤트 추적 픽셀 첨부 [!DNL DSP] 캠페인. 다음 위치에서 그렇게 할 수 있습니다.

* 배치 수준에서 - 기본적으로 배치의 모든 광고에 픽셀을 적용합니다. 배치 설정의 [추적] 섹션에서 [[!UICONTROL Event pixels] 필드](/help/dsp/campaign-management/placements/placement-settings.md).

* 광고 수준에서, 배치 수준 이벤트 픽셀을 무시합니다. 광고 설정에서 [에서 이벤트 픽셀 만들기 [!UICONTROL Pixel] 탭](/help/dsp/campaign-management/ads/ad-edit.md).

* (서드파티 광고 서버의 광고) 광고 서버 내의 광고 수준에서.

#### 클릭 추적 픽셀

광고 서버 내에서 일반적으로 광고의 클릭스루 URL을 삽입하는 위치에 관계없이 클릭 이벤트 픽셀(인코딩된 URL이 추가됨)을 삽입합니다.

## 3단계: 구현 후 작업

이벤트 태그가 구현되면 데이터가 Audience Manager 데이터 수집 서버로 이동합니다. 보고서에서 데이터를 사용하려면 먼저 다음 작업을 완료하십시오.

### 만들기 [!DNL Amazon S3] 버킷 및 데이터 소스

데이터가 Audience Manager 서버에 업로드되면 [!DNL Amazon Simple Storage Service] ([!DNL Amazon S3]) 버킷을 선택한 후 모든 픽셀 데이터가 전송되는 데이터 소스를 선택합니다. Audience Manager 컨설턴트에게 문의하거나 [고객 지원 센터](https://experienceleague.adobe.com/docs/audience-manager/user-guide/help-and-legal/help-legal-contact.html) 지원이 필요한 경우

### Audience Manager 트레이트 및 세그먼트 만들기

이벤트 데이터는 다음과 같이 Audience Manager으로 이동합니다. [사용되지 않은 신호](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reporting/interactive-and-overlap-reports/unused-signals.html). 수동으로 만들기 [규칙 기반 트레이트](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/traits/trait-builder/create-onboarded-rule-based-traits.html) 수집된 데이터에서 가져온 다음 [세그먼트](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/segments/segments-purpose.html) 보고서에서 데이터를 사용하기 전에 이러한 트레이트를 사용하십시오.

DSP의 특정 크리에이티브에 노출된 사용자에 대해 사용자 수준 데이터를 채우는 예제 트레이트:

1. 이벤트를 다음으로 식별 `d_event = imp`.
1. DSP 캠페인 내에서 크리에이티브 ID를 식별한 다음 트레이트에 다음과 같이 매핑합니다 `d_creative=[Creative ID]`.

![트레이트 만들기 화면](/help/dsp/assets/aa-trait.png)

>[!MORELIKETHIS]
>
>* [DSP 매크로](/help/dsp/campaign-management/macros.md)
>* [Adobe Audience Manager에 DSP Media 노출 데이터 전송 개요](overview.md)
>* [사용 사례](use-cases.md)
