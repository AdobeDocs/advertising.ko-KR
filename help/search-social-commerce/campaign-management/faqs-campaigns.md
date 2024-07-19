---
title: 캠페인에 대한 FAQ
description: 캠페인 관리 및 캠페인 데이터 보기에 대한 질문에 대한 답변을 살펴볼 수 있습니다.
exl-id: 999e5aba-f556-4b34-bb92-5931d5e0dd72
feature: Search Campaign Management
source-git-commit: 67fe8581832dc0762d62908d01672e53cc95b847
workflow-type: tm+mt
source-wordcount: '1585'
ht-degree: 0%

---

# 캠페인 관리에 대한 FAQ

## 일반 정보

+++한 계정에서 다른 계정으로 캠페인과 구성 요소를 이동할 수 있습니까?

고유 ID가 있는 캠페인 또는 캠페인 구성 요소를 다른 계정 ID가 있는 계정으로 이동하거나 복사하지 마십시오. 이렇게 하면 데이터 오류가 발생합니다.
+++

+++광고 네트워크에서 클릭 데이터가 언제 업데이트됩니까?

검색엔진에서 전날 클릭 데이터를 가져오는 프로세스는 광고주의 시간대인 06:00부터 시작된다.

또한 현재 날짜의 검색 네트워크에서 [!DNL Google Ads]개의 캠페인 수준 성과 지표를 광고주의 시간대에서 08:00 및 16:00에 가져옵니다.
+++

+++어떤 작업으로 인해 키워드와 광고의 내역이 손실됩니까?

>[!NOTE]
>
>(포트폴리오가 있는 광고주) 검색, 소셜 및 Commerce이 데이터를 수집하여 모델을 생성하는 동안 새로운 키워드와 일치 유형 조합의 성능은 불안정할 것으로 예상합니다.

[!UICONTROL Search] > [!UICONTROL Campaigns] 보기, 일괄 시트 게시 프로세스 및 광고 네트워크의 자체 편집기에서 **작업:**

기존 키워드 또는 광고가 삭제되고 다음 경우에 다른 키워드 또는 광고가 만들어집니다.

* ([!DNL Baidu], [!DNL Google Ads] 및 [!DNL Yandex]) 키워드 이름을 편집했습니다.

* ([!DNL Google Ads], [!DNL Microsoft Advertising] 및 [!DNL Yandex]) 키워드의 일치 유형을 변경합니다.

* 광고 그룹 간에 키워드를 이동합니다.

* ([!DNL Google Ads]개의 동적 검색 광고, [!DNL Microsoft Advertising]개의 확장된 텍스트 광고 및 기타 지원되는 광고 네트워크의 모든 광고 유형) 광고 복사본(헤드라인/제목 또는 설명) 또는 광고 이미지를 편집합니다.

* 광고 그룹 간에 광고를 이동합니다.

**제품 인벤토리 피드 게시 프로세스의 이벤트:**

기존 광고 또는 키워드가 삭제되고 다음 경우에 다른 광고 또는 키워드가 만들어집니다.

* 피드 파일에는 광고 변형에 사용된 열에 대한 새 값이 포함되어 있습니다.

* 마지막 전달 이후 광고의 템플릿 설정이 변경되었습니다.

* 새 피드 파일에는 a) 이전 파일에 있었지만 b) 이후 생략된 광고 또는 키워드에 대한 행이 포함되어 있으며, 피드 데이터 설정에 따라 일시 중지되거나 삭제되었습니다.

[피드 데이터 설정](/help/search-social-commerce/campaign-management/inventory-feeds/feed-settings-manage.md#feed-data-settings)에 따라 다음과 같은 경우 기존 광고 또는 키워드가 삭제될 수 있습니다.

* 새 피드 파일에는 기존 광고 또는 키워드에 대한 행이 포함되지 않습니다.

* 게시된 피드 파일의 구성 요소에 대해 예약된 종료 날짜가 발생합니다.

* 항목의 재고 수준이 피드 데이터 설정에 지정된 최소값 미만으로 떨어집니다.
+++

+++([!DNL Google Ads] 캠페인) 내 [!DNL Google] 추적 전환의 표시 이름에 대한 변경 내용이 되돌려졌습니다.

Search, Social 및 Commerce에서 전환 지표의 표시 이름을 변경하면 변경 내용이 [!DNL Google Ads]에 구성된 이름으로 덮어쓰기됩니다. [!DNL Google Ads] 내에서 이름을 변경합니다.
+++

+++(Google Ads 캠페인) 포트폴리오의 캠페인에 공유 예산을 사용할 수 있습니까?

최상의 결과를 얻으려면 [!DNL Google Ads] 캠페인이 &quot;[!UICONTROL Auto adjust campaign budget limits]&quot;(으)로 구성된 최적화된 포트폴리오에 있는 경우 [!DNL Google Ads] 공유 예산에 추가하지 마십시오. [!DNL Google Ads]이(가) 검색, 소셜 및 Commerce에 최적화된 캠페인 예산을 오버라이드하므로 입찰이 비효율적일 수 있습니다.
+++

+++([!DNL Google Ads]개 캠페인) 모바일과 모바일이 아닌 사용자를 다른 랜딩 페이지로 보낼 수 있습니까?

[!DNL Google Ads] [!DNL ValueTrack] 매개 변수 `{ifmobile}` 및 `{ifnotmobile}`을(를) 사용하여 사이트에 적용할 수 있는 두 가지 방법 중 하나로 랜딩 페이지의 도메인 이름을 확인할 수 있습니다.

* `{ifmobile:m}{ifnotmobile:www}`을(를) 사용하여 모바일 지정을 호스트 서버로 포함합니다.

  예를 들어 `http://{ifmobile:m}{ifnotmobile:www}.example.com`은(는) 모바일 사용자는 m.example.com으로, 비모바일 사용자는 www.example.com으로 이동합니다.

* `{ifmobile:mobi}{ifnotmobile:com}`을(를) 사용하여 모바일 지정을 최상위 도메인으로 포함하십시오.

  예를 들어 `http://www.example.{ifmobile:mobi}{ifnotmobile:com}`은(는) 모바일 사용자를 www.example.mobi로, 비모바일 사용자를 www.example.com으로 이동합니다.

두 경우 모두 Search, Social 및 Commerce 추적을 사용하는 기본 URL에는 인코딩되지 않은 `{}` 태그와 기본 URL에 추가된 모든 추가 매개 변수가 포함되어 있습니다.

>[!NOTE]
>
>전체 URL을 ifnotmobile 및 ifmobile 매개 변수의 값으로 사용하지 말고, URL의 변수 부분(예: &quot;m&quot; 대 &quot;www&quot; 또는 &quot;mobi&quot; 대 &quot;com&quot;)만 사용하십시오.

+++

+++( 검색 네트워크에 있는 [!DNL Google Ads]개 캠페인) 오늘 표시되는 데이터는 무엇입니까?

현재 날짜의 검색 네트워크에서 [!DNL Google Ads]개의 캠페인 수준 성과 지표를 광고주의 시간대에서 08:00 및 16:00에 가져옵니다.

[!UICONTROL Search] > [!UICONTROL Campaigns] > [!UICONTROL Campaigns] 보기와 [!UICONTROL Optimization] > [!UICONTROL Portfolios] 보기 모두의 [!UICONTROL Campaigns] 탭에서 [!UICONTROL Today] 또는 현재 날짜가 포함된 사용자 지정 날짜 범위에 대해 보고할 때 데이터에 가장 최근에 동기화된 데이터가 포함됩니다.

>[!NOTE]
>
>클릭, 노출 및 전환에 대한 데이터는 3시간 정도 지연되며 다음 데이터 가져오기가 완료될 때까지 완료되지 않습니다.

+++

+++추적 템플릿과 랜딩 페이지 접미사의 차이점은 무엇입니까?

병렬 추적을 지원하는 광고 네트워크에만 랜딩 페이지 접미사를 사용하십시오. 검색, 소셜 및 Commerce에서 추적 템플릿과 랜딩 페이지 접미사는 모두 광고 네트워크의 클릭 식별자를 포함해야 하지만, 추적 템플릿에는 추가 추적 매개 변수가 포함됩니다.

사용자가 광고를 클릭할 때 추적 템플릿 및 랜딩 페이지 접미사를 로드하는 방법에 대한 자세한 내용은 [병렬 추적 지원](#parallel-tracking)에 대한 다음 FAQ를 참조하십시오.

+++

+++([!DNL Google Ads] 및 [!DNL Microsoft Advertising]) 검색, 소셜 및 Commerce에서 [!DNL Google Ads] 또는 [!DNL Microsoft Advertising]의 광고에 대한 병렬 추적을 지원합니까? {#parallel-tracking}

병렬 추적은 광고에서 최종 URL로 고객을 직접 보냅니다. 이 URL에는 최종 URL 접미사 또는 &quot;랜딩 페이지 접미사&quot;의 추가 매개 변수가 포함될 수 있습니다. 추적 템플릿 URL(클릭 측정에 대한 추가 매개 변수 포함)은 백그라운드에서 별도로 로드됩니다. 그 결과 랜딩 페이지가 더 빨리 로드됩니다.

Search, Social 및 Commerce에서는 광고 네트워크의 클릭 식별자를 사용하여 검색 및 쇼핑 캠페인에 대한 병렬 추적을 지원합니다([!DNL Microsoft Advertising]의 경우 `msclkid`, [!DNL Google Ads]의 경우 `gclid`). 병렬 추적을 지원하는 브라우저에서 하위 광고에 대한 클릭을 추적하기 위해 랜딩 페이지 URL에 추가되는 [계정 수준](/help/search-social-commerce/campaign-management/accounts/ad-network-account-manage.md#account-settings) 또는 [캠페인 수준](/help/search-social-commerce/campaign-management/campaigns/campaign-settings-google.md) [!UICONTROL Landing Page Suffix](광고 네트워크에서 &quot;[!DNL final URL suffix]&quot;이라고 함)을 사용합니다. [다음에 필요한 접미사 형식 [!DNL Google Ads]](/help/search-social-commerce/tracking/formats-click-tracking-google.md) 및 [다음에 필요한 접미사 형식 [!DNL Microsoft Advertising]](/help/search-social-commerce/tracking/formats-click-tracking-microsoft.md)을(를) 참조하십시오.

사용자가 병렬 추적을 지원하지 않는 브라우저에서 광고를 볼 때 광고 네트워크는 대신 순차적 추적을 사용합니다. 고객이 먼저 추적 템플릿 URL로 전송되어 최종 URL로 리디렉션되기 전에 고객을 중간 추적 서버로 리디렉션할 수 있습니다(랜딩 페이지 접미사에 추가 매개 변수를 포함할 수 있음). 광고 네트워크 계정에 대한 모든 추적 템플릿에는 [!UICONTROL Landing Page Suffix]에서 사용하는 것과 동일한 클릭 식별자 매개 변수가 포함되어야 합니다. [다음에 대한 추적 템플릿 형식 [!DNL Google Ads]](/help/search-social-commerce/tracking/formats-click-tracking-google.md)과 [다음에 대한 추적 템플릿 형식 [!DNL Microsoft Advertising]](/help/search-social-commerce/tracking/formats-click-tracking-microsoft.md)을 참조하세요.
+++

+++내 광고에 대한 추적 URL에 &quot;`&EV_HASH={<hash>}`&quot;이(가) 포함되는 이유는 무엇입니까?&quot;

검색, 소셜 및 Commerce 픽셀 리디렉션 및 키워드 및 크리에이티브 수준 추적이 있는 계정에 대해 [제품 인벤토리 피드](/help/search-social-commerce/campaign-management/inventory-feeds/inventory-feeds-about.md)를 사용하여 광고를 업로드할 때 검색, 소셜 및 Commerce은 해시 매개 변수와 값을 광고의 추적 템플릿 또는 대상 URL에 추가하여 인벤토리 피드 기능을 사용하여 광고를 만들었음을 식별합니다.
+++

## 인벤토리 피드

+++(제품 재고 피드) 더 이상 사용되지 않거나 재고 수준이 지정된 최소 미만인 제품에 대한 광고를 일시 중지하거나 삭제해야 합니까?

광고주의 비즈니스 요구 사항에 따라 다릅니다.

광고를 일시 중지하면, 동일한 광고를 다시 제출하거나 재고 수준이 최소값을 초과할 경우 다시 활성화됩니다. 이렇게 하면 광고 내역을 유지할 수 있습니다.

광고를 삭제하고 다시 제출하면 새 광고가 만들어지고 새 광고에 대한 내역 데이터가 축적되어야 합니다. 그러나 삭제된 광고를 다시 제출하지 않을 경우 내역 데이터를 보유하는 것은 중요하지 않습니다.
+++

+++(제품 인벤토리 피드) 광고 템플릿을 삭제한 다음 동일한 새 템플릿을 만드는 경우 일시 중지된 다음 피드 파일에서 누락된 항목이 있습니다(피드 파일 설정이 그렇게 구성되었을 때).

다음 피드 파일에 라인 항목이 없고 이전에 이전 피드 파일을 통해 새 템플릿의 해당 라인 항목을 게시하지 않은 경우 누락된 라인 항목은 &quot;누락&quot;으로 인식되지 않으므로 생성되지 않습니다. 이를 방지하려면 새 템플릿에서 이전 피드 파일을 전파하고 새 파일의 데이터를 전파하고 게시하기 전에 데이터를 게시합니다.
+++

+++(제품 재고 피드) 광고의 품질 점수에 영향을 주지 않고 제품의 가격을 업데이트할 수 있습니까?

[!DNL Google Ads] 캠페인의 경우 예: [!DNL Google Ads] `{Param 1}` 및 `{Param 2}` 변수를 사용하면 광고를 삭제하고 다시 만들지 않고 광고 변형에 숫자 값을 동적으로 삽입할 수 있으므로 품질 점수에 영향을 주지 않습니다.

가격 데이터에 `{Param 1}` 또는 `{Param 2}` 변수를 사용하려면 데이터 파일의 가격 열을 적절한 피드 템플릿의 해당 변수에 매핑한 다음 광고 변형 템플릿에 변수를 포함하십시오.

예를 들어 열이 &quot;Price&quot;라고 하는 경우 광고를 만드는 피드 템플릿을 열고 **[!UICONTROL Param 1]** 옆의 입력 필드를 클릭한 다음 [!UICONTROL Feeds/Available Columns] 목록에서 **[!UICONTROL Price]** 열을 클릭합니다. 그러면 [!UICONTROL Param 1]에 대한 값으로 `[Price]`이(가) 삽입됩니다. 피드 템플릿 하단의 광고 변형 템플릿에 `{param1:default text}`을(를) 삽입합니다. 여기서 &quot;기본 텍스트&quot;는 피드 파일의 매개 변수 열이 광고 행에 대해 비어 있는 경우 사용할 텍스트입니다.

데이터를 제출할 때 [!UICONTROL Param1] 및 [!UICONTROL Param2] 열의 데이터 필드에는 숫자 데이터, 통화 기호 및 통화 코드와 숫자가 아닌 다음 문자를 포함하여 최대 25자가 포함될 수 있습니다. `, . % + - /`
+++

+++인벤토리 피드에서 생성된 내 캠페인에는 많은 고아 트랜잭션이 있습니다.

[피드 데이터 설정](/help/search-social-commerce/campaign-management/inventory-feeds/feed-settings-manage.md#feed-data-settings)이(가) 다양한 상황에서 광고를 삭제하도록 구성된 경우 광고를 클릭한 후 발생하는 지연된 전환으로 인해 [고립 트랜잭션](/help/search-social-commerce/glossary.md#o-p)이 발생할 수 있습니다. 가장 좋은 방법은 광고를 삭제하는 대신 일시 중지하는 것입니다. 오랫동안 광고가 수익을 받지 못한 경우 일괄 시트 또는 광고 관리 보기를 통해 삭제할 수 있습니다.
+++

## 계정 및 캠페인 관련 성능 문제

+++내 캠페인 중 일부는 캠페인 예산보다 더 많이 또는 더 적게 지출하고 있습니다.

* &quot;[!UICONTROL Auto-adjust campaign budget limits]&quot; 옵션으로 구성된 최적화된 포트폴리오에서는 일반적입니다. 이 옵션이 활성화되면 각 캠페인 예산의 최대 *N*&#x200B;배를 사용할 수 있습니다. 여기서 *N*&#x200B;은(는) &quot;[!UICONTROL Multiple]&quot; 설정의 값입니다. 이 옵션을 사용하면 최적화 기능을 통해 필요에 따라 개별 캠페인에 대한 지출을 조정하는 동시에 전체 포트폴리오를 타겟에 맞게 조정할 수 있습니다.
* [!DNL Google Ads] 캠페인이 공유 예산을 사용하는 경우 [!DNL Google Ads]은(는) 전체 공유 예산을 지출하는 데 필요한 만큼 개별 캠페인에 대한 지출을 조정합니다.
+++
