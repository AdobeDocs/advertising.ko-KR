---
title: 캠페인 복제
description: 캠페인을 복제하는 방법을 알아봅니다.
feature: DSP Campaigns
exl-id: 4e42bd5b-e8a9-45be-af5c-367c48d0b131
source-git-commit: 443f8907644bf3e480626e14713e8abb9bfca284
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 0%

---

# 캠페인 복제

<!-- Some placements don't have this option. Clarify which placement types aren't eligible -- is it PG placements, or all placements using private inventory? And anything else? -->

유사한 설정으로 새 캠페인을 만들려면 캠페인을 복제합니다. 다음을 수행할 수 있습니다.

* 원래 광고주 또는 다른 광고주에 대한 캠페인을 복제합니다
* 원할 경우 원본 패키지 및 배치를 복제합니다
* 새 캠페인의 플라이트 날짜 수정

참조:[복제되지 않은 사항](#campaign-not-duplicated)중복되지 않은 배치 설정 목록입니다.

1. 주 메뉴에서 **[!UICONTROL Campaigns]**.

1. 캠페인 이름 옆의 **[!UICONTROL ...]** > **[!UICONTROL Duplicate]**.

1. 새 캠페인 설정을 지정합니다.

   1. 새 캠페인 이름과 종료 플라이트 날짜를 입력합니다.

   1. (선택 사항) 기본 설정을 변경합니다.

      기본적으로 새 캠페인은 원래 광고주에게 할당되며, 현재 날짜부터 시작하는 플라이트 일정을 가지며, 원래 패키지와 배치를 포함합니다.

1. 클릭 **[!UICONTROL Submit]**.

## 복제되지 않은 사항 {#campaign-not-duplicated}

다음을 제외하고 원래 배치의 모든 설정이 복제됩니다.

* 실험 설정
* (플라이트 날짜를 변경하는 경우) 사용자 지정 광고 예약
* (광고를 첨부하지 않는 경우) 사용자 지정 광고 가중치 및 예약
* 의 프로그래밍 방식 보장(PG) 거래 및 배치에 대한 기본 배치 [!UICONTROL Simple Ad Serving] 거래
* (배치를 다른 캠페인에 복사하는 경우):
   * 지역 타겟
   * 이벤트 픽셀
   * 광고
   * 배치 수준 [!DNL DoubleVerify Authentic Brand Safety] 세그먼트(광고주 수준 세그먼트를 재정의하는 세그먼트)

>[!MORELIKETHIS]
>
>* [Campaign Management 정보](campaign-about.md)
>* [캠페인 만들기](campaign-create.md)
>* [캠페인 편집](campaign-edit.md)
>* [캠페인 설정](campaign-settings.md)

