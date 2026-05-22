---
title: ' [!DNL AdFixus]에서 자사 세그먼트 가져오기'
description: ' [!DNL AdFixus] 범용 ID로 구성된  [!DNL AdFixus] 자사 세그먼트를 DSP으로 가져오는 방법에 대해 알아봅니다.'
feature: DSP Audiences
product_v2: id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2: id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
subfeature_v2: id: fef5c122-6482-4d17-a8ce-4e70b906f1f4
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
source-git-commit: 79f0b3872a0d5d3765093ce83cc8f1c284a8255c
workflow-type: tm+mt
source-wordcount: 448
ht-degree: 0%

---

# [!DNL AdFixus]에서 자사 세그먼트 가져오기

*오스트레일리아의 광고주에만 적용*

[!DNL AdFixus]과(와) Advertising DSP 통합을 사용하여 타깃팅된 광고를 위한 세그먼트 매핑이 있는 [!DNL AdFixus] 유니버설 ID를 가져옵니다. [!DNL AdFixus] ID는 호주에서만 사용할 수 있습니다. DSP은 [!DNL AdFixus] ID를 다른 ID 유형으로 변경하지 않으며 다른 ID 유형을 [!DNL AdFixus] ID로 변환하지 않습니다. DSP은 ID 가져오기에 대한 비용을 청구하지 않습니다.

[!DNL AdFixus] 세그먼트를 DSP으로 가져오면 [!DNL AdFixus] ID와 [!DNL AdFixus]의 특정 자사 세그먼트에 배치를 타깃팅할 수 있습니다. 재사용 가능한 대상에 [!DNL AdFixus] 세그먼트를 추가할 수도 있습니다. 세그먼트에 대한 세부 정보에는 적용 가능한 [!DNL AdFixus] ID의 개수가 포함됩니다.

사용자 지정 보고서에서 [!DNL AdFixus] ID를 가진 사용자의 노출, 클릭, 빈도 및 기타 지표를 볼 수 있습니다. [!DNL Analytics for Advertising]을(를) 사용하는 광고주는 Adobe Analytics의 [!DNL AdFixus] ID에 대한 뷰스루 데이터와 DSP 내의 Adobe Analytics의 데이터를 볼 수도 있습니다.

1. [!DNL AdFixus]을(를) 사용하여 조직의 자사 데이터를 [!DNL AdFixus] ID를 가진 세그먼트로 변환합니다.

   이를 위해서는 [!DNL AdFixus]이(가) 있는 별도의 계정과 활성 라이선스 키가 필요합니다. 웹 사이트 속성 및 도메인에 대해 [!DNL AdFixus]별 코드를 구현해야 합니다. [!DNL AdFixus]&#x200B;(으)로 직접 작업하여 ID가 있는 세그먼트를 생성합니다.

1. (광고주: [[!DNL Adobe] [!DNL Analytics for Advertising]](/help/integrations/analytics/overview.md)) [!DNL Analytics] 측정에 대한 추적을 설정합니다.

   1. 아직 완료하지 않은 경우) 추적 URL에서 [AMO ID 및 EF ID](/help/integrations/analytics/ids.md)와(과)  [!DNL Analytics for Advertising]](/help/integrations/analytics/prerequisites.md)을(를) 구현하기 위한 [필수 구성 요소를 모두 완료하십시오.

   1. 웹 페이지에 [!DNL AdFixus]별 코드를 배포하여 뷰스루에 대한 데스크톱 및 모바일 웹 브라우저(모바일 앱은 아님)의 [!DNL AdFixus] ID의 전환을 일치시키십시오.

1. 자사 [!DNL AdFixus] 세그먼트 가져오기:

   1. [!UICONTROL Type] **[!UICONTROL AdFixus ID]**&#x200B;의 [대상 원본 만들기](source-manage.md) 서비스 약관에 동의해야 합니다.

      소스 설정에는 자동 생성된 소스 키가 포함됩니다.

   1. 필요한 세그먼트를 DSP에 스트리밍할 수 있도록 [!DNL AdFixus] 팀과 소스 키를 공유하십시오.

1. 대상 라이브러리의 [!UICONTROL First Party Segments] 섹션([!UICONTROL Audiences] > [!UICONTROL All Audiences]에서 대상을 만들거나 편집할 때 또는 배치 설정 내에서 사용할 수 있음)에서 세그먼트가 채워지고 있는지 확인합니다. [!DNL AdFixus] ID 수와 [!DNL AdFixus] 내의 사용자 ID 수를 비교합니다.

   세그먼트는 만들어지는 즉시 DSP에서 사용할 수 있습니다.

DSP에 표시된 카운트는 24시간마다 새로 고쳐지지만 세그먼트는 3시간마다 새로 고쳐지고 타깃팅에 사용할 수 있습니다. **참고:** 세그먼트에 포함된 값은 [!DNL AdFixus]에서 구성하는 지정된 만료 기간이 지나면 만료됩니다. 만료 전에 [!DNL AdFixus]에서 세그먼트를 다시 푸시하여 세그먼트를 새로 고치십시오.

>[!MORELIKETHIS]
>
>* [자사 대상 원본 정보](/help/dsp/audiences/sources/source-about.md)
>* [범용 ID 대상을 활성화하기 위한 대상 소스 관리](source-manage.md)
>* [Adobe Advertising DSP 연결](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/advertising/adobe-advertising-cloud-connection.html)
>* Adobe Experience Platform [대상 카탈로그 개요](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/overview.html)
>* [범용 ID 활성화 지원](/help/dsp/audiences/universal-ids.md)
>* [대상자 관리 정보](/help/dsp/audiences/audience-about.md)
