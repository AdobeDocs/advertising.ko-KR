---
title: 지원되는 일괄 시트 파일 형식
description: Bulksheets에 대한 일반 파일 요구 사항을 참조하십시오.
exl-id: f3daf036-8f0c-4c75-9c76-2734abd850ec
feature: Search Bulksheets
source-git-commit: e16bc62127a708de8f4deb1eddfa53a14405cbc2
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# 지원되는 일괄 시트 파일 형식

## 파일 형식

지원되는 광고 네트워크에 대한 일괄 시트 파일을 다음 형식 중 하나로 다운로드, 업로드 및 게시할 수 있습니다.

* CSV (쉼표로 구분된 값)
* TSV(탭으로 구분된 값)
* 쉼표 또는 탭으로 구분된 TXT(유니코드 텍스트)
* CSV 형식, TSV 형식 또는 쉼표나 탭으로 구분된 TXT 형식의 파일이 포함된 ZIP(압축)

일괄 시트를 만들거나 다운로드할 때 지정된 파일 형식으로 생성되며 모든 관련 데이터가 파일에 포함됩니다. 다음 정보를 사용하여 파일의 데이터를 편집하거나 직접 일괄 시트를 만듭니다.

## 일괄 시트의 기본 내용

일괄 시트 파일의 첫 번째 레코드(줄)에는 <i>header</i>(으)로 통칭되는 특정 열 이름 집합이 포함되어 있습니다. 헤더의 열 이름은 지정된 순서로 후속 데이터 레코드의 각 필드에 해당합니다. 헤더에 필요한 열 이름은 광고 네트워크에 따라 다릅니다.

각 후속 레코드(행)에는 헤더에서 각 열에 대한 값이 들어 있거나 값이 없는 필드가 있는 데이터가 포함됩니다.

## 최대 파일 크기

Bulksheet 파일은 최대 2.5GB(약 250만 행)일 수 있습니다.

>[!NOTE]
>
>여러 캠페인에 대한 일괄 시트를 생성하고 결합된 데이터가 500,000개가 넘는 행으로 구성된 경우, 데이터는 캠페인별로 `<bulksheet name>_1.tsv`, `<bulksheet name>_2.tsv` 등의 두 개 이상의 파일로 분할됩니다.

## 다양한 파일 유형에 대한 형식 요구 사항

탭과 쉼표로 구분된 데이터 필드의 형식은 서로 다릅니다.

### 탭으로 구분된 TSV 파일 및 TXT 파일

탭으로 구분된 TSV 파일 및 TXT 파일의 데이터 필드는 다음과 같은 형식으로 지정해야 합니다.

* 각 레코드의 필드는 탭 문자로 구분됩니다. 필드 값을 생략하려면 탭 문자만 사용하십시오.

  예: `Cruises<TAB>5000<TAB>Caribbean<TAB><TAB><TAB>`

* 필드에는 포함된 탭 문자를 사용할 수 없습니다.

### 쉼표로 구분된 CSV 파일 및 TXT 파일

쉼표로 구분된 CSV 파일 및 TXT 파일의 데이터 필드는 다음과 같은 형식으로 지정해야 합니다.

* 레코드의 필드는 쉼표로 구분됩니다. 필드 값을 생략하려면 쉼표만 사용하십시오.

  예: `Cruises,5000,Caribbean,,,`

* 선택적으로 모든 필드를 큰따옴표(`""`)로 묶을 수 있습니다.

  예: `"Cruises","5000","Caribbean",`

* 포함된 쉼표가 있는 필드는 큰따옴표(`""`)로 묶어야 합니다.

  예: `Cruises,5000,Caribbean,"Luxurious, spacious cabins",`

* 포함된 큰따옴표가 있는 필드는 큰따옴표(`""`)로 묶어야 합니다.

  예: `Cruises,5000,Caribbean,"Customers say ""We wish we could stay forever."",`

* 선행 또는 후행 공백이 있는 필드는 큰따옴표(`""`)로 묶어야 합니다.

  예: `Cruises,5000,Caribbean,"  Come see what we mean.  ",`

>[!MORELIKETHIS]
>
>* [일괄 시트를 사용하여 캠페인 데이터 관리 정보](../bulksheet-about.md)
>* [일괄 시트에서 수행할 수 있는 작업](bulksheet-operations.md)
>* [부록 - 일괄 시트 오류](../bulksheet-errors.md)
>* [일괄 시트 파일 다운로드/만들기](../bulksheet-download.md)
