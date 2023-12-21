---
title: 대상 소스 설정
description: 대상 소스의 설정에 대해 알아보십시오.
feature: DSP Audiences
exl-id: 274ea502-ad15-4d3d-922a-17caddb87f69
source-git-commit: 6c918b387067237de5d1eae42ae8ad253884d761
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 0%

---

# 대상 소스 설정

**[!UICONTROL Data Visibility Level]:** 계정에 액세스할 수 있는 단일 광고주가 세그먼트를 사용할 수 있는지 여부(*[!UICONTROL Advertiser]*) 또는 계정에 액세스할 수 있는 모든 광고주 *[!UICONTROL Account]*.

**[!UICONTROL Advertiser]:** (광고주 수준 가시성만 해당) 세그먼트를 사용할 수 있는 광고주입니다. 계정에 액세스할 수 있는 광고주 목록에서 하나를 선택합니다.

**[!UICONTROL Enter IMS Org Id]:** ([!DNL Real-Time CDP] Adobe Experience Cloud 소스만 해당) [!DNL Adobe Experience Platform] 계정입니다.

**[!UICONTROL Convert PII to the following IDs]:** ([!DNL ActionIQ] 및 [!DNL Tealium] 소스만 해당) PII(개인 식별 정보)를 변환할 ID 유형입니다. 그에 따라 데이터 요금이 부과됩니다.

* *[!DNL RampID]:* PII를 RampID로 변환하려면 다음을 선택하는 경우 *[!DNL RampID]*, 세그먼트가 로 변환됩니다. [!DNL RampIDs] 자동으로 표시됩니다.

* *[!DNL Unified ID2.0]:* ([!DNL ActionIQ] 소스만 해당) PII를 [통합 ID 2.0](https://unifiedid.com/).

**[!UICONTROL Source Key]:** (읽기 전용, 자동으로 생성됨) 고객 데이터 플랫폼에서 대상 연결을 생성하여 대상을 Advertising DSP으로 푸시하는 데 사용할 수 있는 소스 키입니다. 값을 클립보드에 복사하여 대상 연결 설정 또는 파일에 붙여넣을 수 있습니다.

>[!MORELIKETHIS]
>
>* [자사 대상을 활성화할 대상 소스 만들기](source-create.md)
>* [대상 소스에서 인증된 세그먼트 활성화 정보](source-about.md)
>* [범용 ID 파트너에서 인증된 세그먼트 활성화](source-universal-id.md)
>* [Adobe Advertising DSP 연결](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/advertising/adobe-advertising-cloud-connection.html)
>* [대상자 관리 기본 정보](/help/dsp/audiences/audience-about.md)
