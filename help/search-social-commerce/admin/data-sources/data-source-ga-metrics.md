---
title: 사용 가능 [!DNL Google Analytics] 지표
description: 참조 [!DNL Google Analytics] 데이터 소스에 사용할 수 있는 지표입니다.
role: User, Admin
exl-id: f7ac93e3-1aed-4165-ae65-7966ca192c84
feature: Search Admin, Search Data Sources
source-git-commit: 9c4dcb19e386d8e1eea541776f5b92c9d500ae9f
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---

# 부록 - 사용 가능 [!DNL Google Analytics] 지표

언급된 제외를 제외하고 다음 지표는에서 고객의 구현에 활성화되어 있을 때 사용할 수 있습니다. [!DNL Google Analytics].

<!-- Notes as FYI to self:
>[!NOTE]
>
>* For some of these metrics, [!DNL Google] assigns the friendly name, and the name is consistent. For some metrics, the advertiser assigns the friendly name in [!DNL Google Analytics], and the name has a dynamic value.
>* Some metrics are assigned at the property level, and others are assigned at the view level.
-->

| 범주 | 제외됨 | 댓글 |
| ---- | ---- | ---- |
| \[All\] | 데이터 유형이 &quot;PERCENT&quot;인 지표 | 백분율로 표시된 지표는 항상 제외됩니다. |
| 사용자 | ga:1dayUsers, ga:7dayUsers, ga:14dayUsers, ga:28dayUsers, ga:sessionsPerUser | — |
| 세션 | ga:uniqueDimensionCombinations | — |
| 목표 전환 | — | — |
| 페이지 추적 | ga:entrances, ga:timeOnPage, ga:exits | — |
| 내부 검색 | — | 내부 검색의 모든 지표에 대한 친숙한 이름 앞에는 &quot;InternalSearch: &quot; 값이 붙습니다. |
| 이벤트 추적 | — | — |
| Ecommerce | — | — |
| 소셜 상호 작용 | — | — |
| 예외 | — | — |
| 사용자 지정 변수 또는 열 | ga:calcMetric_* | 계산된 지표는 항상 제외됩니다. |

>[!MORELIKETHIS]
>
>* [동기화 기본 정보 [!DNL Google Analytics] 전환 지표](data-source-about.md)
>* [구성 사전 요구 사항 [!DNL Google Analytics] 데이터 소스](data-source-prerequisites.md)
>* [구성 [!DNL Google Analytics] 데이터 소스로 보기](data-source-configure.md)
>* [편집 [!DNL Google Analytics] 데이터 소스](data-source-edit.md)
>* [데이터 소스 동기화 일시 중지](data-source-pause.md)
>* [재인증 [!DNL Google Analytics] 데이터 소스](data-source-reauthenticate.md)
>* [[!DNL Google Analytics] 데이터 소스 설정](data-source-settings.md)
