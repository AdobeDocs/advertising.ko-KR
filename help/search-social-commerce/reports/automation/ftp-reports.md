---
title: 보고서에 대한 FTP 액세스
description: 읽기 전용 FTP 위치에서 보고서를 받는 방법을 알아봅니다.
exl-id: eca9f033-5b1b-4afa-926b-b4c31e2dede3
feature: Search Reports
source-git-commit: e517dd5f5fa283ff8a2f57728612937148889732
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

# 보고서에 대한 FTP 액세스

필요한 경우 읽기 전용 FTP 위치에서 보고서를 받을 수 있으며, 이 위치에서 추가적인 자동화된 프로세스(예: 다른 프로그램으로 데이터를 구문 분석하기 위해)에 대해 파일을 검색할 수 있습니다. 을 제외한 모든 기본 보고서 [!UICONTROL Search Engine Account Report] 또한 모든 고급 보고서는 압축 TSV 파일(기본값) 또는 .ZIP 파일 확장자가 있는 CSV 파일로 FTP 위치에 배달될 수 있습니다. 모든 TSV 또는 CSV 파일 헤더가 포함되며 숨길 수 없습니다.

보고서에 대한 FTP 액세스는 지정된 FTP 계정에 대한 액세스 권한이 필요하며, 특정 이름 지정 규칙 및 일정을 사용하여 보고서 템플릿을 설정해야 합니다.

## 보고서에 액세스하기 위한 FTP 계정 설정

* 보고서 액세스를 위한 FTP 계정을 설정하려면 Adobe 계정 팀에 문의하십시오.

  팀에서 사용자 이름과 암호를 제공합니다.

## FTP 게재용 보고서 템플릿 설정

지정된 FTP 디렉터리에 보고서를 생성하려면 [보고서 템플릿](templates/template-create.md) (다음 이름 지정 규칙 및 일정 사용)

>[!NOTE]
>
>다음을 제외한 모든 고급 보고서 및 모든 기본 보고서 [!UICONTROL Search Engine Account Report] 는 FTP 위치에 게재할 수 있습니다.

1. 보고서 템플릿의 템플릿 이름에 다음 정보를 포함하십시오.

   * `FTP` (대문자로 표시).

   * (선택 사항) 대괄호를 포함하여 다음 대소문자를 구분하는 구문을 사용하는 세 가지 시스템 날짜 중 하나입니다.

      * `[TODAY]` — 보고서가 실행된 날짜, 시간 및 분을 포함합니다. 여기에는 정확한 시간이 포함되므로 이전 보고서를 덮어쓰지 않고 동일한 템플릿을 하루에 여러 번 실행할 수 있습니다.

      * `[SDATE]` — 보고서 날짜 범위의 시작 날짜를 포함합니다.

      * `[EDATE]` — 보고서 날짜 범위의 종료 날짜를 포함합니다.

   * (선택 사항) `[CSV]` 기본 TSV 형식이 아닌 CSV 형식으로 파일을 만들 수 있도록(대괄호로 묶인 대문자).

   예: `[TODAY]-Portfolio-FTP-[SDATE]-[EDATE]-[CSV]` 는 202305051656-Portfolio-FTP-20230428-20110504.csv와 같은 파일을 만듭니다.

1. 보고서가 특정 시간에 실행되도록 예약합니다.

   보고서는 완료 후 1시간 이내에 FTP 계정으로 배달됩니다.

>[!NOTE]
>
>* 완료된 보고서를 전자 메일로 보내려면 보고서나 템플릿을 생성할 때 모든 전자 메일 수신자의 주소를 입력하면 됩니다.
>* 보고서는 지정된 일정에 따라 실행되며 완료된 후 1시간 이내에 FTP 계정으로 배달됩니다.

## FTP 저장소의 보고서에 액세스

보고서에 액세스하려면 FTP 계정에 대한 로그인( )을 사용하여 다음 FTP 호스트 중 하나에 연결합니다.`amo<userID>rpt`, (예: amo1234rpt) 및 암호 또는 개인 연결 키(설정된 경우) 중 하나:

* 해외 고객: `ftp3.adobe.net`
* 미국 고객: `ftp5.adobe.net`

>[!NOTE]
>
>보고서 저장소는 읽기 전용이며 15일마다 삭제됩니다.


>[!MORELIKETHIS]
>
>* [보고서 템플릿 만들기](/help/search-social-commerce/reports/automation/templates/template-create.md)
