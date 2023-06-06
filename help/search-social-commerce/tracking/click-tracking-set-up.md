---
title: 쿠키 기반 클릭 추적 설정
description: 클릭 추적 태그를 설정하고 유효성을 검사하는 방법에 대해 알아봅니다.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# 쿠키 기반 클릭 추적 설정

Search, Social 및 Commerce에서 클릭 수를 추적하려면 다음 요소를 구성하고 유효성을 검사해야 합니다.

1. (Adobe 계정 팀) 광고주를 픽셀 고객으로 설정합니다.

1. [광고주의 각 광고 네트워크 계정 및 캠페인에 대한 올바른 추적 옵션을 지정합니다](#set-up-click-tracking-options).

1. 필요한 경우 [추적 URL을 생성하고 업로드합니다](#generate-upload-tracking-urls) 일부 캠페인 요소에 사용할 수 있습니다.

1. [클릭 추적 URL 몇 개의 형식을 확인하고 테스트하여 올바른 랜딩 페이지가 열리는지 확인합니다](#validate-tracking-urls).

## 광고 네트워크 계정 및 캠페인에 대한 추적 옵션 설정 {#set-up-click-tracking-options}

*에이전시 계정 관리자, [!DNL Adobe] 계정 관리자 및 관리자 역할만*

1. 각 광고 네트워크 계정에 대해 다음을 수행합니다.

   1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**. 하위 메뉴에서 **[!UICONTROL Live]>[!UICONTROL Accounts]**.

   1. 계정 이름 위에 커서를 놓고 ![메뉴 아이콘](/help/search-social-commerce/assets/arrow-dropdown-menu.png "메뉴 아이콘")을 선택한 다음 을 선택합니다 **[!UICONTROL Edit]**.

   1. 클릭 **[!UICONTROL Set Account Tracking]**.

   1. 의 경우 [!UICONTROL Tracking Type] 설정, 선택 **[!UICONTROL EF Redirect]**.

   1. (검색, 소셜 및 상거래를 통해 Adobe Analytics과 데이터를 교환하거나 [!DNL Apple Safari]) [!UICONTROL Redirect Type] 옵션 **[!UICONTROL Token]**.

   1. (선택 사항) **[!UICONTROL Auto Upload]** 다음에 검색, 소셜 및 상거래가 동기화할 때 새 추적 URL을 광고 네트워크에 자동으로 업로드하는 옵션입니다. 이 값은 계정의 모든 캠페인에 대한 기본값으로 상속되지만 캠페인 수준에서 재정의할 수 있습니다.

1. 각 캠페인에 대해 다음 작업을 수행합니다.

   1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Campaigns]**. 하위 메뉴에서 **[!UICONTROL Live]>[!UICONTROL Campaigns]**.

   1. 캠페인 이름 위에 커서를 놓고 ![메뉴 아이콘](/help/search-social-commerce/assets/arrow-dropdown-menu.png "메뉴 아이콘")을 선택한 다음 을 선택합니다 **[!UICONTROL Edit]**.

   1. 클릭 **[!UICONTROL Set Campaign Tracking]**. 그런 다음 옵션을 선택합니다. **[!UICONTROL Override Account Tracking]**.

   1. 의 경우 [!UICONTROL Tracking Type] 설정, 선택 **[!UICONTROL EF Redirect]**.

   1. (검색, 소셜 및 상거래를 통해 Adobe Analytics과 데이터를 교환하거나 [!DNL Apple Safari]) [!UICONTROL Redirect Type] 옵션 **[!UICONTROL Token]**.

   1. (선택 사항) **[!UICONTROL Auto Upload]** 다음에 검색, 소셜 및 상거래가 동기화할 때 새 추적 URL을 광고 네트워크에 자동으로 업로드하는 옵션입니다. 이 값은 계정의 모든 캠페인에 대한 기본값으로 상속되지만 캠페인 수준에서 재정의할 수 있습니다.

## 추적 URL 생성 및 업로드 {#generate-upload-tracking-urls}

를 참조하십시오.[클릭 추적 URL 생성 시기 및 방법](/help/search-social-commerce/tracking/click-tracking-ways-to-generate.md).&quot;

### 클릭 추적 URL 형식 테스트 {#validate-tracking-urls}

클릭 추적 URL에 대한 올바른 랜딩 페이지가 열렸는지 확인합니다.

1. 광고주의 스테이징 환경에 트래픽을 전송하여 광고 클릭을 모방합니다.

   1. 텍스트 편집기에서 클릭 추적 URL을 붙여넣고, 광고주의 스테이징 환경 내에서 동일한 페이지를 가리키도록 랜딩 페이지 URL을 변경한 다음, 브라우저의 주소 표시줄에 새 URL을 붙여 넣고 **[!DNL Enter]** 키.

   1. 브라우저의 저장된 쿠키에서 쿠키를 찾습니다.

   1. 스테이징 사이트에서 트랜잭션을 완료하고 성공 페이지가 올바른 픽셀을 실행하는지 확인합니다. 픽셀에서 추적하는 실제 매개변수는 광고주와 추적 URL에 따라 다릅니다. 다음 예에서는 광고주가 새 애플리케이션 수와 새 매출액을 추적하려고 합니다.

      새 최종 사용자(새 쿠키 사용)의 경우 다음 픽셀을 실행해야 합니다.

      `< img width="1" height="1" src="http://pixel-user-everesttech.net/<Advertising_Cloud_UserID>/p?ev_transid=<applicationid>&ev_new_application=1&ev_new_amount=<loanamount>" / >`

      쿠키가 최신 상태가 아니면 다음 픽셀을 실행해야 합니다.

      `< img width="1"height="1" src="http://pixel-user-everesttech.net/<Advertising_Cloud_UserID>/p?ev_transid=<applicationid>&ev_previous_application=1&ev_new_amount=<loanamount>" / >`


1. 도메인의 여러 클릭 추적 URL에 대해 이 작업을 반복합니다.

1. 그에 따라 다른 랜딩 페이지를 사용하여 각 도메인에 대해 1단계를 반복합니다.

1. 필요한 경우 검색, 소셜 및 상거래에 거래 ID에 대한 픽셀이 표시되는지 확인합니다(`ev_transid`)을 생성하지 않습니다.

>[!MORELIKETHIS]
>
>* [클릭 추적 URL 생성 시기 및 방법](/help/search-social-commerce/tracking/click-tracking-ways-to-generate.md)

