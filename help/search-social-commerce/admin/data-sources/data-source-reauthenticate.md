---
title: 재인증 [!DNL Google Analytics] 데이터 소스
description: 을(를) 재인증하는 방법 알아보기 [!DNL Google Analytics] 연결된 암호를 변경하거나 인증서가 만료된 경우 데이터 소스.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 0%

---

# 재인증 [!DNL Google Analytics] 데이터 소스

*기관 관리자, 기관 계정 관리자, Adobe 계정 관리자 및 관리자만*

데이터 소스에 사용되는 이메일 계정의 암호를 변경하는 경우 또는 [!DNL OAuth] 계정에 대한 인증서가 만료되면 이메일 계정에 대한 열려 있는 모든 연결이 닫히고 데이터 동기화를 다시 시작하려면 다시 인증해야 합니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Admin] >[!UICONTROL Data Source Setup]**.

1. 다시 인증하려는 데이터 소스 옆에 있는 확인란을 선택합니다.

1. 데이터 테이블 위의 도구 모음에서 ![편집](/help/search-social-commerce/assets/edit.png "편집").

1. 편집 [데이터 소스 설정](data-source-settings.md):

   1. 다음에서 [!UICONTROL Connect to Google Analytics] 섹션에서 다음을 수행합니다.

      1. (필요한 경우) 이 데이터 소스의 데이터에 액세스하는 데 사용할 새 이메일 주소를 입력합니다. 전자 메일 주소를 다음에 등록해야 합니다. [!DNL Google] 및 을(를) 위한 &quot;읽기 및 분석&quot; 권한이 있어야 합니다. [!DNL Google Analytics] 계정입니다. 다음을 참조하십시오. [에서 사용자 권한을 할당하는 지침 [!DNL Google Analytics]](https://support.google.com/analytics/answer/9305587).

         >[!TIP]
         >
         >특정 항목만 [!DNL Google Analytics] 속성 및 보기는 검색, 소셜 및 상거래 내에서 사용할 수 있으며 해당 속성 및 보기만 액세스할 수 있는 이메일 주소로 로그인합니다.
   1. 계정의 지표에 액세스할 수 있도록 검색, 소셜 및 상거래를 승인하려면 확인란을 선택합니다.

   1. 클릭 **[!UICONTROL Re-Authenticate]**.


1. 클릭 **[!UICONTROL Post]**.

>[!MORELIKETHIS]
>
>* [동기화 기본 정보 [!DNL Google Analytics] 전환 지표](data-source-about.md)
>* [구성 사전 요구 사항 [!DNL Google Analytics] 데이터 소스](data-source-prerequisites.md)
>* [구성 [!DNL Google Analytics] 데이터 소스로 보기](data-source-configure.md)
>* [편집 [!DNL Google Analytics] 데이터 소스](data-source-edit.md)
>* [데이터 소스 동기화 일시 중지](data-source-pause.md)
>* [[!DNL Google Analytics] 데이터 소스 설정](data-source-settings.md)
>* [부록 - 사용 가능 [!DNL Google Analytics] 지표](data-source-ga-metrics.md)

