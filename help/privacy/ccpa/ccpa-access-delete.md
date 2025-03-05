---
title: 캘리포니아 소비자 개인 정보 보호법 &#58;소비자 데이터 액세스 및 삭제 지원에 대한 Adobe Advertising 지원
description: 지원되는 데이터 요청 유형, 필수 설정 및 필드 값, 이전 제품 ID 및 반환된 데이터 필드를 사용한 API 액세스 요청의 예에 대해 알아봅니다.
feature: CCPA
role: User, Developer
exl-id: e7808411-7dc3-499c-bda1-1f5882f651b2
source-git-commit: 8d88a46e82a17ce5d2debf93ea0652f35a734d7a
workflow-type: tm+mt
source-wordcount: '1037'
ht-degree: 0%

---

# 캘리포니아 소비자 개인 정보 보호법을 위한 Adobe Advertising 지원: 소비자 데이터 액세스 및 삭제 지원

[!DNL Adobe Advertising Search, Social, & Commerce], Adobe Advertising DSP, Adobe Advertising Creative 및 Adobe Advertising DCO의 *개*

>[!IMPORTANT]
>
>이 문서의 컨텐츠는 법률적인 조언이 아니며, 법률적인 조언을 대체하지 않습니다. 캘리포니아 소비자 개인 정보 보호법에 대한 법률 자문을 구하십시오.

CCPA(California Consumer Privacy Act)는 2020년 1월 1일에 발효되는 캘리포니아 주의 새로운 개인 정보 보호법입니다. CCPA는 캘리포니아 주민들에게 개인 정보에 대한 새로운 권리를 제공하고 캘리포니아에서 사업을 하는 특정 업체들에 데이터 보호 책임을 부과합니다. CCPA는 소비자에게 개인 정보를 액세스하고 삭제할 수 있는 권한과 제3자에게 &quot;개인 정보 판매&quot;의 자격이 되는 특정 활동을 거부할 수 있는 권한을 제공합니다.

기업은 Adobe Experience Cloud이 기업을 대신하여 처리하고 저장하는 개인 데이터를 결정합니다.

Adobe Advertising은 서비스 제공업체로서, 개인 정보에 액세스하고 삭제하기 위한 요청 관리 및 개인 정보 판매를 거부하기 위한 요청 관리를 포함하여 Adobe Advertising 제품 및 서비스 사용에 적용되는 CCPA에 따른 의무를 이행하도록 비즈니스를 지원합니다.

이 문서에서는 [!DNL Advertising Search, Social, & Commerce], Advertising Creative, Advertising DSP(Demand Side Platform) 및 [!DNL Advertising DCO]&#x200B;(서비스 공급자)이 Adobe [!DNL Experience Platform Privacy Service API] 및 [!DNL Privacy Service UI]을(를) 사용하여 개인 정보에 액세스하고 삭제할 수 있는 소비자의 권한을 지원하는 방법에 대해 설명합니다.

Advertising DSPAdobe Advertising 가 개인 정보 판매를 거부하는 소비자 권한을 지원하는 방법에 대한 자세한 내용은 [캘리포니아 소비자 개인정보 보호법: 소비자 옵트아웃 지원](/help/privacy/ccpa/ccpa-opt-out-of-sale.md)을 참조하십시오.

CCPA를 위한 Adobe 개인 정보 서비스에 대한 자세한 내용은 [Adobe 개인 정보 보호 센터](https://www.adobe.com/privacy/ccpa.html)를 참조하세요.

## Adobe Advertising에 대해 지원되는 데이터 요청 유형

Adobe Experience Platform은 기업이 다음 작업을 완료할 수 있는 기능을 제공합니다.

* [!DNL Search, Social, & Commerce], [!DNL Creative], [!DNL DSP] 또는 [!DNL DCO] 내에서 소비자의 쿠키 수준 데이터 또는 장치 ID 수준 데이터(모바일 앱의 광고용)에 액세스합니다.
* 브라우저를 사용하는 소비자에 대해 [!DNL Search, Social, & Commerce], [!DNL Creative], [!DNL DSP] 또는 [!DNL DCO] 내에 저장된 쿠키 수준 데이터를 삭제하거나, 모바일 장치에서 앱을 사용하는 소비자에 대해 [!DNL DSP] 내에 저장된 ID 수준 데이터를 삭제합니다.
* 하나 또는 모든 기존 요청의 상태를 확인합니다.

## Adobe Advertising에 대한 요청을 전송하기 위한 필수 설정

Adobe Advertising에서 소비자 개인 정보에 액세스하고 삭제를 요청하려면 다음을 수행해야 합니다.

1. JavaScript 라이브러리를 배포하여 고객의 쿠키를 검색하고 제거합니다. 모든 Adobe Experience Cloud 솔루션에 동일한 라이브러리 `AdobePrivacy.js`이(가) 사용됩니다.

   >[!IMPORTANT]
   >
   >일부 Experience Cloud 솔루션에 대한 요청에는 JavaScript 라이브러리가 필요하지 않지만 Adobe Advertising에 대한 요청에는 필요합니다.

   고객이 회사의 개인 정보 보호 포털과 같은 액세스 및 삭제 요청을 제출할 수 있는 웹 페이지에 라이브러리를 배포해야 합니다. 라이브러리를 사용하면 Adobe 쿠키(네임스페이스 ID: `gsurferID`)를 검색하여 [!DNL Adobe Experience Platform Privacy Service API]을(를) 통해 액세스 및 삭제 요청의 일부로 이러한 ID를 제출할 수 있습니다.

   고객이 개인 데이터 삭제를 요청하면 라이브러리가 고객 브라우저에서도 고객 쿠키를 삭제합니다.

   >[!NOTE]
   >
   >개인 데이터 삭제는 옵트아웃과 다르며, 이렇게 하면 대상 세그먼트가 있는 최종 사용자의 타겟팅이 중지됩니다. 그러나 소비자가 [!DNL Creative], [!DNL DSP] 또는 [!DNL DCO]에서 개인 데이터를 삭제하도록 요청하면 라이브러리가 Adobe Advertising에 세그먼트 타깃팅에서 고객을 옵트아웃하도록 요청하기도 합니다. [!DNL Search, Social, & Commerce]을(를) 사용하는 광고주의 경우 대상 세그먼트 타깃팅을 옵트아웃하는 방법을 설명하는 [https://www.adobe.com/privacy/opt-out.html#customeruse](https://www.adobe.com/privacy/opt-out.html#customeruse) 링크를 고객에게 제공하는 것이 좋습니다.

1. Experience Cloud 조직 ID를 식별하고 Adobe Advertising 계정에 연결되어 있는지 확인합니다.

   Experience Cloud 조직 ID는 &quot;@AdobeOrg&quot;가 추가된 24자 영숫자 문자열입니다. 대부분의 Experience Cloud 고객에게는 조직 ID가 할당되었습니다. 마케팅 팀이나 내부 [!DNL Adobe] 시스템 관리자가 조직 ID를 모르거나 조직 ID가 프로비저닝되었는지 확실하지 않은 경우 Adobe 계정 팀에 문의하십시오. `imsOrgID` 네임스페이스를 사용하여 Privacy API에 요청을 제출하려면 조직 ID가 필요합니다.

   >[!IMPORTANT]
   >
   >[!DNL DSP] 계정 또는 광고주, [!DNL Search, Social, & Commerce] 계정, [!DNL Creative] 또는 [!DNL DCO] 계정 등 조직의 모든 Adobe Advertising 계정이 Experience Cloud 조직 ID에 연결되어 있는지 확인하려면 회사의 Adobe Advertising 담당자에게 문의하십시오.

1. [Adobe Experience Platform Privacy Service API](https://experienceleague.adobe.com/docs/experience-platform/privacy/api/privacy-jobs.html)&#x200B;(자동화된 요청의 경우) 또는 [Privacy Service UI](https://experienceleague.adobe.com/docs/experience-platform/privacy/ui/user-guide.html?lang=ko)&#x200B;(임시 요청의 경우)를 사용하여 소비자를 대신하여 Adobe Advertising에 개인 정보에 액세스하고 삭제하는 요청을 제출하고 기존 요청의 상태를 확인합니다.

   [!DNL DSP]을(를) 사용하여 고객과 상호 작용하고 캠페인을 시작하는 모바일 앱이 있는 광고주의 경우 Experience Cloud용 Privacy-ready Mobile SDK를 다운로드해야 합니다. Mobile SDK를 사용하면 비즈니스에서 옵트아웃 상태 플래그를 설정하고 소비자의 장치 ID(네임스페이스 ID: `deviceID`)를 검색한 다음 Privacy Service API에 요청을 제출할 수 있습니다. 모바일 앱에는 SDK 버전 4.15.0 이상이 필요합니다.

   소비자 액세스 요청을 제출하면 Privacy Service API는 지정된 쿠키 또는 장치 ID를 기반으로 소비자 정보를 반환한 다음 소비자에게 반환해야 합니다.

   소비자 삭제 요청을 제출하면 쿠키 ID 또는 장치 ID와 쿠키와 관련된 모든 비용, 클릭 및 매출 데이터가 서버에서 삭제됩니다.

   >[!NOTE]
   >
   >비즈니스에 여러 Experience Cloud 조직 ID가 있는 경우 각각에 대해 별도의 API 요청을 전송해야 합니다. 그러나 하위 솔루션당 하나의 계정으로 여러 Adobe Advertising 하위 솔루션([!DNL Search, Social, & Commerce], [!DNL Creative], [!DNL DSP] 및 [!DNL DCO])에 대한 하나의 API 요청을 만들 수 있습니다.

Adobe Advertising에서 지원을 받으려면 모든 단계가 필요합니다. Adobe Experience Platform Privacy Service을 사용하여 수행해야 하는 이러한 작업 및 기타 관련 작업에 대한 자세한 내용 및 필요한 항목을 찾을 수 있는 위치를 보려면 [https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html)을(를) 참조하십시오.

## Adobe Advertising JSON 요청의 필수 필드 값

`"company context":`

* `"namespace": **imsOrgID**`
* `"value":` &lt;*Experience Cloud 조직 ID*>

&quot;users&quot;:

* `"key":` &lt;*일반적으로 고객의 이름*>

* `"action":` `**access**` 또는 `**delete**`

* `"user IDs":`

   * `"namespace": **411**`([!DNL adCloud] 쿠키 공간을 나타냄)

   * `"value":` &lt;*`AdobePrivacy.js`*&#x200B;에서 검색된 실제 고객의 쿠키 ID 값>

* `"include": **adCloud**`(요청에 적용되는 [!DNL Adobe] 제품)

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

## 액세스 요청에 대해 반환되는 데이터 필드

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
