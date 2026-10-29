---
title: '[!DNL ChatGPT Ads]개의 대화형 광고 캠페인 관리'
description: AI 비서 대화 내에 광고를 배치하는 Beta 기능인 [!DNL ChatGPT Ads] 캠페인, 광고 그룹 및 채팅 카드 광고를 만들고 관리하는 방법을 알아봅니다.
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
    internal-label: Demand Side Platform
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: cb25ab04e8fef5d00935e5325a897b1de97e2674
workflow-type: tm+mt
source-wordcount: '1188'
ht-degree: 0%
---
# [!DNL ChatGPT Ads]개의 대화형 광고 캠페인, 광고 그룹 및 광고 관리

*Beta 기능*

[대화 광고 계정](account-manage.md)에서 [!DNL ChatGPT Ads]개의 캠페인, 광고 그룹 및 채팅 카드 광고를 관리합니다.

다른 인보이스와 함께 월말에 [!DNL ChatGPT Ads] 사용량에 대한 청구됩니다. 청구 질문이 있는 경우 Adobe 계정 팀에 문의하십시오.

## [!UICONTROL Conversational Ads Beta] > [!UICONTROL Campaigns] 보기 {#campaign-views-about}

[!UICONTROL Conversational Ads Beta] > [!UICONTROL Campaigns] 보기에는 [!UICONTROL Campaigns], [!UICONTROL Ad Groups] 및 [!UICONTROL Ads]의 세 가지 탭이 있습니다. 각 탭에는 선택한 날짜 범위에 대한 성능 데이터와 함께 선택한 계정에 대한 캠페인, 광고 그룹 또는 광고가 나열됩니다. 캠페인, 광고 그룹 및 광고 수준의 성능 데이터에는 [!UICONTROL Impressions], [!UICONTROL Clicks], [!UICONTROL Spend], [!UICONTROL CTR], [!UICONTROL Avg CPC] 및 [!UICONTROL Avg CPM]이(가) 포함됩니다.

>[!NOTE]
>
>* 보고 보기에서 세금 값을 보도록 구성된 조직에서는 [!DNL ChatGPT Ads]에 대해 세금 값을 볼 수 없습니다. 세금 값을 수동으로 계산합니다.

### 사용 가능한 작업

<!-- * [Refresh information about your campaigns](#refresh) -- Add topic below. -->

* 캠페인 [만들기](#campaign-create) 또는 [편집](#campaign-edit)

* 기존 캠페인에 대한 광고 그룹을 [만들기](#ad-group-create) 또는 [편집](#ad-group-edit)

* 기존 광고 그룹에 대한 광고를 [만들기](#ad-create) 또는 [편집](#ad-edit)

* [캠페인, 광고 그룹 또는 광고 활성화 또는 일시 중지](#pause-activate)

* [캠페인, 광고 그룹 또는 광고 보관](#archive)

* [캠페인에서 광고 그룹 및 광고로 드릴다운](#drill-down)

* [캠페인, 광고 그룹 또는 광고 목록 새로 고침](#refresh)

## 캠페인

### [!DNL ChatGPT Ads] 대화형 광고 캠페인 만들기 {#campaign-create}

캠페인을 만들 때 선택적으로 첫 번째 광고 그룹 및 광고를 만들 수 있습니다. 각 단계에서는 **[!UICONTROL Next]**&#x200B;을(를) 클릭하는 즉시 해당 엔터티를 만들기 때문에 이전 단계로 돌아갈 수 없습니다. 이후에 변경해야 하는 경우에는 마법사를 닫은 후 해당 엔터티를 편집하십시오.

1. 주 메뉴에서 **[!UICONTROL Conversational Ads Beta]**&#x200B;을(를) 클릭합니다.

1. 하위 메뉴에서 **[!UICONTROL Campaigns]** 탭을 클릭합니다.

1. 오른쪽 상단에서 광고주와 [!DNL ChatGPT Ads] 계정을 선택합니다.

1. 오른쪽 상단에서 **[!UICONTROL Create]>[!UICONTROL Campaign]**&#x200B;을(를) 클릭합니다.

1. [캠페인 설정](#campaign-settings)을 지정하십시오.

1. **[!UICONTROL Next]**&#x200B;을(를) 클릭하여 캠페인 설정을 저장합니다.

1. 다음 중 하나를 수행합니다.

   * 캠페인에 대한 광고 그룹을 만들지 않으려면 **[!UICONTROL Close]**&#x200B;을(를) 클릭합니다.

     >[!TIP]
     >
     >나중에 광고 그룹 또는 광고를 만들려면 &quot;[광고 그룹 만들기](#ad-group-create)&quot; 또는 &quot;[광고 만들기](#ad-create)&quot;를 참조하십시오.

   * (선택 사항) 광고 그룹을 만듭니다.

     1. [광고 그룹 설정](#ad-group-settings)을 지정하십시오.

     1. 광고 그룹 설정을 저장하려면 **[!UICONTROL Next]**&#x200B;을(를) 클릭합니다.

     1. (선택 사항) 캠페인에 대한 광고를 만들지 않으려면 **[!UICONTROL Close]**&#x200B;을(를) 클릭합니다.

   * (광고 그룹을 만든 후 선택 사항) 광고를 만듭니다.

     1. [광고 설정](#ad-settings)을 지정하십시오.

     1. **[!UICONTROL Create ad]**&#x200B;을(를) 클릭합니다.

### [!DNL ChatGPT Ads] 대화형 광고 캠페인 설정 편집 {#campaign-edit}

1. 주 메뉴에서 **[!UICONTROL Conversational Ads Beta]**&#x200B;을(를) 클릭합니다.

1. 왼쪽의 하위 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 오른쪽 상단에서 광고주와 [!DNL ChatGPT Ads] 계정을 선택합니다.

1. (필요한 경우) 데이터 테이블 위에서 **[!UICONTROL Campaigns]** 탭을 클릭합니다.

1. 커서를 행 위에 놓고 **[!UICONTROL ...]>[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. [캠페인 설정](#campaign-settings), [광고 그룹 설정](#ad-group-settings) 및 [광고 설정](#ad-settings)을 편집합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

### [!DNL ChatGPT Ads] 대화형 광고 캠페인 설정 {#campaign-settings}

**[!UICONTROL Campaign name]:** 캠페인의 고유한 이름입니다. 이름에는 최소 3개의 문자가 포함되어야 합니다.

**[!UICONTROL Campaign type]:**(읽기 전용) *Standard*&#x200B;만 사용할 수 있습니다.

**[!UICONTROL Objective]:** 캠페인에 집중할 지표: *도달* 또는 *클릭 수*. 목표는 캠페인 광고 그룹에 대한 입찰 유형을 결정합니다.

**[!UICONTROL Locations]:**(선택 사항) 하나 이상의 특정 위치를 대상으로 합니다. 모든 위치를 타깃팅하려면 이 설정을 비워 둡니다. 특정 위치를 지정하려면 이름 내 아무 곳에나 나타나는 문자를 두 개 이상 입력한 다음 검색 결과 내에서 이름을 클릭합니다.

**[!UICONTROL Budget type]:** *일일 예산* 또는 *평생 예산*.

**[!UICONTROL Budget]:** 지정한 예산 유형에 대한 예산입니다. 값은 0보다 커야 합니다.

**[!UICONTROL Start date]:** 캠페인이 시작되는 날짜입니다(계정의 시간대).

**[!UICONTROL Set an end date]:**(선택 사항) 캠페인의 종료 날짜를 지정할 수 있습니다. 이 옵션을 선택하면 **[!UICONTROL End date]**&#x200B;을(를) 지정하십시오.

## 광고 그룹

### 기존 캠페인에 대한 [!DNL ChatGPT Ads] 광고 그룹 만들기 {#ad-group-create}

1. 주 메뉴에서 **[!UICONTROL Conversational Ads Beta]**&#x200B;을(를) 클릭합니다.

1. 하위 메뉴에서 **[!UICONTROL Campaigns]** 탭을 클릭합니다.

1. 오른쪽 상단에서 광고주와 [!DNL ChatGPT Ads] 계정을 선택합니다.

1. 오른쪽 상단에서 **[!UICONTROL Create]>[!UICONTROL Ad Group]**&#x200B;을(를) 클릭합니다.

1. 상위 캠페인을 포함하여 [광고 그룹 설정](#ad-group-settings)을 지정하십시오.

1. **[!UICONTROL Create ad group]**&#x200B;을(를) 클릭합니다.

## [!DNL ChatGPT Ads] 광고 그룹 편집 {#ad-group-edit}

1. 주 메뉴에서 **[!UICONTROL Conversational Ads Beta]**&#x200B;을(를) 클릭합니다.

1. 왼쪽의 하위 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 오른쪽 상단에서 광고주와 [!DNL ChatGPT Ads] 계정을 선택합니다.

1. 데이터 테이블 위에서 **[!UICONTROL Ad Groups]** 탭을 클릭합니다.

1. 커서를 행 위에 놓고 **[!UICONTROL ...]>[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. [광고 그룹](#ad-group-settings) 설정을 편집합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

### [!DNL ChatGPT Ads] 광고 그룹 설정 {#ad-group-settings}

**[!UICONTROL Parent campaign]:**(기존 캠페인에 대한 광고 그룹만 해당) 광고 그룹이 속한 캠페인입니다.

**[!UICONTROL Ad group name]:** 광고 그룹의 고유한 이름입니다. 이름에는 최소 3개의 문자가 포함되어야 합니다.

**[!UICONTROL Maximum CPC bid]** 또는 **[!UICONTROL Maximum CPM bid]:** 클릭당 또는 1,000회 노출 시 지불해야 하는 최대 금액입니다. 값은 0보다 커야 합니다. 캠페인의 목표는 입찰 필드를 결정합니다. *클릭 수* 캠페인은 **[!UICONTROL Maximum CPC bid]**&#x200B;을(를), *도달* 캠페인은 **[!UICONTROL Maximum CPM bid]**&#x200B;을(를) 표시합니다.

>[!TIP]
>
>더 높은 입찰가는 더 많은 경매를 얻을 수 있다.

**[!UICONTROL Context hints]:**(선택 사항) 제품이나 서비스와 관련된 대화, 주제 또는 키워드에 대한 설명입니다. 이러한 힌트는 일치를 안내하지만 정확히 일치하는 타기팅 규칙은 아닙니다.

## 광고

### 기존 광고 그룹에 대한 [!DNL ChatGPT Ads] 채팅 카드 광고 만들기 {#ad-create}

1. 주 메뉴에서 **[!UICONTROL Conversational Ads Beta]**&#x200B;을(를) 클릭합니다.

1. 하위 메뉴에서 **[!UICONTROL Campaigns]** 탭을 클릭합니다.

1. 오른쪽 상단에서 광고주와 [!DNL ChatGPT Ads] 계정을 선택합니다.

1. 오른쪽 상단에서 **[!UICONTROL Create]>[!UICONTROL Ad]**&#x200B;을(를) 클릭합니다.

1. 상위 캠페인 및 광고 그룹을 포함하여 [광고 설정](#ad-settings)을 지정하십시오.

1. **[!UICONTROL Create ad]**&#x200B;을(를) 클릭합니다.

## [!DNL ChatGPT Ads] 채팅 카드 광고 편집 {#ad-edit}

1. 주 메뉴에서 **[!UICONTROL Conversational Ads Beta]**&#x200B;을(를) 클릭합니다.

1. 왼쪽의 하위 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 오른쪽 상단에서 광고주와 [!DNL ChatGPT Ads] 계정을 선택합니다.

1. 데이터 테이블 위에서 **[!UICONTROL Ads]** 탭을 클릭합니다.

1. 커서를 행 위에 놓고 **[!UICONTROL ...]>[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. [ad](#ad-settings) 설정을 편집합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

### [!DNL ChatGPT Ads] 채팅 카드 광고 설정 {#ad-settings}

**[!UICONTROL Parent campaign]** 및 **[!UICONTROL Parent ad group]:**(기존 광고 그룹의 광고만 해당) 광고가 속한 캠페인 및 광고 그룹입니다.

**[!UICONTROL Ad name]:** 광고의 고유한 이름입니다. 이름에는 최소 3개의 문자가 포함되어야 합니다.

**[!UICONTROL Ad URL (Link)]:** `http://` 또는 `https://`(으)로 시작하는 랜딩 페이지 URL.

**[!UICONTROL Title (headline)]:** 광고 헤드라인입니다. 제목은 3~50자 사이여야 합니다. **참고:** 일부 배치 유형에서는 제목이 잘릴 수 있습니다.

**[!UICONTROL Description]:** 광고 본문입니다. 설명은 3~100자 사이여야 합니다.

**[!UICONTROL Ad image]:** 광고에 포함할 JPG 또는 PNG 이미지입니다. 이미지를 업로드하려면 (새 광고) **[!UICONTROL Upload image (PNG/JPG)]** 또는 **[!UICONTROL Change image]**&#x200B;을(를) 클릭한 다음 장치 또는 네트워크에서 파일을 찾아 선택합니다.

**[!UICONTROL Preview]:** 광고 설정을 기반으로 하는 광고 미리 보기입니다.

## [!DNL ChatGPT Ads] 캠페인, 광고 그룹 또는 광고 활성화 또는 일시 중지 {#pause-activate}

1. 주 메뉴에서 **[!UICONTROL Conversational Ads Beta]**&#x200B;을(를) 클릭합니다.

1. 왼쪽의 하위 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 오른쪽 상단에서 광고주와 [!DNL ChatGPT Ads] 계정을 선택합니다.

1. **[!UICONTROL Campaigns]**, **[!UICONTROL Ad Groups]** 또는 **[!UICONTROL Ads]** 탭에서 행을 찾습니다.

1. **[!UICONTROL Active]** 열에서 다음 중 하나를 실행하십시오.

   * 일시 중지된 항목을 활성화하려면 토글(오른쪽)을 켭니다.

   * 활성 항목을 일시 중지하려면 토글을 끕니다(왼쪽).

## [!DNL ChatGPT Ads] 캠페인, 광고 그룹 또는 광고 보관 {#archive}

보관하면 [!UICONTROL Conversational Ads] 보기에서 캠페인, 광고 그룹 또는 광고가 영구적으로 제거됩니다.

1. 주 메뉴에서 **[!UICONTROL Conversational Ads Beta]**&#x200B;을(를) 클릭합니다.

1. 왼쪽의 하위 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 오른쪽 상단에서 광고주와 [!DNL ChatGPT Ads] 계정을 선택합니다.

1. **[!UICONTROL Campaigns]**, **[!UICONTROL Ad Groups]** 또는 **[!UICONTROL Ads]** 탭에서 행 위에 커서를 놓고 **[!UICONTROL ...]>[!UICONTROL Archive]**&#x200B;을(를) 클릭합니다.

## [!DNL ChatGPT Ads] 캠페인에서 광고 그룹 및 광고로 드릴다운 {#drill-down}

* 캠페인 행을 클릭하여 **[!UICONTROL Ad Groups]** 탭에서 해당 광고 그룹만 보거나 광고 그룹 행을 클릭하여 **[!UICONTROL Ads]** 탭에서 해당 광고만 봅니다.

필터를 제거하고 보기의 모든 행을 보려면 데이터 테이블 위의 필터에서 **X**&#x200B;을(를) 클릭합니다.

## 캠페인, 광고 그룹 또는 광고 목록 새로 고침 {#refresh}

다른 사용자가 변경하거나 추가했을 수 있는 경우 캠페인, 광고 그룹 또는 광고 목록을 다시 표시합니다.

1. 주 메뉴에서 **[!UICONTROL Conversational Ads Beta]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Campaigns]**, **[!UICONTROL Ad Groups]** 또는 **[!UICONTROL Ads]** 보기에서 데이터 테이블 위의 **[!UICONTROL Refresh]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [대화 광고 계정 관리](account-manage.md)
