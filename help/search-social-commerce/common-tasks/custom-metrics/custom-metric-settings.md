---
title: 사용자 지정 지표 설정
description: 표준 지표에서 계산되는 사용자 지정 지표에 대한 설정을 참조하십시오.
exl-id: b9e8434d-5ea2-47cd-9d63-705a6337c34c
feature: Search Common Tasks, Search Custom Metrics
source-git-commit: e16bc62127a708de8f4deb1eddfa53a14405cbc2
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 0%

---

# 사용자 지정 지표 설정

사용자 지정 지표 설정은 인터페이스의 여러 부분에서 약간 다릅니다.

## 캠페인 관리 보기의 사용자 지정 지표 설정

| 매개변수/섹션 | 설명 |
|----|----|
| 사용자 지정 지표 이름 | 열 이름으로 표시되는 지표의 이름입니다. <b>팁:</b> 의미 있는 지표 이름을 사용하되, 이름이 길면 열이 더 넓어집니다. |
| 지표 삽입 | 새 지표(예: [비용]/[등록])를 계산하는 데 사용되는 수학 공식:<ul><li>트래픽 및 매출 지표 목록에서 지표를 삽입하려면 지표를 삽입할 위치에 커서를 놓은 다음 목록에서 지표를 선택하거나 수동으로 대괄호로 묶어 입력합니다(예: `[CPC]`).</li><li>연산자를 삽입하려면 연산자를 삽입할 위치에 커서를 놓은 다음 버튼을 클릭하거나 기호를 수동으로 입력합니다. 사용 가능한 수학 연산자: `+ - * / ( ) ()`</li></ul><b>참고:</b> 복잡한 사용자 지정 지표를 계산하는 데 시간이 오래 걸리고, 이 지표가 포함된 보고서와 보기 횟수(특히 클릭스루 및 뷰스루 전환을 위한 별도의 열을 포함하는 경우)가 생성하는 데 시간이 더 오래 걸립니다. |
| 형식 | 이 지표에 대한 데이터를 제공하는 방법: *[!UICONTROL Currency]*(통화 값), *[!UICONTROL Number to 2 Decimal Points]*, *[!UICONTROL Number to 3 Decimal Points]*, *[!UICONTROL Number w/out Decimal Points]* 또는 *[!UICONTROL Percentage]*(소수점 2개가 있는 백분율).<br><br><b>주의:</b> 형식 [!UICONTROL Number w/out Decimal Points] (데이터를 정수로 표시)의 파생 지표를 만들고 가중 전환 속성 규칙([!UICONTROL Weight First Event More], [!UICONTROL Weight Last Event More] 또는 [!UICONTROL Even Distribution])을 사용하는 보기 또는 보고서에 포함하면 출력이 소수가 아닌 정수로 표시됩니다. 그 결과 합계가 정확하더라도 개별 데이터 필드가 올바르지 않을 수 있습니다. 예를 들어, 순서가 세 이벤트 간에 균등하게 나누어지면 한 개의 순서 (0.33 순서 대신)가 세 이벤트 각각에 기여됩니다. 문제를 방지하려면 지표 형식 [!UICONTROL Number to 2 Decimal Points]을(를) 사용하십시오. |

## 보고서 및 보고서 템플릿, [!UICONTROL Portfolios] 보기의 사용자 지정 지표 설정

| 매개변수/섹션 | 설명 |
|----|----|
| 사용자 지정 지표 이름 | 열 이름으로 표시되는 지표의 이름입니다. <b>팁:</b> 의미 있는 지표 이름을 사용하되, 이름이 길면 열이 더 넓어집니다. |
| 형식 | 이 지표에 대한 데이터를 제공하는 방법: *[!UICONTROL Currency]*(통화 값), *[!UICONTROL Number to 2 Decimal Points]*, *[!UICONTROL Number to 3 Decimal Points]*, *[!UICONTROL Number w/out Decimal Points]* 또는 *[!UICONTROL Percentage]*(소수점 2개가 있는 백분율).<br><br><b>주의:</b> 형식 [!UICONTROL Number w/out Decimal Points] (데이터를 정수로 표시)의 파생 지표를 만들고 가중 전환 속성 규칙([!UICONTROL Weight First Event More], [!UICONTROL Weight Last Event More] 또는 [!UICONTROL Even Distribution])을 사용하는 보기 또는 보고서에 포함하면 출력이 소수가 아닌 정수로 표시됩니다. 그 결과 합계가 정확하더라도 개별 데이터 필드가 올바르지 않을 수 있습니다. 예를 들어, 순서가 세 이벤트 간에 균등하게 나누어지면 한 개의 순서 (0.33 순서 대신)가 세 이벤트 각각에 기여됩니다. 문제를 방지하려면 지표 형식 [!UICONTROL Number to 2 Decimal Points]을(를) 사용하십시오. |
| 지표 삽입 | 공식을 생성할 수 있는 기존 지표 목록입니다.<br><br>수식 입력 필드에 지표를 삽입하려면 지표를 삽입할 위치에 커서를 놓은 다음 목록에서 지표를 선택하거나 수동으로 대괄호로 묶어서 입력합니다(예: `[CPC]`). |
| 연산자 삽입 | 사용할 수 있는 수학 연산자: `+ - x / ( )`<br><br>수식 입력 필드에 연산자를 삽입하려면 연산자를 삽입하려는 위치에 커서를 놓은 다음 단추를 클릭하거나 기호를 수동으로 입력합니다. |
| [지표에 대한 수식 입력 필드] | 하나 이상의 기존 속성 또는 표준 지표(예: `[Cost]/[Registrations]`)를 기반으로 새 지표를 계산하는 데 사용되는 수학 공식입니다. 여기에는 지표와 연산자의 조합이 포함될 수 있습니다.<br><br><b>참고:</b> 복잡한 사용자 지정 지표를 계산하는 데 시간이 오래 걸리고, 이 지표가 포함된 보고서와 보기 횟수(특히 클릭스루 및 뷰스루 전환을 위한 별도의 열을 포함하는 경우)가 생성하는 데 시간이 더 오래 걸립니다. |

>[!MORELIKETHIS]
>
>* [사용자 지정 지표 정보](custom-metric-about.md)
>* [사용자 지정 지표 만들기](custom-metric-create.md)
>* [사용자 지정 지표 편집](custom-metric-edit.md)
>* [사용자 지정 지표 삭제](custom-metric-delete.md)
