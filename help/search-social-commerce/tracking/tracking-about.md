---
title: 검색, 소셜 및 상거래에 대한 추적 정보
description: 검색, 소셜 및 상거래에 대한 추적 옵션에 대해 알아봅니다.
exl-id: 0a26f67c-8b3b-4fa1-ac24-a8461624cfc5
feature: Search Tracking
source-git-commit: 052574217d7ddafb8895c74094da5997b5ff83db
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 0%

---

# 검색, 소셜 및 상거래에 대한 추적 정보

광고의 성과를 추적하려면 검색, 소셜 및 상거래에 광고에 대한 노출, 클릭, 비용 및 전환(거래) 데이터가 필요합니다. Search, Social 및 Commerce는 이 데이터를 사용하여 광고 포트폴리오를 최적화하는 데 필요한 데이터 예측 모델을 구축합니다.

## 비용, 클릭 및 노출 데이터

검색, 소셜 및 상거래는 노출, 클릭 및 비용 데이터를 [지원되는 광고 네트워크](/help/search-social-commerce/introduction/supported-inventory.md) 매일. 또한 Search, Social 및 Commerce에서는 추적 템플릿 및 대상 URL에 고유한 클릭 추적 코드(추적 서버로 리디렉션 포함)를 추가하여 표시/콘텐츠 노출, 클릭 수 및 비용을 추적하고 나중에 이벤트를 전환에 연결할 수 있습니다.

검색, Social 및 Commerce가 데이터를 동기화하지 않는 광고 네트워크에서 캠페인을 추적하려면 노출, 클릭 및 비용 데이터가 포함된 일별 피드 파일을 전송하여 해당 캠페인에 대한 데이터를 제공해야 합니다.

### 클릭 추적 태그

검색, 소셜 및 상거래 구현 팀은 동기화된 광고 캠페인에 광고, 키워드, 배치, 제품 그룹 및 사이트링크 확장에 대한 추적 템플릿과 대상 URL을 업데이트하여 고유한 추적 ID 문자열 및 Adobe Advertising 리디렉션을 포함하도록 클릭 추적을 설정합니다. 또한 의 랜드 페이지 접미사(최종 URL 접미사)에도 추적을 추가합니다. [!DNL Google Ads] 및 [!DNL Microsoft Advertising] 계정 및 캠페인.

추적 매개 변수를 사용하면 Adobe Advertising이 개별 키워드 수준(검색 캠페인) 또는 광고 변형 수준(콘텐츠 또는 사이트 타겟팅으로 캠페인 검색, 캠페인 표시 및 소셜 캠페인)에서 클릭을 추적할 수 있습니다. 사용자가 디스플레이/컨텐츠 광고를 보거나 광고 중 하나를 클릭할 때마다, 광고 네트워크는 키워드 또는 광고와 연결된 클릭 추적 태그를 사용하여 Adobe Advertising 픽셀 서버로 이벤트를 전송합니다. 클릭 수:

* 병렬 추적을 지원하는 브라우저의 Google Ads 및 Microsoft Advertising 광고의 경우, 광고 네트워크는 먼저 웹 사이트로 클릭을 보낸 다음 Adobe Advertising 픽셀 서버로 전송합니다. 픽셀 서버는 쿠키가 아직 존재하지 않는 경우 사용자의 컴퓨터에 배치합니다.

* 다른 모든 경우에는 광고 네트워크가 클릭을 Adobe Advertising 픽셀 서버로 직접 전송합니다. 픽셀 서버는 사용자의 컴퓨터에 쿠키를 배치한 다음(아직 없는 경우) 사용자를 웹 사이트의 관련 URL로 리디렉션합니다. 최종 사용자의 전체 경험은 리디렉션이 없는 경우와 동일합니다.

쿠키가에 설정됩니다. [!DNL Adobe] 도메인(`everesttech.net`)를 자사 쿠키로 사용할 수 있습니다. 리디렉션 후 사용자는 광고주의 도메인에 있고 쿠키는 타사 쿠키로 처리됩니다. Adobe Advertising 쿠키에 대한 자세한 내용은 &quot;[Adobe Advertising 쿠키](https://experienceleague.adobe.com/docs/core-services/interface/ec-cookies/cookies-advertising-cloud.html).&quot;

## 전환 데이터

고객이 광고를 클릭하거나 디스플레이 또는 소셜 광고를 볼 때, 검색, 소셜 및 상거래는 각각의 최종 전환을 원래 클릭 또는 디스플레이/소셜 노출에 다시 매핑해야 합니다.

광고주는 모든 클릭과 디스플레이/소셜 노출에 대한 전환 데이터를 제공하는 역할을 합니다. 전환 데이터에는 입찰 최적화에 사용할 수 있는 웹 사이트에서 발생하는 모든 유형의 이벤트에 대한 정보가 포함될 수 있습니다. 광고주의 전환 페이지(예: 고객이 트랜잭션을 완료한 후 표시되는 &quot;성공&quot; 페이지)에서 전환 추적 코드를 구현하거나 다른 방법으로 캡처된 전환 데이터와 함께 일별 피드 파일을 전송하여 전환 데이터를 제공할 수 있습니다.

### 전환 추적 태그

다음을 사용할 수 있습니다. [다양한 공급업체의 변환 태그](/help/search-social-commerce/tracking/conversion-tracking-about.md).

Adobe Advertising 전환 태그를 사용하는 경우 사용자가 성공적인 트랜잭션을 완료하고 &quot;성공&quot; 페이지에 도달하면, Adobe Advertising 픽셀 서버는 클릭 리디렉션 시 설정된 사용자의 컴퓨터에 쿠키가 있는지 확인합니다. 쿠키를 찾으면 ef_transid 매개 변수를 사용하여 트랜잭션 이벤트에 대한 정보가 전달되고, 트랜잭션이 전환으로 인식되며 이전 광고 클릭 또는 디스플레이 노출에 따라 크레딧됩니다.

사용자가 두 개 이상의 광고를 클릭한 경우 별도로 지정하지 않는 한 Adobe Advertising은 트랜잭션을 최종 광고 클릭 또는 (디스플레이 또는 비디오 캠페인의 경우) 최종 광고 노출로 크레딧합니다. 사용자 [전환 확인 기간 클릭](/help/search-social-commerce/glossary.md#c-d) 및 [노출 전환 확인 기간](/help/search-social-commerce/glossary.md#i-j) 전환으로 이벤트가 귀속될 수 있는 유료 클릭 또는 디스플레이/비디오 노출(각각) 발생 후 일 수를 결정합니다.

Adobe Advertising 구현 팀은 광고주와 함께 광고주가 구현해야 하는 전환 태그의 형식을 결정하고, 각 전환 태그를 삽입해야 하는 웹 페이지를 식별한 다음, 구현할 전환 태그를 제공합니다.
