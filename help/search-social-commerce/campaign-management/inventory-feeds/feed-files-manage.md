---
title: 인벤토리 데이터 피드 파일 관리
description: 피드 데이터 처리 방법을 제어하는 설정을 구성하는 방법에 대해 알아봅니다.
exl-id: 7d19ecc0-c939-4996-b22b-970ce8644b09
feature: Search Inventory Feeds
source-git-commit: 67fe8581832dc0762d62908d01672e53cc95b847
workflow-type: tm+mt
source-wordcount: '1242'
ht-degree: 0%

---

# 인벤토리 데이터 피드 파일 관리

*[!DNL Google Ads], [!DNL Microsoft Advertising], [!DNL Yahoo! Japan Ads] (삭제 작업만) 및 [!DNL Yandex] 계정만*

자체 피드 데이터를 제출하는 경우 제품 데이터가 포함된 파일을 업로드하여 제품 데이터를 기반으로 캠페인 구조, 광고 및 키워드를 동적으로 만들어야 합니다. 그런 다음 광고 네트워크별 광고 템플릿에 연결하고 템플릿을 통해 데이터를 처리하여 관련 광고 네트워크에 데이터를 게시할 수 있습니다. 여러 템플릿을 하나의 피드 파일과 연결할 수 있지만 각 템플릿은 하나의 피드 파일에만 연결할 수 있습니다.

>[!NOTE]
>
>머천트 센터 계정에서 직접 데이터를 사용하는 경우에는 파일을 업로드하지 마십시오.

다음 방법 중 하나로 데이터 피드 파일을 업로드하고 처리할 수 있습니다.

* **FTP 자동 사용:** FTP 디렉터리에 직접 파일을 업로드할 수 있습니다. 피드 서비스는 두 시간마다 새 파일을 확인합니다. 파일을 처음 업로드한 후에는 광고 네트워크별 템플릿과 연결할 수 있습니다. 나중에 같은 이름으로 업로드하는 모든 파일은 자동으로 동일한 템플릿에 연결됩니다. [피드 데이터 설정을 구성하는 방법](feed-settings-manage.md)에 따라 검색, 소셜 및 Commerce은 적용 가능한 모든 템플릿을 통해 피드 데이터를 자동으로 전파하고 선택적으로 결과 캠페인 및 광고 데이터를 관련 광고 네트워크에 게시할 수 있습니다.

  데이터 파일을 저장하고 자동으로 처리하기 위해 FTP 디렉터리를 설정하려면 Adobe 계정 팀에 문의하십시오.

* **수동 처리:** [!UICONTROL Advanced] (ACM) 보기에서 피드 파일을 수동으로 [업로드](#feed-file-upload)할 수 있습니다. 피드 파일을 하나 이상의 광고 네트워크별 [템플릿](/help/search-social-commerce/campaign-management/inventory-feeds/ad-templates/ad-template-manage.md)과 연결한 후 [피드 데이터 설정](feed-settings-manage.md)에 따라 [템플릿을 통해 피드 데이터를 전달](feed-data-propagate.md)하여 캠페인 및 광고 데이터를 생성할 수 있습니다. 선택적으로 캠페인 계층 보기 내에서 생성된 데이터를 미리 보거나, 검토를 위해 일괄 시트 파일을 생성하거나, 광고 네트워크에 즉시 게시하기 위해 일괄 시트 파일을 생성할 수 있습니다. 데이터를 즉시 게시하지 않으면 [미리 보기](propagated-data-view.md)하고 나중에 [게시](propagated-data-post.md)할 수 있습니다. 나중에 기존 템플릿 연결을 끊지 않고 [기존 피드 파일을 새 파일로 바꾸기](#feed-file-replace)할 수 있습니다.

## 피드 파일 요구 사항

개별 파일에는 특정 데이터 필드가 필요하지 않지만, 각 파일에는 다음 필드가 필요합니다.

* 파일의 첫 번째 줄에는 연결된 템플릿의 동적 매개 변수에 해당하는 열 이름(*headers*)이 포함되어야 합니다. 나머지 줄에는 열 이름에 해당하는 데이터가 포함되어야 합니다. 각 데이터 라인(행)은 하나의 캠페인 또는 하나의 광고와 같은 하나의 계정 구성 요소에만 속해야 합니다. 모든 행의 값은 탭이나 쉼표로 구분해야 합니다. 아래의 [CSV 예제 파일](#example-csv-feed-file) 및 [TSV 예제 파일](#example-tsv-feed-file)을 참조하십시오.

* 파일의 크기는 제한이 없지만 `.tsv`(탭으로 구분된 값의 경우), `.txt`([!DNL Unicode] 규격 ASCII 텍스트의 경우), `.csv`(쉼표로 구분된 값의 경우) 또는 `.zip`(TSV 파일로 압축 해제되는 압축 ZIP 형식의 단일 파일의 경우) 파일 확장명 중 하나가 있어야 합니다.

* 파일 이름은 대/소문자를 구분하며 다음 문자를 포함할 수 없습니다. `# % & * | \ : " < > . ? /`

* FTP 디렉토리에 파일을 저장하는 경우 파일의 각 버전에 대해 동일한 파일 이름을 사용해야 합니다.

* ([!DNL Google Ads] 템플릿만 해당) 템플릿에 텍스트 광고에서 Param2 또는 Param2 광고 매개 변수가 사용되는 경우 피드 파일의 해당 데이터 필드에는 금전 기호가 없는 숫자 데이터가 포함되어야 합니다.

* 기존 계정 구성 요소를 업데이트하려면 기존 캠페인의 이름(관련 있는 경우 구성 요소)을 포함합니다. 기존 구조를 지정하지 않으면 새 구성 요소가 만들어집니다.

### 쉼표로 구분된 피드 파일의 예 {#example-csv-feed-file}

```
Product Category,Product Name,Discount Percentage
electronics,iPods,10
apparel,Shirts,15
shoes,Clarks,20
```

### 탭으로 구분된 피드 파일의 예 {#example-tsv-feed-file}

```
Product Category<TAB>Product Name<TAB>Discount Percentage
electronics<TAB>iPods<TAB>10
apparel<TAB>Shirts<TAB>15
shoes<TAB>Clarks<TAB>20
```

## 우수 사례

* 국제 문자가 포함된 데이터의 경우 TSV 또는 TXT 형식의 파일을 사용하십시오.

* 제한된 수동 검토 또는 편집으로 반복 가능한 프로세스를 달성하려면 피드 파일 및 해당 계정 구조 데이터를 다음과 같이 설정합니다.

   * 계정 구조를 만들거나 기존 계정 구조에 매핑하기에 충분한 데이터가 포함된 열과 행을 포함합니다. 이상적으로는 제품 분류법에 밀접하게 연결되어 있고 피드 데이터가 쉽게 매핑되는 기존 계정 구조를 사용하는 것이 좋습니다.

   * 광고 카피에 사용할 수 있을 만큼 짧은 설명을 포함합니다.

   * 제품 행 간에 일관된 데이터 패턴 및 이름 지정 규칙을 사용합니다.

   * 선행 공백 및 후행 공백을 모두 제거합니다.

   * 깨진 문자를 모두 제거합니다.

## 피드 파일 보기 또는 다운로드

수동으로 또는 FTP를 사용하여 업로드한 피드 파일을 열거나 다운로드할 수 있습니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Advanced (ACM)]**&#x200B;을(를) 클릭합니다. 그러면 [!UICONTROL Templates] 탭이 열립니다.

1. 피드 파일을 찾습니다.

1. 템플릿 목록에서 피드 파일을 사용하는 템플릿을 찾습니다.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL Feeds]**&#x200B;을(를) 클릭하여 모든 피드 파일 목록을 엽니다.

1. 피드 파일 이름을 클릭합니다.

1. 브라우저의 일반 절차에 따라 파일을 열거나 저장합니다.

자세한 내용은 브라우저의 온라인 도움말을 참조하십시오.

## 피드 파일 수동 업로드 {#feed-file-upload}

>[!NOTE]
> 템플릿을 수동으로 업로드한 파일에 연결하지만, 이름, 파일 확장명 및 문법적 대소문자가 동일한 다른 파일을 FTP를 통해 업로드하는 경우 템플릿을 통해 데이터를 전파할 때 FTP 파일이 사용됩니다. 예를 들어 myfile.csv는 myfile.csv를 대체하지만 Myfile.CSV는 그렇지 않습니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Advanced (ACM)]**&#x200B;을(를) 클릭합니다. 그러면 [!UICONTROL Templates] 탭이 열립니다.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL Feeds]**&#x200B;을(를) 클릭합니다.

1. 데이터 테이블 위에서 **[!UICONTROL Upload]**&#x200B;을(를) 클릭합니다.

1. 전체 경로와 파일 이름을 입력하거나 **[!UICONTROL Browse]**&#x200B;을(를) 클릭하여 장치 또는 네트워크에서 파일을 찾아 업로드할 파일을 지정하십시오.

1. **[!UICONTROL Upload]을(를) 클릭합니다.

파일의 모든 필드에 대한 유효성이 검사됩니다. 나중에 값을 수정할 때까지 필드 길이가 잘못된 항목을 게시할 수 없습니다. 파일의 모든 열 이름을 템플릿에서 동적 매개 변수로 사용할 수 있습니다.

## 피드 파일 바꾸기 {#feed-file-replace}

새 파일의 파일 이름이나 확장명이 다르더라도 피드 파일을 바꾸면 기존의 모든 템플릿 연결이 유지됩니다. 원래 이전 파일과 연관된 모든 템플릿을 통해 데이터를 전파할 때 새 파일이 사용됩니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Advanced (ACM)]**&#x200B;을(를) 클릭합니다. 그러면 [!UICONTROL Templates] 탭이 열립니다.

1. 다음 중 하나를 수행합니다.

   * 적용 가능한 템플릿의 [!UICONTROL Feed] 열에서 ![추가 옵션](/help/search-social-commerce/assets/options.png "추가 옵션")을 클릭하고 **[!UICONTROL Re-upload]**&#x200B;을(를) 선택합니다.

   * 데이터 테이블 위의 도구 모음에서 **[!UICONTROL Feeds]**&#x200B;을(를) 클릭합니다. 피드 파일 목록에서 기존 파일 이름 옆에 있는 확인란을 선택합니다. 데이터 테이블 위에서 **[!UICONTROL Upload]**&#x200B;을(를) 클릭합니다.

   >[!NOTE]
   >
   >피드 파일의 원본(&quot;[!UICONTROL FTP]&quot; 또는 수동으로 업로드한 파일의 경우 &quot;&amp;mdash&quot;)이 [!UICONTROL Source] 열에 포함되어 있습니다.

1. 전체 경로와 파일 이름을 입력하거나 **[!UICONTROL Browse]**&#x200B;을(를) 클릭하여 장치 또는 네트워크에서 파일을 찾아 업로드할 파일을 지정하십시오.

새 파일의 파일 이름이나 확장명이 다르더라도 기존 파일을 새 파일로 덮어씁니다.

1. **[!UICONTROL Re-Upload]**&#x200B;을(를) 클릭합니다.

파일의 모든 필드에 대한 유효성이 검사됩니다. 나중에 값을 수정할 때까지 필드 길이가 잘못된 항목을 게시할 수 없습니다. 파일의 모든 열 이름을 템플릿에서 동적 매개 변수로 사용할 수 있습니다.

## 피드 파일 삭제

수동으로 또는 FTP를 통해 업로드된 모든 피드 파일을 삭제할 수 있습니다. 피드 파일을 삭제하면 더 이상 템플릿과 연결되지 않습니다.

1. 메인 메뉴에서 **[!UICONTROL Search]> [!UICONTROL Campaigns] >[!UICONTROL Advanced (ACM)]**&#x200B;을(를) 클릭합니다. 그러면 [!UICONTROL Templates] 탭이 열립니다.

1. 데이터 테이블 위의 도구 모음에서 **[!UICONTROL Feeds]**&#x200B;을(를) 클릭합니다.

1. 삭제할 각 파일 옆의 확인란을 선택합니다.

1. 데이터 테이블 위에서 **[!UICONTROL Delete]**&#x200B;을(를) 클릭합니다.

1. 확인 메시지에서 **[!UICONTROL Yes]**&#x200B;을(를) 클릭합니다.

>[!MORELIKETHIS]
>
>* [인벤토리 피드 정보](/help/search-social-commerce/campaign-management/inventory-feeds/inventory-feeds-about.md)
>* [템플릿을 통해 피드 데이터 전파](feed-data-propagate.md)
>* [피드에서 생성된 데이터 보기](propagated-data-view.md)
>* [피드에서 생성된 데이터 편집](propagated-data-edit.md)
>* [피드에서 생성된 캠페인 데이터를 광고 네트워크에 게시](propagated-data-post.md)
>* [인벤토리 피드 데이터에 대한 게시 작업 중지](stop-job.md)
>* [피드에서 생성된 데이터의 상태](propagated-data-status.md)
