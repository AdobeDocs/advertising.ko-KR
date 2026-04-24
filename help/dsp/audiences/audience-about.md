---
title: About audience management in Advertising DSP
description: Learn about audience management features.
feature: DSP Audiences, DSP Segments
exl-id: 44cfe67e-e495-447f-b08f-d3789bd4dd09
TQID: https://experienceleague.adobe.com/IocF0s67I-vJAUx9Eom-aWEf-Q6H-ZOjczyGr0f9PsA
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2:
  - id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
subfeature_v2:
  - id: c193c532-b70e-4556-bde7-857186cbe140
  - id: fef5c122-6482-4d17-a8ce-4e70b906f1f4
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: c4d69b3aac9c963d13e3083f71931e507e58e616
workflow-type: tm+mt
source-wordcount: 1394
ht-degree: 0%

---

# About audience management in Advertising DSP

In DSP, you can create and manage audience segments and audience sets, which you can use as targets for your placements:

* Collect your own first-party audience data by creating and implementing DSP segments. You can later retarget users in the segment with ads or prevent users in the segment from receiving ads. You can create the following types of segments:

   * [Custom segments](/help/dsp/audiences/custom-segment-create.md) to track a) users exposed to ads from desktop and mobile devices and b) users who visit specific webpages. The tracking tag can track either cookie-based users or users associated with ID5 universal IDs.

   * [CCPA opt-out-of-sale segments](/help/dsp/audiences/ccpa-opt-out-segment-create.md) to track the users IDs from consumer opt-out-of-sale requests on your website, per the California Consumer Privacy Act (CCPA). You can retrieve monthly reports of the user IDs from opt-out-of-sale requests.

     For more information about Adobe Advertising support for CCPA opt-out-of-sale requests, see [Adobe Advertising support for the California Consumer Privacy Act: Consumer opt-out of sale support](/help/privacy/ccpa/ccpa-opt-out-of-sale.md).

* (Beta feature) [Obtain and use universal IDs for cookieless targeting](/help/dsp/audiences/universal-ids.md):

   * Manually send your authenticated [!DNL LiveRamp] [!DNL RampID] segments directly to DSP.

   * Allow DSP to import first-party segments from your customer data platform and translate them to supported universal ID types.

   * Include third-party segments that contain universal IDs in your placement targets without any extra steps.

* Create an audience library of [reusable audiences](/help/dsp/audiences/reusable-audience-create.md). Saved audiences are composed of any of your available audience segments and any of your other saved audiences. Any changes you make to a saved audience are automatically applied to all placements that target or exclude the audience and to all other audiences that include the saved audience.

  Saved audiences allow media planners to group audiences as needed, by including and excluding multiple segments using complex Boolean logic. The  (targetable) size of each individual segment and the overall active audience size are indicated as you build an audience. Campaign executioners can then simply select one or more saved audiences as placement targets rather than manually configure audience targets for each placement.

Additional audience types are also available for placement targeting.

## Importing first-party and third-party data segments

You have many options to import first-party and third-party data segments into DSP, using the DSP user interface and/or through custom import services.

* DSP can pull in your Adobe Audience Manager and other [!DNL Adobe] audiences for targeting. For prerequisites and instructions, see &quot;[Import Adobe Audience Manager segments for ad targeting](/help/integrations/audience-manager/import-audiences.md).

* DSP can translate first-party data segments from supported customer data platforms to segments with universal IDs using the [Sources feature](/help/dsp/audiences/sources/source-about.md). You can also [manually send your authenticated [!DNL LiveRamp] [!DNL RampID] segments directly to DSP](/help/dsp/audiences/sources/source-import-liveramp-segments.md).

* DSP can import your other first-party data segments directly from your data management platform (DMP) and provide them to any set of advertisers, as needed.

* DSP can import custom third-party segments, including complex combinations of third-party segments. You can provide the segments to any set of advertisers, as needed.

자세한 내용은 Adobe 계정 팀에 문의하십시오.

## Audiences available as placement targets

You can target your placements to all of the following types of audiences.

* All user-created audience sets that were saved in DSP.

* All user-created audience segments that were created in DSP:

   * Custom segments for users who visited specific webpages and users exposed to impressions of specific ads.

     No fees are incurred for impressions delivered to universal IDs.

   * CCPA opt-out-of-sale audience segments for users who submitted opt-out-of-sale requests on your website, per the California Consumer Privacy Act (CCPA).

* All of your imported first-party data segments, including segments that were translated to universal IDs.

  Additional fees are charged for impressions delivered to universal IDs. See &quot;[About first-party audience sources](/help/dsp/audiences/sources/source-about.md)&quot; for rates.

* All of your imported custom third-party data segments.

* (Placements targeting the U.S. only) [All third-party data segments available to DSP customers from over 30 providers](/help/dsp/audiences/third-party-data-providers.md), including [!DNL eXelate], ([!DNL Eyeota]), ([!DNL LiveRamp]),[!DNL Lotame], [!DNL Neustar], and many more.

  You can target specific segments, which target users based on audience data (for example, users with specific demographics, interests or intents, and/or behavioral profiles). You can browse by data provider and category, search for segments by name or segment ID, or filter the results by data provider, active segment size, web browser count, or devices count.

  타사 세그먼트는 각 세그먼트 이름 옆에 표시되는 추가 비용을 발생시킵니다.

* (Adobe Advertising JavaScript 전환 태그만 사용하는 Adobe Experience Platform 및 [!DNL Real-Time CDP], Adobe Audience Manager 또는 Adobe Analytics을 사용하는 광고주) [!DNL Real-Time CDP]에서 만들었거나, Audience Manager에서 만들었거나, Audience Manager 또는 [!DNL Analytics]에서 Adobe CX Enterprise에 게시한 사용 가능한 모든 퍼스트 파티, 세컨드 파티 또는 서드파티 대상 세그먼트.

  세그먼트 사용에 대한 요금은 사전 협상되며 DSP에 표시되지 않습니다.

  [!DNL Analytics]의 세그먼트는 CX Enterprise 대상자로 만들거나 게시한 후 약 1시간 후에 사용할 수 있습니다. Audience Manager 또는 [!DNL Real-Time CDP]에서 직접 가져온 세그먼트는 공유한 후 24시간 이내에 사용할 수 있습니다.

  >[!NOTE]
  >
  >해당 솔루션의 세그먼트에 대한 데이터 설정 및 수집에 대한 자세한 내용은 [Audience Manager](https://experienceleague.adobe.com/docs/audience-manager/user-guide/aam-home.html?lang=ko), [Analytics](https://experienceleague.adobe.com/docs/analytics.html?lang=ko) 및 [the [!DNL Real-Time CDP]](https://experienceleague.adobe.com/docs/experience-platform/rtcdp/segmentation/segment-builder-guide.html?lang=ko) 설명서를 참조하십시오.

## 대상 크기 데이터

대상 > 모든 대상 및 배치 설정의 대상 타깃팅 섹션에서 특정 장치 유형 또는 범용 ID 유형에 대해 별도의 범위를 포함하여 크기 범위별로 각 세그먼트 목록을 필터링할 수 있습니다.

![대상 크기별로 필터링](/help/dsp/assets/audience-size-filter.png)

또한 자세한 대상 크기 데이터를 볼 수 있습니다.

* 선택한 모든 세그먼트 및 저장된 대상에 대해 중복 제거된 활성 대상 크기가 표시되며, 디바이스 유형(브라우저, 모바일 또는 연결된 TV)별로 세부 정보를 볼 수 있습니다.

  ![결합된 대상 크기](/help/dsp/assets/audience-size.png)

* 개별 세그먼트의 경우 세그먼트 이름 옆에 활성 대상자 크기 및 CPM(해당하는 경우)가 표시됩니다.

  ![개별 세그먼트 크기](/help/dsp/assets/audience-size-segment.png)

* 브라우저, 모바일, 연결된 TV 및 범용 ID 유형 파트너별 크기를 포함하여 개별 세그먼트 또는 저장된 대상자에 대한 자세한 내용을 볼 수 있습니다. 저장된 대상자의 경우, 총 활성 대상자 크기는 중복 제거된 합계입니다.

  ![개별 세그먼트 또는 저장된 대상자 세부 정보](/help/dsp/assets/audience-size-segment-details.png)

## [!UICONTROL Audiences] 보기

### [!UICONTROL All Audiences] 보기

[!UICONTROL All Audiences] 보기 또는 대상 라이브러리에서는 대상 세그먼트 그룹과 다른 저장된 대상을 포함하여 재사용 가능한 대상을 저장하고 관리할 수 있습니다. 여러 배치에 대한 타겟으로 대상을 사용할 수 있습니다. 각 대상자가 사용되는 배치 수는 배치 이름 옆에 표시됩니다.

모든 대상을 편집, 복제, 삭제, 내보내기 또는 공유할 수 있습니다.

### [!UICONTROL Segments] 보기

[!UICONTROL Segments] 보기에서 모든 사용자는 추가 사용자 지정 세그먼트를 만들 수 있습니다.

[!UICONTROL Segments] 보기에는 다음 세그먼트 유형도 나열됩니다.

* 사용자가 만든 모든 사용자 정의 세그먼트를 사용자가 사용할 수 있습니다.

  만든 사용자 지정 세그먼트에 대한 추적 태그를 보고 다른 사용자와 공유할 수 있습니다. 만든 사용자 지정 세그먼트를 편집하거나 삭제할 수도 있습니다.

  다른 사용자가 귀하와 공유한 사용자 지정 세그먼트를 편집하거나 공유할 수 없습니다.

* 있는 그대로 가져온, 사용자가 사용할 수 있는 모든 자사 세그먼트.

  공유된 자사 세그먼트를 편집하거나 공유할 수 없습니다. 자사 세그먼트를 추가 사용자와 공유해야 하는 경우 Adobe 계정 팀에 문의하십시오.

* 사용자가 사용할 수 있는 모든 사용자 지정 타사 세그먼트.

  사용자와 공유된 서드파티 세그먼트를 편집하거나 공유할 수 없습니다. 추가 사용자와 서드파티 세그먼트를 공유해야 하는 경우 Adobe 계정 팀에 문의하십시오.

### [!UICONTROL Sources] 보기

[!UICONTROL Sources] 보기에서는 지정된 범용 ID 유형이 포함된 세그먼트로 변환할 지원되는 고객 데이터 플랫폼의 자사 세그먼트에 대한 소스를 구성할 수 있습니다. 소스 설정에는 연결을 설정하기 위해 고객 데이터 플랫폼에 제공할 자동 생성된 소스 키가 포함되어 있습니다.

지원되는 고객 데이터 플랫폼, 지원되는 범용 ID 유형 및 각 고객 데이터 플랫폼에 대한 연결을 설정하는 워크플로에 대한 자세한 내용은 &quot;[자사 대상 소스 정보](/help/dsp/audiences/sources/source-about.md)&quot;를 참조하십시오.

번역된 세그먼트는 재사용 가능한 대상 및 쿠키 없는 타깃팅을 위한 배치 설정에 포함할 수 있습니다.

>[!MORELIKETHIS]
>
>* [범용 ID 활성화 지원](/help/dsp/audiences/universal-ids.md)
>* [재사용 가능한 대상 만들기](reusable-audience-create.md)
>* [사용자 지정 세그먼트 만들기 및 구현](custom-segment-create.md)
>* [[!UICONTROL CCPA Opt-Out-of-Sale] 세그먼트 만들기 및 구현](ccpa-opt-out-segment-create.md)
>* [자사 대상 원본 정보](/help/dsp/audiences/sources/source-about.md)
>* [범용 ID 대상을 활성화하기 위한 대상 소스 관리](/help/dsp/audiences/sources/source-manage.md)
>* [인증된 세그먼트를 수동으로 가져오기 [!DNL LiveRamp]](/help/dsp/audiences/sources/source-import-liveramp-segments.md)
>* [사용 가능한 타사 데이터 공급자](third-party-data-providers.md)
>* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)
