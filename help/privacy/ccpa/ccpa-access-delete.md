---
title: 캘리포니아 소비자 개인 정보 보호법 &#58;에 대한 Adobe Advertising 지원 소비자 데이터 액세스 및 삭제 지원
description: 지원되는 데이터 요청 유형, 필수 설정 및 필드 값, 이전 제품 ID 및 반환된 데이터 필드를 사용한 API 액세스 요청의 예에 대해 알아봅니다.
feature: CCPA
role: User, Developer
exl-id: e7808411-7dc3-499c-bda1-1f5882f651b2
TQID: https://experienceleague.adobe.com/g7Klc5k3qEPYDKIbTmsQcnklUPVvbN6qqhXaHCHvn3A
product_v2: id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2: id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 7845129ba6566c1aaaf160cc6f9ad33bf1731f75
workflow-type: tm+mt
source-wordcount: 1111
ht-degree: 0%

---

# 캘리포니아 소비자 개인 정보 보호법에 대한 Adobe Advertising 지원: 소비자 데이터 액세스 및 삭제 지원

[!DNL Adobe Advertising Search, Social, & Commerce], Adobe Advertising DSP, Adobe Advertising Creative 및 Adobe Advertising DCO의 *개*

>[!IMPORTANT]
>
>이 문서의 컨텐츠는 법률적인 조언이 아니며, 법률적인 조언을 대체하지 않습니다. 캘리포니아 소비자 개인 정보 보호법에 대한 법률 자문을 구하십시오.

CCPA(California Consumer Privacy Act)는 2020년 1월 1일에 발효되는 캘리포니아 주의 새로운 개인 정보 보호법입니다. CCPA는 캘리포니아 주민들에게 개인 정보에 대한 새로운 권리를 제공하고 캘리포니아에서 사업을 하는 특정 업체들에 데이터 보호 책임을 부과합니다. CCPA는 소비자에게 개인 정보를 액세스하고 삭제할 수 있는 권한과 제3자에게 &quot;개인 정보 판매&quot;의 자격이 되는 특정 활동을 거부할 수 있는 권한을 제공합니다.

기업은 Adobe CX Enterprise이 기업을 대신하여 처리하고 저장하는 개인 데이터를 결정합니다.

Adobe Advertising은 서비스 제공업체로서, 개인 정보에 액세스하고 삭제하기 위한 요청 관리 및 개인 정보 판매를 거부하기 위한 요청 관리를 포함하여 Adobe Advertising 제품 및 서비스 사용에 적용되는 CCPA에 따른 의무를 이행하도록 비즈니스를 지원합니다.

이 문서에서는 [!DNL Advertising Search, Social, & Commerce], Advertising Creative, Advertising DSP(Demand Side Platform) 및 [!DNL Advertising DCO]&#x200B;(서비스 공급자)이 Adobe [!DNL Experience Platform Privacy Service API] 및 [!DNL Privacy Service UI]을(를) 사용하여 개인 정보에 액세스하고 삭제할 수 있는 소비자의 권한을 지원하는 방법에 대해 설명합니다.

Advertising DSP이 개인 정보 판매를 거부하는 소비자 권한을 지원하는 방법에 대한 자세한 내용은 [캘리포니아 소비자 개인정보 보호법: 소비자 판매 거부 지원에 대한 Adobe Advertising 지원](/help/privacy/ccpa/ccpa-opt-out-of-sale.md)을 참조하십시오.

CCPA를 위한 Adobe 개인 정보 서비스에 대한 자세한 내용은 [Adobe 개인 정보 보호 센터](https://www.adobe.com/privacy/ccpa.html)를 참조하세요.

## Adobe Advertising에 대해 지원되는 데이터 요청 유형

Adobe Experience Platform은 기업이 다음 작업을 완료할 수 있는 기능을 제공합니다.

* [!DNL Search, Social, & Commerce], [!DNL Creative], [!DNL DSP] 또는 [!DNL DCO] 내에서 소비자의 쿠키 수준 데이터 또는 장치 ID 수준 데이터(모바일 앱의 광고용)에 액세스합니다.
* 브라우저를 사용하는 소비자에 대해 [!DNL Search, Social, & Commerce], [!DNL Creative], [!DNL DSP] 또는 [!DNL DCO] 내에 저장된 쿠키 수준 데이터를 삭제하거나, 모바일 장치에서 앱을 사용하는 소비자에 대해 [!DNL DSP] 내에 저장된 ID 수준 데이터를 삭제합니다.
* 하나 또는 모든 기존 요청의 상태를 확인합니다.

## Adobe Advertising에 대한 요청을 전송하기 위한 필수 설정

To make requests to access and delete consumer personal information from Adobe Advertising, you must:

1. Deploy a JavaScript library to retrieve and remove your customer&#39;s cookies. 모든 Adobe CX Enterprise 솔루션에 동일한 라이브러리 `AdobePrivacy.js`이(가) 사용됩니다.

   >[!IMPORTANT]
   >
   >일부 CX Enterprise 솔루션에 대한 요청에는 JavaScript 라이브러리가 필요하지 않지만 Adobe Advertising에 대한 요청에는 필요합니다.

   You should deploy the library on the webpage from which your customers can submit access and delete requests, such as your company&#39;s privacy portal. The library helps you retrieve Adobe cookies (namespace ID: `gsurferID`) so that you can submit these identities as part of access and delete requests via the [!DNL Adobe Experience Platform Privacy Service API].

   When the customer asks to delete personal data, the library also deletes the customer&#39;s cookie from the customer&#39;s browser.

   >[!NOTE]
   >
   >Deleting personal data is different than opting out, which stops the targeting of an end user with audience segments. However, when a consumer asks to delete personal data from [!DNL Creative], [!DNL DSP], or [!DNL DCO], the library also sends a request to Adobe Advertising to opt out the customer from segment targeting. For advertisers with [!DNL Search, Social, & Commerce], we recommend that you provide your customers a link to [https://www.adobe.com/privacy/opt-out.html#customeruse](https://www.adobe.com/privacy/opt-out.html#customeruse), which explains how to opt out of audience segment targeting.

1. Identify your CX Enterprise organization ID and make sure that it&#39;s linked to your Adobe Advertising accounts.

   CX Enterprise 조직 ID는 &quot;@AdobeOrg&quot;가 추가된 24자 영숫자 문자열입니다. 대부분의 CX Enterprise 고객에게는 조직 ID가 할당되었습니다. If your marketing team or internal [!DNL Adobe] system administrator doesn&#39;t know your organization ID, or isn&#39;t sure if it&#39;s been provisioned, then contact your Adobe Account Team. `imsOrgID` 네임스페이스를 사용하여 Privacy API에 요청을 제출하려면 조직 ID가 필요합니다.

   >[!IMPORTANT]
   >
   >[!DNL DSP] 계정 또는 광고주, [!DNL Search, Social, & Commerce] 계정, [!DNL Creative] 또는 [!DNL DCO] 계정 등 조직의 모든 Adobe Advertising 계정이 CX Enterprise 조직 ID에 연결되어 있는지 확인하려면 회사의 Adobe Advertising 담당자에게 문의하십시오.

1. Use either the [Adobe Experience Platform Privacy Service API](https://experienceleague.adobe.com/docs/experience-platform/privacy/api/privacy-jobs.html) (for automated requests) or the [Privacy Service UI](https://experienceleague.adobe.com/docs/experience-platform/privacy/ui/user-guide.html) (for ad-hoc requests) to submit requests to access and delete personal information to Adobe Advertising on behalf of consumers, and to check the status of existing requests.

   For advertisers who have a mobile app to interact with customers and launch campaigns with [!DNL DSP], you must download the Privacy-ready Mobile SDKs for CX Enterprise. The Mobile SDKs allow businesses to set opt-out status flags, retrieve the consumer&#39;s device ID (namespace ID: `deviceID`), and submit requests to the Privacy Service API. 모바일 앱에는 SDK 버전 4.15.0 이상이 필요합니다.

   When you submit a consumer access request, the Privacy Service API returns a consumer&#39;s information based on the specified cookie or device ID, which you then must return to the consumer.

   When you submit a consumer delete request, the cookie ID or device ID and all cost, click, and revenue data associated with the cookie are deleted from the server.

   >[!NOTE]
   >
   >If your business has multiple CX Enterprise organization IDs, then you must send separate API requests for each. 그러나 하위 솔루션당 하나의 계정으로 여러 Adobe Advertising 하위 솔루션([!DNL Search, Social, & Commerce], [!DNL Creative], [!DNL DSP] 및 [!DNL DCO])에 대한 하나의 API 요청을 만들 수 있습니다.

Adobe Advertising에서 지원을 받으려면 모든 단계가 필요합니다. Adobe Experience Platform Privacy Service을 사용하여 수행해야 하는 이러한 작업 및 기타 관련 작업에 대한 자세한 내용 및 필요한 항목을 찾을 수 있는 위치를 보려면 [https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html)을(를) 참조하십시오.

## Adobe Advertising JSON 요청의 필수 필드 값

`"company context":`

* `"namespace": **imsOrgID**`
* `"value":` &lt;*CX Enterprise 조직 ID*>

&quot;users&quot;:

* `"key":` &lt;*일반적으로 고객의 이름*>

* `"action":` `**access**` 또는 `**delete**`

* `"user IDs":`

   * `"namespace": **411**`([[!DNL AdCloud] 쿠키 공간](https://experienceleague.adobe.com/en/docs/experience-platform/privacy/api/appendix)을 나타냄)

   * `"value":` &lt;*`AdobePrivacy.js`*&#x200B;에서 검색된 실제 고객의 쿠키 ID 값>

* `"include": **adCloud**`(요청에 적용되는 [[!DNL Adobe] product](https://experienceleague.adobe.com/en/docs/experience-platform/privacy/api/appendix))

* `"regulation": **ccpa**`(요청에 적용되는 개인 정보 보호 규정)

## AdobePrivacy.js에서 검색한 Adobe Advertising 사용자 ID를 사용하여 소비자가 제출한 요청의 예

```
{
"companyContexts":[
    {
        "namespace":"imsOrgID",
        "value":"5AB13068374019BC@AdobeOrg"
      }
   ],
   "users": [
{
 "key": "John Doe",
 "action":["access"],
 "userIDs":[
      { 
        "namespace":"411",
        "value":"Wqersioejr-wdg",
        "type":"namespaceId",
        "deletedClientSide":false
      }
   ]
}
],
"include":[
      "adCloud"
   ],
    "regulation":"ccpa"
}
```

## 액세스 요청을 위해 반환되는 데이터 필드

다음은 Adobe Advertising에 대한 개인 정보 액세스 응답의 예입니다.

```
{
    "jobId":"12345AD43E",
    "action":"access",
    "product":"adCloud",
    "status":"complete",
    "results":{
        "userIDs":[
            {
                "namespace":"411",
                "userID":" Wqersioejr-wdg "
            }
        ],
        "receiptData":{
            "impressionCount":"100",
            "clickCount":5,
            "geo":[
                "United States of America",
                "San Francisco CA"
            ],
            "profile":[
                {
                    "pixelid":"111",
                    "ut1":"abc",
                    "ut2":"def",
                    "ut3":"ghi",
                    "ut4":"jkl",
                    "ut5":"mno"
                },
                {
                    "pixelid":"123",
                    "ut1":"abc",
                    "ut2":"def",
                    "ut3":"ghi",
                    "ut4":"jkl",
                    "ut5":"mno"
                }
            ],
            "matchingSegments":[
                {
                    "segmentName":"AP4 - Art/Culture - In-Market",
                    "segmentID":"kV1mPa2aqPNWKSNtf325",
                    "serviceProvider":"Adobe"
                },
                {
                    "segmentName":"eXelate Australia Demographic - Jobs & Education - Job Seekers",
                    "segmentID":"2213789",
                    "serviceProvider":"exelate"
                }
            ]
        }
    }
}
```
