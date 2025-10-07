---
title: 동적 광고용 워크플로우
description: 동적 광고 관리 워크플로우에 대해 알아봅니다.
feature: Creative Dynamic Creatives
source-git-commit: 0d7a7ab23173a061961c4b5c66ace5b69a746e86
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# 동적 광고용 워크플로우

*동적 광고를 만들 수 있는 권한이 있는 사용자*

다음 두 가지 방법 중 하나로 동적 광고를 설정할 수 있습니다.

* 워크플로우 1: 크리에이티브 라이브러리에 동적 광고를 추가할 때 동적 광고 설정 내에서 직접 광고 템플릿 및 광고 변형 카탈로그를 업로드합니다. 기존 피드 템플릿을 다운로드하여 카탈로그를 만들 수 있습니다.

  동일한 사람이 (피드 템플릿을 제외한) 모든 정보를 제공하여 광고를 만들 수 있는 경우 이 워크플로를 사용하십시오. 업로드된 파일은 나중에 사용할 수 있습니다.

* 워크플로우 2: 별도의 보기 내에서 광고 템플릿 및 광고 변형 카탈로그를 설정한 다음 이미 사용 가능한 광고 템플릿 및 카탈로그를 사용하여 크리에이티브에 동적 광고를 별도로 추가합니다.

  다른 사람이 다른 작업을 완료하거나 한 번에 하나의 작업만 완료하려는 경우 이 워크플로를 사용합니다.

## 워크플로우 1

>[!PREREQUISITES]
>
>* HTML5 형식의 광고 템플릿
>* CSV, TSV 또는 Microsoft Excel 스프레드시트(XLSX) 형식의 제품 카탈로그

1. Creative 라이브러리의 [동적 크리에이티브 만들기](/help/creative/creative-libraries/creative-add-dynamic.md). 다이내믹 HTML5 광고의 경우 광고 템플릿과 카탈로그를 업로드하십시오.

1. 광고 경험에 동적 크리에이티브 사용:

   1. 한 번에 모두 광고 경험에 첨부할 수 있는 [동적 광고 번들을 만듭니다](/help/creative/creative-libraries/bundle-manage.md).

   1. [타깃팅을 사용하여](/help/creative/experiences/experience-create-targeting.md) 또는 [타깃팅 없이](/help/creative/experiences/experience-create-no-targeting.md) 동적 광고 경험을 만들고 [경험에 Creative 번들을 할당](/help/creative/experiences/experience-assign-creative-bundles.md)합니다.

   1. [광고 경험 태그를 생성하고 구현](/help/creative/experiences/experience-tag-export.md)하여 DSP에서 광고로 실행하십시오.

      Adobe Advertising DSP에서 광고 경험을 광고로 사용하려면 광고 경험 태그를 Advertising DSP 캠페인에 업로드하십시오. 다른 DSP에서 광고 경험을 광고로 사용하려면 해당 DSP에서 광고 경험 태그를 구현하십시오.

## 워크플로 2

1. 사용 가능한 자산을 기반으로 동적 광고의 [광고 템플릿을 만듭니다](/help/creative/ad-templates/ad-template-manage.md). 광고 템플릿에는 원하는 광고 형식의 HTML5 파일과 (동적 HTML5 광고만 해당) 광고 특성이 있는 파일이 포함되어 있습니다.

1. 광고 요소 설정:

   * (단일 정적 HTML5 광고의 경우) 광고에 대한 이미지 에셋을 수집하고 [업로드](/help/creative/feeds/asset-manage.md)합니다.

   * (동적 HTML5 광고의 경우) 광고 요소의 카탈로그를 만듭니다.

      1. 각 광고 변형에 대해 하나의 행을 사용하여 Microsoft Excel 스프레드시트(XLSX) 형식으로 피드 파일을 만듭니다. 각 행에 이미지 이름을 포함합니다. 연결된 이미지 에셋을 별도로 수집합니다.

      1. [피드 파일 및 이미지 자산을 업로드합니다](/help/creative/feeds/asset-manage.md).

      1. 피드 파일(스프레드시트)의 필드를 Advertising Creative 백엔드의 필드에 매핑하려면 [피드 템플릿을 만듭니다](/help/creative/feeds/feed-template-manage.md).

      1. [지정된 피드 파일 및 지정된 피드 템플릿에서 카탈로그를 만들고](/help/creative/feeds/catalog-manage.md#feed-catalog-create), 만들 수 있는 광고 변형을 보려면 [카탈로그를 처리](/help/creative/feeds/catalog-manage.md#feed-catalog-process)하십시오.

         각 피드 파일은 하나의 카탈로그에 대해서만 사용할 수 있습니다.

         [ > ](/help/creative/feeds/job-status-track.md) > [!UICONTROL Creative] 탭에서 [!UICONTROL Feeds]카탈로그 처리 작업의 상태를 추적[!UICONTROL Job Status]할 수 있습니다.

1. Creative 라이브러리의 [동적 크리에이티브 만들기](/help/creative/creative-libraries/creative-add-dynamic.md). 다이내믹 HTML5 광고의 경우 지정된 광고 템플릿과 지정된 카탈로그를 사용하십시오.

1. 광고 경험에 동적 크리에이티브 사용:

   1. 한 번에 모두 광고 경험에 첨부할 수 있는 [동적 광고 번들을 만듭니다](/help/creative/creative-libraries/bundle-manage.md).

   1. [타깃팅을 사용하여](/help/creative/experiences/experience-create-targeting.md) 또는 [타깃팅 없이](/help/creative/experiences/experience-create-no-targeting.md) 동적 광고 경험을 만들고 [경험에 Creative 번들을 할당](/help/creative/experiences/experience-assign-creative-bundles.md)합니다.

   1. [광고 경험 태그를 생성하고 구현](/help/creative/experiences/experience-tag-export.md)하여 DSP에서 광고로 실행하십시오.

      Adobe Advertising DSP에서 광고 경험을 광고로 사용하려면 광고 경험 태그를 Advertising DSP 캠페인에 업로드하십시오. 다른 DSP에서 광고 경험을 광고로 사용하려면 해당 DSP에서 광고 경험 태그를 구현하십시오.
