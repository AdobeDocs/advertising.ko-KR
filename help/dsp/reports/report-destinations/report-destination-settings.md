---
title: 보고서 대상 설정
description: 대상 유형별로 보고서 대상에 필요한 세부 정보를 참조하십시오.
feature: DSP Custom Reports
exl-id: 1437ceea-111a-4c2e-a439-037b3a35865c
source-git-commit: 4b9cc5956d573b346eacdf71a8ea490c162b4660
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# 보고서 대상 설정

이메일이 아닌 보고서 대상에 필요한 세부 정보는 대상 유형에 따라 다릅니다.

>[!NOTE]
>
> 저장된 보고서 대상이 필요하지 않은 사용자 지정 보고서를 이메일 수신자에게 전달할 수도 있습니다. 보고서 설정 내에서 저장된 대상 대신 이메일 수신자를 지정할 수 있습니다.

## [!UICONTROL S3]

**[!UICONTROL Name]:** 대상을 식별하는 데 도움이 되는 이름입니다.

**[!UICONTROL S3 Bucket URL]:** 폴더의 전체 경로 [!DNL Amazon Simple Storage Service] (S3) 보고서가 업로드되는 버킷입니다. 예: `s3://dsp_account/reports`

**[!UICONTROL Access Key ID]:** ( )에 대한 액세스 키 ID[!DNL Amazon S3]) 버킷(제공자 [!DNL Amazon]).

**[!UICONTROL Secret Access Key]:** ( )에 대한 비밀 액세스 키[!DNL Amazon S3]) 버킷(제공자 [!DNL Amazon]).

## [!UICONTROL FTP]

**[!UICONTROL Name]:** 대상을 식별하는 데 도움이 되는 이름입니다.

**[!UICONTROL Server]:** 서버의 호스트 이름입니다.

**[!UICONTROL Port]:** 서버에서 사용할 포트 번호입니다. 기본값은 입니다 *[!UICONTROL 21]*.

**[!UICONTROL Username]:** 서버에 로그인할 사용자 이름입니다.

**[!UICONTROL Password]:** 서버에 로그인할 암호입니다.

**[!UICONTROL Path (Optional)]:** 파일이 업로드되는 서버 경로입니다.

## [!UICONTROL SFTP]

**[!UICONTROL Name]:** 대상을 식별하는 데 도움이 되는 이름입니다.

**[!UICONTROL Server]:** 서버의 호스트 이름입니다.

**[!UICONTROL Port]:** 서버에서 사용할 포트 번호입니다. 기본값은 입니다 *[!UICONTROL 21]*.

**[!UICONTROL Username]:** 서버에 로그인할 사용자 이름입니다.

**[!UICONTROL Password]:** 서버에 로그인할 암호입니다.

**[!UICONTROL Path (Optional)]:** 파일이 업로드되는 서버 경로입니다.

## [!UICONTROL FTP SSL]

**[!UICONTROL Name]:** 대상을 식별하는 데 도움이 되는 이름입니다.

**[!UICONTROL Server]:** 서버의 호스트 이름입니다.

**[!UICONTROL Port]:** 서버에서 사용할 포트 번호입니다. 기본값은 입니다 *[!UICONTROL 21]*.

**[!UICONTROL Username]:** 서버에 로그인할 사용자 이름입니다.

**[!UICONTROL Password]:** 서버에 로그인할 암호입니다.

**[!UICONTROL Path (Optional)]:** 파일이 업로드되는 서버 경로입니다.

>[!MORELIKETHIS]
>
>* [정보 [!UICONTROL Report Destinations]](/help/dsp/reports/report-destinations/report-destination-about.md)
>* [만들기 [!UICONTROL Report Destination]](/help/dsp/reports/report-destinations/report-destination-create.md)
>* [편집 [!UICONTROL Report Destination]](/help/dsp/reports/report-destinations/report-destination-edit.md)
>* [삭제 [!UICONTROL Report Destination]](/help/dsp/reports/report-destinations/report-destination-delete.md)
