---
title: 사용자 지정 세그먼트 만들기 및 구현
description: 광고에 노출된 사용자 또는 웹 페이지를 방문하는 사용자를 추적하기 위해 사용자 지정 세그먼트를 만들고 구현하는 방법에 대해 알아봅니다.
feature: DSP Segments
exl-id: 3190fd78-18d2-4da3-920b-d4171e693c03
source-git-commit: dda4ff8e7538bc742caa50862575cb4e46a1371d
workflow-type: tm+mt
source-wordcount: '694'
ht-degree: 0%

---

# 사용자 지정 세그먼트 만들기 및 구현

사용자 지정 DSP 세그먼트를 만들고 구현하여 자신의 자사 대상 데이터를 수집할 수 있습니다. 세그먼트를 사용하여 a) 데스크탑 및 모바일 디바이스에서 광고에 노출된 사용자 및 b) 특정 웹 페이지를 방문하는 사용자를 추적할 수 있습니다. 나중에 추가 광고를 사용하여 세그먼트의 사용자를 다시 타겟팅하거나 세그먼트의 사용자가 추가 광고를 받지 못하도록 할 수 있습니다.

>[!NOTE]
>
>웹 사이트의 소비자 판매 중지 요청에서 사용자 ID를 추적하려면 CCPA(California Consumer Privacy Act)에 따라 [CCPA 판매 중지 세그먼트](ccpa-opt-out-segment-create.md)를 만듭니다.

## 세그먼트가 ID5 ID를 추적하기 위한 사전 요구 사항

*Beta 기능*

* ID5 ID와 연결된 사용자를 추적할 세그먼트를 생성하기 전에 [!DNL ID5](으)로 계약에 서명하고 조직의 파트너 ID를 얻으십시오. 자세한 내용은 Adobe 계정 팀에 문의하십시오.

* Adobe Analytics에서 측정하는 경우 다음을 수행해야 합니다.

   1. 구현하기 위한 모든 [필수 구성 요소 [!DNL Analytics for Advertising]](/help/integrations/analytics/prerequisites.md)를 완료하고 [AMO ID 및 EF ID](/help/integrations/analytics/ids.md)이(가) 추적 URL에 채워져 있는지 확인하십시오.

   1. 마지막 이벤트 서비스가 초기화되기 전이나  [!DNL Analytics for Advertising]](/help/integrations/analytics/javascript.md)에 필요한 [JavaScript 코드 내에서 다음 매개 변수를 웹 페이지에 추가하십시오.

      ```window.id5PartnerId=ID5_PartnerID;```

      예:

      ```
      <script src="https://www.everestjs.net/static/le/last-event-tag-latest.min.js">
      <script>
        window.id5PartnerId=ID5_PartnerID;
             if("undefined" != typeof AdCloudEvent)
                 AdCloudEvent('IMS ORG Id','rsid');
      </script>
      ```

      전체 태그 형식은 &quot;[JavaScript 전환 추적 태그 버전 3](/help/search-social-commerce/tracking/format-conversion-tag-jsv3.md)&quot; 및 &quot;[JavaScript 전환 추적 태그 버전 2](/help/search-social-commerce/tracking/format-conversion-tag-jsv2.md)&quot; 형식을 참조하십시오.

   1. 브라우저 디버깅 도구를 사용하여 각 호출이 도메인 `lasteventf-tm.everesttech.net`에 대해 시작되고 암호화된 ID5 ID를 값으로 하는 `_les_id5` 매개 변수를 포함하는지 확인하십시오.

## 사용자 지정 세그먼트 만들기 및 구현

1. 세그먼트를 만듭니다.

   1. 메인 메뉴에서 **[!UICONTROL Audiences]** > **[!UICONTROL Segments]**&#x200B;을(를) 클릭합니다.

   1. 데이터 테이블 위에서 **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다.

   1. 고유한 **[!UICONTROL Segment Name]**&#x200B;을(를) 입력하십시오.

   1. **[!UICONTROL Segment Type]**&#x200B;에 대해 *[!UICONTROL Custom]*&#x200B;을(를) 선택합니다.

   1. 사용자 쿠키가 세그먼트에 있는 일 수인 **[!UICONTROL Lookback Window]**&#x200B;을(를) 입력합니다.

      기본 기간은 45일입니다. 1에서 365 사이의 값을 입력하십시오.

   1. **[!UICONTROL Advanced]**&#x200B;을(를) 클릭하여 고급 설정을 확장한 다음 세그먼트 태그가 추적하는 사용자 식별자 유형을 선택합니다.

      * *[!UICONTROL Cookies]:*(기본값) 세그먼트 태그가 쿠키를 추적합니다.

      * [!UICONTROL Universal IDs (Beta)]:

         * *[!UICONTROL ID5]:* 세그먼트 태그는 [!DNL ID5]개의 ID를 추적합니다. 범용 ID에 게재되는 노출에 대해서는 요금이 부과되지 않습니다.

        **[!UICONTROL Terms of Service]:** 범용 ID 사용에 대한 서비스 약관 계약입니다. 귀하 또는 DSP 계정의 다른 사용자는 새 ID 유형에 범용 ID를 사용하기 전에 약관에 한 번 동의해야 합니다. 관리 서비스 계약을 보유한 고객의 경우 Adobe 계정 팀이 귀하의 동의를 받고 조직을 대신하여 약관에 동의합니다. 용어를 읽으려면 **>**&#x200B;을(를) 클릭합니다. 약관에 동의하려면 약관의 맨 아래로 스크롤하여 **[!UICONTROL Accept]**&#x200B;을(를) 클릭합니다.

   1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

1. 필요에 따라 태그를 복사하여 구현하여 세그먼트를 추적합니다.

   1. **[!UICONTROL Audiences]** > **[!UICONTROL Segments]**(으)로 돌아갑니다.

   1. 세그먼트 행 위에 커서를 놓고 **[!UICONTROL Get Pixel]**&#x200B;을(를) 클릭합니다.

      * 웹 페이지에서 데스크탑 및 모바일 방문자를 추적하려면 다음을 수행하십시오.

         1. 레이블이 &quot;[!UICONTROL Desktop or mobile websites]&quot;인 페이지 보기 추적 태그를 복사합니다.

         1. ([!DNL ID5] ID를 추적하는 세그먼트의 태그) 복사된 태그에서 `ID5_PARTNER_ID`을(를) [!DNL ID5]이(가) 조직에 할당한 파트너 ID로 바꾸십시오.

            예를 들어 ID5 파트너 ID가 `abcde`이고 생성된 세그먼트 태그가 인 경우

            ```<script src="https://playtime.tubemogul.com/ud/prod/universal_ids/segment.js?sid=012345&id5pid=ID5_PARTNER_ID"></script><img src="https://rtd-tm.everesttech.net/upi/?sid=012345&cs=1" />```

            `ID5_PARTNER_ID`을(를) 태그 내의 `abcde`(으)로 바꾸면 다음을 가져올 수 있습니다.

            ```<script src="https://playtime.tubemogul.com/ud/prod/universal_ids/segment.js?sid=012345&id5pid=abcde"></script><img src="https://rtd-tm.everesttech.net/upi/?sid=012345&cs=1" />```

            조직이 [!DNL ID5]과(와) 계약에 서명할 때 파트너 ID를 받았습니다. 파트너 ID를 모르는 경우 Adobe 계정 팀에 문의하십시오.

            태그는 데스크톱 또는 모바일 장치에서 광고 장치에 노출된 사용자의 [!DNL ID5] ID를 추적할 필요가 없습니다.

         1. 배포를 위해 광고주 또는 웹 사이트 담당자에게 태그를 제공합니다.

            광고주의 IT 부서 또는 다른 그룹은 태그 배포를 예약하거나 그에 대한 정보를 받아야 할 수 있습니다.

      * 데스크탑 또는 모바일 장치에서 광고 장치에 노출된 사용자를 추적하려면 다음 작업을 수행하십시오.

         1. &quot;[!UICONTROL Desktop or mobile ads]&quot;(으)로 레이블이 지정된 노출 추적 태그를 복사합니다.

         1. 관련 있는 각 광고의 [!UICONTROL Pixel] 탭이나 관련 있는 각 배치에 대한 [[!UICONTROL Tracking] 설정의 [!UICONTROL Event Pixels] 섹션에 태그를 추가하십시오](/help/dsp/campaign-management/placements/placement-settings.md#placement-tracking).

추적 태그가 구현되면 모든 배치에 대해 대상 타겟 또는 제외에서 세그먼트를 사용할 수 있습니다.

>[!TIP]
>
>사용자가 추적될 때 세그먼트 크기를 추적합니다.

>[!MORELIKETHIS]
>
>* [대상자 관리 정보](audience-about.md)
>* [세그먼트 정보 편집](segment-edit.md)
>* [세그먼트 삭제](segment-delete.md)
>* [세그먼트에 대한 추적 픽셀 보기](segment-view-pixels.md)
>* [세그먼트 공유 또는 공유 중지](segment-share.md)
>* [[!UICONTROL CCPA Opt-Out-of-Sale] 세그먼트 만들기 및 구현](ccpa-opt-out-segment-create.md)
>* [재사용 가능한 대상 만들기](reusable-audience-create.md)
>* [사용 가능한 타사 데이터 공급자](third-party-data-providers.md)
>* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)
