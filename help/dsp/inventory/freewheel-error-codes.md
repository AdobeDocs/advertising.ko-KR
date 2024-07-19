---
title: ' [!DNL FreeWheel] 광고 제출 오류 코드'
description: 광고 제출을 위해  [!DNL FreeWheel]에 반환되는 오류 코드를 참조합니다.
feature: DSP Private Inventory, DSP Deal IDs
exl-id: e48937c2-ced9-4107-9e1d-65a3bac51fff
source-git-commit: 14f78b89dea8cc680756232c6116975c652feee5
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 3%

---

# [!DNL FreeWheel] 광고 제출에 대한 오류 코드

실패한 광고 제출에 대한 오류 메시지는 Advertising DSP 또는 [!DNL FreeWheel]에서 가져올 수 있습니다. 오류 메시지가 [[!UICONTROL Freewheel Status] 대화 상자](freewheel-check-status.md)의 [!UICONTROL API Response] 열에 표시됩니다.

## Advertising DSP 내부 오류

| 오류 메시지 | 설명 | 다음 단계 |
|--- |--- |--- |
| [!DNL Awaiting status response from [!DNL FreeWheel]] | [!DNL FreeWheel]이(가) 제출 성공 또는 실패에 대해 아직 응답하지 않았습니다. | 10분 후에 상태를 다시 확인하십시오. |
| [!DNL The submitted ad does not have a clock number assigned.] | [!DNL FreeWheel]은(는) 할당된 시계 번호가 없는 영국 광고를 수락하지 않습니다. | 광고에 시계 번호를 할당한 다음 광고를 다시 제출합니다. |
| [!DNL The ad you are attempting to submit has not yet finished transcoding. Please wait ten minutes then try again.] | 광고를 제출하려고 할 때 트랜스코더가 광고 트랜스코딩을 완료하지 않았습니다. | 10분 정도 기다린 후 광고를 다시 제출합니다. |
| [!DNL The deal id you input is not setup as a guaranteed feed. Please submit guaranteed deals only.] | 제출된 거래는 프로그램 보증 거래로 설정되지 않습니다. [!DNL FreeWheel]은(는) 보장된 거래만 수락합니다. | 거래 ID를 프로그램 보증 거래로 설정합니다. 거래 ID 워크플로의 끝에 프로그래밍 방식으로 보장된 기본 배치를 저장하면 광고가 [!DNL FreeWheel]에 자동으로 제출됩니다. |
| [!DNL Invalid external_deal_id:] \&lt;deal_id\> | 제출된 거래 ID가 존재하지 않거나 Adobe 끝에서 활성화되지 않습니다. | 거래가 활성 상태인지 확인한 다음 광고를 다시 제출합니다. |
| [!DNL \[public_id=]\&lt;deal\>]이(가) 없습니다. | 제출된 거래 ID가 [!DNL FreeWheel] 끝에 없습니다. | 거래 ID를 확인하려면 [!DNL FreeWheel] 담당자에게 문의하세요. |
| [!DNL Ad with identifier] \&lt;*광고 이름*\> [!DNL was not found.] | 제출된 광고 키가 존재하지 않거나 Adobe 끝에서 활성화되지 않습니다. | 올바른 광고 키를 찾은 다음 광고를 다시 제출합니다. |
| [!DNL Pending Submission] | 제출이 아직 보류 중입니다. | 페이지를 새로 고칩니다. |

{style="table-layout:auto"}

## [!DNL Freewheel] API 오류

| 코드 | 의미 | 설명 | 다음 단계 |
|--- |--- |--- |--- |
| 401 | 승인되지 않음 | 액세스 자격 증명이 잘못되었거나, 누락되었거나, 잘못되었습니다. | Adobe 계정 팀에 문의하십시오. |
| 403 | 금지됨 | 서버는 요청을 이해했지만 승인을 거부합니다. | Adobe 계정 팀에 문의하십시오. |
| 404 | 찾을 수 없음 | 요청한 리소스를 사용할 수 없습니다. 크리에이티브 ID가 PUT 작업에서 발견되지 않는 경우, 404가 반환됩니다. | Adobe 계정 팀에 문의하십시오. |
| 405 | 메서드가 허용되지 않음 | 해당 리소스에서 지원하지 않는 요청 메서드를 사용하는 리소스에 대해 요청이 이루어졌습니다(예: POST에서 데이터를 보내야 하는 메서드에서 GET 사용 또는 읽기 전용 리소스에서 PUT 사용). | Adobe 계정 팀에 문의하십시오. |
| 408 | 요청 시간 초과 | 이 요청을 처리하는 동안 시간 초과가 발생했습니다. 일반적으로 시간 초과는 특정 리소스에 대한 독점적 액세스 권한을 동시에 요청하여 발생합니다. | 이 상태를 받으면 요청을 다시 제출합니다. 문제가 지속되면 Adobe 계정 팀에 문의하십시오. |
| 422 | 처리할 수 없는 엔티티 | 잘못된 리소스. 이 오류는 요청 본문이 잘못되었거나 생성/업데이트된 리소스가 유효하지 않은 경우(예: 거래 ID를 찾을 수 없는 경우)에 발생합니다. 자세한 내용은 [FreeWheel API 422 오류](#freewheel-422-errors)를 참조하십시오. | Adobe 계정 팀에 문의하십시오. |
| 500 | 내부 서버 오류 | API 시스템 오류. | Adobe 계정 팀에 문의하십시오. |

{style="table-layout:auto"}

## [!DNL Freewheel] API 422 오류 {#freewheel-422-errors}

| 코드 | HTTP 코드 | 설명 |
|--- |--- |--- |
| DATA_UNMARSHALL_FAILURE | 422 | 요청 데이터가 잘못된 json 형식입니다. 자세한 내용은 오류 메시지를 확인하십시오. |
| DATA_VALIDATION_FAILURE | 422 | 요청 데이터에 필수 필드가 누락되었거나 데이터 형식이 잘못되었습니다. 자세한 내용은 오류 메시지를 확인하십시오. |
| DATA_DEAL_INVALID | 422 | 거래가 잘못 구성되거나 존재하지 않습니다. 자세한 내용은 오류 메시지를 확인하십시오. |
| DATA_DEAL_FAILURE GET | 422 | 거래를 찾을 수 없거나 구성에 문제가 있습니다. 자세한 내용은 오류 메시지를 확인하십시오. |
| DATA_CREATIVE_INGEST_FAILURE | 422 | 광고 URL이 잘못되었습니다. 자세한 내용은 오류 메시지를 확인하십시오. |
| DATA_CREATIVE_LINK_FAILURE | 422 | 크리에이티브가 거래의 광고 단위 노드에 연결되지 않았습니다. 자세한 내용은 오류 메시지를 확인하십시오. |
| DATA_CREATIVE_UPDATE_FAILURE | 422 | 크리에이티브가 업데이트되지 않았습니다. 자세한 내용은 오류 메시지를 확인하십시오. |
| DATA_DSP GET_FAILURE | 422 | DSP이 시스템 내에 존재하지 않습니다. |
| DATA_CREATIVE_UNLINK_FAILURE | 422 | 광고 단위에서 크리에이티브의 연결이 해제되지 않았습니다. |
| DATA_CREATIVE_DATA_FAILURE DELETE | 422 | 크리에이티브가 삭제되지 않았습니다. |
| DATA_CREATIVE_DETECTION_FAILURE | 422 | URL이 검색되지 않았습니다. |
| DATA_ENTITY_NOT_FOUND | 422 | 창조물은 존재하지 않습니다. |

{style="table-layout:auto"}

>[!MORELIKETHIS]
>
>* [프로그램 보증 거래 설정 개요 [!DNL Freewheel]](/help/dsp/inventory/freewheel-overview.md)
>* [거래 ID 받은 편지함에서 거래 수락](deal-id-inbox-accept.md)
>* [프로그램 보증 거래에 대한 광고 제출 [!DNL Freewheel]](/help/dsp/inventory/freewheel-submit.md)
>* [광고 상태 확인 [!DNL FreeWheel] 프로그램 보증 거래](/help/dsp/inventory/freewheel-check-status.md)
