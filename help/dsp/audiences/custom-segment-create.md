---
title: 사용자 지정 세그먼트 만들기 및 구현
description: 광고에 노출된 사용자 또는 웹 페이지를 방문하는 사용자를 추적하기 위해 사용자 지정 세그먼트를 만들고 구현하는 방법에 대해 알아봅니다.
feature: DSP Segments
exl-id: 3190fd78-18d2-4da3-920b-d4171e693c03
source-git-commit: e517dd5f5fa283ff8a2f57728612937148889732
workflow-type: tm+mt
source-wordcount: '648'
ht-degree: 0%

---

# 사용자 지정 세그먼트 만들기 및 구현

사용자 지정 DSP 세그먼트를 만들고 구현하여 자신의 자사 대상 데이터를 수집할 수 있습니다. 세그먼트를 사용하여 a) 데스크탑 및 모바일 디바이스에서 광고에 노출된 사용자 및 b) 특정 웹 페이지를 방문하는 사용자를 추적할 수 있습니다. 나중에 추가 광고를 사용하여 세그먼트의 사용자를 다시 타겟팅하거나 세그먼트의 사용자가 추가 광고를 받지 못하도록 할 수 있습니다.

>[!NOTE]
>
>캘리포니아 소비자 개인 정보 보호법(CCPA)에 따라 웹 사이트에서 소비자 판매 중지 요청으로부터 사용자 ID를 추적하려면 다음을 만듭니다. [CCPA 판매 중지 세그먼트](ccpa-opt-out-segment-create.md).

## 세그먼트가 ID5 ID를 추적하기 위한 사전 요구 사항

*Beta 기능*

* ID5 ID와 연결된 사용자를 추적하기 위해 세그먼트를 생성하기 전에 와(과) 계약에 서명해야 합니다 [!DNL ID5] 조직의 파트너 ID를 가져옵니다. 자세한 내용은 Adobe 계정 팀에 문의하십시오.

* Adobe Analytics에서 측정하는 경우 다음을 수행해야 합니다.

   1. 모두 완료 [구현을 위한 사전 요구 사항 [!DNL Analytics for Advertising]](/help/integrations/analytics/prerequisites.md) 및 [추적 URL의 AMO ID 및 EF ID](/help/integrations/analytics/ids.md).

   1. 웹 페이지의 앞 또는 안에 다음 매개 변수를 추가합니다. [에 필요한 JavaScript 코드 [!DNL Analytics for Advertising]](/help/integrations/analytics/javascript.md) — 마지막 이벤트 서비스가 초기화되기 전 임의 위치입니다.

      ```window.id5PartnerId=Your_ID5_PartnerID;```

      예:

      ```
      <script src="https://www.everestjs.net/static/le/last-event-tag-latest.min.js">
      <script>
        window.id5PartnerId=Your_ID5_PartnerID;
             if("undefined" != typeof AdCloudEvent)
                 AdCloudEvent('IMS ORG Id','rsid');
      </script>
      ```

## 사용자 지정 세그먼트 만들기 및 구현

1. 세그먼트를 만듭니다.

   1. 메인 메뉴에서 **[!UICONTROL Audiences]** > **[!UICONTROL Segments]**.

   1. 데이터 테이블 위에서 **[!UICONTROL Create]**.

   1. 고유 항목 입력 **[!UICONTROL Segment Name]**.

   1. 의 경우 **[!UICONTROL Segment Type]**, 선택 *[!UICONTROL Custom]*.

   1. 다음을 입력합니다. **[!UICONTROL Lookback Window]**: 사용자 쿠키가 세그먼트에 있는 일 수입니다.

      기본 기간은 45일입니다. 1에서 365 사이의 값을 입력하십시오.

   1. 클릭 **[!UICONTROL Advanced]** 고급 설정을 확장한 다음 세그먼트 태그가 추적하는 사용자 식별자 유형을 선택합니다.

      * *[!UICONTROL Cookies]:* (기본값) 세그먼트 태그는 쿠키를 추적합니다.

      * [!UICONTROL Universal IDs (Beta)]:

         * *[!UICONTROL ID5]:* 세그먼트 태그가 추적합니다 [!DNL ID5] ID 범용 ID에 게재되는 노출에 대해서는 요금이 부과되지 않습니다.

        **[!UICONTROL Terms of Service]:** 범용 ID 사용에 대한 서비스 약관. 귀하 또는 DSP 계정의 다른 사용자는 새 ID 유형에 범용 ID를 사용하기 전에 약관에 한 번 동의해야 합니다. 관리 서비스 계약을 보유한 고객의 경우 Adobe 계정 팀이 귀하의 동의를 받고 조직을 대신하여 약관에 동의합니다. 용어를 읽으려면 다음을 클릭합니다. **>**. 용어를 수락하려면 약관의 맨 아래로 스크롤하여 을 클릭합니다 **[!UICONTROL Accept]**.

   1. 클릭 **[!UICONTROL Save]**.

1. 필요에 따라 태그를 복사하여 구현하여 세그먼트를 추적합니다.

   1. 다음으로 돌아가기: **[!UICONTROL Audiences]** > **[!UICONTROL Segments]**.

   1. 커서를 세그먼트 행 위에 놓고 를 클릭합니다 **[!UICONTROL Get Pixel]**.

      * 웹 페이지에서 데스크탑 및 모바일 방문자를 추적하려면 다음을 수행하십시오.

         1. 레이블이 &quot;&quot;로 지정된 페이지 보기 추적 태그를 복사합니다.[!UICONTROL Desktop or mobile websites].&quot;

         1. 배포를 위해 광고주 또는 웹 사이트 담당자에게 태그를 제공합니다.

            광고주의 IT 부서 또는 다른 그룹은 태그 배포를 예약하거나 그에 대한 정보를 받아야 할 수 있습니다.

      * 데스크탑 또는 모바일 장치에서 광고 장치에 노출된 사용자를 추적하려면 다음 작업을 수행하십시오.

         1. 라는 레이블이 지정된 노출 추적 태그를 복사합니다.[!UICONTROL Desktop or mobile ads].&quot;

   1. (추적하는 세그먼트의 태그 [!DNL ID5] 데스크탑 및 모바일 웹 페이지 방문자용 ID) 복사한 태그에서 `ID5_PARTNER_ID` (파트너 ID 포함) [!DNL ID5] 조직에 할당되었습니다.

   예를 들어 ID5 파트너 ID가 `abcde` 생성된 세그먼트 태그는

   ```<script src="https://playtime.tubemogul.com/ud/prod/universal_ids/segment.js?sid=012345&id5pid=ID5_PARTNER_ID"></script><img src="https://rtd-tm.everesttech.net/upi/?sid=012345&cs=1" />```

   다음 바꾸기 `ID5_PARTNER_ID` 포함 `abcde` 를 사용하여 다음을 얻을 수 있습니다.

   ```<script src="https://playtime.tubemogul.com/ud/prod/universal_ids/segment.js?sid=012345&id5pid=abcde"></script><img src="https://rtd-tm.everesttech.net/upi/?sid=012345&cs=1" />```

   귀사는 와(과) 계약을 체결할 때 파트너 ID를 받았습니다. [!DNL ID5]. 파트너 ID를 모르는 경우 Adobe 계정 팀에 문의하십시오.

   이 단계는 태그가 추적하는 데 필요하지 않습니다 [!DNL ID5] 데스크탑 또는 모바일 장치에서 광고 장치에 노출된 사용자의 ID입니다.

1. 다음 중 하나에 태그를 추가합니다. [!UICONTROL Pixel] 각 관련 광고 또는 [!UICONTROL Event Pixels] 의 섹션 [[!UICONTROL Tracking] 각 관련 배치에 대한 설정](/help/dsp/campaign-management/placements/placement-settings.md#placement-tracking).

추적 태그가 구현되면 모든 배치에 대해 대상 타겟 또는 제외에서 세그먼트를 사용할 수 있습니다.

>[!TIP]
>
>사용자가 추적될 때 세그먼트 크기를 추적합니다.

>[!MORELIKETHIS]
>
>* [대상자 관리 기본 정보](audience-about.md)
>* [세그먼트 정보 편집](segment-edit.md)
>* [세그먼트 삭제](segment-delete.md)
>* [세그먼트에 대한 추적 픽셀 보기](segment-view-pixels.md)
>* [세그먼트 공유 또는 공유 중지](segment-share.md)
>* [만들기 및 구현 [!UICONTROL CCPA Opt-Out-of-Sale] 세그먼트](ccpa-opt-out-segment-create.md)
>* [재사용 가능한 대상 만들기](reusable-audience-create.md)
>* [사용 가능한 타사 데이터 공급자](third-party-data-providers.md)
>* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)
