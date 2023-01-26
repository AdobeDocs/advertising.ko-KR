---
title: 광고 사양
description: 일반 및 게시자별 광고 사양을 참조합니다.
feature: DSP Ads
exl-id: 905dfd9b-e7a3-4eb6-988f-b49d4b282dd2
source-git-commit: 1c13874967ec4ad264e5fa6a5e0dfeb6120f53cc
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 0%

---

# 지원되는 광고 유형에 대한 사양

## 비디오 광고(프리롤, CTV 및 범용 비디오)

### 지원되는 화면

광고는 기본적으로 데스크탑, 모바일 및 연결된 TV 장치에서 제공됩니다. 장치 타깃팅은 게재를 조정하는 데 사용할 수 있습니다.

### 지원되는 타사 광고 서버

다음에서 태그 시트를 사용할 수 있습니다. [!DNL DCM], [!DNL Flashtalking], [!DNL Innovid], 및 [!DNL Sizmek]. 지원되는 공급업체의 전체 목록은 &quot;[공인 광고 서비스 제공 파트너](certified-ad-servers.md).&quot;

### HD 비디오 자산에 대한 요구 사항(필수)

**비디오 태그 유형:** VPAID 2.0 JavaScript 또는 VAST(CTV). 모든 VPAID 광고 단위는 [VPAID 2.0 사양](https://iabtechlab.com/wp-content/uploads/2016/04/VPAID_2_0_Final_04-10-2012.pdf) iab(Interactive Advertising Bureau)에서 정의한 것입니다.

**비디오 코덱의 경우:** MP4/H.264

**해결 방법:** 720p용 1280x720, 1080p용 1920x1080

**비트율:** 1080p용 1500-2500kbps, 720p용 2500-3500kbps

**H.264 프로필/수준:** 높은 프로필, 720p용 레벨 3.1 높은 프로필, 1080p용 레벨 4.0

**비디오 프레임 속도:** NTSC 국가의 경우 29.970fps(일반적으로 30fps라고도 함), PAL 국가의 경우 25fps, 영화 모양 컨텐츠의 경우 23.976fps(일반적으로 24fps)입니다

**비디오 색상 공간:** 4:2:0 YUV 색상 서브샘플링

**비디오 인터레이스:** 프로그레시브 스캔, 즉 비인터레이스 필드 내 동작(혼합 프레임) 또는 인터레이스가 없습니다.

**리더(슬레이트):** 허용되지 않음

**오디오 코덱은** AAC-LC 또는 HE-AACv1

**오디오 비트율:** AAC-LC의 경우 128-192kbps, HE-AACv1의 경우 64-128kbps

**오디오 채널:** 2채널 스테레오 믹스

**오디오 샘플 속도:** 소스 재료당 44.1kHz 또는 48kHz

**오디오 수준:** ATSC A/85에 따라 미국에서 24개의 LKFS(+/- 2.0dB) EBU R128에 따라 EU에서 23LUFS(+/- 1.0)

#### 연결된 TV 광고에 대한 추가 게시자 요구 사항

* **A+E 네트워크:** A+E 네트워크 [광고 사양](/help/dsp/assets/a-e-networks-tve-video-ad-specs.pdf)

* **검색:** Discovery를 참조하십시오. [광고 사양](/help/dsp/assets/discovery-networks-ad-specs.pdf).

* **디즈니(incr) 후루):** 디즈니 [광고 사양](https://hulu.disneyadsales.com/ad-products/video-commercial/).

* **HBO 최대:** HBO Max를 참조하십시오. [광고 사양](/help/dsp/assets/hbo-max-ad-specs-2022.xlsx).

* **NBCUniversal:**

   * [디지털 비디오](https://together.nbcuni.com/nbcu-creative-guidelines/digital-video/)

   * [실시간 스트리밍](https://together.nbcuni.com/nbcu-creative-guidelines/livestream/)

   * [피콕](https://together.nbcuni.com/nbcu-creative-guidelines/peacock/)

* **파라마운트:** 파라마운트 [광고 사양](https://www.paramount.com/digital-ads).

## 디스플레이 광고

### 지원되는 화면

광고는 기본적으로 데스크탑 및 모바일 장치에서 제공됩니다. 장치 타깃팅은 게재를 조정하는 데 사용할 수 있습니다.

### 지원되는 파일 형식

**이미지:** GIF, JPG/JPEG, PNG

**HTML5:** 이미지 파일 형식: GIF, JPG/JPEG, PNG, SVG

### 이미지 자산에 대한 요구 사항(필수)

범용 표시가 지원됩니다.

**권장 광고 크기:** 120x60, 160x600, 180x150, 300x50, 300x1050, 300x250, 300x600, 320x50, 320x480, 480, 480x60, 400, 40x60 88x31, 728x90, 970x250, 970x90

**지원되는 타사 광고 서버:** 다음에서 태그 시트를 사용할 수 있습니다. [!DNL DCM], [!DNL Flashtalking], [!DNL Innovid], 및 [!DNL Sizmek]. 지원되는 공급업체의 전체 목록은 &quot;[공인 광고 서비스 제공 파트너](certified-ad-servers.md).&quot;

## 오디오 광고

### 지원되는 화면

데스크탑, 모바일, 태블릿, 스마트 스피커 및 연결된 TV

### 지원되는 타사 광고 서버

다음에서 태그 시트를 사용할 수 있습니다. [!DNL DCM], [!DNL Flashtalking], [!DNL Innovid], 및 [!DNL Sizmek]. 지원되는 공급업체의 전체 목록은 &quot;[공인 광고 서비스 제공 파트너](certified-ad-servers.md).&quot;

### 오디오 자산에 대한 요구 사항(필수)

**파일 형식:** MP3, OGG, AAC

**리더(슬레이트):**  허용되지 않음

**최대 파일 크기:** 2MB

**비트율:** 128년

**파일 길이:** 0-60년대

#### 추가 게시자 요구 사항

* **[!DNL iHeartRadio]**
   * 길이: 5, 15, 30 또는 60초
   * 파일 형식: MP3
   * 최대 파일 크기: 320kbps
   * 볼륨: 44.1킬로헤르츠

* **[!DNL Pandora]**
   * 길이: 15초 또는 30초
   * 파일 형식: MP4(인앱), MP3(데스크탑)
   * 최대 파일 크기: 2.2MB

* **[!DNL SoundCloud]**
   * 길이: 6, 15 또는 30초
   * 파일 형식: MP3
   * 최대 파일 크기: 5MB

* **[!DNL Spotify]**
   * 길이: 최대 30초
   * 파일 형식: OGG
   * 최대 파일 크기: 500MB
   * 볼륨: RMS가 -14로 표준화됨; dBFS 피크가 -0.2dBFS로 표준화됨

* **[!DNL TargetSpot]**
   * 길이: 15, 30 또는 60초
   * 파일 형식: MP3

* **[!DNL TuneIn]**
   * 길이: 10, 15 또는 30초
   * 파일 형식: MP3, OGG
   * 볼륨: 44.1킬로헤르츠

### 컴패니언 배너 광고에 대한 요구 사항(선택 사항)

**지원되는 크기:** 300x250, 500x500, 640x640, 1024x1024

#### 추가 게시자 요구 사항

* **[!DNL iHeartRadio]:**
   * 파일 형식: JPEG, JPG, PNG, GIF, SWF, HTML
   * 최대 파일 크기: 2.2MB
   * Dimension: 300x250

* **[!DNL Pandora]:**
   * 파일 형식: JPEG, GIF
   * 최대 파일 크기: 크기: 100KB
   * Dimension: 300x250(모바일 또는 데스크탑) 또는 500x500(데스크탑)

* **[!DNL SoundCloud]:**
   * 파일 형식: 정적 JPG, PNG
   * 최대 파일 크기: 400KB 미만
   * Dimension: 1024x1024

* **[!DNL Spotify]:**
   * 파일 형식: 정적 JPG, PNG
   * 최대 파일 크기: 200KB
   * Dimension: 300x250

* **[!DNL TuneIn]:**
   * 파일 형식: JPEG, JPG, PNG, GIF, HTML
   * 최대 파일 크기: 2MB
   * Dimension: 300x250
 

## 기본 디스플레이 광고

각 광고에는 스틸 이미지나 움직이는 GIF(촬영 단락)가 포함될 수 있습니다.

### 지원되는 화면

광고는 기본적으로 데스크탑 및 모바일 장치에서 제공됩니다. 장치 타깃팅은 게재를 조정하는 데 사용할 수 있습니다.

### 모든 기본 피드 형식에 필요한 자산

#### 이미지 자산

**해결 방법:** 최소 600x600px; 권장 최소 1200x627px

**파일 형식:** JPEG(이미지 광고 또는 비디오 광고 표지 이미지), GIF(cinemograph)

**파일 크기:** 1MB 미만(이미지에는 텍스트가 없어야 함)

#### 광고주 로고

**해결 방법:** 최소 80x80px; 권장 최소 300x300px

**파일 형식:** JPEG 또는 PNG.

**종횡비:**  1x1 비율

>[!NOTE]
>
>오버레이할 이미지에 따라 밝은 로고 또는 어두운 로고 자산 중에서 선택합니다.

#### 텍스트/복사

**제목:** 최대 200자 25자 권장

**캡션:** 최대 200자 100자 권장

**후원자:** 최대 200자 30자 권장

**클릭유도문안(MoPub만 해당):** 최대 15자

>[!NOTE]
>
>최종 레이아웃은 런타임 시 게시자가 정의합니다. 광고가 권장 문자 수를 초과하는 경우 일부 인벤토리 공급자가 광고를 배달하지 않거나 게시자 또는 SSP에서 텍스트를 자를 수 있습니다.

#### 랜딩 페이지 URL

클릭 추적기 선택 사항이 있는 클릭스루 URL입니다.

클릭 추적기 요구 사항:

* 타사 노출 추적 픽셀: 1x1 이미지 URL 형식만

* JavaScript 추적기 보기 기능: IAS에서만 지원됨; JS.append 형식의 1x1 이미지만

* 타사 클릭 추적 픽셀: URL에 포함된 랜딩 페이지로 리디렉션해야 합니다(HTTP 302 리디렉션)

* DMP(데이터 관리 플랫폼) 클릭 추적기(200개 이상의 응답 포함)가 지원되지 않습니다.

>[!MORELIKETHIS]
>
>* [광고 관리](ad-about.md)
>* [단일 광고 만들기](ad-create.md)
>* [여러 타사 광고 만들기](ad-create-multiple.md)
>* [광고 편집](ad-edit.md)

