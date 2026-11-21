---
title: '[!DNL ChatGPT] 광고 그룹 설정'
description: '[!DNL ChatGPT] 광고 그룹에 대한 설정을 참조합니다.'
feature: Search Campaign Management
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: aed5e38a-3e62-42fa-8d16-cd080729b2a0
    internal-label: Search, Social, & Commerce
subfeature_v2:
  - id: f3d33161-c519-436e-bbbd-730ba428736b
    internal-label: Campaign management
source-git-commit: 487af67f7215bf4a070af5e813649288141b0ed4
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 0%
---
# [!DNL ChatGPT] 광고 그룹 설정

[!DNL ChatGPT]의 *광고는[!DNL OpenAI]*&#x200B;의 파일럿 기능입니다.

## [!UICONTROL Basic Settings] 탭

*새 광고 그룹만*

**[!UICONTROL Network]:** 광고 네트워크입니다.

**[!UICONTROL Account]:** 광고 네트워크 계정입니다.

**[!UICONTROL Campaign]:** 캠페인입니다. 광고 그룹을 만든 후에는 캠페인을 변경할 수 없습니다.

## [!UICONTROL Ad Group Details] 탭

**[!UICONTROL Ad Group name]:** 캠페인 내에서 고유하며 최소 세 개의 문자가 포함된 광고 그룹 이름입니다.

**[!UICONTROL Status]:** 광고 그룹의 표시 상태: *[!UICONTROL Active]* 또는 *[!UICONTROL Paused]*. 새 광고 그룹의 기본값은 *[!UICONTROL Active]*&#x200B;입니다.

**[!UICONTROL Bid strategy]:**(목표 [!UICONTROL Clicks] 또는 [!UICONTROL Conversions]을(를) 가진 캠페인) 광고 그룹의 광고에 입찰하는 방법:

* *[!UICONTROL Autobid]:*(새 광고 그룹의 기본값) [!DNL OpenAI]은(는) 예산을 통해 캠페인 목표에 따라 클릭 수 또는 전환을 가장 많이 하도록 입찰을 자동으로 조정합니다. 입찰 금액을 입력하지 않았습니다. 이 옵션은 일간 및 라이프타임 캠페인 예산 모두에 사용할 수 있습니다.

* *[!UICONTROL Target CPC]:*(목표가 [!UICONTROL Clicks]인 캠페인)이 클릭당 평균 비용 목표를 향해 입찰합니다. [!UICONTROL Target CPC] 필드에 목표를 입력하십시오.

* *[!UICONTROL Target CPA]:*(목표가 [!UICONTROL Conversions]인 캠페인)이 전환당 평균 비용 목표를 향해 입찰합니다. [!UICONTROL Target CPA] 필드에 목표를 입력하십시오.

* *[!UICONTROL Manual: Max bid]:*(기존 수동으로 입찰한 광고 그룹만 해당) 기존 최대 입찰가를 읽기 전용 금액으로 유지합니다. 이 전략을 유지하거나 [!UICONTROL Autobid] 또는 캠페인 목표의 대상 전략으로 전환할 수 있습니다. 새 광고 그룹이나 이미 자동 입찰 또는 타겟 입찰을 사용하는 광고 그룹을 편집할 때에는 이 옵션을 사용할 수 없습니다.

기존의 수동 입찰 광고 그룹은 자동으로 다른 전략으로 변경되지 않습니다. 목표 금액 또는 관련 없는 설정만 편집해도 기존 목표 입찰 전략은 변경되지 않습니다.

**[!UICONTROL Target CPC]:**(입찰 전략이 [!UICONTROL Target CPC]인 광고 그룹, 필수) 달성하려는 클릭당 평균 비용(계정 통화 단위)입니다. 양수 금액을 입력합니다. 이는 평균 비용 목표이며 최대 입찰가는 아닙니다.

**[!UICONTROL Target CPA]:**(입찰 전략이 [!UICONTROL Target CPA]인 광고 그룹, 필수) 달성하려는 전환당 평균 비용(계정 통화 단위)입니다. 양수 금액을 입력합니다. 이는 평균 비용 목표이며 최대 입찰가는 아닙니다.

**[!UICONTROL Maximum CPC bid]:**(목표 [!UICONTROL Clicks]의 캠페인; 기존 수동 입찰 광고 그룹만 해당; 읽기 전용) 클릭당 지불할 기존 최대 금액입니다.

**[!UICONTROL Conversion-optimized bid cap]:**(목표 [!UICONTROL Conversions]의 캠페인; 기존 수동 입찰 광고 그룹만 해당; 읽기 전용) 전환을 위해 입찰할 기존 최대 금액입니다. [!DNL OpenAI]은(는) 예측된 전환율을 사용하여 이 값을 노출당 경매 입찰로 변환합니다.

**[!UICONTROL Maximum CPM bid]:**(목표 [!UICONTROL Reach]의 캠페인) 계정 통화로 표시된 1,000회 노출에 대해 지불할 최대 금액입니다. 0.01-5000 사이의 값을 입력합니다. 도달 캠페인에는 [!UICONTROL Bid strategy] 옵션이 없습니다.

**[!UICONTROL Context hints (optional)]:** 제품이나 서비스와 관련된 대화, 주제 또는 키워드에 대한 설명입니다. 쉼표 또는 줄 바꿈을 사용하여 힌트를 구분하십시오. 힌트를 사용하여 일치를 유도할 수 있지만 정확히 일치하는 타기팅 규칙은 아닙니다. 유효한 컨텍스트 힌트를 작성하는 방법에 대한 [[!DNL ChatGPT Ads] 도움말](https://help.openai.com/en/articles/20001211-create-ad-groups-for-chatgpt#writing-effective-context-hints)을 참조하세요.

**[!UICONTROL Landing Page Suffix]:**(선택 사항) 정보를 추적하기 위해 랜딩 페이지 URL의 끝에 추가할 모든 매개 변수입니다. 예: `param1=value1&param2=value2`

>[!MORELIKETHIS]
>
>* [광고 그룹 관리](ad-group-manage.md)
