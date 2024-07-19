---
title: Advertising DSP 매크로
description: 일반 추적에 사용 가능한 매크로를 참조하고 서드파티 디스플레이 광고의 클릭을 추적합니다.
feature: DSP Ads
exl-id: 7058c988-c544-4a61-84dd-eec4ce88ceba
source-git-commit: e517dd5f5fa283ff8a2f57728612937148889732
workflow-type: tm+mt
source-wordcount: '941'
ht-degree: 0%

---

# Advertising DSP 매크로

매크로는 명령에 대한 짧은 명령 또는 축약이며 일반적으로 `${MACRO_NAME}` 형식을 따릅니다. Creative 코드 또는 클릭스루 URL에 포함된 매크로는 광고 서버에서 이해할 수 있는 더 긴 코드 문자열로 확장됩니다. DSP 광고 서버는 광고가 제공되거나 클릭될 때 매크로를 실행합니다.

광고 서버 매크로는 중요한 정보를 DSP 또는 타사 광고 서버에 전달하는 데 유용합니다. 매크로는 서드파티 및 사용자 지정 크리에이티브 코드 또는 메타데이터(예: 서드파티 픽셀)의 트래픽 중에 가장 일반적으로 사용됩니다.

VAST 태그, URL, DSP 또는 타사 이벤트 픽셀과 같은 모든 위치에 매크로를 수동으로 삽입할 수 있습니다. 그러나 각 DSP 클라이언트와 파트너는 서로 다른 광고 태그 형식을 가지며 그에 따라 태그의 서로 다른 지점에 매크로를 삽입해야 합니다. 새 클라이언트나 파트너와 작업할 때마다 DSP에서 트래픽이 발생하는 광고 태그에서 매크로를 삽입할 위치에 대한 설명서를 요청하십시오.

## 일반 추적 매크로

필요에 따라 모든 광고 및 태그 유형에 일반 추적 매크로를 사용하여 특정 데이터를 다시 전달합니다.

| 매크로 | 대체 설명 | 유형 |
| ----- | ----------------------- | ---- |
| `${TM_ACCOUNT_ID}` | 계정 ID. | 정수 |
| `${TM_AD_ID}` | 광고 키(adKey)입니다. | 문자열 |
| `${TM_AD_ID_NUM}` | 광고 ID. | 정수 |
| `${TM_ADVERTISER_ID}` | 광고주 ID입니다. | 정수 |
| `${TM_CAMPAIGN_ID}` | 캠페인 키. | 문자열 |
| `${TM_CAMPAIGN_ID_NUM}` | 캠페인 ID. | 정수 |
| ` ${TM_CLICK_URL}` | 광고 서버에서 광고 클릭을 추적하고 계산할 수 있는 리디렉션 URL입니다. 광고가 게재될 때 사용자가 해당 광고를 클릭하면 매크로가 활성화되고 클릭이 보고용으로 기록 및 카운트됩니다. | 문자열 |
| ` ${TM_CLICK_URL_URLENC}` | 광고 서버에서 광고 클릭을 추적하고 계산할 수 있도록 인코딩된 리디렉션 URL입니다. 광고가 게재될 때 사용자가 해당 광고를 클릭하면 매크로가 활성화되고 클릭이 보고용으로 기록 및 카운트됩니다. 서드파티 광고를 만들고 공급업체에 URL 인코딩이 필요한 경우가 아니면 이 매크로를 사용하지 마십시오. | 문자열 |
| `${TM_FEED_ID}` | 미디어 배치 키(feedKey)입니다. | 문자열 |
| `${TM_FEED_ID_NUM}` | 미디어 배치 ID입니다. | 정수 |
| ` ${TM_MACRO_PLACEMENT_SITE_KEY` | 배치에 대한 사이트 키입니다. 모바일 앱 설치 광고에 대한 [!DNL AppsFlyer] 클릭 추적기에 필요합니다.<!-- should map to placement_site_key column of placement_site table --> | 문자열 |
| `${TM_PLACEMENT_ID}` | 배치 키(cpKey). | 문자열 |
| `${TM_PLACEMENT_ID_NUM}` | 배치 ID. | 정수 |
| `${TM_RANDOM}` | Cachebuster: 1과 1000000 사이의 임의의 숫자. | 길게 |
| `${TM_SESSION_ID}` | 광고 태그의 단일 검색에 해당하는 세션의 ID입니다. | 문자열 |
| `${TM_SITE_DOMAIN_URLENC}` | 입찰 요청의 URL에서 구문 분석된 페이지 하위 도메인입니다. URL로 인코딩됩니다. 배너 내, 클릭-재생 광고에 대해서는 지원되지 않습니다. | 문자열 |
| ` ${TM_SITE_NAME}` | 배치의 사이트 이름입니다. | 문자열 |
| `${TM_SITE_URL_URLENC}` | 입찰 요청에서 전달된 URL. URL로 인코딩됨. 배너 내, 클릭-재생 광고에 대해서는 지원되지 않습니다. | 문자열 |
| `${TM_SITE_ID_NUM}` | 배치용 사이트 ID입니다. | 정수 |
| `${TM_TIMESTAMP}` | 1970년 1월 1일 자정(00:00 UTC) 이후 경과된 시간(초)을 나타내는 Unix 타임스탬프입니다. | 길게 |
| ` ${TM_VIDEO_DURATION}` | 광고 비디오의 지속 시간(초)입니다. | 정수 |

{style="table-layout:auto"}

<!-- Removed because not found in code base:
|` ${TM_MACRO_PROMOTED_AD_KEY}` | The promoted ad key for the placement. Required for [!DNL AppsFlyer] click trackers for mobile app install ads. | string |
 -->

## 모바일 특정 매크로

| 매크로 | 대체 설명 | 유형 |
| ----- | ----------------------- | ---- |
| `${CS_PLATFORM_ID}` | ([!DNL ComScore]) 장치의 운영 체제에 해당하는 플랫폼 ID:<ul><li>`ios` = [!DNL Apple iOS]</li><li>`android` = [!DNL Google Android]</li><li>`windows` = [!DNL Windows Mobile]</li><li>`blackberry` = [!DNL Blackberry]</li> <li>플랫폼이 위에 없는 경우 `other`</li></ul> | varchar(50) |
| `${CS_DEVICE_MODEL}` | ([!DNL ComScore]) URL로 인코딩된 장치 모델 이름입니다. | 문자열 |
| `${CS_IMPLEMENTATION_TYPE}` | ([!DNL ComScore]) 광고가 제공된 환경:<ul><li>`a` = 모바일 애플리케이션</li><li>`b` = 모바일 웹 사이트</li></ul> | 문자열(`a` 또는 `b`) |
| `${NS_PLATFORM_ID}` | ([!DNL Nielsen]) 장치의 운영 체제에 해당하는 플랫폼 ID:<ul><li>`ios`= [!DNL Apple iOS]</li><li>`android` = [!DNL Google Android]</li><li>`windows` = [!DNL Windows Mobile]</li><li>`blackberry` = [!DNL Blackberry]</li> <li>플랫폼이 위에 없는 경우 `other`</li></ul> | 문자열 |
| `${NS_DEVICE_GROUPING}` | ([!DNL Nielsen]) 광고가 뷰어였던 장치 유형:<ul><li>`TAB` = 태블릿</li><li>`PHN` = 모바일</li><li>`computer` = 컴퓨터</li></ul> | 문자열 |
| `${UOO}` | ([!DNL Nielsen]) 사용자가 광고 추적을 옵트아웃했는지 여부:<ul><li>`1`(DNT 플래그 = 1) = 사용자가 광고 추적을 옵트아웃했습니다</li><li>`0`(DNT 플래그 = 0) = 사용자가 광고 추적을 옵트인했습니다.</li></ul> | 정수(`0` 또는 `1`) |
| `${TM_BUNDLE}` | [!DNL iOS] 또는 [!DNL Android] 앱스토어 번들 ID. 예: com.zynga.wwf2.free 또는 id804379658 | 문자열 |
| `gdpr=${GDPR_ENFORCED}&gdpr_consent=${GDPR_CONSENT}` | `gdpr=${GDPR_ENFORCED}`은(는) 입찰자가 입찰 요청이 유럽 연합 기원에서 왔고 GDPR 시행이 필요하다고 판단하는지 여부를 나타냅니다.<ul><li>`1` = GDPR이 적용되어야 합니다.</li><li>`0` = GDPR을 적용할 수 없습니다.</li></ul>`gdpr_consent=${GDPR_CONSENT}`은(는) 인바운드 입찰 요청에서 공급 파트너로부터 전달된 동의 값입니다.<ul><li>대부분의 경우 base64url로 인코딩된 동의 문자열 또는 daisybit입니다(예: BN5lERiOMYEdiAKAWXEND1HoSBE6CAFApAMgBkIDIgM0AgOJxAnQA).</li><li>`0` = 동의 없음</li><li>`1` = 동의</li></ul> | daisybit 또는 integer |

{style="table-layout:auto"}

## 서드파티 디스플레이 광고에 대한 매크로 클릭

서드파티 디스플레이 태그를 사용하여 광고의 클릭 수를 정확하게 추적하려면 DSP에 디스플레이 클릭 매크로가 필요합니다. 매크로는 한 버전만 필요합니다. 관련 매크로는 태그의 유형에 따라 다릅니다.

| 매크로 | 대체 설명 | 유형 |
| ----- | ----------------------- | ---- |
| `${TM_CLICK_URL}` | 광고 서버가 플랫폼에서 광고 클릭을 추적하고 계산할 수 있는 리디렉션 URL입니다. | 문자열 |
| `${TM_CLICK_URL_URLENC}` | URL 인코딩이 필요한 광고 서버가 플랫폼에서 광고 클릭을 추적하고 계산할 수 있도록 하는 리디렉션 URL입니다. | 문자열 |

{style="table-layout:auto"}

DSP은 다음과 같은 경우 서드파티 디스플레이 태그에 디스플레이 클릭 매크로를 자동으로 삽입합니다.

* 광고 서버 파트너 <!-- [Needs PM confirmation.] -->에서 광고 태그 내보내기
* [!DNL Flashtalking] 또는 [!DNL Google DoubleClick for Advertisers] 광고 태그를 DSP에서 직접 일괄 업로드

디스플레이 광고를 작성할 때 클릭 매크로가 없으면 DSP에 경고 메시지가 표시되어 태그의 올바른 영역에 적절한 디스플레이 클릭 매크로를 수동으로 삽입하라는 메시지가 표시됩니다.

## [!DNL Analytics for Advertising]개 매크로

[[!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md) 고객에게만 제공되는 추가 매크로에 대해서는 &quot;[추가 [!DNL Analytics for Advertising] 광고 태그에 매크로 [!DNL Flashtalking] 추가](/help/integrations/analytics/macros-flashtalking.md)&quot; 및 &quot;[광고 태그에 매크로 [!DNL Analytics for Advertising] 추가 [!DNL Google Campaign Manager 360] 광고 태그에 매크로](/help/integrations/analytics/macros-google-campaign-manager.md)&quot;을 참조하십시오.

## 매크로 오류 문제 해결

코드에 매크로를 추가할 때는 매크로의 정확한 구문을 사용해야 합니다. 매크로의 유효성을 검사할 때 DSP에서는 매크로가 유효한 매크로 중 하나와 정확히 일치하는지 확인합니다.

매크로 이름의 시작 또는 끝에서 문자가 누락된 경우 오류가 발생합니다. 예를 들어 다음과 같은 경우 오류 메시지가 표시됩니다.

* 매크로 이름의 시작 부분에 있는 하나 이상의 문자를 잊어버립니다(예: `${`). 전체 구문을 포함하지 않으면 항목이 올바른 매크로로 인식되지 않습니다.
* 매크로가 `}`과(와) 같은 올바른 문자 집합으로 끝나지 않습니다.

>[!MORELIKETHIS]
>
>* [오디오 광고 설정](/help/dsp/campaign-management/ads/ad-settings-audio.md)
>* [연결된 TV 광고 설정](/help/dsp/campaign-management/ads/ad-settings-connected-tv.md)
>* [광고 설정 표시](/help/dsp/campaign-management/ads/ad-settings-display.md)
>* [모바일 광고 설정](/help/dsp/campaign-management/ads/ad-settings-mobile.md)
>* [기본 광고 설정](/help/dsp/campaign-management/ads/ad-settings-native.md)
>* [광고 프리롤 설정](/help/dsp/campaign-management/ads/ad-settings-pre-roll.md)
>* [범용 비디오 광고 설정](/help/dsp/campaign-management/ads/ad-settings-universal-video.md)
