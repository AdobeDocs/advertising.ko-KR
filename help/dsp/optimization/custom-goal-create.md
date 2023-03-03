---
title: 사용자 지정 목표 만들기
description: 사용자 지정 목표 만들기
feature: DSP Optimization
exl-id: 81b0acfa-085d-495b-9516-576b952b1307
source-git-commit: 14f78b89dea8cc680756232c6116975c652feee5
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 0%

---

# 사용자 지정 목표 만들기

다음과 같이 사용자 정의 목표를 생성할 수 있습니다. *목표* 다음 범위 내 [!DNL Adobe Advertising Search].

사용자 지정 목표를 만들려면 DSP 계정이 [!DNL Search] 내에서 동일한 Adobe Experience Cloud 조직 ID를 가진 계정 [!DNL Search] 클라이언트 설정. DSP 계정이 [!DNL Search] 계정, Adobe 계정 팀에 문의하십시오.

>[!TIP]
>
>다음을 참조하십시오. [사용자 정의 목표 생성을 위한 우수 사례](custom-goal-best-practices.md) 사용자 지정 목표를 구성하는 방법에 대한 팁입니다.

1. 에 로그인 [!DNL Adobe Advertising Search] at (북미 사용자) [`https://enterprise-na.efrontier.com`](https://enterprise-na.efrontier.com) 또는 (다른 모든 사용자) [`https://enterprise-intl.efrontier.com`](https://enterprise-intl.efrontier.com).
1. 목표에 포함할 지표가 추적되고 제품에서 사용할 수 있는지 확인하고 표시 이름을 포함하십시오.
   1. 메인 메뉴에서 **[!UICONTROL Search]** > **[!UICONTROL Admin]>[!UICONTROL Transaction Properties]**.
   1. 지표를 찾고 다음을 확인합니다. **[!UICONTROL Show in UI and Reports]** 지표에 대해 활성화됩니다.
   1. 지표에 값이 없는 경우 **[!UICONTROL Display Name]** 열에서 셀을 클릭하고 표시 이름을 입력한 다음 **[!UICONTROL Apply].**
1. 사용자 정의 목표를 다음으로 만들기 *목표*:
   1. 메인 메뉴에서 **[!UICONTROL Search]** > **[!UICONTROL Optimization]>[!UICONTROL Objectives]**.
   1. 도구 모음에서 를 클릭합니다 **[!UICONTROL Create objective].**
   1. 목표 설정을 입력합니다.
      1. 다음에서 **[!UICONTROL Change Objective Name]** 필드에 목표명을 입력합니다.

         목표 이름이에 표시됩니다. [!UICONTROL Custom Goals] 를 DSP 패키지 설정에 나열합니다.

      1. 속성을 목표와 연결:

         >[!NOTE]
         >
         > 광고주에 대해 추적된 모든 트랜잭션 속성은 기본적으로 [!UICONTROL Available Properties] 목록을 표시합니다.

         * 속성 및 해당 가중치가 있는 CSV 파일을 가져오려면 **[!UICONTROL Import]** 가져올 파일을 찾습니다.

            가져온 속성은 광고주에 대해 이미 존재해야 합니다. 이름은 대소문자를 구분하지 않습니다.

            가져온 속성은 지정된 기존 속성을 대체합니다.

         * 기본 가중치(1)를 사용하여 첫 번째 속성을 수동으로 지정하려면 광고주에 대해 추적된 모든 트랜잭션 속성 목록에서 을 선택합니다.

         * 기본 가중치(1)를 사용하여 다른 속성을 수동으로 추가하려면 **[!UICONTROL +]** .

            >[!TIP]
            >
            > 목록에서 등록 정보를 검색하려면 등록 정보 이름 내의 아무 곳에나 문자열을 입력합니다.

         * 여러 속성을 수동으로 추가하려면 **[!UICONTROL Add Multiple Properties].** 추가할 각 속성에 대해 [!UICONTROL Available Properties] 열을 만든 다음 [!UICONTROL Added Properties] 열. 속성 추가를 마쳤으면 **[!UICONTROL Add]**.

            >[!TIP]
            >
            >* 목록에서 등록 정보를 검색하려면 입력 필드의 등록 정보 이름 내 아무 곳에나 문자열을 입력합니다.
            >* 보고서에서 제외된 속성을 제외하도록 목록을 필터링하려면 옵션을 선택합니다 **[!UICONTROL Hide properties excluded from reports].**


         * (목표에 여러 속성이 들어 있는 경우) 목표에 있는 다른 속성에 상대적인 속성의 가중치를 변경하려면 **[!UICONTROL Weight]** 필드.
      1. 설정 하단에서 **[!UICONTROL Save]**.


목표를 만들면 최적화 목표가 &quot;&quot;일 때 이를 사용자 지정 목표로 DSP 패키지에 할당할 수 있습니다.[!UICONTROL Highest ROAS - Custom Goal]&quot; 또는 &quot;[!UICONTROL Lowest CPA - Custom Goal].&quot;

>[!TIP]
>
>최적의 성능을 위해서는 사용자 지정 목표(목표)의 결합된 지표가 하루에 10개 이상의 전환을 수행해야 합니다. 그렇지 않은 경우 제품 페이지나 애플리케이션 시작과 같은 추가 지원 이벤트(트랜잭션 속성)를 목표에 추가하는 것이 좋습니다. 다음을 참조하십시오 [사용자 지정 목표 빌드를 위한 우수 사례](custom-goal-best-practices.md) 지침을 참조하십시오.

>[!MORELIKETHIS]
>
>* [사용자 정의 목표 정보](custom-goal-about.md)
>* [사용자 지정 목표 빌드를 위한 우수 사례](custom-goal-best-practices.md)
>* [최적화 목표 및 사용 방법](optimization-goals.md)
>* [패키지 설정](/help/dsp/campaign-management/packages/package-settings.md)
> * [DSP이 캠페인을 최적화하는 방법](optimization-how-dsp-optimizes-campaigns.md)

