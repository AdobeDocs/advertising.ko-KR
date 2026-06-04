---
title: (새 UI) Microsoft Advertising에서 Google 광고 캠페인을 복제합니다
description: Google Ads 계정의 동기화된 캠페인을 동기화된 Microsoft Advertising 계정으로 직접 내보내는 방법에 대해 알아봅니다.
feature: Search Campaign Management
source-git-commit: e6649d66757333660662a058410221b73a45e6cc
workflow-type: tm+mt
source-wordcount: '962'
ht-degree: 0%

---

# (새 UI) [!DNL Microsoft Advertising]에서 [!DNL Google Ads] 캠페인 복제

*Beta 기능*

[!DNL Google Ads] 계정의 동기화된 캠페인을 eCPC(향상된 CPC) 캠페인으로 동기화된 [!DNL Microsoft Advertising] 계정으로 직접 내보낼 수 있습니다. 기존 입찰 및 캠페인 예산의 크기가 조정됩니다. 기존 검색, 소셜 및 Commerce 추적은 가져오지 않습니다.

다음 유형의 캠페인과 해당 캠페인 구조를 복제할 수 있습니다.

* [!DNL Google Ads] 검색 및 표시 캠페인을 [!DNL Microsoft Advertising] 검색 및 표시 캠페인으로 보냅니다.

* Microsoft Audience Network의 [!DNL Microsoft Advertising] 대상 캠페인에 광고 이미지를 포함한 [!DNL Google Display Network] 캠페인.

  쇼핑 피드 기반 표시 캠페인을 복제하려면 먼저 [!DNL Google Merchant Center] 제품 오퍼를 [!DNL Microsoft Merchant Center]에 복제하십시오. 캠페인을 복제할 때 가져오기 옵션에서 [!DNL Microsoft Merchant Center] 스토어를 선택하여 스토어를 피드 기반 대상 캠페인에 연결합니다.

* [!DNL Google Ads] 성과 최대 캠페인(로컬 인벤토리 광고 포함)을 [!DNL Microsoft Advertising] 성과 최대 캠페인으로 전환합니다.

캠페인을 매일, 매주 또는 매월 한 번 업데이트하거나 [!DNL Microsoft Advertising]의 권장 일정에 따라 업데이트하도록 선택할 수 있습니다. 선택적으로 가져오기 작업이 실행될 때마다 또는 오류나 변경 사항이 발생할 때 알림을 구성할 수 있습니다. 캠페인을 [!DNL Microsoft Advertising]&#x200B;(으)로 가져오면 가져오기 작업의 상태를 확인하고 오류 로그를 검토하며 가져오기 작업을 수동으로 실행하고 가져오기 일정을 편집, 일시 중지, 활성화 또는 삭제할 수 있습니다.

일부 캠페인 정보는 복제되지 않으며 [!DNL Microsoft Advertising] 캠페인에 일부 정보를 추가해야 할 수 있습니다. 가져온 데이터에 대한 자세한 내용은 &quot;[가져온 항목 [!DNL Google Ads]](https://help.ads.microsoft.com/#apex/ads/en/50851){target="_blank"}&quot;에 대한 [!DNL Microsoft Advertising] 도움말을 참조하십시오. 검색, 소셜 및 Commerce 추적을 가져오지 않았으므로 [account](/help/search-social-commerce/campaign-management/accounts/ad-network-account-manage.md), [campaign](/help/search-social-commerce/campaign-management/campaigns/campaign-manage.md), [광고 그룹](/help/search-social-commerce/campaign-management/campaigns/ad-group-manage.md) 또는 [ad](/help/search-social-commerce/campaign-management/campaigns/ad-manage.md) 설정 내에서도 추적을 추가해야 합니다.

## [!DNL Google Ads]개 캠페인 복제

>[!NOTE]
>
>쇼핑 피드 기반 표시 캠페인을 복제하려면 먼저 [내 [!DNL Google Merchant Center] 제품 오퍼를 복제합니다 [!DNL Microsoft Merchant Center]](https://help.ads.microsoft.com/apex/index/3/en/56870){target="_blank"}. 캠페인을 복제할 때 가져오기 옵션에서 [!DNL Microsoft Merchant Center] 스토어를 선택하여 스토어를 피드 기반 대상 캠페인에 연결합니다.

[가져온 항목 [!DNL Google Ads] 캠페인](https://help.ads.microsoft.com/#apex/ads/en/50851/0-500){target="_blank"}을 참조하세요.

1. 주 메뉴에서 **[!UICONTROL Setup]** \> **[!UICONTROL Import Campaigns]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Import Campaigns]**&#x200B;을(를) 클릭합니다.

1. [가져오기 설정](#campaign-import-settings)을 지정하십시오.

1. 오른쪽 상단의 **[!UICONTROL Review and Save]**&#x200B;을(를) 클릭합니다.

1. 요약에서 선택 내용을 검토하고 **[!UICONTROL Start Import]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) [account](/help/search-social-commerce/new-ui/set-up/accounts/api-accounts/api-account-manage.md), [campaign](/help/search-social-commerce/campaign-management/campaigns/campaign-manage.md), [광고 그룹](/help/search-social-commerce/campaign-management/campaigns/ad-group-manage.md) 또는 [ad](/help/search-social-commerce/campaign-management/campaigns/ad-manage.md) 설정 내에서 검색, 소셜 및 Commerce 추적을 추가합니다.

## 캠페인 가져오기 작업에 대한 일정 설정 편집

[가져온 항목 [!DNL Google Ads] 캠페인](https://help.ads.microsoft.com/#apex/ads/en/50851/0-500){target="_blank"}을 참조하세요.

1. 주 메뉴에서 **[!UICONTROL Setup]** \> **[!UICONTROL Import Campaigns]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL List of Import Jobs]** 탭에서 가져오기 작업의 이름을 클릭한 다음 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Set schedule]** 단계에서 [예약 설정](#campaign-import-settings)을 지정하십시오.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 캠페인 가져오기 작업 보기

원본 [!DNL Google Ads] 계정, 대상 [!DNL Microsoft Advertising] 계정, 가져오기 시간 또는 일정, 작업을 만든 사용자를 포함하여 모든 가져오기 작업을 나열할 수 있습니다. 정기적으로 예약된 가져오기 작업을 포함하여 가져오기 작업을 여러 번 실행하면 각 항목이 별도의 작업으로 나열됩니다.

1. 주 메뉴에서 **[!UICONTROL Setup]** \> **[!UICONTROL Import Campaigns]**&#x200B;을(를) 클릭합니다.

   기본적으로 **[!UICONTROL List of Import Jobs]** 탭이 열립니다.

## 캠페인 가져오기 작업 실행

1. 주 메뉴에서 **[!UICONTROL Setup]** \> **[!UICONTROL Import Campaigns]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL List of Import Jobs]** 탭에서 가져오기 작업 옆의 확인란을 선택한 다음 **[!UICONTROL Run Now]**&#x200B;을(를) 클릭합니다.

## 캠페인 가져오기 작업에 대한 로그 보기 {#campaign-import-log}

시작 시간, 원본 [!DNL Google Ads] 계정, 대상 [!DNL Microsoft Advertising] 계정, 작업을 만든 사용자, 성공한 작업 및 실패한 작업 수, 각 작업에 대한 알림을 받은 전자 메일 주소를 포함하여 완료되거나 실패한 모든 가져오기 작업을 나열할 수 있습니다. 추가, 동기화, 삭제된 항목 수, 계정의 각 엔터티 수준(예: 캠페인 또는 키워드)에 대한 오류를 생성한 항목 수 등 각 작업에 대해 발생한 대상 [!DNL Microsoft Advertising] 계정의 변경 사항에 대한 자세한 내용을 볼 수 있습니다.

1. 주 메뉴에서 **[!UICONTROL Setup]** \> **[!UICONTROL Import Campaigns]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Import Logs]** 탭을 클릭합니다.

1. (선택 사항) 가져오기 작업에 대한 세부 정보를 보려면 [!UICONTROL Summary] 열의 값을 클릭합니다.

## 캠페인 가져오기 작업 설정 {#campaign-import-settings}

### [!UICONTROL Select Accounts] 탭

**[!UICONTROL Import Name]:** 가져오기 작업을 식별하는 이름입니다.

**[!UICONTROL Source Google Ads account]:** 캠페인 데이터를 내보내는 동기화된 [!DNL Google Ads] 계정입니다.

**[!UICONTROL Target Microsoft Ads account]:** 캠페인 데이터를 가져오는 동기화된 [!DNL Microsoft Advertising] 계정입니다.

**[!UICONTROL Credential ID]:** [!DNL Microsoft Advertising]에서 [!DNL Google Ads] 자격 증명을 나타내는 데 사용하는 ID입니다. [!DNL Microsoft Advertising] 제한 사항으로 인해 가져오기용 [!DNL Microsoft Advertising] 자격 증명의 자동 생성을 사용할 수 없습니다. Adobe 계정 팀에 문의하여 자격 증명을 생성하고 ID를 제공합니다.

### [!UICONTROL Select Campaigns & Ad Groups] 탭

**\[가져올 데이터\]:** 가져올 데이터:

* *[!UICONTROL Import all new and existing campaigns]:* 이미 존재하는 모든 캠페인과 [!DNL Microsoft Advertising]에 존재하지 않는 캠페인에 대한 데이터를 가져옵니다.

* *[!UICONTROL Import specific campaigns and adgroups]:* 특정 캠페인 및 광고 그룹을 선택합니다.

   * 캠페인을 하위 광고 그룹으로 확장하려면 캠페인 이름 뒤에 있는 **[!UICONTROL >]**&#x200B;을(를) 클릭합니다.

   * 캠페인 또는 광고 그룹을 선택하려면 확인 표시가 나타나도록 항목을 선택합니다.

   * 캠페인 또는 광고 그룹을 제거하려면 항목을 선택 취소하거나 [!UICONTROL Selection] 열에서 ![삭제](/help/search-social-commerce/assets/delete-new.png "삭제")를 클릭하십시오.

### [!UICONTROL Customize Your Import] 탭

**[!UICONTROL Choose specific import options]:** 가져올 항목, 입찰 및 예산 및 기타 옵션을 지정할 수 있습니다.

**[!UICONTROL What to import]:** 가져올 항목을 정의합니다. 기본적으로 항목 범주를 가져오는 옵션이 선택되고 모든 항목 유형이 선택됩니다. 특정 항목 형식만 포함하려면 **[!UICONTROL Show advanced options]**&#x200B;을(를) 클릭하고 포함할 항목 형식을 변경하십시오. 선택적으로 UET 태그 ID를 [!DNL Microsoft Advertising]&#x200B;(으)로 이전에 가져오지 않은 리마케팅 목록 또는 대상자와 연결할 수도 있습니다.

**[!UICONTROL Bids and budgets]:** 가져오기, 업데이트 및 사용자 지정할 입찰 및 예산 설정을 정의합니다. 여기에는 [!DNL Microsoft Advertising]에 대해 지정한 비율만큼 입찰 및 예산을 늘리거나 줄이는 옵션이 포함됩니다.

**[!UICONTROL Other options]:** 가져온 랜딩 페이지 URL, 추적 템플릿, 기타 캠페인, 광고 및 타깃팅 옵션(텍스트 찾기 및 바꾸기 및 접미사 삽입 옵션 포함)을 처리하는 방법을 정의합니다.

### [!UICONTROL Set Schedule] 탭

**[!UICONTROL When]:** 지정된 캠페인을 가져올 시기: *자동*([!DNL Microsoft Advertising]이(가) 캠페인을 최적화하기 위해 일정을 설정하도록 허용), *[!UICONTROL Now]*(작업 설정을 게시할 때 작업 실행), 지정된 시간에 *[!UICONTROL Once]*, 지정된 시간에 *[!UICONTROL Daily]*, 지정된 시간에 *[!UICONTROL Weekly]* 또는 지정된 시간에 *[!UICONTROL Monthly]*.

**[!UICONTROL Receive email notifications]:** 가져오기 작업에 대한 이메일 알림을 [!UICONTROL Send reports to] 필드의 주소로 전송할지 여부 및 전송 시기: *[!UICONTROL No emails]*, *[!UICONTROL Only if there are changes or errors]*(기본값), *[!UICONTROL Only if there are errors]* 또는 *[!UICONTROL Every time this import runs]*.

가져오기 작업에 대한 알림을 받을 **[!UICONTROL Send reports to]:** 이메일 주소. 여러 주소는 쉼표(`,`)로 구분하십시오.

>[!MORELIKETHIS]
>
>* [광고 네트워크 계정 관리](/help/search-social-commerce/new-ui/set-up/accounts/api-accounts/api-account-manage.md)
