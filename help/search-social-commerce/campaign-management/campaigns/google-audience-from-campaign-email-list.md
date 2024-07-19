---
title: Adobe Campaign 이메일 목록에서  [!DNL Google Ads] 고객 일치 대상 만들기
description: 기존 Adobe Campaign 이메일 목록에서  [!DNL Google Ads] 고객 일치 대상자를 만드는 방법을 알아봅니다.
exl-id: 92812af2-ac31-48cd-badf-ea287799bddb
feature: Search Campaign Management
source-git-commit: e16bc62127a708de8f4deb1eddfa53a14405cbc2
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# Adobe Campaign 이메일 목록에서 [!DNL Google Ads] 고객 일치 대상 만들기

고객 일치 항목에만 적합한 계정 *[!DNL Google Ads]개*

[!DNL Campaign]에서 계정 링크 및 워크플로우를 설정하여 Adobe Campaign의 이메일 목록에서 [!DNL Google Ads] 고객 일치 대상을 만들 수 있습니다.

이를 위해서는 [!DNL Campaign] 인스턴스에 대한 액세스 권한과 Adobe 계정 팀이 제공할 필수 워크플로가 포함된 XML 파일이 필요합니다. 지침은 [!DNL Campaign]의 다양한 버전에 따라 다를 수 있습니다. 필요한 경우 Adobe 계정 팀이 [!DNL Campaign]에서 워크플로를 설정하는 데 도움을 줄 수 있습니다.

1. Advertising 검색, 소셜 및 Commerce 제공 SFTP 계정에 대한 자격 증명을 획득합니다.

1. [!DNL Campaign]에서 Advertising 검색, 소셜 및 Commerce에 전자 메일 목록 게재를 설정합니다.

   1. [외부 계정](https://experienceleague.adobe.com/docs/campaign-standard/using/administrating/application-settings/external-accounts.html)을 만들어 검색, 소셜 및 Commerce 제공 SFTP 계정을 연결합니다.

      1. 왼쪽 메뉴에서 **\[Adobe Campaign v6\] > [!UICONTROL Platform] >[!UICONTROL External Accounts]**(으)로 이동합니다.

      1. ![계정 만들기](/help/search-social-commerce/assets/campaign-create-account.png "계정 만들기")를 클릭합니다.

      1. 계정 레이블을 입력하고 계정 유형으로 **[!UICONTROL SFTP]**&#x200B;을(를) 선택하십시오.

      1. [!DNL Adobe] SFTP 서버의 URL 및 포트 번호와 광고주의 폴더 이름, 사용자 이름 및 암호를 입력합니다.

      1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

   1. [!DNL Campaign Client]에서 전자 메일 데이터를 보내는 데 필요한 워크플로가 포함된 데이터 패키지를 설치하십시오.

      1. 메뉴 모음에서 **[!UICONTROL Tools]> [!UICONTROL Advanced] >[!UICONTROL Import Package]**(으)로 이동합니다.

      1. **[!UICONTROL Install a package from a file]**&#x200B;을(를) 선택한 다음 **[!UICONTROL Next]**&#x200B;을(를) 클릭합니다.

      1. 장치 또는 네트워크에서 데이터 패키지 파일(`AMO_Workflow.xml`)을 찾은 다음 **[!UICONTROL Next]**&#x200B;을(를) 클릭합니다.

      1. **[!UICONTROL Start]**&#x200B;을(를) 클릭하고 워크플로가 설치될 때까지 기다립니다.

   1. 설치된 워크플로우를 편집하여 데이터 쿼리에 대한 필터를 선택적으로 편집하고 새 대상 이름 및 외부 SFTP 계정을 식별합니다.

      1. **[!UICONTROL Administration]> [!UICONTROL Configuration] > [!UICONTROL Package management] >[!UICONTROL Installed packages]**(으)로 이동하여 패키지를 엽니다.

      1. (선택 사항) 데이터에 대한 필터를 편집합니다.

         * 워크플로우에서 쿼리 활동(예: ForkTransition 1)을 두 번 클릭합니다.

         * 필터 표현식을 편집합니다.

         * **[!UICONTROL Finish]**&#x200B;을(를) 클릭합니다.

      1. 세그먼트 이름 지정:

         * 워크플로우에서 **[!UICONTROL Data extraction (File)]** 활동을 두 번 클릭합니다.

         * **[!UICONTROL Data extraction (File)]** 탭의 **[!UICONTROL File name]** 필드에 확장명이 &quot;`.added`&quot;인 세그먼트 이름을 입력합니다(예: PaidSubscribers.added).

           세그먼트 이름이 이미 있지 않아야 합니다. 세그먼트 이름은 대/소문자를 구분하며 ASCII 문자로 구성되어야 하지만 밑줄(`_`)은 포함할 수 없습니다.

           그러나 특정 [!DNL Google Ad] 계정에 세그먼트를 추가하려면 밑줄 및 [!UICONTROL User SE Account ID](네트워크 계정 ID가 아닌 [!DNL Google Ads] 계정에 대한 검색, 소셜 및 Commerce의 ID)을 사용하여 세그먼트 이름을 추가하십시오.

           `_<User SE Account ID>`

           예: Paid_Subscribers_1234.added

           >[!NOTE]
           >
           >이는 파일 이름에서 밑줄을 금지하는 규칙의 예외입니다.

           그렇지 않으면 Search, Social 및 Commerce이 광고주에 대해 동기화 중인 모든 [!DNL Google Ads] 계정에 세그먼트가 추가됩니다.

         * **[!UICONTROL Generate an outbound transition]**&#x200B;에 대한 옵션을 선택한 상태로 두십시오.

         * **[!UICONTROL Ok]**&#x200B;을(를) 클릭합니다.

      1. 데이터를 보낼 외부 계정을 지정합니다.

         * 워크플로우에서 **[!UICONTROL File Transfer]** 활동을 두 번 클릭합니다.

         * **[!UICONTROL File Transfer]** 탭의 **[!UICONTROL Remote server]** 섹션에서 **[!UICONTROL Use an external account]** 옵션을 선택합니다.

         * **[!UICONTROL External account]** 필드에서 2단계에서 만든 외부 계정에 대한 레이블을 선택합니다.

         * **[!UICONTROL Server folder]** 필드에서 외부 계정의 [!UICONTROL Account] 필드 값을 선택합니다.

         * (선택 사항) **[!UICONTROL Schedule]** 탭에서 파일 전송에 다른 일정을 지정합니다.

           기본적으로 워크플로우는 00:00(자정)에 실행되므로 모든 레코드가 처리됩니다. 지연을 최소화하려면 워크플로우가 늦어도 18:00까지 실행되도록 예약합니다.

         * **[!UICONTROL Ok]**&#x200B;을(를) 클릭합니다.

Search, Social 및 Commerce은 30분마다(광고주 시간대의 NN:30 및 NN:59에서) 디렉터리를 확인하고 찾은 파일을 다른 위치로 이동한 다음 데이터에서 자동으로 대상을 만들고 22:00(오후 10) Google으로 푸시합니다. Search, Social 및 Commerce은 30분마다 이메일 목록에 대한 업데이트(추가 및 빼기)를 계속 확인하고 매일 22:00에 그에 따라 [!DNL Google Ads]의 대상자를 업데이트합니다.

>[!NOTE]
>
>* 처리 주기 사이에 두 개 이상의 파일 버전을 업로드하면 가장 최근 파일이 사용됩니다.
>
>* Search, Social 및 Commerce은 [!DNL Google Ads] 대상자를 만들거나 편집하는 데 사용되는 전자 메일 목록의 고객 데이터를 저장하지 않습니다.
>
>* [!DNL Google Ads]이(가) 대상자에 대한 업데이트를 처리하는 데 시간이 걸릴 수 있습니다.
>
>* 고객 일치의 작동 방식과 제한 사항에 대해서는 [[!DNL Google Ads] 설명서를 참조하십시오](https://support.google.com/displayvideo/answer/9539301).

>[!MORELIKETHIS]
>
>* [대상자 정보](audience-about.md)
>* [고객 일치 대상자 만들기 [!DNL Google Ads] 출처 [!DNL Adobe] 대상자](google-audience-from-adobe-audience.md)
>* [고객 데이터 목록을 사용하여 고객 일치 대상 관리](audience-from-customer-data-list.md)
>* [동적 리마케팅 대상자 관리](audience-dynamic-remarketing-manage.md)
