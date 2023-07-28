---
title: 광고 네트워크 관리자 계정의 자격 증명 관리
description: 에 대한 자격 증명을 제공하는 방법을 알아봅니다. [!DNL Google Ads] 관리자 계정입니다.
exl-id: bde22f70-12a7-4eef-a141-dafeed9a7dc5
feature: Search Admin
source-git-commit: 052574217d7ddafb8895c74094da5997b5ff83db
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 1%

---

# 광고 네트워크 관리자 계정의 자격 증명 관리

*Beta 기능*

*[!DNL Google Ads]계정만*

에 대한 자격 증명을 제공합니다. [!DNL Google Ads] 계정 간 전환을 업로드할 Search, Social 및 Commerce의 관리자 계정입니다. a) 업로드를 원하는 경우 이 기능 사용 [!DNL Adobe]-추적된 교차 계정 전환 지표를 [!DNL Google Ads] 관리자 계정 또는 b) 계정 간 전환을 포함하는 포트폴리오 목표 업로드 [!DNL Google Ads] 하이브리드 최적화를 위해.

<!-- [Maybe later: and c) sync conversion value rules for accounts that use cross-account conversion tracking with Google Ads.] -->

새 관리자 계정 레코드에 대한 자격 증명을 추가하거나 기존 관리자 계정을 재인증할 수 있습니다.

관리자 계정에 대한 자격 증명을 추가하면 계정 설정에 연결된 관리자 계정 ID가 읽기 전용으로 표시됩니다. 또한 선택적 입니다.[!UICONTROL Manager Account for Cross-Account Conversions]의 &quot; 열 [!UICONTROL Campaigns] > [!UICONTROL Accounts] view에는 각 하위 계정에 대한 관리자 계정 ID가 표시되며, 관리자 계정이 인증되지 않은 경우 오류가 표시됩니다. [!UICONTROL Notification Center] 관리자 계정의 자격 증명이 누락된 경우 알림을 포함합니다([다음 [!UICONTROL Manager Account Missing Error]](/help/search-social-commerce/notifications/notification-about.md)) 또는 manager 계정 인증 토큰이 만료될 때([다음 [!UICONTROL Manager Account Auth Error]](/help/search-social-commerce/notifications/notification-about.md)).

## 새 관리자 계정에 대한 자격 증명을 추가하려면

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Admin] >[!UICONTROL Manager Accounts]**.

1. 선택 **[!UICONTROL Create new manager account]**.

1. 관리자 계정에 대한 로그인 자격 증명을 입력합니다.

   다음 **[!UICONTROL Manager Account ID]** 및 **[!UICONTROL Login Email]** 필수 항목입니다. Search, Social 및 Commerce는 인증에 사용할 계정 토큰을 자동으로 캡처하고 저장합니다.

   다음을 선택적으로 포함할 수 있습니다. **[!UICONTROL MCC Account Name]** 검색, 소셜, 상거래 및 계정 내에서 식별 **[!UICONTROL Password]**. 계정 관리자가 필요에 따라 토큰을 새로 고칠 수 있도록 암호화하고 저장하려면 암호를 입력합니다.

1. 클릭 **[!UICONTROL Authenticate]**.

1. 클릭 **[!UICONTROL Save]**.

## 기존 관리자 계정을 다시 인증하려면

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Admin] >[!UICONTROL Manager Accounts]**.

1. 선택 **[!UICONTROL Reauthenticate existing manager account]**.

1. 관리자 계정을 선택합니다.

1. 관리자 계정에 대한 로그인 자격 증명을 입력합니다.

   다음 **[!UICONTROL Manager Account ID]** 및 **로그인 전자 메일** 필수 항목입니다. Search, Social 및 Commerce는 인증에 사용할 계정 토큰을 자동으로 캡처하고 저장합니다.

   다음을 선택적으로 포함할 수 있습니다. **[!UICONTROL MCC Account Name]** 검색, 소셜, 상거래 및 계정 내에서 식별 **[!UICONTROL Password]**. 계정 관리자가 필요에 따라 토큰을 새로 고칠 수 있도록 암호화하고 저장하려면 암호를 입력합니다.

1. 클릭 **[!UICONTROL Authenticate]**.

1. 클릭 **[!UICONTROL Save]**.

>[!MORELIKETHIS]
>
>* [광고 네트워크에 목표 업로드 활성화](/help/search-social-commerce/tools/objective-upload-to-networks.md)
>* [전환 지표 업로드 [!DNL Google Ads]](/help/search-social-commerce/tools/conversion-metrics-upload-to-google.md)
>* [알림 설정 편집](/help/search-social-commerce/notifications/notification-edit.md)
