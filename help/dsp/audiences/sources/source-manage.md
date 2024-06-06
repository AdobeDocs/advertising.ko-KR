---
title: 범용 ID 대상을 활성화하기 위한 대상 소스 생성 및 관리
description: 소스를 만들고 관리하여 고객 데이터 플랫폼에서 대상을 가져와 범용 ID가 포함된 세그먼트로 변환하는 방법에 대해 알아봅니다.
feature: DSP Audiences
exl-id: 728130d7-d19c-4d5d-9bca-695f8c17f89b
source-git-commit: 295cc610a7e5e811fe555db69373a8bf5b4012f7
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# 범용 ID 대상을 활성화하는 대상 소스 만들기

*Beta 기능*

지정된 범용 ID 유형이 포함된 세그먼트로 변환할 고객 데이터 플랫폼의 각 자사 대상에 대한 DSP 소스를 만듭니다. 조직의 DSP 계정 또는 광고주 계정으로 세그먼트를 가져올 수 있습니다. 데이터 요금은 선택한 범용 ID 유형을 기반으로 적용됩니다.

각 고객 데이터 플랫폼에서 대상을 수집하는 데 추가 단계가 필요합니다. 절차 끝에 있는 메모를 참조하십시오.

## 대상 소스 만들기

1. 메인 메뉴에서 **[!UICONTROL Audiences]** > **[!UICONTROL Sources]**.

1. 클릭 **[!UICONTROL Add Source]**.

1. 다음에서 [!UICONTROL Select a Type] 메뉴에서 고객 데이터 플랫폼을 선택합니다.

   * *[!UICONTROL RT-CDP]*: [다음 [!DNL Adobe Real-Time Customer Data Platform]](source-about.md).

   * *[!UICONTROL ActionIQ]*: [[!DNL ActionIQ] 고객 데이터 플랫폼](source-about.md).

   * *[!UICONTROL Tealium CDP]*: (구성된 사용자만 해당) [[!DNL Tealium] 고객 데이터 플랫폼](source-about.md).

1. 다음을 지정합니다. [!UICONTROL Data Visibility Level]: *[!UICONTROL Advertiser]* 또는 *[!UICONTROL Account]*.

1. 나머지 항목 입력 [소스 설정](source-settings.md).

   복사본 보관 [!UICONTROL Source Key] 생성됩니다. 나중에 값이 필요합니다.

1. 클릭 **[!UICONTROL Save]**.

>[!NOTE]
>
>고객 데이터 플랫폼에 대한 소스를 만든 후에는 추가 단계를 완료해야 합니다. 다음을 참조하십시오. [대상자 가져오기 워크플로우 [!DNL Adobe] [!DNL Real-time CDP]](source-adobe-rtcdp.md)<!-- the [activation workflow for [!DNL ActionIQ]](source-actioniq.md), --> 및 [대상자 가져오기 워크플로우 [!DNL Tealium]](source-tealium.md).

## 대상 소스의 ID 유형 변경

1. 메인 메뉴에서 **[!UICONTROL Audiences]** > **[!UICONTROL Sources]**.

1. 소스 행 위에 커서를 놓고 **[!UICONTROL Edit]**.

1. 변경 [소스에 대해 선택된 ID](source-settings.md).

1. 클릭 **[!UICONTROL Save]**.

## 대상 소스 삭제

소스를 삭제하면 소스를 통해 번역된 세그먼트가 제거됩니다.<!-- Will performance data for the segment still be available in any types of reports?  If yes, which? -->

1. 메인 메뉴에서 **[!UICONTROL Audiences]** > **[!UICONTROL Sources]**.

1. 소스 행 위에 커서를 놓고 **[!UICONTROL Delete]**.

1. 확인 메시지에서 다음을 클릭합니다. **[!UICONTROL Delete]**.

## 대상 소스에 대한 변경 로그 보기

대상자 소스 레코드 변경 사항에 대한 세부 정보를 보고 선택적으로 로그에 메모를 첨부할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Audiences]** > **[!UICONTROL Sources]**.

1. 소스 행 위에 커서를 놓고 **[!UICONTROL Change log]**.

1. (선택 사항) 변경 로그에 메모를 첨부하려면 다음을 수행합니다.

   1. 소스 행 위에 커서를 놓고 **[!UICONTROL Add Notes]**.

   1. 메모를 입력한 다음 **[!UICONTROL Save]**.

      최대 길이는 256자입니다.

1. (선택 사항) 더 큰 세부 사항 화면에서 로그를 열려면 소스 행 위에 커서를 놓고 를 클릭합니다 **[!UICONTROL View Details]**.

>[!MORELIKETHIS]
>
>* [대상 소스 설정](source-settings.md)
>* [자사 대상 소스 정보](source-about.md)
>* [Adobe Advertising Cloud DSP 연결](https://experienceleague.adobe.com/docs/experience-platform/destinations/catalog/advertising/adobe-advertising-cloud-connection.html)
>* [대상자 관리 기본 정보](/help/dsp/audiences/audience-about.md)
