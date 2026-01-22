---
title: 일괄 시트 파일을 사용하여 포트폴리오 설정 일괄 편집
description: 일괄 시트 파일을 사용하여 여러 포트폴리오의 설정을 편집하는 방법에 대해 알아봅니다.
feature: Search Portfolios, Search Optimization
hide: true
exl-id: 20f7419d-9f5e-4477-ae8d-8b85a79b1e81
source-git-commit: 04b6fbaf4a8b360bc3a60bdad4871694d50f1bf9
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# 일괄 시트 파일을 사용하여 포트폴리오 설정 일괄 편집

*Beta 기능*

포트폴리오 일괄 시트 는 특정 형식의 포트폴리오 설정이 포함된 파일로, 설정을 빠르게 검토하고 수정하는 데 사용할 수 있습니다. 하나 이상의 포트폴리오에 대한 설정이 있는 일괄 시트를 생성(다운로드)할 수 있습니다. 이 파일은 두 개의 워크시트(XLSX 형식)가 있는 [!DNL Excel] 통합 문서로 다운로드됩니다. 통합 문서에는 다음이 포함됩니다.

* 필드 편집에 대한 정보가 포함된 읽기 전용 [!UICONTROL Instructions] 워크시트입니다.

* 포함된 포트폴리오당 하나의 행이 있는 [!UICONTROL Portfolio Settings Edit] 탭입니다. 필요에 따라 필드를 편집하고, 로컬에 파일을 저장한 다음 [편집된 파일을 업로드](#portfolio-bulksheet-upload)하여 검색, 소셜 및 Commerce에 추가할 수 있습니다. 편집 가능한 필드는 색상으로 강조 표시됩니다.

## 포트폴리오 설정이 있는 일괄 시트 파일 다운로드

1. (선택 사항) 일괄 시트에 포함할 각 포트폴리오 옆에 있는 확인란을 선택합니다.

   특정 포트폴리오를 선택하지 않으면 모든 포트폴리오에 대한 설정을 다운로드할 수 있습니다.

1. 데이터 테이블 위의 도구 모음에서 다음 을 클릭합니다.

   * (모든 포트폴리오의 경우) **[!UICONTROL Bulk Operations]** > **[!UICONTROL Export All Portfolios]**.

   * (선택한 포트폴리오의 경우) **[!UICONTROL Bulk Operations]** > **[!UICONTROL Export Selected Portfolios]**.

1. 만들 일괄 시트 파일의 이름을 입력한 다음 **[!UICONTROL Export Now]**&#x200B;을(를) 클릭합니다.

   파일은 브라우저의 기본 다운로드 폴더에 저장됩니다.

## 업데이트된 포트폴리오 설정으로 일괄 시트 파일 업로드 {#portfolio-bulksheet-upload}

파일은 XLSX 형식이어야 합니다.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL Bulk Operations]** > **[!UICONTROL Import Portfolio Details]**&#x200B;을(를) 클릭합니다. &lt;!— &quot;Portfolio 설정 가져오기&quot;여야 합니다. — &quot;세부 정보&quot;는 너무 모호할 수 있으며 다른 내용이 포함되어 있을 수 있습니다. —>

1. [!UICONTROL Import Portfolio Details File] 대화 상자:<!-- reword if we change the name of the operation -->

   1. 파일을 상자로 끌어다 놓거나 **[!UICONTROL Browse File]**<!-- "Browse for file" or just "Browse"??? -->을(를) 클릭하여 장치나 네트워크에서 파일을 선택합니다.

   1. **[!UICONTROL Import]**&#x200B;을(를) 클릭합니다.

날짜 범위 선택기 옆에 있는 [!UICONTROL Global Sync Status] 단추(![전역 동기화 상태](/help/search-social-commerce/assets/global-sync-status.png "전역 동기화 상태"))에서 업로드 상태를 확인할 수 있습니다.<!-- icon similar to Refresh -->. 실패한 변경 사항이 있으면 실패한 항목을 보여 주는 오류 파일을 다운로드할 수 있습니다.

알림도 알림 센터에 추가되며 ![ 단추(](/help/search-social-commerce/assets/notifications-new.png ") 옆에 있는 ")알림[!UICONTROL Global Sync Status]알림![전역 동기화 상태](/help/search-social-commerce/assets/global-sync-status.png "전역 동기화 상태") 아이콘에서 알림 창을 열 수 있습니다.

## 업로드된 일괄 시트 파일에 대한 데이터 요구 사항

모든 일괄 시트 파일에는 열 [!UICONTROL Portfolio ID]이(가) 포함되어야 하며, 각 데이터 행에는 [!UICONTROL Portfolio ID]을(를) 실행할 수 있는 값이 포함되어야 합니다. 데이터 요구 사항에 대한 자세한 내용은 다운로드한 일괄 시트 파일의 [!UICONTROL Instructions] 탭을 참조하십시오.

[!UICONTROL Portfolio Settings Edit] 탭의 포트폴리오 설정 열에 대한 자세한 내용은 Search, Social 및 Commerce 내에서 사용할 수 있는 최적화 안내서를 참조하십시오.

<!--
## Data fields on the [!UICONTROL Portfolio Settings Edit] tab

| Field | Required to import data? | Description |
| ----- | ------------------------ | ----------- |
| Portfolio ID |  |  |
| Portfolio Name |  |  |
| Status |  |  |
| Spend Strategy |  |  |
| Target |  |  |
| Hybrid |  |  |
| Auto adjust campaign budgets |  |  |
| Spend Multiple |  |  |
| Minimum Campaign Budget |  |  |
| Objective |  |  |
| Cost Half-Life |  |  |
| Revenue Half-Life |  |  |
| Min. Target CPA |  |  |
| Max. Target CPA |  |  |
| Min. Target ROAS |  |  |
| Max. Target ROAS |  |  |

-->

>[!MORELIKETHIS]
>
>* [(새 UI) 포트폴리오 편집](portfolio-edit.md)
>* [포트폴리오 만들기](portfolio-create.md)
>* 포트폴리오에 대한 [(새 UI)](portfolio-about.md)
