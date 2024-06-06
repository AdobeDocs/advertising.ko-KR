---
title: 대상 소스 설정
description: 대상 소스의 설정에 대해 알아보십시오.
feature: DSP Audiences
exl-id: 274ea502-ad15-4d3d-922a-17caddb87f69
source-git-commit: 295cc610a7e5e811fe555db69373a8bf5b4012f7
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 0%

---

# 대상 소스 설정

*Beta 기능*

**[!UICONTROL Data Visibility Level]:** 계정에 액세스할 수 있는 단일 광고주가 세그먼트를 사용할 수 있는지 여부(*[!UICONTROL Advertiser]*) 또는 계정에 액세스할 수 있는 모든 광고주 *[!UICONTROL Account]*.

**[!UICONTROL Advertiser]:** (광고주 수준 가시성만 해당) 세그먼트를 사용할 수 있는 광고주입니다. 계정에 액세스할 수 있는 광고주 목록에서 하나를 선택합니다.

**[!UICONTROL Enter IMS Org Id]:** ([!DNL Real-Time CDP] Adobe Experience Cloud 소스만 해당) [!DNL Adobe Experience Platform] 계정입니다.

**[!UICONTROL Convert PII to the following IDs]:** PII(개인 식별 정보)를 변환할 ID 유형입니다. 여러 유형을 선택하면 생성된 세그먼트가 선택한 각 ID 유형에 대한 값(예: )으로 채워집니다. [!DNL RampID] 및 a [!DNL Unified ID2.0] (각 이메일 주소). 그에 따라 데이터 요금이 부과됩니다.

대상 [!DNL RampID] 및 [!DNL Unified ID2.0], 공급업체는 ID가 이미 존재하는지 확인하기 위해 각 이메일 주소를 조회하고 사용 가능한 경우 해당 주소를 일치하는 ID로 변환합니다. 주소에 대한 ID가 없는 경우 새 ID가 만들어집니다.

>[!NOTE]
>
>단일 배치에서 한 가지 유형의 ID만 타깃팅할 수 있습니다. ID 유형별로 성능을 테스트하려면 [별도의 배치 만들기](/help/dsp/campaign-management/placements/placement-create.md) 를 참조하십시오.

* *[!DNL RampID]:* PII를 로 변환하려면 [!DNL RampID]. 다음을 사용할 수 있습니다. [!DNL RampIDs] 로그인 사용자 및 을 재타겟팅하기 위한 [[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md) 측정.

* *[!DNL Unified ID2.0](베타):* PII를 로 변환하려면 [통합 ID 2.0](https://unifiedid.com) 로그인 사용자를 재타겟팅하기 위한 ID.

<!-- Later
* *[!DNL ID5] (Beta):* To convert PII to an [!DNL ID5] ID. You can use [!DNL ID5] IDs for retargeting logging-in users and for [[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md) measurement.

-->

**[!UICONTROL Terms of Service]:** PII를 범용 ID로 전환하기 위한 서비스 약관. 데이터를 새 ID 유형으로 변환하려면 사용자나 DSP 계정의 다른 사용자가 약관에 한 번 동의해야 합니다. 관리 서비스 계약을 보유한 고객의 경우 Adobe 계정 팀이 귀하의 동의를 받고 조직을 대신하여 약관에 동의합니다. 용어를 읽으려면 다음을 클릭합니다. **>**. 용어를 수락하려면 약관의 맨 아래로 스크롤하여 을 클릭합니다 **[!UICONTROL Accept]**.

**[!UICONTROL Source Key]:** (읽기 전용, 자동으로 생성됨) 고객 데이터 플랫폼에서 대상 연결을 생성하여 대상을 Advertising DSP으로 푸시하는 데 사용할 수 있는 소스 키입니다. 값을 클립보드에 복사하여 대상 연결 설정 또는 파일에 붙여넣을 수 있습니다.

>[!MORELIKETHIS]
>
>* [범용 ID 대상을 활성화하기 위한 대상 소스 관리](source-manage.md)
>* [자사 대상 소스 정보](source-about.md)
>* [에서 인증된 세그먼트 수동으로 가져오기 [!DNL LiveRamp]](/help/dsp/audiences/sources/source-import-liveramp-segments.md)
>* [Adobe Advertising DSP 연결](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/advertising/adobe-advertising-cloud-connection.html)
>* [대상자 관리 기본 정보](/help/dsp/audiences/audience-about.md)
