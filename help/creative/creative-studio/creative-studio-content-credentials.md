---
title: Creative Studio의 C2PA 메타데이터
description: C2PA 메타데이터가 Creative Studio에서 생성 AI로 생성 또는 편집된 콘텐츠에 자동으로 연결되는 방법에 대해 알아봅니다.
product_v2: id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2: id: d0d9f2ed-c163-44e1-97a1-4ace121416b8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: d335c890ccc3ff8b2d391881660a71d10fcba53a
workflow-type: tm+mt
source-wordcount: 414
ht-degree: 2%

---

# [!UICONTROL Creative Studio]의 C2PA 메타데이터

[!UICONTROL Creative Studio]은(는) 생성 AI로 생성되거나 편집된 콘텐츠에 C2PA 메타데이터를 자동으로 연결하여 광고 콘텐츠의 출처를 보이지 않는 지속적인 메타데이터로 기록합니다. 메타데이터는 [콘텐츠 증명 및 진위 유지를 위한 연합](https://c2pa.org/)&#x200B;(C2PA)의 표준을 따릅니다.

## 컨텐츠 유형 및 해당 범위 {#cc-content-types}

| 컨텐츠 유형 | 지원됨? | 콘텐츠를 생성하는 AI 서비스 | 자격 증명을 생성하는 모델 |
| --- | --- | --- | --- |
| 이미지 | 예. 생성 AI로 이미지를 생성 또는 편집할 때 C2PA 메타데이터가 첨부되고, AI 비서가 수행하는 크로핑·리사이징 작업을 통해 보존된다. | [!DNL Adobe Firefly C2PA] | [!DNL Gemini Flash] |

## C2PA 메타데이터를 첨부하는 작업

다음 표에서는 [!UICONTROL Creative Studio] AI 길잡이에서 수행된 이미지 작업을 기반으로 C2PA 메타데이터가 첨부된 시기를 요약합니다.

| 액션 | 설명 | C2PA 메타데이터가 첨부되었습니까? | 사용 사례 예 |
| --- | --- | --- | --- |
| **이미지 생성** | 텍스트 프롬프트를 사용하여 새 이미지 만들기 | 이미지가 생성 AI에 의해 생성되므로 항상 그럴 수 있습니다. | 텍스트 프롬프트를 사용하여 광고 템플릿에 대한 새 배경 이미지나 로고를 생성합니다.<br><br>텍스트 프롬프트를 사용하여 광고 개념의 기본 이미지를 라이브러리에서 업로드한 자산으로 바꿉니다.<br><br>텍스트 프롬프트를 사용하여 광고 서식 파일에 배경 이미지의 변형을 생성합니다. |

## 콘텐츠가 이동하면 어떻게 됩니까? {#cc-content-moves}

사용자가 이미지 파일을 다운로드하거나 광고에서 제공하도록 전송될 때 전체 증명 체인은 유지됩니다.

## C2PA 메타데이터에는 무엇이 포함됩니까?

각 GenAI 생성 또는 변경에 대해 C2PA 메타데이터에 포함되는 내용은 다음과 같습니다. 에셋이 여러 번 변경되면 각 작업이 C2PA 메타데이터에 나타납니다.

* 사용된 AI 시스템의 이름 및 버전 정보([!DNL Adobe Firefly C2PA])
* 사용된 AI 모델([!DNL Gemini Flash])
* 사용법: GenAI를 사용하여 생성되었는지 또는 편집했는지 여부
* 콘텐츠 생성 및/또는 생성 AI 도구를 사용한 수정 시간과 날짜
* 고유 식별자(생성 AI의 각 사용을 구분하는 데 사용할 수 있음)

## 이미지에 대한 C2PA 메타데이터를 보려면 어떻게 해야 합니까?

이미지에 대한 전체 에셋 내역을 보려면

* https://contentauthenticity.adobe.com/inspect 또는 https://verify.contentauthenticity.org/과 같은 컨텐츠 신뢰성 검사 도구에서 이미지 파일을 엽니다.

* 이미지 메타데이터를 봅니다.

* 브라우저의 코드 검사 도구([!DNL Inspect])를 사용하여 이미지 코드를 봅니다.

![이미지에 대한 C2PA 메타데이터의 예](/help/creative/assets/cs-content-credentials-example.png "이미지에 대한 C2PA 메타데이터")

## 추가 리소스

* [[!DNL Adobe] 생성 AI 사용자 지침](https://www.adobe.com/kr/legal/licenses-terms/adobe-gen-ai-user-guidelines.html)

>[!MORELIKETHIS]
>
>* [Creative Studio 정보](/help/creative/creative-studio/creative-studio-about.md)
