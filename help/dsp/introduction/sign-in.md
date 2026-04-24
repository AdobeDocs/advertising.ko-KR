---
title: DSP에 로그인
description: DSP에 로그인하는 방법에 대해 알아봅니다.
feature: DSP Introduction
exl-id: 1704cd75-81f8-4715-a177-69a03093ba1d
TQID: https://experienceleague.adobe.com/KjBIag8qcpMONcX6pS2IJot3IA4Q-KOq0Av-1VzAot4
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2:
  - id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: c4d69b3aac9c963d13e3083f71931e507e58e616
workflow-type: tm+mt
source-wordcount: 535
ht-degree: 0%

---

# Adobe Advertising DSP에 로그인

Adobe Advertising DSP이 로그인 인증을 위해 Adobe Identity Management 서비스(IMS)로 전환하고 있습니다. IMS는 Real-Time Customer Data Platform, Customer Journey Analytics, [!DNL Target] 및 [!DNL Analytics]을(를) 포함하여 IMS를 지원하는 모든 [!DNL Adobe] 제품에 Federated ID를 사용하여 SSO(Single Sign-On) 액세스를 제공합니다. 변경 사항:

* 하나의 [!DNL Adobe ID]을(를) 사용하여 Adobe CX Enterprise(이전 Adobe Experience Cloud) 로그인 페이지 또는 이전 DSP 로그인 페이지에서 [!DNL Adobe] 제품 간에 로그인할 수 있습니다. [!DNL Adobe ID]에서 사용자 프로필 관리를 제공합니다. 향후 릴리스에서는 상단 메뉴에서 DSP 계정, IMS 조직 계정 및 [!DNL Adobe] 제품을 변경할 수 있습니다.

* 엔터프라이즈 인증이 지원됩니다.

* 매시간 로그인하는 대신 24시간 동안 로그인할 수 있습니다.

현재 DSP 자격 증명은 변경을 준비할 수 있도록 잠시 동안 활성 상태로 유지됩니다.

## 인증에 기존 DSP 로그인 사용

* [advertising.adobe.com](https://advertising.adobe.com)&#x200B;(으)로 이동한 다음 기존 DSP 자격 증명을 사용하여 로그인합니다.

## 인증에 [!DNL Adobe ID] 사용

1. 다음 로그인 화면 중 하나를 엽니다.

   * [advertising.adobe.com](https://advertising.adobe.com)&#x200B;(으)로 이동합니다. &quot;[!UICONTROL Sign in with the Adobe Experience Cloud account]&quot; 아래에서 **[!UICONTROL Continue]**&#x200B;을(를) 클릭합니다.

   * [experience.adobe.com](https://experience.adobe.com)&#x200B;(으)로 이동합니다.

1. Enter your credentials:

   * If you already use an [!DNL Adobe] account, then sign in with your existing credentials.

   * If you don&#39;t have an [!DNL Adobe] account, then look for an email inviting you to create an [!DNL Adobe] account. You&#39;ll receive one invitation for each of your DSP accounts. Follow the link in the email to set up your credentials. If you have multiple DSP accounts, follow the instructions to link them.

1. Choose your organization:

   * If prompted, select either **[!UICONTROL Personal Account]&quot; or &#x200B;** [!UICONTROL Company or School Account]**.

   * If you have access to multiple IMS organizations, select the correct one.

사용자 프로필 관리를 포함하여 CX Enterprise 인터페이스에 대한 자세한 내용은 &quot;[CX Enterprise 인터페이스 및 관리](https://experienceleague.adobe.com/ko/docs/core-services/interface/experience-cloud)&quot;를 참조하십시오.

### 문제 해결

For general sign-in issues, see also &quot;[Solve Adobe account sign-in issues](https://helpx.adobe.com/kr/manage-account/kb/account-password-sign-help.linkfree.html).&quot;

#### Are there any prerequisites to enable a new [!DNL Adobe] IMS login?

To add a new login account, share the email address with your Adobe Account Team. The team will add your address to the user list for the IMS organization to which DSP has been provisioned.

In the meanwhile, the user can continue to use their legacy DSP credentials.

#### After signing in using an Adobe IMS account, I&#39;m redirected back to the adobe.advertising.com login page.

Check with your IMS organization administrator that the email you are using was added to the IMS organization. If the administrator confirms that you are added to the IMS organization, then ask your Adobe Account Team to provision your account to use DSP.

In the meanwhile, you can continue to use your legacy DSP credentials.

#### I signed in using an incorrect email address, which signed me into [!DNL Adobe] but doesn&#39;t provide DSP access.

1. Go to [experience.adobe.com](https://experience.adobe.com) and sign out.

1. Go to [advertising.adobe.com](https://advertising.adobe.com) and sign in with the correct email ID.

#### My [!DNL Adobe] IMS account and DSP account are registered with different emails. How do I sign in using my [!DNL Adobe] IMS account?

Ask your Adobe Account Team to provision your existing [!DNL Adobe] IMS account to use DSP.
