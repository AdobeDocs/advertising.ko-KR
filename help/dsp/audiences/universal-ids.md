---
title: 범용 ID 활성화 지원
description: 범용 ID 세그먼트를 가져오고, 사용자 지정 세그먼트를 만들어 범용 ID를 추적하고, 자사 세그먼트의 다른 사용자 식별자를 쿠키 없는 타깃팅을 위해 범용 ID로 변환하는 지원에 대해 알아봅니다.
feature: DSP Audiences
exl-id: e238537b-217f-44bb-8a69-8adc83dbdfb9
source-git-commit: 202f4ae8e6633672b7af12937f0b35da5052f7fc
workflow-type: tm+mt
source-wordcount: '1500'
ht-degree: 0%

---

# 범용 ID 활성화 지원

<!-- Once we have CDP support for ID5 and can set up activation via sources, then maybe I can move this info into "About Sources" and "About Audiences." Or maybe make this the go-to page, removing info from those other pages? -->

*Beta 기능*

DSP은 DSP에서 지원하는 디지털 형식 간에 쿠키 없는 단일 장치(크로스 장치가 아님) 타깃팅에 대한 사람 기반의 범용 ID를 지원합니다.

* [!DNL LiveRamp] [!DNL Connect] 대시보드를 사용하여 인증된 [[!DNL LiveRamp] [!DNL RampIDs]]을(를) 수동으로 DSP에 직접 보낼 수 있습니다. &quot;[인증된 세그먼트를 수동으로 가져오기 [!DNL LiveRamp]](/help/dsp/audiences/sources/source-import-liveramp-segments.md)&quot;를 참조하십시오.

* DSP은 고객 데이터 플랫폼(CDP) 내에 빌드된 해시된 이메일 ID로 구성된 자사 세그먼트를 수집하여 [!DNL LiveRamp] [!DNL RampIDs] 및 [!DNL Unified ID 2.0 (UID2.0)] ID로 변환할 수 있습니다. 지원되는 고객 데이터 플랫폼, 지원되는 각 범용 ID 유형에 사용할 수 있는 기능 및 관련 워크플로에 대한 자세한 내용은 &quot;[자사 대상 소스 정보](/help/dsp/audiences/sources/source-about.md)&quot;를 참조하십시오.

* 데스크탑 및 모바일 디바이스에서 광고에 노출되고 특정 웹 페이지를 방문하는 ID5 범용 ID와 연결된 사용자를 추적하는 사용자 지정 세그먼트를 만들 수 있습니다. ID5는 확률론적 모델을 사용하여 다양한 사용자 신호 및 브라우저 신호로부터 파생된 ID를 할당합니다. 지침은 &quot;[사용자 지정 세그먼트 만들기 및 구현](/help/dsp/audiences/custom-segment-create.md)&quot;을 참조하세요.

* 일부 공급업체의 서드파티 세그먼트에는 쿠키 또는 디바이스 ID로 추적되는 사용자 외에도 범용 ID가 자동으로 포함될 수 있습니다. 예를 들어 [!DNL Eyeota]의 세그먼트에는 ID5 ID가 자동으로 포함될 수 있으며 [!DNL Lotame]의 세그먼트에는 UID2.0 ID가 포함될 수 있습니다. 세그먼트 세부 정보에는 각 유형의 크기가 포함됩니다. 세그먼트 이름 옆에 표시되는 각 세그먼트에 대한 일반적인 사용 요금이 적용됩니다. ID5 ID에 대해서는 추가 요금이 부과되지 않습니다.

## 범용 ID 유형별 보고

* **사용자 지정 보고서:** 유니버설 ID 유형별 비용, 노출, 클릭, 전환 및 빈도 데이터를 사용자 지정 보고서에서 사용할 수 있습니다.

* **[!DNL Analytics]보고서:** 필요한 모든 단계를 구현한 [[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md)의 광고주가 [!DNL Analytics]에서 유니버설 ID 유형별 보기 통과 전환을 볼 수 있습니다.

  >[!IMPORTANT]
  >
  >적절한 전환 속성을 사용하려면 광고에 대한 클릭스루 URL에 [EF ID와 AMO ID](/help/integrations/analytics/ids.md)가 모두 포함되어 있는지 확인하십시오.

* **세그먼트 세부 정보:** 모든 세그먼트 형식의 경우 세그먼트 세부 정보에는 범용 ID 형식별 대상 크기와 쿠키 또는 장치 ID로 추적되는 장치 형식별 대상 크기가 포함됩니다.

## 배치에서 범용 ID 대상을 타깃팅하는 방법

>[!NOTE]
>
>라이브 배치에서 타겟팅된 ID 유형을 변경할 수 없습니다. 필요한 경우 라이브 배치를 복제하고 새 배치에서 타겟팅된 ID 유형을 변경할 수 있습니다.

새 배치, 예약된 배치 또는 일시 중지된 배치에서 다음을 수행합니다.

1. [!UICONTROL Geo-Targeting] 섹션에서 타겟팅할 지리적 영역을 지정합니다. 각 범용 ID 파트너는 특정 지리적 영역에서만 사용자 타깃팅을 허용하며 [!UICONTROL Targeting] 설정에서 적격한 ID 유형만 사용할 수 있습니다.

1. [!UICONTROL Audience Targeting] 섹션에서 다음을 수행합니다.

   1. [!UICONTROL Included Audiences] 설정에서 사용자 데이터가 범용 ID로 변환된 세그먼트를 선택합니다.

      원할 경우 추가 세그먼트를 포함할 수 있습니다.

   1. [!UICONTROL Targeting] 설정에서:

      1. 타깃팅할 범용 ID 유형을 선택합니다.

         설정에는 하위 옵션 &quot;[!UICONTROL ID5]&quot;, &quot;[!UICONTROL RampID]&quot; 및 &quot;[!UICONTROL Unified ID2.0]&quot;을(를) 포함할 수 있는 옵션 &quot;[!UICONTROL Legacy IDs]&quot; 및 &quot;[!UICONTROL Universal ID]&quot;이(가) 포함되어 있습니다. 선택한 지리적 타겟에 따라 사용 가능한 하위 옵션이 결정됩니다.

         &quot;[!UICONTROL Legacy IDs]&quot;과(와) &quot;[!UICONTROL Universal ID]&quot;을(를) 모두 선택할 수 있지만 배치당 하나의 유니버설 ID 유형만 선택할 수 있습니다. 기존 ID와 범용 ID를 모두 선택하면 범용 ID에 입찰 기본 설정이 지정됩니다.

      1. (필요한 경우) 범용 ID 사용에 대한 서비스 약관에 동의합니다.

         데이터를 새 ID 유형으로 변환하려면 먼저 DSP 계정의 사용자가 서비스 약관에 동의해야 합니다. 약관은 ID 유형, 계정당 한 번만 수락해야 합니다.

&quot;[배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)&quot;을 참조하십시오.

## 테스트 및 데이터 유효성 검사에 대한 우수 사례

Adobe Analytics 측정을 사용할 수 있는 [!DNL RampID] 기반 세그먼트 및 ID5 기반 세그먼트에 대해 다음 모범 사례를 사용하십시오.

* 세그먼트를 활성화한 후 약 24시간이 지나면 [!UICONTROL Audiences] > [!UICONTROL All Audiences] 내에서 변환된 세그먼트 ID 수를 확인합니다. 예기치 않은 ID 카운트인 경우 Adobe 계정 팀에 문의하십시오.

  세그먼트 수가 어떻게 달라질 수 있는지에 대한 자세한 내용은 &quot;[전자 메일 ID와 유니버설 ID 간의 데이터 분산](#universal-ids-data-variances)&quot;을 참조하십시오.

* 기존 패키지 및 배치를 변경하지 마십시오. 그러나 범용 ID를 테스트할 증분 예산이 없는 경우 원래 예산을 줄여서 테스트 자금을 조달합니다.

* 원본 패키지 및 배치를 복사하고, 테스트 크기에 따라 예산을 조정하고, [!DNL RampID] 기반 세그먼트(인증된 사용자의 경우) 또는 ID5 기반 세그먼트(인증되지 않은 사용자의 경우)를 사용하도록 대상을 변경하고, 새 패키지 및 배치가 전체 예산을 사용하는지 확인하십시오.

   * 범용 ID 기반 세그먼트의 성능을 쿠키 또는 모바일 광고 ID와 같은 다른 대상 식별자를 타겟팅하는 배치 성능과 비교하려면 별도의 범용 ID 기반 배치와 레거시 ID 기반 배치로 캠페인을 만드십시오.

     전체 재타겟팅 테스트의 경우 인증된 사용자의 경우 RampID를, 인증되지 않은 사용자의 경우 ID5를 모두 타겟팅하십시오.

     최고의 성능을 얻는 것이 기본 비교가 되어서는 안 됩니다. 대신, 어떤 ID의 크기가 잘 조절되는지 결정하십시오. 그러면 나중에 최적화 및 예산 할당에 영향을 줄 수 있습니다. 장기적인 목표는 쿠키가 더 이상 사용되지 않을 때 손실된 노출 횟수 및 사이트 트래픽을 보전하는 것입니다.

   * 총 브라우저 도달량을 비교하려면 동일한 배치에서 범용 ID 기반 세그먼트 및 레거시 ID 기반 세그먼트를 타겟팅하십시오. 캠페인 예산을 분할할 필요가 없다는 점을 제외하고 이전 사용 사례와 동일한 캠페인 설정을 사용합니다.

     입찰 기본 설정은 범용 ID에 주어지지만 레거시 ID는 범용 ID를 사용할 수 없는 경우 입찰을 받습니다. 서로 다른 브라우저(Chrome, Safari 및 Mozilla 포함)에서 도달 범위를 비교해야 합니다.

     >[!NOTE]
     >
     >빈도 제한은 개별 ID에 적용됩니다. 사용자에게 여러 ID 유형이 있는 경우 예상한 것보다 더 많은 해당 사용자에게 도달할 수 있습니다.

* 인증된 대상 세그먼트에 대한 도달 거리는 쿠키 기반 세그먼트에 대한 도달 거리보다 자연히 더 작으며 추가 타겟팅 옵션을 사용하면 도달 거리가 더 줄어든다는 것을 기억하십시오. 특히 AND 문으로 여러 대상을 연결하여 세분화된 타깃팅을 사용하는 것은 신중해야 합니다.

## 이메일 ID와 범용 ID 간의 데이터 분산 {#universal-ids-data-variances}

### 허용 가능한 차이 수준

범용 ID에 대한 해시된 이메일 주소의 번역률은 90%보다 커야 합니다. 특히 [!DNL RampIDs]의 번역률은 모든 해시된 이메일 주소가 고유한 경우 95%여야 합니다. 예를 들어 고객 데이터 플랫폼에서 100개의 해시된 이메일 주소를 전송하는 경우 최소 95개의 [!DNL RampIDs] 또는 90개 이상의 다른 유형의 범용 ID로 변환되어야 합니다. 낮은 번역률은 문제를 나타낼 수 있습니다. 가능한 설명은 &quot;[분산의 원인] (#universal-ids-data-variances-causes&quot;을(를) 참조하십시오.

[!DNL RampIDs]의 경우 번역 비율이 70%보다 낮은 경우 Adobe 계정 팀에 연락하여 추가 조사를 받으십시오.

### 분산 원인 {#universal-ids-data-variances-causes}

* 모든 세그먼트:

  세그먼트-디바이스 카운트는 오차 분산이 +/- 5%인 확률론적 모델을 사용합니다. 이는 관객 수를 5% 가량 과대 또는 과소 평가할 수 있다는 것을 의미한다.

* [!DNL RampIDs] (으)로 번역된 해시된 이메일 ID:

   * 여러 프로필에서 동일한 이메일 ID를 사용하는 경우 DSP 세그먼트 수가 고객 데이터 플랫폼 내 프로필 수보다 작을 수 있습니다. 예를 들어 Adobe Photoshop에서 단일 이메일 ID를 사용하여 회사 계정과 개인 계정을 만들 수 있습니다. 그러나 두 프로필이 모두 같은 사용자에 속하는 경우 프로필은 하나의 이메일 ID에 매핑되고 하나의 [!DNL RampID]에 대응됩니다.

   * [!DNL RampID]을(를) 새 값으로 업그레이드할 수 있습니다. [!DNL LiveRamp]이(가) 전자 메일 ID를 인식하지 못하거나 데이터베이스의 기존 [!DNL RampID]에 매핑할 수 없는 경우 전자 메일 ID에 새 [!DNL RampID]을(를) 할당합니다. 나중에 전자 메일 ID를 다른 [!DNL RampID]에 매핑하거나 동일한 전자 메일 ID에 대한 자세한 정보를 수집할 수 있으면 [!DNL RampID]을(를) 새 값으로 업그레이드합니다. [!DNL LiveRamp]은(는) 이 작업을 &quot;파생된&quot; [!DNL RampID]에서 &quot;유지 관리되는&quot; [!DNL RampID] (으)로 업그레이드한 것으로 참조합니다. 그러나 DSP은 파생된 [!DNL RampIDs]과(와) 유지 관리되는  간의 매핑을 가져오지 않으므로 DSP 세그먼트에서 이전 버전의 RampID를 제거할 수 없습니다. 이 경우 세그먼트 수가 프로필 수보다 많을 수 있습니다.

     예: 사용자가 [!DNL Adobe] 웹 사이트에 로그인하고 Photoshop 페이지를 방문합니다. [!DNL LiveRamp]에게 전자 메일 ID에 대한 기존 정보가 없는 경우 파생 [!DNL RampID] (예: D123)을(를) 할당합니다. 15일 후 사용자가 같은 페이지를 방문하지만 [!DNL LiveRamp]이(가) 15일 동안 [!DNL RampID]을(를) 업그레이드하고 [!DNL RampID]을(를) M123으로 다시 할당했습니다. 고객 데이터 플랫폼의 세그먼트 &quot;Photoshop Manist&quot;에는 사용자에 대한 이메일 ID가 하나만 있지만 DSP 세그먼트에는 D123과 M123이라는 두 개의 RampID가 있습니다.

## 문제 해결

사용자 수가 표시되지 않거나 대상 크기가 낮은 경우 다음을 확인하십시오.

* [!DNL Flashtalking] 또는 [!DNL Google Campaign Manager 360] 광고를 사용하는 경우 광고의 클릭스루 URL에 올바른 매크로가 추가되어 있는지 확인하십시오. [[!DNL Flashtalking] ads](/help/integrations/analytics/macros-flashtalking.md) 및 [[!DNL Google Campaign Manager 360] ads](/help/integrations/analytics/macros-google-campaign-manager.md)에 대한 매크로를 참조하세요.

* 온사이트 이벤트 및 광고 노출에 맞게 웹 사이트에 올바른 범용 ID 파트너별 코드가 구현되었는지 확인하십시오. 필요에 따라 [!DNL LiveRamp] 또는 [!DNL ID5] 담당자와 협력합니다.

* ([!DNL RampIDs] 및 [!DNL UID 2.0] ID의 경우) [DSP 데이터 소스가 올바르게 구성되었는지](/help/dsp/audiences/sources/source-manage.md#source-settings), 사용자 수가 생성된 대상 세그먼트에 대해 채워졌는지 확인하십시오.

* 도달 범위가 예상보다 짧은 경우 대상 세그먼트 로직이 너무 세분화되지 않았는지 확인하십시오.

* 캠페인, 패키지 및 배치 설정이 올바른지 확인하세요.<!-- wording-->

문제를 해결할 수 없는 경우 Adobe 계정 팀에 문의하십시오.

>[!MORELIKETHIS]
>
>* [자사 대상 소스 정보](/help/dsp/audiences/sources/source-about.md)
>* [범용 ID 대상을 활성화하기 위한 대상 소스 관리](/help/dsp/audiences/sources/source-manage.md)
>* [사용자 지정 세그먼트 만들기 및 구현](/help/dsp/audiences/custom-segment-create.md)
>* [인증된 세그먼트를 수동으로 가져오기 [!DNL LiveRamp]](/help/dsp/audiences/sources/source-import-liveramp-segments.md)
>* [대상자 관리 정보](/help/dsp/audiences/audience-about.md)
>* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)
