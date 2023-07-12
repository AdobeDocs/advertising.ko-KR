---
title: 복제 [!DNL Google Ads] 의 캠페인 [!DNL Microsoft® Advertising]
description: 에서 동기화된 캠페인을 내보내는 방법 알아보기 [!DNL Google Ads] 동기화된 계정에 직접 연결 [!DNL Microsoft® Advertising] 계정입니다.
exl-id: 1bb0d915-bf33-4c50-88a5-268d4de5ccff
source-git-commit: 8d062e5c74c8f873ab5f2491659a32be47bb2afb
workflow-type: tm+mt
source-wordcount: '962'
ht-degree: 0%

---

# 복제 [!DNL Google Ads] 의 캠페인 [!DNL Microsoft® Advertising]

에서 동기화된 캠페인을 내보낼 수 있습니다. [!DNL Google Ads] 동기화된 계정에 직접 연결 [!DNL Microsoft® Advertising] 계정을 eCPC(향상된 CPC) 캠페인으로 지정합니다. 기존 입찰 및 캠페인 예산의 크기가 조정됩니다. 기존 검색, 소셜 및 상거래 추적은 가져오지 않습니다.

다음 유형의 캠페인과 해당 캠페인 구조를 복제할 수 있습니다.

* [!DNL Google Ads] 캠페인 검색 및 표시 [!DNL Microsoft® Advertising] 캠페인을 검색하고 표시합니다.

* [!DNL Google Display Network] 광고 이미지를 포함한 캠페인 [!DNL Microsoft® Advertising] Microsoft® Audience Network의 대상자 캠페인

  쇼핑 피드 기반 표시 캠페인을 복제하려면 먼저 다음을 복제하십시오. [!DNL Google Merchant Center] 에 대한 제품 오퍼 [!DNL Microsoft® Merchant Center]. 캠페인을 복제할 때 다음을 선택합니다. [!DNL Microsoft® Merchant Center] 가져오기 선택 사항에 저장 하여 피드 기반 대상 캠페인에 저장소를 연결합니다.

* [!DNL Google Ads] 성과 최대 캠페인(로컬 인벤토리 광고 포함)을에 [!DNL Microsoft® Advertising] 스마트 쇼핑 캠페인.

캠페인을 한 번, 매일 주별 또는 매월 업데이트하도록 선택하거나 [!DNL Microsoft® Advertising]의 권장 일정입니다. 선택적으로 가져오기 작업이 실행될 때마다 또는 오류나 변경 사항이 발생할 때 알림을 구성할 수 있습니다. 캠페인을 로 가져오면 [!DNL Microsoft® Advertising], 가져오기 작업의 상태를 확인하고, 오류 로그를 검토하고, 가져오기 작업을 수동으로 실행하고, 가져오기 일정을 편집, 일시 중지, 활성화 또는 삭제할 수 있습니다.

일부 캠페인 정보가 복제되는 것은 아니며, 일부 정보를 [!DNL Microsoft® Advertising] 캠페인. 가져온 데이터에 대한 자세한 내용은 [!DNL Microsoft® Advertising] 다음에 대한 도움말[에서 가져오는 항목 [!DNL Google Ads]](https://help.ads.microsoft.com/#apex/ads/en/50851).&quot; 검색, 소셜 및 상거래 추적을 가져오지 않으므로 [account](/help/search-social-commerce/campaign-management/accounts/ad-network-account-manage.md), [campaign](/help/search-social-commerce/campaign-management/campaigns/campaign-manage.md), [광고 그룹](/help/search-social-commerce/campaign-management/campaigns/ad-group-manage.md), 또는 [광고](/help/search-social-commerce/campaign-management/campaigns/ad-manage.md) 설정.

## 복제 [!DNL Google Ads] 캠페인

>[!NOTE]
>
>쇼핑 피드 기반 표시 캠페인을 복제하려면 먼저 [다음을 복제합니다. [!DNL Google Merchant Center] 의 제품 오퍼 [!DNL Microsoft® Merchant Center]](https://help.ads.microsoft.com/apex/index/3/en/56870). 캠페인을 복제할 때 다음을 선택합니다. [!DNL Microsoft® Merchant Center] 가져오기 옵션에 저장 하여 스토어를 피드 기반 대상 캠페인에 연결합니다.

다음을 참조하십시오 [에서 가져온 항목 [!DNL Google Ads] 캠페인](https://help.ads.microsoft.com/#apex/ads/en/50851/0-500).

1. 검색, 소셜 및 상거래 기본 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Tools] >[!UICONTROL Import Campaigns]**.

1. 클릭 **[!UICONTROL +Import]**.

1. 다음을 지정합니다. [가져오기 설정](#campaign-import-settings):

   1. 다음에서 **[!UICONTROL Select accounts]** 섹션:

      1. 소스 및 대상 계정을 선택합니다.

      1. 클릭 **[!UICONTROL Get Credential Id from MSA]**.

      1. 대상에 로그인 [!DNL Microsoft Advertising] 계정을 만든 후 표시되는 자격 증명 ID를 복사하고 값을 **[!UICONTROL Credential ID]** 필드.

   1. 다음에서 **[!UICONTROL Select campaigns & ad groups]** 섹션에서 가져올 캠페인 및 광고 그룹을 지정합니다.

   1. 다음에서 **[!UICONTROL Customize your import]** 섹션에서 가져올 항목 유형을 지정합니다.

   1. 다음에서 **[!UICONTROL Set schedule]** 섹션에서 가져오기 작업을 실행할 시기를 지정합니다.

1. 클릭 **[!UICONTROL Post]**.

1. (선택 사항) 내에서 검색, 소셜 및 상거래 추적 추가 [account](/help/search-social-commerce/campaign-management/accounts/ad-network-account-manage.md), [campaign](/help/search-social-commerce/campaign-management/campaigns/campaign-manage.md), [광고 그룹](/help/search-social-commerce/campaign-management/campaigns/ad-group-manage.md), 또는 [광고](/help/search-social-commerce/campaign-management/campaigns/ad-manage.md) 설정.

## 캠페인 가져오기 작업에 대한 일정 설정 편집

다음을 참조하십시오 [에서 가져온 항목 [!DNL Google Ads] 캠페인](https://help.ads.microsoft.com/#apex/ads/en/50851/0-500).

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Tools] >[!UICONTROL Import Campaigns]**.

1. 가져오기 작업 옆에 있는 확인란을 선택한 다음 을 클릭합니다. ![편집](/help/search-social-commerce/assets/edit.png "편집").

1. 다음에서 **[!UICONTROL Set schedule]** 섹션에서 다음을 지정합니다. [예약 설정](#campaign-import-settings).

1. 클릭 **[!UICONTROL Post]**.

## 캠페인 가져오기 작업 보기

소스를 포함하여 모든 가져오기 작업을 나열할 수 있습니다 [!DNL Google Ads] 계정, 대상 [!DNL Microsoft® Advertising] 계정, 가져오기 시간 또는 일정 및 작업을 만든 사용자입니다. 정기적으로 예약된 가져오기 작업을 포함하여 가져오기 작업을 여러 번 실행하면 각 항목이 별도의 작업으로 나열됩니다.

* 다음 중 하나를 수행합니다.

   * 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Tools] >[!UICONTROL Import Campaigns]**.

     기본적으로 뷰는 [!UICONTROL List of Import Jobs] 탭.

   * 다음에서 [[!UICONTROL Import Logs] 탭](#campaign-import-log)를 클릭하고 **[!UICONTROL List of Import Jobs]** 탭.

## 캠페인 가져오기 작업 실행

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Tools] >[!UICONTROL Import Campaigns]**.

1. 가져오기 작업 옆의 확인란을 선택합니다.

1. 클릭 ![지금 실행](/help/search-social-commerce/assets/run.png "지금 실행").

## 캠페인 가져오기 작업에 대한 로그 보기 {#campaign-import-log}

시작 시간을 비롯하여 완료되거나 실패한 모든 가져오기 작업을 나열할 수 있습니다. [!DNL Google Ads] 계정, 대상 [!DNL Microsoft® Advertising] 계정, 작업을 만든 사용자, 성공 및 실패한 작업 수 및 각 작업에 대한 알림을 받은 이메일 주소. 대상 변경에 대한 자세한 내용을 볼 수 있습니다 [!DNL Microsoft® Advertising] 추가, 동기화, 삭제된 항목 수를 포함하여 각 작업에 대해 발생한 계정이며, 해당 계정에서 각 엔티티 수준(예: 캠페인 또는 키워드)에 대해 오류가 발생한 계정입니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Tools] >[!UICONTROL Import Campaigns]**.

1. 다음을 클릭합니다. **[!UICONTROL Import Logs]** 탭.

1. (선택 사항) 가져오기 작업에 대한 세부 정보를 보려면 [!UICONTROL Summary] 열.

## 캠페인 가져오기 작업 설정 {#campaign-import-settings}

### [!UICONTROL Select accounts]

**[!UICONTROL Source Google Ads account]:** 동기화됨 [!DNL Google Ads] 캠페인 데이터를 내보내는 계정입니다.

**[!UICONTROL Credential ID]:** 다음 ID [!DNL Microsoft® Advertising] 은 을(를) 나타내는 데 을(를) 사용합니다. [!DNL Google Ads] 자격 증명.

자동 생성 [!DNL Microsoft® Advertising] 가져오기 용 자격 증명은 다음 이유로 사용할 수 없습니다. [!DNL Microsoft® Advertising] 제한 사항. Adobe 기술 지원 또는 Adobe 계정 팀에 문의하면 자격 증명을 생성하고 ID를 제공합니다.

**[!UICONTROL Target Microsoft® Ads account]:** 동기화됨 [!DNL Microsoft® Advertising] 캠페인 데이터를 가져오는 계정입니다.

### [!UICONTROL Select campaigns & ad groups]

**\[가져올 데이터\]:** 가져올 데이터 지정:

* *[!UICONTROL Import all new and existing campaigns]:* 이미 존재하는 모든 캠페인과 존재하지 않는 캠페인에 대한 데이터를 가져오려면 [!DNL Microsoft® Advertising].

* *[!UICONTROL Import specific campaigns and adgroups]:* 특정 캠페인 및 광고 그룹을 선택하려면 다음을 수행하십시오.

   * 캠페인을 하위 광고 그룹으로 확장하려면 **[!UICONTROL >]** 캠페인 이름 뒤에.

   * 캠페인 또는 광고 그룹을 선택하려면 확인 표시가 나타나도록 항목을 선택합니다.

   * 캠페인 또는 광고 그룹을 제거하려면 다음 작업을 수행하십시오.

      * 다음에서 [!UICONTROL Campaigns] 또는 [!UICONTROL Adgroups] 열에서 캠페인 또는 광고 그룹을 선택 해제하여 확인 표시가 사라지도록 합니다.

      * 다음에서 [!UICONTROL Selected] 열, 클릭 ![삭제](/help/search-social-commerce/assets/delete.png "삭제").

### [!UICONTROL Customize your import]

**[!UICONTROL Choose specific import options]:** 가져올 항목, 입찰 및 예산 및 기타 옵션을 지정할 수 있습니다.

**[!UICONTROL What to import]:** 가져올 항목을 정의합니다. 기본적으로 항목 범주를 가져오는 옵션이 선택되어 있으며 모든 항목 유형이 선택되어 있습니다. 특정 항목 유형만 포함하려면 **[!UICONTROL Show advanced options]** 포함할 항목 유형을 변경합니다.

**[!UICONTROL Bids and budgets]:** 가져오기, 업데이트 및 사용자 지정할 입찰 및 예산 설정을 정의합니다.

**[!UICONTROL Other options]:** 가져온 랜딩 페이지 URL, 추적 템플릿, 기타 캠페인, 광고 및 타깃팅 옵션을 처리하는 방법을 정의합니다.

### [!UICONTROL Set schedule]

**[!UICONTROL Import name]:** 가져오기 작업의 이름입니다.

**[!UICONTROL When]:** 지정된 캠페인을 가져오는 시기: *자동* (허용 [!DNL Microsoft® Advertising] 캠페인을 가장 잘 최적화하기 위한 일정을 설정합니다.), *[!UICONTROL Now]* (작업 설정을 게시할 때 작업을 실행하려면) *[!UICONTROL Once]* 지정된 시간에 *[!UICONTROL Daily]* 지정된 시간에 *[!UICONTROL Weekly]* 지정된 시간에 또는 *[!UICONTROL Monthly]* 지정한 시간에.

**[!UICONTROL Receive email notifications]:** 보고서 보내기 필드의 이메일 주소로 가져오기 작업에 대한 이메일 알림을 보낼 경우 및 보낼 때.

**[!UICONTROL Send reports to]:** 가져오기 작업에 대한 알림을 수신할 이메일 주소. 쉼표()로 여러 주소 구분`,`).
