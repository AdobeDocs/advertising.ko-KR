---
title: 여러 타사 광고 만들기
description: 한 번에 여러 타사 광고를 만드는 방법을 알아봅니다.
feature: DSP Ads
exl-id: be7c1cc4-3c17-4e37-aae7-c8601d2222a0
source-git-commit: 4b9cc5956d573b346eacdf71a8ea490c162b4660
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# 여러 타사 광고 만들기

타사 광고 서버에서 호스팅되는 크리에이티브 에셋을 가리키는 태그를 업로드하여 한 번에 최대 500개의 타사 광고를 만들 수 있습니다. 광고에 추적 픽셀을 포함할 수 있습니다.<!-- The bulksheet template for other ad servers says you can include 200. Which is it: 200 or 500? -->

제공된 템플릿을 사용하여 [!DNL DoubleClick] 및 [!DNL Flashtalking] 태그 시트 또는 수동으로 채워진 파일을 업로드할 수 있습니다.

>[!TIP]
>
> 가장 좋은 방법은 HTTPS를 사용하여 안전하게 제공되는 타사 광고를 사용하는 것입니다. HTTPS를 사용하여 제공되는 URL은 &quot;https&quot;로 시작합니다.

1. 주 메뉴에서 **[!UICONTROL Campaigns]**&#x200B;을(를) 클릭합니다.

1. 광고를 포함할 캠페인의 이름을 클릭합니다.

1. 데이터 테이블 위에서 **[!UICONTROL Create]**&#x200B;을(를) 클릭합니다. 메뉴의 광고 형식 섹션에서 **[!UICONTROL Bulk upload ads]**&#x200B;을(를) 클릭합니다.

1. 광고가 호스팅되는 광고 서버를 선택합니다. *[!UICONTROL DoubleClick]*, *[!UICONTROL Flashtalking]* 또는 *[!UICONTROL Other]*.

1. ([!DNL DoubleClick] 및 [!DNL Flashtalking] 광고) 각 비디오 에셋 및 각 디스플레이 에셋에 사용할 태그 유형을 선택합니다. 사용 가능한 옵션은 광고 서버에 따라 다릅니다.

1. (모든 광고 서버에서 [!DNL DoubleClick] 및 [!DNL Flashtalking]을(를) 제외한 광고) **[!UICONTROL Download this template]**&#x200B;을(를) 클릭하여 광고 데이터로 채우고 로컬로 저장할 수 있는 [!DNL Microsoft Excel] 스프레드시트(XLSX) 형식으로 템플릿을 다운로드합니다. 필수 열에는 [!UICONTROL Ad Name], [!UICONTROL VAST/VPAID URL or Ad Tag] 및 [!UICONTROL Ad Types]이(가) 포함됩니다.

1. **[!UICONTROL Upload]**&#x200B;을(를) 클릭하고 장치 또는 네트워크에서 .xlsx 또는 .xls 형식의 파일을 선택하십시오.

   [!DNL DoubleClick] 및 [!DNL Flashtalking] 광고의 경우 광고 서버에서 편집되지 않은 태그 시트를 업로드하십시오. 다른 광고 서버의 경우 3단계에서 다운로드한 템플릿을 사용합니다.

1. 업로드가 완료되면 **[!UICONTROL Start Building Ads]**&#x200B;을(를) 클릭합니다.

1. 각 광고의 세부 사항 및 상태를 검토합니다.

   1. (범용 비디오 광고에서 [!DNL Google] 또는 [!DNL Flashtalking] 태그를 사용) **[!UICONTROL Ad Type]** 필드를 클릭하고 **[!UICONTROL Universal Video]**&#x200B;을(를) 선택합니다.

   1. (범용 비디오 광고) 새 광고마다 ![편집](/help/dsp/assets/edit.png)을 클릭하고 [적용 가능한 비디오 형식](/help/dsp/campaign-management/ads/ad-settings-universal-video.md)을 선택한 다음 **저장**&#x200B;을 클릭합니다.

   1. 업로드된 태그에 대한 유효성 검사를 기반으로 하는 각 광고의 상태를 검토합니다.

   1. (선택 사항) 각 광고에 대해 다음 중 하나를 수행합니다.

      * 광고를 미리 보려면 광고 행에서 ![재생](/help/dsp/assets/play.png)을 클릭하세요.

      * 광고 세부 정보를 편집하려면 ![편집](/help/dsp/assets/edit.png)을 클릭하고 세부 정보를 편집한 다음 **저장**&#x200B;을 클릭합니다.

      * 광고를 제거하려면 광고 행에서 **[!UICONTROL X]**&#x200B;을(를) 클릭합니다.

1. **[!UICONTROL Create *N *개의 광고]**&#x200B;를 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * **[!UICONTROL Done]**&#x200B;을(를) 클릭합니다.

   * (광고가 거부된 경우, 선택 사항) 광고 레코드를 편집하고 검토를 위해 광고를 다시 제출하려면 다음을 수행하십시오.

      1. 광고 이름을 클릭합니다.

      1. 광고 설정을 편집합니다.

      1. **[!UICONTROL Save & submit for review]**&#x200B;을(를) 클릭합니다.

>[!NOTE]
>
>범용 비디오 광고는 범용 비디오 배치에만 첨부할 수 있습니다.

>[!MORELIKETHIS]
>
>* [광고 관리 정보](ad-about.md)
>* [광고 사양](ad-specs.md)
>* [단일 광고 만들기](ad-create.md)
>* [비디오: 타사 광고 태그를 일괄 업로드하는 방법](https://experienceleague.adobe.com/docs/advertising-learn/tutorials/dsp/bulk-upload-third-party-ad-tags.html?lang=ko)
>* 범용 비디오에 대한 [FAQ](/help/dsp/campaign-management/faq-universal-video.md)
