---
title: ' [!DNL Google Analytics] 데이터 원본 재인증'
description: 연결된 암호를 변경하거나 인증서가 만료된 경우  [!DNL Google Analytics] 데이터 원본을 다시 인증하는 방법을 알아보세요.
role: User, Admin
exl-id: 624f0f0e-3f2f-45b1-b3dc-c1b107b4736f
feature: Search Admin, Search Data Sources
source-git-commit: d0f1c413134a0868ddec79ded7672af316267edd
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---

# [!DNL Google Analytics] 데이터 원본 재인증

*에이전시 관리자, 에이전시 계정 관리자, Adobe 계정 관리자 및 관리자만*

데이터 원본에 사용되는 전자 메일 계정의 암호를 변경하거나 해당 계정의 [!DNL OAuth] 인증서가 만료되면 전자 메일 계정에 대한 열려 있는 모든 연결이 닫히므로 데이터 동기화를 다시 시작하려면 다시 인증해야 합니다.

1. 메인 메뉴에서 **[!UICONTROL Search, Social, & Commerce]> [!UICONTROL Admin] >[!UICONTROL Data Source Setup]**&#x200B;을(를) 클릭합니다.

1. 다시 인증하려는 데이터 소스 옆에 있는 확인란을 선택합니다.

1. 데이터 테이블 위의 도구 모음에서 ![편집](/help/search-social-commerce/assets/edit.png "편집")을 클릭합니다.

1. [데이터 원본 설정](data-source-settings.md)을(를) 편집합니다.

   1. [!UICONTROL Connect to Google Analytics] 섹션에서 다음을 수행합니다.

      1. (필요한 경우) 이 데이터 소스의 데이터에 액세스하는 데 사용할 새 이메일 주소를 입력합니다. 전자 메일 주소는 [!DNL Google] 계정에 등록되어야 하며 [!DNL Google Analytics] 계정에 대한 &quot;읽기 및 분석&quot; 권한이 있어야 합니다.  [!DNL Google Analytics][&#128279;](https://support.google.com/analytics/answer/9305587)에서 사용자 권한 할당에 대한 지침을 참조하세요.

         >[!TIP]
         >
         >검색, 소셜 및 Commerce 내에서 특정 [!DNL Google Analytics] 속성 및 보기만 사용할 수 있도록 하려면 해당 속성 및 보기에만 액세스할 수 있는 전자 메일 주소를 사용하여 로그인하십시오.

   1. 계정의 지표에 액세스할 수 있도록 검색, 소셜 및 Commerce을 승인하려면 확인란을 선택합니다.

   1. **[!UICONTROL Re-Authenticate]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Post]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [동기화 정보 [!DNL Google Analytics] 전환 지표](data-source-about.md)
>* [데이터 원본 [!DNL Google Analytics] 구성을 위한 필수 구성 요소](data-source-prerequisites.md)
>* [데이터 소스로  [!DNL Google Analytics] 보기 구성](data-source-configure.md)
>* [데이터 원본 편집 [!DNL Google Analytics] 2&rbrace;](data-source-edit.md)
>* [데이터 원본 동기화 일시 중지](data-source-pause.md)
>* [[!DNL Google Analytics] 데이터 원본 설정](data-source-settings.md)
>* [부록 - 사용 가능 [!DNL Google Analytics] 지표](data-source-ga-metrics.md)
