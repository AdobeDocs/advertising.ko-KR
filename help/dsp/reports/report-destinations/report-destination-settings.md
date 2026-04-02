---
title: 보고서 대상 설정
description: 대상 유형별로 보고서 대상에 필요한 세부 정보를 참조하십시오.
feature: DSP Custom Reports
exl-id: 1437ceea-111a-4c2e-a439-037b3a35865c
TQID: https://experienceleague.adobe.com/VB5UY9vm147LQJMKKyGOlhZdNcq6mVDYTT0Ef4RcwVs
product_v2: id: a829a185-511f-4bf8-8dcf-9e684f8011cf
feature_v2: id: ee30758d-9ffe-4cd7-8f26-0d4394f041f6
subfeature_v2: id: cc3b7f3c-58f0-4ba4-b808-391002930fd4id: e8b92199-d82f-4b20-9fc3-ffe694f93ce5
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 527ca2bb74de388c13ba1ce5bde3f8be1cead8d0
workflow-type: tm+mt
source-wordcount: 267
ht-degree: 0%

---

# 보고서 대상 설정

이메일이 아닌 보고서 대상에 필요한 세부 정보는 대상 유형에 따라 다릅니다.

>[!NOTE]
>
> 저장된 보고서 대상이 필요하지 않은 사용자 지정 보고서를 이메일 수신자에게 전달할 수도 있습니다. 보고서 설정 내에서 저장된 대상 대신 이메일 수신자를 지정할 수 있습니다.

## [!UICONTROL S3]

**[!UICONTROL Name]:** 대상을 식별하는 데 도움이 되는 이름입니다.

**[!UICONTROL S3 Bucket URL]:** 보고서가 업로드되는 [!DNL Amazon Simple Storage Service]&#x200B;(S3) 버킷의 폴더에 대한 전체 경로입니다. 예: `s3://dsp_account/reports`

**[!UICONTROL Access Key ID]:** ([!DNL Amazon S3]) 버킷에 대한 액세스 키 ID([!DNL Amazon]에서 제공)입니다.

**[!UICONTROL Secret Access Key]:** ([!DNL Amazon S3]) 버킷에 대한 비밀 액세스 키([!DNL Amazon]에서 제공)입니다.

## [!UICONTROL FTP]

**[!UICONTROL Name]:** 대상을 식별하는 데 도움이 되는 이름입니다.

**[!UICONTROL Server]:** 서버의 호스트 이름입니다.

**[!UICONTROL Port]:** 서버에서 사용할 포트 번호입니다. 기본값은 *[!UICONTROL 21]*&#x200B;입니다.

**[!UICONTROL Username]:** 서버에 로그인할 사용자 이름입니다.

**[!UICONTROL Password]:** 서버에 로그인할 암호입니다.

**[!UICONTROL Path (Optional)]:** 파일이 업로드되는 서버 경로입니다.

## [!UICONTROL SFTP]

**[!UICONTROL Name]:** 대상을 식별하는 데 도움이 되는 이름입니다.

**[!UICONTROL Server]:** 서버의 호스트 이름입니다.

**[!UICONTROL Port]:** 서버에서 사용할 포트 번호입니다. 기본값은 *[!UICONTROL 21]*&#x200B;입니다.

**[!UICONTROL Username]:** 서버에 로그인할 사용자 이름입니다.

**[!UICONTROL Password]:** 서버에 로그인할 암호입니다.

**[!UICONTROL Path (Optional)]:** 파일이 업로드되는 서버 경로입니다.

## [!UICONTROL FTP SSL]

**[!UICONTROL Name]:** 대상을 식별하는 데 도움이 되는 이름입니다.

**[!UICONTROL Server]:** 서버의 호스트 이름입니다.

**[!UICONTROL Port]:** 서버에서 사용할 포트 번호입니다. 기본값은 *[!UICONTROL 21]*&#x200B;입니다.

**[!UICONTROL Username]:** 서버에 로그인할 사용자 이름입니다.

**[!UICONTROL Password]:** 서버에 로그인할 암호입니다.

**[!UICONTROL Path (Optional)]:** 파일이 업로드되는 서버 경로입니다.

>[!MORELIKETHIS]
>
>* [보고서 대상 정보](/help/dsp/reports/report-destinations/report-destination-about.md)
>* [보고서 대상 만들기](/help/dsp/reports/report-destinations/report-destination-create.md)
>* [[!UICONTROL Report Destination]](/help/dsp/reports/report-destinations/report-destination-edit.md) 편집
>* [보고서 대상 삭제](/help/dsp/reports/report-destinations/report-destination-delete.md)
