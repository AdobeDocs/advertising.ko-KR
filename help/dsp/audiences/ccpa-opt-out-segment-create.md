---
title: CCPA 판매 중지 세그먼트 만들기 및 구현
description: 소비자 판매 중지 요청에서 사용자 ID를 추적하는 세그먼트를 만들고 구현하는 방법을 알아봅니다.
feature: CCPA, DSP Segments
exl-id: 0623c52e-02ea-4e06-bc54-8abb7a87765a
source-git-commit: 4b9cc5956d573b346eacdf71a8ea490c162b4660
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

# CCPA 판매 중지 세그먼트 만들기 및 구현

캘리포니아 소비자 개인 정보 보호법(CCPA)에 따라 웹 사이트의 소비자 판매 중지 요청에서 사용자 ID를 추적하는 세그먼트를 만들 수 있습니다. 사용자는 CCPA 판매 중지 세그먼트에 무기한 유지됩니다.

세그먼트 픽셀 태그가 구현되면 Adobe Advertising은 광고주를 대신하여 ID 풀을 수집하기 시작합니다.

>[!NOTE]
>
>* Adobe Experience Platform Privacy Service API를 사용하여 CCPA 판매 중지 요청을 Adobe Advertising에게 전달하는 방법에 대한 자세한 내용은 을 참조하십시오. [https://experienceleague.adobe.com/docs/advertising/privacy/ccpa/ccpa-opt-out-of-sale.html](https://experienceleague.adobe.com/docs/advertising/privacy/ccpa/ccpa-opt-out-of-sale.html).
>* CCPA 판매 중지 이벤트 추적과 관련이 없는 목적으로 웹 페이지를 방문하는 사용자뿐만 아니라 데스크탑, 모바일 및 CTV 디바이스에서 광고에 노출된 사용자를 추적하려면 [사용자 지정 세그먼트](/help/dsp/audiences/custom-segment-create.md).

1. 세그먼트를 만듭니다.

   1. 메인 메뉴에서 **대상 > 세그먼트**.

   1. 데이터 테이블 위에서 **[!UICONTROL Create]**.

   1. 고유 항목 입력 **[!UICONTROL Segment Name]**.

      권장 세그먼트 이름: &quot;&lt;*광고주 이름*> - CCPA 판매 중지&quot;(예: &quot;Acme - CCPA 판매 중지&quot;)

   1. 의 경우 [!UICONTROL Segment Type], 선택 **[!UICONTROL CCPA Opt-out of sale]**.

   1. 클릭 **[!UICONTROL Save]**.

1. 픽셀 태그를 복사하여 구현하여 세그먼트를 추적합니다.

   1. 다음으로 돌아가기: **[!UICONTROL Audiences]** > **[!UICONTROL Segments]**.

   1. 세그먼트 행에서 새 세그먼트 위에 커서를 놓고 을 클릭합니다 **[!UICONTROL Get pixel]**.

   1. 이미지 픽셀 복사( `<img src="https://rtd-tm.everesttech.net"`)을 클릭하여 웹 페이지에서 데스크탑 및 모바일 방문자의 사용자 ID를 수집할 수 있습니다.

   1. 회사가 CCPA 판매 중지 요청을 추적하는 데 사용하는 메커니즘(예: 동의 관리 플랫폼 사용)을 사용하여 배포를 위해 광고주 또는 웹 사이트 담당자에게 태그를 제공합니다.

      광고주의 IT 부서 또는 다른 그룹은 태그 배포를 예약하거나 그에 대한 정보를 받아야 할 수 있습니다.

      픽셀이 구현되면 Adobe Advertising은 광고주를 대신하여 ID 풀을 수집하기 시작합니다.

      구현 선택 및 논리는 광고주에게 달려 있지만 다음은 광고주가 픽셀을 실행하는 방법의 예입니다.

      1. 한 소비자가 그 광고주의 홈페이지에 온다.
      1. 소비자는 광고주의 &quot;CCPA 판매 중지&quot; 버튼을 찾아 클릭합니다.
      1. 소비자는 광고주가 일하는 서비스 제공자의 목록을 제시받는다.
      1. 소비자가 상자를 선택하여 Adobe Advertising에 데이터 판매를 거부합니다.

         이 작업은 픽셀이 실행되고 지정된 &quot;&quot; 내에서 소비자의 쿠키 ID가 수집되도록 트리거합니다.[!UICONTROL CCPA Opt-out of sale]&quot; 세그먼트.

>[!MORELIKETHIS]
>
>* [캘리포니아 소비자 개인 정보 보호법에 대한 Adobe Advertising 지원: 소비자 옵트아웃 지원](/help/privacy/ccpa/ccpa-opt-out-of-sale.md)
>* [정보 [!UICONTROL CCPA Opt-out-of-Sale] 세그먼트 및 보고서](ccpa-opt-out-about.md)
>* [소비자 판매 중지 보고서 검색](ccpa-opt-out-segment-report-retrieve.md)
>* [사용자 지정 세그먼트 만들기 및 구현](custom-segment-create.md)
>* [대상자 관리 기본 정보](audience-about.md)
