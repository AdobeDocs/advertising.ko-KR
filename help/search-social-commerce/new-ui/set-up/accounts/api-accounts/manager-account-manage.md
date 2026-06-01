---
title: (새 UI) Google Ads Manager 계정의 자격 증명 관리
description: 새 UI에서 Google Ads Manager 계정에 대한 자격 증명을 설정하고 관리하는 방법을 알아봅니다.
feature: Search Admin
source-git-commit: bf1ca7f6133c19bb68dbe0395416dca8ef647464
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---

# (새 UI) [!DNL Google Ads] 관리자 계정의 자격 증명을 관리합니다.

*Beta 기능*

*[!DNL Google Ads]개의 계정만*

Search, Social 및 Commerce에서 계정 간 전환을 업로드할 [!DNL Google Ads] 관리자 계정에 대한 자격 증명을 제공합니다. a) [!DNL Adobe]이(가) 추적된 교차 계정 전환 지표를 [!DNL Google Ads] 관리자 계정에 업로드하거나, b) 하이브리드 최적화를 위해 [!DNL Google Ads]에 대한 교차 계정 전환을 포함하는 포트폴리오 목표를 업로드하려면 이 기능을 사용하십시오.

새 관리자 계정 레코드에 대한 자격 증명을 추가하거나 기존 관리자 계정을 재인증할 수 있습니다.

관리자 계정에 대한 자격 증명을 추가하면 계정 설정에 연결된 관리자 계정 ID가 읽기 전용으로 표시됩니다. 관리자 계정의 자격 증명이 없거나([!UICONTROL Manager Account Missing Error]) 관리자 계정 인증 토큰이 만료된 경우([!UICONTROL Manager Account Auth Error]) [!UICONTROL Notification Center]에 [알림](/help/search-social-commerce/new-ui/notifications-manage.md)이(가) 포함됩니다.

## 새 관리자 계정에 대한 자격 증명 추가 {#create-manager-account}

1. 주 메뉴에서 **[!UICONTROL Setup]** \> **[!UICONTROL Manager Accounts]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL +]**&#x200B;을(를) 클릭합니다.

1. 광고 네트워크를 선택한 다음 **[!UICONTROL Next]**&#x200B;을(를) 클릭합니다.

1. [관리자 계정 설정](#manager-account-settings)을 지정하십시오.

1. **[!UICONTROL Authenticate]**&#x200B;을(를) 클릭하고 관리자 계정 자격 증명을 사용하여 로그인합니다.

   Search, Social 및 Commerce은 인증 토큰을 자동으로 캡처하고 저장합니다.

1. 검색, 소셜 및 Commerce에서 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 관리자 계정 세부 정보 편집 {#edit-manager-account}

1. 주 메뉴에서 **[!UICONTROL Setup]** \> **[!UICONTROL Manager Accounts]**&#x200B;을(를) 클릭합니다.

1. 다음 방법 중 하나로 계정을 선택합니다.

   * 계정 이름 옆의 확인란을 선택한 다음 일괄 작업 도구 모음에서 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

   * 계정 이름 위에 커서를 놓고 **..**&#x200B;을 클릭한 다음 (/help/search-social-commerce/assets/edit-new.png &quot;편집)을 클릭합니다.

1. [관리자 계정 설정](#manager-account-settings)을(를) 편집합니다.

1. **[!UICONTROL Re-Authenticate]**&#x200B;을(를) 클릭하고 관리자 계정 자격 증명을 사용하여 로그인합니다.

   Search, Social 및 Commerce은 인증 토큰을 자동으로 캡처하고 저장합니다.

1. 검색, 소셜 및 Commerce에서 **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 관리자 계정 재인증 {#reauthenticate-manager-account}

OAuth 토큰이 만료되거나 유효하지 않게 된 경우 관리자 계정을 재인증합니다.

1. 주 메뉴에서 **[!UICONTROL Setup]** \> **[!UICONTROL Manager Accounts]**&#x200B;을(를) 클릭합니다.

1. 계정 이름 위에 커서를 놓고 **..**&#x200B;을 클릭한 다음 **[!UICONTROL Reauthenticate]**&#x200B;을(를) 클릭합니다.

1. 관리자 계정 자격 증명을 사용하여 로그인합니다.

   Search, Social 및 Commerce은 자동으로 새 인증 토큰을 캡처하고 저장합니다.

## 관리자 계정 설정 {#manager-account-settings}

**[!UICONTROL Manager Account ID]:** 광고 네트워크의 관리자 계정에 대한 고유한 계정 ID입니다.

**[!UICONTROL Mnaager Account Name]:** Search, Social 및 Commerce 내에서 관리자 계정에 대해 표시할 이름입니다.

**[!UICONTROL Login Email]:** 관리자 계정 로그인과 연결된 전자 메일 주소입니다. 인증에 필요합니다.

**[!UICONTROL Password]:**(선택 사항) 계정의 암호입니다. 계정 관리자가 필요에 따라 토큰을 새로 고칠 수 있도록 암호화하고 저장하려면 암호를 입력합니다.

>[!MORELIKETHIS]
>
>* [광고 네트워크에 목표를 업로드할 수 있도록 설정](/help/search-social-commerce/new-ui/goals/objectives/objective-upload-to-networks.md)
>* [알림 관리](/help/search-social-commerce/new-ui/notifications-manage.md)

<!--
I don't see this yet in new UI:
>* [Upload Search, Social, & Commerce-tracked conversion metrics to [!DNL Google Ads]](/help/search-social-commerce/tools/conversion-metrics-upload-to-google.md)
-->
