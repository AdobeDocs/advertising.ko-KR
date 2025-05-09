---
title: 캘리포니아 소비자 개인 정보 보호법 &#58;소비자 판매 중지 지원에 대한 Adobe Advertising 지원
description: 소비자 판매 옵트아웃 요청 캡처를 위한 지원에 대해 알아봅니다.
feature: CCPA
role: User, Developer
exl-id: df2b8679-8a1c-4cd7-b867-cd2f53c76c8f
source-git-commit: 26a4451fb09f2a42ac60ba123ddf0cf38323312d
workflow-type: tm+mt
source-wordcount: '996'
ht-degree: 0%

---

# 캘리포니아 소비자 개인 정보 보호법에 대한 Adobe Advertising 지원: 소비자 판매 옵트아웃 지원

*Adobe Advertising Demand Side Platform(DSP)의 경우*

>[!IMPORTANT]
>
>이 문서의 컨텐츠는 법률적인 조언이 아니며, 법률적인 조언을 대체하지 않습니다. 캘리포니아 소비자 개인 정보 보호법에 대한 법률 자문을 구하십시오.

CCPA(California Consumer Privacy Act)는 2020년 1월 1일에 발효되는 캘리포니아 주의 새로운 개인 정보 보호법입니다. CCPA는 캘리포니아 주민들에게 개인 정보에 대한 새로운 권리를 제공하고 캘리포니아에서 사업을 하는 특정 업체들에 데이터 보호 책임을 부과합니다. CCPA는 소비자에게 데이터에 액세스하고 삭제할 수 있는 권한과 서드파티에 대한 개인 정보 &quot;판매&quot;의 자격이 되는 특정 활동을 거부할 수 있는 권한을 제공합니다.

기업은 Adobe Experience Cloud이 기업을 대신하여 처리하고 저장하는 개인 데이터를 결정합니다.

Adobe Advertising은 서비스 제공업체로서, 개인 정보에 액세스하고 삭제하기 위한 소비자 요청 관리 및 개인 정보 판매를 거부하기 위한 소비자 요청 관리를 포함하여 Adobe Advertising 제품 및 서비스 사용에 적용되는 CCPA에 따른 의무를 이행하도록 비즈니스를 지원합니다.

이 문서에서는 CCPA에 의해 각 용어가 정의된 대로 서비스 공급자인 Adobe Advertising Demand Side Platform(DSP)가 &quot;개인 정보&quot;의 &quot;판매&quot;를 거부할 수 있는 소비자 권리를 지원하는 방법에 대해 설명합니다. 여기에는 Adobe Advertising에 판매 옵트아웃 요청을 전달하는 방법 및 조직의 판매 옵트아웃 요청 보고서를 검색하는 방법에 대한 정보가 포함됩니다.

[!DNL Advertising Search, Social, & Commerce]; Advertising Creative 및 [!DNL Advertising DCO]이(가) 소비자의 개인 정보 액세스 및 삭제 권한을 지원하는 방법에 대한 자세한 내용은 [캘리포니아 소비자 개인정보 보호법: 소비자 데이터 액세스 및 삭제 지원에 대한 Adobe Advertising 지원](/help/privacy/ccpa/ccpa-access-delete.md)을 참조하십시오.

CCPA를 위한 Adobe 개인 정보 서비스에 대한 자세한 내용은 [Adobe 개인 정보 보호 센터](https://www.adobe.com/privacy/ccpa.html)를 참조하세요.

## Adobe Advertising에 소비자 판매 중지 요청 통신

다음 중 하나를 사용하여 소비자 판매 거부 요청을 전달할 수 있습니다.

* Advertising DSP에서 생성된 CCPA 판매 중지 세그먼트
* ADOBE EXPERIENCE PLATFORM PRIVACY SERVICE API

### 방법 1: Advertising DSP에서 [!UICONTROL CCPA Opt-Out-of-Sale] 세그먼트를 사용하여 CCPA 판매 중지 요청 전달

>[!NOTE]
>
>사용자는 CCPA 판매 중지 세그먼트에 무기한 유지됩니다.

1. [https://advertising.adobe.com/](https://advertising.adobe.com/)에서 Advertising DSP의 광고주 계정에 로그인합니다.

1. [CCPA 판매 중지 세그먼트를 만들고 세그먼트 픽셀을 구현하여 옵트아웃 요청을 캡처합니다](/help/dsp/audiences/ccpa-opt-out-segment-create.md).

### 방법 2: Adobe Experience Platform Privacy Service API를 사용하여 CCPA 판매 중지 요청 전달

*광고주가 Adobe Experience Cloud 조직 ID만 할당함*

1. JavaScript 라이브러리를 배포하여 고객의 쿠키를 검색합니다. 모든 Adobe Experience Cloud 솔루션에 동일한 라이브러리 `AdobePrivacy.js`이(가) 사용됩니다.

   >[!IMPORTANT]
   >
   >일부 Adobe Experience Cloud 솔루션에 대한 요청에는 JavaScript 라이브러리가 필요하지 않지만 Adobe Advertising에 대한 요청에는 필요합니다.

   귀사의 개인 정보 보호 포털과 같은 고객이 판매 중지 요청을 제출할 수 있는 웹 페이지에 라이브러리를 배포해야 합니다. 라이브러리는 Adobe API를 통해 판매 중지 요청의 일부로 이러한 ID를 제출할 수 있도록 Adobe Experience Platform Privacy Service 쿠키(네임스페이스 ID: `gsurferID`)를 검색하는 데 도움이 됩니다.

1. Experience Cloud 조직 ID를 식별하고 Adobe Advertising 계정에 연결되어 있는지 확인합니다.

   Experience Cloud 조직 ID는 &quot;@AdobeOrg&quot;가 추가된 24자 영숫자 문자열입니다. 대부분의 Experience Cloud 고객에게는 조직 ID가 할당되었습니다. 마케팅 팀이나 내부 Adobe 시스템 관리자가 조직 ID를 모르거나 조직 ID가 프로비저닝되었는지 확실하지 않은 경우 Adobe 계정 팀에 문의하십시오. `imsOrgID` 네임스페이스를 사용하여 Privacy API에 요청을 제출하려면 조직 ID가 필요합니다.

   >[!IMPORTANT]
   >
   >[!DNL DSP] 계정 또는 광고주, [!DNL Search, Social, & Commerce] 계정, [!DNL Creative] 또는 [!DNL DCO] 계정 등 조직의 모든 Adobe Advertising 계정이 Experience Cloud 조직 ID에 연결되어 있는지 확인하려면 회사의 Adobe Advertising 담당자에게 문의하십시오.

1. Adobe Experience Platform Privacy Service API를 사용하여 소비자를 대신하여 Adobe Advertising에 [판매 중지 요청을 제출](https://experienceleague.adobe.com/docs/experience-platform/privacy/api/consent.html?lang=ko)하고 기존 요청의 상태를 확인합니다.

   판매 중지 요청의 예는 아래 부록 을 참조하십시오.

   >[!NOTE]
   >
   >비즈니스에 여러 Experience Cloud 조직 ID가 있는 경우 각각에 대해 별도의 API 요청을 전송해야 합니다. 그러나 하위 솔루션당 하나의 계정으로 여러 Adobe Advertising 하위 솔루션([!DNL Search, Social, & Commerce], [!DNL Creative], [!DNL DSP] 및 [!DNL DCO])에 대한 하나의 API 요청을 만들 수 있습니다.

이 모든 단계는 Adobe Advertising의 지원을 받는 데 필요합니다. Adobe Experience Platform Privacy Service을 사용하여 수행해야 하는 이러한 작업 및 기타 관련 작업에 대한 자세한 내용 및 필요한 항목을 찾을 수 있는 위치를 보려면 [https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html?lang=ko](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html?lang=ko)을(를) 참조하십시오.

## 판매 중지 요청을 제출한 소비자의 보고서 검색

Adobe Advertising은 고객이 계정에 대한 판매 중지 요청을 제출한 ID에 대한 월별 보고서를 생성합니다. 각 보고서는 GZIP 형식으로 압축된 탭으로 구분된 텍스트 파일로 사용할 수 있습니다. 이 데이터는 Advertising DSP에서 생성된 CCPA 판매 중지 세그먼트를 사용하여 캡처된 요청과 Privacy Service API를 통해 제출된 모든 요청을 통합합니다. CCPA 판매 중지 세그먼트에 캡처된 사용자 ID는 세그먼트 및 광고주별로 식별됩니다. 보고서는 이전 달의 매월 1일에 생성됩니다. 예를 들어 6월의 월별 사용자 목록은 7월 1일에 제공됩니다.

Advertising DSP 내에서 또는 Advertising DSP [!DNL Trafficking API]을(를) 사용하여 이전 3개월 동안 만든 월별 보고서에 대한 링크를 검색할 수 있습니다. 각 링크는 7일 동안 유효하지만 고객이 하나를 검색하려고 할 때마다 새로 고침됩니다.

### 방법 1: Advertising DSP 내에서 소비자 판매 중지 보고서 검색

1. [https://advertising.adobe.com/](https://advertising.adobe.com/)에서 Advertising DSP의 광고주 계정에 로그인합니다.

1. [보고서 검색](/help/dsp/audiences/ccpa-opt-out-segment-report-retrieve.md).

### 방법 2: Advertising DSP [!DNL Trafficking API]을(를) 사용하여 소비자 판매 중지 보고서 검색

이 기능은 [!DNL Trafficking API]을(를) 사용하는 조직에서 사용할 수 있습니다. 자세한 내용은 [!DNL Trafficking API]에 대한 설명서를 참조하십시오.<!-- Add link to API doc once it's published. -->

조직에서 [!DNL Trafficking API]을(를) 사용하지 않지만 자세한 정보를 보려면 Adobe 계정 팀에 문의하십시오.

## 부록: Privacy Service API 사용자에 대한 [!UICONTROL CCPA Opt-Out-of-Sale] 요청 예

```
curl -X POST \
  https://platform.adobe.io/data/privacy/gdpr/ \
  -H 'Authorization: Bearer {ACCESS_TOKEN}' \
  -H 'Content-Type: application/json' \
  -H 'x-api-key: {API_KEY}' \
  -H 'x-gw-ims-org-id: {IMS_ORG}' \
  -d '{
    "companyContexts": [
      {
        "namespace": "imsOrgID",
        "value": "{IMS_ORG}"
      }
    ],
    "users": [
      {
        "key": "DavidSmith",
        "action": ["opt-out-of-sale"],
        "userIDs": [
          {
            "namespace": "email",
            "value": "dsmith@acme.com",
            "type": "standard"
          },
          {
            "namespace": "AdCloud",
            "type": "standard",
            "value":  "Wqersioejr-wdg",
          }
    ],
    "include": ["adCloud"],
    "regulation": "ccpa"
}'
```

여기서, [Privacy Service API 사양](https://experienceleague.adobe.com/ko/docs/experience-platform/privacy/api/appendix)에 따라

* `"namespace": "AdCloud"`은(는) `AdCloud` 쿠키 공간을 나타내며, 해당 값은 `AdobePrivacy.js`에서 검색된 고객의 쿠키 ID입니다.
* `"include": ["adCloud"]`은(는) 요청이 제품 Adobe Advertising에 적용됨을 나타냅니다
