---
title: 광고 타깃팅을 위한 Adobe Audience Manager 세그먼트 가져오기
description: 을(를) 가져오는 방법 알아보기 [!DNL Adobe] 대상을 Advertising DSP 및 Adobe Audience Manager을 사용한 검색
feature: Integration with Adobe Audience Manager
exl-id: 6ff80699-9554-4b39-a019-d8055d68c174
source-git-commit: 7f35b3f3b33ed320ac186d219cbd0f826666bb3b
workflow-type: tm+mt
source-wordcount: '763'
ht-degree: 0%

---

# 광고 타깃팅을 위한 Adobe Audience Manager 세그먼트 가져오기

Advertising DSP 및 [!DNL Advertising Search, Social, & Commerce] 는 각각 모든 광고주 또는 에이전시에 대한 메타데이터, 계층 데이터 및 고유 대상 데이터를 가져올 수 있습니다 [!DNL Adobe] 대상<!-- segments or audiences? Standardize terms per AAM's docs -->. 여기에는 다음에 대한 데이터가 포함됩니다.

* Adobe Audience Manager 세그먼트

* Adobe Experience Cloud에 게시된 Adobe Analytics 세그먼트

* Adobe Experience Cloud을 사용하여 생성된 세그먼트 [!DNL Audience Library]

* Adobe Experience Platform에서 생성되어 Audience Manager을 통해 Adobe 광고로 전송되는 세그먼트

액세스하려면 [!DNL Adobe] DSP 또는 의 대상 [!DNL Creative], 대상자를 DSP으로 가져와야 합니다. 액세스하려면 [!DNL Adobe] 의 대상 [!DNL Search, Social, & Commerce], 대상자를 (으)로 가져와야 합니다 [!DNL Search, Social, & Commerce].

## 전제 조건

* 광고주가 다음을 구현해야 합니다. [다음 [!DNL Adobe Experience Cloud Identity (ECID) Service]](https://experienceleague.adobe.com/docs/id-service/using/intro/overview.html) 버전 2.0 이상 다음 [!DNL Identity Service] 는 Experience Cloud의 모든 솔루션에서 방문자를 식별하는 범용 영구 ID를 제공합니다.

   구현에는 다음 항목 추가가 포함됩니다 [!DNL Identity service] 광고주 사이트의 각 웹 페이지에 코드를 추가합니다.

* 조직은 다음과 같아야 합니다. [Experience Cloud 서비스에 대해 활성화됨](https://experienceleague.adobe.com/docs/core-services/interface/services/core-services.html) Experience Cloud [!DNL Organization ID] (이전 호출 [!DNL IMS org ID]).

   다음 [!UICONTROL Organization ID] 여러 Adobe Experience Cloud 제품이 있는 조직이 일부 제품 간에 데이터를 공유할 수 있도록 합니다.

* (광고주: [!DNL Analytics]) 광고주는 [구현 [!DNL Analytics] 사용 `appMeasurement.js`](https://experienceleague.adobe.com/docs/analytics/implementation/js/overview.html) 버전 1.6.4 이상

* 광고주의 웹 사이트 방문자는 많은 양을 포함하지 않습니다 [!DNL Apple Safari] 사용자.

* (광고주가 Audience Manager과 을 모두 사용할 때 권장됨) [!DNL Analytics]) 각 웹 페이지에 대한 호출을 줄이려면 기존 Audience Manager을 제거하십시오 [!DNL Data Integration Library] 데이터 수집을 위한 코드 및 각 코드에 대한 서버측 전달 활성화 [!DNL Analytics] 보고서 세트 를 사용하십시오. 자세한 내용은 &quot;[서버측 전달 개요](https://experienceleague.adobe.com/docs/analytics/admin/admin-tools/server-side-forwarding/ssf.html).

* (권장) 일치율이 높으면 자사 웹 사이트 데이터만 Adobe 광고로 보냅니다. 광고주가 고객 관계 관리 시스템의 타사 데이터 또는 오프라인 데이터를 번들로 제공하는 경우 데이터 유출로 인해 일치율이 감소할 수 있습니다.

## DSP에 Audience Manager 대상 가져오기

### 대상을 DSP으로 가져오는 단계

다음 [!DNL Adobe] account 및 data operations 팀이 다음 단계를 수행합니다.

1. Adobe 계정 팀은 광고주 수준 설정 을 구성해야 합니다.[!UICONTROL Adobe Analytics Cloud].&quot;

1. Adobe 계정 팀이 요청을 제출해야 합니다.<!-- Submit a request as a JIRA task? --> 데이터 운영 팀에 전달<!-- implementation team? --> advertising DSP 기본 API 통합을 사용하여 조직의 Audience Manager 세그먼트를 가져오려면 다음을 수행하십시오.

### 어떤 변경 사항이 Audience Manager을 발생시킵니까?

API는 자동으로

* Audience Manager에서 두 개의 DSP 대상을 만듭니다.

   * **[!UICONTROL Adobe Ad Cloud Cross-Channel (real-time)]**

   * **[!UICONTROL Adobe AdCloud Cross-Channel (batch)])**

* 두 대상을 모든 Audience Manager 세그먼트에 매핑하여 Audience Manager이 동일한 Experience Cloud과 연결된 DSP 광고주 계정과 세그먼트를 공유할 수 있도록 합니다 [!DNL Organization ID] Audience Manager에 사용됩니다. <!-- Verify -->

   조직은 선택적으로 Audience Manager 내의 대상에서 불필요한 세그먼트를 제거할 수 있습니다.

* 다음 Exchange 쿠키 동기화 픽셀을 조직의 Audience Manager 컨테이너에 추가하여 고객 캠페인의 도달 범위를 개선합니다.

   * Adobe AdCloud: 411(표준 및 의 일부로 자동 제공) [!DNL Identity Service] 버전 2.0. 다음을 보유한 조직 [!DNL Identity Service] 2.0 이하 버전에서는 이 픽셀을 Audience Manager 컨테이너에 추가해야 합니다.

## Audience Manager 대상 가져오기 [!DNL Search, Social, & Commerce]

### 대상자를 가져오는 단계 [!DNL Search, Social, & Commerce]

[!DNL Adobe] 직원은 다음 단계 중 대부분 또는 모두를 수행합니다.

1. Adobe 계정 팀은 데이터 운영 팀에 다음 작업 간의 통합을 설정하도록 요청을 제출해야 합니다. [!DNL Search, Social, & Commerce] Audience Manager. 내보낼 Audience Manager 세그먼트의 이름을 포함합니다 [!DNL Search, Social, & Commerce].

1. Audience Manager 내에서 대상 구성 [!DNL Search, Social, & Commerce]:

   1. 두 개의 새 대상을 만듭니다. `[!UICONTROL Adobe Media Optimizer (HTTP)]` 및 `[!UICONTROL Adobe Media Optimizer Batch Destination]`.

      [!DNL Media Optimizer] 은(는) 의 이전 이름입니다 [!DNL Search, Social, & Commerce].

   1. 각 대상에 대한 세그먼트를 지정합니다.

      포함 [!UICONTROL Automatically map all current and future segments] 옵션을 선택하면 모든 세그먼트가 매일 매핑되고 동기화됩니다.

      다음 [!UICONTROL Manually map segments] 옵션을 사용하면 세그먼트를 수동으로 매핑하여 배치 대상(`[!UICONTROL Adobe Media Optimizer Batch Destination]`). 세그먼트를 HTTP 대상에 수동으로 매핑할 필요가 없습니다.

1. 다음 범위 내 [!DNL Search, Social, & Commerce], 또는 [!DNL Search, Social, & Commerce] 구현 팀 또는 직접 액세스 클라이언트 관리자 역할이 있는 사용자가에서 가져오기를 시작해야 합니다. [!UICONTROL Search] > [!UICONTROL Admin] > [!UICONTROL Audience Manager Setup].

   조직의 Experience Cloud을 입력해야 합니다. [!DNL Organization ID] ([!DNL IMS org ID]). ID는 조직의 Audience Manager 계정에 사용되는 ID와 동일해야 합니다.

### 어떤 변경 사항이 Audience Manager을 발생시킵니까?

조직에 두 개의 항목이 표시됩니다. [!DNL Search, Social, & Commerce] Audience Manager의 대상:

* **[!UICONTROL Adobe Media Optimizer (HTTP)]**
* **[!UICONTROL Adobe Media Optimizer Batch Destination])**

## 데이터 동기화

초기 가져오기는 약 24시간이 소요됩니다. 처음 가져오기를 수행하면 데이터가 1~2초 지연으로 실시간으로 동기화됩니다.

<!--
### How DSP Syncs the Data

DSP syncs the data automatically using the [!DNL Adobe Experience Cloud Identity (ECID) Service]. During synchronization, the [!DNL ECID Service] calls Adobe Advertising at [!DNL cm.eversttech.net]. Because Adobe Advertising is a trusted domain, ID syncs take place from parent pages rather than within the destination publishing iframes, as they do with most third-party activation partners. Audience Manager identifies unique users by device IDs, using the [Audience Manager [!DNL Unique User ID (AAM UUID)]](https://experienceleague.adobe.com/docs/audience-manager/user-guide/reference/ids-in-aam.html#global-device-ids), also called the [!DNL Device ID].

![Synchronization of [!DNL Adobe] audiences in DSP](/help/integrations/assets/audience-manager-sync.png)

### How Search Syncs the Data
-->

<!-- 
Segment membership data is sent only after one of the following events occurs:

* (Advertisers with DSP):

  * The segment is targeted in an Adobe Advertising display ad.

  * The segment is added to the [!DNL Adobe AdCloud Cross-Channel] batch and real-time destinations within the Audience Manager user interface.

* (Advertisers with [!DNL Search, Social, & Commerce]):

  * The segment is targeted in an Adobe Advertising search ad.

  * The segment is added to the [!DNL Adobe Media Optimizer] batch and HTTP destinations within the Audience Manager user interface.
 -->
<!-- Is membership data/whatever available in Creative? If so, does it show the same as DSP? -->

## 동기화된 세그먼트를 찾을 수 있는 곳

### DSP

DSP에서 세그먼트 이름은 Audience Manager 분류법에 따라 구성되고 의 해당 세그먼트 멤버십 카운트와 함께 사용할 수 있습니다.

* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md#audience-targeting): 다음에서 [!UICONTROL Adobe Segments] 의 탭 [!UICONTROL Audience Targeting] 섹션.

* 위치 [대상자 설정](/help/dsp/audiences/audience-settings.md): 다음에서 [!UICONTROL Adobe Segments] 탭.

### Advertising Creative

위치 [!DNL Creative], 세그먼트는 target 노드에 대한 경험 설정에서 사용할 수 있습니다.

### 위치 [!DNL Advertising Search, Social, & Commerce]

위치 [!DNL Search, Social, & Commerce], 세그먼트는 를 만들 때 사용할 수 있습니다. [!DNL Google] 대상 사용 [!UICONTROL Data Source] &quot;[!UICONTROL Adobe Audience]&quot; 출처: [!UICONTROL Campaigns] > [!UICONTROL Audiences] > [!UICONTROL Library].

각 [!DNL Google] 사용자가 만드는 대상, [!DNL Google] 대상 크기를 제공합니다.

>[!MORELIKETHIS]
>
>* [Adobe Audience Manager과 Advertising 통합 Adobe](/help/integrations/audience-manager/overview.md)

