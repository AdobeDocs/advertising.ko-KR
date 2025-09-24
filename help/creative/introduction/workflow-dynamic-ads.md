---
title: 동적 광고의 워크플로
description: 동적 광고 관리 워크플로우에 대해 알아봅니다.
feature: Creative Dynamic Creatives
source-git-commit: e08a3c841e733840058f85a7ecc67571631314b3
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# 동적 광고의 워크플로

1. 사용 가능한 자산을 기반으로 동적 광고의 [광고 템플릿을 만듭니다](/help/creative/ad-templates/ad-template-manage.md)

1. 광고 요소 설정:

   * (단일 정적 HTML5 광고의 경우) 광고에 대한 이미지 에셋을 수집하고 [업로드](/help/creative/feeds/asset-manage.md)합니다.

   * (동적 HTML5 광고의 경우) 광고 요소의 카탈로그를 만듭니다.

      1. 각 광고 변형에 대해 하나의 행을 사용하여 Microsoft Excel 스프레드시트(XLSX) 형식으로 피드 파일을 만듭니다. 각 행에 이미지 이름 또는 Adobe Experience Manager에 대한 참조를 포함합니다. 연결된 이미지 에셋을 별도로 수집합니다.

      1. [피드 파일 및 이미지 자산을 업로드합니다](/help/creative/feeds/asset-manage.md).

      1. 피드 파일(스프레드시트)의 필드를 Advertising Creative 백엔드의 필드에 매핑하려면 [피드 템플릿을 만듭니다](/help/creative/feeds/feed-template-manage.md).

      1. [지정된 피드 파일 및 지정된 피드 템플릿에서 카탈로그를 만들고](/help/creative/feeds/catalog-manage.md#feed-catalog-create), 만들 수 있는 광고 변형을 보려면 [카탈로그를 처리](/help/creative/feeds/catalog-manage.md#feed-catalog-process)하십시오.

         각 피드 파일은 하나의 카탈로그에 대해서만 사용할 수 있습니다.

         [ > ](/help/creative/feeds/job-status-track.md) > [!UICONTROL Creative] 탭에서 [!UICONTROL Feeds]카탈로그 처리 작업의 상태를 추적[!UICONTROL Job Status]할 수 있습니다.

1. Creative 라이브러리의 [동적 크리에이티브 만들기](/help/creative/creative-libraries/creative-add-dynamic.md). 다이내믹 HTML5 광고의 경우 지정된 광고 템플릿과 지정된 카탈로그를 사용하십시오.

1. 한 번에 모두 광고 경험에 첨부할 수 있는 [동적 광고 번들을 만듭니다](/help/creative/creative-libraries/bundle-manage.md).

1. [타깃팅 포함](/help/creative/experiences/experience-create-targeting.md) 또는 [타깃팅 없음](/help/creative/experiences/experience-create-no-targeting.md)으로 동적 광고 경험을 만들고 [이러한 경험을 동적 광고 경험에 번들로 할당](/help/creative/experiences/experience-assign-creative-bundles.md)합니다.

1. [광고 경험 태그를 생성하고 구현](/help/creative/experiences/experience-tag-export.md)하여 DSP에서 광고로 실행하십시오.

   Adobe Advertising DSP에서 광고 경험을 광고로 사용하려면 광고 경험 태그를 Advertising DSP 캠페인에 업로드하십시오. 다른 DSP에서 광고 경험을 광고로 사용하려면 해당 DSP에서 광고 경험 태그를 구현하십시오.
