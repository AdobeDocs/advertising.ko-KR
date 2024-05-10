---
title: 범용 ID 활성화 지원
description: 범용 ID 세그먼트를 가져오고, 사용자 지정 세그먼트를 만들어 범용 ID를 추적하고, 자사 세그먼트의 다른 사용자 식별자를 쿠키 없는 타깃팅을 위해 범용 ID로 변환하는 지원에 대해 알아봅니다.
feature: DSP Audiences
source-git-commit: e517dd5f5fa283ff8a2f57728612937148889732
workflow-type: tm+mt
source-wordcount: '1160'
ht-degree: 0%

---

# 범용 ID 활성화 지원

<!-- Once we have CDP support for ID5 and can set up activation via sources, then maybe I can move this info into "About Sources" and "About Audiences." Or maybe make this the go-to page, removing info from those other pages? -->

*Beta 기능*

DSP은 DSP에서 지원하는 디지털 형식 간에 쿠키 없는 단일 장치(크로스 장치가 아님) 타깃팅에 대한 사람 기반의 범용 ID를 지원합니다.

* 인증된 [[!DNL LiveRamp] [!DNL RampIDs]] 를 사용하여 DSP으로 직접 이동 [!DNL LiveRamp] [!DNL Connect] 대시보드입니다. 를 참조하십시오.[에서 인증된 세그먼트 수동으로 가져오기 [!DNL LiveRamp]](/help/dsp/audiences/sources/source-import-liveramp-segments.md).&quot;

* DSP은 고객 데이터 플랫폼(CDP) 내에 구축된 해시된 이메일 ID로 구성된 자사 세그먼트를 수집하여 다음으로 변환할 수 있습니다. [!DNL LiveRamp] [!DNL RampIDs] 및 [!DNL Unified ID 2.0 (UID2.0)] ID 지원되는 고객 데이터 플랫폼, 지원되는 각 범용 ID 유형에 사용할 수 있는 기능 및 관련 워크플로우에 대한 자세한 내용은 &quot;[자사 대상 소스 정보](/help/dsp/audiences/sources/source-about.md).&quot;

* 데스크탑 및 모바일 디바이스에서 광고에 노출되고 특정 웹 페이지를 방문하는 ID5 범용 ID와 연결된 사용자를 추적하는 사용자 지정 세그먼트를 만들 수 있습니다. ID5는 확률론적 모델을 사용하여 다양한 사용자 신호 및 브라우저 신호로부터 파생된 ID를 할당합니다. 자세한 내용은 &quot;[사용자 지정 세그먼트 만들기 및 구현](/help/dsp/audiences/custom-segment-create.md).&quot;

* 의 타사 세그먼트 [!DNL Eyeota] 및 일부 다른 공급업체는 쿠키 또는 장치 ID로 추적되는 사용자 외에도 ID5 ID를 자동으로 포함할 수 있습니다. 세그먼트 세부 정보에는 각 유형의 크기가 포함됩니다. 세그먼트 이름 옆에 표시되는 각 세그먼트에 대한 일반적인 사용 요금이 적용됩니다. ID5 ID에 대해서는 추가 요금이 부과되지 않습니다.

<!-- Make above statement more generic when other ID types are available 

* Some third-party segment vendors have started including universal IDs in their segments, and you can use them in saved audiences and as placement targets without any extra steps or extra fees.
-->

## 범용 ID 유형별 보고

* **사용자 지정 보고서:** 범용 ID 유형별 비용, 노출, 클릭, 전환 및 빈도 데이터는 사용자 지정 보고서에서 사용할 수 있습니다.

* **[!DNL Analytics]보고서:** 를 사용하는 광고주 [[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md) 필요한 모든 단계를 구현한 사용자는에서 범용 ID 유형별로 뷰스루 전환을 볼 수 있습니다. [!DNL Analytics].

* **세그먼트 세부 정보:** 모든 세그먼트 유형의 경우 세그먼트 세부 사항에는 범용 ID 유형별 및 쿠키 또는 장치 ID로 추적되는 장치 유형별 대상 크기가 포함됩니다.

## 배치에서 범용 ID 대상을 타깃팅하는 방법

>[!NOTE]
>
>라이브 배치에서 타겟팅된 ID 유형을 변경할 수 없습니다. 필요한 경우 라이브 배치를 복제하고 새 배치에서 타겟팅된 ID 유형을 변경할 수 있습니다.

새 배치, 예약된 배치 또는 일시 중지된 배치에서 다음을 수행합니다.

* 다음에서 [!UICONTROL Geo-Targeting] 섹션에서 타겟팅할 지리적 영역을 지정합니다. 각 범용 ID 파트너는 특정 지리적 영역에서만 사용자 타겟팅을 허용하며 의 적격 ID 유형만 사용할 수 있습니다. [!UICONTROL Targeting] 설정.

* 다음에서 [!UICONTROL Audience Targeting] 섹션에서 다음을 수행합니다.

   * 다음에서 [!UICONTROL Included Audiences] 을(를) 설정하고 사용자 데이터가 범용 ID로 변환된 세그먼트를 선택합니다.

     원할 경우 추가 세그먼트를 포함할 수 있습니다.

   * 다음에서 [!UICONTROL Targeting] 을(를) 설정하고, 타깃팅할 범용 ID 유형을 선택합니다.

     이 설정에는 옵션 이 포함됩니다.[!UICONTROL Legacy IDs]&quot; 및 &quot;[!UICONTROL Universal ID],&quot; 하위 옵션을 포함할 수 있음 &quot;[!UICONTROL ID5],&quot; &quot;[!UICONTROL RampID]및 &quot;[!UICONTROL Unified ID2.0].&quot; 실제 하위 옵션은 선택한 지리적 대상에 의해 결정됩니다.

     둘 다 선택할 수 있습니다.[!UICONTROL Legacy IDs]&quot; 및 &quot;[!UICONTROL Universal ID],&quot;이지만 배치당 하나의 범용 ID 유형만 선택할 수 있습니다. 기존 ID와 범용 ID를 모두 선택하면 범용 ID에 입찰 기본 설정이 지정됩니다.

를 참조하십시오.[배치 설정](/help/dsp/campaign-management/placements/placement-settings.md).&quot;

## 테스트 및 데이터 유효성 검사에 대한 우수 사례

다음 모범 사례 사용 [!DNL RampID]Adobe Analytics 측정을 사용할 수 있는 기반 세그먼트 및 ID5 기반 세그먼트.

* 세그먼트를 활성화한 후 약 24시간 후에 변환된 다음 내 세그먼트의 ID 수를 확인합니다. [!UICONTROL Audiences] > [!UICONTROL All Audiences]. 예기치 않은 ID 카운트인 경우 Adobe 계정 팀에 문의하십시오.

  를 참조하십시오.[이메일 ID와 범용 ID 간의 데이터 분산 원인](#universal-ids-data-variances)세그먼트 카운트가 달라질 수 있는 방법에 대한 자세한 내용은 &quot;을 참조하십시오.

* 기존 패키지 및 배치를 변경하지 마십시오. 그러나 범용 ID를 테스트할 증분 예산이 없는 경우 원래 예산을 줄여서 테스트 자금을 조달합니다.

* 원본 패키지 및 배치를 복사하고 테스트 크기에 따라 예산을 조정하며 사용할 대상을 변경합니다 [!DNL RampID]- 기반 세그먼트(인증된 사용자용) 또는 ID5 기반 세그먼트(인증되지 않은 사용자용)를 실행하고, 새 패키지 및 배치가 전체 예산을 사용하는지 확인합니다.

   * 범용 ID 기반 세그먼트의 성능을 쿠키 또는 모바일 광고 ID와 같은 다른 대상 식별자를 타겟팅하는 배치 성능과 비교하려면 별도의 범용 ID 기반 배치와 레거시 ID 기반 배치로 캠페인을 만드십시오.

     최고의 성능을 얻는 것이 기본 비교가 되어서는 안 됩니다. 대신, 어떤 ID의 크기가 잘 조절되는지 결정하십시오. 그러면 나중에 최적화 및 예산 할당에 영향을 줄 수 있습니다. 장기적인 목표는 쿠키가 더 이상 사용되지 않을 때 손실된 노출 횟수 및 사이트 트래픽을 보전하는 것입니다.

   * 총 브라우저 도달량을 비교하려면 동일한 배치에서 범용 ID 기반 세그먼트 및 레거시 ID 기반 세그먼트를 타겟팅하십시오. 캠페인 예산을 분할할 필요가 없다는 점을 제외하고 이전 사용 사례와 동일한 캠페인 설정을 사용합니다.

     입찰 기본 설정은 범용 ID에 주어지지만 레거시 ID는 범용 ID를 사용할 수 없는 경우 입찰을 받습니다. 서로 다른 브라우저(Chrome, Safari 및 Mozilla 포함)에서 도달 범위를 비교해야 합니다.

     >[!NOTE]
     >
     >빈도 제한은 개별 ID에 적용됩니다. 사용자에게 여러 ID 유형이 있는 경우 예상했던 것보다 해당 사용자에게 더 많이 도달했을 수 있습니다.

* 인증된 대상 세그먼트에 대한 도달 거리는 쿠키 기반 세그먼트에 대한 도달 거리보다 자연히 더 작으며 추가 타겟팅 옵션을 사용하면 도달 거리가 더 줄어든다는 것을 기억하십시오. 특히 AND 문으로 여러 대상을 연결하여 세분화된 타깃팅을 사용하는 것은 신중해야 합니다.

## 이메일 ID와 범용 ID 간의 데이터 분산 원인 {#universal-ids-data-variances}

해시된 이메일 ID가 로 번역되는 이유는 두 가지가 있습니다 [!DNL RampIDs]:

* 여러 프로필에서 동일한 이메일 ID를 사용하는 경우 DSP 세그먼트 수가 고객 데이터 플랫폼 내 프로필 수보다 작을 수 있습니다. 예를 들어 Adobe Photoshop에서 단일 이메일 ID를 사용하여 회사 계정과 개인 계정을 만들 수 있습니다. 하지만 두 프로필이 모두 동일한 세그먼트에 속하는 경우 프로필은 하나의 이메일 ID에 매핑되고 이에 따라 하나의 이메일 ID에 매핑됩니다 [!DNL RampID].

* A [!DNL RampID] 를 새 값으로 업그레이드할 수 있습니다. If [!DNL LiveRamp] 은(는) 이메일 ID를 인식하지 못하거나 기존 ID에 매핑할 수 없습니다 [!DNL RampID] 데이터베이스에서 새 [!DNL RampID] 이메일 ID로. 나중에 이메일 ID를 다른 ID에 매핑할 수 있을 때 [!DNL RampID] 또는 동일한 이메일 ID에 대한 자세한 정보를 수집할 수 있으며 [!DNL RampID] 을 새 값으로 바꿉니다. [!DNL LiveRamp] 파생된 항목에서 업그레이드하는 것으로 이 작업을 참조합니다. [!DNL RampID] &quot;유지 관리됨&quot;으로 [!DNL RampID]. 그러나 DSP은 파생된 와 유지 관리되는 간에 매핑을 가져오지 않습니다 [!DNL RampIDs] 따라서 DSP 세그먼트에서 이전 버전의 RampID를 제거할 수 없습니다. 이 경우 세그먼트 수가 프로필 수보다 많을 수 있습니다.

  예: 사용자가에 로그인합니다 [!DNL Adobe] 웹 사이트를 방문하여 Photoshop 페이지를 방문하십시오. If [!DNL LiveRamp] 은(는) 이메일 ID에 대한 기존 정보가 없는 경우 파생된 ID를 할당합니다 [!DNL RampID]예, D123입니다. 15일 후 사용자는 동일한 페이지를 방문하지만 [!DNL LiveRamp] 이(가) 다음을 업그레이드했습니다. [!DNL RampID] 15일 동안 이(가) [!DNL RampID] M123으로 고객 데이터 플랫폼의 세그먼트 &quot;Photoshop Manist&quot;에는 사용자에 대한 이메일 ID가 하나만 있지만 DSP 세그먼트에는 D123과 M123이라는 두 개의 RampID가 있습니다.

>[!MORELIKETHIS]
>
>* [범용 ID 대상을 활성화하는 대상 소스 만들기](/help/dsp/audiences/sources/source-create.md)
>* [다음에서 사용자 ID 변환 [!DNL Adobe Real-Time CDP] 범용 ID로](/help/dsp/audiences/sources/source-adobe-rtcdp.md)
>* [다음에서 사용자 ID 변환 [!DNL Tealium] 범용 ID로](/help/dsp/audiences/sources/source-tealium.md)
>* [사용자 지정 세그먼트 만들기 및 구현](/help/dsp/audiences/custom-segment-create.md)
>* [에서 인증된 세그먼트 수동으로 가져오기 [!DNL LiveRamp]](/help/dsp/audiences/sources/source-import-liveramp-segments.md)
>* [대상자 관리 기본 정보](/help/dsp/audiences/audience-about.md)
>* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)
