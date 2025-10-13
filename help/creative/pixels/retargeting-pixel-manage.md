---
title: 픽셀 재타겟팅 관리
description: 광고 경험의 타겟으로 사용할 리타기팅 픽셀을 만들고 구현하는 방법에 대해 알아봅니다.
feature: Creative Pixels
exl-id: dcd13c5a-315d-4380-99f9-6dbab3e1e1be
source-git-commit: ed3bf0200d3d3b31ef80c790c4e702914459c521
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 0%

---

# 픽셀 재타겟팅 관리

<!-- Note to self: These aren't segments -- we don't create a pool of users. -->

사용자 쿠키 또는 범용 ID를 사용하여 광고주의 랜딩 페이지 또는 전환 페이지의 방문자를 식별하는 재타겟팅 픽셀을 만들 수 있습니다. 픽셀은 방문자가 페이지에서 수행하는 가장 최근 이벤트를 추적하고 해당 방문자에 대해 페이지가 추적하는 특정 속성을 캡처합니다. 픽셀을 만든 후 관련 웹 페이지에 삽입할 픽셀 태그를 생성하여 방문자 추적을 시작합니다.<!-- Note to self: surfer id=cookie or universal ID -->

그런 다음 광고 경험 내의 크리에이티브에 대한 타겟으로 픽셀을 사용하여 픽셀과 연관된 웹 페이지를 이전에 방문한 지정된 속성을 가진 사용자에게만 광고를 표시할 수 있습니다. 예를 들어, 웹 페이지에서 해당 속성 값을 추적하는 경우 크기 10의 빨간색 신발을 보는 방문자를 타깃팅할 수 있습니다.<!-- better example? Make sure they match attribute examples below --> 경험 수준 대상은 DSP의 타깃팅 옵션과 함께 적용됩니다. 계층 타깃팅 동작은 DSP에 따라 다를 수 있습니다.

프로필 재타겟팅은 180일 동안 저장됩니다.

픽셀 예:

```
<img src="https://creative-assets-uat.efrontier.com/creative/scripts/rt.js?advId=141731&pxId=oGwrDCSZRWu5ZQKSEy8Y&ut1=--Insert Color--&ut2=--Insert Size--" />  <script src="https://creative-assets-uat.efrontier.com/creative/scripts/rt.js?advId=141731&cro=F&id5Consent=T&id5pid=--Insert ID5_PARTNER_ID--&lrConsent=T&pxId=oGwrDCSZRWu5ZQKSEy8Y&ut1=--Insert Color--&ut2=--Insert Size--"></script>
```

>[!NOTE]
>
> * [!DNL Creative]은(는) Advertising DSP에 대해서만 범용 ID를 지원합니다.
>* 또한 Adobe Audience Manager 및 Adobe Analytics의 자사 대상을 [경험의 크리에이티브 대상](/help/creative/experiences/experience-settings-targeting.md)(으)로 사용할 수 있습니다.
>* Advertising DSP 배치 내에서 경험을 광고로 사용할 때 DSP에서 사용할 수 있는 모든 대상자에게 배치를 타깃팅할 수 있습니다. [사용자 지정 대상 세그먼트 태그를 만들어](/help/dsp/audiences/custom-segment-create.md) 특정 랜딩 페이지에 대한 모든 방문자를 추적한 다음 해당 세그먼트를 배치를 위한 크리에이티브 대상으로 사용할 수도 있습니다. Advertising DSP은 배치 수준 타깃팅의 맨 위에(대신 아님) 광고 수준 타깃팅을 적용합니다.
>* 광고 타깃팅을 위한 추적을 옵트아웃한 웹 사이트 방문자는 대상 세그먼트 또는 재타깃팅 프로필을 기반으로 개인화된 크리에이티브 콘텐츠가 포함된 광고를 받지 않습니다.

## 리타겟팅 픽셀 만들기

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Pixels]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위에서 **[!UICONTROL Creative]**&#x200B;을(를) 클릭한 다음 > **[!UICONTROL Retargeting Pixel]**&#x200B;을(를) 선택합니다.

1. [픽셀 설정 재지정](#retargeting-pixel-settings)을 지정하십시오.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

1. 광고주 또는 웹 사이트 연락처에 제공할 픽셀 태그를 [생성](#retargeting-pixel-generate)합니다.

   재타겟팅 픽셀 태그는 페이지의 마지막 동작이어야 합니다.<!-- verify here and below -->

   광고주의 IT 부서 또는 다른 그룹은 태그 배포를 예약하거나 그에 대한 정보를 받아야 할 수 있습니다.

## 리타겟팅 픽셀 편집

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Pixels]**&#x200B;을(를) 클릭합니다.

1. 픽셀 이름 위에 커서를 놓고 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

1. [픽셀 설정 다시 타깃팅](#retargeting-pixel-settings)을(를) 편집합니다.

1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

1. [원래 태그를 대체할 수 있도록 광고주나 웹 사이트 연락처에 제공할 픽셀 태그를 생성](#retargeting-pixel-generate)합니다.

   픽셀 태그 재타겟팅은 랜딩 페이지의 마지막 작업이어야 합니다.

   광고주의 IT 부서 또는 다른 그룹은 태그 배포를 예약하거나 그에 대한 정보를 받아야 할 수 있습니다.

## 리타겟팅 픽셀에 대한 태그 생성 {#retargeting-pixel-generate}

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Pixels]**&#x200B;을(를) 클릭합니다.

1. 픽셀 이름 위에 커서를 놓고 **[!UICONTROL Generate Tag]**&#x200B;을(를) 클릭합니다.

1. 태그를 컴퓨터의 클립보드에 복사하려면 **[!UICONTROL Copy to Clipboard]**&#x200B;을(를) 클릭합니다. 그러면 텍스트를 저장할 파일에 붙여넣을 수 있습니다.

1. 픽셀 태그에서 각 &quot;`<img src>`&quot;을(를) 값으로 대체하여 `<script src>` 및 `Insert <attribute>` 섹션 모두에서 각 특성의 값을 지정하십시오. 태그가 범용 ID를 캡처하는 경우 ID5 파트너 ID를 지정합니다.

   추가 속성을 수동으로 추가하는 경우 URL 인코딩을 포함하십시오.

   예를 들어 &quot;category&quot;, &quot;color&quot; 및 &quot;size&quot; 특성을 포함하고 ID5 유니버설 ID를 캡처한 경우 픽셀 태그에 `&ut1=--Insert category--&ut2=--Insert color--&ut3=--Insert size--` 및 `&id5pid=--Insert ID5_PARTNER_ID--` 매개 변수가 포함됩니다. 크기 10의 빨간색 샌들을 선택하는 사용자를 타겟팅하려면 이미지 태그와 스크립트 태그의 매개 변수를 모두 `&ut1=sandals&ut2=red&ut3=10`(으)로 변경하고 스크립트 태그에 ID5 파트너 ID(예: `&id5pid=0123456789`)를 입력하십시오.

   `<img src="https://creative-assets-uat.efrontier.com/creative/scripts/rt.js?advId=141731&pxId=oGwrDCSZRWu5ZQKSEy8Y&ut1=--sandals--&ut2=--red--&ut3=--10--" />  <script src="https://creative-assets-uat.efrontier.com/creative/scripts/rt.js?advId=141731&cro=F&id5Consent=T&id5pid=--0123456789--&lrConsent=T&pxId=oGwrDCSZRWu5ZQKSEy8Y&ut1=--sandals--&ut2=--red--&ut3=--10--"></script>`

1. 광고주나 웹 사이트 연락처에 완성된 픽셀 태그를 삽입할 관련 랜딩 페이지 목록과 함께 제공합니다.

   픽셀 태그 재타겟팅은 랜딩 페이지의 마지막 작업이어야 합니다.

   광고주의 IT 부서 또는 다른 그룹은 태그 배포를 예약하거나 그에 대한 정보를 받아야 할 수 있습니다.

## 리타겟팅 픽셀 삭제

1. 메인 메뉴에서 **[!UICONTROL Creative]** > **[!UICONTROL Creative Pixels]**&#x200B;을(를) 클릭합니다.

1. 픽셀 이름 위에 커서를 놓고 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

## 픽셀 설정 재타겟팅 {#retargeting-pixel-settings}

**[!UICONTROL Pixel Name]:** 픽셀의 이름입니다. **참고:** 픽셀 태그에는 픽셀 이름이 아닌 픽셀 ID(`pxId=<ID>`)가 포함됩니다.

**[!UICONTROL Advertiser]:**(기존 픽셀의 경우 읽기 전용) 픽셀을 추적하는 광고주입니다.

**[!UICONTROL Attribute 1]:** &quot;SKU&quot;, &quot;category&quot;, &quot;size&quot; 또는 페이지 또는 페이지에 표시된 제품의 기타 특성과 같이 픽셀 태그에 포함할 특성입니다. 관련 웹 페이지에 삽입하기 전에 픽셀 태그의 속성 값을 지정합니다.

픽셀에 노출된 사용자에게 광고 경험을 타깃팅할 때 타깃팅 설정은 크리에이티브를 표시하기 위해 존재해야 하는 속성 값을 지정합니다.

픽셀 태그에 포함할 **[!UICONTROL Attribute 2]**, **[!UICONTROL Attribute 3]**, **[!UICONTROL Attribute 4]**, **[!UICONTROL Attribute 5]:**(선택 사항) 추가 특성입니다. 관련 웹 페이지에 삽입하기 전에 픽셀 태그의 각 추가 속성에 대한 값을 지정합니다.

픽셀에 노출된 사용자에게 광고 경험을 타깃팅할 때 타깃팅 설정은 크리에이티브를 표시하기 위해 존재해야 하는 속성 값을 지정합니다.

**[!UICONTROL Advanced]** > **[!UICONTROL Universal IDs]:**(새 픽셀만 해당, 선택 사항) 추적할 픽셀 태그에 대한 범용 ID 유형:

* *[!UICONTROL ID5]:* 픽셀 태그가 [!DNL ID5]개의 ID를 추적합니다. 범용 ID에 게재되는 노출에 대해서는 요금이 부과되지 않습니다.

* *[!UICONTROL Ramp ID]:* 픽셀 태그가 [!DNL Ramp IDs]을(를) 추적합니다. 범용 ID에 게재되는 노출에 대해서는 요금이 부과되지 않습니다.

이 기능을 사용하려면 새 ID 유형에 범용 ID를 사용하기 전에 사용자 또는 DSP 계정의 다른 사용자가 범용 ID 사용에 대한 서비스 약관에 동의해야 합니다. 관리 서비스 계약을 보유한 고객의 경우 Adobe 계정 팀이 사용자의 동의를 얻고 조직을 대신하여 약관에 동의합니다. 용어를 읽으려면 **[!UICONTROL Terms of Service]**&#x200B;을(를) 클릭합니다. 약관에 동의하려면 약관의 맨 아래로 스크롤하여 **[!UICONTROL Accept]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [타깃팅된 광고 경험 설정](/help/creative/experiences/experience-settings-targeting.md)
>* [광고 경험 정보](/help/creative/experiences/experience-about.md)
