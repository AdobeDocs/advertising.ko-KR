---
title: 광고 타깃팅을 위한 Adobe Audience Manager 세그먼트 가져오기
description: ' [!DNL Adobe] 대상자를 Advertising DSP으로 가져오고 Adobe Audience Manager을 사용하여 검색하는 방법에 대해 알아봅니다.'
feature: Integration with Adobe Audience Manager
exl-id: 6ff80699-9554-4b39-a019-d8055d68c174
source-git-commit: e6635abdb34444bc40d833a3c6a5eaf07f9f1789
workflow-type: tm+mt
source-wordcount: '920'
ht-degree: 0%

---

# 광고 타깃팅을 위한 Adobe Audience Manager 세그먼트 가져오기

Advertising DSP 및 [!DNL Advertising Search, Social, & Commerce]은(는) 다음을 포함하여 모든 광고주 또는 에이전시의 [!DNL Adobe] 대상<!-- segments or audiences? Standardize terms per AAM's docs -->에 대한 메타데이터, 계층 데이터 및 고유한 대상 데이터를 가져올 수 있습니다.

* Adobe Audience Manager 세그먼트

* Adobe Experience Cloud에 게시된 Adobe Analytics 세그먼트

* Adobe Experience Cloud [!DNL Audience Library]을(를) 사용하여 만든 세그먼트

* Adobe Experience Platform에서 생성되어 Audience Manager을 통해 Adobe Advertising으로 전송되는 세그먼트

DSP 또는 [!DNL Creative]에서 [!DNL Adobe]개의 대상에 액세스하려면 대상을 DSP으로 가져와야 합니다. [!DNL Search, Social, & Commerce]에서 [!DNL Adobe]명의 대상자에 액세스하려면 대상자를 [!DNL Search, Social, & Commerce] (으)로 가져와야 합니다.

## 전제 조건

* 광고주는 [the [!DNL Adobe Experience Cloud Identity (ECID) Service]](https://experienceleague.adobe.com/en/docs/id-service/using/intro/overview) 버전 2.0 이상을 구현해야 합니다. [!DNL Identity Service]은(는) Experience Cloud의 모든 솔루션에서 방문자를 식별하는 범용 영구 ID를 제공합니다.

  구현에는 광고주 사이트의 각 웹 페이지에 [!DNL Identity service] 코드를 추가하는 작업이 포함됩니다.

* 조직은 Experience Cloud 서비스에 대해 [활성화됨](https://experienceleague.adobe.com/en/docs/core-services/interface/services/overview)이어야 하며 [!DNL Organization ID] Experience Cloud(이전 이름: [!DNL IMS org ID])이 있어야 합니다.

  [!UICONTROL Organization ID]을(를) 사용하면 여러 Adobe Experience Cloud 제품이 있는 조직에서 일부 제품 간에 데이터를 공유할 수 있습니다.

* (광고주: [!DNL Analytics]) 광고주는 `appMeasurement.js`[&#128279;](https://experienceleague.adobe.com/en/docs/analytics/implementation/js/overview) 버전 1.6.4 이상을 사용하여 구현 [!DNL Analytics] 해야 합니다.

* 광고주의 웹 사이트 방문자에 [!DNL Apple Safari]명의 사용자가 포함되지 않습니다.

* (광고주가 Audience Manager과 [!DNL Analytics]을(를) 모두 사용하는 경우 권장) 각 웹 페이지에 대한 호출을 줄이려면 데이터 수집을 위해 기존 Audience Manager [!DNL Data Integration Library] 코드를 제거하고 대신 각 [!DNL Analytics] 보고서 세트에 대해 서버측 전달을 사용하도록 설정하십시오. 자세한 내용은 &quot;[서버측 전달 개요](https://experienceleague.adobe.com/en/docs/analytics/admin/admin-tools/manage-report-suites/edit-report-suite/report-suite-general/server-side-forwarding/ssf)를 참조하십시오.

* (권장) 일치율을 높이려면 자사 웹 사이트 데이터만 Adobe Advertising으로 보냅니다. 광고주가 고객 관계 관리 시스템의 타사 데이터 또는 오프라인 데이터를 번들로 제공하는 경우 데이터 유출로 인해 일치율이 감소할 수 있습니다.

## DSP에 Audience Manager 대상 가져오기

### 대상을 DSP으로 가져오는 단계

[!DNL Adobe] 계정 및 데이터 작업 팀은 다음 단계를 수행합니다.

1. Adobe 계정 팀은 광고주 수준 설정 &quot;[!UICONTROL Adobe Analytics Cloud]&quot;을(를) 구성해야 합니다.

1. Adobe 계정 팀은 Advertising DSP 기본 API 통합을 사용하여 조직의 Audience Manager 세그먼트를 가져오도록 데이터 운영 팀에 요청을 제출해야 합니다.

### 어떤 변경 사항이 Audience Manager을 발생시킵니까?

API는 자동으로

* Audience Manager에서 두 개의 DSP 대상을 만듭니다.

   * **[!UICONTROL Adobe AdCloud Cross-Channel (real-time)]**

   * **[!UICONTROL Adobe AdCloud Cross-Channel (batch)]**

* 두 대상을 모든 Audience Manager 세그먼트에 매핑하여 Audience Manager이 Audience Manager에 사용된 동일한 Experience Cloud [!DNL Organization ID]과(와) 연결된 DSP 광고주 계정과 세그먼트를 공유할 수 있도록 합니다.

  조직은 선택적으로 Audience Manager 내의 대상에서 불필요한 세그먼트를 제거할 수 있습니다.

* 다음 Exchange 쿠키 동기화 픽셀을 조직의 Audience Manager 컨테이너에 추가하여 고객 캠페인의 도달 범위를 개선합니다.

   * Adobe AdCloud: 411(이 픽셀은 [!DNL Identity Service] 버전 2.0의 일부로 기본적으로 제공되며 자동으로 제공됩니다. [!DNL Identity Service] 버전이 2.0 미만인 조직에서는 이 픽셀을 Audience Manager 컨테이너에 추가해야 합니다.

## [!DNL Search, Social, & Commerce] (으)로 Audience Manager 대상 가져오기

### 대상자를 [!DNL Search, Social, & Commerce] (으)로 가져오는 단계

[!DNL Adobe]명의 직원이 다음 단계를 대부분 또는 모두 수행합니다.

1. Adobe 계정 팀은 [!DNL Search, Social, & Commerce]과(와) Audience Manager 간의 통합을 설정하도록 데이터 작업 팀에 요청을 제출해야 합니다. [!DNL Search, Social, & Commerce] (으)로 내보낼 Audience Manager 세그먼트의 이름을 포함합니다.

1. Audience Manager 내에서 [!DNL Search, Social, & Commerce]의 대상을 구성합니다.

   1. 두 개의 새 대상을 만듭니다. `[!UICONTROL Adobe Media Optimizer (HTTP)]` 및 `[!UICONTROL Adobe Media Optimizer Batch Destination]`.

      [!DNL Media Optimizer]은(는) [!DNL Search, Social, & Commerce]의 이전 이름입니다.

   1. 각 대상에 대한 세그먼트를 지정합니다.

      [!UICONTROL Automatically map all current and future segments] 옵션을 사용하면 모든 세그먼트가 매일 매핑되고 동기화됩니다.

      [!UICONTROL Manually map segments] 옵션을 사용하면 세그먼트를 수동으로 매핑하여 배치 대상(`[!UICONTROL Adobe Media Optimizer Batch Destination]`)과 동기화할 수 있습니다. 세그먼트를 HTTP 대상에 수동으로 매핑할 필요가 없습니다.

1. [!DNL Search, Social, & Commerce] 내에서 [!DNL Search, Social, & Commerce] 구현 팀이나 직접 액세스 클라이언트 관리자 역할을 가진 사용자가 [!UICONTROL Search] > [!UICONTROL Admin] > [!UICONTROL Audience Manager Setup]에서 가져오기를 시작해야 합니다.

   조직의 Experience Cloud [!DNL Organization ID] ([!DNL IMS org ID])이(가) 필요합니다. ID는 조직의 Audience Manager 계정에 사용되는 ID와 동일해야 합니다.

### 어떤 변경 사항이 Audience Manager을 발생시킵니까?

Audience Manager에서 조직에 대해 두 개의 [!DNL Search, Social, & Commerce] 대상을 사용할 수 있게 되었습니다.

* **[!UICONTROL Adobe Media Optimizer (HTTP)]**
* **[!UICONTROL Adobe Media Optimizer Batch Destination]**

## 데이터 동기화

초기 가져오기는 약 24시간이 소요됩니다. 초기 가져오기 후 데이터는 1~2초 지연으로 실시간으로 동기화됩니다.

다음 이벤트 중 하나가 발생한 후에만 세그먼트 멤버십 데이터가 전송됩니다.

* (DSP 사용 광고주):

   * 세그먼트는 Adobe Advertising 표시 광고에서 타겟팅됩니다.

   * 세그먼트가 Audience Manager 사용자 인터페이스 내의 [!DNL Adobe AdCloud Cross-Channel] 일괄 처리 및 실시간 대상에 추가됩니다.

* ([!DNL Search, Social, & Commerce]을(를) 가진 광고주):

   * 세그먼트는 Adobe Advertising 검색 광고에서 타겟팅됩니다.

   * 세그먼트가 Audience Manager 사용자 인터페이스 내의 [!DNL Adobe Media Optimizer] 일괄 처리 및 HTTP 대상에 추가됩니다.

<!-- Is membership data/whatever available in Creative? If so, does it show the same as DSP? -->

### DSP이 데이터를 동기화하는 방법

DSP은 [!DNL Adobe Experience Cloud Identity (ECID) Service]을(를) 사용하여 데이터를 자동으로 동기화합니다. 동기화하는 동안 [!DNL ECID Service]이(가) [!DNL cm.everesttech.net]에 Adobe Advertising을 호출합니다. Adobe Advertising은 신뢰할 수 있는 도메인이므로 대부분의 타사 활성화 파트너와 마찬가지로 ID 동기화는 대상 게시 iframe 내에서가 아니라 상위 페이지에서 수행됩니다. Audience Manager은 [!DNL Device ID]이라고도 하는 [Audience Manager [!DNL Unique User ID (AAM UUID)]](https://experienceleague.adobe.com/en/docs/audience-manager/user-guide/reference/ids-in-aam)을(를) 사용하여 장치 ID별로 고유 사용자를 식별합니다.

<!--
![Synchronization of [!DNL Adobe] audiences in DSP](/help/integrations/assets/audience-manager-sync.png)
-->

### 검색, 소셜 및 Commerce이 데이터를 동기화하는 방법

Search, Social 및 Commerce은 [!DNL Adobe Experience Cloud Identity (ECID) Service]을(를) 사용하여 데이터를 자동으로 동기화합니다. 동기화하는 동안 [!DNL ECID Service]이(가) Adobe Advertising에 속하는 신뢰할 수 있는 도메인인 [!DNL cm.everesttech.net]에서 Adobe Advertising을 호출합니다. Audience Manager은 [!DNL Device ID]이라고도 하는 [Audience Manager [!DNL Unique User ID (AAM UUID)]](https://experienceleague.adobe.com/en/docs/audience-manager/user-guide/reference/ids-in-aam)을(를) 사용하여 장치 ID별로 고유 사용자를 식별합니다.

## 동기화된 세그먼트를 찾을 수 있는 곳

### DSP

DSP은 세그먼트 분류법에 따라 Audience Manager 이름을 구성하고 해당 세그먼트 멤버십 수를 다음 위치에 포함합니다.

* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md#audience-targeting): [!UICONTROL Audience Targeting] 섹션의 [!UICONTROL Adobe Segments] 탭에서.

* [대상 설정](/help/dsp/audiences/audience-settings.md)에서: [!UICONTROL Adobe Segments] 탭에서.

### Advertising Creative

[!DNL Creative]에서 대상 노드에 대한 경험 설정에서 세그먼트를 사용할 수 있습니다.

### [!DNL Advertising Search, Social, & Commerce]에서

[!DNL Search, Social, & Commerce]에서 [!UICONTROL Campaigns] > [!UICONTROL Audiences] > [!UICONTROL Library]에서 [!UICONTROL Data Source] &quot;[!UICONTROL Adobe Audience]&quot;을(를) 사용하여 [!DNL Google] 대상자를 만들 때 세그먼트를 사용할 수 있습니다.

만든 각 [!DNL Google] 대상에 대해 [!DNL Google]에서 대상 크기를 제공합니다.

>[!MORELIKETHIS]
>
>* [Adobe Audience Manager과 통합 Adobe Advertising](/help/integrations/audience-manager/overview.md)
