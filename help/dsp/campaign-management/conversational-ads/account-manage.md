---
title: '[!DNL ChatGPT Ads]개의 대화형 광고 계정 관리'
description: AI 비서 대화 내에 광고를 배치하는 베타 기능인 [!DNL ChatGPT Ads] 채팅 카드 광고의 계정을 만들고 관리하는 방법에 대해 알아봅니다.
product_v2:
  - id: a829a185-511f-4bf8-8dcf-9e684f8011cf
    internal-label: Advertising
feature_v2:
  - id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
    internal-label: Demand Side Platform
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: cb25ab04e8fef5d00935e5325a897b1de97e2674
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 0%
---
# [!DNL ChatGPT Ads]개의 대화형 광고 계정 관리

*Beta 기능*

Adobe DSP과 [!DNL OpenAI Ads]의 통합을 통해 [!DNL ChatGPT]개의 대화 내에 표시되는 [!DNL ChatGPT Ads]개의 채팅 카드 광고를 실행할 수 있습니다. 이 기능을 위해 DSP은 대화형 광고 계정을 만들고 조직을 대신하여 미디어를 구입합니다. ads.openai.com에서 광고 계정에 액세스할 수 없습니다. 이 기능을 사용하여 [!DNL ChatGPT Ads]과(와) 직접 관계를 설정하지 않고도 AI 미디어를 테스트합니다.

구조가 다른 일반 DSP 캠페인과 별도로 캠페인, 광고 그룹 및 광고를 포함한 [!DNL ChatGPT Ads] 대화 광고 계정을 관리합니다. 또한 DSP 캠페인과 별도로 [캠페인, 광고 그룹 및 광고에 대한 성과 데이터를  [!DNL ChatGPT Ads] 볼 수 있습니다](campaign-manage.md#campaign-views-about).

## 적격성

다음은 이 기능의 적격성을 결정합니다.

* **기존 [!DNL Search, Social, & Commerce] 고객:** 광고주가 이미 [!DNL Search, Social, & Commerce]을(를) 사용하고 있는 경우 [DSP이 아닌 검색, 소셜 및 Commerce에서  [!DNL ChatGPT Ads] 캠페인을 만들고 관리](/help/search-social-commerce/new-ui/manage/campaigns/campaign-manage.md)합니다.

* **제한된 업종:** 제한된 범주(예: 금융 또는 의료)의 광고주는 대화 광고 계정이나 캠페인을 만들 수 없습니다.

선택한 광고주가 적격하지 않은 경우 [!UICONTROL Accounts] 및 [!UICONTROL Campaigns] 탭에 원인이 표시됩니다. 광고주 선택기를 사용하여 다른 광고주로 전환할 수 있습니다.

이 기능을 사용하려면 Adobe 계정 팀에 문의하여 온보딩 프로세스를 시작하십시오.

## 청구

 [!DNL ChatGPT Ads] account](#account-settings)에 사용된 [통화 및 시간대에 관계없이 DSP 계정에 대한 청구 통화 및 청구 시간대를 사용하여 다른 인보이스와 함께 월말에 [!DNL ChatGPT Ads] 사용에 대해 청구됩니다. 청구 질문이 있는 경우 Adobe 계정 팀에 문의하십시오.

## [!UICONTROL Conversational Ads Beta] > [!UICONTROL Accounts] 보기 {#accounts-view}

[!UICONTROL Conversational Ads Beta] > [!UICONTROL Accounts] 탭에는 선택한 광고주의 [!DNL OpenAI] 계정이 나열됩니다. 각 계정에 대한 정보는 다음과 같습니다.

**[!UICONTROL Status]:** 계정이 현재 광고를 제공하고 있는지 여부: *활성* 또는 *일시 중지됨*. 계정의 상태를 변경할 수 없습니다. 계정을 일시 중지하거나 다시 활성화하려면 Adobe 계정 팀에 문의하십시오.

**[!UICONTROL Review status]:** [!DNL OpenAI] 검토 상태: *검토 중*, *승인됨* 또는 *승인되지 않음*. 가능한 경우 커서를 해당 사유의 상태 위에 놓습니다.

**[!UICONTROL Active campaigns]:** 계정의 현재 활성 캠페인 수입니다.

**[!UICONTROL Cost]:** 계정의 총 지출입니다.

### 사용 가능한 작업

* [계정 제한 보기](#account-limits)

<!-- * [Refresh information about your accounts](#refresh) -- Add topic below. -->

* [계정 만들기](#account-create)

* [계정 편집](#account-edit)

* [계정 목록 새로 고침](#account-refresh)

* [DSP 메인 메뉴로 돌아가기](#return-to-menu)

## 계정 관리

### 계정 제한 보기 {#account-limits}

계정 제한은 특정 날짜 범위 동안의 계정 총 지출을 제한합니다. 계정의 제한을 볼 수 있지만, Adobe 계정 팀만 제한을 생성, 편집 또는 제거할 수 있습니다.

1. 주 메뉴에서 **[!UICONTROL Conversational Ads Beta]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Accounts]** 보기에서 계정 행 위에 커서를 놓고 **[!UICONTROL ...]>[!UICONTROL View account limit]**&#x200B;을(를) 클릭합니다.

[!UICONTROL Account limits] 페이지에는 계정의 각 제한이 나열됩니다.

**[!UICONTROL Name]:** 한도 이름입니다.

**[!UICONTROL Amount]:** 제한 기간 동안의 총 지출 한도입니다.

**[!UICONTROL Period]:** 제한이 적용되는 날짜 범위입니다.

**[!UICONTROL Status]:** *활성*, *예정* 또는 *완료됨*.

**[!UICONTROL Spent]:** 제한 기간 내에 지금까지 사용한 금액입니다.

>[!NOTE]
>
>완료된 제한을 편집하거나 제거할 수 없으며, 동일한 계정에 대한 제한 기간은 겹칠 수 없습니다.

### [!DNL ChatGPT Ads] 대화형 광고 계정 만들기 {#account-create}

광고주에 대해 두 개 이상의 [!DNL ChatGPT Ads] 계정을 만들려면 Adobe 계정 팀에 문의하십시오.

1. 주 메뉴에서 **[!UICONTROL Conversational Ads Beta]**&#x200B;을(를) 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * (첫 번째 계정만 해당) 시작 화면에서 **[!UICONTROL Create an Account]**&#x200B;을(를) 클릭합니다.

   * **[!UICONTROL Accounts]** 보기에서 광고주를 선택한 다음 **[!UICONTROL Create Account]**&#x200B;을(를) 클릭합니다.

1. [계정 설정](#account-settings)을 지정하십시오.

1. **[!UICONTROL I agree to the Terms and Conditions]** 확인란을 선택합니다.

1. **[!UICONTROL Create account]**&#x200B;을(를) 클릭합니다.

[!DNL OpenAI]이(가) 새 계정을 검토하는 동안 일시 중지된 상태에서 새 계정이 만들어집니다. DSP은 승인되면 계정을 활성화합니다.

### [!DNL ChatGPT Ads] 대화형 광고 계정 편집 {#account-edit}

계정의 법적 비즈니스 이름과 웹 사이트를 만든 후 편집할 수 있습니다.

1. 주 메뉴에서 **[!UICONTROL Conversational Ads Beta]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Accounts]** 보기에서 계정 행 위에 커서를 놓고 **[!UICONTROL ...]>[!UICONTROL Edit account]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Legal Business Name]** 및/또는 **[!UICONTROL Advertiser Website]** 편집 필드에 대한 자세한 내용은 &quot;[계정 설정](#account-settings)&quot;을 참조하세요.

1. **[!UICONTROL Save changes]**&#x200B;을(를) 클릭합니다.

>[!IMPORTANT]
>
>변경 내용을 저장하면 계정에 대한 [!DNL OpenAI]의 검토가 다시 시작됩니다. 계정이 다시 승인될 때까지 해당 계정은 광고를 다시 게재하지 않습니다.

### 계정 목록 새로 고침 {#account-refresh}

다른 사용자가 변경 또는 추가했을 수 있는 경우 계정 목록을 다시 표시합니다.

1. 주 메뉴에서 **[!UICONTROL Conversational Ads Beta]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Accounts]** 보기에서 계정 목록 위에 있는 **[!UICONTROL Refresh]**&#x200B;을(를) 클릭합니다.

### DSP 메인 메뉴로 돌아가기 {#return-to-menu}

* 주 메뉴 위에서 **[!UICONTROL Back to DSP]**&#x200B;을(를) 클릭합니다.

### [!DNL ChatGPT Ads] 대화 광고 계정 설정 {#account-settings}

**[!UICONTROL Legal Business Name]:** 조직의 등록된 비즈니스 이름입니다.

**[!UICONTROL Advertiser Website]:** `http://` 또는 `https://`(으)로 시작하는 광고주 웹 사이트의 URL입니다.

**[!UICONTROL Country]:** 조직이 법적으로 등록된 국가(광고를 실행할 국가가 아님). 조직의 DSP 계약에 사용되는 국가와 동일해야 합니다. 계정을 저장한 후에는 이 값을 변경할 수 없습니다.

**[!UICONTROL Currency]:**(읽기 전용) Adobe 계정 팀이 [!DNL ChatGPT Ads] 계정에 대해 설정하는 통화입니다. 이는 DSP 내 다른 곳에서 볼 수 있는 DSP 계정에 대한 통화와 다를 수 있습니다. **참고:** 이 값에 관계없이 모든 사용 청구서는 DSP 계정에 사용되는 *청구 통화*&#x200B;로 표시됩니다.

**[!UICONTROL Timezone]:**(읽기 전용) Adobe 계정 팀이 [!DNL ChatGPT Ads] 계정에 대해 설정하는 시간대입니다. 이는 DSP 계정에 사용된 시간대와 다를 수 있으며 DSP 내 다른 곳에서 볼 수 있습니다. **참고:** 이 값에 관계없이 모든 사용 요금은 DSP 계정에 사용되는 *청구 시간대*&#x200B;를 나타냅니다.

**[!UICONTROL Favicon]:** 계정의 웹 사이트 favicon으로 사용할 이미지 파일입니다.<!-- How is this used within this context? --> 주소 표시줄, 탭 또는 책갈피와 같은 다양한 위치에 파비콘이 브라우저에 표시됩니다. 파일은 JPG, PNG 또는 WEBP 형식이어야 하며 최소 256x256픽셀이어야 합니다.

아이콘을 업로드하려면 **[!UICONTROL Upload favicon]**&#x200B;을(를) 클릭한 다음 장치 또는 네트워크에서 파일을 찾아 선택합니다.

**[!UICONTROL I agree to the Terms and Conditions]:** 모든 약관에 동의함을 나타내는 확인란입니다. 계정을 만들거나 계정 설정을 업데이트하려면 확인란을 선택합니다.

>[!MORELIKETHIS]
>
>* [대화형 광고 캠페인 관리](campaign-manage.md)
