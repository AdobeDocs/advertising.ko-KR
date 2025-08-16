---
title: 비디오 광고 경험 태그에 대한 코드 변환 옵션 사용자 지정
description: 비디오 광고 태그에 대한 코드 변환 옵션을 사용자 지정하는 방법을 알아봅니다.
feature: Creative Experiences
exl-id: 6100213c-2e7d-4e98-a3ab-045ca10e5174
source-git-commit: f7d5bf3193cb41ca2a0d4415998209e5a9b724ba
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# 비디오 광고 경험 태그에 대한 코드 변환 옵션 사용자 지정

비디오 광고 경험에 대한 트랜스코딩 옵션을 사용자 지정하여 게시자 간에 빠르게 재생하고 품질을 제어할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Experiences]**&#x200B;을(를) 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * 카드 보기에서 경험 이름 옆의 **[!UICONTROL ...]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Tag Manager]**&#x200B;을(를) 클릭합니다.

   * 테이블 보기에서 행 위에 커서를 놓고 **[!UICONTROL More]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Tag Manager]**&#x200B;을(를) 클릭합니다.

1. 적용 가능한 광고 태그의 행 위에 커서를 놓고 **[!UICONTROL More]**&#x200B;을(를) 클릭한 다음 **[!UICONTROL Video Settings]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Publisher-specific transcodes]** 목록에서 코드 변환을 적용할 DSP을 선택합니다.

1. **[!UICONTROL Save Settings]**&#x200B;을(를) 클릭합니다.

## 기본([!DNL Adobe] DSP) 코드 변환 사양

| 파일 유형 | 치수 | 비디오 비트율 | 비디오 프레임 속도 | 오디오 비트율 | 오디오 샘플링 속도 | 오디오 레벨 |
|---|---|---|---|---|---|---|
| mp4 | 640x360 | 1000kbps | 23.98fps | 128Kbps | 48.000킬로헤르츠 | 24LKFS(+/- 2.0dB) |
| mp4 | 400x300 | 1000kbps | 23.98fps | 128Kbps | 48.000킬로헤르츠 | 24LKFS(+/- 2.0dB) |
| mp4 | 1024x768 | 500Kbps | 23.98fps | 128Kbps | 48.000킬로헤르츠 | 24LKFS(+/- 2.0dB) |
| mp4 | 640x480 | 1000kbps | 23.98fps | 128Kbps | 48.000킬로헤르츠 | 24LKFS(+/- 2.0dB) |
| mp4 | 960x540 | 2000kbps | 23.98fps | 128Kbps | 48.000킬로헤르츠 | 24LKFS(+/- 2.0dB) |
| mp4 | 960x720 | 2000kbps | 23.98fps | 128Kbps | 48.000킬로헤르츠 | 24LKFS(+/- 2.0dB) |
| mp4 | 1280x720 | 2000kbps | 23.98fps | 128Kbps | 48.000킬로헤르츠 | 24LKFS(+/- 2.0dB) |
| mp4 | 1920x1080 | 3500Kbps | 23.98fps | 128Kbps | 44.100킬로헤르츠 | 24LKFS(+/- 2.0dB) |
| mp4 | 640x360 | 800Kbps | 23.98fps | 96kbps | 48.000킬로헤르츠 | 24LKFS(+/- 2.0dB) |
| mp4 | 640x360 | 400Kbps | 23.98fps | 128Kbps | 48.000킬로헤르츠 | 24LKFS(+/- 2.0dB) |
| mp4 | 1920x1080 | 16000kbps | 23.98fps | 256kbps | 48.000킬로헤르츠 | 24LKFS(+/- 2.0dB) |

>[!MORELIKETHIS]
>
>* [크리에이티브 라이브러리 정보](/help/creative/creative-libraries/creative-libraries-about.md)
>* [타깃팅으로 경험 만들기](/help/creative/experiences/experience-create-targeting.md)
>* [적용 가능한 광고 크기에 대한 광고 태그를 수동으로 만듭니다](experience-tag-create-manually.md)
>* [라이브 경험에 대한 광고 경험 태그 내보내기 및 구현](experience-tag-export.md)
