---
title: FAQ
description: xxx
source-git-commit: e517dd5f5fa283ff8a2f57728612937148889732
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---

# FAQ xxx

## 제목

https://adobeadcloud.zendesk.com/agent/tickets/14214 기본적으로 Adobe Analytics은 모든 보고서에서 캡처된 모든 이벤트를 보고합니다. &quot;[!UICONTROL Unspecified]&quot;이벤트는 Adobe Advertising에 연결되지 않은 양식 완료 이벤트를 나타냅니다. 예를 들어 광고 플랫폼 보고서에서 이메일 캠페인으로 구동되는 유기 전환 또는 전환은 &quot;지정되지 않음&quot;으로 표시됩니다.

필터를 사용하여 &quot;지정되지 않음(없음) 포함&quot; 선택 사항으로 확인 표시를 제거하여 보고서에서 지정되지 않은 이벤트를 제거할 수 있습니다. <!-- Not sure if this is in DSP or in Analytics Workspace -->

## 제목

https://adobeadcloud.zendesk.com/agent/tickets/24323 Analytics 이벤트 태그를 Ad Cloud 픽셀과 동일한 지점에 배치하여 XXX가 일치하는지 확인합니다.

## 제목

https://adobeadcloud.zendesk.com/agent/tickets/24323

Q: 내부 보안 감사 중에 특정 기능은 Ad Cloud을 기존 Adobe Analytics 설치에 통합했을 때 활성화한 보안 문제로 플래그가 지정되었습니다.

문제가 되는 통합은 AdCloud와 Adobe Audience Manager 사이입니다. 이 기능은 AdCloud와 Adobe Audience Manager 간의 방문자 ID에 대한 일치율을 높입니다. 이 작업은 pagead.l.doubleclick.net, star-mini.c10r.facebook.com 및 pug88000nf.pubmatic.com에 네트워크 요청을 전송하여 이러한 서비스에 활용할 수 있는 방문자에 대한 기존 ID가 있는지 확인합니다. 이는 보안 위험으로 플래그가 지정된 네트워크 요청으로 모든 사이트 방문자에 대해 발생하고 있습니다.

감사에서 이 기능을 비활성화하도록 요청하고 있습니다. 네트워크 요청을 차단하면 어떻게 됩니까?

A: 당사의 제품과 함께 확인했으며 문제의 픽셀이 Ad Cloud, 특정 재고/SSP 파트너(DSP과 관련하여) 및 AAM 간의 쿠키 일치율을 높이기 위한 목적이라고 언급했습니다.  이러한 구성 요소가 제거되면 고객은 AAC/AAM과 각 픽셀이 사용되는 인벤토리 파트너 간에 일정 수준의 일치율이 감소하는 것을 볼 수 있지만 실제로 수행되지는 않을 것입니다.

Ad Cloud 검색의 경우 광고주의 Experience Cloud 조직 ID가 Mathworks에 대해 설정되어 있지만 제품 팀에 Ad Cloud에서 대상을 활성화하기 위한 Mathworks 설정이 표시되지 않습니다. Ad Cloud 검색으로 대상을 보내는 데 Adobe Audience Manager를 사용하고 있습니까? 그렇지 않으면 이러한 매개 변수를 제거해도 현재 워크플로우에는 영향을 주지 않습니다. AAM 고객 지원 센터는 이러한 픽셀을 실행하지 않으려면 이러한 픽셀을 제거하는 데 도움을 줄 수 있습니다.

