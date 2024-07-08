---
title: 범용 ID 활성화 지원
description: 유니버설 ID 세그먼트 가져오기, 유니버설 ID를 추적하기 위한 맞춤 세그먼트 생성, 쿠키 없는 타겟팅을 위해 자사 세그먼트의 다른 사용자 식별자를 유니버설 ID로 전환 지원에 대해 알아보세요.
feature: DSP Audiences
exl-id: e238537b-217f-44bb-8a69-8adc83dbdfb9
source-git-commit: ea50b94ebc6d27fda9c0bd9f61da16750fa58f83
workflow-type: tm+mt
source-wordcount: '1403'
ht-degree: 0%

---

# 범용 ID 활성화 지원

<!-- Once we have CDP support for ID5 and can set up activation via sources, then maybe I can move this info into "About Sources" and "About Audiences." Or maybe make this the go-to page, removing info from those other pages? -->

*Beta 기능*

DSP는 DSP에서 지원하는 디지털 형식에서 쿠키가 없는 단일 디바이스(크로스 디바이스 아님) 타겟팅에 대해 사용자 기반의 범용 ID를 지원합니다.

* 대시보드를 [!DNL Connect] [!DNL LiveRamp] 사용하여 인증된 [[!DNL LiveRamp] [!DNL RampIDs]]을(를) 수동으로 DSP 직접 보낼 수 있습니다. &quot;[다음에서 인증된 세그먼트를 수동으로 가져오기&quot;를 [!DNL LiveRamp]](/help/dsp/audiences/sources/source-import-liveramp-segments.md) 참조하십시오.

* DSP는 고객 데이터 플랫폼 (CDP) 내에 구축 된 해시 된 이메일 ID로 구성된 자사 세그먼트를 수집하여 및 [!DNL Unified ID 2.0 (UID2.0)] ID로 [!DNL LiveRamp] [!DNL RampIDs] 전환 할 수 있습니다. 지원되는 고객 데이터 플랫폼, 지원되는 각 유니버설 ID 유형에 사용할 수 있는 기능 및 관련 워크플로우에 대한 자세한 내용은 &quot;자사 대상 소스](/help/dsp/audiences/sources/source-about.md) 정보&quot;[를 참조하십시오.

* 데스크탑 및 모바일 디바이스 기기의 광고에 노출되고 특정 웹페이지를 방문 하는 ID5 유니버설 ID와 연결된 사용자를 추적하는 사용자 지정 세그먼트를 만들 수 있습니다. ID5는 확률적 모델을 사용하여 다양한 사용자 신호 및 브라우저 신호에서 파생된 ID를 할당합니다. 자세한 내용은 &quot;[사용자 지정 세그먼트](/help/dsp/audiences/custom-segment-create.md) 만들기 및 구현&quot;을 참조하십시오.

* 일부 공급업체의 타사 세그먼트에는 쿠키 또는 디바이스 ID로 추적되는 사용자 외에도 유니버설 ID가 자동으로 포함될 수 있습니다. 예를 들어, 의 [!DNL Eyeota] 세그먼트는 자동으로 ID5 ID를 포함할 수 있고, 의 [!DNL Lotame] 세그먼트는 UID2.0 ID를 포함할 수 있습니다. 세그먼트 세부 정보에는 각 유형의 크기가 포함됩니다. 세그먼트 이름 옆에 명시된 각 세그먼트에 대한 일반 사용 요금이 적용됩니다. ID5 ID에 대해서는 추가 수수료가 부과되지 않습니다.

## 범용 ID 유형별 보고

* **사용자 지정 보고서:** 사용자 지정 보고서에서 유니버설 ID 유형별 비용, 노출 횟수, 클릭, 전환 및 빈도 데이터를 사용할 수 있습니다.

* **[!DNL Analytics]보고서:** 모든 필수 단계를 구현한 광고주 [[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md) 는 에서 유니버설 ID 유형별 조회연결 전환을 볼 수 있습니다 [!DNL Analytics].

  >[!IMPORTANT]
  >
  >올바른 전환 기여도 분석 위해 광고의 클릭연결 URL에 EF ID와 AMO ID](/help/integrations/analytics/ids.md)가 모두 [포함되어 있는지 확인하세요.

* **세그먼트 세부정보:** 모든 세그먼트 유형의 경우 세그먼트 세부정보에는 유니버설 ID 유형별 대상자 크기 및 쿠키 또는 디바이스 ID로 추적되는 디바이스 유형별 크기가 포함됩니다.

## 배치에서 유니버설 ID 대상자를 Target하는 방법

>[!NOTE]
>
>라이브 배치 상태에서는 타깃팅된 ID 유형을 변경할 수 없습니다. 필요한 경우 라이브 배치를 복제하고 새 배치에서 타깃팅된 ID 유형을 변경할 수 있습니다.

새 배치, 예약된 배치 또는 일시 중지된 배치 배치에서 다음을 수행합니다.

1. [!UICONTROL Geo-Targeting] 섹션에서 타겟 지역을 지정합니다. 각 범용 ID 파트너는 특정 지역에서만 사용자 타겟팅 수 있도록 허용하며, 설정에서 [!UICONTROL Targeting] 적합한 ID 유형만 사용할 수 있습니다.

1. 섹션에서 [!UICONTROL Audience Targeting] 다음을 수행합니다.

   1. [!UICONTROL Included Audiences] 설정에서 사용자 데이터가 유니버설 ID로 변환된 세그먼트를 선택합니다.

      원하는 경우 추가 세그먼트를 포함할 수 있습니다.

   1. 설정에서 다음을 수행합니다.[!UICONTROL Targeting]

      1. 타겟 유니버설 ID 유형을 선택합니다.

         이 설정에는 옵션 &quot;[!UICONTROL Legacy IDs]&quot; 및 &quot;[!UICONTROL Universal ID],&quot; 하위 옵션 &quot;[!UICONTROL ID5],&quot;[!UICONTROL RampID] 및 &quot;[!UICONTROL Unified ID2.0].&quot; 선택한 지리적 타겟에 따라 사용 가능한 하위 옵션이 결정됩니다.

         &quot;[!UICONTROL Legacy IDs]&quot;와 &quot;[!UICONTROL Universal ID]&quot;를 모두 선택할 수 있지만 배치 당 하나의 유니버설 ID 유형만 선택할 수 있습니다. 기존 ID와 유니버설 ID를 모두 선택하면 유니버설 ID에 입찰 우선권이 주어집니다.

      1. (필요한 경우) 범용 ID 사용에 대한 서비스 약관에 동의합니다.

         데이터를 새 ID 유형으로 전환하려면 DSP 계정의 사용자 서비스 약관에 동의해야 합니다. 약관은 ID 유형, 계정 당 한 번만 수락해야 합니다.

&quot;배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)&quot;[을 참조하십시오.

## 테스트 및 데이터 유효성 검사에 대한 우수 사례

Adobe Analytics 측정을 사용할 수 있는 기반 세그먼트 및 ID5 기반 세그먼트에 대해 [!DNL RampID]다음 우수 사례를 사용하십시오.

* 세그먼트 활성화한 후 약 24시간 후에 > [!UICONTROL All Audiences]내 [!UICONTROL Audiences] 세그먼트의 변환된 ID 수를 확인하십시오. ID 개수가 예상치 못한 경우 Adobe Systems 계정 팀에 문의하십시오.

  세그먼트 수가 어떻게 달라질 수 있는지에](#universal-ids-data-variances) 대한 자세한 내용은 &quot;[이메일 ID와 유니버설 ID 간의 데이터 차이 원인&quot;을 참조하십시오.

* 기존 패키지 및 배치를 변경하지 마세요. 그러나 유니버설 ID를 테스트하기 위한 증분 예산이 없는 경우 원래 예산을 줄여 테스트 비용을 충당하세요.

* 원본 패키지 및 게재위치를 복사하고, 테스트 크기에 따라 예산을 조정하고, 기반 세그먼트(인증된 사용자의 경우) 또는 ID5 기반 세그먼트(인증되지 않은 사용자의 경우)를 사용하도록 [!DNL RampID]잠재고객을 변경하고, 새 패키지 및 게재위치가 전체 예산을 지출하는지 확인합니다.

   * 유니버설 ID 기반 세그먼트의 실적을 게재위치 타겟팅 기타 대상자 식별자(예: 쿠키 또는 모바일 광고 ID)의 실적과 비교하려면 별도의 유니버설 ID 기반 배치 및 기존 ID 기반 배치 사용하여 캠페인을 만듭니다.

     전체 리타게팅 테스트 테스트의 경우 인증된 사용자의 경우 RampID를 모두 타겟 지정하고 인증되지 않은 사용자의 경우 ID5를 모두 타게팅합니다.

     최고의 성능을 얻는 것이 주요 비교가 되어서는 안 됩니다. 대신 확장이 잘 되는 ID를 확인하여 나중에 최적화 및 예산 할당에 정보를 제공할 수 있습니다. 장기적인 목표는 쿠키를 더 이상 사용하지 않을 때 손실되는 노출 횟수와 사이트 트래픽 수를 보충하는 것입니다.

   * 총 도달브라우저 비교하려면 동일한 배치에서 유니버설 ID 기반 세그먼트와 기존 ID 기반 세그먼트를 타겟하십시오. 캠페인 예산을 분할할 필요가 없다는 점을 제외하고는 이전 사용 사례와 동일한 캠페인 설정을 사용합니다.

     입찰 우선권은 유니버설 ID에 부여되지만, 유니버설 ID를 사용할 수 없는 경우 기존 ID가 입찰을 받습니다. 다양한 브라우저(크롬, 사파리, 모질라 포함)에서 도달범위를 비교하세요.

     >[!NOTE]
     >
     >최대 게재빈도 설정은 개별 ID에 적용됩니다. 사용자에 여러 ID 유형이 있는 경우 해당 사용자에 예상보다 많이 도달할 수 있습니다.

* 인증된 대상자 세그먼트의 도달범위는 쿠키 기반 세그먼트의 도달범위보다 당연히 작으며, 추가 타겟팅 옵션을 사용하면 도달범위가 더 줄어듭니다. 세분화된 타겟팅 사용, 특히 여러 대상을 AND 문과 결합하는 경우 주의해야 합니다.

## 이메일 ID와 유니버설 ID 간의 데이터 차이의 원인 {#universal-ids-data-variances}

* ID5 ID로 변환된 해시된 이메일 ID:

  확률적 모델의 오차 변량 범위는 +/- 5%입니다. 즉, 대상자 수를 5% 정도 과대 평가하거나 과소 평가할 수 있습니다.

* 다음으로 변환 [!DNL RampIDs]되는 해시된 이메일 ID:

   * 여러 프로필에서 동일한 이메일 ID를 사용하는 경우 DSP 세그먼트 수는 고객 데이터 플랫폼 내의 프로필 수보다 작을 수 있습니다. 예를 들어 Adobe Photoshop에서 단일 이메일 ID를 사용하여 회사 계정과 개인 계정을 만들 수 있습니다. 그러나 두 프로필이 동일한 사람에게 속하는 경우 프로필은 하나의 이메일 ID에 매핑되고 그에 따라 하나의 [!DNL RampID].

   * A [!DNL RampID] 를 새 값으로 업그레이드할 수 있습니다. [!DNL LiveRamp] 이메일 ID를 인식하지 못하거나 데이터베이스의 기존 [!DNL RampID] 이메일 ID에 매핑할 수 없는 경우 이메일 ID에 새 [!DNL RampID] 이메일 ID를 할당합니다. 나중에 이메일 ID를 다른 [!DNL RampID] 이메일 ID에 매핑하거나 동일한 이메일 ID에 대한 자세한 정보를 수집할 수 있게 되면 을 [!DNL RampID] 새 값으로 업그레이드합니다. [!DNL LiveRamp] 이 작업을 &quot;파생&quot; [!DNL RampID] 에서 &quot;유지 관리&quot; [!DNL RampID]로 업그레이드하는 것을 나타냅니다. 그러나 DSP는 파생된 것과 유지 관리되는 [!DNL RampIDs] 것 간에 매핑을 가져오지 않으므로 DSP 세그먼트에서 이전 버전의 RampID를 제거할 수 없습니다. 이 경우 세그먼트 수는 프로필 수보다 많을 수 있습니다.

     예: 사용자 웹 사이트에 로그인 [!DNL Adobe] 하여 Photoshop 페이지 방문합니다. 이메일 ID에 대한 기존 정보가 없는 경우 [!DNL LiveRamp] 파생 [!DNL RampID]된 (예: D123)을 할당합니다. 15일 후 사용자 동일한 페이지 방문하지만 [!DNL LiveRamp] 해당 15일 동안 를 업그레이드 [!DNL RampID] 하고 M123에 다시 할당 [!DNL RampID] 했습니다. 고객 데이터 플랫폼의 세그먼트 &quot;Photoshop Enthusiast&quot;에는 사용자에 대한 이메일 ID가 하나만 있지만 DSP 세그먼트에는 D123 및 M123이라는 두 개의 RampID가 있습니다.

## 문제 해결

사용자 수가 표시되지 않거나 대상자 크기가 적은 경우 다음을 확인합니다.

* 또는 [!DNL Google Campaign Manager 360] 광고를 사용하는 [!DNL Flashtalking] 경우 광고의 클릭연결 URL에 올바른 매크로가 추가되었는지 확인하세요. 광고](/help/integrations/analytics/macros-flashtalking.md) 및 [[!DNL Google Campaign Manager 360] 광고](/help/integrations/analytics/macros-google-campaign-manager.md)에 대한 [[!DNL Flashtalking] 매크로를 참조하십시오.

* 사이트 내 이벤트 및 광고 노출과 일치하도록 올바른 유니버설 ID 파트너 관련 코드가 웹사이트에 구현되어 있는지 확인하세요. 필요에 따라 귀하 또는 [!DNL ID5] 담당자와 협력하십시오[!DNL LiveRamp].

* (및 [!DNL UID 2.0] ID의 경우[!DNL RampIDs]) DSP 데이터 소스가 올바르게](/help/dsp/audiences/sources/source-manage.md#source-settings) 구성되어 있고 생성된 대상자 세그먼트에 대해 사용자 카운트가 채워졌는지 확인하십시오[.

* 도달 범위가 예상보다 적은 경우 대상 세그먼트 로직이 너무 세분화되어 있지 않은지 확인하세요.

* 캠페인, 패키지 및 배치 설정이 올바른지 확인합니다.<!-- wording-->

문제를 해결할 수 없는 경우에는 Adobe Systems 계정 팀에 문의하십시오.

>[!MORELIKETHIS]
>
>* [자사 대상 소스 정보](/help/dsp/audiences/sources/source-about.md)
>* [대상 소스를 관리하여 유니버설 ID Audiences 활성화](/help/dsp/audiences/sources/source-manage.md)
>* [사용자 지정 세그먼트 만들기 및 구현](/help/dsp/audiences/custom-segment-create.md)
>* [인증된 세그먼트를 다음에서 수동으로 가져오기 [!DNL LiveRamp]](/help/dsp/audiences/sources/source-import-liveramp-segments.md)
>* [고객 관리 정보](/help/dsp/audiences/audience-about.md)
>* [배치 설정](/help/dsp/campaign-management/placements/placement-settings.md)
