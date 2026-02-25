---
title: 보고 및 시뮬레이션을 위한 오프라인 계정 데이터 업로드
description: 보고 및 시뮬레이션 지원을 위해 오프라인 계정 데이터를 수동으로 업로드하거나  [!DNL Amazon] [!DNL S3] 버킷에 업로드하는 방법을 알아봅니다. 로그 파일은 업로드 작업의 진행 상황을 추적합니다.
source-git-commit: bfa5403ff66bed73797fc4c7115b8c043856745d
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 0%

---

# 보고 및 시뮬레이션을 위한 오프라인 계정 데이터 업로드

*계정 데이터 업로드를 사용할 수 있는 광고주*

보고 및 성능 시뮬레이션에 대한 API 지원 없이 계정에 대한 캠페인 컨텐츠 및 오프라인 비용, 클릭 및 전환 데이터를 업로드하십시오.

[!UICONTROL Upload Logs] 기능을 사용하여 업로드 작업의 진행 상황을 추적할 수 있습니다.

* 계정에 대해 업로드된 각 파일의 목록을 봅니다. 각 파일 업로드 작업에 대한 정보에는 파일 이름, 업로드 채널(*[!UICONTROL Cloud Storage]* 또는 *[!UICONTROL Drag & Drop]*), 동기화 날짜 및 상태, 업로드가 완료되지 않은 이유 등이 포함됩니다.

* 모든 작업에 대해 업로드된 계정 엔티티 및 관련 지표가 있는 파일을 다운로드합니다. 파일은 쉼표로 구분된 값(CSV) 형식입니다.

## 계정 데이터 수동으로 업로드

파일에 데이터를 수동으로 업로드하여 캠페인 콘텐츠 및 비용, 클릭 및 전환 데이터로 계정을 채울 수 있습니다.

<!--
See "XXX" for information about supported ad networks and account structures.

[supported ad networks and campaign types](/help/search-social-commerce/introduction/supported-inventory.md)
-->

1. 주 메뉴에서 **[!UICONTROL Setup]** \> **[!UICONTROL Accounts]**&#x200B;을(를) 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * [!UICONTROL Accounts] 보기에서:

      1. 계정 이름 옆의 확인란을 선택한 다음 일괄 작업 도구 모음에서 **[!UICONTROL Upload]**&#x200B;을(를) 클릭합니다.

      1. 파일을 상자로 끌어 놓거나 **[!UICONTROL Browse Files]**&#x200B;을(를) 클릭하고 장치나 네트워크에서 파일을 선택합니다.

      1. **[!UICONTROL Upload Files]**&#x200B;을(를) 클릭합니다.

   * (계정 설정에서):

      1. 다음 방법 중 하나로 계정을 선택합니다.

         * 계정 이름 위에 커서를 놓고 **..**&#x200B;을 클릭한 다음 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

         * 계정 이름 옆의 확인란을 선택한 다음 일괄 작업 도구 모음에서 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

      1. **[!UICONTROL Upload File]** 탭을 클릭합니다.

      1. 파일을 상자로 끌어 놓거나 **[!UICONTROL Browse Files]**&#x200B;을(를) 클릭하고 장치나 네트워크에서 파일을 선택합니다.

      1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

&#x200B;# [!DNL Amazon] [!DNL S3] 버킷에 계정 데이터 업로드 {#data-upload-s3}

[!DNL Amazon Web Services]&#x200B;(AWS) [!DNL Simple Storage Service]&#x200B;([!DNL S3]) 버킷의 Search, Social 및 Commerce 할당 폴더에 데이터를 업로드하여 캠페인 콘텐츠와 비용, 클릭 및 전환 데이터로 계정을 채울 수 있습니다.

<!--
See "XXX" for information about supported ad networks and account structures.

[supported ad networks and campaign types](/help/search-social-commerce/introduction/supported-inventory.md)
-->

>[!PREREQUISITES]
>
>* Adobe 계정 팀에 문의하여 검색, 소셜 및 Commerce 광고주 계정에 대한 계정 데이터 업로드를 활성화하십시오. 팀은 [!DNL S3] 버킷에 조직별 폴더를 쉽게 만들 수 있으며, 작업이 완료되면 알려 줍니다.<!-- Add more context about the bucket we'll use here or in the intro. Do we have one bucket (potentially with multiple folders) per client, or do we share them (if so, do we need to state how in docs? -->
>* 계정의 [!DNL S3] 클라우드 저장소 경로, 액세스 키 ID 및 비밀 액세스 키를 검색합니다. 조직의 모든 데이터 업로드 <!-- naming convention?--> 계정에 대해 동일한 액세스 키 ID 및 비밀 액세스 키가 사용됩니다.

1. 주 메뉴에서 **[!UICONTROL Setup]** \> **[!UICONTROL Accounts]**&#x200B;을(를) 클릭합니다.

1. 다음 중 하나를 수행합니다.

   * [!UICONTROL Accounts] 보기에서:

      1. 계정 이름 옆의 확인란을 선택한 다음 일괄 작업 도구 모음에서 **[!UICONTROL Upload]**&#x200B;을(를) 클릭합니다.

      1. [!UICONTROL Cloud Storage Link] 상자에서 **[!UICONTROL Go to the Link]**&#x200B;을(를) 클릭합니다.

      1. **[!UICONTROL Show Access Key and Secret]**&#x200B;을(를) 클릭합니다.

      1. [!UICONTROL Storage Link] 필드 옆에 있는 **[!UICONTROL Copy]**&#x200B;을(를) 클릭하여 클립보드에 링크를 복사하고 안전한 위치에 저장합니다.

      1. 마찬가지로 [!UICONTROL Access Key] 및 [!UICONTROL Secret Key] 값을 복사하여 안전하게 저장하십시오.

      1. **[!UICONTROL Done]**&#x200B;을(를) 클릭합니다.

   * (계정 설정에서):

      1. 다음 방법 중 하나로 계정을 선택합니다.

         * 계정 이름 위에 커서를 놓고 **..**&#x200B;을 클릭한 다음 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

         * 계정 이름 옆의 확인란을 선택한 다음 일괄 작업 도구 모음에서 **[!UICONTROL Edit]**&#x200B;을(를) 클릭합니다.

      1. **[!UICONTROL Upload File]** 탭을 클릭합니다.

      1. [!UICONTROL Cloud Storage Link] 상자에서 **[!UICONTROL Go to the Link]**&#x200B;을(를) 클릭합니다.

      1. **[!UICONTROL Show Access Key and Secret]**&#x200B;을(를) 클릭합니다.

      1. [!UICONTROL Storage Link] 필드 옆에 있는 **[!UICONTROL Copy]**&#x200B;을(를) 클릭하여 클립보드에 링크를 복사하고 안전한 위치에 저장합니다.

      1. 마찬가지로 [!UICONTROL Access Key] 및 [!UICONTROL Secret Key] 값을 복사하여 안전하게 저장하십시오.

      1. **[!UICONTROL Done]**&#x200B;을(를) 클릭합니다.

      1. **[!UICONTROL Save]**&#x200B;을(를) 클릭합니다.

1. (조직당 한 번) 로컬 AWS 환경을 설정합니다.

   1. [!DNL AWS Command Line Interface]https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html[&#x200B; 위치에서 &#x200B;](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)&#x200B;(AWS CLI)을 다운로드하여 설치하십시오.

   1. AWS 자격 증명을 구성합니다.

      1. 일반 텍스트 파일을 만들고 이름을 `~/.aws/credentials`(파일 확장명 없음)으로 지정합니다.

      1. 텍스트 편집기에서 파일을 열고 다음과 같이 조직의 액세스 키 ID와 비밀 액세스 키를 입력합니다.

         ```
         [default]
         aws_access_key_id = <Access key copied in Step 2>
         aws_secret_access_key = <Secret key copied in Step 2>
         ```

1. 광고 네트워크에서 계정 데이터 보고서를 다운로드하고 저장합니다.

1. AWS CLI에서 다음 명령을 실행하여 계정 데이터를 [!DNL S3] 클라우드 위치에 업로드합니다.

   ```
   aws s3 cp <local-report-file-location <S3-cloud-location-associated-with-your-account>
   ```

   예: `aws s3 cp filename.txt s3://cloud-location/`

## 업로드된 계정 데이터 파일 로그 보기

1. 주 메뉴에서 **[!UICONTROL Setup]** \> **[!UICONTROL Accounts]**&#x200B;을(를) 클릭합니다.

1. 계정 이름 위에 커서를 놓고 **..**&#x200B;을 클릭한 다음 **[!UICONTROL Upload Logs]**&#x200B;을(를) 클릭합니다.

1. (선택 사항) 업로드된 파일의 데이터를 다운로드하려면 ![&#x200B; 열의 &#x200B;](/help/search-social-commerce/assets/download.png "다운로드")다운로드[!UICONTROL Download]를 클릭하고 브라우저의 일반적인 절차에 따라 파일을 다운로드합니다.

## 필수 데이터

데이터는 광고 네트워크에 대한 데이터 요구 사항을 준수해야 합니다. 각 엔티티의 데이터 필드는 광고 네트워크에 따라 다를 수 있습니다.
