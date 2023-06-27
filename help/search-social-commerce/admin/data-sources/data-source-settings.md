---
title: '''[!DNL Google Analytics] 데이터 소스 설정'
description: 에 필요한 설정 참조 [!DNL Google Analytics] 데이터 소스.
role: User, Admin
exl-id: 531351b4-07f1-43ef-a3d2-892a49ffb5ca
source-git-commit: ec7d7f5531c038eb772339a36d13208fc97d2728
workflow-type: tm+mt
source-wordcount: '820'
ht-degree: 0%

---

# [!DNL Google Analytics] 데이터 소스 설정

| 섹션 | 매개 변수 | 설명 |
| ---- | ---- | ---- |
| [!UICONTROL Connect to Google Analytics] | [!UICONTROL Google Analytics Account ID] | 의 ID [!DNL Google Analytics] 데이터를 가져올 계정입니다. 데이터를 가져오는 데 사용된 모든 API 사용이 지정된 계정에 청구됩니다. 계정은 지정된 이메일 주소에 대해 &quot;읽기 및 분석&quot; 권한을 부여해야 합니다.<br><br>ID를 찾으려면 다음으로 로그인합니다. [!DNL Google Analytics]. 왼쪽 상단에서 **[!DNL All accounts]** 계정 목록을 엽니다. 각 계정의 ID는 계정 이름 아래에 있습니다. |
| | [!UICONTROL Google Analytics Login] | 이 데이터 소스의 데이터에 액세스하는 데 사용할 로그인/이메일 주소를 지정하십시오. 로그인을 다음에 등록해야 합니다. [!DNL Google] 및 을(를) 위한 &quot;읽기 및 분석&quot; 권한이 있어야 합니다. [!DNL Google Analytics] 계정입니다. 다음을 참조하십시오. [에서 사용자 권한을 할당하는 지침 [!DNL Google Analytics]](https://support.google.com/analytics/answer/9305587).<br><br><b>참고:</b> 이 로그인 계정의 암호를 변경하면 계정에 대한 모든 열려 있는 연결이 닫힙니다. 데이터 동기화를 재개하려면 이 페이지로 돌아가서 [재인증](data-source-reauthenticate.md). |
| [!UICONTROL Account Details] | [!UICONTROL Google Analytics Account Name] | (읽기 전용, 연결된 계정만 해당) 계정 이름. |
| | [!UICONTROL Google Analytics Property] | 다음에 대한 데이터를 수집할 속성(웹 사이트, 모바일 애플리케이션 또는 장치) [!DNL Google Analytics] 계정입니다.<br><br> 여러 속성에 대한 지표를 통합하려면 각 속성에 대해 별도의 데이터 소스를 설정합니다. |
| | [!UICONTROL Google Analytics View] | 액세스하려는 데이터 세트가 포함된 보기입니다. 속성에 여러 개의 보기가 있는 경우 모든 데이터가 포함된 가장 높은 수준에서 필터링되지 않은 보기를 가져오는 것이 좋습니다.<br><br>동일한 속성에 대해 여러 보기에 대한 지표를 통합하려면 각 보기에 대해 별도의 데이터 소스를 설정합니다. 보기에 겹치는 데이터가 없는지 확인합니다. |
| | [!UICONTROL Google Analytics Dimension] | 다음 [!DNL Google Analytics] Adobe 광고 &quot;ef_id&quot; 쿼리 문자열 매개 변수의 값으로 채워진 사용자 지정 차원입니다. 올바른 차원이 목록에 없으면 다음 주소로 문의하십시오. [!DNL Google Analytics] 구현 팀.<br><br>ef_id는 데이터를 전달할 기본 키로 사용됩니다. [!DNL Google Analytics] Adobe Advertising. |
| [!UICONTROL Import Metrics] | [!UICONTROL Available Metrics] | 지정된 의 사용 가능한 모든 지표 [!DNL Google Analytics] 데이터 원본에 대해 가져오지 않은 속성 및 보기를 범주별로 정리합니다. 목록에는 가져온 친숙한 이름과 백엔드 이름(&quot;ga&quot;로 시작)이 포함됩니다. 각 지표에 대해. 다음 [!UICONTROL Refresh] 버튼은에서 새 지표를 사용하여 목록을 새로 고칩니다. [!DNL Google Analytics].<br><br>사용 가능한 지표를 가져오려면 지표를 [!UICONTROL Selected Metrics] 섹션.<br><br>를 참조하십시오.[사용 가능 [!DNL Google Analytics] Advertising Cloud의 지표](data-source-ga-metrics.md).&quot; |
| | 선택한 지표 | 지정된 의 모든 지표 [!DNL Google Analytics] 데이터 소스에 대해 가져온 속성 및 보기와 각 지표에 대한 유효성 검사 상태. 목록에는 가져온 친숙한 이름과 백엔드 이름(&quot;로 시작)이 포함됩니다.`ga.`각 지표에 대해 &quot;)를 입력합니다. 각 데이터 소스에는 제거할 수 없는 4개의 기본 트래픽 지표가 포함될 수 있습니다([!UICONTROL Pageviews], [!UICONTROL Sessions], [!UICONTROL Bounces], 및 [!UICONTROL Session Duration]) 및 데이터가 없는 최대 16개의 추가 유효한 지표 또는 지표입니다. 언제든지 지표 목록을 편집할 수 있습니다.<br><br>지표를 가져오려면 [!UICONTROL Available Metrics] 창에서 여기로 드래그합니다.<br><br><b>주의:</b> [!DNL Google Analytics] 단일 데이터 피드에서 최대 10개의 지표를 허용합니다. 검색, 소셜 및 상거래에 있는 각 데이터 소스에는 총 20개의 지표가 있는 최대 2개의 피드를 포함할 수 있지만, 두 번째 피드를 사용하면 API 호출이 두 배가 됩니다. [!DNL Google Analytics]. 지표가 많은 경우 최적화를 위해 목표에 사용할 지표만 선택합니다. 다음에서 이 프로젝트에 대한 할당량을 볼 수 있습니다. [다음 [!DNL Google API Console]](https://console.developers.google.com/apis/api/analytics-json.googleapis.com/quotas). 자세한 내용 [에 대한 API 요청에 대한 할당량 및 호출 제한 [!DNL Google Analytics]](https://developers.google.com/analytics/devguides/reporting/core/v4/limits-quotas).<br><br><b>참고:</b><br><ul><li>친숙한 이름을 의 지표 표시 이름으로 가져옵니다. [!UICONTROL Admin] > [!UICONTROL Transactions Properties] 보기 및 가 추가됨<code>_ga:&lt;metric_tag configured=&quot;&quot; in=&quot;&quot; the=&quot;&quot; metric=&quot;&quot; tag=&quot;&quot; field=&quot;&quot;></code>&quot;(예: &quot;Pageviews_ga:UK&quot;). 사용자 정의 목표 및 사용자 정의 지표의 표시 이름을 선택적으로 편집할 수 있지만, 모든 일반 지표의 표시 이름은에서 친숙한 이름으로 매일 덮어씁니다 [!DNL Google Analytics]: 지정된 태그가 추가됩니다.</li><li>페이지 보기 수, 세션, 바운스 비율(바운스/세션으로 계산됨) 및 세션 기간은 포트폴리오 입찰 알고리즘에 자동으로 반영됩니다. 포트폴리오 목표에 다른 지표를 수동으로 추가할 수 있습니다.</li><li>데이터 소스에서 지표를 제거하면 Adobe 광고가 평소에 따라 내역 데이터를 유지합니다 [데이터 보존 정책](/help/search-social-commerce/reports/data-used-for-reports.md).</li></ul> |
| 지표 태그 | 지표 태그 | 선택한 각 항목에 추가할 태그 [!DNL Google Analytics] Adobe Advertising의 지표, 앞에 &quot;<code>_ga:</code>&quot; ( 예: &quot;Pageviews_ga:&lt;metric_tag>&quot;). 태그는 2~5자의 영숫자 문자일 수 있으며 광고주에 대해 고유해야 합니다.<br><br>이 태그는 각 지표에 대한 데이터 소스를 식별하는 데 도움이 됩니다. 이 태그는 각 데이터 소스에 동일한 지표 이름(포함)의 일부가 포함되어 있으므로 여러 데이터 소스를 설정할 때 특히 중요합니다 [!UICONTROL Pageviews], [!UICONTROL Sessions], [!UICONTROL Bounces], 및 [!UICONTROL Session Duration], 및 잠재적으로 다른 지표)를 참조하십시오. 다른 지표 태그를 추가하면 지표 이름이 중복되지 않습니다.<br><br>예를 들어 UK 속성과 JP 속성에 대해 별도의 통합을 설정하는 경우 &quot;UK&quot; 및 &quot;JP&quot;를 지표 태그로 사용할 수 있습니다. 다음 [!UICONTROL Pageviews] 그런 다음 두 속성에 대한 지표가 그에 따라 Adobe Advertising에 &quot;Pageviews_ga:UK&quot; 및 &quot;Pageviews_ga:JP&quot;로 표시됩니다. |

>[!MORELIKETHIS]
>
>* [동기화 기본 정보 [!DNL Google Analytics] 전환 지표](data-source-about.md)
>* [구성 사전 요구 사항 [!DNL Google Analytics] 데이터 소스](data-source-prerequisites.md)
>* [구성 [!DNL Google Analytics] 데이터 소스로 보기](data-source-configure.md)
>* [편집 [!DNL Google Analytics] 데이터 소스](data-source-edit.md)
>* [데이터 소스 동기화 일시 중지](data-source-pause.md)
>* [재인증 [!DNL Google Analytics] 데이터 소스](data-source-reauthenticate.md)
>* [부록 - 사용 가능 [!DNL Google Analytics] 지표](data-source-ga-metrics.md)
