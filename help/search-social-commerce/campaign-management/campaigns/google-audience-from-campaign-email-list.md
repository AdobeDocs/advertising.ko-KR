---
title: 만들기 [!DNL Google Ads] Adobe Campaign 이메일 목록의 고객 일치 대상
description: 을(를) 만드는 방법 알아보기 [!DNL Google Ads] 기존 Adobe Campaign 이메일 목록의 고객 일치 대상입니다.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 0%

---

# 만들기 [!DNL Google Ads] Adobe Campaign 이메일 목록의 고객 일치 대상

*[!DNL Google Ads]고객 대응에만 적합한 계정*

다음을 만들 수 있습니다. [!DNL Google Ads] 에서 계정 링크 및 워크플로우를 설정하여 Adobe Campaign 내의 이메일 목록에서 고객을 일치시키십시오. [!DNL Campaign].

이렇게 하려면 다음에 대한 액세스 권한이 필요합니다. [!DNL Campaign] 인스턴스 및 Adobe 계정 팀에서 제공할 필수 워크플로가 포함된 XML 파일입니다. 지침은 의 다양한 버전에 따라 다를 수 있습니다 [!DNL Campaign]. 필요한 경우 Adobe 계정 팀에서에서 워크플로우를 설정할 수 있습니다. [!DNL Campaign].

1. Advertising Search, Social 및 Commerce에서 제공한 SFTP 계정에 대한 자격 증명을 획득합니다.

1. 위치 [!DNL Campaign], 이메일 목록을 Advertising Search, Social 및 Commerce로 게재 설정:

   1. 만들기 [외부 계정](https://experienceleague.adobe.com/docs/campaign-standard/using/administrating/application-settings/external-accounts.html) 검색, 소셜 및 상거래에서 제공한 SFTP 계정을 연결하려면:

      1. 왼쪽 메뉴에서 **\[Adobe Campaign v6\] > [!UICONTROL Platform] >[!UICONTROL External Accounts]**.

      1. 클릭 ![계정 만들기](/help/search-social-commerce/assets/campaign-create-account.png "계정 만들기").

      1. 계정에 대한 레이블을 입력하고 다음을 선택합니다. **[!UICONTROL SFTP]** 계정 유형으로 선택해야 합니다.

      1. 에 대한 URL 및 포트 번호 입력 [!DNL Adobe] SFTP 서버 및 광고주의 폴더 이름, 사용자 이름 및 암호입니다.

      1. 클릭 **[!UICONTROL Save]**.
   1. 위치 [!DNL Campaign Client], 이메일 데이터를 보내는 데 필요한 워크플로가 포함된 데이터 패키지를 설치합니다.

      1. 메뉴 모음에서 다음 위치로 이동합니다 **[!UICONTROL Tools]> [!UICONTROL Advanced] >[!UICONTROL Import Package]**.

      1. 선택 **[!UICONTROL Install a package from a file]**&#x200B;을 클릭한 다음 을 클릭합니다 **[!UICONTROL Next]**.

      1. 데이터 패키지 파일(`AMO_Workflow.xml`) 장치 또는 네트워크에서 다음을 클릭합니다. **[!UICONTROL Next]**.

      1. 클릭 **[!UICONTROL Start]** 워크플로우가 설치될 때까지 기다립니다.
   1. 설치된 워크플로우를 편집하여 데이터 쿼리에 대한 필터를 선택적으로 편집하고 새 대상 이름 및 외부 SFTP 계정을 식별합니다.

      1. 다음으로 이동 **[!UICONTROL Administration]> [!UICONTROL Configuration] > [!UICONTROL Package management] >[!UICONTROL Installed packages]** 패키지를 엽니다.

      1. (선택 사항) 데이터에 대한 필터를 편집합니다.

         * 워크플로우에서 쿼리 활동(예: ForkTransition 1)을 두 번 클릭합니다.

         * 필터 표현식을 편집합니다.

         * 클릭 **[!UICONTROL Finish]**.
      1. 세그먼트 이름 지정:

         * 워크플로우에서 활동을 두 번 클릭합니다 **[!UICONTROL Data extraction (File)]**.

         * 다음에 대한 **[!UICONTROL Data extraction (File)]** 탭, **[!UICONTROL File name]** 필드에 확장자가 인 세그먼트 이름을 입력합니다.`.added`&quot;(예: PaidSubscribers.added).

            세그먼트 이름이 이미 있지 않아야 합니다. 세그먼트 이름은 대소문자를 구분하며 ASCII 문자로 구성되어야 하지만 밑줄(`_`).

            그러나 세그먼트를 특정 항목에 추가하려면 [!DNL Google Ad] account를 선택한 다음 밑줄 및 [!UICONTROL User SE Account ID] (검색, 소셜 및 상거래의 ID [!DNL Google Ads] 네트워크 계정 ID가 아닌 계정):

            `_<User SE Account ID>`

            예: Paid_Subscribers_1234.added

            >[!NOTE]
            >
            >이는 파일 이름에서 밑줄을 금지하는 규칙의 예외입니다.

            그렇지 않으면 세그먼트가 모든 항목에 추가됩니다 [!DNL Google Ads] 광고주에 대해 검색, 소셜 및 상거래를 동기화하는 계정입니다.

         * 옵션을 다음으로 유지 **[!UICONTROL Generate an outbound transition]** 선택됨.

         * 클릭 **[!UICONTROL Ok]**.
      1. 데이터를 보낼 외부 계정을 지정합니다.

         * 워크플로우에서 활동을 두 번 클릭합니다 **[!UICONTROL File Transfer]**.

         * 다음에 대한 **[!UICONTROL File Transfer]** 탭, **[!UICONTROL Remote server]** 섹션에서 다음 옵션을 선택합니다. **[!UICONTROL Use an external account]**.

         * 다음에서 **[!UICONTROL External account]** 필드에서 2단계에서 만든 외부 계정에 대한 레이블을 선택합니다.

         * 다음에서 **[!UICONTROL Server folder]** 필드에서 다음에 대한 값을 선택합니다. [!UICONTROL Account] 외부 계정용 필드.

         * (선택 사항) **[!UICONTROL Schedule]** 탭에서 파일 전송에 대해 다른 일정을 지정합니다.

            기본적으로 워크플로우는 00:00(자정)에 실행되므로 모든 레코드가 처리됩니다. 지연을 최소화하려면 워크플로우가 늦어도 18:00까지 실행되도록 예약합니다.

         * 클릭 **[!UICONTROL Ok]**.





Search, Social 및 Commerce는 30분마다(광고주 시간대의 NN:30 및 NN:59에서) 디렉터리를 확인하고 찾은 파일을 다른 위치로 이동한 다음 데이터에서 자동으로 대상을 만들고 22:00(오후 10) Google으로 푸시합니다. Search, Social 및 Commerce에서는 30분마다 이메일 목록에 대한 업데이트(추가 및 빼기)를 계속 확인하고 대상자를 업데이트합니다. [!DNL Google Ads] 따라서 매일 22:00에.

>[!NOTE]
>
>* 처리 주기 사이에 두 개 이상의 파일 버전을 업로드하면 가장 최근 파일이 사용됩니다.
>
>* Search, Social 및 Commerce는 를 만들거나 편집하는 데 사용되는 이메일 목록의 고객 데이터를 저장하지 않습니다. [!DNL Google Ads] 대상입니다.
>
>* [!DNL Google Ads] 대상자에 대한 업데이트를 처리하는 데 시간이 걸릴 수 있습니다.
>
>* 다음을 참조하십시오 [[!DNL Google Ads] 고객 일치 작동 방식 및 제한 사항에 대한 설명서](https://support.google.com/displayvideo/answer/9539301).


>[!MORELIKETHIS]
>
>* [대상자 기본 정보](audience-about.md)
>* [만들기 [!DNL Google Ads] 의 고객 일치 대상 [!DNL Adobe] 대상](google-audience-from-adobe-audience.md)
>* [고객 데이터 목록을 사용하여 고객 일치 대상 관리](audience-from-customer-data-list.md)
>* [동적 리마케팅 대상자 관리](audience-dynamic-remarketing-manage.md)

