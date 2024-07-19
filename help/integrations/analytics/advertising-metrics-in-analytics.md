---
title: Analysis Workspace에서 지표 Adobe Advertising
description: Analysis Workspace에서 지표 Adobe Advertising
feature: Integration with Adobe Analytics
exl-id: da5e5704-4504-4fc5-93d2-db7d28f0c349
source-git-commit: da69280679a4e0c5ce04f55ee94ce984745395ff
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# Analysis Workspace에서 지표 Adobe Advertising

*Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

>[!NOTE]
>
>* Adobe Advertising이 트래픽 지표 및 차원을 매일 [!DNL Analytics]에 전달합니다.
>* [!DNL Analytics]은(는) Adobe Advertising 클릭스루 및 뷰스루를 실시간으로 캡처합니다.
>* [!DNL Search, Social, & Commerce]의 경우 이 기능은 대부분의 광고 네트워크 및 캠페인 유형에 대해 지원됩니다. 자세한 내용은 [!DNL Search, Social, & Commerce] 안내서의 &quot;[지원되는 인벤토리](/help/search-social-commerce/introduction/supported-inventory.md)&quot;을(를) 참조하십시오.

## Adobe Advertising의 트래픽 지표

[!DNL Analytics]의 Adobe Advertising 트래픽 지표는 일반적으로 &quot;[!UICONTROL AMO ID Instances]&quot;을(를) 제외하고 &quot;Adobe Advertising&quot;로 시작합니다. 그러나 예약된 이벤트가 아닌 사용자 지정 이벤트를 사용하여 원래 클릭, 비용 및 노출에 대한 지표를 만든 장기 고객의 경우 해당 지표는 여전히 &quot;AMO&quot;로 시작합니다.

| 트래픽 지표 | 설명 |
| -------------- | ----------- |
| [!UICONTROL Adobe Advertising Clicks] 또는 (일부 이전 고객) [!UICONTROL AMO Clicks] | 총 Adobe Advertising 클릭 수입니다. |
| [!UICONTROL Adobe Advertising Cost] 또는 (일부 이전 고객) [!UICONTROL AMO Cost] | Adobe Advertising은 보고서 세트의 통화로 지출합니다. |
| [!UICONTROL Adobe Advertising Impressions] 또는 (일부 이전 고객) [!UICONTROL AMO Impressions] | Adobe Advertising 노출 횟수입니다. |
| [!UICONTROL Adobe Advertising Measurable Impressions] | 조회 계측을 성공적으로 초기화하기 위해 제공된 노출 횟수입니다. 이 값은 (계측된 노출 횟수 - 측정할 수 없는 노출 횟수)로 계산됩니다. |
| [!UICONTROL Adobe Advertising Minutes Viewed] | Adobe Advertising 비디오를 본 시간(분)입니다. |
| [!UICONTROL Adobe Advertising Not Viewable Impressions] | 볼 수 없는 것으로 결정된 노출 횟수입니다. 이 값은 ([!UICONTROL Adobe Advertising Measurable Impressions] - [!UICONTROL Adobe Advertising Viewable])로 계산됩니다. |
| [!UICONTROL Adobe Advertising Viewable Impressions] | 배치 구성에 따라 볼 수 있도록 측정된 노출 횟수. |
| [!UICONTROL Adobe Advertising Views] | 광고에 대한 보기 횟수입니다. 뷰어는 뷰어가 Adobe Advertising 비디오를 시작할 때 카운트됩니다. |
| [!UICONTROL Adobe Advertising Views 25% Complete] | Adobe Advertising 비디오를 25% 이상 시청한 보기 횟수. |
| [!UICONTROL Adobe Advertising Views 50% Complete] | Adobe Advertising 비디오를 50% 이상 시청한 보기 횟수. |
| [!UICONTROL Adobe Advertising Views 75% Complete] | Adobe Advertising 비디오를 75% 이상 시청한 보기 횟수. |
| [!UICONTROL Adobe Advertising Views 100% Complete] | Adobe Advertising 비디오를 100% 시청한 보기 횟수. |
| [!UICONTROL AMO ID Instances] | [!UICONTROL AMO ID]이(가) 설정된 횟수입니다. |

## Adobe Advertising Dimension

>[!NOTE]
>
>[!DNL Analytics]의 모든 Adobe Advertising 차원 뒤에 &quot;[!DNL (AMO ID)]&quot;이(가) 있습니다.

| 차원 | 적용 가능한 Adobe Advertising 데이터 | 설명 |
| ----------- | ---------- | ---------- |
| [!UICONTROL Ad Platform (AMO ID)] | [!DNL DSP] 및 [!DNL Search, Social, & Commerce] 데이터 | Advertising DSP 또는 검색 엔진 이름 |
| [!UICONTROL Account (AMO ID] | [!DNL DSP] 및 [!DNL Search, Social, & Commerce] 데이터 | 계정 이름. |
| [!UICONTROL Network (AMO ID)] | [!DNL DSP] 및 [!DNL Search, Social, & Commerce] 데이터 | RTB([!DNL DSP]) 또는 광고 네트워크 이름([!DNL Search, Social, & Commerce]) |
| [!UICONTROL Campaign (AMO ID)] | [!DNL DSP] 및 [!DNL Search, Social, & Commerce] 데이터 | 캠페인 이름. |
| [!UICONTROL Optimization (AMO ID)] | [!DNL DSP] 및 [!DNL Search, Social, & Commerce] 데이터 | 패키지([!DNL DSP]) 또는 포트폴리오([!DNL Search, Social, & Commerce]) 이름입니다. |
| [!UICONTROL Placement (AMO ID)] | [!DNL DSP] 데이터 | 배치 이름입니다. |
| [!UICONTROL Ad Group (AMO ID)] | [!DNL Search, Social, & Commerce] 데이터 | 광고 그룹 이름입니다. |
| [!UICONTROL Keyword (AMO ID)] | [!DNL Search, Social, & Commerce] 데이터 | 키워드. |
| [!UICONTROL Match Type (AMO ID)] | [!DNL Search, Social, & Commerce] 데이터 | 검색 일치 유형입니다. |
| [!UICONTROL Keyword Match Type (AMO ID)] | [!DNL Search, Social, & Commerce] 데이터 | 키워드 및 일치 유형입니다. |
| [!UICONTROL Ad Type (AMO ID)] | [!DNL DSP] 및 [!DNL Search, Social, & Commerce] 데이터 | 광고 유형(예: `text`, `video`, `display` 또는 `native`). |
| [!UICONTROL Ad Title (AMO ID)] | [!DNL DSP] 및 [!DNL Search, Social, & Commerce] 데이터 | 광고 유형([!DNL DSP]) 또는 광고 제목([!DNL Search, Social, & Commerce])입니다. |
| [!UICONTROL Ad Description (AMO ID)] | [!DNL DSP] 및 [!DNL Search, Social, & Commerce] 데이터 | 광고 설명([!DNL DSP]) 또는 광고 본문([!DNL Search, Social, & Commerce])입니다. |
| [!UICONTROL Ad Display URL (AMO ID)] | [!DNL Search, Social, & Commerce] 데이터 | 광고에 표시되는 URL. |
| [!UICONTROL Ad Destination URL (AMO ID)] | [!DNL Search, Social, & Commerce] 데이터 | 광고의 대상 URL입니다. |
| [!UICONTROL Landing Type (AMO ID)] | [!DNL DSP] 및 [!DNL Search, Social, & Commerce] 데이터 | 랜딩 페이지 항목이 뷰스루인지 또는 클릭스루인지 여부를 나타냅니다. |
| [!UICONTROL Product Target (AMO ID)] | [!DNL Search, Social, & Commerce] 데이터 | 제품 목록 광고에 대한 제품 타겟. |

## Adobe Advertising에 유용한 사용자 지정 계산된 지표

Adobe Advertising 데이터에 대해 다음 지표를 만드는 것이 좋습니다.

* 랜딩 페이지 인스턴스 클릭 수([!UICONTROL AMO ID Instances] / [!UICONTROL Adobe Advertising Clicks]): 광고를 클릭하여 랜딩 페이지로 이동한 사용자의 비율입니다.
* 측정 가능한 비율([!UICONTROL Adobe Advertising Viewable Impressions] / [!UICONTROL Adobe Advertising Impressions] * 100)
* 볼 수 있는 노출률([!UICONTROL Adobe Advertising Viewable Impressions] / [!UICONTROL Adobe Advertising Measureable Impressions] * 100)
* 보당 비용([!UICONTROL Adobe Advertising Cost] / [!UICONTROL Adobe Advertising Views])
* 클릭당 비용([!UICONTROL Adobe Advertising Cost] / [!UICONTROL Adobe Advertising Clicks])

>[!MORELIKETHIS]
>
>* [개요 [!DNL Analytics for Advertising]](overview.md)
>* [[!DNL Analytics] Adobe Advertising의 데이터](/help/integrations/analytics/analytics-data-in-advertising.md)
