---
title: '[!DNL Google Analytics] 데이터 원본 설정'
description: ' [!DNL Google Analytics] 데이터 원본에 필요한 설정을 참조합니다.'
role: User, Admin
exl-id: 78422c2c-ed58-410e-8996-882759ed5556
feature: Search Data Sources
source-git-commit: e16bc62127a708de8f4deb1eddfa53a14405cbc2
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 0%

---

# [!DNL Google Analytics] 데이터 원본 설정

| 섹션 | 매개 변수 | 설명 |
| ---- | ---- | ---- |
| [!UICONTROL Connect to Google Analytics] | [!UICONTROL Google Analytics Account ID] | 데이터를 가져올 [!DNL Google Analytics] 계정의 ID입니다. 데이터를 가져오는 데 사용된 모든 API 사용이 지정된 계정에 청구됩니다. 계정은 지정된 이메일 주소에 대해 &quot;읽기 및 분석&quot; 권한을 부여해야 합니다.<br><br>ID를 찾으려면 [!DNL Google Analytics]에 로그인하세요. 왼쪽 상단에서 **[!DNL All accounts]**&#x200B;을(를) 클릭하여 계정 목록을 엽니다. 각 계정의 ID는 계정 이름 아래에 있습니다. |
| | [!UICONTROL Google Analytics Login] | 이 데이터 소스의 데이터에 액세스하는 데 사용할 로그인/이메일 주소를 지정하십시오. 로그인은 [!DNL Google] 계정에 등록되어야 하며 [!DNL Google Analytics] 계정에 대한 &quot;읽기 및 분석&quot; 권한이 있어야 합니다.  [!DNL Google Analytics]](https://support.google.com/analytics/answer/9305587)에서 사용자 권한 할당에 대한 [지침을 참조하세요.<br><br><b>참고:</b> 이 로그인 계정의 암호를 변경하면 계정에 대한 모든 열려 있는 연결이 닫힙니다. 데이터 동기화를 다시 시작하려면 이 페이지로 돌아가서 [다시 인증](data-source-reauthenticate.md)하세요. |
| [!UICONTROL Account Details] | [!UICONTROL Google Analytics Account Name] | (읽기 전용, 연결된 계정만 해당) 계정 이름. |
| | [!UICONTROL Google Analytics Property] | [!DNL Google Analytics] 계정에 대한 데이터를 수집할 속성(웹 사이트, 모바일 애플리케이션 또는 장치)입니다.<br><br> 여러 속성에 대한 지표를 통합하려면 각 속성에 대해 별도의 데이터 소스를 설정하십시오. |
| | [!UICONTROL Google Analytics View] | 액세스하려는 데이터 세트가 포함된 보기입니다. 속성에 여러 개의 보기가 있는 경우 모든 데이터가 포함된 가장 높은 수준에서 필터링되지 않은 보기를 가져오는 것이 좋습니다.<br><br>동일한 속성의 여러 보기에 대한 지표를 통합하려면 각 보기에 대해 별도의 데이터 원본을 설정하십시오. 보기에 겹치는 데이터가 없는지 확인합니다. |
| | [!UICONTROL Google Analytics Dimension] | Adobe Advertising &quot;ef_id&quot; 쿼리 문자열 매개 변수의 값으로 채워진 [!DNL Google Analytics] 사용자 지정 차원입니다. 올바른 차원이 표시되지 않으면 [!DNL Google Analytics] 구현 팀에 문의하십시오.<br><br>기본 키로 &quot;ef_id&quot;를 사용하여 [!DNL Google Analytics]에서 Adobe Advertising으로 데이터를 전달합니다. |
| [!UICONTROL Import Metrics] | [!UICONTROL Available Metrics] | 지정된 [!DNL Google Analytics] 속성 및 보기에 대해 사용 가능한 모든 지표가 데이터 원본에 대해 가져오지 않았으며 범주별로 구성되어 있습니다. 목록에는 가져온 친숙한 이름과 백엔드 이름(&quot;ga&quot;로 시작)이 포함됩니다. 각 지표에 대해. [!UICONTROL Refresh] 단추는 [!DNL Google Analytics]에서 새 지표로 목록을 새로 고칩니다.<br><br>사용 가능한 지표를 가져오려면 지표를 [!UICONTROL Selected Metrics] 섹션으로 끌어옵니다.<br><br>Advertising Cloud의 &quot;[사용 가능 [!DNL Google Analytics] 지표](data-source-ga-metrics.md)를 참조하세요.&quot; |
| | 선택한 지표 | 데이터 원본에 대해 가져온 지정된 [!DNL Google Analytics] 속성 및 보기의 모든 지표 및 각 지표에 대한 유효성 검사 상태. 목록에는 각 지표에 대해 가져온 친숙한 이름 및 백 엔드 이름(&quot;`ga.`&quot;(으)로 시작)이 포함됩니다. 각 데이터 소스에는 제거할 수 없는 4개의 기본 트래픽 지표([!UICONTROL Pageviews], [!UICONTROL Sessions], [!UICONTROL Bounces] 및 [!UICONTROL Session Duration])와 데이터가 없는 최대 16개의 유효한 지표나 지표가 추가로 포함될 수 있습니다. 언제든지 지표 목록을 편집할 수 있습니다.<br><br>지표를 가져오려면 [!UICONTROL Available Metrics] 창에서 선택한 다음 여기로 드래그하십시오.<br><br><b>주의:</b> [!DNL Google Analytics]은(는) 단일 데이터 피드에서 최대 10개의 지표를 허용합니다. 검색, 소셜 및 Commerce의 각 데이터 소스에는 총 20개의 지표가 있는 최대 2개의 피드를 포함할 수 있지만, 두 번째 피드를 사용하면 API 호출이 [!DNL Google Analytics]에 두 배가 됩니다. 지표가 많은 경우 최적화를 위해 목표에 사용할 지표만 선택합니다. [다음 [!DNL Google API Console]](https://console.developers.google.com/apis/api/analytics-json.googleapis.com/quotas)에서 이 프로젝트에 대한 할당량을 볼 수 있습니다.  [!DNL Google Analytics]](https://developers.google.com/analytics/devguides/reporting/core/v4/limits-quotas)에 대한 API 요청에 대한 [할당량 및 호출 제한에 대해 자세히 알아보십시오.<br><br><b>메모:</b><br><ul><li>친숙한 이름을 [!UICONTROL Admin] > [!UICONTROL Transactions Properties] 보기에서 지표의 표시 이름으로 가져오고 &quot;<code>_ga:&lt;지표 태그 필드에 구성된 metric_tag>&quot;로 추가합니다.</code>&quot;(예: &quot;Pageviews_ga:UK&quot;). 사용자 지정 목표 및 사용자 지정 지표의 표시 이름을 선택적으로 편집할 수 있지만, 모든 일반 지표의 표시 이름은 지정된 태그가 추가된 [!DNL Google Analytics]의 친숙한 이름으로 매일 덮어쓰기됩니다.</li><li>페이지 보기 수, 세션, 바운스 비율(바운스/세션으로 계산됨) 및 세션 기간은 포트폴리오 입찰 알고리즘에 자동으로 반영됩니다. 포트폴리오 목표에 다른 지표를 수동으로 추가할 수 있습니다.</li><li>데이터 소스에서 지표를 제거하면 Adobe Advertising이 일반 [데이터 보존 정책](/help/search-social-commerce/reports/data-used-for-reports.md)에 따라 기록 데이터를 유지합니다.</li></ul> |
| 지표 태그 | 지표 태그 | Adobe Advertising에서 선택한 각 [!DNL Google Analytics] 지표에 추가할 태그로 앞에 &quot;<code>_ga가 있습니다.</code>&quot; (&quot;Pageviews_ga:&lt;metric_tag>&quot; 등). 태그는 2~5자의 영숫자 문자일 수 있으며 광고주에 대해 고유해야 합니다.<br><br>이 태그는 각 지표의 데이터 원본을 식별하는 데 도움이 됩니다. 각 데이터 원본에는 동일한 지표 이름([!UICONTROL Pageviews], [!UICONTROL Sessions], [!UICONTROL Bounces] 및 [!UICONTROL Session Duration], 잠재적으로 다른 지표 포함) 중 일부가 포함되어 있으므로 이 태그는 여러 데이터 원본을 설정할 때 특히 중요합니다. 다른 지표 태그를 추가하면 지표 이름이 중복되지 않습니다.<br><br>예를 들어 영국 속성과 JP 속성에 대해 별도의 통합을 설정한 경우 지표 태그로 &quot;UK&quot;와 &quot;JP&quot;를 사용할 수 있습니다. 그런 다음 두 속성에 대한 [!UICONTROL Pageviews] 지표가 그에 따라 Adobe Advertising에 &quot;Pageviews_ga:UK&quot; 및 &quot;Pageviews_ga:JP&quot;로 표시됩니다. |

>[!MORELIKETHIS]
>
>* [동기화 정보 [!DNL Google Analytics] 전환 지표](data-source-about.md)
>* [데이터 원본 [!DNL Google Analytics] 구성을 위한 필수 구성 요소](data-source-prerequisites.md)
>* [데이터 소스로  [!DNL Google Analytics] 보기 구성](data-source-configure.md)
>* [데이터 원본 편집 [!DNL Google Analytics] 2}](data-source-edit.md)
>* [데이터 원본 동기화 일시 중지](data-source-pause.md)
>* [데이터 원본 다시 인증 [!DNL Google Analytics] 2}](data-source-reauthenticate.md)
>* [부록 - 사용 가능 [!DNL Google Analytics] 지표](data-source-ga-metrics.md)
