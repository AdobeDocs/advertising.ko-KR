---
title: 연결된 TV 도달 계획에 대한 설정
description: 연결된 TV 도달 계획에 대한 설정 설명을 참조하십시오.
feature: DSP Planner
exl-id: 65edd6f5-557c-44d1-a0ed-8cd26d8a2f6e
source-git-commit: 84cf49c9e366938479e9fea2ede55925f1cb3e51
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 0%

---

# 연결된 TV 도달 계획에 대한 설정

| 매개 변수 | 설명 | 필수? |
| --- | --- | --- |
| [!UICONTROL Name] | 플랜을 식별하는 이름입니다. | 예 |
| [!UICONTROL Advertiser] | 플랜이 생성되는 계정의 특정 광고주입니다. | 예 |
| [!UICONTROL Media Type] | 플랜에 포함할 미디어 유형입니다.<br><br>현재 [!UICONTROL Connected TV]만 사용할 수 있습니다. | 예 |
| [!UICONTROL Date Range] | 플랜의 시작 및 종료 일자.<br><br>시작 날짜는 현재 날짜보다 이전일 수 없습니다. 날짜 범위는 90일을 초과할 수 없습니다. | 예 |
| [!UICONTROL Goal Type] | 플랜에 대해 고려할 목표의 유형(예: [!UICONTROL Budget]).<br><br>현재 [!UICONTROL Budget]만 사용할 수 있습니다. | 예 |
| [!UICONTROL Goal Value] | 예측에 대한 목표 값. 보다 정확한 예측 결과를 얻으려면 5000 USD보다 큰 값을 사용하십시오. | 예 |
| [!UICONTROL Max Bid] | 1000회 노출에 대해 지불할 최대 금액입니다. [!UICONTROL Connected TV] 미디어 유형을 선택한 경우 최소 10USD 이상의 값을 입력하십시오. | 예 |
| [!UICONTROL Frequency Cap] | 고유 가구에 대한 광고가 게재되는 횟수.<br><br>계획을 구현하고 여러 배치를 만들어야 하는 경우 올바른 전달을 위해 배치 수준이 아닌 패키지 수준에서 빈도 상한 설정을 적용합니다. | 예 |
| [!UICONTROL Geo-Targeting] | 대상으로 포함하거나 제외할 위치입니다. 옵션은 다음과 같습니다.<ul><li>국가, 도시, 주: **[!UICONTROL Country/State/City]** 탭을 클릭하고 영역이 *국가*, *주* 또는 *도시*&#x200B;인지 선택합니다. 필요한 경우 위치를 확장하여 하위 구성 요소를 확인한 다음 위치 옆에 있는 **[!UICONTROL Include]** 또는 **[!UICONTROL Exclude]**&#x200B;을(를) 클릭합니다.</li><li>미국에 있는 DMA(지정된 마켓 영역): **[!UICONTROL DMA]** 탭을 클릭합니다. 선택적으로 모든 상태를 확장하여 해당 DMA를 본 다음 위치 옆에 있는 **[!UICONTROL Include]** 또는 **[!UICONTROL Exclude]**&#x200B;을(를) 클릭합니다.</li><li>우편 번호: 다음 중 하나를 수행할 수 있습니다.<ul><li>**[!UICONTROL Search postal code]** 탭을 클릭하고 국가를 선택하고 도시 이름에 포함된 전체 도시 이름을 입력한 다음 **[Enter]** 키를 누르고 올바른 도시 이름을 클릭하여 도시에 대한 모든 우편 번호를 보고 올바른 우편 번호를 클릭한 다음 **[!UICONTROL Include]** 또는 **[!UICONTROL Exclude]**&#x200B;을(를) 클릭합니다.</li><li>**[!UICONTROL Paste postal code]** 탭을 클릭하고 국가를 선택하고 쉼표로 구분된 값을 입력하거나 붙여 넣은 다음 **[!UICONTROL Include All]** 또는 **[!UICONTROL Exclude All]**&#x200B;을(를) 클릭합니다.</li></ul></li></ul> | 예 |
| [!UICONTROL Inventory Targeting] | 대상으로 포함하거나 제외할 인벤토리 소스입니다. 피드 또는 소스를 하나 이상 선택하십시오. | 예 |
| [!UICONTROL Site/App Targeting] | 타겟으로 포함하거나 제외할 웹 사이트 및 앱입니다. 한 줄에 하나의 URL을 입력한 다음 **[!UICONTROL Include All]** 또는 **[!UICONTROL Exclude All]**&#x200B;을(를) 클릭합니다. | 아니요 |
| [!UICONTROL Audience Targeting] | 타겟으로 포함하거나 제외할 대상입니다. | 아니요 |
| [!UICONTROL Ad duration] | 플랜에 대해 고려할 광고의 기간입니다. | 아니요 |

>[!MORELIKETHIS]
>
>* [DSP Planner 도구 정보](planner-about.md)
>* [연결된 TV 도달 계획 만들기](planner-create.md)
>* [연결된 TV 도달 계획 복제](planner-duplicate.md)
>* [연결된 TV 도달 계획 편집](planner-edit.md)
>* [연결된 TV 도달 계획 내보내기](planner-export.md)
>* [연결된 TV 도달 계획에 대한 예측 다시 생성](planner-forecast.md)
>* [연결된 TV 도달 계획 보관](planner-archive.md)
