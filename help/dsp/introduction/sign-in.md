---
title: DSP에 로그인
description: DSP에 로그인하는 방법에 대해 알아봅니다.
feature: DSP Introduction
exl-id: 1704cd75-81f8-4715-a177-69a03093ba1d
source-git-commit: a7e28cb2e37e1c9b6951f844b5f542ae2c8ac1a0
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 0%

---

# Adobe Advertising DSP에 로그인

Adobe Advertising DSP이 로그인 인증을 위해 Adobe Identity Management 서비스(IMS)로 전환하고 있습니다. IMS는 Real-Time Customer Data Platform, Customer Journey Analytics, Target 및 Analytics를 포함하여 IMS를 지원하는 모든 [!DNL Adobe] 제품에 SSO(Single Sign-On) 액세스를 제공합니다. 변경 사항:

* [!DNL Adobe ID] 하나를 사용하여 Experience Cloud 로그인 페이지 또는 기존 DSP 로그인 페이지에서 [!DNL Adobe] 제품 간에 로그인할 수 있습니다. [!DNL Adobe ID]에서 사용자 프로필 관리를 제공합니다. 향후 릴리스에서는 상단 메뉴에서 DSP 계정, IMS 조직 계정 및 [!DNL Adobe] 제품을 변경할 수 있습니다.

* 엔터프라이즈 인증이 지원됩니다.

* 매시간 로그인하는 대신 24시간 동안 로그인할 수 있습니다.

현재 DSP 자격 증명은 변경을 준비할 수 있도록 2025년 6월 26일까지 활성 상태로 유지됩니다.

## 인증에 기존 DSP 로그인 사용

* [advertising.adobe.com](https://advertising.adobe.com)&#x200B;(으)로 이동한 다음 기존 DSP 자격 증명을 사용하여 로그인합니다.

## 인증에 [!DNL Adobe ID] 사용

1. 다음 로그인 화면 중 하나를 엽니다.

   * [advertising.adobe.com](https://advertising.adobe.com)&#x200B;(으)로 이동합니다. &quot;[!UICONTROL Sign in with the Adobe Experience Cloud account]&quot; 아래에서 **[!UICONTROL Continue]**&#x200B;을(를) 클릭합니다.

   * [experience.adobe.com](https://experience.adobe.com)&#x200B;(으)로 이동합니다.

1. 자격 증명 입력:

   * 이미 [!DNL Adobe] 계정을 사용하고 있다면 기존 자격 증명으로 로그인하십시오.

   * [!DNL Adobe] 계정이 없는 경우 [!DNL Adobe] 계정을 만들 수 있도록 초대하는 전자 메일을 찾습니다. 각 DSP 계정에 대해 하나의 초대를 받게 됩니다. 이메일의 링크를 따라 자격 증명을 설정합니다. DSP 계정이 여러 개 있는 경우 지침에 따라 연결합니다.

1. 조직 선택:

   * 메시지가 표시되면 **개인 계정&quot; 또는 &#x200B;** 회사 또는 학교 계정**&#x200B;을 선택합니다.

   * 여러 IMS 조직에 액세스할 수 있는 경우 올바른 조직을 선택합니다.

사용자 프로필 관리를 포함하여 Experience Cloud 인터페이스에 대한 자세한 내용은 &quot;[Experience Cloud 인터페이스 및 관리](https://experienceleague.adobe.com/en/docs/core-services/interface/experience-cloud)&quot;를 참조하십시오.

### 문제 해결

일반적인 로그인 문제에 대해서는 &quot;[Adobe 계정 로그인 문제 해결](https://helpx.adobe.com/manage-account/kb/account-password-sign-help.linkfree.html)&quot;도 참조하십시오.

#### 새 [!DNL Adobe] IMS 로그인을 활성화하기 위한 필수 구성 요소가 있습니까?

새 로그인 계정을 추가하려면 Adobe 계정 팀과 이메일 주소를 공유하십시오. 팀은 DSP이 프로비저닝된 IMS 조직의 사용자 목록에 사용자 주소를 추가합니다.

그동안 사용자는 기존 DSP 자격 증명을 계속 사용할 수 있습니다.

#### Adobe IMS 계정을 사용하여 로그인하면 adobe.advertising.com 로그인 페이지로 다시 리디렉션됩니다.

사용 중인 이메일이 IMS 조직에 추가되었는지 IMS 조직 관리자에게 문의하십시오. 관리자가 사용자가 IMS 조직에 추가된 것을 확인한 경우 Adobe 계정 팀에 DSP을 사용할 계정을 프로비저닝하도록 요청합니다.

그동안 기존 DSP 자격 증명을 계속 사용할 수 있습니다.

#### 잘못된 전자 메일 주소를 사용하여 로그인했습니다. 이 전자 메일 주소는 [!DNL Adobe]에 로그인했지만 DSP 액세스를 제공하지 않습니다.

1. [experience.adobe.com](https://experience.adobe.com)&#x200B;(으)로 이동하여 로그아웃합니다.

1. [advertising.adobe.com](https://advertising.adobe.com)&#x200B;(으)로 이동하여 올바른 전자 메일 ID로 로그인합니다.

#### 내 [!DNL Adobe] IMS 계정과 DSP 계정이 다른 전자 메일로 등록되었습니다. [!DNL Adobe] IMS 계정을 사용하여 로그인하려면 어떻게 해야 합니까?

Adobe 계정 팀에 DSP을 사용하도록 기존 [!DNL Adobe] IMS 계정을 프로비저닝하도록 요청하십시오.
