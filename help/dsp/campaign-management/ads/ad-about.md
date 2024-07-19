---
title: Advertising DSP의 광고 관리 정보
description: 광고 관리에 대해 알아봅니다.
feature: DSP Ads
exl-id: 41dbe28e-a476-4601-a3d8-a9111eae3f6b
source-git-commit: e517dd5f5fa283ff8a2f57728612937148889732
workflow-type: tm+mt
source-wordcount: '733'
ht-degree: 0%

---

# Advertising DSP의 광고 관리 정보

<!-- add "The Ads View (Dashboard?)" section -->

DSP은 다양한 광고 유형에 대한 서드파티 광고 서비스 태그(예: Google, Flashtalking 또는 Sizmek)를 통한 광고 게재와 기본 디스플레이 광고에 대한 직접 에셋 업로드를 지원합니다. 개별적으로 또는 대량으로 타사 태그를 업로드할 수 있습니다. 벌크 업로드는 파트너 태그 시트 또는 벌크 태그 템플릿을 사용합니다.

<!-- The bulk upload feature requires you to either a) upload DoubleClick and Flashtalking tag sheets or b) download a template, input your tags into the template, and then re-upload the template. -->
<!-- need a list of all supported third-party ad servers; see file in future-tbd folder -->

광고가 설정되면 캠페인의 게재 방법을 제어하는 타겟팅 매개 변수(예: 지역, 대상자, 디바이스 및 인벤토리 타겟팅)가 포함된 배치에 각 광고를 첨부합니다. 단일 광고를 하나 또는 여러 배치에 첨부할 수 있습니다.

## 사용 가능한 광고 유형 {#ad-types}

DSP에서 다음 광고 유형을 모두 사용할 수 있습니다. 각 광고 유형에 대한 전체 사양은 [광고 사양](ad-specs.md)을 참조하십시오.

* **오디오 광고(타사 제품만 해당)**: 오디오 광고는 디지털 게시자 사이트의 콘텐츠 간에 재생되며 오디오 파일 또는 컴패니언 배너와 함께 독립 실행형으로 실행할 수 있습니다. 오디오는 브랜드 인지도를 높이고 이동 중인 대상자와 교류하는 데 가장 적합합니다. 오디오의 주요 성능 표시기에는 [!UICONTROL Completion Rate] 및 [!UICONTROL Cost per Completion]이(가) 포함됩니다.

* **디스플레이 광고(타사 전용)**: 디스플레이 광고는 웹 브라우저나 앱에 표시되는 애니메이션 이미지나 정적 이미지입니다. 광고 단위를 클릭하면 사용자가 브랜드 사이트 또는 마이크로사이트로 이동합니다. 디스플레이는 효율적인 CPM을 유도하고, 메시지 연관성을 높이고, 추가 브랜드 또는 제품 접점을 추가하고, 구매 단계를 단축하는 데 가장 적절하게 사용됩니다. 표시할 주요 성능 표시기에는 [!UICONTROL Clicks], [!UICONTROL Cost per Click], [!UICONTROL Conversions] 및 [!UICONTROL Cost per Conversion]이(가) 포함됩니다. DSP은 다양한 디스플레이 배너 광고 크기를 지원합니다.

* **모바일 광고(타사 전용)**: 모바일 광고는 프리롤 비디오(VAST, MRAID) 또는 표준 디스플레이 형식일 수 있습니다. 모바일 프리롤 비디오는 자동 재생 또는 클릭투플레이가 가능하며 여러 화면에서 시청자에게 도달하기 위해 가장 잘 사용됩니다. 모바일 표준 디스플레이는 모바일 웹 브라우저 또는 앱에 표시되는 정적 이미지이며 디지털 비디오 구매를 보완하고 메시지 연결을 유도하며 추가 브랜딩 또는 제품 접점을 추가하는 데 가장 적합합니다. 모바일 광고는 전체 화면 인수 또는 모바일 삽입 광고로도 작동할 수 있습니다. 이는 모바일 대상에 대한 브랜드 인지도를 높이고 전환을 유도하는 데 가장 잘 사용되는 전체 화면, 영향력이 큰 모바일 광고입니다.

* **기본 디스플레이 광고(자사 전용)**: 기본 광고는 표준 디스플레이 형식으로 지원됩니다. 기본 광고에는 헤드라인 및/또는 제목, 설명, 로고 및 이미지가 포함됩니다. 광고가 게시자의 유기 컨텐츠와 혼합되도록 광고 요소가 게시자의 페이지 스타일에 맞게 결합 및 렌더링되어 참여도가 높아집니다. 네이티브는 브랜드 인지도와 시청자 친화적 광고로 대상자 보기 및 참여율을 높이는 데 가장 잘 사용됩니다. 주요 성능 표시기에는 [!UICONTROL Clicks], [!UICONTROL Cost Per Click], [!UICONTROL Conversions] 및 [!UICONTROL Cost Per Conversion]이(가) 포함됩니다.

* **프리롤 광고(타사 전용)**: 프리롤 광고(VAST 및 VPAID)는 프리미엄 비디오 콘텐츠 앞에 표시되고 몰입감 있고 매력적인 뷰어 경험을 제공합니다. 프리롤 비디오는 대화형일 수 있고, 리치 미디어 기능을 포함하고, 오버레이, 롤오버 및 콜 투 액션을 포함할 수 있다. 프리롤 비디오 광고의 주요 성능 표시기에는 [!UICONTROL Video Completion Rate] 및 [!UICONTROL Viewability Rate]이(가) 포함됩니다.

* **연결된 TV 광고(타사 전용)**: 연결된 TV 광고는 프리미엄 TV 비디오 콘텐츠 이전 및 중에 표시됩니다. 연결된 모든 TV 인벤토리는 TV 장치에서 실행되며, 이는 비디오가 시청자가 건너뛸 수 없는 린 백, 전체 화면 환경에서 자동으로 재생됨을 의미합니다. 커넥티드 TV는 TV 광고에 가장 가까운 디지털 비디오 형식입니다. 연결된 TV의 주요 성능 표시기에는 [!UICONTROL Completion Rate]이(가) 포함됩니다.

* **범용 비디오 광고(타사 전용)**: 범용 비디오 광고를 사용하면 단일 비디오 배치를 사용하여 VPAID 및 VAST 인벤토리를 위해 데스크톱, 모바일 및 연결된 TV 환경에서 비디오 인벤토리를 타깃팅할 수 있습니다. 연결된 TV, 프리롤 및 모바일 프리롤 광고의 모든 기능을 결합하고 비디오 콘텐츠 전후에 표시됩니다. 유니버설 비디오의 주요 성능 표시기에는 [!UICONTROL Completion Rate] 및 [!UICONTROL Viewability Rate]이(가) 포함됩니다.

  범용 비디오 광고는 범용 비디오 배치에만 첨부할 수 있습니다.

  범용 비디오 광고에 대한 자세한 내용은 &quot;[범용 비디오에 대한 FAQ](/help/dsp/campaign-management/faq-universal-video.md)&quot;를 참조하십시오.

## DSP 광고 승인

광고를 만들 때 DSP에서 중요한 카테고리에 대해 광고를 검토하고 URL 기능을 클릭한 다음 렌더링을 미리 봅니다.

처음에는 광고의 [!UICONTROL Status] 열에 빨간색 점이 표시됩니다. 검토 프로세스는 일반적으로 24-48시간이 소요됩니다. 그러나 끊어진 광고는 48시간 이상 보류 상태일 수 있으므로 광고가 거부되기 전에 오류를 수정할 시간이 있습니다. 거부된 광고에는 거부 사유가 포함됩니다.

DSP이 광고를 승인하면 광고의 상태 열에 녹색 점이 표시됩니다.

[!UICONTROL Status] 열의 ![승인 표시기](/help/dsp/assets/ad-approval-status.png)

>[!NOTE]
>
>광고는 DSP과 SSP가 모두 크리에이티브를 승인한 경우에만 제공할 수 있습니다. 각 SSP에는 고유한 승인 요구 사항 및 프로세스가 있습니다.

>[!MORELIKETHIS]
>
>* [단일 광고 만들기](ad-create.md)
>* [여러 타사 광고 만들기](ad-create-multiple.md)
>* [광고 사양](ad-specs.md)
