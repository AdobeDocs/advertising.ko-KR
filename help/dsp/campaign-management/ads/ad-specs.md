---
title: 광고 사양
description: 일반 및 게시자별 광고 사양을 참조하십시오.
feature: DSP Ads
exl-id: 133dfc0d-d839-4e06-a819-21e3e630830c
source-git-commit: 10e85f9ec0b7b867828cc9ac154af6f4982c44d2
workflow-type: tm+mt
source-wordcount: '870'
ht-degree: 0%

---

# 지원되는 광고 유형에 대한 사양

## 비디오 광고(프리롤, CTV 및 유니버설 비디오)

### 지원되는 Screens

광고는 기본적으로 데스크탑, 모바일 및 연결된 TV 디바이스에서 제공됩니다. 장치 타깃팅을 사용하여 게재를 조정할 수 있습니다.

### 지원되는 타사 광고 서버

[!DNL DCM], [!DNL Flashtalking], [!DNL Innovid] 및 [!DNL Sizmek]의 태그 시트를 사용할 수 있습니다. 지원되는 공급업체의 전체 목록에 대해서는 &quot;[인증된 광고 서비스 제공 파트너](certified-ad-servers.md)&quot;를 참조하십시오.

### HD 비디오 Assets 요구 사항

**비디오 태그 유형:** VPAID 2.0 JavaScript 또는 VAST(CTV). 모든 VPAID 광고 단위는 IAB(Advertising Bureau)에서 정의한 [VPAID 2.0 사양](https://iabtechlab.com/wp-content/uploads/2016/04/VPAID_2_0_Final_04-10-2012.pdf)을 준수해야 합니다.

**비디오 코덱:** MP4/H.264

**해상도:** 720p의 경우 1280x720, 1080p의 경우 1920x1080

**비트율:** 720p의 경우 1500-2500kbps, 1080p의 경우 2500-3500kbps

**H.264 프로필/수준:** 높은 프로필, 720p용 수준 3.1; 높은 프로필, 1080p용 수준 4.0

**비디오 프레임 속도:** NTSC 국가의 경우 29.970fps(일반적으로 30fps라고 함), PAL 국가의 경우 25fps, 필름 모양 컨텐츠의 경우 23.976fps(일반적으로 24fps라고 함)

**비디오 색상 공간:** 4:2:0 YUV 크로마 서브샘플링

**비디오 인터레이싱:** 프로그레시브 스캔, 즉 비인터레이스입니다. 필드 내 동작(프레임 혼합) 또는 인터레이스가 없습니다.

**Leaders(슬레이트):**&#x200B;은(는) 허용되지 않습니다.

**오디오 코덱:** AAC-LC 또는 HE-AACv1

**오디오 비트 전송률:** AAC-LC의 경우 128-192kbps, HE-AACv1의 경우 64-128kbps

**오디오 채널:** 2채널 스테레오 믹스

**오디오 샘플링 속도:** 소스 재료당 44.1kHz 또는 48kHz

**오디오 수준:** ATSC A/85에 따라 미국에서는 24개의 LKFS(+/- 2.0dB), EBU R128에 따라 유럽에서는 23개의 LUFS(+/- 1.0)

#### 연결된 TV 광고에 대한 추가 게시자 요구 사항

* **A+E 네트워크:** A+E 네트워크의 [광고 사양 보기](/help/dsp/assets/a-e-networks-tve-video-ad-specs.pdf)

* **검색:** 검색의 [광고 사양](/help/dsp/assets/discovery-networks-ad-specs.pdf)을 참조하세요.

* **Disney(포함) Hulu):** Disney의 [광고 사양](https://hulu.disneyadsales.com/ad-products/video-commercial/)을 참조하십시오.

* **HBO 최대:** HBO 최대 [광고 사양](/help/dsp/assets/hbo-max-ad-specs-2022.xlsx)을 참조하십시오.

* **NBCUniversal:**

   * [디지털 비디오](https://together.nbcuni.com/nbcu-creative-guidelines/digital-video/)

   * [실시간 스트리밍](https://together.nbcuni.com/nbcu-creative-guidelines/livestream/)

   * [Peacock](https://together.nbcuni.com/nbcu-creative-guidelines/peacock/)

* **Paramount:** Paramount의 [광고 사양](https://www.paramount.com/digital-ads)을 참조하십시오.

## 디스플레이 광고

### 지원되는 Screens

광고는 기본적으로 데스크탑 및 모바일 디바이스에서 제공됩니다. 장치 타깃팅을 사용하여 게재를 조정할 수 있습니다.

### 지원되는 파일 유형

**이미지:** GIF, JPG/JPEG, PNG

**HTML5:** 이미지 파일 형식: GIF, JPG/JPEG, PNG, SVG

### 이미지 Assets 요구 사항

범용 디스플레이가 지원됩니다.

**권장 광고 크기:** 120x60, 160x600, 180x150, 300x50, 300x1050, 300x250, 300x600, 320x50, 320x480, 480x60, 640x480, 88x31, 728x90, 970x250, 970x90

**지원되는 타사 광고 서버:** [!DNL DCM], [!DNL Flashtalking], [!DNL Innovid] 및 [!DNL Sizmek]의 태그 시트를 사용할 수 있습니다. 지원되는 공급업체의 전체 목록에 대해서는 &quot;[인증된 광고 서비스 제공 파트너](certified-ad-servers.md)&quot;를 참조하십시오.

## 오디오 광고

### 지원되는 Screens

데스크탑, 모바일, 태블릿, 스마트 스피커 및 연결된 TV

### 지원되는 타사 광고 서버

[!DNL DCM], [!DNL Flashtalking], [!DNL Innovid] 및 [!DNL Sizmek]의 태그 시트를 사용할 수 있습니다. 지원되는 공급업체의 전체 목록에 대해서는 &quot;[인증된 광고 서비스 제공 파트너](certified-ad-servers.md)&quot;를 참조하십시오.

### Audio Assets 요구 사항

**파일 형식:** MP3, OGG, AAC

**Leaders(슬레이트):**&#x200B;은(는) 허용되지 않음

**최대 파일 크기:** 2MB

**비트율:** 128

**파일 길이:** 0-60초

#### 추가 게시자 요구 사항

* **[!DNL iHeartRadio]**
   * 길이: 5, 15, 30 또는 60초
   * 파일 유형: MP3
   * 최대 파일 크기: 320kbps
   * 볼륨: 44.1kHz

* **[!DNL Pandora]**
   * 길이: 15 또는 30초
   * 파일 유형: MP4(인앱), MP3(데스크탑)
   * 최대 파일 크기: 2.2MB

* **[!DNL SoundCloud]**
   * 길이: 6, 15 또는 30초
   * 파일 유형: MP3
   * 최대 파일 크기: 5MB

* **[!DNL Spotify]**
   * 길이: 최대 30초
   * 파일 유형: OGG
   * 최대 파일 크기: 500MB
   * 볼륨: RMS가 -14로 표준화됨; dBFS 피크가 -0.2dBFS로 표준화됨

* **[!DNL TargetSpot]**
   * 길이: 15, 30 또는 60초
   * 파일 유형: MP3

* **[!DNL TuneIn]**
   * 길이: 10, 15 또는 30초
   * 파일 유형: MP3, OGG
   * 볼륨: 44.1kHz

### 컴패니언 배너 광고 요구 사항(선택 사항)

**지원되는 크기:** 300x250, 500x500, 640x640, 1024x1024

#### 추가 게시자 요구 사항

* **[!DNL iHeartRadio]:**
   * 파일 유형: JPEG, JPG, PNG, GIF, SWF, HTML
   * 최대 파일 크기: 2.2MB
   * 크기: 300x250

* **[!DNL Pandora]:**
   * 파일 유형: JPEG, GIF
   * 최대 파일 크기: 크기: 100KB
   * 크기: 300x250(모바일 또는 데스크탑) 또는 500x500(데스크탑)

* **[!DNL SoundCloud]:**
   * 파일 유형: 정적 JPG, PNG
   * 최대 파일 크기: 400KB 미만
   * 크기: 1024x1024

* **[!DNL Spotify]:**
   * 파일 유형: 정적 JPG, PNG
   * 최대 파일 크기: 200KB
   * 크기: 300x250

* **[!DNL TuneIn]:**
   * 파일 유형: JPEG, JPG, PNG, GIF, HTML
   * 최대 파일 크기: 2MB
   * 크기: 300x250

## 기본 디스플레이 광고

각 광고에는 스틸 이미지 또는 움직이는 GIF(cinemagraph)가 포함될 수 있습니다.

### 지원되는 Screens

광고는 기본적으로 데스크탑 및 모바일 디바이스에서 제공됩니다. 장치 타깃팅을 사용하여 게재를 조정할 수 있습니다.

### 모든 기본 인피드 형식에 필요한 Assets

#### 이미지 자산

**해상도:** 최소 600x600px, 권장 최소 1200x627px

**파일 형식:** JPEG(이미지 광고 또는 비디오 광고 표지 이미지), GIF(cinemograph)

**파일 크기:** 1MB 미만(이미지에 텍스트가 없어야 함)

#### 광고주 로고

**해상도:** 최소 80x80px, 권장 최소 300x300px

**파일 형식:** JPEG 또는 PNG.

**종횡비:** 1x1 비율

>[!NOTE]
>
>오버레이할 이미지에 따라 밝은 로고 또는 어두운 로고 자산 중에서 선택합니다.

#### 텍스트/복사

**헤드라인:** 최대 200자, 25자 권장

**캡션:** 최대 200자, 100자 권장

**후원:** 최대 200자, 30자 권장

**Call to action(MoPub만 해당):** 최대 15자

>[!NOTE]
>
>최종 레이아웃은 런타임에 게시자가 정의합니다. 광고가 권장 문자 수를 초과하는 경우 일부 인벤토리 공급자가 광고를 전달하지 않거나 게시자 또는 SSP에서 텍스트를 자를 수 있습니다.

#### 랜딩 페이지 URL

클릭 추적기(선택 사항)가 있는 클릭스루 URL.

클릭 추적기 요구 사항:

* 타사 노출 추적 픽셀: 1x1 이미지 URL 형식만 해당

* 가시성 JavaScript 추적기: IAS에 대해서만 지원되며, JS.append 형식의 1x1 이미지만 지원합니다.

* 타사 클릭 추적 픽셀: URL에 포함된 랜딩 페이지로 리디렉션해야 함(HTTP 302 리디렉션)

* 응답이 200개 이상인 데이터 관리 플랫폼(DMP) 클릭 추적기는 지원되지 않습니다.

>[!MORELIKETHIS]
>
>* [광고 관리 정보](ad-about.md)
>* [단일 광고 만들기](ad-create.md)
>* [여러 타사 광고 만들기](ad-create-multiple.md)
>* [광고 편집](ad-edit.md)
