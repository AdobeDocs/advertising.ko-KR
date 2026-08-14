---
title: Customer Journey Analytics의 Adobe Advertising 데이터 문제 해결
description: Customer Journey Analytics에서 Adobe Advertising 데이터 문제를 해결하고 해결하는 방법에 대해 알아봅니다.
feature: Integration with Adobe Customer Journey Analytics
hide: true
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2:
  - id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
  - id: d3cdead0-685a-4489-9250-4bb709942f66
source-git-commit: d6ceaa9749e6b700cc738b3de8d6088150e8ffd0
workflow-type: tm+mt
source-wordcount: 3033
ht-degree: 0%

---

# Customer Journey Analytics의 Adobe Advertising 데이터 문제 해결

다음은 잠재적인 문제, 가능한 원인 및 해결 방법입니다.

## 모든 잠재적 증상 목록

| 증상 | 추가 정보 |
| ------- | ---------------- |
| 브라우저 네트워크 탭에 alloy() 호출이 표시되지 않음 | 섹션 &quot;[설치 및 설정 문제](#issues-installation-setup)&quot; > &quot;[WebSDK 확장이 초기화되지 않음](#websdk-extension-doesn't-initialize)&quot;을 참조하십시오. |
| 콘솔 오류: 합금이 정의되지 않았습니다. | &quot;[설치 및 설치 문제](#issues-installation-setup)&quot; > &quot;[WebSDK 확장이 초기화되지 않음](#websdk-extension-doesn't-initialize)&quot;을 참조하십시오. |
| edge.adobedc.net에 대한 상호 작용 또는 수집 요청 없음 | &quot;[설치 및 설치 문제](#issues-installation-setup)&quot; > &quot;[WebSDK 확장이 초기화되지 않음](#websdk-extension-doesn't-initialize)&quot;을 참조하십시오. |
| 요청이 에지에 도달하지만 400 또는 500 오류를 반환함 | 섹션 &quot;[설치 및 설정 문제](#issues-installation-setup)&quot; > &quot;[데이터 스트림이 구성되지 않았거나 잘못 구성됨](#datastream-not-configured-or-misconfigured)&quot;을 참조하십시오. |
| Adobe Analytics 또는 Adobe Advertising 보고서에 데이터가 표시되지 않음 | 섹션 &quot;[설치 및 설정 문제](#issues-installation-setup)&quot; > &quot;[데이터 스트림이 구성되지 않았거나 잘못 구성됨](#datastream-not-configured-or-misconfigured)&quot;을 참조하십시오. |
| 네트워크 응답 오류: &quot;데이터 스트림을 찾을 수 없음&quot; | 섹션 &quot;[설치 및 설정 문제](#issues-installation-setup)&quot; > &quot;[데이터 스트림이 구성되지 않았거나 잘못 구성됨](#datastream-not-configured-or-misconfigured)&quot;을 참조하십시오. |
| 페이지 간 방문자 ID 변경 | &quot;[설치 및 설정 문제](#issues-installation-setup)&quot; > &quot;[ID 및 ECID 문제](#identity-and-ecid-issues)&quot; 섹션을 참조하십시오. |
| Advertising 대상 세그먼트가 일치하지 않음 | &quot;[설치 및 설정 문제](#issues-installation-setup)&quot; > &quot;[ID 및 ECID 문제](#identity-and-ecid-issues)&quot; 섹션을 참조하십시오. |
| 디버거에 규칙 조건이 충족되지 않은 것으로 표시됩니다. | &quot;[설치 및 설정 문제](#issues-installation-setup)&quot; > &quot;[규칙 또는 이벤트가 실행되지 않음](#rules-or-events-aren't-firing)&quot; 섹션을 참조하십시오. |
| [!UICONTROL Send Event] 작업이 실행되지 않습니다. | &quot;[설치 및 설정 문제](#issues-installation-setup)&quot; > &quot;[규칙 또는 이벤트가 실행되지 않음](#rules-or-events-aren't-firing)&quot; 섹션을 참조하십시오. |
| [!DNL Tags]에서 변경한 내용이 라이브 사이트에 반영되지 않습니다. | 섹션 &quot;[설치 및 설정 문제](#issues-installation-setup)&quot; > &quot;[라이브러리 빌드 및 게시 문제](#library-build-and-publishing-issues)&quot;를 참조하십시오. |
| 확장 업데이트가 적용되었지만 이전 동작이 지속됨 | 섹션 &quot;[설치 및 설정 문제](#issues-installation-setup)&quot; > &quot;[라이브러리 빌드 및 게시 문제](#library-build-and-publishing-issues)&quot;를 참조하십시오. |
| `alloy()` 전송 이벤트 호출이 성공했지만(200 응답 포함) Adobe Advertising 전환 데이터가 보고서에 없습니다 | &quot;[설치 및 설정 문제](#issues-installation-setup)&quot; > &quot;[Advertising 필드에 대한 스키마 유효성 검사 문제](#schema-validation-for-advertising-fields)&quot; 섹션을 참조하십시오. |
| 디버거의 XDM 페이로드에 `_experience.adcloud` 개체가 없습니다. | &quot;[설치 및 설정 문제](#issues-installation-setup)&quot; > &quot;[Advertising 필드에 대한 스키마 유효성 검사 문제](#schema-validation-for-advertising-fields)&quot; 섹션을 참조하십시오. |
| 웹 페이지에 대해 뷰스루 또는 클릭스루 전환이 기록되지 않음 | 섹션 &quot;[Advertising 확장 설정 문제](#advertising-extension-setup-issues)&quot;를 참조하십시오. |
| 클릭스루에 대한 XDM(경험 데이터 모델) 페이로드에서 `_experience.adcloud`이(가) 누락되었습니다. | 섹션 &quot;[Advertising 확장 설정 문제](#advertising-extension-setup-issues)&quot;를 참조하십시오. |
| 전환은 디버거 도구에서 확인되지만 Adobe Advertising 보고서에는 표시되지 않습니다 | 섹션 &quot;[Advertising 확장 설정 문제](#advertising-extension-setup-issues)&quot;를 참조하십시오. |

## 설치 및 설정 문제 {#issues-installation-setup}

### WebSDK 확장이 초기화되지 않음 {#websdk-extension-doesnt-initialize}

증상:

* 브라우저 네트워크 탭에 alloy() 호출이 표시되지 않음
* 콘솔 오류: 합금이 정의되지 않았습니다.
* edge.adobedc.net에 대한 상호 작용 또는 수집 요청 없음

| 원인 | 수정 |
| ----- | --- |
| 라이브러리가 게시되지 않았거나 초안 상태에 있음 | [게시 흐름](https://experienceleague.adobe.com/en/docs/experience-platform/tags/publish/publishing-flow)&#x200B;(으)로 이동하여 WebSDK 확장이 포함된 라이브러리가 승인됨/게시됨 상태인지 확인하십시오. |
| 포함 코드가 누락되었거나 잘못된 환경 | 웹 페이지의 [!DNL Tags] 포함 코드가 올바른 환경(Dev/Stage/Prod)을 참조하는지 확인하십시오. `<head>` 태그에서 `//assets.adobedtm.com/...` 스크립트 태그에 대한 환경을 찾습니다. |
| 비동기 및 동기 로드 충돌 | 웹 페이지당 하나의 [!DNL Tags] 포함 코드만 있는지 확인하십시오. 포함 코드가 중복되면 경합 조건이 발생합니다. |
| CSP(콘텐츠 보안 정책) 차단 | CSP `connect-src` 및 `script-src` 지침에 `edge.adobedc.net` `and assets.adobedtm.com`을(를) 추가합니다. |

### 데이터 스트림이 구성되지 않았거나 잘못 구성되었습니다. {#datastream-not-configured-or-misconfigured}

증상:

* 요청이 에지에 도달하지만 400 또는 500 오류를 반환함
* Adobe Analytics 또는 Adobe Advertising 보고서에 데이터가 표시되지 않음<!-- It's not useful to organize this info by cause, not symptom -->
* 네트워크 응답 오류: &quot;데이터 스트림을 찾을 수 없음&quot;

| 원인 | 수정 |
| ----- | --- |
| 태그 속성에 대한 데이터 스트림 ID가 없거나 잘못되었습니다. | <ol><li>[!DNL Tags]에서 태그 속성에 대한 [데이터 스트림 구성 설정](https://experienceleague.adobe.com/en/docs/experience-platform/tags/extensions/client/web-sdk/configure/datastreams)을 엽니다.</li><li>[!UICONTROL Datastream] 필드가 각 환경(개발, 스테이징 및 프로덕션)에 대한 올바른 데이터 스트림과 올바른 스키마 및 데이터 집합을 가리키는지 확인합니다.<br><br>세 환경에서 하나의 데이터스트림을 명시적으로 공유하지 않는 한 각 환경에는 고유한 데이터스트림이 있어야 합니다.</li></ol> |
| 태그 속성에 대해 데이터 스트림 서비스를 사용할 수 없습니다. | [데이터 스트림 설정을 열고](https://experienceleague.adobe.com/en/docs/experience-platform/datastreams/configure) 다음 서비스가 활성화되어 있는지 확인하십시오.<ul><li>Adobe Advertising(전환/대상 동기화용)</li><li>Adobe Experience Platform(프로필 수집용)</li></ul> |
| 샌드박스 불일치 | 데이터 스트림이 스키마 및 데이터 세트와 동일한 Adobe Experience Platform 샌드박스에 속하는지 확인합니다. 일반적인 실수는 프로덕션 샌드박스에서 데이터스트림을 만들지만 스키마를 개발 샌드박스로 지정하는 것입니다. |

### ID 및 ECID 문제 {#identity-and-ecid-issues}

증상:

* 페이지 간 방문자 ID 변경
* Advertising 대상 세그먼트가 일치하지 않음

| 원인 | 수정 |
| ----- | --- |
| 서드파티 쿠키가 차단됨 | 데이터 스트림의 에지 구성에서 자사 도메인을 구성하여 자사 CNAME 데이터 수집으로 마이그레이션합니다. |
| 기존 `s_ecid` 쿠키가 있는 동안 `idMigrationEnabled`이(가) `false`(으)로 설정됩니다. | WebSDK 기본 구성에서 `idMigrationEnabled: true`을(를) 설정하여 `s_ecid` 또는 `AMCV_` 쿠키에서 기존 ECID를 마이그레이션합니다. |

### 규칙 또는 이벤트가 실행되지 않습니다. #rules-or-events-aren이 실행되지 않음

증상:

* 디버거에 규칙 조건이 충족되지 않은 것으로 표시됩니다.
* [!UICONTROL Send Event] 작업이 실행되지 않습니다.

다음을 확인하십시오.

* 규칙이 저장되고 활성 라이브러리 빌드에 포함됩니다.
* 이벤트 유형은 실제 페이지 동작과 일치합니다(예: [!UICONTROL Library Loaded] 대 [!UICONTROL DOM Ready] 대 [!UICONTROL Window Loaded]).
* 그 규칙의 조건은 그다지 제한적이지 않다. 문제를 격리하기 위해 조건을 일시적으로 제거하여 테스트합니다.
* 규칙 순서가 올바릅니다. 여러 규칙이 동일한 이벤트를 공유하는 경우 규칙 순서를 확인합니다.
* 페이지의 이전 부분에서 JavaScript 오류가 발생하여 실행이 중지되지 않았습니다. 브라우저 콘솔에서 발견되지 않은 예외를 확인합니다.

### 라이브러리 빌드 및 게시 문제 {#library-build-and-publishing-issues}

증상:

* [!DNL Tags]에서 변경한 내용이 라이브 사이트에 반영되지 않습니다.
* 확장 업데이트가 적용되었지만 이전 동작이 지속됨

| 원인 | 수정 |
| ----- | --- |
| 변경 사항이 라이브러리에 추가되지 않았습니다. | [!UICONTROL Publishing Flow]에서 변경 내용이 개발 환경의 라이브러리에 추가되었는지 확인합니다. [!UICONTROL Libraries]&#x200B;(으)로 이동하여 작업 라이브러리를 열고 **변경된 모든 리소스 추가**&#x200B;를 선택한 다음 **저장 및 빌드**&#x200B;를 선택합니다. |
| 브라우저가 이전 라이브러리를 캐싱합니다. | 하드 새로 고침(Ctrl+Shift+R 또는 Cmd+Shift+R)을 수행하거나 시크릿/비공개 창에서 페이지를 엽니다. 문제가 지속되면 브라우저 캐시를 완전히 지웁니다. |
| 포함 코드는 잘못된 환경에 대한 것입니다. | 프로덕션 동작을 테스트하는 경우 페이지의 포함 코드가 프로덕션 포함 코드인지 확인합니다. |
| 라이브러리 빌드가 자동으로 실패했습니다. | [!UICONTROL Publishing Flow]&#x200B;(으)로 이동하여 라이브러리에 [!UICONTROL Build Failed] 상태가 표시되는지 확인하십시오. 라이브러리를 열고 빌드 로그를 검토하십시오. 일반적인 원인은 잘못된 규칙 구성 또는 확장 버전 충돌입니다. |

### Advertising 필드에 대한 스키마 유효성 검사 문제 {#schema-validation-for-advertising-fields}

증상:

* `alloy()` 전송 이벤트 호출이 성공했지만(200 응답 포함) Adobe Advertising 전환 데이터가 보고서에 없습니다
* 디버거의 XDM 페이로드에 `_experience.adcloud` 개체가 없습니다.

#### 1단계: [!UICONTROL Advertising] 필드 그룹이 스키마에 추가되었는지 확인

1. Adobe Experience Platform > [!UICONTROL Data Management] > [!UICONTROL Schemas]&#x200B;(으)로 이동합니다.
1. 데이터 스트림에서 사용하는 스키마를 엽니다.
1. [!UICONTROL Field Groups] 패널에서 **Adobe Advertising Cloud ExperienceEvent 전체 확장**&#x200B;이 나열되어 있는지 확인합니다.
1. 누락된 경우 **추가**&#x200B;를 선택하고 **Adobe Advertising Cloud를 검색**&#x200B;한 다음 **Adobe Advertising Cloud ExperienceEvent 전체 확장**&#x200B;을 선택한 다음 **저장**&#x200B;을 선택합니다.

>[!NOTE]
>스키마 변경에만 [!DNL Tags] 라이브러리를 다시 게시하는 것은 필요하지 않지만 새 필드가 추가된 경우 [!DNL Tags]에서 XDM 데이터 요소를 다시 매핑해야 합니다.

#### 2단계: 필요한 Adobe Advertising 필드가 `_experience.adcloud.conversionDetails`의 스키마에 있는지 확인

| 필드 경로 | 유형 | 설명 |
| ----- | --- | --- |
| `_experience.adcloud.conversionDetails.trackingCode` | 문자열 | 원래 광고 클릭에 전환을 매핑합니다. 랜딩 페이지 URL의 `s_kwcid` 쿼리 매개 변수로 채워집니다. |
| `_experience.adcloud.conversionDetails.trackingIdentity` | 문자열 | 추적된 뷰스루 또는 클릭스루 전환 이벤트에 대한 고유 ID 및 기타 세부 정보를 저장합니다. 랜딩 페이지 URL의 `ef_id` 쿼리 매개 변수로 채워집니다. |

필드가 누락된 경우 **Adobe Advertising Cloud ExperienceEvent 전체 확장** 필드 그룹이 스키마에 저장되었는지 확인한 다음 스키마 편집기를 새로 고치십시오.

#### 3단계: 랜딩 페이지 URL에 쿼리 매개 변수가 포함되어 있는지 확인

광고 클릭스루의 경우 랜딩 페이지 URL에 다음과 같은 쿼리 매개 변수를 모두 포함해야 합니다.

`https://www.example.com/landing-page?s_kwcid=AL!12345!3!abc123&ef_id=abc123xyz:G:s`

| 매개변수 누락 | 가능한 원인 |
| ----- | --- |
| `s_kwcid` | 자동 태깅은 Adobe Advertising 검색 또는 DSP 캠페인 설정에서 활성화되지 않습니다. |
| `ef_id` | 랜딩 페이지 URL이 Adobe Advertising 추적 리디렉션을 사용하지 않거나 EF ID 추가가 캠페인 설정에서 활성화되지 않습니다. |

#### 4단계: 아웃바운드 XDM 페이로드의 유효성 검사

AEP Debugger 또는 브라우저 [!UICONTROL Network] 탭을 열고 `edge.adobedc.net`을(를) 필터링한 다음 상호 작용 요청 본문을 검사합니다. 유효한 클릭스루 페이로드는 다음과 유사합니다.

```json
{
  "events": [{
    "xdm": {
      "eventType": "advertising.clicks",
      "_experience": {
        "adcloud": {
          "conversionDetails": {
            "trackingCode": "AL!12345!3!abc123",
            "trackingIdentity": "abc123xyz:G:s"
          }
        }
      }
    }
  }]
}
```

`trackingCode` 또는 `trackingIdentity`이(가) 비어 있거나 누락된 경우:

* 규칙이 실행될 때 쿼리 매개 변수가 페이지에 없습니다. URL 및 규칙의 이벤트 타이밍을 확인합니다.
* 스키마에서 필드 그룹이 누락되었습니다. 위의 스키마 단계를 다시 확인하십시오.

## [!UICONTROL Advertising] 확장 설치 문제 {#advertising-extension-setup-issues}

증상:

* 웹 페이지에 대해 뷰스루 또는 클릭스루 전환이 기록되지 않습니다.

  전환이 기록되는지 확인하려면 다음을 수행하십시오.

  1. URL에 `ef_id=test&s_kwcid=test`이(가) 추가된 웹 페이지를 엽니다.
  1. 브라우저의 코드 검사 도구([!DNL Inspect])를 열고 [!DNL Network] 탭을 열고 Adobe Experience Platform에서 event_type=&quot;advertising.enrichment_ct&quot;에 대한 상호 작용 호출을 찾습니다.
  1. 데이터 수집 인터페이스에서 수집하려는 웹 사이트 데이터에 대한 스키마 정의를 [열고](https://experienceleague.adobe.com/en/docs/platform-learn/implement-web-sdk/initial-configuration/configure-schemas) `xdm->_experience->adcloud->conversionDetails->trackingCode` 및 `trackingIdentities`에 `ef_id` 및 `s_kwcid`이(가) 포함되어 있는지 확인합니다.

* 클릭스루에 대한 XDM(경험 데이터 모델) 페이로드에서 `_experience.adcloud`이(가) 없습니다.

* 전환은 디버거 도구에서 확인되지만 Adobe Advertising 보고서에는 표시되지 않습니다

| 원인 | 수정 |
| ----- | --- |
| 데이터 스트림에 대해 `Adobe Advertising` 서비스를 사용할 수 없습니다. | <ol><li>[!DNL Tags]에서 태그 속성에 대한 [데이터 스트림 구성 설정](https://experienceleague.adobe.com/en/docs/experience-platform/tags/extensions/client/web-sdk/configure/datastreams)을 엽니다.</li><li>다음 서비스를 활성화하고 설정을 저장합니다.<ul><li>Adobe Advertising(전환/대상 동기화용)</li><li>Adobe Experience Platform(프로필 수집용)</li></ul></ol> |
| [!UICONTROL WebSDK] 확장에 대해 `Adobe Advertising` 구성 요소를 사용할 수 없습니다. | WebSDK 확장 내의 `Adobe Advertising` 구성 요소는 기본적으로 비활성화되며 XDM 스키마 또는 규칙 구성 방법과 관계없이 Adobe Advertising 클릭스루 또는 뷰스루에 대한 추적이 작동하기 전에 명시적으로 활성화되어야 합니다.<ol><li>[!DNL Tags]에서 Adobe Experience Platform Web SDK 구성 설정에서 속성에 대한 [빌드 옵션을 엽니다](https://experienceleague.adobe.com/en/docs/experience-platform/tags/extensions/client/web-sdk/configure/custom-build-components).</li><li>**Advertising** 구성 요소를 사용하도록 설정하고 설정을 저장합니다.</li><li>라이브러리를 다시 빌드하고 다시 게시합니다.</li></ol> |
| 클릭스루 전환만 기록되며 뷰스루 전환은 표시되지 않습니다 | 이는 예상되는 기본 동작입니다. `Adobe Advertising` 구성 요소가 활성화되면 `s_kwcid` 및 `ef_id` URL 쿼리 매개 변수를 사용하여 클릭스루 추적이 자동으로 활성화됩니다. 뷰스루 추적은 기본적으로 비활성화되며 추가 구성이 필요합니다. 다음 행을 참조하십시오. |
| 뷰스루 추적이 활성화되거나 구성되지 않음 | <ol><li>데이터스트림에 대한 Adobe Advertising 서비스 활성화</li><ol><li>Adobe Experience Platform의 [!UICONTROL Data Collection] > [!UICONTROL Datastreams]&#x200B;(으)로 이동하여 [!DNL Tags] 속성에서 사용하는 데이터 스트림을 엽니다.</li><li>**서비스 추가**&#x200B;를 선택하고 **Adobe Advertising** 및 **Adobe Experience Platform**&#x200B;를 선택한 다음 **저장**&#x200B;을 선택합니다.</li></ol><li>Adobe Advertising DSP에서 광고주 구성</li><ol><li>[!DNL Tags]에서 [!UICONTROL Extensions] > [!UICONTROL Installed] > **Adobe Experience Platform Web SDK** > [!UICONTROL Configure]&#x200B;(으)로 이동합니다.</li><li>[!UICONTROL Advertiser] 섹션 아래에서 드롭다운에서 광고주를 선택하고 활성화합니다. 여러 광고주를 구성하려면 **광고주 추가**&#x200B;를 선택하십시오.</li></ol><li>뷰스루 변환 픽셀이 실행되고 있는지 확인합니다.</li><ol><li>AEP Debugger에서 interact 호출에 `xdm.query` 필드 아래의 `stitchId`이(가) 포함되어 있는지 확인합니다.</li><li>브라우저 [!UICONTROL Network] 탭에서 형식이 `advertising.enrichment`인 이벤트가 실행되었고 `xdm.query`의 `stitchId`을(를) 포함하는지 확인하십시오.</li></ol></ol> 뷰스루 전환은 방문 수에 관계없이 30분마다 실행됩니다. 상호 작용 호출이 표시되지 않으면 브라우저 캐시를 지우고 다시 시도하십시오. |
| (뷰스루 상호 작용 호출이 실행된 후 Experience Platform에 뷰스루 이벤트가 없는 경우) 드롭다운에서 선택하는 대신 광고주를 수동으로 입력했습니다 | 광고주를 수동으로 입력하는 대신 [!UICONTROL Advertiser] 드롭다운에서 다시 선택합니다. |
| (뷰스루 상호 작용 호출이 실행된 후 Experience Platform에 뷰스루 이벤트가 없는 경우) 광고주 ID가 뷰스루 상호 작용 호출과 함께 전송되지 않습니다 | WebSDK 확장 구성의 [!UICONTROL Advertiser] 섹션에서 광고주가 구성되어 있고 활성화되어 있는지 확인한 다음 라이브러리를 다시 빌드하고 다시 게시합니다. |

[!UICONTROL Advertising] 확장 설치 문제에 대한 지원 티켓을 열기 전에 다음을 확인하십시오.

* **Adobe Advertising** 및 **Adobe Experience Platform** 서비스가 데이터 스트림에 추가됩니다.
* **Adobe Advertising** 구성 요소는 WebSDK 확장 구성에서 사용할 수 있습니다.
* 구성 요소를 활성화한 후 라이브러리가 다시 빌드되고 다시 게시되었습니다.
* 클릭스루 추적을 위해 랜딩 페이지 URL에는 광고 클릭에 대한 `s_kwcid` 및 `ef_id`이(가) 포함되어 있습니다.
* 뷰스루 추적을 위해 광고주가 올바른 광고주 ID로 Adobe Advertising DSP에 구성됩니다.
* WebSDK 확장 프로그램은 버전 2.36.0 이상입니다.

## 유효성 검사 및 디버깅 도구

### Adobe Experience Platform Debugger

[!DNL Chrome]에 대한 [!DNL Adobe Experience Platform Debugger] 확장을 설치합니다. 다음을 제공합니다.

* 모든 WebSDK `alloy()` 호출의 실시간 보기
* 데이터 스트림 ID 및 환경 유효성 검사
* XDM 페이로드 검사
* Edge Network 요청 및 응답 세부 정보

디버거에서 키 확인:

| 탭 | 확인할 사항 |
| ----- | --- |
| [!UICONTROL Summary] | WebSDK가 검색되고 설치된 버전을 표시하는지 확인합니다. |
| [!UICONTROL AEP Web SDK] | 실행된 각 이벤트, 전체 XDM 페이로드 및 Edge 응답을 표시합니다. |
| [!UICONTROL Adobe Advertising] | AMO ID 캡처 및 XDM 인터랙션 호출을 `advertising.enrichment` 이벤트 유형과 확인합니다. |

### 브라우저 네트워크 탭

`edge.adobedc.net`별로 필터링하여 원시 에지 요청을 검사합니다.

* 요청 URL: `https://[org-id].data.adobedc.net/ee/v2/interact`
* 메서드: `POST`
* 상태: `200`(정상), `400`(잘못된 페이로드) 또는 `500`(서버 또는 데이터스트림 오류)

다음에 대한 요청 페이로드를 확인합니다.

* 올바른 `dataStreamId`
* 예상 필드가 있는 `xdm` 개체가 있음
* ECID가 채워진 `identityMap`

### 콘솔 유효성 검사

설치된 WebSDK 버전 확인:

```js
window.alloy.version
```

테스트 이벤트를 수동으로 트리거합니다.

```js
alloy("sendEvent", {
  xdm: {
    eventType: "web.webpagedetails.pageViews",
    web: {
      webPageDetails: { name: "Test Page", URL: window.location.href }
    }
  }
}).then(result => console.log("Edge response:", result))
  .catch(err => console.error("Send event error:", err));
```

## 빠른 참조 체크리스트

지원 티켓을 열기 전에 다음 사항을 확인하십시오.

* WebSDK 확장이 최신 버전입니다.
* 라이브러리가 게시되고 포함 코드가 환경에 적합합니다.
* 데이터 스트림 ID가 개발, 스테이징 및 프로덕션에 대해 올바르게 설정됩니다.
* 모든 필수 데이터 스트림 서비스가 활성화됩니다.
* [!UICONTROL Advertising] 구성 요소가 WebSDK 확장 구성에 활성화되어 있고 DSP 광고주 ID가 구성되어 있습니다.
* XDM 스키마에 [!UICONTROL Advertising] 필드 그룹이 포함되어 있습니다.
* [!UICONTROL Send Event] 규칙에는 ID 맵이 포함되어 있으며 올바른 이벤트에서 실행됩니다.
* CSP 또는 브라우저 개인 정보 설정이 Edge 요청을 차단하지 않습니다.
* AEP Debugger가 이벤트가 에지에 도달하고 있는지 확인합니다.
* 브라우저 콘솔에서 JavaScript 오류가 발생하여 실행이 중지되지 않습니다.
* **Adobe Advertising Cloud ExperienceEvent 전체 확장** 필드 그룹이 스키마에 추가됩니다.
* `_experience.adcloud.conversionDetails.trackingCode`이(가) 스키마에 있습니다.
* `_experience.adcloud.conversionDetails.trackingIdentity`이(가) 스키마에 있습니다.
* 랜딩 페이지 URL에는 클릭스루에 `s_kwcid`과(와) `ef_id`이(가) 모두 포함되어 있습니다.
* AEP Debugger가 `conversionDetails`이(가) 아웃바운드 페이로드에 채워져 있는지 확인합니다.

## 에스컬레이션 시기

다음과 같은 경우 Adobe 계정 팀 또는 엔지니어링 팀으로 에스컬레이션합니다.

* Edge 요청이 데이터 스트림 유효성 검사 후 지속적인 `500` 오류를 반환합니다.
* [!UICONTROL Advertising] 전환은 디버거에서 확인되지만 24-48시간 후에는 보고서에 표시되지 않습니다.
* WebSDK 버전 업데이트에서는 이전 버전에 없는 회귀 문제를 해결했습니다. 지원 티켓에 특정 버전 번호를 포함하십시오.

## 보고 문제

### 요약 보고

| 증상 | 확인 및 해결 |
| ----- | --- |
| Customer Journey Analytics for Advertising DSP 또는 Advertising Search, Social, Commerce에서 사용할 수 있는 요약 보고 데이터가 없습니다. | <ol><li>Customer Journey Analytics Workspace이 올바른 데이터 보기를 참조하는지 확인합니다.</li><li>Adobe Advertising에서 Customer Journey Analytics으로의 피드가 활성화되어 있는지 확인합니다. Adobe 계정 팀에 문의하십시오.</li><li>Adobe Advertising 차원/분류/조회 데이터 세트와 요약 데이터 세트가 Customer Journey Analytics 연결에 포함되어 있는지 확인합니다.</li><li>Adobe Advertising 차원 및 요약 지표가 Customer Journey Analytics 데이터 보기에 포함되어 있는지 확인합니다.</li></ol>위의 모든 설정을 확인했지만 요약 데이터가 표시되지 않는 경우 조직에 대한 [지원 티켓](https://experienceleague.adobe.com/home?support-tab=home#support)을 여십시오. |
| 요약 보고 데이터는 Customer Journey Analytics for Advertiser 1에서 사용할 수 있지만 Advertiser 2에서는 사용할 수 없습니다. | <ol><li>Adobe Advertising에서 Customer Journey Analytics으로의 피드가 광고주 2에 대해 활성화되어 있는지 확인합니다. Adobe 계정 팀에 문의하십시오.</li><li>Customer Journey Analytics 연결에서 세 개의 데이터 세트(차원/분류/조회, 요약 및 이벤트 지표)에 대해 &quot;[!UICONTROL Backfill all existing data]&quot; 설정이 활성화되었는지 확인하십시오.</li></ol>위의 모든 조건을 확인했지만 요약 데이터가 표시되지 않는 경우 조직에 대한 [지원 티켓](https://experienceleague.adobe.com/home?support-tab=home#support)을 여십시오. |
| (Search, Social 및 Commerce 사용자) 요약 보고 데이터는 한 [!DNL Google Ads], [!DNL Meta Ads] 또는 [!DNL Microsoft Advertising] 계정에 대해 Customer Journey Analytics에서 사용할 수 있지만 다른 계정에 대해서는 사용할 수 없습니다. | Adobe Advertising에서 Customer Journey Analytics으로의 피드가 특정 광고 네트워크 계정에 대해 활성화되어 있는지 확인합니다. Adobe 계정 팀에 문의하십시오.<br><br>계정에 대해 피드가 활성화되어 있지만 요약 데이터가 표시되지 않는 경우 조직에 대해 [지원 티켓](https://experienceleague.adobe.com/home?support-tab=home#support)을 여십시오. 광고 네트워크 계정에 대한 [!UICONTROL Account ID]을(를) 포함합니다. |
| Customer Journey Analytics Workspace의 요약 보고 데이터가 Advertising DSP 또는 Advertising 검색, 소셜 및 Commerce의 데이터와 다르거나 일부 캠페인 및 캠페인 엔티티에 대한 요약 데이터가 누락되었습니다. | <ol><li>[!DNL Workspace]과(와) Adobe Advertising 보고서 모두에서 동일한 날짜 범위를 사용하고 있는지 확인하십시오.</li><li>[!DNL Workspace] 및 Adobe Advertising 보고서에 적용된 필터 및 세그먼트로 인해 데이터의 차이가 발생하지 않는지 확인하십시오.</li><li>Customer Journey Analytics 데이터 보기의 [!UICONTROL Time Zone]이(가) [Advertising DSP 계정](/help/dsp/admin/user-own-profile-edit.md)의 [!UICONTROL Default Timezone]과(와) 일치하는지 확인하십시오.</li><li>Customer Journey Analytics 연결에서 세 개의 데이터 세트(차원/분류/조회, 요약 및 이벤트 지표)에 대해 &quot;[!UICONTROL Backfill all existing data]&quot; 설정이 활성화되었는지 확인하십시오.</li></ol>데이터 불일치가 확실하면 조직에 대한 [지원 티켓](https://experienceleague.adobe.com/home?support-tab=home#support)을 여십시오. 광고 네트워크 계정에 대한 [!UICONTROL Account ID]을(를) 포함합니다. 불일치의 증거를 보이기 위해 스크린샷과 스프레드시트를 포함하십시오. Adobe 계정 팀은 필요한 경우 데이터 피드를 소급하여 수정하여 불일치를 해결할 수 있습니다. |

### 이벤트 수준 보고

| 증상 | 확인 및 해결 |
| ----- | --- |
| Customer Journey Analytics Workspace의 보고 차원(예: `Campaign`)에 전환 데이터(예: `Page Views`)를 사용할 수 없습니다. | 검증 장벽이 가장 낮은 항목부터 시작하여 다음을 확인하십시오.<ol><li>올바른 데이터 보기를 사용하고 있는지 확인합니다.</li><li>적용 가능한 전환 지표가 Adobe Advertising에서 차원에 할당할 수 있는 웹/온라인 이벤트인지 확인합니다.</li><li>Adobe Advertising이 해당 사이트에서 클릭스루 및 뷰스루를 추적하고 있는지 확인합니다.</li><li>분류 데이터 세트에 대한 Customer Journey Analytics 연결에서 [!DNL Key] 및 [!DNL Matching Key] 설정의 값이 올바른지 확인하십시오. [!DNL Key]: `Tracking Code`(_customername.adLens2.trackingCode), [!DNL Matching Key]: `Tracking Code`(event._experience.adcloud.conversionDetails.trackingCode).</li><li>[!DNL Adobe Advertising] 서비스가 Adobe Experience Platform 데이터 스트림에 추가되었는지, 데이터 스트림에 대해 매핑된 스키마가 `XDM ExperienceEvent Schema`인지, 필드 그룹 `Adobe Advertising Cloud ExperienceEvent Full Extension`이(가) `XDM ExperienceEvent` 스키마에 추가되었는지 확인하십시오.</li><li>Adobe Advertising 설정이 WebSDK 확장에 올바르게 구성되고 게시되었는지 확인합니다.</li></ol>위의 모든 설정을 확인했지만 전환 데이터가 여전히 표시되지 않으면 조직에 대한 [지원 티켓](https://experienceleague.adobe.com/home?support-tab=home#support)을 여십시오. 광고 네트워크 계정에 대한 [!UICONTROL Account ID]을(를) 포함합니다. |

<!--

+++ Question

Answer

+++

+++ Question

Answer

+++

+++ Question

Answer

+++

-->

>[!MORELIKETHIS]
>
>* [개요](overview.md)
>*  [!DNL Customer Journey Analytics][&#128279;](ids.md)에서 사용하는 Adobe Advertising ID
>* [필수 구성 요소](prerequisites.md)
>* [데이터 수집, 데이터 전송 및 보고 설정](set-up.md)
>* [Customer Journey Analytics의 Adobe Advertising 지표 및 차원](advertising-data-in-cja.md)
>* (Adobe Analytics 사용자) [Adobe Customer Journey Analytics에서 사용할 AMO ID 및 EF ID에 대한 내역 데이터 수집](/help/integrations/analytics/rvars-to-evars.md).
