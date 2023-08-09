---
title: 구성 [!DNL Google Analytics] 데이터 소스로 보기
description: 에서 데이터 소스를 구성하는 방법 알아보기 [!DNL Google Analytics] 보기.
role: User, Admin
exl-id: 583cf9aa-861c-4faf-a707-1def4e983b93
feature: Search Admin, Search Data Sources
source-git-commit: 5141c332fc00e9eae62ef507d215dd435e86e8ba
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# 구성 [!DNL Google Analytics] 데이터 소스로 보기

*기관 관리자, 기관 계정 관리자, Adobe 계정 관리자 및 관리자만*

각 데이터 소스에 대해 하나의 데이터 소스를 생성할 수 있습니다. [!DNL Google Analytics] 계정, 등록 정보 및 보기 조합

단일 속성에 대해 여러 속성 또는 여러 보기의 지표를 통합하려면 각각에 대해 별도의 데이터 소스를 설정합니다.

1. [을(를) 통합하기 위한 모든 전제 조건을 수행합니다. [!DNL Google Analytics] account](data-source-prerequisites.md).

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Admin] >[!UICONTROL Data Source Setup]**.

1. 데이터 테이블 위의 도구 모음에서 ![만들기](/help/search-social-commerce/assets/add.png "만들기").

1. 다음에서 [!UICONTROL Deployment Prerequisites] 대화 상자에서 확인란을 선택하여 필요한 사용자 지정 차원 &quot;ef_id&quot;가 [!DNL Google Analytics] 계정 을 클릭한 다음 **[!UICONTROL Continue]**.

   조직의 다른 역할이 일부 전제 조건을 수행했을 수 있습니다. 필수 구성 요소에 대한 질문이 있는 경우 Adobe 계정 팀에 문의하십시오.

1. 다음을 입력합니다. [데이터 소스 설정](data-source-settings.md):

   1. 다음에서 **[!UICONTROL Connect to [!DNL Google Analytics]]** 섹션에서 다음을 수행합니다.

      1. 숫자 ID를 입력합니다. [!DNL Google Analytics] 계정입니다.

      1. 이 데이터 소스의 데이터에 액세스하는 데 사용할 이메일 주소를 입력하십시오. 전자 메일 주소를 다음에 등록해야 합니다. [!DNL Google] 및 을(를) 위한 &quot;읽기 및 분석&quot; 권한이 있어야 합니다. [!DNL Google Analytics] 계정입니다. 다음을 참조하십시오. [에서 사용자 권한을 할당하는 지침 [!DNL Google Analytics]](https://support.google.com/analytics/answer/9305587).

         >[!TIP]
         >
         >특정 항목만 [!DNL Google Analytics] Adobe Advertising 내에서 속성 및 보기를 사용할 수 있으며, 해당 속성 및 보기에만 액세스할 수 있는 이메일 주소를 사용하여 로그인합니다.

         >[!NOTE]
         >
         >나중에 이 이메일 계정의 암호를 변경하면 이메일 계정에 대한 모든 열려 있는 연결이 닫힙니다. 데이터 동기화를 재개하려면 이 페이지로 돌아가서 [재인증](data-source-reauthenticate.md).

      1. 계정의 지표에 액세스할 수 있도록 Adobe Advertising에게 권한을 부여하려면 확인란을 선택합니다.

      1. 클릭 **[!UICONTROL Authenticate]**.

   1. 다음에서 [!UICONTROL Account Details] 섹션에서 가져올 지표에 대한 속성 및 보기를 지정합니다. 또한 &quot;ef_id&quot; 쿼리 문자열 매개 변수의 값으로 채워지는 사용자 지정 차원을 지정합니다.

   1. 다음에서 [!UICONTROL Import Metrics] 섹션에서 피드에 포함할 지표를 지정합니다.

      제거할 수 없습니다. [!UICONTROL Pageviews], [!UICONTROL Sessions], [!UICONTROL Bounces], 또는 [!UICONTROL Session Duration]: 자동으로 포함됩니다. 데이터 없이 최대 16개의 유효한 지표 또는 지표를 추가할 수 있습니다.

      >[!WARNING]
      >
      >[!DNL Google Analytics] 단일 데이터 피드에서 최대 10개의 지표를 허용합니다. Search, Social 및 Commerce는 총 20개의 지표로 최대 2개의 피드를 지원할 수 있지만, 두 번째 피드를 사용하면 API 호출이 [!DNL Google Analytics]. 지표가 많은 경우 최적화를 위해 목표에 사용할 지표만 선택합니다. 자세한 내용 [에 대한 API 요청에 대한 할당량 및 호출 제한 [!DNL Google Analytics]](https://developers.google.com/analytics/devguides/reporting/core/v4/limits-quotas).

   1. 다음에서 [!UICONTROL Metric Tag] 섹션에서 데이터 소스의 각 지표에 추가할 태그의 이름을 입력합니다.

1. 오른쪽 상단에서 **[!UICONTROL Post]**.

   데이터 소스의 이름은 &quot;AccountName > PropertyName > ViewName&quot;이고 자동으로 활성화됩니다. 데이터 소스를 일시 중지하려면 &quot;[데이터 소스에서 피드 일시 중지](data-source-pause.md).&quot;

   이 지표는 광고주의 시간대에서 05:00부터 시작되는 일별 데이터 동기화가 완료된 다음 날에 사용할 수 있습니다. 지표를 사용할 수 있으면에서 볼 수 있습니다. [[!UICONTROL Admin] > [!UICONTROL Conversions]](/help/search-social-commerce/admin/conversion-metrics/conversion-metric-about.md). 각 새 전환 지표의 이름은 &quot;`ga:backEndMetricName_propertyID_viewID`,&quot; 여기서 &quot;backEndMetricName&quot;은 API에서 사용되는 지표 이름입니다. 각 새 전환 지표의 표시 이름은 &quot;입니다.`friendlyMetricName_ga:MetricTag`,&quot; 여기서 &quot;friendlyMetricName&quot;은에 표시되는 지표 이름입니다. [!DNL Google Analytics] 및 &quot;MetricTag&quot;는 [!UICONTROL Metric Tag] 데이터 소스 설정에 정의됩니다.

   캠페인 관리 및 포트폴리오 관리 보기, 보고서 및 최적화 목표에 지표를 직접 추가할 수 있습니다.

>[!MORELIKETHIS]
>
>* [동기화 기본 정보 [!DNL Google Analytics] 전환 지표](data-source-about.md)
>* [구성 사전 요구 사항 [!DNL Google Analytics] 데이터 소스](data-source-prerequisites.md)
>* [편집 [!DNL Google Analytics] 데이터 소스](data-source-edit.md)
>* [데이터 소스 동기화 일시 중지](data-source-pause.md)
>* [재인증 [!DNL Google Analytics] 데이터 소스](data-source-reauthenticate.md)
>* [[!DNL Google Analytics] 데이터 소스 설정](data-source-settings.md)
>* [부록 - 사용 가능 [!DNL Google Analytics] 지표](data-source-ga-metrics.md)
