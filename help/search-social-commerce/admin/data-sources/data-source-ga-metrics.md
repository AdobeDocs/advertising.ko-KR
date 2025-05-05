---
title: 사용 가능한 [!DNL Google Analytics] 지표
description: 데이터 원본에 사용할 수 있는  [!DNL Google Analytics] 지표를 참조합니다.
role: User, Admin
exl-id: 434c569d-7869-4874-90a5-5af18bc8157e
feature: Search Admin, Search Data Sources
source-git-commit: e16bc62127a708de8f4deb1eddfa53a14405cbc2
workflow-type: tm+mt
source-wordcount: '141'
ht-degree: 0%

---

# 부록 - 사용 가능한 [!DNL Google Analytics] 지표

제외를 제외한 다음 지표는 [!DNL Google Analytics]의 고객 구현에서 사용하도록 설정된 경우 사용할 수 있습니다.

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
>* [동기화 정보 [!DNL Google Analytics] 전환 지표](data-source-about.md)
>* [데이터 원본 [!DNL Google Analytics] 구성을 위한 필수 구성 요소](data-source-prerequisites.md)
>* [데이터 소스로  [!DNL Google Analytics] 보기 구성](data-source-configure.md)
>* [데이터 원본 편집 [!DNL Google Analytics] 2&rbrace;](data-source-edit.md)
>* [데이터 원본 동기화 일시 중지](data-source-pause.md)
>* [데이터 원본 다시 인증 [!DNL Google Analytics] 2&rbrace;](data-source-reauthenticate.md)
>* [[!DNL Google Analytics] 데이터 원본 설정](data-source-settings.md)
