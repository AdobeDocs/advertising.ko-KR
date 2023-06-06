---
title: 인벤토리 피드를 사용한 광고 관리 자동화 정보
description: 제품 또는 서비스 인벤토리에 대한 데이터를 기반으로 계정 구조를 자동으로 관리하고 동적 광고를 게재하는 워크플로우에 대해 알아봅니다.
source-git-commit: cd461f73f4a70a5647844a6075ba1c65d64a9b04
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# 재고 피드를 사용한 캠페인 데이터 관리 워크플로우

*[!DNL Google Ads], [!DNL Microsoft® Advertising], [!DNL Yahoo! Japan Ads] (작업만 삭제) 및 [!DNL Yandex] 계정만*

처음에는 적어도 한 개의 피드 파일 또는 계정을 테스트한 다음 프로세스를 완전히 자동화하거나 각 단계에서 계속 제어할 수 있습니다.

1. (선택 사항) 데이터 파일을 저장하기 위한 FTP 디렉터리를 설정하려면 Adobe 계정 팀에 문의하십시오.

   FTP 디렉터리를 사용하는 경우 피드 서비스는 2시간마다 새 파일을 확인합니다.

   그렇지 않으면 [!UICONTROL Advanced (ACM)] 보기.

1. 설정 [피드 데이터 처리를 위한 매개 변수](feed-settings-manage.md#feed-data-settings).

   FTP를 사용하는 경우 처음에 데이터를 광고 네트워크에 자동으로 게시하지 마십시오. 첫 번째 파일의 출력을 확인하고 결과에 만족하면 설정을 변경할 수 있습니다.

1. FTP 디렉토리에 데이터 파일 업로드, [수동으로 데이터 파일 업로드](feed-files-manage.md) 다음에서 [!UICONTROL Advanced (ACM) view], 또는 [Google 또는 Microsoft® 머천트 센터 계정에 대한 액세스 활성화](/help/search-social-commerce/campaign-management/accounts/merchant-account-manage.md).

파일을 수동으로 업로드하려면 데이터 파일을 사용하는 템플릿을 만들 때까지 기다릴 수 있습니다.

1. (선택 사항) 그룹 만들기 [수정자](modifiers-manage.md) 피드 데이터 템플릿의 다양한 데이터 필드에 변수로 사용할 수 있습니다.

1. [하나 이상의 템플릿 만들기](ad-templates/ad-template-manage.md) 데이터 열을 사용하여 특정 광고 네트워크 계정에 대한 캠페인, 광고 그룹, 키워드 및/또는 광고 사본을 만듭니다.

1. [템플릿을 통해 피드 데이터 전파](feed-data-propagate.md)- 템플릿의 열 이름을 파일 또는 계정의 데이터로 대체합니다. 템플릿 옵션에 따라 검색, 소셜 및 상거래는 기본 설정을 사용하여 광고에 대한 새 계정 구조(캠페인, 광고 그룹, 키워드)를 생성하거나 광고를 기존 계정 구조에 매핑합니다.

1. (선택 사항) [출력 미리 보기](propagated-data-view.md) 다음에서 [!UICONTROL Advanced (ACM)] 을(를) 확인하고 선택적으로 의 데이터 변경 사항 요약을 확인합니다. [!UICONTROL Propagations] 탭.

1. [데이터 게시](propagated-data-post.md) 관련 광고 네트워크 계정에 연결합니다.

1. (FTP 또는 머천트 센터 계정을 사용하여 데이터를 업로드하는 경우, 선택 사항) 첫 번째 피드 파일의 출력을 검증한 후, [매개 변수 편집](feed-settings-manage.md#feed-data-settings) 관련 템플릿을 통해 후속 데이터를 자동으로 전파하고 관련 광고 네트워크에 게시할 수 있습니다.

1. (새 데이터 파일이 있는 경우) 필요한 경우 새 파일을 업로드하고, 템플릿을 통해 데이터를 전파하고, 관련 광고 네트워크에 데이터를 게시합니다. 선택적으로 한 단계로 데이터를 전파하고 게시할 수 있습니다.

>[!MORELIKETHIS]
>
>* [인벤토리 피드를 사용한 광고 관리 자동화 정보](inventory-feeds-about.md)
>* [계정 구성 요소는 언제 재고 피드에서 생성되거나 삭제됩니까?](when-are-components-created-deleted.md)

