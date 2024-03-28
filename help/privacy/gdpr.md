---
title: 개인 정보 보호 규정에 대한 Adobe Advertising 지원
description: 지원되는 데이터 요청 유형, 필수 설정 및 필드 값, 이전 제품 ID 및 반환된 데이터 필드를 사용하는 API 액세스 요청의 예에 대해 알아봅니다
feature: GDPR
role: User, Developer
exl-id: abf0dc51-e23b-4c9a-95aa-14e0844939bb
source-git-commit: 80072930c0506a017a927ce53eaad900a2642e92
workflow-type: tm+mt
source-wordcount: '1002'
ht-degree: 0%

---

# 개인 정보 보호 규정에 대한 Adobe Advertising 지원

*대상 [!DNL Adobe Advertising Search, Social, & Commerce]; Adobe Advertising DSP, Adobe Advertising Creative 및 Adobe Advertising DCO*

>[!IMPORTANT]
>
>이 문서의 컨텐츠는 법률적인 조언이 아니며, 법률적인 조언을 대체하지 않습니다. 개인 정보 보호 규정에 대한 법률 자문을 구하십시오.

2018년 5월 25일부터 적용되는 개인 정보 보호 규정(GDPR)은 유럽 연합(EU)의 국경 내의 모든 개인(데이터 주체)이 개인 데이터를 통제하도록 하고 국제 비즈니스를 위한 규정 환경을 단순화합니다. 이 법은 데이터 관리자의 비즈니스 위치에 상관없이 개인 데이터를 처리할 때 EU의 국경 내의 개인에게 재화 또는 서비스를 제공하거나, 개인의 행동을 모니터링하거나, 개인으로부터 개인 데이터를 수집하는 모든 기업(데이터 관리자)에 적용됩니다.

Adobe Experience Cloud은 고객을 대신하여 수신하여 저장하는 모든 개인 데이터에 대한 데이터 처리자 역할을 합니다. 귀하는 데이터 관리자로서 Adobe Experience Cloud이 귀하를 대신하여 처리하고 저장하는 개인 데이터를 결정합니다.

이 문서에서는 다음 방법을 설명합니다 [!DNL Advertising Search, Social, & Commerce]; Advertising Creative; Advertising DSP(Demand Side Platform); 및 [!DNL Advertising DCO] Adobe Experience Platform Privacy Service API 및 Privacy Service UI를 사용하여 데이터 주체의 GDPR 데이터 액세스 및 삭제 권한을 지원합니다.

GDPR의 비즈니스 의미에 대한 자세한 내용은 [GDPR 및 비즈니스](https://www.adobe.com/privacy/general-data-protection-regulation.html).

## Adobe Advertising에 지원되는 데이터 요청 유형

Adobe Experience Platform은 기업이 다음 작업을 완료할 수 있는 기능을 제공합니다.

* 내에서 데이터 주체의 쿠키 수준 데이터 또는 장치 ID 수준 데이터(모바일 앱의 광고용)에 액세스합니다 [!DNL Search, Social, & Commerce], [!DNL Creative], [!DNL DSP], 또는 [!DNL DCO].
* 내에 저장된 쿠키 수준 데이터 삭제 [!DNL Search, Social, & Commerce], [!DNL Creative], [!DNL DSP], 또는 [!DNL DCO] 브라우저를 사용하는 데이터 주체의 경우 또는 내에 저장된 ID 수준 데이터를 삭제합니다. [!DNL DSP] 모바일 디바이스에서 앱을 사용하는 데이터 주체의 경우.
* 하나 또는 모든 기존 요청의 상태를 확인합니다.

## Adobe Advertising 요청을 전송하기 위한 필수 설정

Adobe Advertising을 위해 데이터에 액세스하고 삭제를 요청하려면 다음을 수행해야 합니다.

1. JavaScript 라이브러리를 배포하여 데이터 주체 쿠키를 검색하고 제거합니다. 같은 라이브러리, `AdobePrivacy.js`는 모든 Adobe Experience Cloud 솔루션에 사용됩니다.

   >[!IMPORTANT]
   >
   >일부 Experience Cloud 솔루션에 대한 요청에는 JavaScript 라이브러리가 필요하지 않지만 Adobe Advertising에 대한 요청에는 필요합니다.

   데이터 주체가 액세스 및 삭제 요청을 제출할 수 있는 웹 페이지(예: 회사의 개인 정보 보호 포털)에 라이브러리를 배포해야 합니다. 라이브러리는 다음을 검색하는 데 도움이 됩니다. [!DNL Adobe] 쿠키(네임스페이스 ID: `gsurferID`)를 클릭하여 Adobe Experience Platform Privacy Service API를 통해 액세스 및 삭제 요청의 일부로 이러한 ID를 제출할 수 있습니다.

   데이터 주체가 개인 데이터 삭제를 요청하면 라이브러리도 데이터 주체의 브라우저에서 데이터 주체의 쿠키를 삭제합니다.

   >[!NOTE]
   >
   >개인 데이터 삭제는 대상 세그먼트가 있는 최종 사용자의 타깃팅을 중지하는 옵트아웃과 다릅니다. 단, 데이터 주체에서 개인 데이터 삭제를 요청할 때는 [!DNL Creative], [!DNL DSP], 또는 [!DNL DCO], 라이브러리도 Adobe Advertising 타기팅에서 데이터 주체를 옵트아웃하도록 요청합니다. 다음을 포함하는 광고주용 [!DNL Search, Social, & Commerce], 데이터 주체에 대한 링크를 제공하는 것이 좋습니다. [https://www.adobe.com/privacy/opt-out.html](https://www.adobe.com/privacy/opt-out.html): 대상 세그먼트 타깃팅을 옵트아웃하는 방법을 설명합니다.

1. Experience Cloud 조직 ID를 식별하고 Adobe Advertising 계정에 연결되어 있는지 확인합니다.

   Experience Cloud 조직 ID는 &quot;@AdobeOrg&quot;가 추가된 24자 영숫자 문자열입니다. 대부분의 Experience Cloud 고객에게는 조직 ID가 할당되었습니다. 마케팅 팀이나 내부용 [!DNL Adobe] 시스템 관리자가 조직 ID를 모르거나 조직 ID가 프로비저닝되었는지 확실하지 않은 경우 gdprsupport@adobe.com에서 Adobe 고객 지원 센터에 문의하십시오. 다음을 사용하여 Privacy API에 요청을 제출하려면 조직 ID가 필요합니다. `imsOrgID` 네임스페이스입니다.

   >[!IMPORTANT]
   >
   >귀사의 Adobe Advertising 담당자에게 문의하여 다음을 포함한 조직의 모든 Adobe Advertising 계정을 확인하십시오. [!DNL DSP] 계정 또는 광고주, [!DNL Search, Social, & Commerce] 계정 및 [!DNL Creative] 또는 [!DNL DCO] 계정 — Experience Cloud 조직 ID에 연결됩니다.

1. 다음 중 하나를 사용합니다. [ADOBE EXPERIENCE PLATFORM PRIVACY SERVICE API](https://experienceleague.adobe.com/docs/experience-platform/privacy/api/privacy-jobs.html) (자동화된 요청의 경우) 또는 [PRIVACY SERVICE UI](https://experienceleague.adobe.com/docs/experience-platform/privacy/ui/user-guide.html?lang=ko-KR) (임시 요청의 경우) 데이터 주체를 대신하여 Adobe Advertising에 액세스 및 삭제 요청을 제출하고 기존 요청의 상태를 확인합니다.

   데이터 주체와 상호 작용하고 DSP으로 캠페인을 시작할 수 있는 모바일 앱이 있는 광고주의 경우 Experience Cloud을 위해 개인 정보 보호 지원 Mobile SDK를 다운로드해야 합니다. Mobile SDK를 사용하면 데이터 제어자가 옵트아웃 상태 플래그를 설정하고 데이터 주체의 장치 ID(네임스페이스 ID: `deviceID`)를 참조하고 Privacy Service API에 요청을 제출하십시오. 모바일 앱에는 SDK 버전 4.15.0 이상이 필요합니다.

   데이터 주체의 액세스 요청을 제출하면 Privacy Service API는 지정된 쿠키 또는 장치 ID를 기반으로 데이터 주체의 정보를 반환한 다음 데이터 주체에게 반환해야 합니다.

   데이터 주체의 삭제 요청을 제출하면 쿠키 ID 또는 장치 ID와 쿠키와 관련된 모든 비용, 클릭 및 매출 데이터가 서버에서 삭제됩니다.

   >[!NOTE]
   >
   >회사에 여러 Experience Cloud 조직 ID가 있는 경우 각각에 대해 별도의 API 요청을 보내야 합니다. 그러나 여러 Adobe Advertising 하위 솔루션에 대해 하나의 API 요청을 수행할 수 있습니다([!DNL Search, Social, & Commerce], [!DNL Creative], [!DNL DSP], 및 [!DNL DCO])을 사용하여 하위 솔루션당 하나의 계정을 만들 수 있습니다.

이 모든 단계는 Adobe Advertising에 필요합니다. 이러한 작업 및 Adobe Experience Platform Privacy Service을 사용하여 수행해야 하는 기타 관련 작업과 필요한 항목을 찾을 수 있는 위치에 대한 자세한 내용은 &quot;[Privacy Service 개요](https://experienceleague.adobe.com/docs/experience-platform/privacy/home.html).&quot;

## Adobe Advertising JSON 요청의 필수 필드 값

`"company context":`

* `"namespace": **imsOrgID**`
* `"value":` &lt;*Experience Cloud 조직 ID*>

`"users":`

* `"key":` &lt;*일반적으로 데이터 주체의 이름*>

* `"action":` 다음 중 하나 `**access**` 또는 `**delete**`

* `"user IDs":`

   * `"namespace": **411**` (다음을 나타냄) [!DNL adcloud] cookie space)

   * `"value":` &lt;*에서 검색된 실제 데이터 주체의 쿠키 ID 값`AdobePrivacy.js`*>

* `"include": **adCloud**` (는 [!DNL Adobe] 요청에 적용되는 제품)

* `"regulation": **gdpr**` (요청에 적용되는 개인정보 보호 규정)

## 데이터 주체에서 가져온 Adobe Advertising 사용자 ID를 사용하여 제출한 요청의 예 `AdobePrivacy.js`

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
    "regulation":"gdpr"
}
```

## 액세스 요청에 대해 반환되는 데이터 필드

다음은 Adobe Advertising에 대한 액세스 응답의 예입니다.

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
                    "segmentName":"EMEA - UK - Health Food Buyers",
                    "segmentID":"eP2oJ2UPsfsDVDhvlGewx",
                    "serviceProvider":"BlueKai"
                }
            ]
        }
    }
}
```
