---
title: 광고 네트워크 관리자 계정의 자격 증명 관리
description: ' [!DNL Google Ads] 관리자 계정의 자격 증명을 제공하는 방법을 알아봅니다.'
exl-id: 95866a2e-4695-4b1d-ac23-844d3b9a0a74
feature: Search Admin
TQID: https://experienceleague.adobe.com/NHgpx-F19gX8jsOIPijPzNlGVhBje-CVsj4jjlV1OR0
product_v2: id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2: id: e55292b5-d4a1-4c98-9c20-2a2c5bea07fb
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1id: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: 527ca2bb74de388c13ba1ce5bde3f8be1cead8d0
workflow-type: tm+mt
source-wordcount: 327
ht-degree: 0%

---

# 광고 네트워크 관리자 계정의 자격 증명 관리

*[!DNL Google Ads]개의 계정만*

Search, Social 및 Commerce에서 계정 간 전환을 업로드할 [!DNL Google Ads] 관리자 계정의 자격 증명을 제공합니다. a) [!DNL Adobe]이(가) 추적된 교차 계정 전환 지표를 [!DNL Google Ads] 관리자 계정에 업로드하거나, b) 하이브리드 최적화를 위해 [!DNL Google Ads]에 대한 교차 계정 전환을 포함하는 포트폴리오 목표를 업로드하려면 이 기능을 사용하십시오.

<!-- [Maybe later: and c) sync conversion value rules for accounts that use cross-account conversion tracking with Google Ads.] -->

새 관리자 계정 레코드에 대한 자격 증명을 추가하거나 기존 관리자 계정을 재인증할 수 있습니다.

관리자 계정에 대한 자격 증명을 추가하면 계정 설정에 연결된 관리자 계정 ID가 읽기 전용으로 표시됩니다. 또한 [!UICONTROL Manager Account for Cross-Account Conversions] > [!UICONTROL Campaigns] 보기의 선택적 &quot;[!UICONTROL Accounts]&quot; 열은 각 하위 계정의 관리자 계정 ID를 표시하며 관리자 계정이 인증되지 않은 경우 오류를 나타냅니다. [!UICONTROL Notification Center]은(는) 관리자 계정의 자격 증명이 없거나([the [!UICONTROL Manager Account Missing Error]](/help/search-social-commerce/notifications/notification-about.md)) 관리자 계정 인증 토큰이 만료된 경우([the [!UICONTROL Manager Account Auth Error]](/help/search-social-commerce/notifications/notification-about.md)) 알림을 포함합니다.

## 새 관리자 계정에 대한 자격 증명을 추가하려면

1. 메인 메뉴에서 **[!UICONTROL Search, Social, & Commerce]> [!UICONTROL Admin] >[!UICONTROL Manager Accounts]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Create new manager account]**&#x200B;을(를) 선택합니다.

1. 관리자 계정에 대한 로그인 자격 증명을 입력합니다.

   **[!UICONTROL Manager Account ID]** 및 **[!UICONTROL Login Email]**&#x200B;은(는) 필수입니다. Search, Social 및 Commerce은 인증에 사용할 계정 토큰을 자동으로 캡처하고 저장합니다.

   Search, Social, &amp; Commerce 및 **[!UICONTROL MCC Account Name]** 계정 내에서 식별을 위해 **[!UICONTROL Password]**&#x200B;을(를) 선택적으로 포함할 수 있습니다. 계정 관리자가 필요에 따라 토큰을 새로 고칠 수 있도록 암호화하고 저장하려면 암호를 입력합니다.

1. **[!UICONTROL Authenticate]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

## 기존 관리자 계정을 다시 인증하려면

1. 메인 메뉴에서 **[!UICONTROL Search, Social, & Commerce]> [!UICONTROL Admin] >[!UICONTROL Manager Accounts]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Reauthenticate existing manager account]**&#x200B;을(를) 선택합니다.

1. 관리자 계정을 선택합니다.

1. 관리자 계정에 대한 로그인 자격 증명을 입력합니다.

   **[!UICONTROL Manager Account ID]** 및 **로그인 전자 메일**&#x200B;이 필요합니다. Search, Social 및 Commerce은 인증에 사용할 계정 토큰을 자동으로 캡처하고 저장합니다.

   Search, Social, &amp; Commerce 및 **[!UICONTROL MCC Account Name]** 계정 내에서 식별을 위해 **[!UICONTROL Password]**&#x200B;을(를) 선택적으로 포함할 수 있습니다. 계정 관리자가 필요에 따라 토큰을 새로 고칠 수 있도록 암호화하고 저장하려면 암호를 입력합니다.

1. **[!UICONTROL Authenticate]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [광고 네트워크에 목표를 업로드할 수 있도록 설정](/help/search-social-commerce/tools/objective-upload-to-networks.md)
>* [검색, 소셜 및 Commerce에서 추적한 전환 지표를  [!DNL Google Ads]](/help/search-social-commerce/tools/conversion-metrics-upload-to-google.md)에 업로드합니다.
>* [알림 설정 편집](/help/search-social-commerce/notifications/notification-edit.md)
