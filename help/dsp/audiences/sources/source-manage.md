---
title: 범용 ID 대상을 활성화하기 위한 대상 소스 관리
description: 소스를 만들고 관리하여 고객 데이터 플랫폼에서 대상을 가져와 범용 ID가 포함된 세그먼트로 변환하는 방법에 대해 알아봅니다.
feature: DSP Audiences
exl-id: 728130d7-d19c-4d5d-9bca-695f8c17f89b
source-git-commit: e9ce180e302f619c85a3d6db813c83903e437d04
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# 범용 ID 대상을 활성화하기 위한 대상 소스 관리

*Beta 기능*

지정된 범용 ID 유형이 포함된 세그먼트로 변환할 고객 데이터 플랫폼의 각 자사 대상에 대한 DSP 소스를 만듭니다. 조직의 DSP 계정 또는 광고주 계정으로 세그먼트를 가져올 수 있습니다. 데이터 요금은 선택한 범용 ID 유형을 기반으로 적용됩니다. 소스를 만들고 나면 각 고객 데이터 플랫폼에서 대상을 수집하는 추가 단계가 필요합니다. 소스를 만들려면 절차 끝에 있는 메모를 참조하십시오.

나중에 소스 대상이 번역되는 범용 ID 유형을 변경하고 변경 내용의 로그를 볼 수 있습니다.

소스를 삭제할 수도 있습니다.

## 대상 Source 만들기

<!-- Not sure about this

You can create one source for each combination of universal ID partner and data visibility level.

-->

1. 메인 메뉴에서 **[!UICONTROL Audiences]** > **[!UICONTROL Sources]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Add Source]**&#x200B;을(를) 클릭합니다.

1. [!UICONTROL Select a Type] 메뉴에서 [고객 데이터 플랫폼](source-about.md)을 선택합니다.

   * *[!UICONTROL RT-CDP]*: [!DNL Adobe Real-Time CDP].

   * *[!UICONTROL ActionIQ]*: [!DNL ActionIQ] 고객 데이터 플랫폼입니다.

   * *[!UICONTROL Amperity]*: [!DNL Amperity] 고객 데이터 플랫폼입니다.

   * *[!UICONTROL Optimizely]*: [!DNL Optimizely] 고객 데이터 플랫폼입니다.

   * *[!UICONTROL Tealium CDP]*: (구성된 사용자만 해당) [!DNL Tealium] 고객 데이터 플랫폼입니다.

1. [!UICONTROL Data Visibility Level]: *[!UICONTROL Advertiser]* 또는 *[!UICONTROL Account]*&#x200B;을(를) 지정하십시오.

1. 나머지 [원본 설정](#source-settings)을 입력하십시오.

   생성된 [!UICONTROL Source Key]의 복사본을 보관합니다. 나중에 값이 필요합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

>[!NOTE]
>
>고객 데이터 플랫폼에 대한 소스를 만든 후에는 대상을 가져오기 위한 추가 단계를 완료해야 합니다. [워크플로  [!DNL Adobe] [!DNL Real-time CDP]](source-adobe-rtcdp.md),<!-- the [workflow for [!DNL ActionIQ]](source-actioniq.md), --> [워크플로 [!DNL Amperity]](source-amperity.md), [워크플로 [!DNL Optimizely]](source-optimizely.md) 및 [워크플로 [!DNL Tealium]](source-tealium.md)를 참조하십시오.

## 대상 Source의 ID 유형 변경

<!-- Clarify this:
All changes to universal IDs translated from the source are applied after you save the the source record. For example, if a new ID is added, any hashed email addresses shared before making the changes aren't converted. Similarly, if an ID is removed, we don't delete any historical data from the segments shared through the source.

OR 

All changes to universal IDs translated from the source are applied after you save the the source record. For example, if you add a new ID type, then we convert hashed email addresses shared before making the changes to the new ID type. Similarly, if you remove an ID type, then we delete any historical IDs of that type from the segments shared through the source.

-->

1. 메인 메뉴에서 **[!UICONTROL Audiences]** > **[!UICONTROL Sources]**&#x200B;을(를) 클릭합니다.

1. 원본 행 위에 커서를 놓고 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. 소스에 대해 선택한 [ID](#source-settings)을(를) 변경합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 대상 Source 삭제

원본을 삭제하면 원본을 통해 번역된 세그먼트가 제거됩니다.<!-- Will performance data for the segment still be available in any types of reports?  If yes, which? -->

1. 메인 메뉴에서 **[!UICONTROL Audiences]** > **[!UICONTROL Sources]**&#x200B;을(를) 클릭합니다.

1. 원본 행 위에 커서를 놓고 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

## 대상 Source에 대한 변경 로그 보기

대상자 소스 레코드 변경 사항에 대한 세부 정보를 보고 선택적으로 로그에 메모를 첨부할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Audiences]** > **[!UICONTROL Sources]**&#x200B;을(를) 클릭합니다.

1. 원본 행 위에 커서를 놓고 **[!UICONTROL Change log]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 변경 로그에 메모를 첨부하려면 다음을 수행합니다.

   1. 원본 행 위에 커서를 놓고 **[!UICONTROL Add Notes]**&#x200B;을(를) 클릭합니다.

   1. 메모를 입력한 다음 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

      최대 길이는 256자입니다.

1. (선택 사항) 더 큰 세부 정보 화면에서 로그를 열려면 원본 행 위에 커서를 놓고 **[!UICONTROL View Details]**&#x200B;을(를) 클릭합니다.

## 대상 Source 설정 {#source-settings}

**[!UICONTROL Data Visibility Level]:** 계정에 대한 액세스 권한이 있는 단일 광고주(*[!UICONTROL Advertiser]*)나 *[!UICONTROL Account]* 계정에 대한 액세스 권한이 있는 모든 광고주가 세그먼트를 사용할 수 있는지 여부.

**[!UICONTROL Advertiser]:**(광고주 수준 가시성만 해당) 세그먼트를 사용할 수 있는 광고주입니다. 계정에 액세스할 수 있는 광고주 목록에서 하나를 선택합니다.

**[!UICONTROL Enter IMS Org Id]:**([!DNL Real-Time CDP] 소스만 해당) [!DNL Adobe Experience Platform] 계정에 대한 Adobe Experience Cloud 조직 ID입니다.

**[!UICONTROL Convert PII to the following IDs]:** PII(개인 식별 정보)를 변환할 ID 유형입니다. 여러 유형을 선택하면 생성된 세그먼트는 선택한 각 ID 유형의 값으로 채워집니다(예: 각 이메일 주소의 [!DNL RampID] 및 [!DNL Unified ID2.0]). 그에 따라 데이터 요금이 부과됩니다.

[!DNL RampID] 및 [!DNL Unified ID2.0]의 경우 공급업체는 각 이메일 주소를 조회하여 ID가 이미 있는지 확인하고 가능한 경우 해당 주소를 일치하는 ID로 변환합니다. 주소에 대한 ID가 없는 경우 새 ID가 만들어집니다.

>[!NOTE]
>
>단일 배치에서 한 가지 유형의 ID만 타깃팅할 수 있습니다. ID 유형별로 성능을 테스트하려면 [세그먼트의 각 ID 유형에 대해 별도의 배치를 만듭니다](/help/dsp/campaign-management/placements/placement-create.md).

* *[!DNL RampID]:* PII를 [!DNL RampID] (으)로 변환하려는 경우 로그인 사용자를 다시 타겟팅하고 [[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md) 측정을 위해 [!DNL RampIDs]을(를) 사용할 수 있습니다.

* *[!DNL Unified ID2.0] (Beta):* 로그인 사용자를 다시 타깃팅하기 위해 PII를 [통합 ID 2.0](https://unifiedid.com) ID로 변환하려는 경우

<!-- Later
* *[!DNL ID5] (Beta):* To convert PII to an [!DNL ID5] ID. You can use [!DNL ID5] IDs for retargeting logging-in users and for [[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md) measurement.

-->

**[!UICONTROL Terms of Service]:** PII를 범용 ID로 변환하는 서비스 약관 계약입니다. 데이터를 새 ID 유형으로 변환하려면 사용자나 DSP 계정의 다른 사용자가 약관에 한 번 동의해야 합니다. 관리 서비스 계약을 보유한 고객의 경우 Adobe 계정 팀이 귀하의 동의를 받고 조직을 대신하여 약관에 동의합니다. 용어를 읽으려면 **>**&#x200B;을(를) 클릭합니다. 약관에 동의하려면 약관의 맨 아래로 스크롤하여 **[!UICONTROL Accept]**&#x200B;을(를) 클릭합니다.

**[!UICONTROL Source Key]:**(읽기 전용, 자동으로 생성됨) 고객 데이터 플랫폼에서 대상 연결을 만들어 대상을 Advertising DSP으로 푸시하는 데 사용할 수 있는 소스 키입니다. 값을 클립보드에 복사하여 대상 연결 설정 또는 파일에 붙여넣을 수 있습니다.

>[!MORELIKETHIS]
>
>* [자사 대상 소스 정보](source-about.md)
>* [범용 ID 활성화 지원](/help/dsp/audiences/universal-ids.md)
>* [사용자 ID를  [!DNL Adobe Real-Time CDP] 에서 범용 ID로 변환](/help/dsp/audiences/sources/source-adobe-rtcdp.md)
>* [사용자 ID를  [!DNL Amperity] 에서 범용 ID로 변환](/help/dsp/audiences/sources/source-amperity.md)
>* [사용자 ID를  [!DNL Optimizely] 에서 범용 ID로 변환](/help/dsp/audiences/sources/source-optimizely.md)
>* [사용자 ID를  [!DNL Tealium] 에서 범용 ID로 변환](/help/dsp/audiences/sources/source-tealium.md)
>* [대상자 관리 정보](/help/dsp/audiences/audience-about.md)
