---
title: Adobe Advertising Creative 구현 개요
description: ' [!DNL Creative]을(를) 구현하기 위한 기본 워크플로에 대해 알아봅니다.'
feature: Creative Introduction
source-git-commit: fbd85ce99ab177c70b95bae42166265ef9053034
workflow-type: tm+mt
source-wordcount: '998'
ht-degree: 0%

---

# Adobe Advertising Creative 구현 개요

*베타가 닫힘*

<!-- CLARIFY HOW "ad" and "creative" are delineated, if they are. If they're not, why do we have different terms scattered around? -->

[!DNL Creative] 운영 팀은 각 광고주와 함께 광고 경험을 DSP 내의 광고로 구현하거나 팀에 타사 광고 태그를 제공하여 자체적으로 구현하고 초기 비용, 클릭 및 전환 데이터를 확인하는 크리에이티브 및 크리에이티브 경험을 설정합니다.

계속적으로 Adobe 계정 팀, 에이전시 팀 또는 광고주(service level agreement 약관에 따라 다름)는 각 경험을 모니터링하고 광고주의 목표를 달성하기 위해 필요에 따라 편집해야 합니다.

## [!DNL Creative] 경험에 대한 초기 설정 작업

구현 팀 및/또는 에이전시는 귀하와 함께 다음 작업을 수행합니다.

1. 개인화 목표(예: 전망 또는 재타겟팅을 위한 광고를 개인화할 것인지 여부), 크리에이티브 자산 및 대상 세그먼트를 포함하여 사용 가능한 모든 자사, 제2자 및 타사 데이터, 그리고 목표를 달성하기 위한 전략을 정의합니다.<!-- and CRM data? used how/where? -->

1. (새 광고주 계정) 관리 계정을 설정합니다.

   1. [!DNL Creative]에 대한 광고주 계정을 설정하고 Advertising 검색, 소셜 및 Commerce에서도 계정을 만드십시오.

      광고주가 DSP의 나머지 부분을 사용하지 않더라도 [!DNL Creative] 계정 설정은 Advertising DSP 내에 있습니다.

      마찬가지로 광고주가 [!DNL Search, Social, & Commerce] 고객이 아닌 경우에도 [!DNL Search, Social, & Commerce] 계정을 사용하여 전환 추적 태그를 만들고 [!DNL Creative]에서 전환 열을 설정합니다.

   1. (필요한 경우) 광고주가 광고 크리에이티브 및 광고 경험을 보고 관리하고 보고서를 생성할 수 있도록 사용자 계정을 생성합니다.

1. (선택 사항) 크리에이티브 대상으로 포함할 자사 대상 세그먼트를 만들려면 다음 방법 중 하나로 태그를 만듭니다.

   * 특정 특성을 가진 방문자에게 특정 랜딩 페이지나 전환 페이지에 대한 광고를 다시 타깃팅할 수 있는 [픽셀 다시 타깃팅](/help/creative/pixels/retargeting-pixel-manage.md)을 만든 다음 관련 웹 페이지에 삽입할 태그를 생성합니다.

   * (DSP을 사용하는 광고주) DSP 내에서 [사용자 지정 대상 세그먼트를 만들어](/help/dsp/audiences/custom-segment-create.md)특정 랜딩 페이지나 전환 페이지에 대한 모든 방문자를 추적한 다음 관련 웹 페이지에 삽입할 태그를 생성합니다.

   두 종류의 태그는 모두 이미지 태그로, 최종 사용자가 볼 수 없는 1픽셀 x 1픽셀 투명 이미지(픽셀)를 추가한 웹 페이지에 표시합니다. 나중에 특정 재타겟팅 픽셀 또는 세그먼트를 타겟팅하도록 광고 경험에서 크리에이티브를 구성할 수 있으므로 관련 광고 요소는 픽셀 또는 세그먼트와 연관된 사이트 페이지를 이전에 방문한 사용자에게만 표시됩니다.

   광고주의 IT 부서 또는 다른 그룹은 태그 배포를 예약하거나 그에 대한 정보를 받아야 할 수 있습니다.

   **참고:** Adobe Audience Manager 및 Adobe Analytics의 자사 대상자를 크리에이티브 대상으로 사용할 수도 있습니다. 방문자가 [!DNL Analytics]에서 공유한 대상 자격을 얻으면 [!DNL Creative]에서 약 24~48시간 내에 정보를 실행할 수 있습니다. <!--Are times still true? -->

1. 광고 경험을 구현할 DSP 내에서 캠페인 계층 구조를 설정합니다. 캠페인 내에서 구현할 광고 경험의 타겟팅과 호환되는 타겟팅을 사용하십시오.

   계층 타겟팅 동작은 DSP에 따라 다를 수 있습니다. Advertising DSP은 배치 수준 타깃팅의 맨 위에(대신 아님) 광고 수준 타깃팅을 적용합니다. 예를 들어 배치가 오스트레일리아의 사용자를 타겟팅하고 광고가 일본의 사용자를 타겟팅하는 경우 광고는 경험에 대한 &quot;기타 사용자&quot; 분기를 타겟팅합니다. 전체 캠페인 구조를 통해 생각하도록 하십시오.

1. 광고 목표를 기반으로 광고 경험을 설정합니다.

   * **자동화 워크플로:** [!DNL Creative] 운영팀은 광고 템플릿 및 데이터 피드를 사용하여 조직에 대한 동적 광고를 만들 수 있습니다.

     자세한 내용은 Adobe 계정 팀에 문의하십시오.

     <!-- LATER, in a later phase: (Advertisers with Adobe Experience Manager; optional) Configure access to image assets in the Experience Manager account. --><!-- I think this will be automatic based on their IMS organization. But I'm not sure if they need to be logged in via SSO using their Adobe login or if it will also work using their legacy DSP login. -->

   * **수동 워크플로:** 광고 환경을 수동으로 설정:

      1. [경험에서 사용할 표준 광고 설정](/help/creative/creative-libraries/creative-add-standard.md):

         * [!DNL Creative]이(가) 호스팅할 크리에이티브의 경우 업로드하십시오. Adobe Experience Manager 계정에 이미지 자산이 포함될 수 있습니다.

         * 지원되는 타사 광고 서버에서 호스팅되는 크리에이티브의 경우 크리에이티브 파일을 가리킵니다.

      1. (선택 사항) 한 단계에서 타깃팅된 경험에 연결할 수 있는 [크리에이티브를 번들로 그룹화](/help/creative/creative-libraries/bundle-manage.md)합니다.

      1. [광고 경험](/help/creative/experiences/experience-about.md) 설정:

         * [타깃팅된 광고 경험](/help/creative/experiences/experience-create-targeting.md)의 경우 광고 크리에이티브 및 선택적 광고 타겟의 시퀀스를 지정하십시오.

           광고 대상에는 [!DNL Creative]에서 만든 재타겟팅 픽셀, Adobe Experience Cloud의 대상 세그먼트(DSP, Audience Manager 또는 [!DNL Analytics]에서 포함), 지리적 대상 또는 웹 페이지의 특정 데이터 트리거(예: SKU=01234567890123 또는 Cart=empty)가 포함될 수 있습니다.

         * [타깃팅되지 않은 광고 경험](/help/creative/experiences/experience-create-no-targeting.md)의 경우 일반 경험 설정을 만드십시오.

           광고 대상에는 [!DNL Creative]에서 만든 재타겟팅 픽셀, Adobe Experience Cloud의 대상 세그먼트(DSP, Audience Manager 또는 [!DNL Analytics]에서 포함), 지리적 대상 또는 웹 페이지의 특정 데이터 트리거(예: SKU=01234567890123 또는 Cart=empty)가 포함될 수 있습니다.













1. 광고 경험에 대한 전환 추적을 설정합니다.


전환 추적을 설정합니다. 구현에 따라 다음과 같은 작업이 포함될 수 있습니다.
광고주의 웹 페이지에 대한 전환 추적 태그 및/또는 매일 설정
광고주가 별도로 수집한 전환 데이터에 대한 피드 삭제.


Advertising 검색, 소셜 및 Commerce 내에서 또는 Adobe 다이내믹 태그 관리자(이전 명칭: 다이내믹 태그 관리자) 내에서 Adobe Advertising 전환 추적 태그를 생성할 수 있습니다.
참고: 이미지 태그가 아닌 JavaScript 전환 태그를 사용해야 합니다.


광고주의 IT 부서나 다른 그룹에게 일정을 정하거나 정보를 제공해야 할 수 있습니다
태그 배포에 대한 정보입니다.


(선택 사항) 검색, 소셜 및 Commerce 내에서 각 전환(거래 속성)을 수행합니다
데이터 보기 및 보고서에서 개별 열 세트로 사용할 수 있습니다.


전환(거래 속성)은 다음 시간 이후에 검색, 소셜 및 Commerce에 나열됩니다.
하나 이상의 전환 이벤트가 추적되었습니다.


특정 지표를 사용할 수 있도록 하지 않으면 모든 전환이 통합됩니다
하나의 &quot;전환&quot; 열 집합에서


추적되는 데이터의 유효성을 검사합니다.


(선택 사항) 지정된 이메일 주소에 예약된 보고서의 전달을 설정합니다.


자세한 내용은 &quot;보고서&quot;의 도움말 장을 참조하십시오.


Advertising DSP 또는 다른 DSP에서 광고 캠페인을 설정하고 JavaScript을 제공합니다.
또는 를 구현할 수 있는 광고주에게 광고 경험에 대한 iframe 태그
DSP의 타사 광고.


사전 정의된 광고를 보면서 완료된 광고 경험의 성능을 모니터링합니다
개별 경험에 대한 성능 세부 정보 또는 사용자 지정 성능 보고서 만들기


(필요한 경우) 성능 및 업데이트된 메시징을 기반으로 광고 경험을 업데이트합니다.






>[!MORELIKETHIS]
>
>* [Adobe Advertising Creative 정보](/help/creative/introduction/creative-about.md)
>* [사용자 인터페이스를 구성하는 방법](/help/creative/introduction/ui.md)
