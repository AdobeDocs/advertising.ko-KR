---
title: 동기화 [!DNL Adobe] 대상
description: ' [!DNL Adobe] 대상자에 대한 메타데이터, 계층 데이터 및 고유 대상자 데이터를 동기화하는 방법을 알아봅니다.'
exl-id: 8b8c3aa0-2aa9-4ad7-a4c0-1b7ba881acd3
feature: Search Admin
source-git-commit: e16bc62127a708de8f4deb1eddfa53a14405cbc2
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---

# [!DNL Adobe]개 대상 동기화

*[!DNL Direct Access]명의 클라이언트 관리자 및 관리자만*

*Adobe Advertising-Adobe Audience Manager 또는 Adobe Advertising-Adobe Analytics 통합만 있는 광고주*

Search, Social 및 Commerce을 허용하면 광고주나 에이전시의 모든 [!DNL Adobe] 대상에 대한 메타데이터, 계층 데이터 및 고유한 대상 데이터를 [!UICONTROL Campaigns] > [!UICONTROL Audiences] 보기로 가져올 수 있습니다. 이 정보에는 다음에 대한 데이터가 포함됩니다.

* Adobe Audience Manager 세그먼트

* Adobe Experience Cloud에 게시된 Adobe Analytics 세그먼트

* Adobe Experience Cloud [!DNL Audience Library]을(를) 사용하여 만든 세그먼트

자격을 얻으려면 광고주나 에이전시는 [Adobe Experience Platform Identity 서비스](https://experienceleague.adobe.com/docs/id-service/using/home.html?lang=ko)를 구현하고 해당 조직 ID(이전의 [!DNL IMS Org ID])를 제공해야 합니다.

초기 동기화는 약 24시간이 소요됩니다. 그 후에는 데이터가 1~2초 지연으로 실시간으로 동기화됩니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Admin] >[!UICONTROL Audience Manager Setup]**&#x200B;을(를) 클릭합니다.

1. 광고주의 Adobe Experience Cloud 계정에 대한 고유한 조직 ID를 입력한 다음 **[!UICONTROL Submit]**&#x200B;을(를) 클릭합니다.

   광고주의 조직 ID를 모를 경우 [!UICONTROL Admin] > [!UICONTROL Manage Client]의 광고주 설정의 **[!UICONTROL IMS Org ID]** 필드에서 검색하십시오.

>[!MORELIKETHIS]
>
>* [대상자 정보](/help/search-social-commerce/campaign-management/campaigns/audience-about.md)
>* [Adobe Experience Cloud 솔루션 및 서비스와 통합](/help/search-social-commerce/introduction/integrations.md)
