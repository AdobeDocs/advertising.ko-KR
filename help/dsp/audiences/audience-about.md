---
title: Advertising DSP의 고객 관리 정보
description: 대상자 관리 기능에 대해 알아봅니다.
feature: DSP Audiences, DSP Segments
exl-id: 44cfe67e-e495-447f-b08f-d3789bd4dd09
source-git-commit: 31f20bcfb79265326f515218a02d8a4fa3efd586
workflow-type: tm+mt
source-wordcount: '1324'
ht-degree: 0%

---

# Advertising DSP의 고객 관리 정보

DSP에서 배치에 대한 타겟으로 사용할 수 있는 대상 세그먼트 및 대상 세트를 만들고 관리할 수 있습니다.

* DSP 세그먼트를 만들고 구현하여 고유한 자사 대상 데이터를 수집합니다. 나중에 광고를 사용하여 세그먼트의 사용자를 다시 타겟팅하거나 세그먼트의 사용자가 광고를 받지 못하도록 할 수 있습니다. 다음 유형의 세그먼트를 만들 수 있습니다.

   * [사용자 지정 세그먼트](/help/dsp/audiences/custom-segment-create.md) - a) 데스크톱 및 모바일 장치에서 광고에 노출되는 사용자, b) 특정 웹 페이지를 방문하는 사용자를 추적합니다. 추적 태그는 쿠키 기반 사용자 또는 ID5 범용 ID와 연결된 사용자를 추적할 수 있습니다.

   * CCPA(California Consumer Privacy Act)에 따라 [CCPA 판매 중지 세그먼트](/help/dsp/audiences/ccpa-opt-out-segment-create.md)를 통해 웹 사이트의 소비자 판매 중지 요청에서 사용자 ID를 추적할 수 있습니다. 판매 중지 요청에서 사용자 ID의 월별 보고서를 검색할 수 있습니다.

     CCPA 판매 중지 요청에 대한 Adobe Advertising 지원에 대한 자세한 내용은 [캘리포니아 소비자 개인정보 보호법: 소비자 옵트아웃 지원에 대한 Adobe Advertising 지원](/help/privacy/ccpa/ccpa-opt-out-of-sale.md)을 참조하십시오.

* (Beta 기능) [쿠키 없는 타깃팅을 위해 유니버설 ID를 가져와 사용](/help/dsp/audiences/universal-ids.md):

   * 인증된 [!DNL LiveRamp] [!DNL RampID] 세그먼트를 수동으로 DSP에 직접 보냅니다.

   * DSP에서 고객 데이터 플랫폼에서 자사 세그먼트를 가져와 지원되는 범용 ID 유형으로 번역할 수 있도록 허용합니다.

   * 추가 단계 없이 배치 대상에 범용 ID가 포함된 서드파티 세그먼트를 포함합니다.

* [재사용 가능한 대상](/help/dsp/audiences/reusable-audience-create.md)의 대상 라이브러리를 만듭니다. 저장된 대상은 사용 가능한 대상 세그먼트와 다른 저장된 대상으로 구성됩니다. 저장된 대상에 대한 변경 사항은 대상을 타깃팅하거나 제외하는 모든 배치와 저장된 대상을 포함하는 다른 모든 대상에 자동으로 적용됩니다.

  저장된 대상을 사용하면 미디어 플래너는 복잡한 부울 논리를 사용하여 여러 세그먼트를 포함 및 제외함으로써, 필요에 따라 대상을 그룹화할 수 있습니다. 대상자를 만들 때 각 개별 세그먼트의 크기와 총 대상자 크기가 표시됩니다. 그런 다음 캠페인 실행자는 각 배치에 대한 대상 타겟을 수동으로 구성하는 대신, 저장된 하나 이상의 대상을 배치 타겟으로 선택하면 됩니다.

배치 타깃팅에 추가 대상자 유형을 사용할 수도 있습니다.

## 자사 및 타사 데이터 세그먼트 가져오기

DSP 사용자 인터페이스를 사용하거나 사용자 지정 가져오기 서비스를 통해 자사 및 타사 데이터 세그먼트를 DSP으로 가져오는 다양한 옵션이 있습니다.

* DSP은 타깃팅을 위해 Adobe Audience Manager 및 기타 [!DNL Adobe]개의 대상을 가져올 수 있습니다. 전제 조건 및 지침은 &quot;[광고 타깃팅을 위한 Adobe Audience Manager 세그먼트 가져오기](/help/integrations/audience-manager/import-audiences.md)를 참조하십시오.

* DSP은 [소스 기능](/help/dsp/audiences/sources/source-about.md)을 사용하여 지원되는 고객 데이터 플랫폼의 자사 데이터 세그먼트를 범용 ID가 있는 세그먼트로 변환할 수 있습니다. [인증된  [!DNL LiveRamp] [!DNL RampID] 세그먼트를 수동으로 DSP에 보낼 수 있습니다](/help/dsp/audiences/sources/source-import-liveramp-segments.md).

* DSP은 DMP(데이터 관리 플랫폼)에서 직접 다른 자사 데이터 세그먼트를 가져와 필요한 경우 광고주 집합에 제공할 수 있습니다.

* DSP은 복잡한 타사 세그먼트의 조합을 포함하는 사용자 지정 타사 세그먼트를 가져올 수 있습니다. 필요에 따라 모든 광고주 세트에 세그먼트를 제공할 수 있습니다.

자세한 내용은 Adobe 계정 팀에 문의하십시오.

## 배치 타겟으로 사용할 수 있는 대상

배치를 다음 유형의 모든 대상으로 타깃팅할 수 있습니다.

* DSP에 저장된 사용자가 만든 모든 대상자 세트입니다.

* DSP에서 만든 사용자가 만든 모든 대상 세그먼트:

   * 특정 웹 페이지를 방문한 사용자 및 특정 광고의 노출에 노출된 사용자를 위한 사용자 지정 세그먼트입니다.

     범용 ID에 게재되는 노출에 대해서는 요금이 부과되지 않습니다.

   * 캘리포니아 소비자 개인정보 보호법(CCPA)에 따라 웹 사이트에서 판매 중지 요청을 제출한 사용자에 대한 CCPA 판매 중지 대상 세그먼트입니다.

* 범용 ID로 번역된 세그먼트를 포함하여 가져온 모든 자사 데이터 세그먼트.

  범용 ID에 게재되는 노출에 대해 추가 비용이 청구됩니다. 요율은 &quot;[자사 대상 소스 정보](/help/dsp/audiences/sources/source-about.md)&quot;를 참조하십시오.

* 가져온 모든 사용자 지정 타사 데이터 세그먼트.

* (미국만 대상으로 하는 배치) [모든 타사 데이터 세그먼트는 DSP 고객이 30개 이상의 공급자에서 사용할 수 있습니다](/help/dsp/audiences/third-party-data-providers.md)(예: [!DNL eXelate], ([!DNL Eyeota]), ([!DNL LiveRamp]),[!DNL Lotame], [!DNL Neustar] 등).

  대상 데이터에 따라 사용자를 타겟팅하는 특정 세그먼트를 타겟팅할 수 있습니다(예: 특정 인구 통계, 관심사나 의도를 가진 사용자 및/또는 행동 프로필). 데이터 공급자와 범주별로 찾아보거나, 이름 또는 세그먼트 ID별로 세그먼트를 검색하거나, 데이터 공급자, 총 세그먼트 크기, 웹 브라우저 개수 또는 장치 개수별로 결과를 필터링할 수 있습니다.

  타사 세그먼트는 각 세그먼트 이름 옆에 표시되는 추가 비용을 발생시킵니다.

* (Adobe Advertising JavaScript 전환 태그만 사용하는 Adobe Experience Platform 및 [!DNL Real-Time CDP], Adobe Audience Manager 또는 Adobe Analytics을 사용하는 광고주) [!DNL Real-Time CDP]에서 만들었거나, Audience Manager에서 만들었거나, Audience Manager 또는 [!DNL Analytics]에서 Adobe Experience Cloud에 게시한 모든 사용 가능한 자사, 타사 또는 타사 대상 세그먼트입니다.

  세그먼트 사용에 대한 요금은 사전 협상되며 DSP에 표시되지 않습니다.

  [!DNL Analytics]의 세그먼트는 Experience Cloud 대상으로 만들거나 게시한 후 약 1시간 후에 사용할 수 있습니다. Audience Manager 또는 [!DNL Real-Time CDP]에서 직접 가져온 세그먼트는 공유한 후 24시간 이내에 사용할 수 있습니다.

  >[!NOTE]
  >
  >해당 솔루션의 세그먼트에 대한 데이터 설정 및 수집에 대한 자세한 내용은 [Audience Manager](https://experienceleague.adobe.com/docs/audience-manager/user-guide/aam-home.html), [분석](https://experienceleague.adobe.com/docs/analytics.html) 및 [추가 [!DNL Real-Time CDP]](https://experienceleague.adobe.com/docs/experience-platform/rtcdp/segmentation/segment-builder-guide.html)에 대한 설명서를 참조하십시오.

## 대상 크기 데이터

대상 > 모든 대상 및 배치 설정의 대상 타깃팅 섹션에서 특정 장치 유형 또는 범용 ID 유형에 대한 전체 범위 및 개별 범위를 포함하여 크기 범위별로 각 세그먼트 목록을 필터링할 수 있습니다.

![대상 크기별로 필터링](/help/dsp/assets/audience-size-filter.png)

또한 자세한 대상 크기 데이터를 볼 수 있습니다.

* 선택한 모든 세그먼트 및 저장된 대상에 걸쳐 중복 제거된 총 활성 대상 크기가 표시되며, 디바이스 유형(브라우저, 모바일 또는 연결된 TV)별로 세부 정보를 볼 수 있습니다.

  ![결합된 대상 크기](/help/dsp/assets/audience-size.png)

* 개별 세그먼트의 경우 세그먼트 이름 옆에 총 대상자 크기 및 CPM(해당되는 경우)이 표시됩니다.

  ![개별 세그먼트 크기](/help/dsp/assets/audience-size-segment.png)

* 브라우저, 모바일, 연결된 TV 및 범용 ID 유형 파트너별 크기를 포함하여 개별 세그먼트 또는 저장된 대상자에 대한 자세한 내용을 볼 수 있습니다. 저장된 대상자의 경우, 총 크기는 중복 제거된 합계입니다.

  ![개별 세그먼트 또는 저장된 대상자 세부 정보](/help/dsp/assets/audience-size-segment-details.png)

## 대상 보기

### 모든 대상 보기

[!UICONTROL All Audiences] 보기 또는 대상 라이브러리에서는 대상 세그먼트 그룹과 다른 저장된 대상을 포함하여 재사용 가능한 대상을 저장하고 관리할 수 있습니다. 여러 배치에 대한 타겟으로 대상을 사용할 수 있습니다. 각 대상자가 사용되는 배치 수는 배치 이름 옆에 표시됩니다.

모든 대상을 편집, 복제, 삭제, 내보내기 또는 공유할 수 있습니다.

### 세그먼트 보기

[!UICONTROL Segments] 보기에서 모든 사용자는 추가 사용자 지정 세그먼트를 만들 수 있습니다.

[!UICONTROL Segments] 보기에는 다음 세그먼트 유형도 나열됩니다.

* 사용자가 만든 모든 사용자 정의 세그먼트를 사용자가 사용할 수 있습니다.

  만든 사용자 지정 세그먼트에 대한 추적 태그를 보고 다른 사용자와 공유할 수 있습니다. 만든 사용자 지정 세그먼트를 편집하거나 삭제할 수도 있습니다.

  다른 사용자가 귀하와 공유한 사용자 지정 세그먼트를 편집하거나 공유할 수 없습니다.

* 있는 그대로 가져온, 사용자가 사용할 수 있는 모든 자사 세그먼트.

  공유된 자사 세그먼트를 편집하거나 공유할 수 없습니다. 추가 사용자와 자사 세그먼트를 공유해야 하는 경우 Adobe 계정 팀에 문의하십시오.

* 사용자가 사용할 수 있는 모든 사용자 지정 타사 세그먼트.

  사용자와 공유된 서드파티 세그먼트를 편집하거나 공유할 수 없습니다. 추가 사용자와 서드파티 세그먼트를 공유해야 하는 경우 Adobe 계정 팀에 문의하십시오.

### 소스 보기

[!UICONTROL Sources] 보기에서는 지정된 범용 ID 유형이 포함된 세그먼트로 변환할 지원되는 고객 데이터 플랫폼의 자사 세그먼트에 대한 소스를 구성할 수 있습니다. 소스 설정에는 연결을 설정하기 위해 고객 데이터 플랫폼에 제공할 자동 생성된 소스 키가 포함되어 있습니다.

지원되는 고객 데이터 플랫폼, 지원되는 범용 ID 유형 및 각 고객 데이터 플랫폼에 대한 연결을 설정하는 워크플로에 대한 자세한 내용은 &quot;[소스 정보](/help/dsp/audiences/sources/source-about.md)&quot;를 참조하십시오.

번역된 세그먼트는 재사용 가능한 대상 및 쿠키 없는 타깃팅을 위한 배치 설정에 포함할 수 있습니다.

>[!MORELIKETHIS]
>
>* [범용 ID 활성화 지원](/help/dsp/audiences/universal-ids.md)
>* [재사용 가능한 대상 만들기](reusable-audience-create.md)
>* [사용자 지정 세그먼트 만들기 및 구현](custom-segment-create.md)
>* [[!UICONTROL CCPA Opt-Out-of-Sale] 세그먼트 만들기 및 구현](ccpa-opt-out-segment-create.md)
>* [자사 대상 소스 정보](/help/dsp/audiences/sources/source-about.md)
>* [범용 ID 대상을 활성화하기 위한 대상 소스 관리](/help/dsp/audiences/sources/source-manage.md)
>* [인증된 세그먼트를 수동으로 가져오기 [!DNL LiveRamp]](/help/dsp/audiences/sources/source-import-liveramp-segments.md)
>* [사용 가능한 타사 데이터 공급자](third-party-data-providers.md)
>* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)
