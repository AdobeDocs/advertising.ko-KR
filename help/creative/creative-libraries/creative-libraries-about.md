---
title: 크리에이티브 라이브러리 정보
description: 광고 경험을 위한 크리에이티브 관리에 대해 알아봅니다.
feature: Creative Libraries, Creative Standard Creatives, Creative Dynamic Creatives
exl-id: 77dc6528-a455-4406-98b6-15e7ce529370
source-git-commit: e79becc860143b749ec96134e7b224649686c672
workflow-type: tm+mt
source-wordcount: '1410'
ht-degree: 0%

---

# 크리에이티브 라이브러리 정보

*닫힌 Beta 기능*

크리에이티브 라이브러리를 사용하면 광고 경험에서 사용할 크리에이티브를 관리할 수 있습니다. 한 경험에 한 단위로 추가할 수 있는 크리에이티브 그룹인 크리에이티브 세트와 *크리에이티브 번들*&#x200B;이 포함된 여러 라이브러리를 만들 수 있습니다.

라이브러리는 다음을 포함할 수 있습니다.

* **개별 크리에이티브:** 사용자 타겟이 정의되지 않은 광고 경험 내에 개별 크리에이티브를 직접 포함할 수 있습니다. 또한 크리에이티브를 사용하여 번들을 만들 수도 있습니다. 이 번들은 타깃팅된 [광고 경험](/help/creative/experiences/experience-about.md)에 포함할 수 있습니다.

   * **표준 크리에이티브:** [다양한 형식](#creative-creative-formats)의 크리에이티브를 업로드하고 관리할 수 있습니다. 각 크리에이티브에 대해 크리에이티브를 연결하는 각 광고의 기본 언어와 사용자가 크리에이티브가 포함된 광고를 클릭할 때 열리는 기본 랜딩 페이지를 지정합니다. [!DNL Creative] 차원을 사용할 것을 포함할 때 [!UICONTROL Custom Creative Report] 내의 다양한 보기에서 필터로 사용하고 [!UICONTROL Creative Label]의 열 값으로 사용할 레이블을 선택적으로 지정할 수 있습니다.

   * **동적 크리에이티브:**(기존 Adobe Advertising DCO 고객만 해당) 관리자 사용자는 광고 템플릿의 동적 변수를 피드 파일의 값에 매핑하여 동적으로 생성된 크리에이티브를 만들 수 있습니다. 모든 사용자는 기존 동적 광고를 미리 보고, 복제하고, 삭제할 수 있습니다.

* **크리에이티브 번들:** 정의된 사용자 대상이 있는 여러 경험에서 사용할 크리에이티브를 번들로 그룹화합니다. 표준 디스플레이 광고로 구성된 *표준 디스플레이 번들*, 표준 비디오 광고로 구성된 *표준 비디오 번들*, 동적으로 생성된 디스플레이 광고로 구성된 *동적 디스플레이 번들*&#x200B;을 만들 수 있습니다.

## 지원되는 Creative 형식 {#creative-creative-formats}

### 표준 광고 형식

[지원되는 크리에이티브 크기](creative-sizes.md)에서 다음 크리에이티브 유형을 추가하고 관리할 수 있습니다.

>[!IMPORTANT]
>
>* 표준 디스플레이 광고 경험을 위해 HTML5, 유연한 HTML5 또는 서드파티 크리에이티브를 사용하려는 경우에도 사용하는 각 크리에이티브 크기에 대해 이미지 크리에이티브를 추가해야 합니다.
>* 각 표준 디스플레이 경험에는 경험에 지정된 각 크리에이티브 크기에 대한 기본 이미지 크리에이티브가 필요합니다. 기본 이미지 크리에이티브는 브라우저가 JavaScript을 사용할 수 없거나 광고 서버가 지연 때문에 광고를 개인화할 수 없는 경우에 사용됩니다.
>* 각 표준 비디오 경험에는 경험에 지정된 각 제작 기간 동안 기본 비디오 크리에이티브가 필요합니다.<!-- when is it used? -->

#### 유연한 HTML5

유연한 HTML5 크리에이티브는 모든 이미지 및 기타 특성을 표준 HTML 태그로 사용하는 HTML5 크리에이티브 기능으로, 크리에이티브 라이브러리 또는 개별 경험(원본 크리에이티브의 변형을 만드는)에서 [!DNL Creative] 내에서 직접 편집할 수 있습니다. DSP에서 유연한 HTML5 크리에이티브는 단일 특정 광고 크기(픽셀 단위)에 해당합니다. 유연한 HTML5 크리에이티브에 지정된 속성의 기본값을 선택적으로 변경할 수 있습니다. 나중에 특정 경험 내의 속성에 대해 사용자 지정 값을 지정할 수 있습니다. 이렇게 하면 상위 크리에이티브의 변형이 만들어집니다.

유연한 HTML5 크리에이티브를 ZIP 파일로 업로드하거나 계정에 사용할 수 있는 템플릿 중 하나를 시작점으로 사용할 수 있습니다. [유연한 HTML5 광고 사양](html5-creative-specification.md)을 참조하세요.

#### HTML5 광고

모든 속성과 이미지가 지정된 단순 또는 정적 HTML5 크리에이티브를 ZIP 파일로 업로드할 수 있습니다. 속성을 편집하거나 이미지를 추가할 수 없습니다. 대신 새 ZIP 파일을 업로드하여 새 크리에이티브를 추가하십시오. [단순 및 정적 HTML5 광고 사양](html5-creative-specification.md)을 참조하세요.

#### 이미지 크리에이티브

GIF, JPEG, JPG 또는 PNG 형식의 이미지 크리에이티브를 포함할 수 있습니다. Adobe Experience Manager 계정에서 승인된 이미지를 업로드하거나 장치 또는 네트워크에서 이미지를 업로드할 수 있습니다.

각 표준 디스플레이 광고 경험에는 경험에 지정된 각 크리에이티브 크기에 대한 기본 이미지 크리에이티브가 필요합니다.

#### 서드파티 크리에이티브

타사 광고 서버에서 호스팅하는 크리에이티브에 대한 JavaScript 추적 태그를 입력합니다. 스크립트는 광고 서버마다 다릅니다. 예를 들면 다음과 같습니다.

```
<SCRIPT language='JavaScript1.1' SRC="https://ad.doubleclick.net/ddm/adj/A123456.12345GDN.COM/B1234567.123456789;sz=300x250;ord=[timestamp];dc_lat=;dc_rdid=;tag_for_child_directed_treatment=?"></SCRIPT> <NOSCRIPT> <A HREF="https://ad.doubleclick.net/ddm/jump/A123456.12345GDN.COM/B1234567.123456789;sz=300x250;ord=[timestamp]?"><IMG SRC="https://ad.doubleclick.net/ddm/ad/A123456.12345GDN.COM/B1234567.123456789;sz=300x250;ord=[timestamp];dc_lat=;dc_rdid=;tag_for_child_directed_treatment=?"BORDER=0 WIDTH=300 HEIGHT=250 ALT="Advertisement"></A></NOSCRIPT>
```

#### 비디오 크리에이티브 {#creative-video-specs}

장치나 네트워크에서 웹, 모바일 또는 연결된 TV에 대한 자사 비디오 크리에이티브를 업로드할 수 있습니다. 각 표준 비디오 광고 경험은 경험에 지정된 각 크리에이티브 기간에 대해 기본 비디오 크리에이티브를 필요로 합니다. 모든 비디오 크리에이티브는 DSP as VAST 2.0 태그로 자동으로 코드 변환되므로 미리 볼 수 있습니다. [!UICONTROL Tag Manager]에서 비디오 광고 경험 태그에 선택적으로 [DSP 전용 코드 변환](/help/creative/experiences/experience-tag-video-transcoding.md)을 적용할 수 있습니다.

다음 비디오 크리에이티브 요구 사항을 참조하십시오. **참고:** 비디오 경험을 Advertising DSP에 업로드하려면 DSP의 [HD 비디오 Assets 요구 사항](https://experienceleague.adobe.com/en/docs/advertising/dsp/campaign-management/ads/ad-specs#requirements-for-high-definition-video-assets)도 참조하세요. 이는 더 제한될 수 있습니다.

**파일 형식:** .mov, .mp4, .webm

**파일 크기:** 최대 512MB

**비디오 종횡비:** 16:9, 4:3

**비디오 해상도:** 360p의 경우 640x360, 720p의 경우 1280x720, 1080p의 경우 1920x1080

**비디오 길이:** 최대 90초

**비트율:** 360p의 경우 600-1200kbps, 720p의 경우 1500-2500kbps, 1080p의 경우 3000-5000kbps 이상

**비디오 프레임 속도:** 23.98FPS. 지역 또는 게시자 요구 사항에 따라 추가 프레임 속도가 허용될 수 있습니다

**비디오 코덱:** H.264(업계 표준), AV1, H.265

**오디오 형식:** ACC(업계 표준/MP4), Opus(WebM/AV1)

**오디오 비트 전송률:** 16-512kbps

**오디오 샘플링 속도:** 44100-48000Hz

**오디오 속도:** 44.1kHz 또는 48kHz

**오디오 기타:** 업로드한 파일은 비인터레이스이고 혼합되어 있으며 오디오 트랙을 포함해야 합니다. 사운드가 없을 수 있지만 오디오 트랙이 비디오 파일에 포함되어야 합니다.

### 다이내믹 광고 형식

관리자 사용자는 광고 템플릿의 동적 변수를 피드 파일의 값에 매핑하여 정적 HTML5 및 동적 HTML5 형식으로 동적으로 크리에이티브를 생성할 수 있습니다. 동적 크리에이티브에는 기존 Adobe Advertising DCO(Dynamic Creative Optimization) 경험의 크리에이티브가 포함될 수 있습니다.

## [!UICONTROL Creative Libraries] 보기

각 보기 사용자 지정에 대한 자세한 내용은 &quot;[데이터 보기 사용자 지정](/help/creative/introduction/customize-data-views.md)&quot;을 참조하십시오.

### [!UICONTROL Creative Libraries] 기본 보기

[!UICONTROL Creative Libraries] 기본 보기에는 모든 크리에이티브 라이브러리가 표시됩니다. 각 라이브러리에 대한 데이터에는 라이브러리의 번들이 할당된 경험 수, 번들 수, 크리에이티브 수, 크리에이티브 크기 수, 기본 언어 대상 수, 생성 날짜 및 라이브러리의 모든 요소에 대한 마지막 수정 날짜가 포함됩니다. 테이블 모드에는 광고주에 대한 열도 포함됩니다.

카드 모드에서는 &lt; 및 > 버튼을 사용하여 여러 크리에이티브가 있는 라이브러리의 이미지를 스크롤할 수 있습니다.

#### 사용 가능한 작업

* [새 라이브러리 만들기](/help/creative/creative-libraries/creative-library-manage.md#create-a-creative-library)

* 각 Creative Library의 경우:

   * [라이브러리 이름 편집](/help/creative/creative-libraries/creative-library-manage.md#edit-the-name-of-a-creative-library)

   * [라이브러리를 열어 라이브러리에 할당된 크리에이티브 및 번들을 봅니다](/help/creative/creative-libraries/creative-library-manage.md#open-a-creative-library)

   * [라이브러리 삭제](/help/creative/creative-libraries/creative-library-manage.md#delete-creative-libraries)

### [!UICONTROL Creative Libraries] > [!UICONTROL Creatives] 보기

#### [!UICONTROL Standard Ads]

[!UICONTROL Standard Ads] 탭에는 사용자가 만든 모든 표준 광고 정보가 표시됩니다. 각 창작물별 자료는 창작규모, 창작유형, 창작시기 등이 포함된다. 테이블 모드에는 기본 언어 및 기본 랜딩 페이지에 대한 열도 포함됩니다.

##### 사용 가능한 작업

* [라이브러리에 표준 크리에이티브 추가](creative-add-standard.md)

* [표준 문안 편집](creative-edit-standard.md)

* [표준 크리에이티브 미리 보기](creative-preview.md)

* [표준 디스플레이 번들에 표준 크리에이티브를 추가하고 표준 디스플레이 번들에서 표준 크리에이티브를 제거합니다.](creative-attach-detach-bundles.md)

* [표준 비디오 번들에 비디오 크리에이티브를 추가하고 표준 비디오 번들에서 비디오 크리에이티브를 제거합니다.](creative-attach-detach-bundles.md)

* [중복 표준 크리에이티브](creative-duplicate.md)

* [표준 광고 다운로드](creative-download.md)

* [표준 광고 삭제](creative-delete.md)

#### [!UICONTROL Dynamic Ads]

[!UICONTROL Dynamic Ads] 탭에는 Creative 카탈로그에 대해 동적으로 만들어진 모든 동적 크리에이티브가 표시됩니다. 단, [ 탭에서 ](creative-delete.md)수동으로 삭제[!UICONTROL Dynamic Ads]한 동적 크리에이티브는 예외입니다. 카탈로그가 마지막으로 처리된 이후의 모든 동적 크리에이티브를 [수동으로 복제](creative-duplicate.md)하면 해당 카탈로그에 대한 크리에이티브 목록에도 중복 크리에이티브가 포함됩니다.

각 창작물별 데이터에는 창작유형, 창작규모, 창작물이 속한 카탈로그 개수, 창작날짜 등이 포함된다. 테이블 모드에는 크리에이티브가 생성된 템플릿 및 오퍼 수에 대한 열도 포함됩니다.

>[!NOTE]
>
>카탈로그가 처리될 때마다 해당 카탈로그의 기존 동적 크리에이티브에 대한 데이터가 새로 고쳐집니다.

##### 사용 가능한 작업

동적 크리에이티브를 만들고 편집하는 기능은 현재 Adobe 계정 팀에서만 사용할 수 있습니다. 그러나 모든 사용자는 다음과 같은 작업을 수행할 수 있습니다.

* [동적 크리에이티브 미리 보기](creative-preview.md)

* [동적 디스플레이 번들에 동적 크리에이티브를 추가하고 동적 디스플레이 번들에서 동적 크리에이티브를 제거합니다.](creative-attach-detach-bundles.md)

* [동적 크리에이티브 복제](creative-duplicate.md)

* [동적 크리에이티브 삭제](creative-delete.md)

<!-- Later:  Dynamic creatives are generated automatically when you save a catalog, but can regenerate the catalog using the contents of an updated asset file [using the Run Now option]. -->

### [!UICONTROL Creative Libraries] > [!UICONTROL Bundles] 보기

[!UICONTROL Bundles] 보기에는 표준 및 동적 번들 컨테이너가 모두 표시됩니다. 각 번들에 포함된 창작자들의 창작이름, 창작크기, 언어를 살펴볼 수 있다. 카드 모드에서는 &lt; 및 > 버튼을 사용하여 여러 크리에이티브가 포함된 번들로 이미지를 스크롤할 수 있습니다.

#### 사용 가능한 작업

* 라이브러리에 표준 디스플레이, 표준 비디오 및 동적 디스플레이 번들 추가

* 번들에서 크리에이티브 나열 및 미리보기

* 번들 이름 편집

* 표준 디스플레이 번들에 표준 디스플레이 크리에이티브를 추가하고 표준 디스플레이 번들에서 표준 디스플레이 크리에이티브를 제거합니다.

* 표준 비디오 번들에 표준 비디오 크리에이티브를 추가하고 표준 비디오 번들에서 표준 비디오 크리에이티브를 제거합니다

* 번들 복제

* 번들 삭제

>[!MORELIKETHIS]
>
>* [Creative 라이브러리 관리](/help/creative/creative-libraries/creative-library-manage.md)
>* [Creative 라이브러리에 표준 크리에이티브 추가](creative-add-standard.md)
>* [Creative 번들 관리](bundle-manage.md)
>* [데이터 보기 사용자 지정](/help/creative/introduction/customize-data-views.md)
